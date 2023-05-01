# Comparing `tmp/ssl-labs-screenshot-1.0.7.tar.gz` & `tmp/ssl-labs-screenshot-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl-labs-screenshot-1.0.7.tar", last modified: Sun Apr 30 22:16:49 2023, max compression
+gzip compressed data, was "ssl-labs-screenshot-1.0.8.tar", last modified: Mon May  1 05:24:14 2023, max compression
```

## Comparing `ssl-labs-screenshot-1.0.7.tar` & `ssl-labs-screenshot-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:16:49.189152 ssl-labs-screenshot-1.0.7/
--rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.7/LICENSE.txt
--rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:16:49.188986 ssl-labs-screenshot-1.0.7/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1340 2023-04-30 21:33:41.000000 ssl-labs-screenshot-1.0.7/README.md
--rw-r--r--   0 mark       (501) staff       (20)      634 2023-04-30 22:16:43.000000 ssl-labs-screenshot-1.0.7/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-30 22:16:49.189202 ssl-labs-screenshot-1.0.7/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:16:49.180173 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-04-30 18:53:22.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4104 2023-04-29 01:32:27.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/__main__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-30 22:16:49.188677 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     1760 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      360 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       74 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 mark       (501) staff       (20)       32 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       20 2023-04-30 22:16:49.000000 ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.622182 ssl-labs-screenshot-1.0.8/
+-rw-r--r--   0 mark       (501) staff       (20)     1068 2023-04-30 18:51:38.000000 ssl-labs-screenshot-1.0.8/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)     1969 2023-05-01 05:24:14.622054 ssl-labs-screenshot-1.0.8/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1549 2023-05-01 05:19:27.000000 ssl-labs-screenshot-1.0.8/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      634 2023-05-01 05:23:05.000000 ssl-labs-screenshot-1.0.8/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-01 05:24:14.622219 ssl-labs-screenshot-1.0.8/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.620628 ssl-labs-screenshot-1.0.8/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.621184 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-05-01 03:09:04.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4772 2023-05-01 05:22:59.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/__main__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 05:24:14.621911 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     1969 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      392 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       74 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 mark       (501) staff       (20)       32 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       20 2023-05-01 05:24:14.000000 ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/top_level.txt
```

### Comparing `ssl-labs-screenshot-1.0.7/LICENSE.txt` & `ssl-labs-screenshot-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssl-labs-screenshot-1.0.7/PKG-INFO` & `ssl-labs-screenshot-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 Author-email: Mark Sowell <mark@marksowell.com>
 License: MIT
 Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
 Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-SSL Labs Screenshot is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain.
+# SSL Labs Screenshot
+A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
+
+<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
 
 ## Requirements
-- Python 3.x
+- Python 3.6
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
-1. Install SSL Labs Screenshot using pip:
+1. Install using pip:
    ```
    pip install ssl-labs-screenshot
    ```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
-4. Extract the contents of the downloaded ZIP file to a directory on your system.
-5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
+4. Extract the contents of the downloaded ZIP file.
+5. Either move the ChromeDriver executable to a directory that is already included in your system's `PATH` environment variable, or add the directory containing the extracted ChromeDriver executable to your system's `PATH` variable.
 
 ## Usage
 Run the script with the following command:
 ```
 ssl-labs-screenshot domain.com
 ```
 Replace domain.com with the domain you want to test. The script will open a headless Chrome browser and load the SSL Labs report for the domain. It will capture a temporary screenshot of the report and save it as a PNG file in the same directory as the script, with the name domain_report_tmp.png. The script will delete the temporary screenshot after the trimmed image is created with the name domain_report.png
 
 ## Limitations
 The script only captures the first server's report for domains with multiple servers.
