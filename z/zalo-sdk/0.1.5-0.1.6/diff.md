# Comparing `tmp/zalo_sdk-0.1.5.tar.gz` & `tmp/zalo_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalo_sdk-0.1.5.tar", last modified: Thu Apr 20 19:57:17 2023, max compression
+gzip compressed data, was "zalo_sdk-0.1.6.tar", last modified: Mon May  1 12:04:25 2023, max compression
```

## Comparing `zalo_sdk-0.1.5.tar` & `zalo_sdk-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-04-20 19:57:17.185095 zalo_sdk-0.1.5/
--rw-r--r--   0 kenji      (502) staff       (20)     1064 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/LICENSE
--rw-r--r--   0 kenji      (502) staff       (20)     1821 2023-04-20 19:57:17.184965 zalo_sdk-0.1.5/PKG-INFO
--rw-r--r--   0 kenji      (502) staff       (20)      377 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/README.md
--rw-r--r--   0 kenji      (502) staff       (20)       38 2023-04-20 19:57:17.185137 zalo_sdk-0.1.5/setup.cfg
--rw-r--r--   0 kenji      (502) staff       (20)      452 2023-04-20 19:52:41.000000 zalo_sdk-0.1.5/setup.py
-drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-04-20 19:57:17.183486 zalo_sdk-0.1.5/zalo_sdk/
--rw-r--r--   0 kenji      (502) staff       (20)     1512 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/zalo_sdk/BaseClient.py
--rw-r--r--   0 kenji      (502) staff       (20)       34 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/zalo_sdk/__init__.py
-drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-04-20 19:57:17.184770 zalo_sdk-0.1.5/zalo_sdk/oa/
--rw-r--r--   0 kenji      (502) staff       (20)     5490 2023-04-20 09:06:28.000000 zalo_sdk-0.1.5/zalo_sdk/oa/Client.py
--rw-r--r--   0 kenji      (502) staff       (20)     5414 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/zalo_sdk/oa/ZaloMessage.py
--rw-r--r--   0 kenji      (502) staff       (20)     2426 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/zalo_sdk/oa/ZaloOAException.py
--rw-r--r--   0 kenji      (502) staff       (20)       79 2023-04-20 07:02:15.000000 zalo_sdk-0.1.5/zalo_sdk/oa/__init__.py
-drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-04-20 19:57:17.184046 zalo_sdk-0.1.5/zalo_sdk.egg-info/
--rw-r--r--   0 kenji      (502) staff       (20)     1821 2023-04-20 19:57:17.000000 zalo_sdk-0.1.5/zalo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 kenji      (502) staff       (20)      302 2023-04-20 19:57:17.000000 zalo_sdk-0.1.5/zalo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 kenji      (502) staff       (20)        1 2023-04-20 19:57:17.000000 zalo_sdk-0.1.5/zalo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 kenji      (502) staff       (20)        9 2023-04-20 19:57:17.000000 zalo_sdk-0.1.5/zalo_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-05-01 12:04:25.179134 zalo_sdk-0.1.6/
+-rw-r--r--   0 kenji      (502) staff       (20)     1064 2023-04-20 07:02:15.000000 zalo_sdk-0.1.6/LICENSE
+-rw-r--r--   0 kenji      (502) staff       (20)     1779 2023-05-01 12:04:25.178990 zalo_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0 kenji      (502) staff       (20)      335 2023-05-01 12:04:08.000000 zalo_sdk-0.1.6/README.md
+-rw-r--r--   0 kenji      (502) staff       (20)       38 2023-05-01 12:04:25.179185 zalo_sdk-0.1.6/setup.cfg
+-rw-r--r--   0 kenji      (502) staff       (20)      452 2023-05-01 12:03:50.000000 zalo_sdk-0.1.6/setup.py
+drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-05-01 12:04:25.177137 zalo_sdk-0.1.6/zalo_sdk/
+-rw-r--r--   0 kenji      (502) staff       (20)     1512 2023-04-20 07:02:15.000000 zalo_sdk-0.1.6/zalo_sdk/BaseClient.py
+-rw-r--r--   0 kenji      (502) staff       (20)       34 2023-04-20 07:02:15.000000 zalo_sdk-0.1.6/zalo_sdk/__init__.py
+drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-05-01 12:04:25.178769 zalo_sdk-0.1.6/zalo_sdk/oa/
+-rw-r--r--   0 kenji      (502) staff       (20)     5474 2023-05-01 11:51:05.000000 zalo_sdk-0.1.6/zalo_sdk/oa/Client.py
+-rw-r--r--   0 kenji      (502) staff       (20)     5414 2023-04-20 07:02:15.000000 zalo_sdk-0.1.6/zalo_sdk/oa/ZaloMessage.py
+-rw-r--r--   0 kenji      (502) staff       (20)     2426 2023-04-20 07:02:15.000000 zalo_sdk-0.1.6/zalo_sdk/oa/ZaloOAException.py
+-rw-r--r--   0 kenji      (502) staff       (20)       79 2023-04-20 07:02:15.000000 zalo_sdk-0.1.6/zalo_sdk/oa/__init__.py
+drwxr-xr-x   0 kenji      (502) staff       (20)        0 2023-05-01 12:04:25.178043 zalo_sdk-0.1.6/zalo_sdk.egg-info/
+-rw-r--r--   0 kenji      (502) staff       (20)     1779 2023-05-01 12:04:25.000000 zalo_sdk-0.1.6/zalo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 kenji      (502) staff       (20)      302 2023-05-01 12:04:25.000000 zalo_sdk-0.1.6/zalo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 kenji      (502) staff       (20)        1 2023-05-01 12:04:25.000000 zalo_sdk-0.1.6/zalo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 kenji      (502) staff       (20)        9 2023-05-01 12:04:25.000000 zalo_sdk-0.1.6/zalo_sdk.egg-info/top_level.txt
```

### Comparing `zalo_sdk-0.1.5/LICENSE` & `zalo_sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zalo_sdk-0.1.5/PKG-INFO` & `zalo_sdk-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Zalo SDK
 Home-page: https://github.com/connext-biz/zalo_integration
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
@@ -33,17 +33,12 @@
 
 This is a work in progress project. **Use at your own risk!**
 
 At this point, this library only support Official Account APIs.
 
 If you found any problems, please create an issue to track it, or feel free to open a PR.
 
