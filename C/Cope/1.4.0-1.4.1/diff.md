# Comparing `tmp/Cope-1.4.0.tar.gz` & `tmp/Cope-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cope-1.4.0.tar", last modified: Thu Apr 27 02:09:38 2023, max compression
+gzip compressed data, was "Cope-1.4.1.tar", last modified: Mon May  1 20:35:46 2023, max compression
```

## Comparing `Cope-1.4.0.tar` & `Cope-1.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 02:09:38.420020 Cope-1.4.0/
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 02:09:38.417021 Cope-1.4.0/Cope/
--rw-r--r--   0 leonard   (1000) leonard   (1000)      509 2023-04-19 19:49:02.000000 Cope-1.4.0/Cope/Psuedonym.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)       56 2023-04-19 19:39:52.000000 Cope-1.4.0/Cope/_None.py
--rw-------   0 leonard   (1000) leonard   (1000)      476 2023-04-27 02:08:39.000000 Cope-1.4.0/Cope/__init__.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      440 2023-04-27 02:04:30.000000 Cope-1.4.0/Cope/_config.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2410 2023-04-19 19:39:57.000000 Cope-1.4.0/Cope/bak.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     5659 2023-04-19 19:40:20.000000 Cope-1.4.0/Cope/colors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)        0 2023-04-24 20:08:10.000000 Cope-1.4.0/Cope/constants.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    18362 2023-04-27 02:05:44.000000 Cope-1.4.0/Cope/debugging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     6995 2023-04-26 23:32:38.000000 Cope-1.4.0/Cope/decorators.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)       41 2023-04-19 20:53:26.000000 Cope-1.4.0/Cope/errors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1678 2023-04-19 19:43:55.000000 Cope-1.4.0/Cope/func.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1762 2023-04-19 19:54:46.000000 Cope-1.4.0/Cope/geometry.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4937 2023-04-24 19:14:51.000000 Cope-1.4.0/Cope/imports.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    19332 2023-04-19 20:04:30.000000 Cope-1.4.0/Cope/iterables.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    29346 2023-04-19 19:48:23.000000 Cope-1.4.0/Cope/key.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    10240 2023-04-20 21:06:35.000000 Cope-1.4.0/Cope/linalg.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      760 2023-04-26 23:08:59.000000 Cope-1.4.0/Cope/logging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    13221 2023-04-27 02:07:32.000000 Cope-1.4.0/Cope/misc.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2838 2023-04-19 19:48:50.000000 Cope-1.4.0/Cope/point.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      818 2023-04-19 19:48:58.000000 Cope-1.4.0/Cope/prettyTable.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1226 2023-04-19 19:49:09.000000 Cope-1.4.0/Cope/pygame.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2325 2023-04-19 19:49:10.000000 Cope-1.4.0/Cope/timing.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 02:09:38.418021 Cope-1.4.0/Cope.egg-info/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2239 2023-04-27 02:09:38.000000 Cope-1.4.0/Cope.egg-info/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)      867 2023-04-27 02:09:38.000000 Cope-1.4.0/Cope.egg-info/SOURCES.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-04-27 02:09:38.000000 Cope-1.4.0/Cope.egg-info/dependency_links.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)       24 2023-04-27 02:09:38.000000 Cope-1.4.0/Cope.egg-info/requires.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        5 2023-04-27 02:09:38.000000 Cope-1.4.0/Cope.egg-info/top_level.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 01:57:58.000000 Cope-1.4.0/LICENSE-APACHE
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 01:57:58.000000 Cope-1.4.0/LICENSE-MIT
--rw-r--r--   0 leonard   (1000) leonard   (1000)       61 2023-04-20 01:57:58.000000 Cope-1.4.0/MANIFEST.in
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2239 2023-04-27 02:09:38.420020 Cope-1.4.0/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1117 2023-04-20 02:04:21.000000 Cope-1.4.0/README.md
--rw-r--r--   0 leonard   (1000) leonard   (1000)      666 2023-04-27 02:09:11.000000 Cope-1.4.0/pyproject.toml
--rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-04-27 02:09:38.420020 Cope-1.4.0/setup.cfg
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2125 2023-04-20 22:23:00.000000 Cope-1.4.0/setup.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-27 02:09:38.420020 Cope-1.4.0/tests/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1186 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_colors.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2659 2023-04-26 23:49:56.000000 Cope-1.4.0/tests/test_debugging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3045 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_decorators.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      194 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_func.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      943 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_geometry.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      309 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_imports.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1743 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_iterables.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1262 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_key.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      228 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_logging.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1680 2023-04-27 00:33:06.000000 Cope-1.4.0/tests/test_misc.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      462 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_point.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      437 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_psuedonym.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      714 2023-04-27 00:21:44.000000 Cope-1.4.0/tests/test_replace_lines.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      280 2022-09-10 20:02:11.000000 Cope-1.4.0/tests/test_timing.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:35:46.709272 Cope-1.4.1/
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:35:46.707272 Cope-1.4.1/Cope/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      509 2023-04-19 19:49:02.000000 Cope-1.4.1/Cope/Psuedonym.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       56 2023-04-19 19:39:52.000000 Cope-1.4.1/Cope/_None.py
+-rw-------   0 leonard   (1000) leonard   (1000)      476 2023-05-01 20:35:15.000000 Cope-1.4.1/Cope/__init__.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      440 2023-04-27 02:04:30.000000 Cope-1.4.1/Cope/_config.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2410 2023-04-19 19:39:57.000000 Cope-1.4.1/Cope/bak.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     5659 2023-04-19 19:40:20.000000 Cope-1.4.1/Cope/colors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        0 2023-04-24 20:08:10.000000 Cope-1.4.1/Cope/constants.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    18362 2023-04-27 02:05:44.000000 Cope-1.4.1/Cope/debugging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     6995 2023-04-26 23:32:38.000000 Cope-1.4.1/Cope/decorators.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       41 2023-04-19 20:53:26.000000 Cope-1.4.1/Cope/errors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1678 2023-04-19 19:43:55.000000 Cope-1.4.1/Cope/func.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1762 2023-04-19 19:54:46.000000 Cope-1.4.1/Cope/geometry.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     4937 2023-04-24 19:14:51.000000 Cope-1.4.1/Cope/imports.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    19332 2023-04-19 20:04:30.000000 Cope-1.4.1/Cope/iterables.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    29346 2023-04-19 19:48:23.000000 Cope-1.4.1/Cope/key.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    10240 2023-04-20 21:06:35.000000 Cope-1.4.1/Cope/linalg.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      760 2023-04-26 23:08:59.000000 Cope-1.4.1/Cope/logging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    13223 2023-05-01 20:34:13.000000 Cope-1.4.1/Cope/misc.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2838 2023-04-19 19:48:50.000000 Cope-1.4.1/Cope/point.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      818 2023-04-19 19:48:58.000000 Cope-1.4.1/Cope/prettyTable.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1226 2023-04-19 19:49:09.000000 Cope-1.4.1/Cope/pygame.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2325 2023-04-19 19:49:10.000000 Cope-1.4.1/Cope/timing.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:35:46.707272 Cope-1.4.1/Cope.egg-info/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2239 2023-05-01 20:35:46.000000 Cope-1.4.1/Cope.egg-info/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      867 2023-05-01 20:35:46.000000 Cope-1.4.1/Cope.egg-info/SOURCES.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-05-01 20:35:46.000000 Cope-1.4.1/Cope.egg-info/dependency_links.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       24 2023-05-01 20:35:46.000000 Cope-1.4.1/Cope.egg-info/requires.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        5 2023-05-01 20:35:46.000000 Cope-1.4.1/Cope.egg-info/top_level.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 01:57:58.000000 Cope-1.4.1/LICENSE-APACHE
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 01:57:58.000000 Cope-1.4.1/LICENSE-MIT
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       61 2023-04-20 01:57:58.000000 Cope-1.4.1/MANIFEST.in
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2239 2023-05-01 20:35:46.709272 Cope-1.4.1/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1117 2023-04-20 02:04:21.000000 Cope-1.4.1/README.md
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      666 2023-05-01 20:35:39.000000 Cope-1.4.1/pyproject.toml
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-05-01 20:35:46.709272 Cope-1.4.1/setup.cfg
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2125 2023-04-20 22:23:00.000000 Cope-1.4.1/setup.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:35:46.708272 Cope-1.4.1/tests/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1186 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_colors.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2659 2023-04-26 23:49:56.000000 Cope-1.4.1/tests/test_debugging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     3045 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_decorators.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      194 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_func.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      943 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_geometry.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      309 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_imports.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1743 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_iterables.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1262 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_key.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      228 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_logging.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1680 2023-04-27 00:33:06.000000 Cope-1.4.1/tests/test_misc.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      462 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_point.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      437 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_psuedonym.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      714 2023-04-27 00:21:44.000000 Cope-1.4.1/tests/test_replace_lines.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      280 2022-09-10 20:02:11.000000 Cope-1.4.1/tests/test_timing.py
```

### Comparing `Cope-1.4.0/Cope/bak.py` & `Cope-1.4.1/Cope/bak.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/colors.py` & `Cope-1.4.1/Cope/colors.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/debugging.py` & `Cope-1.4.1/Cope/debugging.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/decorators.py` & `Cope-1.4.1/Cope/decorators.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/func.py` & `Cope-1.4.1/Cope/func.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/geometry.py` & `Cope-1.4.1/Cope/geometry.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/imports.py` & `Cope-1.4.1/Cope/imports.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/iterables.py` & `Cope-1.4.1/Cope/iterables.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/key.py` & `Cope-1.4.1/Cope/key.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/linalg.py` & `Cope-1.4.1/Cope/linalg.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/logging.py` & `Cope-1.4.1/Cope/logging.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/misc.py` & `Cope-1.4.1/Cope/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .debugging import get_varname, called_as_decorator, debug, get_metadata
 from .colors import ERROR
 import re
 import subprocess
 from os.path import join
 from random import randint
 import sys
