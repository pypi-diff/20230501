# Comparing `tmp/fmpy_qi-0.1.0.tar.gz` & `tmp/fmpy_qi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpy_qi-0.1.0.tar", last modified: Mon May  1 14:54:01 2023, max compression
+gzip compressed data, was "fmpy_qi-0.1.1.tar", last modified: Mon May  1 15:00:19 2023, max compression
```

## Comparing `fmpy_qi-0.1.0.tar` & `fmpy_qi-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 14:54:01.212794 fmpy_qi-0.1.0/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.0/LICENSE
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-01 14:54:01.212408 fmpy_qi-0.1.0/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2106 2023-05-01 13:29:43.000000 fmpy_qi-0.1.0/README.md
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-01 14:53:39.000000 fmpy_qi-0.1.0/pyproject.toml
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-01 14:54:01.212895 fmpy_qi-0.1.0/setup.cfg
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 14:54:00.994712 fmpy_qi-0.1.0/src/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.0/src/__init__.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 14:54:01.143774 fmpy_qi-0.1.0/src/fmpy/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.0/src/fmpy/__init__.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     7967 2023-05-01 09:45:22.000000 fmpy_qi-0.1.0/src/fmpy/client.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-04-23 08:55:58.000000 fmpy_qi-0.1.0/src/fmpy/urls.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      940 2023-04-30 16:47:40.000000 fmpy_qi-0.1.0/src/fmpy/utils.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 14:54:01.211867 fmpy_qi-0.1.0/src/fmpy_qi.egg-info/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-01 14:54:00.000000 fmpy_qi-0.1.0/src/fmpy_qi.egg-info/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-01 14:54:00.000000 fmpy_qi-0.1.0/src/fmpy_qi.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-01 14:54:00.000000 fmpy_qi-0.1.0/src/fmpy_qi.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-01 14:54:00.000000 fmpy_qi-0.1.0/src/fmpy_qi.egg-info/requires.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-01 14:54:00.000000 fmpy_qi-0.1.0/src/fmpy_qi.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 15:00:19.278411 fmpy_qi-0.1.1/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.1/LICENSE
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-01 15:00:19.278057 fmpy_qi-0.1.1/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2106 2023-05-01 13:29:43.000000 fmpy_qi-0.1.1/README.md
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-01 14:59:53.000000 fmpy_qi-0.1.1/pyproject.toml
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-01 15:00:19.278517 fmpy_qi-0.1.1/setup.cfg
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 15:00:19.204894 fmpy_qi-0.1.1/src/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.1/src/__init__.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 15:00:19.258057 fmpy_qi-0.1.1/src/fmpy/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.1/src/fmpy/__init__.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     7959 2023-05-01 14:59:30.000000 fmpy_qi-0.1.1/src/fmpy/client.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-04-23 08:55:58.000000 fmpy_qi-0.1.1/src/fmpy/urls.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      940 2023-04-30 16:47:40.000000 fmpy_qi-0.1.1/src/fmpy/utils.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 15:00:19.277591 fmpy_qi-0.1.1/src/fmpy_qi.egg-info/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-01 15:00:19.000000 fmpy_qi-0.1.1/src/fmpy_qi.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-01 15:00:19.000000 fmpy_qi-0.1.1/src/fmpy_qi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-01 15:00:19.000000 fmpy_qi-0.1.1/src/fmpy_qi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-01 15:00:19.000000 fmpy_qi-0.1.1/src/fmpy_qi.egg-info/requires.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-01 15:00:19.000000 fmpy_qi-0.1.1/src/fmpy_qi.egg-info/top_level.txt
```

### Comparing `fmpy_qi-0.1.0/LICENSE` & `fmpy_qi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.0/PKG-INFO` & `fmpy_qi-0.1.1/src/fmpy_qi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fmpy_qi
-Version: 0.1.0
+Name: fmpy-qi
+Version: 0.1.1
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fmpy_qi-0.1.0/README.md` & `fmpy_qi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.0/pyproject.toml` & `fmpy_qi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fmpy_qi"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Nicolas THIERY", email="nicles.thiery@gmail.com" },
 ]
 description = "A python wrapper for the Financial Modeling Prep API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `fmpy_qi-0.1.0/src/fmpy/client.py` & `fmpy_qi-0.1.1/src/fmpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 import os
 import time
 import sys
 import urllib
 import urllib3
 import pandas as pd
-from src.fmpy import urls
-from src.fmpy import utils
+from fmpy import urls
+from fmpy import utils
 from datetime import datetime, timedelta
 
 
 class FmpClient:
 
     rate_limit = 300
```

### Comparing `fmpy_qi-0.1.0/src/fmpy/urls.py` & `fmpy_qi-0.1.1/src/fmpy/urls.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.0/src/fmpy/utils.py` & `fmpy_qi-0.1.1/src/fmpy/utils.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.0/src/fmpy_qi.egg-info/PKG-INFO` & `fmpy_qi-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fmpy-qi
-Version: 0.1.0
+Name: fmpy_qi
+Version: 0.1.1
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

