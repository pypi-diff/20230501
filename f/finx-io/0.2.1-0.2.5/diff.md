# Comparing `tmp/finx_io-0.2.1.tar.gz` & `tmp/finx_io-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finx_io-0.2.1.tar", last modified: Thu Nov 17 15:30:47 2022, max compression
+gzip compressed data, was "finx_io-0.2.5.tar", last modified: Mon May  1 18:40:38 2023, max compression
```

## Comparing `finx_io-0.2.1.tar` & `finx_io-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2022-11-17 15:30:47.299872 finx_io-0.2.1/
--rw-r--r--   0 geoffreyfite   (501) staff       (20)    34500 2022-11-15 22:20:27.000000 finx_io-0.2.1/LICENSE
--rw-r--r--   0 geoffreyfite   (501) staff       (20)       18 2022-11-15 22:20:27.000000 finx_io-0.2.1/MANIFEST.in
--rw-r--r--   0 geoffreyfite   (501) staff       (20)    41622 2022-11-17 15:30:47.299600 finx_io-0.2.1/PKG-INFO
--rw-r--r--   0 geoffreyfite   (501) staff       (20)     1266 2022-11-15 22:20:27.000000 finx_io-0.2.1/README.md
--rw-r--r--   0 geoffreyfite   (501) staff       (20)     1462 2022-11-17 15:28:16.000000 finx_io-0.2.1/pyproject.toml
--rw-r--r--   0 geoffreyfite   (501) staff       (20)       38 2022-11-17 15:30:47.299950 finx_io-0.2.1/setup.cfg
--rw-r--r--   0 geoffreyfite   (501) staff       (20)      317 2022-11-17 15:21:51.000000 finx_io-0.2.1/setup.py
-drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2022-11-17 15:30:47.296378 finx_io-0.2.1/src/
--rw-r--r--   0 geoffreyfite   (501) staff       (20)        0 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/__init__.py
-drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2022-11-17 15:30:47.297498 finx_io-0.2.1/src/finx/
--rw-r--r--   0 geoffreyfite   (501) staff       (20)        0 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/__init__.py
--rw-r--r--   0 geoffreyfite   (501) staff       (20)    25360 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/client.py
--rw-r--r--   0 geoffreyfite   (501) staff       (20)     9832 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/finx_rest.py
--rw-r--r--   0 geoffreyfite   (501) staff       (20)     3743 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/finx_streamer.py
-drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2022-11-17 15:30:47.297914 finx_io-0.2.1/src/finx/tests/
--rw-r--r--   0 geoffreyfite   (501) staff       (20)        0 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/tests/__init__.py
--rw-r--r--   0 geoffreyfite   (501) staff       (20)      412 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/tests/test_finx_rest.py
--rw-r--r--   0 geoffreyfite   (501) staff       (20)     6441 2022-11-15 22:20:27.000000 finx_io-0.2.1/src/finx/tick_client.py
-drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2022-11-17 15:30:47.299132 finx_io-0.2.1/src/finx_io.egg-info/
--rw-r--r--   0 geoffreyfite   (501) staff       (20)    41622 2022-11-17 15:30:47.000000 finx_io-0.2.1/src/finx_io.egg-info/PKG-INFO
--rw-r--r--   0 geoffreyfite   (501) staff       (20)      415 2022-11-17 15:30:47.000000 finx_io-0.2.1/src/finx_io.egg-info/SOURCES.txt
--rw-r--r--   0 geoffreyfite   (501) staff       (20)        1 2022-11-17 15:30:47.000000 finx_io-0.2.1/src/finx_io.egg-info/dependency_links.txt
--rw-r--r--   0 geoffreyfite   (501) staff       (20)      182 2022-11-17 15:30:47.000000 finx_io-0.2.1/src/finx_io.egg-info/requires.txt
--rw-r--r--   0 geoffreyfite   (501) staff       (20)       14 2022-11-17 15:30:47.000000 finx_io-0.2.1/src/finx_io.egg-info/top_level.txt
+drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:40:38.917595 finx_io-0.2.5/
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)    34500 2023-05-01 18:28:20.000000 finx_io-0.2.5/LICENSE
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)       18 2023-05-01 18:28:20.000000 finx_io-0.2.5/MANIFEST.in
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)    41623 2023-05-01 18:40:38.917288 finx_io-0.2.5/PKG-INFO
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)     1266 2023-05-01 18:28:20.000000 finx_io-0.2.5/README.md
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)     1432 2023-05-01 18:28:20.000000 finx_io-0.2.5/pyproject.toml
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)       38 2023-05-01 18:40:38.917667 finx_io-0.2.5/setup.cfg
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)      299 2023-05-01 18:28:20.000000 finx_io-0.2.5/setup.py
+drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:40:38.913306 finx_io-0.2.5/src/
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/__init__.py
+drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:40:38.914721 finx_io-0.2.5/src/finx/
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/__init__.py
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)    25382 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/client.py
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)     9832 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/finx_rest.py
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)     3743 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/finx_streamer.py
+drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:40:38.915190 finx_io-0.2.5/src/finx/tests/
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/tests/__init__.py
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)      412 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/tests/test_finx_rest.py
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)     6441 2023-05-01 18:28:20.000000 finx_io-0.2.5/src/finx/tick_client.py
+drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:40:38.916566 finx_io-0.2.5/src/finx_io.egg-info/
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)    41623 2023-05-01 18:40:38.000000 finx_io-0.2.5/src/finx_io.egg-info/PKG-INFO
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)      433 2023-05-01 18:40:38.000000 finx_io-0.2.5/src/finx_io.egg-info/SOURCES.txt
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)        1 2023-05-01 18:40:38.000000 finx_io-0.2.5/src/finx_io.egg-info/dependency_links.txt
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)      171 2023-05-01 18:40:38.000000 finx_io-0.2.5/src/finx_io.egg-info/requires.txt
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)       14 2023-05-01 18:40:38.000000 finx_io-0.2.5/src/finx_io.egg-info/top_level.txt
+drwxr-xr-x   0 geoffreyfite   (501) staff       (20)        0 2023-05-01 18:40:38.916840 finx_io-0.2.5/tests/
+-rw-r--r--   0 geoffreyfite   (501) staff       (20)     3065 2023-05-01 18:28:20.000000 finx_io-0.2.5/tests/test_all.py
```

### Comparing `finx_io-0.2.1/LICENSE` & `finx_io-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finx_io-0.2.1/PKG-INFO` & `finx_io-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finx_io
-Version: 0.2.1
+Version: 0.2.5
 Summary: FinX Capital Markets Python SDK
 Author-email: FinX Capital Markets LLC <info@finx.io>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -667,15 +667,15 @@
         
 Project-URL: Homepage, https://finx.io
 Project-URL: Github, https://github.com/FinX-IO/sdk
 Project-URL: Bug Tracker, https://github.com/FinX-IO/sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
 title: APIs
 tags: technology, documentation
 ---
