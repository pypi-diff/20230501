# Comparing `tmp/qm_tools_aw-1.0.0.tar.gz` & `tmp/qm_tools_aw-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm_tools_aw-1.0.0.tar", last modified: Fri Feb 24 20:26:25 2023, max compression
+gzip compressed data, was "qm_tools_aw-1.0.1.tar", last modified: Mon May  1 14:11:00 2023, max compression
```

## Comparing `qm_tools_aw-1.0.0.tar` & `qm_tools_aw-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:26:25.857181 qm_tools_aw-1.0.0/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     1074 2023-01-17 19:48:33.000000 qm_tools_aw-1.0.0/LICENSE
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-02-24 20:26:25.858181 qm_tools_aw-1.0.0/PKG-INFO
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      107 2023-01-17 19:48:33.000000 qm_tools_aw-1.0.0/README.md
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      649 2023-02-24 20:26:08.000000 qm_tools_aw-1.0.0/pyproject.toml
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      189 2023-02-24 20:26:25.860181 qm_tools_aw-1.0.0/setup.cfg
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:26:25.833181 qm_tools_aw-1.0.0/src/
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:26:25.845181 qm_tools_aw-1.0.0/src/qm_tools_aw/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        0 2023-01-18 18:59:42.000000 qm_tools_aw-1.0.0/src/qm_tools_aw/__init__.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     4102 2023-02-21 19:03:02.000000 qm_tools_aw-1.0.0/src/qm_tools_aw/tools.py
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:26:25.856181 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      689 2023-02-24 20:26:25.000000 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/PKG-INFO
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      323 2023-02-24 20:26:25.000000 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/SOURCES.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-02-24 20:26:25.000000 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/dependency_links.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       20 2023-02-24 20:26:25.000000 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/requires.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       12 2023-02-24 20:26:25.000000 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/top_level.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-01-18 18:58:47.000000 qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/zip-safe
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.382060 qm_tools_aw-1.0.1/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/LICENSE
+-rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-01 14:11:00.382150 qm_tools_aw-1.0.1/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      107 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/README.md
+-rw-r--r--   0 austinwallace   (501) staff       (20)      649 2023-05-01 14:10:54.000000 qm_tools_aw-1.0.1/pyproject.toml
+-rw-r--r--   0 austinwallace   (501) staff       (20)      202 2023-05-01 14:11:00.382521 qm_tools_aw-1.0.1/setup.cfg
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.378329 qm_tools_aw-1.0.1/src/
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.379927 qm_tools_aw-1.0.1/src/qm_tools_aw/
+-rw-r--r--   0 austinwallace   (501) staff       (20)       20 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/src/qm_tools_aw/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     6177 2023-03-27 20:06:41.000000 qm_tools_aw-1.0.1/src/qm_tools_aw/tools.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:11:00.381823 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      689 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      323 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/SOURCES.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/dependency_links.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       32 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/requires.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       12 2023-05-01 14:11:00.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/top_level.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-03-27 20:27:35.000000 qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/zip-safe
```

### Comparing `qm_tools_aw-1.0.0/LICENSE` & `qm_tools_aw-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qm_tools_aw-1.0.0/PKG-INFO` & `qm_tools_aw-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm_tools_aw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qm_tools_aw-1.0.0/pyproject.toml` & `qm_tools_aw-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qm_tools_aw"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Provides some functions that I have found value in reusing for quantum chemistry related tasks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qm_tools_aw-1.0.0/src/qm_tools_aw.egg-info/PKG-INFO` & `qm_tools_aw-1.0.1/src/qm_tools_aw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-tools-aw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provides some functions that I have found value in reusing for quantum chemistry related tasks.
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/qm_tools
 Project-URL: Bug Tracker, https://github.com/Awallace3/qm_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

