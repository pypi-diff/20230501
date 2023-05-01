# Comparing `tmp/simulateIRAS-0.1.0.tar.gz` & `tmp/simulateIRAS-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulateIRAS-0.1.0.tar", last modified: Mon May  1 18:01:14 2023, max compression
+gzip compressed data, was "simulateIRAS-0.1.0.post1.tar", last modified: Mon May  1 20:53:32 2023, max compression
```

## Comparing `simulateIRAS-0.1.0.tar` & `simulateIRAS-0.1.0.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 18:01:14.849035 simulateIRAS-0.1.0/
--rw-rw-rw-   0        0        0    35184 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1282 2023-05-01 18:01:14.849035 simulateIRAS-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/README.md
--rw-rw-rw-   0        0        0       99 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 18:01:14.849035 simulateIRAS-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1581 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:01:14.835457 simulateIRAS-0.1.0/src/
--rw-rw-rw-   0        0        0        2 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:01:14.847036 simulateIRAS-0.1.0/src/simulateIRAS.egg-info/
--rw-rw-rw-   0        0        0     1282 2023-05-01 18:01:14.000000 simulateIRAS-0.1.0/src/simulateIRAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-01 18:01:14.000000 simulateIRAS-0.1.0/src/simulateIRAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 18:01:14.000000 simulateIRAS-0.1.0/src/simulateIRAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 18:01:14.000000 simulateIRAS-0.1.0/src/simulateIRAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 18:01:14.000000 simulateIRAS-0.1.0/src/simulateIRAS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9905 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/src/simulateIRAS.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:01:14.848035 simulateIRAS-0.1.0/tests/
--rw-rw-rw-   0        0        0      146 2023-05-01 18:00:59.000000 simulateIRAS-0.1.0/tests/test_code.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.091927 simulateIRAS-0.1.0.post1/
+-rw-rw-rw-   0        0        0    35184 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1288 2023-05-01 20:53:32.091927 simulateIRAS-0.1.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/README.md
+-rw-rw-rw-   0        0        0       99 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:53:32.091927 simulateIRAS-0.1.0.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-05-01 20:53:22.000000 simulateIRAS-0.1.0.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.083927 simulateIRAS-0.1.0.post1/src/
+-rw-rw-rw-   0        0        0        2 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.090927 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/
+-rw-rw-rw-   0        0        0     1288 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-01 20:53:32.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9905 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.090927 simulateIRAS-0.1.0.post1/tests/
+-rw-rw-rw-   0        0        0      146 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/tests/test_code.py
```

### Comparing `simulateIRAS-0.1.0/LICENSE` & `simulateIRAS-0.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0/PKG-INFO` & `simulateIRAS-0.1.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0
+Version: 0.1.0.post1
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simulateIRAS-0.1.0/setup.py` & `simulateIRAS-0.1.0.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="simulateIRAS",
-    version = '0.1.0',
+    version = '0.1.0-1',
     description="A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements",
     py_modules = ["simulateIRAS"],
     package_dir = {'':'src'},
     
     author="coconnor24",
     author_email="coconnor@g.harvard.edu",
     
@@ -38,10 +38,10 @@
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics',
         
         'Operating System :: Microsoft :: Windows',
         'Operating System :: OS Independent',
         ],
         
-    install_requires=["numpy>=1.21.5", "scipy>=1.9.1"],
+    install_requires=["numpy", "scipy"],
     keywords = ["IRAS", "Surface Science", "FTIR", "doi:"]
 )
```

### Comparing `simulateIRAS-0.1.0/src/simulateIRAS.egg-info/PKG-INFO` & `simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0
+Version: 0.1.0.post1
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simulateIRAS-0.1.0/src/simulateIRAS.py` & `simulateIRAS-0.1.0.post1/src/simulateIRAS.py`

 * *Files identical despite different names*

