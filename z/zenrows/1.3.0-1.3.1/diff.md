# Comparing `tmp/zenrows-1.3.0.tar.gz` & `tmp/zenrows-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenrows-1.3.0.tar", last modified: Tue Jun 14 15:12:18 2022, max compression
+gzip compressed data, was "zenrows-1.3.1.tar", last modified: Mon May  1 14:35:31 2023, max compression
```

## Comparing `zenrows-1.3.0.tar` & `zenrows-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 ander     (1000) ander     (1000)        0 2022-06-14 15:12:18.310141 zenrows-1.3.0/
--rw-rw-r--   0 ander     (1000) ander     (1000)     1063 2021-12-13 15:55:20.000000 zenrows-1.3.0/LICENSE
--rw-rw-r--   0 ander     (1000) ander     (1000)     5717 2022-06-14 15:12:18.306141 zenrows-1.3.0/PKG-INFO
--rw-rw-r--   0 ander     (1000) ander     (1000)     4664 2022-06-14 07:55:12.000000 zenrows-1.3.0/README.md
--rw-rw-r--   0 ander     (1000) ander     (1000)       38 2022-06-14 15:12:18.310141 zenrows-1.3.0/setup.cfg
--rw-rw-r--   0 ander     (1000) ander     (1000)     1381 2021-12-15 13:01:56.000000 zenrows-1.3.0/setup.py
-drwxrwxr-x   0 ander     (1000) ander     (1000)        0 2022-06-14 15:12:18.302141 zenrows-1.3.0/zenrows/
--rw-rw-r--   0 ander     (1000) ander     (1000)       70 2021-12-13 15:30:15.000000 zenrows-1.3.0/zenrows/__init__.py
--rw-rw-r--   0 ander     (1000) ander     (1000)       22 2022-06-13 16:12:14.000000 zenrows-1.3.0/zenrows/__version__.py
--rw-rw-r--   0 ander     (1000) ander     (1000)     2556 2022-06-14 08:13:19.000000 zenrows-1.3.0/zenrows/client.py
--rw-rw-r--   0 ander     (1000) ander     (1000)     1410 2022-02-02 11:22:35.000000 zenrows-1.3.0/zenrows/eci.py
-drwxrwxr-x   0 ander     (1000) ander     (1000)        0 2022-06-14 15:12:18.306141 zenrows-1.3.0/zenrows.egg-info/
--rw-rw-r--   0 ander     (1000) ander     (1000)     5717 2022-06-14 15:12:18.000000 zenrows-1.3.0/zenrows.egg-info/PKG-INFO
--rw-rw-r--   0 ander     (1000) ander     (1000)      256 2022-06-14 15:12:18.000000 zenrows-1.3.0/zenrows.egg-info/SOURCES.txt
--rw-rw-r--   0 ander     (1000) ander     (1000)        1 2022-06-14 15:12:18.000000 zenrows-1.3.0/zenrows.egg-info/dependency_links.txt
--rw-rw-r--   0 ander     (1000) ander     (1000)        9 2022-06-14 15:12:18.000000 zenrows-1.3.0/zenrows.egg-info/requires.txt
--rw-rw-r--   0 ander     (1000) ander     (1000)        8 2022-06-14 15:12:18.000000 zenrows-1.3.0/zenrows.egg-info/top_level.txt
+drwxr-xr-x   0 ander      (501) staff       (20)        0 2023-05-01 14:35:31.094509 zenrows-1.3.1/
+-rw-r--r--   0 ander      (501) staff       (20)     1063 2023-05-01 12:21:40.000000 zenrows-1.3.1/LICENSE
+-rw-r--r--   0 ander      (501) staff       (20)     5717 2023-05-01 14:35:31.094383 zenrows-1.3.1/PKG-INFO
+-rw-r--r--   0 ander      (501) staff       (20)     4664 2023-05-01 12:21:40.000000 zenrows-1.3.1/README.md
+-rw-r--r--   0 ander      (501) staff       (20)       38 2023-05-01 14:35:31.094559 zenrows-1.3.1/setup.cfg
+-rw-r--r--   0 ander      (501) staff       (20)     1381 2023-05-01 12:21:40.000000 zenrows-1.3.1/setup.py
+drwxr-xr-x   0 ander      (501) staff       (20)        0 2023-05-01 14:35:31.093567 zenrows-1.3.1/zenrows/
+-rw-r--r--   0 ander      (501) staff       (20)       70 2023-05-01 12:21:40.000000 zenrows-1.3.1/zenrows/__init__.py
+-rw-r--r--   0 ander      (501) staff       (20)       22 2023-05-01 13:15:56.000000 zenrows-1.3.1/zenrows/__version__.py
+-rw-r--r--   0 ander      (501) staff       (20)     2740 2023-05-01 12:36:04.000000 zenrows-1.3.1/zenrows/client.py
+drwxr-xr-x   0 ander      (501) staff       (20)        0 2023-05-01 14:35:31.094140 zenrows-1.3.1/zenrows.egg-info/
+-rw-r--r--   0 ander      (501) staff       (20)     5717 2023-05-01 14:35:31.000000 zenrows-1.3.1/zenrows.egg-info/PKG-INFO
+-rw-r--r--   0 ander      (501) staff       (20)      241 2023-05-01 14:35:31.000000 zenrows-1.3.1/zenrows.egg-info/SOURCES.txt
+-rw-r--r--   0 ander      (501) staff       (20)        1 2023-05-01 14:35:31.000000 zenrows-1.3.1/zenrows.egg-info/dependency_links.txt
+-rw-r--r--   0 ander      (501) staff       (20)        9 2023-05-01 14:35:31.000000 zenrows-1.3.1/zenrows.egg-info/requires.txt
+-rw-r--r--   0 ander      (501) staff       (20)        8 2023-05-01 14:35:31.000000 zenrows-1.3.1/zenrows.egg-info/top_level.txt
```

### Comparing `zenrows-1.3.0/LICENSE` & `zenrows-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zenrows-1.3.0/PKG-INFO` & `zenrows-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenrows
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for ZenRows API
 Home-page: https://github.com/ZenRows/zenrows-python-sdk
 Author: Ander Rodriguez
 Author-email: ander@zenrows.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ZenRows/zenrows-python-sdk/issues
 Project-URL: Documentation, https://www.zenrows.com/documentation
