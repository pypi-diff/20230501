# Comparing `tmp/citizenk-0.1.43.tar.gz` & `tmp/citizenk-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.43.tar", max compression
+gzip compressed data, was "citizenk-0.1.44.tar", max compression
```

## Comparing `citizenk-0.1.43.tar` & `citizenk-0.1.44.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2023-05-01 09:49:27.845822 citizenk-0.1.43/citizenk/__init__.py
--rw-r--r--   0        0        0     8556 2023-05-01 17:06:07.155429 citizenk-0.1.43/citizenk/agent.py
--rw-r--r--   0        0        0    20613 2023-05-01 17:07:14.097178 citizenk-0.1.43/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.43/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.43/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.43/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.43/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-05-01 17:07:52.215548 citizenk-0.1.43/pyproject.toml
--rw-r--r--   0        0        0      863 2023-05-01 17:08:03.484598 citizenk-0.1.43/setup.py
--rw-r--r--   0        0        0     1076 2023-05-01 17:08:03.484851 citizenk-0.1.43/PKG-INFO
+-rw-r--r--   0        0        0      382 2023-05-01 09:49:27.845822 citizenk-0.1.44/citizenk/__init__.py
+-rw-r--r--   0        0        0     8576 2023-05-01 17:21:54.061835 citizenk-0.1.44/citizenk/agent.py
+-rw-r--r--   0        0        0    20613 2023-05-01 17:07:14.097178 citizenk-0.1.44/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.44/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.44/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.44/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.44/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-05-01 17:22:39.525375 citizenk-0.1.44/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-05-01 17:22:45.176355 citizenk-0.1.44/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-01 17:22:45.176615 citizenk-0.1.44/PKG-INFO
```

### Comparing `citizenk-0.1.43/citizenk/agent.py` & `citizenk-0.1.44/citizenk/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     async def consume(self):
         if self.consumer is not None:
             msgs = self.consumer.consume(
                 num_messages=self.batch_size, timeout=0.1
             )
             if len(msgs) > 0:
                 logger.debug("Agent %s consumed %s messages",self.name,len(msgs))
-                events = Agent.validate_messages(msgs, self.topics)
+                events = Agent.validate_messages(msgs, {t.name:t for t in self.topics})
                 await self.process(events)
                 return True
         return False
 
     def close(self):
         if self.consumer is not None:
             self.consumer.close()
```

### Comparing `citizenk-0.1.43/citizenk/citizenk.py` & `citizenk-0.1.44/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.43/citizenk/kafka_adapter.py` & `citizenk-0.1.44/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.43/citizenk/murmur2.py` & `citizenk-0.1.44/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.43/citizenk/topic.py` & `citizenk-0.1.44/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.43/pyproject.toml` & `citizenk-0.1.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.43"
+version = "0.1.44"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.43/setup.py` & `citizenk-0.1.44/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.43',
+    'version': '0.1.44',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.43/PKG-INFO` & `citizenk-0.1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.43
+Version: 0.1.44
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

