# Comparing `tmp/wikiserieswillemlib-0.1.0.tar.gz` & `tmp/wikiserieswillemlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiserieswillemlib-0.1.0.tar", last modified: Mon May  1 07:33:22 2023, max compression
+gzip compressed data, was "wikiserieswillemlib-0.2.0.tar", last modified: Mon May  1 08:34:41 2023, max compression
```

## Comparing `wikiserieswillemlib-0.1.0.tar` & `wikiserieswillemlib-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 willem.kuipers   (502) staff       (20)        0 2023-05-01 07:33:22.066617 wikiserieswillemlib-0.1.0/
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)        5 2023-05-01 07:26:49.000000 wikiserieswillemlib-0.1.0/.VERSION
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      160 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/AUTHORS.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     1287 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/CONTRIBUTING.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      161 2023-05-01 07:27:03.000000 wikiserieswillemlib-0.1.0/HISTORY.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     1061 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/LICENSE
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      412 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/MANIFEST.in
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     3013 2023-05-01 07:33:22.066753 wikiserieswillemlib-0.1.0/PKG-INFO
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      508 2023-05-01 07:20:07.000000 wikiserieswillemlib-0.1.0/Pipfile
--rw-r--r--   0 willem.kuipers   (502) staff       (20)    67627 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/Pipfile.lock
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     2319 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/README.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      949 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/USAGE.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      588 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/dev-requirements.txt
-drwxr-xr-x   0 willem.kuipers   (502) staff       (20)        0 2023-05-01 07:33:22.030248 wikiserieswillemlib-0.1.0/docs/
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     6814 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/Makefile
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)       28 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/authors.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     9040 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/conf.py
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)       33 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/contributing.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)       28 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/history.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      531 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/index.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)       33 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/installation.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)       27 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/readme.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)       26 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/docs/usage.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      361 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/requirements.txt
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      159 2023-05-01 07:33:22.069009 wikiserieswillemlib-0.1.0/setup.cfg
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     1956 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/setup.py
-drwxr-xr-x   0 willem.kuipers   (502) staff       (20)        0 2023-05-01 07:33:22.031091 wikiserieswillemlib-0.1.0/tests/
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     2261 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/tests/test_wikiserieswillemlib.py
-drwxr-xr-x   0 willem.kuipers   (502) staff       (20)        0 2023-05-01 07:33:22.059984 wikiserieswillemlib-0.1.0/wikiserieswillemlib/
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)        5 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/.VERSION
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      160 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/AUTHORS.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     1287 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/CONTRIBUTING.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)      161 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/HISTORY.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     1061 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/LICENSE
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      508 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/Pipfile
--rw-r--r--   0 willem.kuipers   (502) staff       (20)    67627 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/Pipfile.lock
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     2319 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/README.rst
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      949 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/USAGE.rst
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     1801 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/__init__.py
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     2186 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/_version.py
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      588 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/dev-requirements.txt
--rw-r--r--   0 willem.kuipers   (502) staff       (20)      361 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/requirements.txt
--rwxr-xr-x   0 willem.kuipers   (502) staff       (20)     2970 2023-05-01 07:29:35.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/wikiserieswillemlib.py
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     1713 2023-05-01 07:12:53.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib/wikiserieswillemlibexceptions.py
-drwxr-xr-x   0 willem.kuipers   (502) staff       (20)        0 2023-05-01 07:33:22.066145 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     3013 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/PKG-INFO
--rw-r--r--   0 willem.kuipers   (502) staff       (20)     1127 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/SOURCES.txt
--rw-r--r--   0 willem.kuipers   (502) staff       (20)        1 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/dependency_links.txt
--rw-r--r--   0 willem.kuipers   (502) staff       (20)        1 2023-05-01 07:31:37.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/not-zip-safe
--rw-r--r--   0 willem.kuipers   (502) staff       (20)       28 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/requires.txt
--rw-r--r--   0 willem.kuipers   (502) staff       (20)       20 2023-05-01 07:33:21.000000 wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:34:41.410454 wikiserieswillemlib-0.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-01 08:34:41.410454 wikiserieswillemlib-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    77168 2023-05-01 08:34:40.000000 wikiserieswillemlib-0.2.0/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2319 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/USAGE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:34:41.406453 wikiserieswillemlib-0.2.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9040 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-05-01 08:34:41.410454 wikiserieswillemlib-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1956 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:34:41.406453 wikiserieswillemlib-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/tests/test_wikiserieswillemlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:34:41.406453 wikiserieswillemlib-0.2.0/wikiserieswillemlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      160 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    77168 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2319 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2970 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/wikiserieswillemlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-01 08:33:14.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib/wikiserieswillemlibexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:34:41.406453 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 08:34:41.000000 wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/top_level.txt
```

### Comparing `wikiserieswillemlib-0.1.0/CONTRIBUTING.rst` & `wikiserieswillemlib-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/LICENSE` & `wikiserieswillemlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/PKG-INFO` & `wikiserieswillemlib-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikiserieswillemlib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library for parsing Wiki series
 Home-page: https://github.com/wmkuipers/wikiserieswillemlib
 Author: Willem Kuipers
 Author-email: willem@kuipers.co.uk
 License: MIT
 Keywords: wikiserieswillemlib
 Classifier: Development Status :: 3 - Alpha
