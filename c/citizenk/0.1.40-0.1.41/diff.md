# Comparing `tmp/citizenk-0.1.40.tar.gz` & `tmp/citizenk-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.40.tar", max compression
+gzip compressed data, was "citizenk-0.1.41.tar", max compression
```

## Comparing `citizenk-0.1.40.tar` & `citizenk-0.1.41.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      364 2023-05-01 08:02:00.667857 citizenk-0.1.40/citizenk/__init__.py
--rw-r--r--   0        0        0     8057 2023-05-01 09:22:53.462103 citizenk-0.1.40/citizenk/agent.py
--rw-r--r--   0        0        0    20667 2023-05-01 09:24:22.181659 citizenk-0.1.40/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.40/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.40/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.40/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.40/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-05-01 09:25:30.357973 citizenk-0.1.40/pyproject.toml
--rw-r--r--   0        0        0      863 2023-05-01 09:25:36.217545 citizenk-0.1.40/setup.py
--rw-r--r--   0        0        0     1076 2023-05-01 09:25:36.217821 citizenk-0.1.40/PKG-INFO
+-rw-r--r--   0        0        0      382 2023-05-01 09:49:27.845822 citizenk-0.1.41/citizenk/__init__.py
+-rw-r--r--   0        0        0     8281 2023-05-01 09:39:19.585970 citizenk-0.1.41/citizenk/agent.py
+-rw-r--r--   0        0        0    20616 2023-05-01 09:33:15.425455 citizenk-0.1.41/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.41/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.41/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.41/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.41/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-05-01 09:49:41.218689 citizenk-0.1.41/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-05-01 09:49:47.789543 citizenk-0.1.41/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-01 09:49:47.789801 citizenk-0.1.41/PKG-INFO
```

### Comparing `citizenk-0.1.40/citizenk/agent.py` & `citizenk-0.1.41/citizenk/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             async def endpoint(values: int):
                 result = await self.coroutine(values=values)
                 return result
 
             annotate_function(
                 endpoint,
                 name=f"send_to_agent_{self.name}_from_{topic.name}",
-                doc=f"This endpoint send value to agent {self.name} from topic {topic.name}",
+                doc=f"This endpoint sends value to agent {self.name} from topic {topic.name}",
                 argument_types={"values": List[topic.value_type]},
             )
 
             self.app.add_api_route(
                 path=f"{self.app.api_router_prefix}/agent/{self.name}/{topic.name}",
                 response_class=JSONResponse,
                 methods=["POST"],
@@ -175,17 +175,20 @@
             "name": self.name,
             "cycles": self.cycles,
             "connections": len(self.active_websocket_connections)
         }
 
     def _handle_consumer(self):
         if len(self.active_websocket_connections) > 0 and self.consumer is None:
+            # Start consumer once there is at least one connection
+            # No consumer group, by default consumes from all partitions latest
             self.consumer = KafkaAdapter(self.app.kafka_config,KafkaRole.CONSUMER)
             self.consumer.start_consumer(topics=self.topic_names)
         if len(self.active_websocket_connections) == 0 and self.consumer is not None:
+            # Close consumer if there are no live connections...
             self.consumer.close()
             self.consumer = None
 
     async def consume(self):
         msgs = self.consumer.consume(
             num_messages=self.batch_size, timeout=0.1
         )
