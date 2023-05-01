# Comparing `tmp/deche-0.7.0.tar.gz` & `tmp/deche-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deche-0.7.0.tar", max compression
+gzip compressed data, was "deche-0.8.0.tar", max compression
```

## Comparing `deche-0.7.0.tar` & `deche-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       99 2023-05-01 03:34:25.365554 deche-0.7.0/deche/__init__.py
--rw-r--r--   0        0        0    15628 2023-05-01 03:34:25.365747 deche-0.7.0/deche/core.py
--rw-r--r--   0        0        0      609 2023-05-01 03:34:20.574161 deche-0.7.0/deche/inspection.py
--rw-r--r--   0        0        0     1154 2023-05-01 03:34:20.574359 deche-0.7.0/deche/test_utils/__init__.py
--rw-r--r--   0        0        0     2277 2023-05-01 03:34:25.365890 deche-0.7.0/deche/util.py
--rw-r--r--   0        0        0      660 2023-05-01 03:34:20.575068 deche-0.7.0/deche/validators.py
--rw-r--r--   0        0        0      636 2023-05-01 03:34:25.368210 deche-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 deche-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2023-05-01 03:34:25.365554 deche-0.8.0/deche/__init__.py
+-rw-r--r--   0        0        0    15329 2023-05-01 04:07:21.289318 deche-0.8.0/deche/core.py
+-rw-r--r--   0        0        0      609 2023-05-01 03:34:20.574161 deche-0.8.0/deche/inspection.py
+-rw-r--r--   0        0        0     1154 2023-05-01 03:34:20.574359 deche-0.8.0/deche/test_utils/__init__.py
+-rw-r--r--   0        0        0     2277 2023-05-01 03:34:25.365890 deche-0.8.0/deche/util.py
+-rw-r--r--   0        0        0      660 2023-05-01 03:34:20.575068 deche-0.8.0/deche/validators.py
+-rw-r--r--   0        0        0      636 2023-05-01 04:07:36.105951 deche-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 deche-0.8.0/PKG-INFO
```

### Comparing `deche-0.7.0/deche/core.py` & `deche-0.8.0/deche/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import functools
 import hashlib
 import inspect
 import logging
 import pathlib
 import pickle
+import time
 from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum
 from functools import partial
 from typing import Any, Optional, Union
 
 import cloudpickle
@@ -167,40 +168,29 @@
         return deserializer(data)
 
     def read_output(self, path, deserializer=None):
         deserializer = deserializer or self.output_deserializer
         data = self.read(path=path)
         return deserializer(data)
 
-    def _write_ttl_append(self, path: str):
-        # move any existing files
-        key = pathlib.Path(path).name
-        for f in sorted(self.fs.glob(f"{path}*"), reverse=True):
-            if is_input_filename(f):
-                continue
-            if pathlib.Path(f).name == key:
-                num = 0
-                suffix = ""
-            else:
-                num = int(f.replace(f"{path}-", ""))
-                f = f[:-2]
-                suffix = f"-{num}"
-            self.fs.mv(f"{f}{suffix}", f"{f}-{num + 1}")
-
     def write(self, path: str, data: bytes):
-        if self.cache_ttl and self.cache_expiry_mode == CacheExpiryMode.APPEND and not is_input_filename(path):
-            self._write_ttl_append(path=path)
-
         # Ensure parent exists
         parent = str(pathlib.Path(path).parent)
         if parent not in self._parents:
             if not self.fs.exists(parent):
                 self.fs.mkdir(parent)
             self._parents.add(parent)
 
+        # If cache_ttl append, write a timestamped file.
+        if self.cache_ttl and self.cache_expiry_mode == CacheExpiryMode.APPEND and not is_input_filename(path):
+            ts_us = int(time.time() * 1e6)
+            with self.fs.open(f"{path}-{ts_us}", mode="wb") as f:
+                logger.debug(f"{self.fs_protocol}://{path}-{ts_us}")
+                f.write(data)
+
         with self.fs.open(path, mode="wb") as f:
             logger.debug(f"{self.fs_protocol}://{path}")
             return f.write(data)
 
     def write_input(self, path, inputs, input_serializer=None):
         key, input_value = tokenize(obj=inputs, serializer=input_serializer or self.input_serializer)
         self.write(path=f"{path}{Extensions.inputs}", data=input_value)
```

### Comparing `deche-0.7.0/deche/inspection.py` & `deche-0.8.0/deche/inspection.py`

 * *Files identical despite different names*

### Comparing `deche-0.7.0/deche/test_utils/__init__.py` & `deche-0.8.0/deche/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deche-0.7.0/deche/util.py` & `deche-0.8.0/deche/util.py`

 * *Files identical despite different names*

### Comparing `deche-0.7.0/deche/validators.py` & `deche-0.8.0/deche/validators.py`

 * *Files identical despite different names*

### Comparing `deche-0.7.0/pyproject.toml` & `deche-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deche"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fsspec = ">=2021.10.1"
 donfig = "^0.7.0"
```

### Comparing `deche-0.7.0/PKG-INFO` & `deche-0.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deche
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

