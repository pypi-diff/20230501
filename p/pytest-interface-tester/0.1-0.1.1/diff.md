# Comparing `tmp/pytest-interface-tester-0.1.tar.gz` & `tmp/pytest-interface-tester-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-interface-tester-0.1.tar", last modified: Mon May  1 14:39:44 2023, max compression
+gzip compressed data, was "pytest-interface-tester-0.1.1.tar", last modified: Mon May  1 15:01:12 2023, max compression
```

## Comparing `pytest-interface-tester-0.1.tar` & `pytest-interface-tester-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxr-x   0 pietro    (1000) pietro    (1000)        0 2023-05-01 14:39:44.700835 pytest-interface-tester-0.1/
--rw-rw-r--   0 pietro    (1000) pietro    (1000)       53 2023-04-18 15:14:12.000000 pytest-interface-tester-0.1/.gitignore
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     6503 2023-05-01 14:39:44.700835 pytest-interface-tester-0.1/PKG-INFO
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     5394 2023-04-17 07:44:08.000000 pytest-interface-tester-0.1/README.md
-drwxrwxr-x   0 pietro    (1000) pietro    (1000)        0 2023-05-01 14:39:44.696835 pytest-interface-tester-0.1/interface_tester/
--rw-rw-r--   0 pietro    (1000) pietro    (1000)      328 2023-04-24 08:38:16.000000 pytest-interface-tester-0.1/interface_tester/__init__.py
-drwxrwxr-x   0 pietro    (1000) pietro    (1000)        0 2023-05-01 14:39:44.696835 pytest-interface-tester-0.1/interface_tester/cli/
--rw-rw-r--   0 pietro    (1000) pietro    (1000)        0 2023-04-05 11:39:18.000000 pytest-interface-tester-0.1/interface_tester/cli/__init__.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     2822 2023-04-24 08:37:54.000000 pytest-interface-tester-0.1/interface_tester/cli/discover.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)      372 2023-04-05 14:42:38.000000 pytest-interface-tester-0.1/interface_tester/cli/main.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)    10808 2023-04-24 08:37:59.000000 pytest-interface-tester-0.1/interface_tester/collector.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)      515 2023-04-24 13:55:20.000000 pytest-interface-tester-0.1/interface_tester/errors.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     6920 2023-04-24 08:33:04.000000 pytest-interface-tester-0.1/interface_tester/interface_test.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)    19445 2023-04-24 14:22:57.000000 pytest-interface-tester-0.1/interface_tester/plugin.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     4812 2023-04-24 14:34:31.000000 pytest-interface-tester-0.1/interface_tester/runner.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     1573 2023-04-05 14:44:33.000000 pytest-interface-tester-0.1/interface_tester/schema_base.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     2687 2023-04-24 08:30:55.000000 pytest-interface-tester-0.1/pyproject.toml
-drwxrwxr-x   0 pietro    (1000) pietro    (1000)        0 2023-05-01 14:39:44.700835 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     6503 2023-05-01 14:39:44.000000 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/PKG-INFO
--rw-rw-r--   0 pietro    (1000) pietro    (1000)      707 2023-05-01 14:39:44.000000 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/SOURCES.txt
--rw-rw-r--   0 pietro    (1000) pietro    (1000)        1 2023-05-01 14:39:44.000000 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/dependency_links.txt
--rw-rw-r--   0 pietro    (1000) pietro    (1000)      116 2023-05-01 14:39:44.000000 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/entry_points.txt
--rw-rw-r--   0 pietro    (1000) pietro    (1000)       35 2023-05-01 14:39:44.000000 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/requires.txt
--rw-rw-r--   0 pietro    (1000) pietro    (1000)       17 2023-05-01 14:39:44.000000 pytest-interface-tester-0.1/pytest_interface_tester.egg-info/top_level.txt
--rw-rw-r--   0 pietro    (1000) pietro    (1000)       38 2023-05-01 14:39:44.700835 pytest-interface-tester-0.1/setup.cfg
-drwxrwxr-x   0 pietro    (1000) pietro    (1000)        0 2023-05-01 14:39:44.696835 pytest-interface-tester-0.1/tests/
-drwxrwxr-x   0 pietro    (1000) pietro    (1000)        0 2023-05-01 14:39:44.700835 pytest-interface-tester-0.1/tests/unit/
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     4027 2023-04-24 08:29:24.000000 pytest-interface-tester-0.1/tests/unit/test_collect_interface_tests.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)     3397 2023-04-24 08:37:29.000000 pytest-interface-tester-0.1/tests/unit/test_collect_schemas.py
--rw-rw-r--   0 pietro    (1000) pietro    (1000)      801 2023-04-05 14:44:32.000000 pytest-interface-tester-0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.494055 pytest-interface-tester-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.494055 pytest-interface-tester-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/interface_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/interface_tester/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/cli/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/interface_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/schema_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.494055 pytest-interface-tester-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/tests/unit/test_collect_interface_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/tests/unit/test_collect_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/tox.ini
```

### Comparing `pytest-interface-tester-0.1/PKG-INFO` & `pytest-interface-tester-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-interface-tester
-Version: 0.1
+Version: 0.1.1
 Summary: Pytest plugin for checking charm relation interface protocol compliance.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/interface-tester-pytest
 Keywords: juju,relation interfaces
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

### Comparing `pytest-interface-tester-0.1/README.md` & `pytest-interface-tester-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/cli/discover.py` & `pytest-interface-tester-0.1.1/interface_tester/cli/discover.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/collector.py` & `pytest-interface-tester-0.1.1/interface_tester/collector.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/errors.py` & `pytest-interface-tester-0.1.1/interface_tester/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/interface_test.py` & `pytest-interface-tester-0.1.1/interface_tester/interface_test.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/plugin.py` & `pytest-interface-tester-0.1.1/interface_tester/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/runner.py` & `pytest-interface-tester-0.1.1/interface_tester/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/interface_tester/schema_base.py` & `pytest-interface-tester-0.1.1/interface_tester/schema_base.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/pyproject.toml` & `pytest-interface-tester-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pytest-interface-tester"
 
-version = "0.1"
+version = "0.1.1"
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" },
 ]
 description = "Pytest plugin for checking charm relation interface protocol compliance."
 license.text = "Apache-2.0"
 keywords = ["juju", "relation interfaces"]
```

### Comparing `pytest-interface-tester-0.1/pytest_interface_tester.egg-info/PKG-INFO` & `pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-interface-tester
-Version: 0.1
+Version: 0.1.1
 Summary: Pytest plugin for checking charm relation interface protocol compliance.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/interface-tester-pytest
 Keywords: juju,relation interfaces
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

### Comparing `pytest-interface-tester-0.1/pytest_interface_tester.egg-info/SOURCES.txt` & `pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 .gitignore
 README.md
 pyproject.toml
 tox.ini
+.github/workflows/build_wheels.yaml
+.github/workflows/quality_checks.yaml
 interface_tester/__init__.py
 interface_tester/collector.py
 interface_tester/errors.py
 interface_tester/interface_test.py
 interface_tester/plugin.py
 interface_tester/runner.py
 interface_tester/schema_base.py
```

### Comparing `pytest-interface-tester-0.1/tests/unit/test_collect_interface_tests.py` & `pytest-interface-tester-0.1.1/tests/unit/test_collect_interface_tests.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/tests/unit/test_collect_schemas.py` & `pytest-interface-tester-0.1.1/tests/unit/test_collect_schemas.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1/tox.ini` & `pytest-interface-tester-0.1.1/tox.ini`

 * *Files identical despite different names*