```

### Comparing `zenrows-1.3.0/README.md` & `zenrows-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zenrows-1.3.0/setup.py` & `zenrows-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `zenrows-1.3.0/zenrows/client.py` & `zenrows-1.3.1/zenrows/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 import asyncio
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 from concurrent.futures import ThreadPoolExecutor
+import urllib3
 
 from .__version__ import __version__
 
 
 class ZenRowsClient:
     api_url = "https://api.zenrows.com/v1/"
 
@@ -16,15 +17,15 @@
         self.executor = ThreadPoolExecutor(max_workers=concurrency)
 
         self.requests_session = requests.Session()
         if (retries > 0):
             max_retries = Retry().new(
                 total=retries,
                 backoff_factor=0.5,
-                status_forcelist=[429, 500, 502, 503, 504],
+                status_forcelist=[422, 429, 500, 502, 503, 504],
                 raise_on_status=False,
             )
             adapter = HTTPAdapter(max_retries=max_retries)
             self.requests_session.mount("https://", adapter)
             self.requests_session.mount("http://", adapter)
 
     def get(
@@ -53,18 +54,23 @@
         self, method, url: str, params: dict = None, headers: dict = None, data: dict = None, **kwargs
     ):
         final_params = {}
         if params:
             final_params.update(params)
         final_params.update({"url": url, "apikey": self.apikey})
 
+        final_headers = {"User-Agent": f"zenrows/{__version__} python"}
+
         if headers:
             final_params["custom_headers"] = True
+
+            final_headers["Accept"] = None
+            final_headers["Accept-Encoding"] = urllib3.util.SKIP_HEADER
+            final_headers["Connection"] = None
         else:
             headers = {}
 
-        final_headers = {"User-Agent": f"zenrows/{__version__} python"}
         final_headers.update(headers)
 
         return self.requests_session.request(
             method, self.api_url, params=final_params, headers=final_headers, data=data, **kwargs
         )
```

### Comparing `zenrows-1.3.0/zenrows.egg-info/PKG-INFO` & `zenrows-1.3.1/zenrows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenrows
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for ZenRows API
 Home-page: https://github.com/ZenRows/zenrows-python-sdk
 Author: Ander Rodriguez
 Author-email: ander@zenrows.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ZenRows/zenrows-python-sdk/issues
 Project-URL: Documentation, https://www.zenrows.com/documentation
```

