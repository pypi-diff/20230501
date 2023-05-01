# Comparing `tmp/overloaded-iterables-0.7.12.tar.gz` & `tmp/overloaded-iterables-0.7.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.12.tar", last modified: Mon May  1 05:58:04 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.14.tar", last modified: Mon May  1 06:00:50 2023, max compression
```

## Comparing `overloaded-iterables-0.7.12.tar` & `overloaded-iterables-0.7.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.277460 overloaded-iterables-0.7.12/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.12/LICENSE
--rw-rw-rw-   0        0        0     8079 2023-05-01 05:58:04.277460 overloaded-iterables-0.7.12/PKG-INFO
--rw-rw-rw-   0        0        0     7365 2023-05-01 05:45:35.000000 overloaded-iterables-0.7.12/README.md
--rw-rw-rw-   0        0        0      111 2023-05-01 05:58:04.279460 overloaded-iterables-0.7.12/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.263458 overloaded-iterables-0.7.12/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.268459 overloaded-iterables-0.7.12/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.7.12/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    15059 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.12/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-05-01 05:58:04.276459 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     8079 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-01 05:58:04.000000 overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.581390 overloaded-iterables-0.7.14/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.14/LICENSE
+-rw-rw-rw-   0        0        0     8090 2023-05-01 06:00:50.581390 overloaded-iterables-0.7.14/PKG-INFO
+-rw-rw-rw-   0        0        0     7376 2023-05-01 05:58:56.000000 overloaded-iterables-0.7.14/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-01 06:00:50.583393 overloaded-iterables-0.7.14/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.557390 overloaded-iterables-0.7.14/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.563392 overloaded-iterables-0.7.14/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.7.14/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    15059 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.14/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.580391 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     8090 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.12/LICENSE` & `overloaded-iterables-0.7.14/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.12/PKG-INFO` & `overloaded-iterables-0.7.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.12
+Version: 0.7.14
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-[![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
+[comment]: [![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
 
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
```

### Comparing `overloaded-iterables-0.7.12/README.md` & `overloaded-iterables-0.7.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Overloaded Iterables
 
-[![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
+[comment]: [![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
 
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
```

### Comparing `overloaded-iterables-0.7.12/setup.py` & `overloaded-iterables-0.7.14/setup.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.12/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.14/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.12/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.12
+Version: 0.7.14
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-[![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
+[comment]: [![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
 
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
```