+
+## License
+The scripts and documentation in this project are released under the [MIT License](https://github.com/marksowell/SSL-Labs-Screenshot/blob/main/LICENSE)
```

### Comparing `ssl-labs-screenshot-1.0.7/pyproject.toml` & `ssl-labs-screenshot-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "ssl-labs-screenshot"
-version = "1.0.7"
+version = "1.0.8"
 description = "A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain."
 authors = [
     {name = "Mark Sowell", email = "mark@marksowell.com"},
 ]
 readme = "README.md"
 keywords = ["ssl", "screenshot", "ssllabs"]
 requires-python = ">=3.6"
```

### Comparing `ssl-labs-screenshot-1.0.7/ssl_labs_screenshot/__main__.py` & `ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,48 @@
 import time
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from PIL import Image
+from urllib.parse import urlparse
 
-VERSION = "v1.0.1"
+VERSION = "v1.0.8"
+
+def is_valid_domain(domain):
+    try:
+        parsed_domain = urlparse(domain)
+        if parsed_domain.scheme in ["http", "https"]:
+            domain = parsed_domain.netloc
+        else:
+            domain = parsed_domain.path
+        if len(domain) > 0 and domain.count(".") > 0:
+            # Remove any trailing slashes or path elements
+            domain = domain.split('/')[0]
+            return domain
+    except Exception as e:
+        return None
+    return None
 
 def main():
-    print(f"SSL Labs Screenshot Script - Version {VERSION}")
+    print(f"SSL Labs Screenshot - Version {VERSION}")
     if len(sys.argv) < 2:
         print("Usage: python script.py domain.com")
         sys.exit(1)
 
-    domain = sys.argv[1].replace("https://", "")
+    domain = sys.argv[1]
+
+    sanitized_domain = is_valid_domain(domain)
+
+    if not sanitized_domain:
+        print("Invalid domain. Please enter a valid domain.")
+        sys.exit(1)
+
+    domain = sanitized_domain
     ssl_labs_url = f"https://www.ssllabs.com/ssltest/analyze.html?d={domain}&hideResults=on"
 
     print("Formatting and parsing the URL...")
     chrome_options = Options()
     chrome_options.add_argument("--headless")
     chrome_options.add_argument("--disable-gpu")
     chrome_options.add_argument("--no-sandbox")
```

### Comparing `ssl-labs-screenshot-1.0.7/ssl_labs_screenshot.egg-info/PKG-INFO` & `ssl-labs-screenshot-1.0.8/src/ssl_labs_screenshot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: ssl-labs-screenshot
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
 Author-email: Mark Sowell <mark@marksowell.com>
 License: MIT
 Project-URL: Source, https://github.com/marksowell/ssl-labs-screenshot
 Keywords: ssl,screenshot,ssllabs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-SSL Labs Screenshot is a Python script that captures a trimmed screenshot of the SSL Labs report for a given domain.
+# SSL Labs Screenshot
+A Python package to capture a trimmed screenshot of the SSL Labs report for a given domain.
+
+<p align="center"><img src="images/www.ssllabs.com_report.png" width="300px" />
 
 ## Requirements
-- Python 3.x
+- Python 3.6
 - Chrome browser (version 89 or later)
 - ChromeDriver
 
 ## Installation
-1. Install SSL Labs Screenshot using pip:
+1. Install using pip:
    ```
    pip install ssl-labs-screenshot
    ```
 3. Download the latest version of ChromeDriver from the following link: https://sites.google.com/chromium.org/driver/downloads
-4. Extract the contents of the downloaded ZIP file to a directory on your system.
-5. Either move the ChromeDriver executable to a directory already in your system's `PATH` environment variable or add the path to the directory where you extracted the ChromeDriver executable to the `PATH` variable.
+4. Extract the contents of the downloaded ZIP file.
+5. Either move the ChromeDriver executable to a directory that is already included in your system's `PATH` environment variable, or add the directory containing the extracted ChromeDriver executable to your system's `PATH` variable.
 
 ## Usage
 Run the script with the following command:
 ```
 ssl-labs-screenshot domain.com
 ```
 Replace domain.com with the domain you want to test. The script will open a headless Chrome browser and load the SSL Labs report for the domain. It will capture a temporary screenshot of the report and save it as a PNG file in the same directory as the script, with the name domain_report_tmp.png. The script will delete the temporary screenshot after the trimmed image is created with the name domain_report.png
 
 ## Limitations
 The script only captures the first server's report for domains with multiple servers.
+
+## License
+The scripts and documentation in this project are released under the [MIT License](https://github.com/marksowell/SSL-Labs-Screenshot/blob/main/LICENSE)
```

