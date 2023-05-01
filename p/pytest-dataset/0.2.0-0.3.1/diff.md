# Comparing `tmp/pytest-dataset-0.2.0.tar.gz` & `tmp/pytest-dataset-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-dataset-0.2.0.tar", last modified: Mon Oct 10 14:09:25 2022, max compression
+gzip compressed data, was "pytest-dataset-0.3.1.tar", last modified: Mon May  1 08:57:34 2023, max compression
```

## Comparing `pytest-dataset-0.2.0.tar` & `pytest-dataset-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lavis      (501) staff       (20)        0 2022-10-10 14:09:25.886278 pytest-dataset-0.2.0/
--rw-r--r--   0 lavis      (501) staff       (20)      174 2022-09-05 11:03:22.000000 pytest-dataset-0.2.0/.gitignore
--rw-r--r--   0 lavis      (501) staff       (20)     1513 2022-09-05 08:23:52.000000 pytest-dataset-0.2.0/LICENSE
--rw-r--r--   0 lavis      (501) staff       (20)       16 2022-09-05 11:19:53.000000 pytest-dataset-0.2.0/MANIFEST.in
--rw-r--r--   0 lavis      (501) staff       (20)     6980 2022-10-10 14:09:25.886383 pytest-dataset-0.2.0/PKG-INFO
--rw-r--r--   0 lavis      (501) staff       (20)     5604 2022-09-05 11:07:56.000000 pytest-dataset-0.2.0/README.rst
-drwxr-xr-x   0 lavis      (501) staff       (20)        0 2022-10-10 14:09:25.886166 pytest-dataset-0.2.0/pytest_dataset.egg-info/
--rw-r--r--   0 lavis      (501) staff       (20)     6980 2022-10-10 14:09:25.000000 pytest-dataset-0.2.0/pytest_dataset.egg-info/PKG-INFO
--rw-r--r--   0 lavis      (501) staff       (20)      308 2022-10-10 14:09:25.000000 pytest-dataset-0.2.0/pytest_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 lavis      (501) staff       (20)        1 2022-10-10 14:09:25.000000 pytest-dataset-0.2.0/pytest_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 lavis      (501) staff       (20)       44 2022-10-10 14:09:25.000000 pytest-dataset-0.2.0/pytest_dataset.egg-info/entry_points.txt
--rw-r--r--   0 lavis      (501) staff       (20)       20 2022-10-10 14:09:25.000000 pytest-dataset-0.2.0/pytest_dataset.egg-info/requires.txt
--rw-r--r--   0 lavis      (501) staff       (20)       15 2022-10-10 14:09:25.000000 pytest-dataset-0.2.0/pytest_dataset.egg-info/top_level.txt
--rw-r--r--   0 lavis      (501) staff       (20)     9499 2022-10-10 13:52:38.000000 pytest-dataset-0.2.0/pytest_dataset.py
--rw-r--r--   0 lavis      (501) staff       (20)       67 2022-10-10 14:09:25.886761 pytest-dataset-0.2.0/setup.cfg
--rw-r--r--   0 lavis      (501) staff       (20)     2027 2022-09-05 11:20:25.000000 pytest-dataset-0.2.0/setup.py
+drwxr-xr-x   0 lavis      (501) staff       (20)        0 2023-05-01 08:57:34.333910 pytest-dataset-0.3.1/
+-rw-r--r--   0 lavis      (501) staff       (20)      174 2022-09-05 11:03:22.000000 pytest-dataset-0.3.1/.gitignore
+-rw-r--r--   0 lavis      (501) staff       (20)     1513 2022-09-05 08:23:52.000000 pytest-dataset-0.3.1/LICENSE
+-rw-r--r--   0 lavis      (501) staff       (20)       16 2022-09-05 11:19:53.000000 pytest-dataset-0.3.1/MANIFEST.in
+-rw-r--r--   0 lavis      (501) staff       (20)     7424 2023-05-01 08:57:34.333999 pytest-dataset-0.3.1/PKG-INFO
+-rw-r--r--   0 lavis      (501) staff       (20)     6048 2023-05-01 08:55:29.000000 pytest-dataset-0.3.1/README.rst
+drwxr-xr-x   0 lavis      (501) staff       (20)        0 2023-05-01 08:57:34.333793 pytest-dataset-0.3.1/pytest_dataset.egg-info/
+-rw-r--r--   0 lavis      (501) staff       (20)     7424 2023-05-01 08:57:34.000000 pytest-dataset-0.3.1/pytest_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 lavis      (501) staff       (20)      308 2023-05-01 08:57:34.000000 pytest-dataset-0.3.1/pytest_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 lavis      (501) staff       (20)        1 2023-05-01 08:57:34.000000 pytest-dataset-0.3.1/pytest_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 lavis      (501) staff       (20)       44 2023-05-01 08:57:34.000000 pytest-dataset-0.3.1/pytest_dataset.egg-info/entry_points.txt
+-rw-r--r--   0 lavis      (501) staff       (20)       20 2023-05-01 08:57:34.000000 pytest-dataset-0.3.1/pytest_dataset.egg-info/requires.txt
+-rw-r--r--   0 lavis      (501) staff       (20)       15 2023-05-01 08:57:34.000000 pytest-dataset-0.3.1/pytest_dataset.egg-info/top_level.txt
+-rw-r--r--   0 lavis      (501) staff       (20)    10359 2023-05-01 08:27:13.000000 pytest-dataset-0.3.1/pytest_dataset.py
+-rw-r--r--   0 lavis      (501) staff       (20)       67 2023-05-01 08:57:34.334277 pytest-dataset-0.3.1/setup.cfg
+-rw-r--r--   0 lavis      (501) staff       (20)     2027 2022-09-05 11:20:25.000000 pytest-dataset-0.3.1/setup.py
```

### Comparing `pytest-dataset-0.2.0/LICENSE` & `pytest-dataset-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-dataset-0.2.0/PKG-INFO` & `pytest-dataset-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dataset
-Version: 0.2.0
+Version: 0.3.1
 Summary: Plugin for loading different datasets for pytest by prefix from json or yaml files
 Home-page: https://github.com/Lavisx/pytest-dataset
 Author: Lavisx
 Author-email: lavis@seznam.cz
 License: BSD 3-Clause License
 Keywords: py.test resources files data directory directories dataset json yaml
 Platform: UNKNOWN
