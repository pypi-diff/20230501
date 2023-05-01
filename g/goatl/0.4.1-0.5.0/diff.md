# Comparing `tmp/goatl-0.4.1.tar.gz` & `tmp/goatl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goatl-0.4.1.tar", max compression
+gzip compressed data, was "goatl-0.5.0.tar", max compression
```

## Comparing `goatl-0.4.1.tar` & `goatl-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.4.1/LICENSE
--rw-r--r--   0        0        0     3611 2023-05-01 17:47:27.445311 goatl-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1833 2023-05-01 17:09:23.873407 goatl-0.4.1/README.md
--rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.4.1/src/goatl/__init__.py
--rw-r--r--   0        0        0    11739 2023-05-01 18:15:42.624341 goatl-0.4.1/src/goatl/core.py
--rw-r--r--   0        0        0     1423 2023-05-01 18:21:49.215963 goatl-0.4.1/src/goatl/utils.py
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 goatl-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3611 2023-05-01 18:56:36.069949 goatl-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1833 2023-05-01 17:09:23.873407 goatl-0.5.0/README.md
+-rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.5.0/src/goatl/__init__.py
+-rw-r--r--   0        0        0    11739 2023-05-01 18:15:42.624341 goatl-0.5.0/src/goatl/core.py
+-rw-r--r--   0        0        0     1423 2023-05-01 18:21:49.215963 goatl-0.5.0/src/goatl/utils.py
+-rw-r--r--   0        0        0     2431 2023-05-01 18:56:56.120227 goatl-0.5.0/setup.py
+-rw-r--r--   0        0        0     2501 2023-05-01 18:56:56.120227 goatl-0.5.0/PKG-INFO
```

### Comparing `goatl-0.4.1/LICENSE` & `goatl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goatl-0.4.1/pyproject.toml` & `goatl-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "goatl"
-version = "0.4.1"
+version = "0.5.0"
 description = "Greatest of all time logger"
 readme = "README.md"
 authors = ["goatl <EytanDn@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/EytanDn/goatl"
 homepage = "https://github.com/EytanDn/goatl"
```

### Comparing `goatl-0.4.1/README.md` & `goatl-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `goatl-0.4.1/src/goatl/__init__.py` & `goatl-0.5.0/src/goatl/__init__.py`

 * *Files identical despite different names*

### Comparing `goatl-0.4.1/src/goatl/core.py` & `goatl-0.5.0/src/goatl/core.py`

 * *Files identical despite different names*

### Comparing `goatl-0.4.1/src/goatl/utils.py` & `goatl-0.5.0/src/goatl/utils.py`

 * *Files identical despite different names*

### Comparing `goatl-0.4.1/PKG-INFO` & `goatl-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: goatl
-Version: 0.4.1
+Version: 0.5.0
 Summary: Greatest of all time logger
 Home-page: https://github.com/EytanDn/goatl
 License: MIT
 Author: goatl
 Author-email: EytanDn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/EytanDn/goatl
 Description-Content-Type: text/markdown
 
 # goatl
```

