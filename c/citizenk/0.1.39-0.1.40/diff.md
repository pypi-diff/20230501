# Comparing `tmp/citizenk-0.1.39.tar.gz` & `tmp/citizenk-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.39.tar", max compression
+gzip compressed data, was "citizenk-0.1.40.tar", max compression
```

## Comparing `citizenk-0.1.39.tar` & `citizenk-0.1.40.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.39/citizenk/__init__.py
--rw-r--r--   0        0        0     3885 2023-04-29 16:34:03.427065 citizenk-0.1.39/citizenk/agent.py
--rw-r--r--   0        0        0    20872 2023-04-30 11:32:53.917080 citizenk-0.1.39/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.39/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.39/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.39/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.39/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-30 11:33:42.913446 citizenk-0.1.39/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-30 11:33:53.924372 citizenk-0.1.39/setup.py
--rw-r--r--   0        0        0     1076 2023-04-30 11:33:53.924628 citizenk-0.1.39/PKG-INFO
+-rw-r--r--   0        0        0      364 2023-05-01 08:02:00.667857 citizenk-0.1.40/citizenk/__init__.py
+-rw-r--r--   0        0        0     8057 2023-05-01 09:22:53.462103 citizenk-0.1.40/citizenk/agent.py
+-rw-r--r--   0        0        0    20667 2023-05-01 09:24:22.181659 citizenk-0.1.40/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.40/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.40/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.40/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.40/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-05-01 09:25:30.357973 citizenk-0.1.40/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-05-01 09:25:36.217545 citizenk-0.1.40/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-01 09:25:36.217821 citizenk-0.1.40/PKG-INFO
```

### Comparing `citizenk-0.1.39/citizenk/citizenk.py` & `citizenk-0.1.40/citizenk/citizenk.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from enum import Enum
 from functools import wraps
 from inspect import signature
 from typing import Callable, List, Optional, Union
 
 import httpx
 from confluent_kafka import KafkaException
-from confluent_kafka import Message as ConfluentMessage
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse
-from pydantic import BaseModel, ValidationError
+from pydantic import BaseModel
 
-from .agent import Agent, KafkaEvent
+from .agent import Agent, WebSocketAgent
 from .kafka_adapter import KafkaAdapter, KafkaConfig, KafkaRole
 from .topic import Topic, TopicDir
 from .utils import CitizenKError
 
 logger = logging.getLogger(__name__)
 
 
@@ -41,15 +40,15 @@
         app_type: AppType = AppType.SOURCE,
         consumer_group_init_offset: str = "latest",
         schema_registry_url: Optional[str] = None,
         auto_generate_apis: bool = True,
         max_processing_cycle_ms: int = 5 * 1000,
         api_router_prefix: str = "",
         api_port: Optional[int] = None,
-        consumer_in_thred: bool = False,
+        agents_in_thread: bool = False,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.app_name = app_name
         self.app_type = app_type
         self.kafka_config = kafka_config
@@ -63,15 +62,16 @@
         self.consumer = None
         self._started = datetime.utcnow()
 
         self.total_batch_size = 0
         self.consumer_topics = set()
         self.topics = {}
         self.agents = {}
-        self.consumer_in_thred = consumer_in_thred
+        self.websocket_agents = {}
+        self.agents_in_thread = agents_in_thread
         self.background_loop = None
         self.background_thread = None
         self.main_consumer_loop_task = None
         self.monitor_loop_task = None
 
         self.add_event_handler("startup", self.startup)
         self.add_event_handler("shutdown", self.shutdown)
@@ -127,14 +127,15 @@
                         for t in self.topics.values()
                         if t.topic_dir != TopicDir.INPUT
                     ],
                 },
                 "lag": lag,
                 "assignments": assignments,
                 "agents": [a.info() for a in self.agents.values()],
+                "websocket_agents": [a.info() for a in self.websocket_agents.values()],
                 "hosts": {f"{tp[0]}-{tp[1]}": h for tp, h in hosts.items()},
             }
 
     def is_sink(self) -> bool:
         return self.app_type == AppType.SINK
 
     def fast_status(self) -> bool:
