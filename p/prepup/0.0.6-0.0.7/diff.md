# Comparing `tmp/prepup-0.0.6.tar.gz` & `tmp/prepup-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.0.6.tar", last modified: Mon May  1 00:41:12 2023, max compression
+gzip compressed data, was "prepup-0.0.7.tar", last modified: Mon May  1 01:40:27 2023, max compression
```

## Comparing `prepup-0.0.6.tar` & `prepup-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.133244 prepup-0.0.6/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      493 2023-05-01 00:41:12.132266 prepup-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.114599 prepup-0.0.6/prepup/
--rw-rw-rw-   0        0        0     5353 2023-04-30 23:58:51.000000 prepup-0.0.6/prepup/__init__.py
--rw-rw-rw-   0        0        0    27774 2023-04-29 22:23:28.000000 prepup-0.0.6/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.126393 prepup-0.0.6/prepup.egg-info/
--rw-rw-rw-   0        0        0      493 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-01 00:41:12.000000 prepup-0.0.6/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 00:41:11.000000 prepup-0.0.6/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 00:41:12.134216 prepup-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3162 2023-05-01 00:40:12.000000 prepup-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 00:41:12.130311 prepup-0.0.6/tests/
--rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.6/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:40:27.188176 prepup-0.0.7/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      493 2023-05-01 01:40:27.183290 prepup-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 01:40:27.153393 prepup-0.0.7/prepup/
+-rw-rw-rw-   0        0        0     5353 2023-04-30 23:58:51.000000 prepup-0.0.7/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27791 2023-05-01 00:56:15.000000 prepup-0.0.7/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:40:27.176458 prepup-0.0.7/prepup.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-05-01 01:40:26.000000 prepup-0.0.7/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-01 01:40:27.000000 prepup-0.0.7/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 01:40:26.000000 prepup-0.0.7/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-01 01:40:26.000000 prepup-0.0.7/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2023-05-01 01:40:26.000000 prepup-0.0.7/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 01:40:26.000000 prepup-0.0.7/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 01:40:27.189150 prepup-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3155 2023-05-01 01:40:21.000000 prepup-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:40:27.181335 prepup-0.0.7/tests/
+-rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.7/tests/test_prepup.py
```

### Comparing `prepup-0.0.6/LICENSE` & `prepup-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.0.6/prepup/__init__.py` & `prepup-0.0.7/prepup/__init__.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.6/prepup/common.py` & `prepup-0.0.7/prepup/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 import nbformat as nbf
 import os
 from sklearn.preprocessing import StandardScaler
 from scipy.stats import shapiro
 from termcolor import colored
 from pyfiglet import Figlet
 
+os.system()
+
+
 term_font = Figlet(font="term")
 
 class Prepup:
     
     def __init__(self, dataframe):
         """
         The __init__ function is called when the class is instantiated.
```

### Comparing `prepup-0.0.6/setup.py` & `prepup-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 #     zip_safe=False,
 # )
 
 import setuptools
 
 setuptools.setup(
     name="prepup",
-    version="0.0.6",
+    version="0.0.7",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
-            "prepup = prepup.prepup:main",
+            "prepup = prepup:main",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

