# Comparing `tmp/asytest-0.1.2.tar.gz` & `tmp/asytest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asytest-0.1.2.tar", last modified: Mon May  1 17:44:53 2023, max compression
+gzip compressed data, was "asytest-0.1.3.tar", last modified: Mon May  1 18:02:40 2023, max compression
```

## Comparing `asytest-0.1.2.tar` & `asytest-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.732447 asytest-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.728447 asytest-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.728447 asytest-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 17:44:28.000000 asytest-0.1.2/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 17:44:28.000000 asytest-0.1.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 17:44:28.000000 asytest-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 17:44:28.000000 asytest-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 17:44:53.732447 asytest-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 17:44:28.000000 asytest-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 17:44:28.000000 asytest-0.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.728447 asytest-0.1.2/example_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 17:44:28.000000 asytest-0.1.2/example_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-01 17:44:28.000000 asytest-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 17:44:28.000000 asytest-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:44:53.732447 asytest-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.728447 asytest-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.732447 asytest-0.1.2/src/asytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:28.000000 asytest-0.1.2/src/asytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 17:44:28.000000 asytest-0.1.2/src/asytest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 17:44:53.000000 asytest-0.1.2/src/asytest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-01 17:44:28.000000 asytest-0.1.2/src/asytest/asytest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.732447 asytest-0.1.2/src/asytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 17:44:53.000000 asytest-0.1.2/src/asytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 17:44:53.000000 asytest-0.1.2/src/asytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:44:53.000000 asytest-0.1.2/src/asytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 17:44:53.000000 asytest-0.1.2/src/asytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 17:44:53.000000 asytest-0.1.2/src/asytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:44:53.732447 asytest-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 17:44:28.000000 asytest-0.1.2/tests/test_asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.065968 asytest-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.069968 asytest-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 18:02:22.000000 asytest-0.1.3/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 18:02:22.000000 asytest-0.1.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 18:02:22.000000 asytest-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 18:02:22.000000 asytest-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 18:02:40.073968 asytest-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 18:02:22.000000 asytest-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 18:02:22.000000 asytest-0.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.069968 asytest-0.1.3/example_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 18:02:22.000000 asytest-0.1.3/example_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-01 18:02:22.000000 asytest-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 18:02:22.000000 asytest-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:02:40.073968 asytest-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.069968 asytest-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/src/asytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:22.000000 asytest-0.1.3/src/asytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-01 18:02:22.000000 asytest-0.1.3/src/asytest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 18:02:39.000000 asytest-0.1.3/src/asytest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-01 18:02:22.000000 asytest-0.1.3/src/asytest/asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/src/asytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 18:02:22.000000 asytest-0.1.3/tests/test_asytest.py
```

### Comparing `asytest-0.1.2/.github/workflows/build.yaml` & `asytest-0.1.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/.github/workflows/release.yaml` & `asytest-0.1.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/LICENSE` & `asytest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/PKG-INFO` & `asytest-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asytest-0.1.2/dev-requirements.txt` & `asytest-0.1.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/example_tests/test_dummy.py` & `asytest-0.1.3/example_tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/pyproject.toml` & `asytest-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/src/asytest/asytest.py` & `asytest-0.1.3/src/asytest/asytest.py`

 * *Files identical despite different names*

### Comparing `asytest-0.1.2/src/asytest.egg-info/PKG-INFO` & `asytest-0.1.3/src/asytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