@@ -194,48 +195,47 @@
         """CitizenK startup. Called on FastAPI startup"""
         logger.debug("CitizenK starting up...")
 
         # Find all consumer topics
         for agent in self.agents.values():
             self.consumer_topics.update({t.name for t in agent.topics})
             self.total_batch_size += agent.batch_size
-            for t in agent.topics:
-                if t.topic_dir == TopicDir.OUTPUT:
-                    raise CitizenKError("Trying to consume from an output topic")
 
         # Create consumer
         if len(self.consumer_topics) > 0:
             if self.app_type == AppType.SOURCE:
                 raise CitizenKError("Trying to consume topics in a source app")
             self.consumer = KafkaAdapter(
                 self.kafka_config,
                 KafkaRole.CONSUMER,
                 self.app_name,
                 self.consumer_group_init_offset,
             )
+            self.consumer.start_consumer(list(self.consumer_topics))
 
         # Create producer
         if self.app_type in [AppType.SOURCE, AppType.TRANSFORM]:
             self.producer = KafkaAdapter(self.kafka_config, KafkaRole.PRODUCER)
 
-        # Check that all topic exists in broker
+        # Check that all topics exist in broker
         broker = self.producer if self.consumer is None else self.consumer
         broker_topics = broker.get_all_broker_topics()
         for topic_name, topic in self.topics.items():
             if topic_name not in broker_topics:
                 raise CitizenKError(f"Can't find topic {topic_name} in broker")
             # Set num partitions and replicas in topic
             topic.partition_count = len(broker_topics[topic_name].partitions)
             topic.replica_count = len(broker_topics[topic_name].partitions[0].replicas)
 
-        # Start consumer
-        if len(self.consumer_topics) > 0:
-            self.consumer.start_consumer(list(self.consumer_topics))
+        # Start Main consumer loop if there is any consumer
+        # Normal consumer (with group)
+        # Websocket consumers (no group)
+        if self.consumer is not None or len(self.websocket_agents) > 0:
 
