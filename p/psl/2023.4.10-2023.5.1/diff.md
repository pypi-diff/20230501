# Comparing `tmp/psl-2023.4.10.tar.gz` & `tmp/psl-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.4.10.tar", last modified: Mon Apr 10 13:05:27 2023, max compression
+gzip compressed data, was "psl-2023.5.1.tar", last modified: Mon May  1 13:05:00 2023, max compression
```

## Comparing `psl-2023.4.10.tar` & `psl-2023.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:05:27.813867 psl-2023.4.10/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-10 13:04:53.000000 psl-2023.4.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 13:04:53.000000 psl-2023.4.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-10 13:05:27.813867 psl-2023.4.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-10 13:04:53.000000 psl-2023.4.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:05:27.813867 psl-2023.4.10/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-10 13:05:01.000000 psl-2023.4.10/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   108947 2023-04-10 13:05:01.000000 psl-2023.4.10/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:04:53.000000 psl-2023.4.10/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:05:27.813867 psl-2023.4.10/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:05:15.000000 psl-2023.4.10/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:05:27.813867 psl-2023.4.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-10 13:04:53.000000 psl-2023.4.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:05:00.642043 psl-2023.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-01 13:04:29.000000 psl-2023.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 13:04:29.000000 psl-2023.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-01 13:05:00.642043 psl-2023.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-01 13:04:29.000000 psl-2023.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:05:00.638043 psl-2023.5.1/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-01 13:04:36.000000 psl-2023.5.1/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   108964 2023-05-01 13:04:36.000000 psl-2023.5.1/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:04:29.000000 psl-2023.5.1/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:05:00.642043 psl-2023.5.1/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:04:49.000000 psl-2023.5.1/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-01 13:05:00.000000 psl-2023.5.1/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:05:00.642043 psl-2023.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-01 13:04:29.000000 psl-2023.5.1/setup.py
```

### Comparing `psl-2023.4.10/LICENSE` & `psl-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.4.10/PKG-INFO` & `psl-2023.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.4.10
+Version: 2023.5.1
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.4.10/README.md` & `psl-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.4.10/psl/__init__.py` & `psl-2023.5.1/psl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.4.10"
-__checksum__ = "39ac0fd18a8d6b9126a82fc3d5b5e96ea4d9808e"
+__version__ = "2023.5.1"
+__checksum__ = "88c37e4a48740c9940a7765f98c68ac8cb05706b"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.4.10/psl/psl.txt` & `psl-2023.5.1/psl/psl.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5183,14 +5183,15 @@
 kherson.ua
 khmelnitskiy.ua
 khmelnytskyi.ua
 kiev.ua
 kirovograd.ua
 km.ua
 kr.ua
+kropyvnytskyi.ua
 krym.ua
 ks.ua
 kv.ua
 kyiv.ua
 lg.ua
 lt.ua
 lugansk.ua
```

### Comparing `psl-2023.4.10/psl.egg-info/PKG-INFO` & `psl-2023.5.1/psl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.4.10
+Version: 2023.5.1
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.4.10/setup.py` & `psl-2023.5.1/setup.py`

 * *Files identical despite different names*

