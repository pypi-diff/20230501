# Comparing `tmp/petrolib-1.2.4.tar.gz` & `tmp/petrolib-1.2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrolib-1.2.4.tar", last modified: Mon May  1 16:29:46 2023, max compression
+gzip compressed data, was "petrolib-1.2.4.1.tar", last modified: Mon May  1 18:01:58 2023, max compression
```

## Comparing `petrolib-1.2.4.tar` & `petrolib-1.2.4.1.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.796733 petrolib-1.2.4/
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     1093 2023-03-26 20:57:50.000000 petrolib-1.2.4/LICENSE
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       40 2023-05-01 16:09:25.000000 petrolib-1.2.4/MANIFEST.in
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3759 2023-05-01 16:29:46.792734 petrolib-1.2.4/PKG-INFO
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3137 2023-03-31 13:29:52.000000 petrolib-1.2.4/README.md
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      833 2023-05-01 16:22:17.000000 petrolib-1.2.4/pyproject.toml
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       38 2023-05-01 16:29:46.796733 petrolib-1.2.4/setup.cfg
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      984 2023-05-01 15:58:22.000000 petrolib-1.2.4/setup.py
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.760735 petrolib-1.2.4/src/
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.764735 petrolib-1.2.4/src/petrolib/
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)       21 2023-05-01 15:30:58.000000 petrolib-1.2.4/src/petrolib/__init__.py
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.768735 petrolib-1.2.4/src/petrolib/data/
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      286 2023-02-13 04:26:20.000000 petrolib-1.2.4/src/petrolib/data/litho_info.csv
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     4893 2023-05-01 15:44:07.000000 petrolib-1.2.4/src/petrolib/file_reader.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     8001 2023-04-12 22:16:51.000000 petrolib-1.2.4/src/petrolib/interp.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    58756 2023-05-01 16:14:23.000000 petrolib-1.2.4/src/petrolib/plots.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     6786 2023-04-12 22:19:13.000000 petrolib-1.2.4/src/petrolib/procs.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     5394 2023-03-26 17:12:05.000000 petrolib-1.2.4/src/petrolib/stats.py
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      236 2023-05-01 15:40:48.000000 petrolib-1.2.4/src/petrolib/utils.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    57715 2023-03-26 20:12:21.000000 petrolib-1.2.4/src/petrolib/workflow.py
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.768735 petrolib-1.2.4/src/petrolib.egg-info/
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3759 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/PKG-INFO
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      454 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/SOURCES.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        1 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/dependency_links.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       59 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/requires.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        9 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/top_level.txt
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.661255 petrolib-1.2.4.1/
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     1093 2023-03-26 20:57:50.000000 petrolib-1.2.4.1/LICENSE
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       40 2023-05-01 16:09:25.000000 petrolib-1.2.4.1/MANIFEST.in
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3691 2023-05-01 18:01:58.661255 petrolib-1.2.4.1/PKG-INFO
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3146 2023-05-01 17:54:18.000000 petrolib-1.2.4.1/README.md
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      853 2023-05-01 17:55:01.000000 petrolib-1.2.4.1/pyproject.toml
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       38 2023-05-01 18:01:58.661255 petrolib-1.2.4.1/setup.cfg
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.625255 petrolib-1.2.4.1/src/
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.633255 petrolib-1.2.4.1/src/petrolib/
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      278 2023-05-01 17:59:23.000000 petrolib-1.2.4.1/src/petrolib/__init__.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.633255 petrolib-1.2.4.1/src/petrolib/data/
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      286 2023-02-13 04:26:20.000000 petrolib-1.2.4.1/src/petrolib/data/litho_info.csv
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     4893 2023-05-01 15:44:07.000000 petrolib-1.2.4.1/src/petrolib/file_reader.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     8001 2023-04-12 22:16:51.000000 petrolib-1.2.4.1/src/petrolib/interp.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    58756 2023-05-01 16:14:23.000000 petrolib-1.2.4.1/src/petrolib/plots.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     6786 2023-04-12 22:19:13.000000 petrolib-1.2.4.1/src/petrolib/procs.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     5394 2023-03-26 17:12:05.000000 petrolib-1.2.4.1/src/petrolib/stats.py
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      236 2023-05-01 15:40:48.000000 petrolib-1.2.4.1/src/petrolib/utils.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    57715 2023-03-26 20:12:21.000000 petrolib-1.2.4.1/src/petrolib/workflow.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.633255 petrolib-1.2.4.1/src/petrolib.egg-info/
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3691 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/PKG-INFO
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      410 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        1 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        9 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/top_level.txt
```

### Comparing `petrolib-1.2.4/LICENSE` & `petrolib-1.2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/PKG-INFO` & `petrolib-1.2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: petrolib
-Version: 1.2.4
+Version: 1.2.4.1
 Summary: A Python Package for Petrophysical Evaluation
