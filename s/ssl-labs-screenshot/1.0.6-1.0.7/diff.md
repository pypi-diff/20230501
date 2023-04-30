# Comparing `tmp/ssl-labs-screenshot-1.0.6.tar.gz` & `tmp/ssl-labs-screenshot-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.6.tar", last modified: Sun Apr 30 22:02:27 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.7.tar", last modified: Sun Apr 30 22:16:49 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.6.tar` & `ssl-labs-screenshot-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:02:27.034026 ssl-labs-screenshot-1.0.6/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.6/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:02:27.033909 ssl-labs-screenshot-1.0.6/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1340 2023-04-30 21:33:41.000000 ssl-labs-screenshot-1.0.6/README.md
--rw-r--r--   0 mark       (501) staff       (20)      625 2023-04-30 22:02:15.000000 ssl-labs-screenshot-1.0.6/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 22:02:27.034059 ssl-labs-screenshot-1.0.6/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:02:27.033040 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:02:27.033760 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      360 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       65 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 22:02:27.000000 ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:16:49.189152 ssl-labs-screenshot-1.0.7/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.7/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:16:49.188986 ssl-labs-screenshot-1.0.7/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1340 2023-04-30 21:33:41.000000 ssl-labs-screenshot-1.0.7/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      634 2023-04-30 22:16:43.000000 ssl-labs-screenshot-1.0.7/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 22:16:49.189202 ssl-labs-screenshot-1.0.7/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:16:49.180173 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:16:49.188677 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      360 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.6/LICENSE.txt` & `ssl-labs-screenshot-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.6/PKG-INFO` & `ssl-labs-screenshot-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 Author-email: Mark Sowell <mark@marksowell.com>
 License: MIT
 Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
 Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ssl-labs-screenshot-1.0.6/README.md` & `ssl-labs-screenshot-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.6/pyproject.toml` & `ssl-labs-screenshot-1.0.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "ssl-labs-screenshot"
-version = "1.0.6"
+version = "1.0.7"
 description = "A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain."
 authors = [
     {name = "Mark Sowell", email = "mark@marksowell.com"},
 ]
 readme = "README.md"
 keywords = ["ssl", "screenshot", "ssllabs"]
 requires-python = ">=3.6"
 dependencies = [
-    'selenium >= 3.141.0',
-    'Pillow >= 8.3.2',
+    "selenium >= 3.141.0",
+    "Pillow >= 8.3.2",
 ]
 
 [project.urls]
 Source = "https://github.com/marksowell/ssl-labs-screenshot"
 
 [project.scripts]
-ssl-labs-screenshot = "ssl_labs_screenshot:main"
+ssl-labs-screenshot = "ssl_labs_screenshot.__main__:main"
 
 [project.license]
 text = "MIT"
```

### Comparing `ssl-labs-screenshot-1.0.6/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/__main__.py`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.6/ssl_labs_screenshot.egg-info/PKG-INFO` & `ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 Author-email: Mark Sowell <mark@marksowell.com>
 License: MIT
 Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
 Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

