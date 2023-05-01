# Comparing `tmp/cloudflare_images-0.0.2.tar.gz` & `tmp/cloudflare_images-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_images-0.0.2.tar", max compression
+gzip compressed data, was "cloudflare_images-0.0.3.tar", max compression
```

## Comparing `cloudflare_images-0.0.2.tar` & `cloudflare_images-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-04-23 21:35:59.824537 cloudflare_images-0.0.2/LICENSE
--rw-r--r--   0        0        0      265 2023-04-23 22:17:07.618439 cloudflare_images-0.0.2/README.md
--rw-r--r--   0        0        0      112 2023-04-26 17:25:29.603974 cloudflare_images-0.0.2/cloudflare_images/__init__.py
--rw-r--r--   0        0        0     7737 2023-04-23 22:59:59.288543 cloudflare_images-0.0.2/cloudflare_images/api.py
--rw-r--r--   0        0        0     3827 2023-04-26 17:23:10.020196 cloudflare_images-0.0.2/cloudflare_images/django.py
--rw-r--r--   0        0        0     1572 2023-04-26 17:24:56.870390 cloudflare_images-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 cloudflare_images-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-04-23 21:35:59.824537 cloudflare_images-0.0.3/LICENSE
+-rw-r--r--   0        0        0      265 2023-04-23 22:17:07.618439 cloudflare_images-0.0.3/README.md
+-rw-r--r--   0        0        0      112 2023-05-01 02:28:42.966649 cloudflare_images-0.0.3/cloudflare_images/__init__.py
+-rw-r--r--   0        0        0     7737 2023-04-23 22:59:59.288543 cloudflare_images-0.0.3/cloudflare_images/api.py
+-rw-r--r--   0        0        0     3827 2023-04-26 17:23:10.020196 cloudflare_images-0.0.3/cloudflare_images/django.py
+-rw-r--r--   0        0        0     1581 2023-05-01 02:28:00.153503 cloudflare_images-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 cloudflare_images-0.0.3/PKG-INFO
```

### Comparing `cloudflare_images-0.0.2/LICENSE` & `cloudflare_images-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_images-0.0.2/cloudflare_images/api.py` & `cloudflare_images-0.0.3/cloudflare_images/api.py`

 * *Files identical despite different names*

### Comparing `cloudflare_images-0.0.2/cloudflare_images/django.py` & `cloudflare_images-0.0.3/cloudflare_images/django.py`

 * *Files identical despite different names*

### Comparing `cloudflare_images-0.0.2/pyproject.toml` & `cloudflare_images-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "cloudflare-images"
 description = "Wrapper around Cloudflare Images API, usable custom Django storage class."
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
-license = "MIT"
+license = "BSD-3-Clause"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/cloudflare-images"
 documentation = "https://mv3.dev/cloudflare-images"
 classifiers = [
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
```

### Comparing `cloudflare_images-0.0.2/PKG-INFO` & `cloudflare_images-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cloudflare-images
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around Cloudflare Images API, usable custom Django storage class.
 Home-page: https://mv3.dev
-License: MIT
+License: BSD-3-Clause
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: django (>=4.2,<5.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
```

