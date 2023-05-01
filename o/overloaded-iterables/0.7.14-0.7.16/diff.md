# Comparing `tmp/overloaded-iterables-0.7.14.tar.gz` & `tmp/overloaded-iterables-0.7.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.14.tar", last modified: Mon May  1 06:00:50 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.16.tar", last modified: Mon May  1 08:08:20 2023, max compression
```

## Comparing `overloaded-iterables-0.7.14.tar` & `overloaded-iterables-0.7.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.581390 overloaded-iterables-0.7.14/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.14/LICENSE
--rw-rw-rw-   0        0        0     8090 2023-05-01 06:00:50.581390 overloaded-iterables-0.7.14/PKG-INFO
--rw-rw-rw-   0        0        0     7376 2023-05-01 05:58:56.000000 overloaded-iterables-0.7.14/README.md
--rw-rw-rw-   0        0        0      111 2023-05-01 06:00:50.583393 overloaded-iterables-0.7.14/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.557390 overloaded-iterables-0.7.14/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.563392 overloaded-iterables-0.7.14/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-04-29 23:52:39.000000 overloaded-iterables-0.7.14/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    15059 2023-05-01 05:41:11.000000 overloaded-iterables-0.7.14/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:00:50.580391 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     8090 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-01 06:00:50.000000 overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 08:08:20.022153 overloaded-iterables-0.7.16/
+-rw-rw-rw-   0        0        0     1097 2023-05-01 06:21:45.000000 overloaded-iterables-0.7.16/LICENSE
+-rw-rw-rw-   0        0        0     7908 2023-05-01 08:08:20.023164 overloaded-iterables-0.7.16/PKG-INFO
+-rw-rw-rw-   0        0        0     7194 2023-05-01 08:05:48.000000 overloaded-iterables-0.7.16/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-01 08:08:20.029846 overloaded-iterables-0.7.16/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-05-01 06:21:45.000000 overloaded-iterables-0.7.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:08:19.963958 overloaded-iterables-0.7.16/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 08:08:19.983438 overloaded-iterables-0.7.16/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0        0 2023-05-01 06:21:45.000000 overloaded-iterables-0.7.16/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    14919 2023-05-01 08:06:01.000000 overloaded-iterables-0.7.16/src/overloaded_iterables/classes.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:08:20.020985 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0     7908 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.14/LICENSE` & `overloaded-iterables-0.7.16/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.14/PKG-INFO` & `overloaded-iterables-0.7.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.14
+Version: 0.7.16
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,16 +14,14 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-[comment]: [![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
-
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
```

### Comparing `overloaded-iterables-0.7.14/README.md` & `overloaded-iterables-0.7.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Overloaded Iterables
 
-[comment]: [![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
-
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
```

### Comparing `overloaded-iterables-0.7.14/setup.py` & `overloaded-iterables-0.7.16/setup.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.14/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.16/src/overloaded_iterables/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,18 +288,15 @@
         Return the length of the current OverloadedList object.
 
         Assuming a property of a class object is persistent in memory unless garbage-collected or updated and hence will be cheaper to call than
         a full method/function. 
 
         I might be grossly mistaken in this however so feel free to correct me (with proof, kindly).
         """
-        count = 0
-        for _ in self:
-            count = count + 1
-        return count
+        return len(self)
 
     @property
     def frequencies(self):
         """
         Finds and returns the frequencies of the values in th `OverloadedList` object.
 
         Assuming a property of a class object is persistent in memory unless garbage-collected or updated and hence will be cheaper to call than
@@ -429,11 +426,8 @@
         Return the length of the current OverloadedSet object.
 
         Assuming a property of a class object is persistent in memory unless garbage-collected or updated and hence will be cheaper to call than
         a full method/function. 
 
         I might be grossly mistaken in this however so feel free to correct me (with proof, kindly).
         """
-        count = 0
-        for _ in self:
-            count = count + 1
-        return count
+        return len(self)
```

### Comparing `overloaded-iterables-0.7.14/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.14
+Version: 0.7.16
 Summary: Overloaded version of the built-in python classes: list and set to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot
 Platform: windows
@@ -14,16 +14,14 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-[comment]: [![codecov](https://codecov.io/gh/Arkiralor/overloaded_iterables/branch/master/graph/badge.svg?token=3CZT98MXIK)](https://codecov.io/gh/Arkiralor/overloaded_iterables)
-
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
 
 1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
```