-from math import floor
+# from math import floor
 from unicodedata import normalize
 
 def available(*args, fail_if_none=True):
     """ Returns the parameter passed to it which is not None, failing if more than one is None,
         and optionally failing if none of them are None """
     from varname import argname
```

### Comparing `Cope-1.4.0/Cope/point.py` & `Cope-1.4.1/Cope/point.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/prettyTable.py` & `Cope-1.4.1/Cope/prettyTable.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/pygame.py` & `Cope-1.4.1/Cope/pygame.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope/timing.py` & `Cope-1.4.1/Cope/timing.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/Cope.egg-info/PKG-INFO` & `Cope-1.4.1/Cope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cope
-Version: 1.4.0
+Version: 1.4.1
 Summary: A bunch of generic functions and classes useful in multiple projects
 Home-page: https://github.com/smartycope/Cope
 Author: Copeland Carter
 Author-email: smartycope@gmail.com
 Maintainer: Copeland Carter
 Maintainer-email: smartycope@gmail.com
 License: MIT/Apache-2.0
```

### Comparing `Cope-1.4.0/Cope.egg-info/SOURCES.txt` & `Cope-1.4.1/Cope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/LICENSE-APACHE` & `Cope-1.4.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/LICENSE-MIT` & `Cope-1.4.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/PKG-INFO` & `Cope-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cope
-Version: 1.4.0
+Version: 1.4.1
 Summary: A bunch of generic functions and classes useful in multiple projects
 Home-page: https://github.com/smartycope/Cope
 Author: Copeland Carter
 Author-email: smartycope@gmail.com
 Maintainer: Copeland Carter
 Maintainer-email: smartycope@gmail.com
 License: MIT/Apache-2.0
