# Comparing `tmp/hydrogibs-0.1.11.tar.gz` & `tmp/hydrogibs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.1.11.tar", last modified: Sun Apr 30 22:43:03 2023, max compression
+gzip compressed data, was "hydrogibs-0.1.9.tar", last modified: Tue Apr 25 13:36:59 2023, max compression
```

## Comparing `hydrogibs-0.1.11.tar` & `hydrogibs-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-30 22:43:03.790372 hydrogibs-0.1.11/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.11/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      538 2023-04-30 22:43:03.790372 hydrogibs-0.1.11/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.11/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-30 22:43:03.786372 hydrogibs-0.1.11/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    12675 2023-04-29 15:14:25.000000 hydrogibs-0.1.11/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5115 2023-04-29 12:01:49.000000 hydrogibs-0.1.11/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.1.11/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     8728 2023-04-29 14:31:45.000000 hydrogibs-0.1.11/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.11/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.11/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.11/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.11/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-30 22:43:03.790372 hydrogibs-0.1.11/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      538 2023-04-30 22:43:03.000000 hydrogibs-0.1.11/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-04-30 22:43:03.000000 hydrogibs-0.1.11/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-30 22:43:03.000000 hydrogibs-0.1.11/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-30 22:43:03.000000 hydrogibs-0.1.11/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      486 2023-04-29 16:14:13.000000 hydrogibs-0.1.11/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-30 22:43:03.790372 hydrogibs-0.1.11/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.9/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.9/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    21938 2023-04-25 13:35:15.000000 hydrogibs-0.1.9/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     2926 2023-04-25 12:03:41.000000 hydrogibs-0.1.9/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.9/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.9/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.9/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-04-25 12:12:22.000000 hydrogibs-0.1.9/hydrogibs/__main__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.9/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 13:36:58.000000 hydrogibs-0.1.9/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      308 2023-04-25 13:36:59.000000 hydrogibs-0.1.9/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 13:36:58.000000 hydrogibs-0.1.9/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 13:36:59.000000 hydrogibs-0.1.9/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-04-25 13:36:12.000000 hydrogibs-0.1.9/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/setup.cfg
```

### Comparing `hydrogibs-0.1.11/LICENSE` & `hydrogibs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.11/PKG-INFO` & `hydrogibs-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.1.11
+Version: 0.1.9
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.1.11/hydrogibs/RationalMethod.py` & `hydrogibs-0.1.9/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.11/hydrogibs/SoCoSe.py` & `hydrogibs-0.1.9/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.11/hydrogibs/misc.py` & `hydrogibs-0.1.9/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.11/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.1.9/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.1.11
+Version: 0.1.9
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