@@ -96,7 +96,13 @@
 * First code creation
 
 
 0.1.0 (01-05-2023)
 ------------------
 
 * Initial code release
+
+
+0.2.0 (01-05-2023)
+------------------
+
+* Fix dependencies
```

### Comparing `wikiserieswillemlib-0.1.0/Pipfile.lock` & `wikiserieswillemlib-0.2.0/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.956030701754386%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'19fb07706ef198e6795109a9653ec474b400bb7cbeb32c19feb0441e2a13c80b'}, 'requires': "*

 * *            "{replace: OrderedDict([('python_full_version', '3.9.15'), ('python_version', "*

 * *            "'3.9')])}}",*

 * * "'develop'": '{\'dill\': {\'markers\': "python_version < \'3.11\'"}, \'importlib-metadata\': '*

 * *              '{\'markers\': "python_version < \'3.10\'"}, \'wrapt\': {\'markers\': '*

 * *              '"python_version < \'3.11\'"}, \'cffi\': OrderedDict([(\'hashes\',  […]*

```diff
@@ -1,14 +1,17 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "ed6448431ec0ef13ead82c632c14f5c93b9064cdaaaa759e9bfdee0503fbd17b"
+            "sha256": "19fb07706ef198e6795109a9653ec474b400bb7cbeb32c19feb0441e2a13c80b"
         },
         "pipfile-spec": 6,
-        "requires": {},
+        "requires": {
+            "python_full_version": "3.9.15",
+            "python_version": "3.9"
+        },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
                 "verify_ssl": true
             }
         ]
@@ -212,14 +215,83 @@
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2022.12.7"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
         "chardet": {
             "hashes": [
                 "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
                 "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.1.0"
@@ -374,20 +446,45 @@
                 "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
                 "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
                 "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "index": "pypi",
             "version": "==7.2.5"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==40.0.2"
+        },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
@@ -487,15 +584,15 @@
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
                 "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
                 "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.10'",
             "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
@@ -506,14 +603,22 @@
             "hashes": [
                 "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
                 "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.2.3"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
@@ -732,14 +837,21 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
+                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+            ],
+            "version": "==2.21"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -893,14 +1005,22 @@
             "hashes": [
                 "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
                 "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.3.5"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "semver": {
             "hashes": [
                 "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4",
                 "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"
             ],
             "index": "pypi",
             "version": "==2.13.0"
@@ -1019,14 +1139,22 @@
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "tomlkit": {
             "hashes": [
                 "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
                 "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.8"
@@ -1043,14 +1171,22 @@
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
+                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==4.5.0"
+        },
         "urllib3": {
             "hashes": [
                 "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.15"
@@ -1144,15 +1280,15 @@
                 "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
                 "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
                 "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
                 "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
                 "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==1.15.0"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
```