```

### Comparing `Cope-1.4.0/README.md` & `Cope-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/pyproject.toml` & `Cope-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'Cope'
-version = '1.4.0'
+version = '1.4.1'
 description = 'A bunch of generic functions and classes useful in multiple projects'
 author = 'Copeland Carter'
 author_email = 'smartycope@gmail.com'
 license = 'MIT/Apache-2.0'
 url = 'https://github.com/smartycope/Cope'
 
 [requires]
@@ -14,15 +14,15 @@
 requires = ['setuptools', 'wheel']
 
 [tool.hatch.commands]
 prerelease = 'hatch build'
 
 [project]
 name = 'Cope'
-version = '1.4.0'
+version = '1.4.1'
 description = 'A bunch of generic functions and classes useful in multiple projects'
 dependencies = [
     'varname',
 ]
 
 [project.optional-dependencies]
 linalg = [
```

### Comparing `Cope-1.4.0/setup.py` & `Cope-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_colors.py` & `Cope-1.4.1/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_debugging.py` & `Cope-1.4.1/tests/test_debugging.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_decorators.py` & `Cope-1.4.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_geometry.py` & `Cope-1.4.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_iterables.py` & `Cope-1.4.1/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_key.py` & `Cope-1.4.1/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_misc.py` & `Cope-1.4.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `Cope-1.4.0/tests/test_replace_lines.py` & `Cope-1.4.1/tests/test_replace_lines.py`

 * *Files identical despite different names*

