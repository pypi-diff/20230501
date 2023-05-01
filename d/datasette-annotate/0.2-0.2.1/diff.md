# Comparing `tmp/datasette-annotate-0.2.tar.gz` & `tmp/datasette-annotate-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-annotate-0.2.tar", last modified: Mon May  1 18:29:48 2023, max compression
+gzip compressed data, was "datasette-annotate-0.2.1.tar", last modified: Mon May  1 19:41:52 2023, max compression
```

## Comparing `datasette-annotate-0.2.tar` & `datasette-annotate-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 18:29:33.000000 datasette-annotate-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 18:29:48.547711 datasette-annotate-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-01 18:29:33.000000 datasette-annotate-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/datasette_annotate/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-01 18:29:33.000000 datasette-annotate-0.2/datasette_annotate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/datasette_annotate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:29:48.547711 datasette-annotate-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-01 18:29:33.000000 datasette-annotate-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-01 18:29:33.000000 datasette-annotate-0.2/tests/test_datasette_annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 19:41:33.000000 datasette-annotate-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-01 19:41:33.000000 datasette-annotate-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/datasette_annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-01 19:41:33.000000 datasette-annotate-0.2.1/datasette_annotate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/datasette_annotate/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 19:41:33.000000 datasette-annotate-0.2.1/datasette_annotate/templates/annotate-row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/datasette_annotate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-01 19:41:52.000000 datasette-annotate-0.2.1/datasette_annotate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-01 19:41:52.000000 datasette-annotate-0.2.1/datasette_annotate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:41:52.000000 datasette-annotate-0.2.1/datasette_annotate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-01 19:41:52.000000 datasette-annotate-0.2.1/datasette_annotate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 19:41:52.000000 datasette-annotate-0.2.1/datasette_annotate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 19:41:52.000000 datasette-annotate-0.2.1/datasette_annotate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-01 19:41:33.000000 datasette-annotate-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:41:52.956016 datasette-annotate-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-01 19:41:33.000000 datasette-annotate-0.2.1/tests/test_datasette_annotate.py
```

### Comparing `datasette-annotate-0.2/LICENSE` & `datasette-annotate-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-annotate-0.2/PKG-INFO` & `datasette-annotate-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-annotate
-Version: 0.2
+Version: 0.2.1
 Summary: Datasette plugin for annotating / labelling your training data.
 Home-page: https://github.com/MischaU8/datasette-annotate
 Author: Mischa Untaga
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/MischaU8/datasette-annotate/issues
 Project-URL: CI, https://github.com/MischaU8/datasette-annotate/actions
 Project-URL: Changelog, https://github.com/MischaU8/datasette-annotate/releases
```

### Comparing `datasette-annotate-0.2/README.md` & `datasette-annotate-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `datasette-annotate-0.2/datasette_annotate/__init__.py` & `datasette-annotate-0.2.1/datasette_annotate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 request.actor, "annotate-row", default=False
             ):
                 raise Forbidden("Permission denied for annotate-row")
             data, template_data, templates = await super().data(request, default_labels)
             return (
                 data,
                 template_data,
-                ("datasette_annotate/annotate-row.html",) + templates,
+                ("annotate-row.html",) + templates,
             )
 
         async def post(self, request, *args, **kwargs):
             datasette = self.ds
             if not await datasette.permission_allowed(
                 request.actor, "annotate-row", default=False
             ):
```

### Comparing `datasette-annotate-0.2/datasette_annotate.egg-info/PKG-INFO` & `datasette-annotate-0.2.1/datasette_annotate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-annotate
-Version: 0.2
+Version: 0.2.1
 Summary: Datasette plugin for annotating / labelling your training data.
 Home-page: https://github.com/MischaU8/datasette-annotate
 Author: Mischa Untaga
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/MischaU8/datasette-annotate/issues
 Project-URL: CI, https://github.com/MischaU8/datasette-annotate/actions
 Project-URL: Changelog, https://github.com/MischaU8/datasette-annotate/releases
```

### Comparing `datasette-annotate-0.2/setup.py` & `datasette-annotate-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2"
+VERSION = "0.2.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -27,13 +27,13 @@
     license="Apache License, Version 2.0",
     classifiers=[
         "Framework :: Datasette",
         "License :: OSI Approved :: Apache Software License",
     ],
     version=VERSION,
     packages=["datasette_annotate"],
-    entry_points={"datasette": ["datasette_annotate = datasette_annotate"]},
-    install_requires=["datasette"],
+    entry_points={"datasette": ["annotate = datasette_annotate"]},
+    install_requires=["datasette>=0.64"],
     extras_require={"test": ["pytest", "pytest-asyncio"]},
-    package_data={"datasette_annotate": ["templates/*"]},
+    package_data={"datasette_annotate": ["templates/*.html"]},
     python_requires=">=3.7",
 )
```

