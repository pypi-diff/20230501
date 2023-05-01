# Comparing `tmp/nuclio_sdk-0.5.1.tar.gz` & `tmp/nuclio_sdk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/tmpov6e68xs/nuclio_sdk-0.5.1.tar", last modified: Thu Aug 11 13:00:08 2022, max compression
+gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-jfy0923j/nuclio_sdk-0.5.2.tar", last modified: Mon May  1 08:30:35 2023, max compression
```

## Comparing `nuclio_sdk-0.5.1.tar` & `nuclio_sdk-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    18920 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     7863 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/mock_platform.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/nuclio_sdk/test/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/nuclio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-11 13:00:08.000000 nuclio_sdk-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2022-08-11 12:59:13.000000 nuclio_sdk-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/mock_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/nuclio_sdk/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/nuclio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 08:30:35.000000 nuclio_sdk-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-01 08:29:44.000000 nuclio_sdk-0.5.2/setup.py
```

### Comparing `nuclio_sdk-0.5.1/LICENSE.txt` & `nuclio_sdk-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/PKG-INFO` & `nuclio_sdk-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nuclio_sdk
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `nuclio_sdk-0.5.1/Pipfile` & `nuclio_sdk-0.5.2/Pipfile`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/Pipfile.lock` & `nuclio_sdk-0.5.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/__init__.py` & `nuclio_sdk-0.5.2/nuclio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/context.py` & `nuclio_sdk-0.5.2/nuclio_sdk/context.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/event.py` & `nuclio_sdk-0.5.2/nuclio_sdk/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 import enum
 import base64
 import sys
 import json
 import datetime
 
+import nuclio_sdk
+
 
 class _EventDeserializer(object):
     def deserialize(self, event_message):
         raise NotImplementedError
 
     @staticmethod
     def _try_deserialize_json(body):
@@ -224,19 +226,13 @@
         """
         return kind.value.deserialize(data)
 
     def compile_explicit_ack_message(self):
         """
         Return json of offset data
         """
-        return {
-            "kind": "streamMessageAck",
-            "attributes": {
-                "topic": self.path,
-                "partition": self.shard_id,
-                "offset": self.offset,
-                "triggerName": self.trigger.name,
-            },
-        }
+        return nuclio_sdk.QualifiedOffset.from_event(
+            self
+        ).compile_explicit_ack_message()
 
     def __repr__(self):
         return self.to_json()
```

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/exceptions.py` & `nuclio_sdk-0.5.2/nuclio_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/helpers.py` & `nuclio_sdk-0.5.2/nuclio_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/json_encoder.py` & `nuclio_sdk-0.5.2/nuclio_sdk/json_encoder.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/logger.py` & `nuclio_sdk-0.5.2/nuclio_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/platform.py` & `nuclio_sdk-0.5.2/nuclio_sdk/platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/qualified_offset.py` & `nuclio_sdk-0.5.2/nuclio_sdk/qualified_offset.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,21 @@
     def __init__(self, topic, partition, offset):
         self.topic = topic
         self.partition = partition
         self.offset = offset
 
     @staticmethod
     def from_event(event):
-        return QualifiedOffset(event.topic, event.partition, event.offset)
+        return QualifiedOffset(event.path, event.shard_id, event.offset)
 
     def compile_explicit_ack_message(self):
+        """
+        Return a stream ack message with json of offset data
+        """
         return {
-            "topic": self.topic,
-            "partition": self.partition,
-            "offset": self.offset,
+            "kind": "streamMessageAck",
+            "attributes": {
+                "topic": self.topic,
+                "partition": self.partition,
+                "offset": self.offset,
+            },
         }
```

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/response.py` & `nuclio_sdk-0.5.2/nuclio_sdk/response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/test/__init__.py` & `nuclio_sdk-0.5.2/nuclio_sdk/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/test/mock_platform.py` & `nuclio_sdk-0.5.2/nuclio_sdk/test/mock_platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/test/test_case.py` & `nuclio_sdk-0.5.2/nuclio_sdk/test/test_case.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/test/test_event.py` & `nuclio_sdk-0.5.2/nuclio_sdk/test/test_event.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/test/test_logger.py` & `nuclio_sdk-0.5.2/nuclio_sdk/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk/test/test_response.py` & `nuclio_sdk-0.5.2/nuclio_sdk/test/test_response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk.egg-info/PKG-INFO` & `nuclio_sdk-0.5.2/nuclio_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nuclio-sdk
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `nuclio_sdk-0.5.1/nuclio_sdk.egg-info/SOURCES.txt` & `nuclio_sdk-0.5.2/nuclio_sdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 nuclio_sdk.egg-info/dependency_links.txt
 nuclio_sdk.egg-info/top_level.txt
 nuclio_sdk/test/__init__.py
 nuclio_sdk/test/mock_platform.py
 nuclio_sdk/test/test_case.py
 nuclio_sdk/test/test_event.py
 nuclio_sdk/test/test_logger.py
+nuclio_sdk/test/test_qualified_offset.py
 nuclio_sdk/test/test_response.py
```

### Comparing `nuclio_sdk-0.5.1/setup.py` & `nuclio_sdk-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries",
     ],
     tests_require=["pytest", "flake8"],
 )
```

