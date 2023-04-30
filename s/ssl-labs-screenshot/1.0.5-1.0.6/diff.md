# Comparing `tmp/ssl-labs-screenshot-1.0.5.tar.gz` & `tmp/ssl-labs-screenshot-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.5.tar", last modified: Sun Apr 30 21:33:51 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.6.tar", last modified: Sun Apr 30 22:02:27 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.5.tar` & `ssl-labs-screenshot-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:33:51.736444 ssl-labs-screenshot-1.0.5/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.5/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)       24 2023-04-30 20:06:51.000000 ssl-labs-screenshot-1.0.5/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     2065 2023-04-30 21:33:51.736302 ssl-labs-screenshot-1.0.5/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1340 2023-04-30 21:33:41.000000 ssl-labs-screenshot-1.0.5/README.md
--rw-r--r--   0 mark       (501) staff       (20)       56 2023-04-30 20:02:02.000000 ssl-labs-screenshot-1.0.5/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       31 2023-04-30 18:30:24.000000 ssl-labs-screenshot-1.0.5/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 21:33:51.736481 ssl-labs-screenshot-1.0.5/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1270 2023-04-30 21:33:24.000000 ssl-labs-screenshot-1.0.5/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:33:51.731411 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 21:33:51.736131 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     2065 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      398 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 21:33:51.000000 ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:02:27.034026 ssl-labs-screenshot-1.0.6/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.6/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:02:27.033909 ssl-labs-screenshot-1.0.6/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1340 2023-04-30 21:33:41.000000 ssl-labs-screenshot-1.0.6/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      625 2023-04-30 22:02:15.000000 ssl-labs-screenshot-1.0.6/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 22:02:27.034059 ssl-labs-screenshot-1.0.6/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:02:27.033040 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:02:27.033760 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      360 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       65 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.5/LICENSE.txt` & `ssl-labs-screenshot-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.5/PKG-INFO` & `ssl-labs-screenshot-1.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.5
-Summary: A script to capture SSL Labs server test report screenshots
-Home-page: https://github.com/marksowell/ssl-labs-screenshot
-Author: Mark Sowell
-Author-email: mark@marksowell.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 1.0.6
+Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
+Author-email: Mark Sowell <mark@marksowell.com>
+License: MIT
+Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
+Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 SSL Labs Screenshot is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain.
 
 ## Requirements
```

### Comparing `ssl-labs-screenshot-1.0.5/README.md` & `ssl-labs-screenshot-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.5/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/__main__.py`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.5/ssl_labs_screenshot.egg-info/PKG-INFO` & `ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.5
-Summary: A script to capture SSL Labs server test report screenshots
-Home-page: https://github.com/marksowell/ssl-labs-screenshot
-Author: Mark Sowell
-Author-email: mark@marksowell.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 1.0.6
+Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
+Author-email: Mark Sowell <mark@marksowell.com>
+License: MIT
+Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
+Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 SSL Labs Screenshot is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain.
 
 ## Requirements
```