@@ -146,16 +146,32 @@
 since no other directory in the searched directory hierarchy contains
 the file. In other words, the ``tests/data/`` directory
 is the place for global (or fallback) resources.
 
 If a resource cannot be found in *any* of the searched directories, a
 `KeyError` is raised.
 
+.. _dataset_module:
+
+The dataset_module fixture
+--------------------------
+
+Similar to "dataset" only used for scope "module".
+The path, where are searched the dataset files are reduced to only possible for "module" scope.
+
 .. _dataset_copy:
 
+.. _dataset_class:
+
+The dataset_class fixture
+--------------------------
+
+Similar to "dataset" only used for scope "class".
+The path, where are searched the dataset files are reduced to only possible for "class" scope.
+
 The dataset_copy fixture
 ------------------------
 
 The "dataset_copy" fixture is similar to the dataset_ fixture, but copies the requested resources to a
 temporary directory first so that test functions or methods can modify their resources on-disk without affecting
 other test functions and methods.
```

### Comparing `pytest-dataset-0.2.0/README.rst` & `pytest-dataset-0.3.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -114,16 +114,32 @@
 since no other directory in the searched directory hierarchy contains
 the file. In other words, the ``tests/data/`` directory
 is the place for global (or fallback) resources.
 
 If a resource cannot be found in *any* of the searched directories, a
 `KeyError` is raised.
 
+.. _dataset_module:
+
+The dataset_module fixture
+--------------------------
+
+Similar to "dataset" only used for scope "module".
+The path, where are searched the dataset files are reduced to only possible for "module" scope.
+
 .. _dataset_copy:
 
+.. _dataset_class:
+
+The dataset_class fixture
+--------------------------
+
+Similar to "dataset" only used for scope "class".
+The path, where are searched the dataset files are reduced to only possible for "class" scope.
+
 The dataset_copy fixture
 ------------------------
 
 The "dataset_copy" fixture is similar to the dataset_ fixture, but copies the requested resources to a
 temporary directory first so that test functions or methods can modify their resources on-disk without affecting
 other test functions and methods.
```

### Comparing `pytest-dataset-0.2.0/pytest_dataset.egg-info/PKG-INFO` & `pytest-dataset-0.3.1/pytest_dataset.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dataset
-Version: 0.2.0
+Version: 0.3.1
 Summary: Plugin for loading different datasets for pytest by prefix from json or yaml files
 Home-page: https://github.com/Lavisx/pytest-dataset
 Author: Lavisx
 Author-email: lavis@seznam.cz
 License: BSD 3-Clause License
 Keywords: py.test resources files data directory directories dataset json yaml
 Platform: UNKNOWN
