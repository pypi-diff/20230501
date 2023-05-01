# Comparing `tmp/ssl-labs-screenshot-1.0.8.tar.gz` & `tmp/ssl-labs-screenshot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.8.tar", last modified: Mon May  1 05:24:14 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.9.tar", last modified: Mon May  1 05:30:11 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.8.tar` & `ssl-labs-screenshot-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.622182 ssl-labs-screenshot-1.0.8/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.8/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)     1969 2023-05-01 05:24:14.622054 ssl-labs-screenshot-1.0.8/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1549 2023-05-01 05:19:27.000000 ssl-labs-screenshot-1.0.8/README.md
--rw-r--r--   0 mark       (501) staff       (20)      634 2023-05-01 05:23:05.000000 ssl-labs-screenshot-1.0.8/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-01 05:24:14.622219 ssl-labs-screenshot-1.0.8/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.620628 ssl-labs-screenshot-1.0.8/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.621184 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-05-01 03:09:04.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4772 2023-05-01 05:22:59.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.621911 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     1969 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      392 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       74 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:30:11.880728 ssl-labs-screenshot-1.0.9/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.9/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)     2039 2023-05-01 05:30:11.880565 ssl-labs-screenshot-1.0.9/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1619 2023-05-01 05:28:46.000000 ssl-labs-screenshot-1.0.9/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      634 2023-05-01 05:29:42.000000 ssl-labs-screenshot-1.0.9/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-01 05:30:11.880770 ssl-labs-screenshot-1.0.9/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:30:11.872528 ssl-labs-screenshot-1.0.9/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:30:11.873120 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-05-01 03:09:04.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4772 2023-05-01 05:29:37.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:30:11.880381 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     2039 2023-05-01 05:30:11.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      392 2023-05-01 05:30:11.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-01 05:30:11.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       74 2023-05-01 05:30:11.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-05-01 05:30:11.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-05-01 05:30:11.000000 ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.8/LICENSE.txt` & `ssl-labs-screenshot-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.8/PKG-INFO` & `ssl-labs-screenshot-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 Author-email: Mark Sowell <mark@marksowell.com>
 License: MIT
 Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
 Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SSL Labs Screenshot
 A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 
-<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
+<p align="center"><img src="https://raw.githubusercontent.com/marksowell/SSL-Labs-Screenshot/main/images/www.ssllabs.com_report.png" width="300px" />
 
 ## Requirements
 - Python 3.6
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
```

### Comparing `ssl-labs-screenshot-1.0.8/README.md` & `ssl-labs-screenshot-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SSL Labs Screenshot
 A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 
-<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
+<p align="center"><img src="https://raw.githubusercontent.com/marksowell/SSL-Labs-Screenshot/main/images/www.ssllabs.com_report.png" width="300px" />
 
 ## Requirements
 - Python 3.6
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
```

### Comparing `ssl-labs-screenshot-1.0.8/pyproject.toml` & `ssl-labs-screenshot-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "ssl-labs-screenshot"
-version = "1.0.8"
+version = "1.0.9"
 description = "A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain."
 authors = [
     {name = "Mark Sowell", email = "mark@marksowell.com"},
 ]
 readme = "README.md"
 keywords = ["ssl", "screenshot", "ssllabs"]
 requires-python = ">=3.6"
```

### Comparing `ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from PIL import Image
 from urllib.parse import urlparse
 
-VERSION = "v1.0.8"
+VERSION = "v1.0.9"
 
 def is_valid_domain(domain):
     try:
         parsed_domain = urlparse(domain)
         if parsed_domain.scheme in ["http", "https"]:
             domain = parsed_domain.netloc
         else:
```

### Comparing `ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/PKG-INFO` & `ssl-labs-screenshot-1.0.9/src/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 Author-email: Mark Sowell <mark@marksowell.com>
 License: MIT
 Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
 Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SSL Labs Screenshot
 A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 
-<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
+<p align="center"><img src="https://raw.githubusercontent.com/marksowell/SSL-Labs-Screenshot/main/images/www.ssllabs.com_report.png" width="300px" />
 
 ## Requirements
 - Python 3.6
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
```