### Comparing `wikiserieswillemlib-0.1.0/README.rst` & `wikiserieswillemlib-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/USAGE.rst` & `wikiserieswillemlib-0.2.0/USAGE.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/dev-requirements.txt` & `wikiserieswillemlib-0.2.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/docs/Makefile` & `wikiserieswillemlib-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/docs/conf.py` & `wikiserieswillemlib-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/docs/index.rst` & `wikiserieswillemlib-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/setup.py` & `wikiserieswillemlib-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/tests/test_wikiserieswillemlib.py` & `wikiserieswillemlib-0.2.0/tests/test_wikiserieswillemlib.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/CONTRIBUTING.rst` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/LICENSE` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/Pipfile.lock` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.956030701754386%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'19fb07706ef198e6795109a9653ec474b400bb7cbeb32c19feb0441e2a13c80b'}, 'requires': "*

 * *            "{replace: OrderedDict([('python_full_version', '3.9.15'), ('python_version', "*

 * *            "'3.9')])}}",*

 * * "'develop'": '{\'dill\': {\'markers\': "python_version < \'3.11\'"}, \'importlib-metadata\': '*

 * *              '{\'markers\': "python_version < \'3.10\'"}, \'wrapt\': {\'markers\': '*

 * *              '"python_version < \'3.11\'"}, \'cffi\': OrderedDict([(\'hashes\',  […]*

```diff
@@ -1,14 +1,17 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "ed6448431ec0ef13ead82c632c14f5c93b9064cdaaaa759e9bfdee0503fbd17b"
+            "sha256": "19fb07706ef198e6795109a9653ec474b400bb7cbeb32c19feb0441e2a13c80b"
         },
         "pipfile-spec": 6,
-        "requires": {},
+        "requires": {
+            "python_full_version": "3.9.15",
+            "python_version": "3.9"
+        },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
                 "verify_ssl": true
             }
         ]
@@ -212,14 +215,83 @@
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2022.12.7"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
         "chardet": {
             "hashes": [
                 "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
                 "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.1.0"
@@ -374,20 +446,45 @@
                 "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
                 "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
                 "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "index": "pypi",
             "version": "==7.2.5"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==40.0.2"
+        },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
@@ -487,15 +584,15 @@
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
                 "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
                 "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.10'",
             "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
@@ -506,14 +603,22 @@
             "hashes": [
                 "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
                 "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.2.3"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
@@ -732,14 +837,21 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
+                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+            ],
+            "version": "==2.21"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -893,14 +1005,22 @@
             "hashes": [
                 "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
                 "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.3.5"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "semver": {
             "hashes": [
                 "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4",
                 "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"
             ],
             "index": "pypi",
             "version": "==2.13.0"
@@ -1019,14 +1139,22 @@
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "tomlkit": {
             "hashes": [
                 "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
                 "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.8"
@@ -1043,14 +1171,22 @@
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
+                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==4.5.0"
+        },
         "urllib3": {
             "hashes": [
                 "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.15"
@@ -1144,15 +1280,15 @@
                 "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
                 "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
                 "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
                 "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
                 "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==1.15.0"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
```

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/README.rst` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/README.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/USAGE.rst` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/__init__.py` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/__init__.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/_version.py` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/_version.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/dev-requirements.txt` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/wikiserieswillemlib.py` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/wikiserieswillemlib.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib/wikiserieswillemlibexceptions.py` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib/wikiserieswillemlibexceptions.py`

 * *Files identical despite different names*

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/PKG-INFO` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikiserieswillemlib
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library for parsing Wiki series
 Home-page: https://github.com/wmkuipers/wikiserieswillemlib
 Author: Willem Kuipers
 Author-email: willem@kuipers.co.uk
 License: MIT
 Keywords: wikiserieswillemlib
 Classifier: Development Status :: 3 - Alpha
@@ -96,7 +96,13 @@
 * First code creation
 
 
 0.1.0 (01-05-2023)
 ------------------
 
 * Initial code release
+
+
+0.2.0 (01-05-2023)
+------------------
+
+* Fix dependencies
```

### Comparing `wikiserieswillemlib-0.1.0/wikiserieswillemlib.egg-info/SOURCES.txt` & `wikiserieswillemlib-0.2.0/wikiserieswillemlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

