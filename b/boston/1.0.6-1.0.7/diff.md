# Comparing `tmp/boston-1.0.6.tar.gz` & `tmp/boston-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boston-1.0.6.tar", last modified: Mon May  1 09:28:36 2023, max compression
+gzip compressed data, was "boston-1.0.7.tar", last modified: Mon May  1 09:30:50 2023, max compression
```

## Comparing `boston-1.0.6.tar` & `boston-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:28:36.678264 boston-1.0.6/
--rw-rw-rw-   0        0        0       41 2023-05-01 09:27:51.000000 boston-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      451 2023-05-01 09:28:36.677265 boston-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 09:28:36.648261 boston-1.0.6/boston/
--rw-rw-rw-   0        0        0       66 2023-05-01 09:28:12.000000 boston-1.0.6/boston/__init__.py
--rw-rw-rw-   0        0        0      459 2023-05-01 09:27:45.000000 boston-1.0.6/boston/house.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:28:36.670240 boston-1.0.6/boston.egg-info/
--rw-rw-rw-   0        0        0      451 2023-05-01 09:28:36.000000 boston-1.0.6/boston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-01 09:28:36.000000 boston-1.0.6/boston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:28:36.000000 boston-1.0.6/boston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 09:28:36.000000 boston-1.0.6/boston.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 09:28:36.000000 boston-1.0.6/boston.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 09:28:36.674248 boston-1.0.6/resources/
--rw-rw-rw-   0        0        0    35230 2023-04-27 10:15:02.000000 boston-1.0.6/resources/boston_house_prices.csv
--rw-rw-rw-   0        0        0       42 2023-05-01 09:28:36.678264 boston-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-01 08:49:50.000000 boston-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:30:50.528108 boston-1.0.7/
+-rw-rw-rw-   0        0        0       41 2023-05-01 09:27:51.000000 boston-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      451 2023-05-01 09:30:50.527109 boston-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 09:30:50.498110 boston-1.0.7/boston/
+-rw-rw-rw-   0        0        0       66 2023-05-01 09:30:38.000000 boston-1.0.7/boston/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-05-01 09:30:33.000000 boston-1.0.7/boston/house.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:30:50.521106 boston-1.0.7/boston.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-05-01 09:30:50.000000 boston-1.0.7/boston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-01 09:30:50.000000 boston-1.0.7/boston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:30:50.000000 boston-1.0.7/boston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 09:30:50.000000 boston-1.0.7/boston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 09:30:50.000000 boston-1.0.7/boston.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 09:30:50.524110 boston-1.0.7/resources/
+-rw-rw-rw-   0        0        0    35230 2023-04-27 10:15:02.000000 boston-1.0.7/resources/boston_house_prices.csv
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:30:50.529113 boston-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-05-01 09:30:43.000000 boston-1.0.7/setup.py
```

### Comparing `boston-1.0.6/resources/boston_house_prices.csv` & `boston-1.0.7/resources/boston_house_prices.csv`

 * *Files identical despite different names*

### Comparing `boston-1.0.6/setup.py` & `boston-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="boston", # Replace with your own username
-    version="1.0.6",
+    version="1.0.7",
     author="julmubm",
     author_email="dltpdn@gmail.com",
     description="loading boston housing price dataset like sklearn.datasets.load_boston() style.",
     long_description_content_type="text/markdown",
     url="https://github.com/dltpdn/boston",
     install_requires=['pandas'],
     packages=setuptools.find_packages(),
```