-            if self.consumer_in_thred:
+            if self.agents_in_thread:
                 # Start in thread
                 self.background_loop = asyncio.new_event_loop()
                 self.background_thread = threading.Thread(
                     target=self.background_consumer_thread, args=(self.background_loop,)
                 )
                 self.background_thread.start()
                 self.main_consumer_loop_task = asyncio.run_coroutine_threadsafe(
@@ -253,50 +253,21 @@
         logger.debug("CitizenK shutting down...")
         if self.consumer is not None:
             self.consumer.close()
             self.consumer = None
         if self.producer is not None:
             self.producer.close()
             self.producer = None
+        for agent in self.websocket_agents.values():
+            agent.close()
         if self.main_consumer_loop_task is not None:
             self.main_consumer_loop_task.cancel()
         if self.background_loop is not None:
             self.background_loop.stop()
 
-    def validate_messages(self, msgs: List[ConfluentMessage]) -> List[KafkaEvent]:
-        """Validate the incoming Kafka messages"""
-        events = []
-        for msg in msgs:
-            topic_name = msg.topic()
-            if topic_name not in self.consumer_topics:
-                raise CitizenKError(
-                    "Weird, got a message from an unexpected topic", topic_name
-                )
-            topic = self.topics[topic_name]
-            try:
-                value = topic.value_type(**json.loads(msg.value()))
-            except json.decoder.JSONDecodeError as e:
-                logger.error("For now, CitizenK only supports JSON values %s", e)
-                continue
-            except ValidationError as e:
-                logger.error("Error while validating received value %s", e.json())
-                continue
-
-            events.append(
-                KafkaEvent(
-                    key=msg.key(),
-                    value=value,
-                    topic=topic,
-                    partition=msg.partition(),
-                    offset=msg.offset(),
-                    timestamp=msg.timestamp()[1],
-                    headers=msg.headers(),
-                )
-            )
-        return events
 
     def background_consumer_thread(self, loop: asyncio.BaseEventLoop):
         logger.debug("CitizenK background consumer thread started...")
         asyncio.set_event_loop(loop)
         try:
             loop.run_forever()
         except asyncio.CancelledError as e:
@@ -321,44 +292,63 @@
                 await asyncio.sleep(60)
                 os.kill(os.getpid(), signal.SIGKILL)
 
     async def _main_consumer_loop(self):
         """Main Kafka consumer loop which invokes the process agents"""
         logger.debug("CitizenK main processing loop started...")
         while True:
-            if self.consumer is None:
+            # Check if consumer was deleted
+            if self.consumer is None and len(self.consumer_topics) > 0:
                 break
+            
+            duration = 0
+            processed = False
             try:
-                msgs = self.consumer.consume(
-                    num_messages=self.total_batch_size, timeout=0.1
-                )
-                if len(msgs) == 0:
-                    logger.debug("No kafka events, sleeping")
-                    await asyncio.sleep(1)
-                else:
-                    start_time = time.time()
+                if self.consumer is not None:
+                    msgs = self.consumer.consume(
+                        num_messages=self.total_batch_size, timeout=0.1
+                    )
+                    if len(msgs) > 0:
+                        processed = True
+                        start_time = time.time()
+                        events = Agent.validate_messages(msgs, self.topics)
+                        for agent in self.agents.values():
+                            await agent.process(events)
+                        duration = 1000 * (time.time() - start_time)
+
+                # Consume from websocket agents consumers (no group)
+                start_time = time.time()
+                for agent in self.websocket_agents.values():
+                    if agent.consume():
+                        processed = True
+                duration += 1000 * (time.time() - start_time)
+
+                # Poll producer
+                if self.producer is not None:
+                    self.producer.poll()
+
+                if duration > self.max_processing_cycle_ms:
+                    logger.error(
+                        "Processing cycle took %s ms > %s",
+                        duration,
+                        self.max_processing_cycle_ms,
+                    )
 
-                    events = self.validate_messages(msgs)
-                    for agent in self.agents.values():
-                        await agent.process(events)
-
-                    duration = 1000 * (time.time() - start_time)
-                    if duration > self.max_processing_cycle_ms:
-                        logger.error(
-                            "Processing cycle took %s ms > %s",
-                            duration,
-                            self.max_processing_cycle_ms,
-                        )
+                if processed:
                     # Just to give other tasks opportunity to run
                     await asyncio.sleep(0)
-                if self.app_type == AppType.TRANSFORM:
-                    self.producer.poll()
+                else:
+                    # Wait a bit until messages arrive
+                    logger.debug("No kafka events, sleeping")
+                    await asyncio.sleep(1)
+
             except Exception as e:
                 logger.exception("Exception in main loop: %s", str(e))
                 await asyncio.sleep(3)
+            
 
     def topic(
         self,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
         subject_name: Optional[str] = None,
@@ -405,17 +395,23 @@
             agent_name = f.__name__
             if "values" in signature(f).parameters:
                 return_type = "values"
             elif "events" in signature(f).parameters:
                 return_type = "events"
             else:
                 raise CitizenKError("Agents can only accept values and events")
-            self.agents[agent_name] = Agent(
-                self, agent_name, f, topics, batch_size, return_type, websocket_route
-            )
+            if websocket_route is None:
+                self.agents[agent_name] = Agent(
+                    self, agent_name, f, topics, batch_size, return_type
+                )
+            else:
+                self.websocket_agents[agent_name] = WebSocketAgent(
+                    self, agent_name, f, topics, batch_size, return_type, websocket_route
+                )
+
             logger.debug("Adding agent %s %s", agent_name, topics)
             return wrapper
 
         return decorator
 
     def topic_router(self, topic: Topic, match_info: str) -> Callable:
         """
```

### Comparing `citizenk-0.1.39/citizenk/kafka_adapter.py` & `citizenk-0.1.40/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.39/citizenk/murmur2.py` & `citizenk-0.1.40/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.39/citizenk/topic.py` & `citizenk-0.1.40/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.39/pyproject.toml` & `citizenk-0.1.40/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.39"
+version = "0.1.40"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.39/setup.py` & `citizenk-0.1.40/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.39',
+    'version': '0.1.40',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.39/PKG-INFO` & `citizenk-0.1.40/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.39
+Version: 0.1.40
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

