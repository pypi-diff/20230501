# Comparing `tmp/start_url-0.0.6.tar.gz` & `tmp/start_url-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_url-0.0.6.tar", max compression
+gzip compressed data, was "start_url-0.0.7.tar", max compression
```

## Comparing `start_url-0.0.6.tar` & `start_url-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.6/README.md
--rw-r--r--   0        0        0     1558 2023-05-01 16:46:29.911105 start_url-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      152 2023-05-01 16:46:32.972989 start_url-0.0.6/start_url/__init__.py
--rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.6/start_url/headers.py
--rw-r--r--   0        0        0     1920 2023-05-01 16:47:18.833042 start_url-0.0.6/start_url/main.py
--rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.6/start_url/meta.py
--rw-r--r--   0        0        0      844 2023-05-01 16:44:56.866528 start_url-0.0.6/start_url/url.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 start_url-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.7/README.md
+-rw-r--r--   0        0        0     1558 2023-05-01 16:50:15.455095 start_url-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-05-01 16:50:18.443961 start_url-0.0.7/start_url/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.7/start_url/headers.py
+-rw-r--r--   0        0        0     1920 2023-05-01 16:47:18.833042 start_url-0.0.7/start_url/main.py
+-rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.7/start_url/meta.py
+-rw-r--r--   0        0        0     1050 2023-05-01 16:49:28.441557 start_url-0.0.7/start_url/url.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 start_url-0.0.7/PKG-INFO
```

### Comparing `start_url-0.0.6/pyproject.toml` & `start_url-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-url"
 description = "httpx.get URL metadata with BeautifulSoup"
-version = "0.0.6"
+version = "0.0.7"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-url"
 documentation = "https://mv3.dev/start-url"
 classifiers = [
```

### Comparing `start_url-0.0.6/start_url/headers.py` & `start_url-0.0.7/start_url/headers.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.6/start_url/main.py` & `start_url-0.0.7/start_url/main.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.6/start_url/meta.py` & `start_url-0.0.7/start_url/meta.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.6/PKG-INFO` & `start_url-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-url
-Version: 0.0.6
+Version: 0.0.7
 Summary: httpx.get URL metadata with BeautifulSoup
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

