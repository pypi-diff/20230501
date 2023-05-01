# Comparing `tmp/trident_models_package-0.0.2.tar.gz` & `tmp/trident_models_package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trident_models_package-0.0.2.tar", last modified: Mon Mar 27 16:40:50 2023, max compression
+gzip compressed data, was "trident_models_package-0.0.3.tar", last modified: Mon May  1 03:26:28 2023, max compression
```

## Comparing `trident_models_package-0.0.2.tar` & `trident_models_package-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 16:40:50.925106 trident_models_package-0.0.2/
--rw-rw-rw-   0        0        0     1081 2023-03-23 16:58:44.000000 trident_models_package-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      459 2023-03-27 16:40:50.922150 trident_models_package-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-03-23 16:55:40.000000 trident_models_package-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 16:40:50.926492 trident_models_package-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      533 2023-03-27 16:40:45.000000 trident_models_package-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 16:40:50.874226 trident_models_package-0.0.2/trident_models_package/
--rw-rw-rw-   0        0        0        0 2023-03-13 16:25:30.000000 trident_models_package-0.0.2/trident_models_package/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-03-22 21:46:50.000000 trident_models_package-0.0.2/trident_models_package/models.py
-drwxrwxrwx   0        0        0        0 2023-03-27 16:40:50.908200 trident_models_package-0.0.2/trident_models_package.egg-info/
--rw-rw-rw-   0        0        0      459 2023-03-27 16:40:50.000000 trident_models_package-0.0.2/trident_models_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-03-27 16:40:50.000000 trident_models_package-0.0.2/trident_models_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 16:40:50.000000 trident_models_package-0.0.2/trident_models_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-03-27 16:40:50.000000 trident_models_package-0.0.2/trident_models_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 03:26:28.878296 trident_models_package-0.0.3/
+-rw-rw-rw-   0        0        0     1081 2023-03-23 16:58:44.000000 trident_models_package-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      459 2023-05-01 03:26:28.876187 trident_models_package-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-03-23 16:55:40.000000 trident_models_package-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 03:26:28.880034 trident_models_package-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      533 2023-05-01 03:26:24.000000 trident_models_package-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 03:26:28.849132 trident_models_package-0.0.3/trident_models_package/
+-rw-rw-rw-   0        0        0        0 2023-03-13 16:25:30.000000 trident_models_package-0.0.3/trident_models_package/__init__.py
+-rw-rw-rw-   0        0        0     1602 2023-03-22 21:46:50.000000 trident_models_package-0.0.3/trident_models_package/models.py
+drwxrwxrwx   0        0        0        0 2023-05-01 03:26:28.870820 trident_models_package-0.0.3/trident_models_package.egg-info/
+-rw-rw-rw-   0        0        0      459 2023-05-01 03:26:28.000000 trident_models_package-0.0.3/trident_models_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-01 03:26:28.000000 trident_models_package-0.0.3/trident_models_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 03:26:28.000000 trident_models_package-0.0.3/trident_models_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-01 03:26:28.000000 trident_models_package-0.0.3/trident_models_package.egg-info/top_level.txt
```

### Comparing `trident_models_package-0.0.2/LICENSE` & `trident_models_package-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trident_models_package-0.0.2/setup.py` & `trident_models_package-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="trident_models_package",
-    version="0.0.2",
+    version="0.0.3",
     author="Karina",
     author_email="karina.ge@slalom.com",
     packages=["trident_models_package"],
     description="ORM Mmodels",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/karina.ge-slalom/trident-models",
```

### Comparing `trident_models_package-0.0.2/trident_models_package/models.py` & `trident_models_package-0.0.3/trident_models_package/models.py`

 * *Files identical despite different names*

