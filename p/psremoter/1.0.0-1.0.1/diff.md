# Comparing `tmp/psremoter-1.0.0.tar.gz` & `tmp/psremoter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psremoter-1.0.0.tar", last modified: Mon May  1 10:33:43 2023, max compression
+gzip compressed data, was "psremoter-1.0.1.tar", last modified: Mon May  1 10:51:42 2023, max compression
```

## Comparing `psremoter-1.0.0.tar` & `psremoter-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:33:43.662789 psremoter-1.0.0/
--rw-rw-rw-   0        0        0     1422 2023-05-01 10:33:43.662789 psremoter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      823 2023-05-01 08:55:38.000000 psremoter-1.0.0/README.md
--rw-rw-rw-   0        0        0      877 2023-05-01 10:30:14.000000 psremoter-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      666 2023-05-01 10:33:43.664788 psremoter-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 10:33:43.633806 psremoter-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 10:33:43.658791 psremoter-1.0.0/src/PSRemoter.egg-info/
--rw-rw-rw-   0        0        0     1422 2023-05-01 10:33:43.000000 psremoter-1.0.0/src/PSRemoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-05-01 10:33:43.000000 psremoter-1.0.0/src/PSRemoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:33:43.000000 psremoter-1.0.0/src/PSRemoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-05-01 10:33:43.000000 psremoter-1.0.0/src/PSRemoter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:33:43.000000 psremoter-1.0.0/src/PSRemoter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 10:33:43.661790 psremoter-1.0.0/tests/
--rw-rw-rw-   0        0        0      541 2023-05-01 08:55:38.000000 psremoter-1.0.0/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:51:42.216030 psremoter-1.0.1/
+-rw-rw-rw-   0        0        0     1345 2023-05-01 10:51:42.215031 psremoter-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      823 2023-05-01 08:55:38.000000 psremoter-1.0.1/README.md
+-rw-rw-rw-   0        0        0      879 2023-05-01 10:49:55.000000 psremoter-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:51:42.216030 psremoter-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 10:51:42.170057 psremoter-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 10:51:42.211034 psremoter-1.0.1/src/PSRemoter.egg-info/
+-rw-rw-rw-   0        0        0     1345 2023-05-01 10:51:42.000000 psremoter-1.0.1/src/PSRemoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-01 10:51:42.000000 psremoter-1.0.1/src/PSRemoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:51:42.000000 psremoter-1.0.1/src/PSRemoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-05-01 10:51:42.000000 psremoter-1.0.1/src/PSRemoter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-01 10:51:42.000000 psremoter-1.0.1/src/PSRemoter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0     3394 2023-05-01 10:47:51.000000 psremoter-1.0.1/src/connector.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:51:42.214032 psremoter-1.0.1/tests/
+-rw-rw-rw-   0        0        0      545 2023-05-01 10:47:51.000000 psremoter-1.0.1/tests/tests.py
```

### Comparing `psremoter-1.0.0/PKG-INFO` & `psremoter-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Powershell remote client tool for Python
-Home-page: https://github.com/pypa/sampleproject
-Author: Daniel Mandelblat
 Author-email: Daniel Mandelblat <danielmande@gmail.com>
 Project-URL: Homepage, https://github.com/danielMandelblat/psremoter
 Keywords: Powershell,remote,client,commands,Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `psremoter-1.0.0/README.md` & `psremoter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `psremoter-1.0.0/pyproject.toml` & `psremoter-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psremoter"
-version = "1.0.0"
+version = "1.0.1"
 description = "Powershell remote client tool for Python"
 readme = "README.md"
 authors = [{ name = "Daniel Mandelblat", email = "danielmande@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -26,7 +26,8 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/danielMandelblat/psremoter"
+
```

### Comparing `psremoter-1.0.0/src/PSRemoter.egg-info/PKG-INFO` & `psremoter-1.0.1/src/PSRemoter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: psremoter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Powershell remote client tool for Python
-Home-page: https://github.com/pypa/sampleproject
-Author: Daniel Mandelblat
 Author-email: Daniel Mandelblat <danielmande@gmail.com>
 Project-URL: Homepage, https://github.com/danielMandelblat/psremoter
 Keywords: Powershell,remote,client,commands,Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `psremoter-1.0.0/tests/tests.py` & `psremoter-1.0.1/tests/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
-from ..src.connector import Execute
+from ..src.connector import psremoter
 
-exec = Execute(hostname='localhost', command="echo test command").local_execution()
+exec = psremoter(hostname='localhost', command="echo test command").local_execution()
 
 class TestExecution(unittest.TestCase):
     def test_echo_command(self):
         self.assertEqual(exec.output.strip(), 'test command')
 
     def test_return_code_are_0(self):
         self.assertEqual(exec.return_code, 0)
```