@@ -208,16 +211,16 @@
             async def endpoint(values: int):
                 result = await self.coroutine(values=values)
                 await self.websocket_broadcast_result(result)
                 return result
 
             annotate_function(
                 endpoint,
-                name=f"send_to_agent_{self.name}_from_{topic.name}",
-                doc=f"This endpoint send value to agent {self.name} from topic {topic.name}",
+                name=f"send_to_websocket_agent_{self.name}_from_{topic.name}",
+                doc=f"This endpoint sends value to agent {self.name} from topic {topic.name}",
                 argument_types={"values": List[topic.value_type]},
             )
 
             self.app.add_api_route(
                 path=f"{self.app.api_router_prefix}/agent/{self.name}/{topic.name}",
                 response_class=JSONResponse,
                 methods=["POST"],
```

### Comparing `citizenk-0.1.40/citizenk/citizenk.py` & `citizenk-0.1.41/citizenk/citizenk.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         logger.debug("CitizenK starting up...")
 
         # Find all consumer topics
         for agent in self.agents.values():
             self.consumer_topics.update({t.name for t in agent.topics})
             self.total_batch_size += agent.batch_size
 
-        # Create consumer
+        # Create and start consumer
         if len(self.consumer_topics) > 0:
             if self.app_type == AppType.SOURCE:
                 raise CitizenKError("Trying to consume topics in a source app")
             self.consumer = KafkaAdapter(
                 self.kafka_config,
                 KafkaRole.CONSUMER,
                 self.app_name,
@@ -218,35 +218,35 @@
 
         # Check that all topics exist in broker
         broker = self.producer if self.consumer is None else self.consumer
         broker_topics = broker.get_all_broker_topics()
         for topic_name, topic in self.topics.items():
             if topic_name not in broker_topics:
                 raise CitizenKError(f"Can't find topic {topic_name} in broker")
-            # Set num partitions and replicas in topic
+            # Set num partitions and replicas in topic. Might be usefull...
             topic.partition_count = len(broker_topics[topic_name].partitions)
             topic.replica_count = len(broker_topics[topic_name].partitions[0].replicas)
 
         # Start Main consumer loop if there is any consumer
-        # Normal consumer (with group)
+        # Normal gobal consumer (with group)
         # Websocket consumers (no group)
         if self.consumer is not None or len(self.websocket_agents) > 0:
 
             if self.agents_in_thread:
-                # Start in thread
+                # Start in a thread
                 self.background_loop = asyncio.new_event_loop()
                 self.background_thread = threading.Thread(
                     target=self.background_consumer_thread, args=(self.background_loop,)
                 )
                 self.background_thread.start()
                 self.main_consumer_loop_task = asyncio.run_coroutine_threadsafe(
                     self._main_consumer_loop(), self.background_loop
                 )
             else:
-                # Start in task
+                # Start in a task
                 self.main_consumer_loop_task = asyncio.create_task(
                     self._main_consumer_loop()
                 )
             self.monitor_loop_task = asyncio.create_task(self._monitor_loop())
 
     def shutdown(self):
         """CitizenK shutdown called on FastAPI shutown"""
@@ -296,47 +296,46 @@
         """Main Kafka consumer loop which invokes the process agents"""
         logger.debug("CitizenK main processing loop started...")
         while True:
             # Check if consumer was deleted
             if self.consumer is None and len(self.consumer_topics) > 0:
                 break
             
-            duration = 0
-            processed = False
             try:
+                start_time = time.time()
+                processed = False
+                # Consume from global consumer
                 if self.consumer is not None:
                     msgs = self.consumer.consume(
                         num_messages=self.total_batch_size, timeout=0.1
                     )
                     if len(msgs) > 0:
                         processed = True
-                        start_time = time.time()
                         events = Agent.validate_messages(msgs, self.topics)
                         for agent in self.agents.values():
                             await agent.process(events)
-                        duration = 1000 * (time.time() - start_time)
 
                 # Consume from websocket agents consumers (no group)
-                start_time = time.time()
                 for agent in self.websocket_agents.values():
                     if agent.consume():
                         processed = True
-                duration += 1000 * (time.time() - start_time)
 
-                # Poll producer
-                if self.producer is not None:
-                    self.producer.poll()
+                duration = 1000 * (time.time() - start_time)
 
                 if duration > self.max_processing_cycle_ms:
                     logger.error(
                         "Processing cycle took %s ms > %s",
                         duration,
                         self.max_processing_cycle_ms,
                     )
 
+                # Poll producer
+                if self.producer is not None:
+                    self.producer.poll()
+
                 if processed:
                     # Just to give other tasks opportunity to run
                     await asyncio.sleep(0)
                 else:
                     # Wait a bit until messages arrive
                     logger.debug("No kafka events, sleeping")
                     await asyncio.sleep(1)
```

### Comparing `citizenk-0.1.40/citizenk/kafka_adapter.py` & `citizenk-0.1.41/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.40/citizenk/murmur2.py` & `citizenk-0.1.41/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.40/citizenk/topic.py` & `citizenk-0.1.41/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.40/pyproject.toml` & `citizenk-0.1.41/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.40"
+version = "0.1.41"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.40/setup.py` & `citizenk-0.1.41/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.40',
+    'version': '0.1.41',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.40/PKG-INFO` & `citizenk-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.40
+Version: 0.1.41
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

