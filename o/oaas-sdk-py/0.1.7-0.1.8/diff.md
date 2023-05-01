# Comparing `tmp/oaas_sdk_py-0.1.7.tar.gz` & `tmp/oaas_sdk_py-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.1.7.tar", last modified: Mon Apr 24 11:03:18 2023, max compression
+gzip compressed data, was "oaas_sdk_py-0.1.8.tar", last modified: Mon May  1 10:14:35 2023, max compression
```

## Comparing `oaas_sdk_py-0.1.7.tar` & `oaas_sdk_py-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.235846 oaas_sdk_py-0.1.7/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      258 2023-04-24 11:03:18.234846 oaas_sdk_py-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.7/README.md
--rw-rw-rw-   0        0        0      495 2023-04-24 11:01:50.000000 oaas_sdk_py-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 11:03:18.235846 oaas_sdk_py-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.221095 oaas_sdk_py-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.226097 oaas_sdk_py-0.1.7/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     8948 2023-04-24 10:44:39.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1789 2023-04-24 11:01:38.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.233847 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.618412 oaas_sdk_py-0.1.8/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      258 2023-05-01 10:14:35.617875 oaas_sdk_py-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.8/README.md
+-rw-rw-rw-   0        0        0      495 2023-05-01 10:12:29.000000 oaas_sdk_py-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:14:35.618412 oaas_sdk_py-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.603930 oaas_sdk_py-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.609766 oaas_sdk_py-0.1.8/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     8945 2023-05-01 10:10:36.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-04-24 11:01:38.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:35.614613 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 10:14:35.000000 oaas_sdk_py-0.1.8/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.1.7/LICENSE` & `oaas_sdk_py-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.7/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.1.8/src/oaas_sdk_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import json
 from abc import abstractmethod
 from typing import Dict, List
 
 import aiofiles
 import aiofiles.os
+import aiohttp
 from aiohttp import ClientSession, ClientResponse
 
 from .model import *
 
 
 class OaasException(BaseException):
     pass
@@ -29,16 +30,16 @@
         raise OaasException(f"Got error when allocate keys (code:{resp.status})")
     return await resp.json()
 
 
 async def _upload(session: ClientSession,
                   path,
                   url):
-    async with aiofiles.open(path, "rb") as f:
-        size = await aiofiles.os.path.getsize(path)
+    size = await aiofiles.os.path.getsize(path)
+    with open(path, "rb") as f:
         headers = {"content-length": str(size)}
         resp = await session.put(url, headers=headers, data=f)
         if not resp.ok:
             raise OaasException(f"Got error when put the data to S3 (code:{resp.status})")
 
 
 class OaasInvocationCtx:
```

### Comparing `oaas_sdk_py-0.1.7/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.1.8/src/oaas_sdk_py/model.py`

 * *Files identical despite different names*

