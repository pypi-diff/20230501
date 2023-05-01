# Comparing `tmp/image-charts-6.1.28.tar.gz` & `tmp/image-charts-6.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-charts-6.1.28.tar", last modified: Wed Apr 19 18:02:35 2023, max compression
+gzip compressed data, was "dist/image-charts-6.1.29.tar", last modified: Mon May  1 19:12:25 2023, max compression
```

## Comparing `image-charts-6.1.28.tar` & `image-charts-6.1.29.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:02:35.000000 image-charts-6.1.28/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-04-19 18:01:42.000000 image-charts-6.1.28/ImageCharts.py
--rw-r--r--   0 root         (0) root         (0)    61353 2023-04-19 18:02:35.000000 image-charts-6.1.28/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    60526 2023-04-19 18:01:42.000000 image-charts-6.1.28/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:02:35.000000 image-charts-6.1.28/image_charts.egg-info/
--rw-r--r--   0 root         (0) root         (0)    61353 2023-04-19 18:02:35.000000 image-charts-6.1.28/image_charts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-19 18:02:35.000000 image-charts-6.1.28/image_charts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 18:02:35.000000 image-charts-6.1.28/image_charts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-19 18:02:35.000000 image-charts-6.1.28/image_charts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-19 18:02:35.000000 image-charts-6.1.28/image_charts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 18:02:35.000000 image-charts-6.1.28/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-19 18:02:34.000000 image-charts-6.1.28/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 19:12:25.000000 image-charts-6.1.29/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-05-01 19:11:29.000000 image-charts-6.1.29/ImageCharts.py
+-rw-r--r--   0 root         (0) root         (0)    61353 2023-05-01 19:12:25.000000 image-charts-6.1.29/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    60526 2023-05-01 19:11:29.000000 image-charts-6.1.29/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 19:12:25.000000 image-charts-6.1.29/image_charts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    61353 2023-05-01 19:12:25.000000 image-charts-6.1.29/image_charts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-01 19:12:25.000000 image-charts-6.1.29/image_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 19:12:25.000000 image-charts-6.1.29/image_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-01 19:12:25.000000 image-charts-6.1.29/image_charts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-01 19:12:25.000000 image-charts-6.1.29/image_charts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 19:12:25.000000 image-charts-6.1.29/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-01 19:12:24.000000 image-charts-6.1.29/setup.py
```

### Comparing `image-charts-6.1.28/ImageCharts.py` & `image-charts-6.1.29/ImageCharts.py`

 * *Files identical despite different names*

### Comparing `image-charts-6.1.28/PKG-INFO` & `image-charts-6.1.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-charts
-Version: 6.1.28
+Version: 6.1.29
 Summary: Official Image-Charts.com API client library
 Home-page: https://github.com/image-charts/python
 Author: Francois-Guillaume Ribreau
 Author-email: github@fgribreau.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-charts Version: 6.1.28 Summary: Official
+Metadata-Version: 2.1 Name: image-charts Version: 6.1.29 Summary: Official
 Image-Charts.com API client library Home-page: https://github.com/image-charts/
 python Author: Francois-Guillaume Ribreau Author-email: github@fgribreau.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications :: Email Classifier: Topic :: Software
```

### Comparing `image-charts-6.1.28/README.md` & `image-charts-6.1.29/README.md`

 * *Files identical despite different names*

### Comparing `image-charts-6.1.28/image_charts.egg-info/PKG-INFO` & `image-charts-6.1.29/image_charts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-charts
-Version: 6.1.28
+Version: 6.1.29
 Summary: Official Image-Charts.com API client library
 Home-page: https://github.com/image-charts/python
 Author: Francois-Guillaume Ribreau
 Author-email: github@fgribreau.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-charts Version: 6.1.28 Summary: Official
+Metadata-Version: 2.1 Name: image-charts Version: 6.1.29 Summary: Official
 Image-Charts.com API client library Home-page: https://github.com/image-charts/
 python Author: Francois-Guillaume Ribreau Author-email: github@fgribreau.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications :: Email Classifier: Topic :: Software
```

### Comparing `image-charts-6.1.28/setup.py` & `image-charts-6.1.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='image-charts',
-  version="6.1.28",
+  version="6.1.29",
   py_modules=['ImageCharts'],
   url='https://github.com/image-charts/python',
   license='MIT',
   author='Francois-Guillaume Ribreau',
   author_email='github@fgribreau.com',
   description='Official Image-Charts.com API client library',
   long_description=long_description,
```

