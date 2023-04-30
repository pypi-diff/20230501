# Comparing `tmp/pytest_oar-1.3.1.tar.gz` & `tmp/pytest_oar-2.0.0.tar.gz`

## Comparing `pytest_oar-1.3.1.tar` & `pytest_oar-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/requirements.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/setup.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/client.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/config.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/consts.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/plugin.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/report.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/oar/result.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/.gitignore
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/README.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 pytest_oar-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/requirements.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/setup.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/__init__.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/client.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/config.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/consts.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/plugin.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/report.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/oar/result.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/.gitignore
+-rw-r--r--   0        0        0    10939 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11576 2020-02-02 00:00:00.000000 pytest_oar-2.0.0/PKG-INFO
```

### Comparing `pytest_oar-1.3.1/oar/config.py` & `pytest_oar-2.0.0/oar/config.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-1.3.1/oar/consts.py` & `pytest_oar-2.0.0/oar/consts.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-1.3.1/oar/plugin.py` & `pytest_oar-2.0.0/oar/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-1.3.1/oar/report.py` & `pytest_oar-2.0.0/oar/report.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-1.3.1/README.md` & `pytest_oar-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,14 @@
 ```
 
 Result:
 ```
 collected 1 item                                                                                                                                               
 
 test_example.py .
-============OAR SUMMARY===============
-Passed IDs: [0]
-Failed IDs: []
-Tests that need analysis: []
-Tests that need resolution: []
-======================================
-
 
 ====================================================================== 1 passed in 0.00s =======================================================================
 ```
 Not necessarily the most helpful on its own.
 
 In the current working directory, there is a new folder, by default titled **oar-results**:
```

### Comparing `pytest_oar-1.3.1/pyproject.toml` & `pytest_oar-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-oar"
-version = "1.3.1"
+version = "2.0.0"
 description = "PyTest plugin for the OAR testing framework"
 license = "MIT"
 authors = [
   { name="Ryan de Marigny", email="ryandemarigny@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `pytest_oar-1.3.1/PKG-INFO` & `pytest_oar-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-oar
-Version: 1.3.1
+Version: 2.0.0
 Summary: PyTest plugin for the OAR testing framework
 Project-URL: Homepage, https://github.com/ryandem1/oar
 Project-URL: Bug Tracker, https://github.com/ryandem1/oar/issues
 Author-email: Ryan de Marigny <ryandemarigny@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,21 +64,14 @@
 ```
 
 Result:
 ```
 collected 1 item                                                                                                                                               
 
 test_example.py .
-============OAR SUMMARY===============
-Passed IDs: [0]
-Failed IDs: []
-Tests that need analysis: []
-Tests that need resolution: []
-======================================
-
 
 ====================================================================== 1 passed in 0.00s =======================================================================
 ```
 Not necessarily the most helpful on its own.
 
 In the current working directory, there is a new folder, by default titled **oar-results**:
```