-## Installation
-
-`pip install zalo_sdk`
-
-
 ## Documentation
 
 The code is its own document.
 
 (I'm kidding, I'll add documentation later)
```

### Comparing `zalo_sdk-0.1.5/zalo_sdk/BaseClient.py` & `zalo_sdk-0.1.6/zalo_sdk/BaseClient.py`

 * *Files identical despite different names*

### Comparing `zalo_sdk-0.1.5/zalo_sdk/oa/Client.py` & `zalo_sdk-0.1.6/zalo_sdk/oa/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def check_zalo_error(self, response):
         if "error" in response and response["error"] != 0:
             if "message" in response:
                 if response["error"] == -216 and "expired" in response["message"]:
                     raise zalo_sdk.oa.ZaloOAAuthTokenExpiredException(response["error"], response["message"])
                 raise zalo_sdk.oa.ZaloOAException(response["error"], response["message"])
-            raise zalo_sdk.oa.ZaloOAException.ZaloOAException(response["error"])
+            raise zalo_sdk.oa.ZaloOAException(response["error"])
 
     def request_authoriation_code_url(self, callback_url, code_challenge=None, state=None):
         """
         Get the URL to request the authorization code.
 
         Official Documentation:
         https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-1-xac-thuc-voi-giao-thuc-oauth/yeu-cau-cap-moi-oa-access-token-post-4307
```

### Comparing `zalo_sdk-0.1.5/zalo_sdk/oa/ZaloMessage.py` & `zalo_sdk-0.1.6/zalo_sdk/oa/ZaloMessage.py`

 * *Files identical despite different names*

### Comparing `zalo_sdk-0.1.5/zalo_sdk/oa/ZaloOAException.py` & `zalo_sdk-0.1.6/zalo_sdk/oa/ZaloOAException.py`

 * *Files identical despite different names*

### Comparing `zalo_sdk-0.1.5/zalo_sdk.egg-info/PKG-INFO` & `zalo_sdk-0.1.6/zalo_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Zalo SDK
 Home-page: https://github.com/connext-biz/zalo_integration
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
@@ -33,17 +33,12 @@
 
 This is a work in progress project. **Use at your own risk!**
 
 At this point, this library only support Official Account APIs.
 
 If you found any problems, please create an issue to track it, or feel free to open a PR.
 
-## Installation
-
-`pip install zalo_sdk`
-
-
 ## Documentation
 
 The code is its own document.
 
 (I'm kidding, I'll add documentation later)
```

