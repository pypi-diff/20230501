# Comparing `tmp/prepup-0.0.8.tar.gz` & `tmp/prepup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.0.8.tar", last modified: Mon May  1 01:46:16 2023, max compression
+gzip compressed data, was "prepup-0.0.9.tar", last modified: Mon May  1 01:53:26 2023, max compression
```

## Comparing `prepup-0.0.8.tar` & `prepup-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 01:46:16.965240 prepup-0.0.8/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      493 2023-05-01 01:46:16.962306 prepup-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 01:46:16.936294 prepup-0.0.8/prepup/
--rw-rw-rw-   0        0        0     5350 2023-05-01 01:45:53.000000 prepup-0.0.8/prepup/__init__.py
--rw-rw-rw-   0        0        0    27791 2023-05-01 00:56:15.000000 prepup-0.0.8/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:46:16.953520 prepup-0.0.8/prepup.egg-info/
--rw-rw-rw-   0        0        0      493 2023-05-01 01:46:16.000000 prepup-0.0.8/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-01 01:46:16.000000 prepup-0.0.8/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:46:16.000000 prepup-0.0.8/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-01 01:46:16.000000 prepup-0.0.8/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2023-05-01 01:46:16.000000 prepup-0.0.8/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 01:46:16.000000 prepup-0.0.8/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 01:46:16.966236 prepup-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3155 2023-05-01 01:46:02.000000 prepup-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:46:16.960353 prepup-0.0.8/tests/
--rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.8/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.715836 prepup-0.0.9/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      493 2023-05-01 01:53:26.713902 prepup-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.685939 prepup-0.0.9/prepup/
+-rw-rw-rw-   0        0        0     5350 2023-05-01 01:45:53.000000 prepup-0.0.9/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27778 2023-05-01 01:52:39.000000 prepup-0.0.9/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.703529 prepup-0.0.9/prepup.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      170 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 01:53:26.715836 prepup-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3159 2023-05-01 01:53:20.000000 prepup-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.709977 prepup-0.0.9/tests/
+-rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.9/tests/test_prepup.py
```

### Comparing `prepup-0.0.8/LICENSE` & `prepup-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.0.8/prepup/__init__.py` & `prepup-0.0.9/prepup/__init__.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.8/prepup/common.py` & `prepup-0.0.9/prepup/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import nbformat as nbf
 import os
 from sklearn.preprocessing import StandardScaler
 from scipy.stats import shapiro
 from termcolor import colored
 from pyfiglet import Figlet
 
-os.system()
 
 
 term_font = Figlet(font="term")
 
 class Prepup:
     
     def __init__(self, dataframe):
```

### Comparing `prepup-0.0.8/setup.py` & `prepup-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 #     zip_safe=False,
 # )
 
 import setuptools
 
 setuptools.setup(
     name="prepup",
-    version="0.0.8",
+    version="0.0.9",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             "prepup = prepup:main",
@@ -82,21 +82,21 @@
         "termcolor",
         "pyfiglet",
         "blessed",
         "imbalanced_learn",
         "imblearn",
         "joblib",
         "matplotlib",
-        "nbclient",
-        "nbformat",
+        #"nbclient",
+        #"nbformat",
         "numpy",
         "pandas",
         "plotext",
-        "prefect",
-        "prefect_jupyter",
+        #"prefect",
+        #"prefect_jupyter",
         "pydantic",
         "pyfiglet",
         "pytest",
         "scikit_learn",
         "scipy",
         "seaborn",
         "termcolor",
```

