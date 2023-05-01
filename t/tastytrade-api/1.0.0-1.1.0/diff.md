# Comparing `tmp/tastytrade-api-1.0.0.tar.gz` & `tmp/tastytrade-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-1.0.0.tar", last modified: Thu Apr 27 08:25:14 2023, max compression
+gzip compressed data, was "tastytrade-api-1.1.0.tar", last modified: Mon May  1 11:02:00 2023, max compression
```

## Comparing `tastytrade-api-1.0.0.tar` & `tastytrade-api-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.157120 tastytrade-api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-27 08:25:14.157120 tastytrade-api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:25:14.157120 tastytrade-api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.153119 tastytrade-api-1.0.0/tastytrade_api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.153119 tastytrade-api-1.0.0/tastytrade_api/account/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/account/account_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/account/balances_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/account/watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.153119 tastytrade-api-1.0.0/tastytrade_api/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/market_data/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/market_data/market_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.157120 tastytrade-api-1.0.0/tastytrade_api/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/streamer/dx_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/streamer/dxfeed_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/streamer/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tastytrade_api/symbology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.153119 tastytrade-api-1.0.0/tastytrade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-27 08:25:14.000000 tastytrade-api-1.0.0/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 08:25:14.000000 tastytrade-api-1.0.0/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:25:14.000000 tastytrade-api-1.0.0/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 08:25:14.000000 tastytrade-api-1.0.0/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 08:25:14.000000 tastytrade-api-1.0.0/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:25:14.157120 tastytrade-api-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-27 08:24:48.000000 tastytrade-api-1.0.0/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/account_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/balances_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/market_data/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/market_data/market_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/dx_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/dxfeed_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/symbology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tests/test_authentication.py
```

### Comparing `tastytrade-api-1.0.0/PKG-INFO` & `tastytrade-api-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-1.0.0/README.md` & `tastytrade-api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/setup.py` & `tastytrade-api-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="1.0.0",
+    version="1.1.0",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client and SDK for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
@@ -24,11 +24,11 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
 
     ],
     python_requires=">=3.6",
     install_requires=[
         "requests",
-        "websocket",
+        "websocket-client",
         "websockets"
     ],
 )
```

### Comparing `tastytrade-api-1.0.0/tastytrade_api/account/account_handler.py` & `tastytrade-api-1.1.0/tastytrade_api/account/account_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/account/balances_positions.py` & `tastytrade-api-1.1.0/tastytrade_api/account/balances_positions.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/account/watchlist.py` & `tastytrade-api-1.1.0/tastytrade_api/account/watchlist.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/authentication.py` & `tastytrade-api-1.1.0/tastytrade_api/authentication.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/market_data/instruments.py` & `tastytrade-api-1.1.0/tastytrade_api/market_data/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/market_data/market_metrics.py` & `tastytrade-api-1.1.0/tastytrade_api/market_data/market_metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/streamer/streamer.py` & `tastytrade-api-1.1.0/tastytrade_api/streamer/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api/symbology.py` & `tastytrade-api-1.1.0/tastytrade_api/symbology.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-1.1.0/tastytrade_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-1.0.0/tastytrade_api.egg-info/SOURCES.txt` & `tastytrade-api-1.1.0/tastytrade_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.0.0/tests/test_authentication.py` & `tastytrade-api-1.1.0/tests/test_authentication.py`

 * *Files identical despite different names*

