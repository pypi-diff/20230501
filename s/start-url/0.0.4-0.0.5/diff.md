# Comparing `tmp/start_url-0.0.4.tar.gz` & `tmp/start_url-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_url-0.0.4.tar", max compression
+gzip compressed data, was "start_url-0.0.5.tar", max compression
```

## Comparing `start_url-0.0.4.tar` & `start_url-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.4/README.md
--rw-r--r--   0        0        0     1559 2023-05-01 04:36:42.312109 start_url-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      152 2023-05-01 04:34:26.114367 start_url-0.0.4/start_url/__init__.py
--rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.4/start_url/headers.py
--rw-r--r--   0        0        0     2098 2023-05-01 04:36:02.631836 start_url-0.0.4/start_url/main.py
--rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.4/start_url/meta.py
--rw-r--r--   0        0        0      596 2023-04-30 15:25:08.484611 start_url-0.0.4/start_url/url.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 start_url-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.5/README.md
+-rw-r--r--   0        0        0     1535 2023-05-01 04:42:59.958311 start_url-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-05-01 04:43:04.258611 start_url-0.0.5/start_url/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.5/start_url/headers.py
+-rw-r--r--   0        0        0     2098 2023-05-01 04:36:02.631836 start_url-0.0.5/start_url/main.py
+-rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.5/start_url/meta.py
+-rw-r--r--   0        0        0      596 2023-04-30 15:25:08.484611 start_url-0.0.5/start_url/url.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 start_url-0.0.5/PKG-INFO
```

### Comparing `start_url-0.0.4/pyproject.toml` & `start_url-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-url"
 description = "httpx.get URL metadata with BeautifulSoup"
-version = "0.0.4"
+version = "0.0.5"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-url"
 documentation = "https://mv3.dev/start-url"
 classifiers = [
@@ -14,18 +14,17 @@
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0"
+httpx = "^0.24"
 python-dateutil = "^2.8.2"
 beautifulsoup4 = "^4.11.2"
-httpx = "^0.23.3"
-start-sdk = "^0.0.22"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
 black = "^23.1.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
```

### Comparing `start_url-0.0.4/start_url/headers.py` & `start_url-0.0.5/start_url/headers.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.4/start_url/main.py` & `start_url-0.0.5/start_url/main.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.4/start_url/meta.py` & `start_url-0.0.5/start_url/meta.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.4/start_url/url.py` & `start_url-0.0.5/start_url/url.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.4/PKG-INFO` & `start_url-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: start-url
-Version: 0.0.4
+Version: 0.0.5
 Summary: httpx.get URL metadata with BeautifulSoup
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.24,<0.25)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
-Requires-Dist: start-sdk (>=0.0.22,<0.0.23)
 Project-URL: Documentation, https://mv3.dev/start-url
 Project-URL: Repository, https://github.com/justmars/start-url
 Description-Content-Type: text/markdown
 
 # start-url
 
 ![Github CI](https://github.com/justmars/start-url/actions/workflows/main.yml/badge.svg)
```

