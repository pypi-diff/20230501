# Comparing `tmp/django-filter-autotools-0.0.1.tar.gz` & `tmp/django-filter-autotools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-filter-autotools-0.0.1.tar", last modified: Mon May  1 20:54:17 2023, max compression
+gzip compressed data, was "dist/django-filter-autotools-0.0.2.tar", last modified: Mon May  1 20:56:38 2023, max compression
```

## Comparing `django-filter-autotools-0.0.1.tar` & `django-filter-autotools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 20:54:14.000000 django-filter-autotools-0.0.1/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/django_filter_autotools.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      302 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/django_filter_autotools.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/django_filter_autotools.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/django_filter_autotools.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/django_filter_autotools.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      622 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/django_filter_autotools.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.1/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-01 20:50:35.000000 django-filter-autotools-0.0.1/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/autotools/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6600 2023-05-01 17:15:11.000000 django-filter-autotools-0.0.1/autotools/mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.1/autotools/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      622 2023-05-01 20:54:17.000000 django-filter-autotools-0.0.1/PKG-INFO
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 20:56:35.000000 django-filter-autotools-0.0.2/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      302 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      622 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.2/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-01 20:50:35.000000 django-filter-autotools-0.0.2/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/autotools/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6600 2023-05-01 17:15:11.000000 django-filter-autotools-0.0.2/autotools/mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.2/autotools/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      622 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/PKG-INFO
```

### Comparing `django-filter-autotools-0.0.1/setup.py` & `django-filter-autotools-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="django-filter-autotools", 
-    version="0.0.1", 
+    version="0.0.2", 
     description=(
         "Provides some mixins which allow automatic generation of filtersets with"
         "a list of lookups, including new lookups not registered into Django."
     ),
     author="Carlos Pastor",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `django-filter-autotools-0.0.1/django_filter_autotools.egg-info/PKG-INFO` & `django-filter-autotools-0.0.2/django_filter_autotools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-filter-autotools-0.0.1/LICENSE` & `django-filter-autotools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.1/autotools/mixins.py` & `django-filter-autotools-0.0.2/autotools/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.1/PKG-INFO` & `django-filter-autotools-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

