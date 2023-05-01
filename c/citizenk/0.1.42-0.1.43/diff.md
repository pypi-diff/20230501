# Comparing `tmp/citizenk-0.1.42.tar.gz` & `tmp/citizenk-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.42.tar", max compression
+gzip compressed data, was "citizenk-0.1.43.tar", max compression
```

## Comparing `citizenk-0.1.42.tar` & `citizenk-0.1.43.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2023-05-01 09:49:27.845822 citizenk-0.1.42/citizenk/__init__.py
--rw-r--r--   0        0        0     8486 2023-05-01 11:31:34.103533 citizenk-0.1.42/citizenk/agent.py
--rw-r--r--   0        0        0    20607 2023-05-01 11:19:44.986124 citizenk-0.1.42/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.42/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.42/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.42/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.42/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-05-01 11:32:00.758890 citizenk-0.1.42/pyproject.toml
--rw-r--r--   0        0        0      863 2023-05-01 11:32:04.191542 citizenk-0.1.42/setup.py
--rw-r--r--   0        0        0     1076 2023-05-01 11:32:04.191804 citizenk-0.1.42/PKG-INFO
+-rw-r--r--   0        0        0      382 2023-05-01 09:49:27.845822 citizenk-0.1.43/citizenk/__init__.py
+-rw-r--r--   0        0        0     8556 2023-05-01 17:06:07.155429 citizenk-0.1.43/citizenk/agent.py
+-rw-r--r--   0        0        0    20613 2023-05-01 17:07:14.097178 citizenk-0.1.43/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.43/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.43/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.43/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.43/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-05-01 17:07:52.215548 citizenk-0.1.43/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-05-01 17:08:03.484598 citizenk-0.1.43/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-01 17:08:03.484851 citizenk-0.1.43/PKG-INFO
```

### Comparing `citizenk-0.1.42/citizenk/agent.py` & `citizenk-0.1.43/citizenk/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,22 +187,23 @@
         if len(self.active_websocket_connections) == 0 and self.consumer is not None:
             # Close consumer if there are no live connections...
             self.consumer.close()
             self.consumer = None
             logger.debug("Closed agent %s consumer",self.name)
 
     async def consume(self):
-        msgs = self.consumer.consume(
-            num_messages=self.batch_size, timeout=0.1
-        )
-        if len(msgs) > 0:
-            logger.debug("Agent %s consumed %s messages",self.name,len(msgs))
-            events = Agent.validate_messages(msgs, self.topics)
-            await self.process(events)
-            return True
+        if self.consumer is not None:
+            msgs = self.consumer.consume(
+                num_messages=self.batch_size, timeout=0.1
+            )
+            if len(msgs) > 0:
+                logger.debug("Agent %s consumed %s messages",self.name,len(msgs))
+                events = Agent.validate_messages(msgs, self.topics)
+                await self.process(events)
+                return True
         return False
 
     def close(self):
         if self.consumer is not None:
             self.consumer.close()
             self.consumer = None
         for connection in self.active_websocket_connections:
```

### Comparing `citizenk-0.1.42/citizenk/citizenk.py` & `citizenk-0.1.43/citizenk/citizenk.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
                         processed = True
                         events = Agent.validate_messages(msgs, self.topics)
                         for agent in self.agents.values():
                             await agent.process(events)
 
                 # Consume from websocket agents consumers (no group)
                 for agent in self.websocket_agents.values():
-                    if agent.consume():
+                    if await agent.consume():
                         processed = True
 
                 duration = 1000 * (time.time() - start_time)
 
                 if duration > self.max_processing_cycle_ms:
                     logger.error(
                         "Processing cycle took %s ms > %s",
```

### Comparing `citizenk-0.1.42/citizenk/kafka_adapter.py` & `citizenk-0.1.43/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.42/citizenk/murmur2.py` & `citizenk-0.1.43/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.42/citizenk/topic.py` & `citizenk-0.1.43/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.42/pyproject.toml` & `citizenk-0.1.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.42"
+version = "0.1.43"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.42/setup.py` & `citizenk-0.1.43/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.42',
+    'version': '0.1.43',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.42/PKG-INFO` & `citizenk-0.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.42
+Version: 0.1.43
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

