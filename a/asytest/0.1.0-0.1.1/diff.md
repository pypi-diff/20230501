# Comparing `tmp/asytest-0.1.0.tar.gz` & `tmp/asytest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asytest-0.1.0.tar", last modified: Mon May  1 17:21:28 2023, max compression
+gzip compressed data, was "asytest-0.1.1.tar", last modified: Mon May  1 17:36:59 2023, max compression
```

## Comparing `asytest-0.1.0.tar` & `asytest-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 17:21:05.000000 asytest-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 17:21:05.000000 asytest-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 17:21:05.000000 asytest-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 17:21:05.000000 asytest-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 17:21:28.627219 asytest-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 17:21:05.000000 asytest-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 17:21:05.000000 asytest-0.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/example_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 17:21:05.000000 asytest-0.1.0/example_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 17:21:05.000000 asytest-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 17:21:05.000000 asytest-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:21:28.627219 asytest-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 17:21:28.000000 asytest-0.1.0/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/src/asytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 17:21:28.000000 asytest-0.1.0/src/asytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-01 17:21:28.000000 asytest-0.1.0/src/asytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:21:28.000000 asytest-0.1.0/src/asytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 17:21:28.000000 asytest-0.1.0/src/asytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 17:21:28.000000 asytest-0.1.0/src/asytest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-01 17:21:05.000000 asytest-0.1.0/src/atest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:28.627219 asytest-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 17:21:05.000000 asytest-0.1.0/tests/test_asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.244654 asytest-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 17:36:40.000000 asytest-0.1.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 17:36:40.000000 asytest-0.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 17:36:40.000000 asytest-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 17:36:40.000000 asytest-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 17:36:59.248654 asytest-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 17:36:40.000000 asytest-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 17:36:40.000000 asytest-0.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/example_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 17:36:40.000000 asytest-0.1.1/example_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-01 17:36:40.000000 asytest-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 17:36:40.000000 asytest-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:36:59.248654 asytest-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/src/asytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:40.000000 asytest-0.1.1/src/asytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 17:36:59.000000 asytest-0.1.1/src/asytest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-01 17:36:40.000000 asytest-0.1.1/src/asytest/asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/src/asytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 17:36:59.000000 asytest-0.1.1/src/asytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 17:36:59.000000 asytest-0.1.1/src/asytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:36:59.000000 asytest-0.1.1/src/asytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 17:36:59.000000 asytest-0.1.1/src/asytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 17:36:59.000000 asytest-0.1.1/src/asytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:36:59.248654 asytest-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 17:36:40.000000 asytest-0.1.1/tests/test_asytest.py
```

### Comparing `asytest-0.1.0/.github/workflows/build.yaml` & `asytest-0.1.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.0/.github/workflows/release.yaml` & `asytest-0.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.0/LICENSE` & `asytest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asytest-0.1.0/PKG-INFO` & `asytest-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asytest-0.1.0/dev-requirements.txt` & `asytest-0.1.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `asytest-0.1.0/example_tests/test_dummy.py` & `asytest-0.1.1/example_tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `asytest-0.1.0/pyproject.toml` & `asytest-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,12 +18,12 @@
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "pip-tools"]
 
 [tool.setuptools_scm]
-write_to = "src/_version.py"
+write_to = "src/asytest/_version.py"
 
 [project.urls]
 "Homepage" = "https://github.com/pavradev/asytest"
 "Bug Tracker" = "https://github.com/pavradev/asytest/issues"
```

### Comparing `asytest-0.1.0/src/asytest.egg-info/PKG-INFO` & `asytest-0.1.1/src/asytest.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asytest-0.1.0/src/atest.py` & `asytest-0.1.1/src/asytest/asytest.py`

 * *Files identical despite different names*