@@ -146,16 +146,32 @@
 since no other directory in the searched directory hierarchy contains
 the file. In other words, the ``tests/data/`` directory
 is the place for global (or fallback) resources.
 
 If a resource cannot be found in *any* of the searched directories, a
 `KeyError` is raised.
 
+.. _dataset_module:
+
+The dataset_module fixture
+--------------------------
+
+Similar to "dataset" only used for scope "module".
+The path, where are searched the dataset files are reduced to only possible for "module" scope.
+
 .. _dataset_copy:
 
+.. _dataset_class:
+
+The dataset_class fixture
+--------------------------
+
+Similar to "dataset" only used for scope "class".
+The path, where are searched the dataset files are reduced to only possible for "class" scope.
+
 The dataset_copy fixture
 ------------------------
 
 The "dataset_copy" fixture is similar to the dataset_ fixture, but copies the requested resources to a
 temporary directory first so that test functions or methods can modify their resources on-disk without affecting
 other test functions and methods.
```

### Comparing `pytest-dataset-0.2.0/pytest_dataset.py` & `pytest-dataset-0.3.1/pytest_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,34 +35,38 @@
 import yaml
 
 def pytest_addoption(parser):
     parser.addoption('--dataset-prefix', help='prefix file name for used dataset for example testing4net used as {prefix}_{name}.(yaml|json)')
     parser.addini('dataset_prefix', help='prefix file name for used dataset for example testing4net used as {prefix}_{name}.(yaml|json)')
 
 class _Dataset(object):
-    def __init__(self, request):
+    def __init__(self, request, scope="function"):
         basedir = request.fspath.dirpath()
         datadir = basedir.join("data")
         self._dataset_prefix = request.config.getoption('--dataset-prefix') or request.config.getini('dataset_prefix')
         if self._dataset_prefix:
             self._dataset_prefix = self._dataset_prefix +"_"
 
         self._datadirs = []
 
         for d in (basedir, datadir):
-            testdir = d.join(request.module.__name__)
-            if request.cls is not None:
-                clsdir = testdir.join(request.cls.__name__)
-                self._datadirs.extend([
-                    clsdir.join(request.function.__name__),
-                    clsdir
-                ])
-            else:
-                self._datadirs.append(testdir.join(request.function.__name__))
-            self._datadirs.append(testdir)
+            if scope in ("module", "class", "function"):
+                testdir = d.join(request.module.__name__)
+                if scope in ("class", "function"):
+                    if request.cls is not None:
+                        clsdir = testdir.join(request.cls.__name__)
+                        if scope == "function":
+                            self._datadirs.extend([
+                                clsdir.join(request.function.__name__),
+                                clsdir
+                            ])
+                    else:
+                        if scope == "function":
+                            self._datadirs.append(testdir.join(request.function.__name__))
+                self._datadirs.append(testdir)
         # add data dir to parent folders before rootdir
         for d in reversed(basedir.parts()):
             if d==request.config.rootdir:
                 break
             self._datadirs.append(d.join("data"))
 
     def __getitem__(self, path):
@@ -193,14 +197,29 @@
     is the place for global (or fallback) resources.
 
     If a resource cannot be found in *any* of the searched directories, a
     :class:`KeyError` is raised.
     """
     return _Dataset(request)
 
+@pytest.fixture(scope="module")
+def dataset_module(request):
+    """
+    Similar to dataset only used for scope `module`.
+    The path, where are searched the dataset files are reduced to only possible for `module` scope.
+    """
+    return _Dataset(request, scope="module")
+
+@pytest.fixture(scope="class")
+def dataset_class(request):
+    """
+    Similar to dataset only used for scope `class`.
+    The path, where are searched the dataset files are reduced to only possible for `class` scope.
+    """
+    return _Dataset(request, scope="class")
 
 @pytest.fixture
 def dataset_copy(request, tmpdir):
     """
     Similar to the :func:`.dataset` fixture, but copies the requested resources to a temporary directory first so that
     test functions or methods can modify their resources on-disk without affecting other test functions
     and methods.
```

### Comparing `pytest-dataset-0.2.0/setup.py` & `pytest-dataset-0.3.1/setup.py`

 * *Files identical despite different names*

