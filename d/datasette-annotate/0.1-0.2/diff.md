# Comparing `tmp/datasette-annotate-0.1.tar.gz` & `tmp/datasette-annotate-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-annotate-0.1.tar", last modified: Mon May  1 13:45:36 2023, max compression
+gzip compressed data, was "datasette-annotate-0.2.tar", last modified: Mon May  1 18:29:48 2023, max compression
```

## Comparing `datasette-annotate-0.1.tar` & `datasette-annotate-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:45:36.614819 datasette-annotate-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 13:45:22.000000 datasette-annotate-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 13:45:36.614819 datasette-annotate-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-01 13:45:22.000000 datasette-annotate-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:45:36.614819 datasette-annotate-0.1/datasette_annotate/
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-01 13:45:22.000000 datasette-annotate-0.1/datasette_annotate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:45:36.614819 datasette-annotate-0.1/datasette_annotate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 13:45:36.000000 datasette-annotate-0.1/datasette_annotate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 13:45:36.000000 datasette-annotate-0.1/datasette_annotate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:45:36.000000 datasette-annotate-0.1/datasette_annotate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 13:45:36.000000 datasette-annotate-0.1/datasette_annotate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 13:45:36.000000 datasette-annotate-0.1/datasette_annotate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 13:45:36.000000 datasette-annotate-0.1/datasette_annotate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:45:36.614819 datasette-annotate-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-01 13:45:22.000000 datasette-annotate-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:45:36.614819 datasette-annotate-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-01 13:45:22.000000 datasette-annotate-0.1/tests/test_datasette_annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 18:29:33.000000 datasette-annotate-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 18:29:48.547711 datasette-annotate-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-01 18:29:33.000000 datasette-annotate-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/datasette_annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-01 18:29:33.000000 datasette-annotate-0.2/datasette_annotate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/datasette_annotate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 18:29:48.000000 datasette-annotate-0.2/datasette_annotate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:29:48.547711 datasette-annotate-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-01 18:29:33.000000 datasette-annotate-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:29:48.547711 datasette-annotate-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-01 18:29:33.000000 datasette-annotate-0.2/tests/test_datasette_annotate.py
```

### Comparing `datasette-annotate-0.1/LICENSE` & `datasette-annotate-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-annotate-0.1/PKG-INFO` & `datasette-annotate-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-annotate
-Version: 0.1
+Version: 0.2
 Summary: Datasette plugin for annotating / labelling your training data.
 Home-page: https://github.com/MischaU8/datasette-annotate
 Author: Mischa Untaga
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/MischaU8/datasette-annotate/issues
 Project-URL: CI, https://github.com/MischaU8/datasette-annotate/actions
 Project-URL: Changelog, https://github.com/MischaU8/datasette-annotate/releases
```

### Comparing `datasette-annotate-0.1/README.md` & `datasette-annotate-0.2/README.md`

 * *Files identical despite different names*

### Comparing `datasette-annotate-0.1/datasette_annotate/__init__.py` & `datasette-annotate-0.2/datasette_annotate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import sys
 import textwrap
 
 from datasette import hookimpl
 from datasette.database import MultipleValues
 from datasette.views.base import DatasetteError
 from datasette.utils.asgi import Forbidden, NotFound, Response
 
 
 @hookimpl
 def permission_allowed(actor, action):
-    if action == "annotate-row" and actor and actor.get("id") == "root":
+    if action == "annotate-row" and (
+        (actor and actor.get("id") == "root") or (sys.platform == "emscripten")
+    ):
+        # running in Pyodide or other Emscripten based build
         return True
 
 
 async def _ensure_annotations_table(db, table):
     # create annotations table if it doesn't exist
     await db.execute_write(
         textwrap.dedent(
```

### Comparing `datasette-annotate-0.1/datasette_annotate.egg-info/PKG-INFO` & `datasette-annotate-0.2/datasette_annotate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-annotate
-Version: 0.1
+Version: 0.2
 Summary: Datasette plugin for annotating / labelling your training data.
 Home-page: https://github.com/MischaU8/datasette-annotate
 Author: Mischa Untaga
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/MischaU8/datasette-annotate/issues
 Project-URL: CI, https://github.com/MischaU8/datasette-annotate/actions
 Project-URL: Changelog, https://github.com/MischaU8/datasette-annotate/releases
```

### Comparing `datasette-annotate-0.1/setup.py` & `datasette-annotate-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1"
+VERSION = "0.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

