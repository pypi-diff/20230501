# Comparing `tmp/globus-compute-sdk-2.0.1a4.tar.gz` & `tmp/globus-compute-sdk-2.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.0.1a4.tar", last modified: Thu Apr 20 15:07:35 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.0.2a0.tar", last modified: Mon May  1 15:14:27 2023, max compression
```

## Comparing `globus-compute-sdk-2.0.1a4.tar` & `globus-compute-sdk-2.0.2a0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.982274 globus-compute-sdk-2.0.1a4/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.0.1a4/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1821 2023-04-20 15:07:35.982346 globus-compute-sdk-2.0.1a4/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.0.1a4/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.976064 globus-compute-sdk-2.0.1a4/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.977160 globus-compute-sdk-2.0.1a4/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.979020 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      970 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.979604 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11442 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    26362 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46344 2023-04-14 19:00:55.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.981206 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7287 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     2887 2023-04-13 00:34:31.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.981515 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8618 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.982132 globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-04-20 15:03:46.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-20 15:07:35.976736 globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1821 2023-04-20 15:07:35.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1577 2023-04-20 15:07:35.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-20 15:07:35.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      397 2023-04-20 15:07:35.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-04-20 15:07:35.000000 globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-20 15:07:35.982663 globus-compute-sdk-2.0.1a4/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3161 2023-04-20 15:03:07.000000 globus-compute-sdk-2.0.1a4/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.411738 globus-compute-sdk-2.0.2a0/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.0.2a0/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1821 2023-05-01 15:14:27.411809 globus-compute-sdk-2.0.2a0/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.0.2a0/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.407528 globus-compute-sdk-2.0.2a0/globus_compute_sdk/
+-rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.408482 globus-compute-sdk-2.0.2a0/globus_compute_sdk/errors/
+-rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.409357 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      986 2023-04-24 21:22:25.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.409814 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 lei        (501) staff       (20)    11458 2023-04-24 21:22:25.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 lei        (501) staff       (20)    26362 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 lei        (501) staff       (20)    46344 2023-04-14 19:00:55.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.410902 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 lei        (501) staff       (20)     7287 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)     2887 2023-04-13 00:34:31.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.411136 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 lei        (501) staff       (20)     8618 2023-04-25 15:43:22.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.411612 globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)      834 2023-05-01 15:05:12.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:27.408233 globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1821 2023-05-01 15:14:27.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1577 2023-05-01 15:14:27.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-01 15:14:27.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      397 2023-05-01 15:14:27.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       19 2023-05-01 15:14:27.000000 globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-05-01 15:14:27.412115 globus-compute-sdk-2.0.2a0/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3161 2023-04-25 18:18:02.000000 globus-compute-sdk-2.0.2a0/setup.py
```

### Comparing `globus-compute-sdk-2.0.1a4/LICENSE` & `globus-compute-sdk-2.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/PKG-INFO` & `globus-compute-sdk-2.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.1a4
+Version: 2.0.2a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.0.1a4/PyPI.md` & `globus-compute-sdk-2.0.2a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/_environments.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 def _get_envname():
     return os.getenv("FUNCX_SDK_ENVIRONMENT", "production")
 
 
 def get_web_service_url(envname: str | None) -> str:
     env = envname or _get_envname()
     urls = {
-        "production": "https://api2.funcx.org/v2",
+        "production": "https://compute.api.globus.org/v2",
         "dev": "https://api.dev.funcx.org/v2",
         "local": "http://localhost:5000/v2",
     }
     return urls.get(env, urls["production"])
 
 
 def get_web_socket_url(envname: str | None) -> str:
     env = envname or _get_envname()
     urls = {
-        "production": "wss://api2.funcx.org/ws/v2/",
+        "production": "wss://compute.api.globus.org/ws/v2/",
         "dev": "wss://api.dev.funcx.org/ws/v2/",
         "local": "ws://localhost:6000/v2",
     }
     return urls.get(env, urls["production"])
 
 
 def urls_might_mismatch(service_url: str, socket_url: str) -> bool:
```

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def __init__(
         self,
         funcx_client,
         loop: AbstractEventLoop,
         atomic_controller=None,
         init_task_group_id: str | None = None,
-        results_ws_uri: str = "wss://api2.funcx.org/ws/v2/",
+        results_ws_uri: str = "wss://compute.api.globus.org/ws/v2/",
         auto_start: bool = True,
     ):
         """
         Parameters
         ==========
 
         funcx_client : client object
@@ -59,15 +59,15 @@
 
         init_task_group_id : str
             Optional task_group_id UUID string that the WebSocket client
             can immediately poll for after initialization
 
         results_ws_uri : str
             Web sockets URI for the results.
-            Default: wss://api2.funcx.org/ws/v2
+            Default: wss://compute.api.globus.org/ws/v2
 
         auto_start : Bool
             Set this to start the WebSocket client immediately.
             Otherwise init_ws must be called.
             Default: True
         """
         self.funcx_client = funcx_client
```

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk/version.py` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a4"
+__version__ = "2.0.2a0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.1a4
+Version: 2.0.2a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.0.1a4/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.0.2a0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a4/setup.py` & `globus-compute-sdk-2.0.2a0/setup.py`

 * *Files identical despite different names*

