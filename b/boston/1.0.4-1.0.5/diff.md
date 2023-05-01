# Comparing `tmp/boston-1.0.4.tar.gz` & `tmp/boston-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boston-1.0.4.tar", last modified: Fri Apr 28 08:10:20 2023, max compression
+gzip compressed data, was "boston-1.0.5.tar", last modified: Mon May  1 08:47:23 2023, max compression
```

## Comparing `boston-1.0.4.tar` & `boston-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:10:20.368877 boston-1.0.4/
--rw-rw-rw-   0        0        0       41 2023-04-28 08:07:34.000000 boston-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      451 2023-04-28 08:10:20.366852 boston-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-28 08:10:20.336189 boston-1.0.4/boston/
--rw-rw-rw-   0        0        0      338 2023-04-28 08:07:48.000000 boston-1.0.4/boston/__init__.py
--rw-rw-rw-   0        0        0      374 2023-04-28 08:08:34.000000 boston-1.0.4/boston/house.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:10:20.357412 boston-1.0.4/boston.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-28 08:10:19.000000 boston-1.0.4/boston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-28 08:10:20.000000 boston-1.0.4/boston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:10:19.000000 boston-1.0.4/boston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 08:10:19.000000 boston-1.0.4/boston.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 08:10:19.000000 boston-1.0.4/boston.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 08:10:20.361852 boston-1.0.4/resources/
--rw-rw-rw-   0        0        0    35230 2023-04-27 10:15:02.000000 boston-1.0.4/resources/boston_house_prices.csv
--rw-rw-rw-   0        0        0       42 2023-04-28 08:10:20.368877 boston-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-04-28 08:07:44.000000 boston-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:47:23.844156 boston-1.0.5/
+-rw-rw-rw-   0        0        0       31 2023-05-01 08:35:17.000000 boston-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      451 2023-05-01 08:47:23.843155 boston-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 08:47:23.813178 boston-1.0.5/boston/
+-rw-rw-rw-   0        0        0       66 2023-05-01 08:47:08.000000 boston-1.0.5/boston/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-05-01 08:36:16.000000 boston-1.0.5/boston/house.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:47:23.839160 boston-1.0.5/boston.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-05-01 08:47:23.000000 boston-1.0.5/boston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-05-01 08:47:23.000000 boston-1.0.5/boston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:47:23.000000 boston-1.0.5/boston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 08:47:23.000000 boston-1.0.5/boston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 08:47:23.000000 boston-1.0.5/boston.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35230 2023-04-27 10:15:02.000000 boston-1.0.5/boston_house_prices.csv
+-rw-rw-rw-   0        0        0       42 2023-05-01 08:47:23.844156 boston-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-05-01 08:47:04.000000 boston-1.0.5/setup.py
```

### Comparing `boston-1.0.4/resources/boston_house_prices.csv` & `boston-1.0.5/boston_house_prices.csv`

 * *Files identical despite different names*

### Comparing `boston-1.0.4/setup.py` & `boston-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="boston", # Replace with your own username
-    version="1.0.4",
+    version="1.0.5",
     author="julmubm",
     author_email="dltpdn@gmail.com",
     description="loading boston housing price dataset like sklearn.datasets.load_boston() style.",
     long_description_content_type="text/markdown",
     url="https://github.com/dltpdn/boston",
     install_requires=['pandas'],
     packages=setuptools.find_packages(),
```