-Home-page: https://github.com/joshua-atolagbe/petrolib
-Author: Joshua Atolagbe
 Author-email: Joshua Atolagbe <atolagbejoshua2@gmail.com>
 Project-URL: Homepage, https://github.com/mayor-of-geology/petrolib
 Project-URL: Bug Tracker, https://github.com/mayor-of-geology/petrolib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -90,9 +88,9 @@
 
 ps = pp.paySummary(name='15-9_F1A')
 
 #save results to excel
 pp.save(file_name='Pay Summary')
 ```
 
-Tutorial [link](https://github.com/mayor-of-geology/tutorials)
+Tutorial [link](https://github.com/mayor-of-geology/tutorials/petrolib)
```

### Comparing `petrolib-1.2.4/README.md` & `petrolib-1.2.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,9 +74,9 @@
 
 ps = pp.paySummary(name='15-9_F1A')
 
 #save results to excel
 pp.save(file_name='Pay Summary')
 ```
 
-Tutorial [link](https://github.com/mayor-of-geology/tutorials)
+Tutorial [link](https://github.com/mayor-of-geology/tutorials/petrolib)
```

### Comparing `petrolib-1.2.4/pyproject.toml` & `petrolib-1.2.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ['matplotlib', 'pandas', 'numpy', 'lasio',
 			'scipy', 'seaborn', 'geopandas', 'contextily'
 		]
 build-backend = "setuptools.build_meta"
 
 [project]			
 name = "petrolib"
-version = "1.2.4"
+version = "1.2.4.1"
 authors = [
 	{name="Joshua Atolagbe", email="atolagbejoshua2@gmail.com"},	
 ]
 description = "A Python Package for Petrophysical Evaluation"
 readme = "README.md"
 requires-python = ">=3.5"
 license = {file = "LICENSE.txt"}
@@ -21,11 +21,12 @@
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/mayor-of-geology/petrolib"
 "Bug Tracker" = "https://github.com/mayor-of-geology/petrolib/issues"
 
 [tool.setuptools.packages.find]
+namespaces = true
 where = ["src"]
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `petrolib-1.2.4/src/petrolib/file_reader.py` & `petrolib-1.2.4.1/src/petrolib/file_reader.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/src/petrolib/interp.py` & `petrolib-1.2.4.1/src/petrolib/interp.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/src/petrolib/plots.py` & `petrolib-1.2.4.1/src/petrolib/plots.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/src/petrolib/procs.py` & `petrolib-1.2.4.1/src/petrolib/procs.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/src/petrolib/stats.py` & `petrolib-1.2.4.1/src/petrolib/stats.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/src/petrolib/workflow.py` & `petrolib-1.2.4.1/src/petrolib/workflow.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4/src/petrolib.egg-info/PKG-INFO` & `petrolib-1.2.4.1/src/petrolib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: petrolib
-Version: 1.2.4
+Version: 1.2.4.1
 Summary: A Python Package for Petrophysical Evaluation
-Home-page: https://github.com/joshua-atolagbe/petrolib
-Author: Joshua Atolagbe
 Author-email: Joshua Atolagbe <atolagbejoshua2@gmail.com>
 Project-URL: Homepage, https://github.com/mayor-of-geology/petrolib
 Project-URL: Bug Tracker, https://github.com/mayor-of-geology/petrolib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -90,9 +88,9 @@
 
 ps = pp.paySummary(name='15-9_F1A')
 
 #save results to excel
 pp.save(file_name='Pay Summary')
 ```
 
-Tutorial [link](https://github.com/mayor-of-geology/tutorials)
+Tutorial [link](https://github.com/mayor-of-geology/tutorials/petrolib)
```

