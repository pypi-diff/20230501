# Comparing `tmp/rankgun-2.0.5.tar.gz` & `tmp/rankgun-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankgun-2.0.5.tar", last modified: Sun Apr 30 22:29:04 2023, max compression
+gzip compressed data, was "rankgun-2.0.6.tar", last modified: Sun Apr 30 22:37:06 2023, max compression
```

## Comparing `rankgun-2.0.5.tar` & `rankgun-2.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:29:04.419171 rankgun-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35852 2023-04-30 22:28:47.000000 rankgun-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-30 22:29:04.419171 rankgun-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-30 22:28:47.000000 rankgun-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 22:28:47.000000 rankgun-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-30 22:29:04.419171 rankgun-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:29:04.415171 rankgun-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:29:04.415171 rankgun-2.0.5/src/rankgun/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-30 22:28:47.000000 rankgun-2.0.5/src/rankgun/__innit__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:29:04.419171 rankgun-2.0.5/src/rankgun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-30 22:29:04.000000 rankgun-2.0.5/src/rankgun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-30 22:29:04.000000 rankgun-2.0.5/src/rankgun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:29:04.000000 rankgun-2.0.5/src/rankgun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 22:29:04.000000 rankgun-2.0.5/src/rankgun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 22:29:04.000000 rankgun-2.0.5/src/rankgun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:29:04.419171 rankgun-2.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 22:28:47.000000 rankgun-2.0.5/tests/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:37:06.807125 rankgun-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35852 2023-04-30 22:36:38.000000 rankgun-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-30 22:37:06.807125 rankgun-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-30 22:36:38.000000 rankgun-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 22:36:38.000000 rankgun-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-30 22:37:06.807125 rankgun-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:37:06.803125 rankgun-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:37:06.803125 rankgun-2.0.6/src/rankgun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-30 22:36:38.000000 rankgun-2.0.6/src/rankgun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:37:06.807125 rankgun-2.0.6/src/rankgun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-30 22:37:06.000000 rankgun-2.0.6/src/rankgun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 22:37:06.000000 rankgun-2.0.6/src/rankgun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:37:06.000000 rankgun-2.0.6/src/rankgun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 22:37:06.000000 rankgun-2.0.6/src/rankgun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 22:37:06.000000 rankgun-2.0.6/src/rankgun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:37:06.807125 rankgun-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 22:36:38.000000 rankgun-2.0.6/tests/testing.py
```

### Comparing `rankgun-2.0.5/LICENSE` & `rankgun-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rankgun-2.0.5/PKG-INFO` & `rankgun-2.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: rankgun
-Version: 2.0.5
+Version: 2.0.6
 Summary: https://rankgun.works
 Home-page: https://rankgun.works
 Author: Noah-Haf
 Author-email: RobloxCookie_DevX@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# RankGun V2.0.5
+# RankGun V2.0.6
 
 An API wrapper for the RankGun API.
 
 Make for [rankgun](https://rankgun.works), read the [docs](https://docs.rankgun.works).
```

### Comparing `rankgun-2.0.5/setup.cfg` & `rankgun-2.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rankgun
-version = 2.0.5
+version = 2.0.6
 author = Noah-Haf
 author_email = RobloxCookie_DevX@outlook.com
 description = https://rankgun.works
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://rankgun.works
 classifiers =
```

### Comparing `rankgun-2.0.5/src/rankgun/__innit__.py` & `rankgun-2.0.6/src/rankgun/__init__.py`

 * *Files identical despite different names*

### Comparing `rankgun-2.0.5/src/rankgun.egg-info/PKG-INFO` & `rankgun-2.0.6/src/rankgun.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: rankgun
-Version: 2.0.5
+Version: 2.0.6
 Summary: https://rankgun.works
 Home-page: https://rankgun.works
 Author: Noah-Haf
 Author-email: RobloxCookie_DevX@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# RankGun V2.0.5
+# RankGun V2.0.6
 
 An API wrapper for the RankGun API.
 
 Make for [rankgun](https://rankgun.works), read the [docs](https://docs.rankgun.works).
```

### Comparing `rankgun-2.0.5/tests/testing.py` & `rankgun-2.0.6/tests/testing.py`

 * *Files identical despite different names*