```

### Comparing `finx_io-0.2.1/README.md` & `finx_io-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `finx_io-0.2.1/src/finx/client.py` & `finx_io-0.2.5/src/finx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import aiohttp
 import asyncio
 import requests
 import functools
 import nest_asyncio
 import pandas as pd
 
-from lru import LRU
+# from lru import LRU
 from uuid import uuid4
 from gc import collect
 from time import sleep
 from io import StringIO
 from sys import getsizeof
 from threading import Thread
 from traceback import format_exc
@@ -120,15 +120,15 @@
         """
         self.__api_key = kwargs.get('finx_api_key') or os.environ.get('FINX_API_KEY')
         if self.__api_key is None:
             raise Exception('API key not found - please include the keyword argument '
                             'finx_api_key or set the environment variable FINX_API_KEY')
         self.__api_url = kwargs.get('finx_api_endpoint') or os.environ.get('FINX_API_ENDPOINT') or DEFAULT_API_URL
         self.cache_size = kwargs.get('cache_size') or 100000
-        self.cache = LRU(self.cache_size)
+        self.cache = dict()  # LRU(self.cache_size)
         self.cache_method_size = dict(security_analytics=3, cash_flows=1, reference_data=3)
         self.timeout = kwargs.get('timeout', 100)
         if not kwargs.get('no_init'):
             self._init_api_functions(**kwargs)
 
     async def __aenter__(self):
         self._session = aiohttp.ClientSession()
@@ -155,15 +155,15 @@
         cache_key = f'{f"{security_id}:{as_of_date}:" if security_id else ""}{api_method}'
         params_key = ','.join(
             [f'{key}:{params[key]}' for key in sorted(params.keys())
              if key not in ['security_id', 'as_of_date', 'api_method', 'input_file', 'output_file', 'block']])
         params_key = params_key if len(params_key) > 0 else 'NONE'
         cached_value = self.cache.get(cache_key, dict()).get(params_key)
         if cached_value is None:
-            self.cache[cache_key] = LRU(1) if security_id is None else LRU(self.cache_method_size.get(api_method, 1))
+            self.cache[cache_key] = dict()  # LRU(1) if security_id is None else LRU(self.cache_method_size.get(api_method, 1))
             self.cache[cache_key][params_key] = None
         return cached_value, cache_key, params_key
 
     def _init_api_functions(self, **kwargs):
         """
         Add all valid API Methods to Class
         """
```

### Comparing `finx_io-0.2.1/src/finx/finx_rest.py` & `finx_io-0.2.5/src/finx/finx_rest.py`

 * *Files identical despite different names*

### Comparing `finx_io-0.2.1/src/finx/finx_streamer.py` & `finx_io-0.2.5/src/finx/finx_streamer.py`

 * *Files identical despite different names*

### Comparing `finx_io-0.2.1/src/finx/tick_client.py` & `finx_io-0.2.5/src/finx/tick_client.py`

 * *Files identical despite different names*

### Comparing `finx_io-0.2.1/src/finx_io.egg-info/PKG-INFO` & `finx_io-0.2.5/src/finx_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finx-io
-Version: 0.2.1
+Version: 0.2.5
 Summary: FinX Capital Markets Python SDK
 Author-email: FinX Capital Markets LLC <info@finx.io>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -667,15 +667,15 @@
         
 Project-URL: Homepage, https://finx.io
 Project-URL: Github, https://github.com/FinX-IO/sdk
 Project-URL: Bug Tracker, https://github.com/FinX-IO/sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
 title: APIs
 tags: technology, documentation
 ---
```

