# Comparing `tmp/goatl-0.5.3.tar.gz` & `tmp/goatl-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goatl-0.5.3.tar", max compression
+gzip compressed data, was "goatl-0.5.4.tar", max compression
```

## Comparing `goatl-0.5.3.tar` & `goatl-0.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.5.3/LICENSE
--rw-r--r--   0        0        0     3768 2023-05-01 20:26:40.577772 goatl-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1833 2023-05-01 17:09:23.873407 goatl-0.5.3/README.md
--rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.5.3/src/goatl/__init__.py
--rw-r--r--   0        0        0    11718 2023-05-01 19:22:05.810863 goatl-0.5.3/src/goatl/core.py
--rw-r--r--   0        0        0     1478 2023-05-01 20:22:33.439577 goatl-0.5.3/src/goatl/utils.py
--rw-r--r--   0        0        0     2431 2023-05-01 20:26:55.742778 goatl-0.5.3/setup.py
--rw-r--r--   0        0        0     2501 2023-05-01 20:26:55.742778 goatl-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3735 2023-05-01 21:12:03.779858 goatl-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3714 2023-05-01 21:09:47.753862 goatl-0.5.4/README.md
+-rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.5.4/src/goatl/__init__.py
+-rw-r--r--   0        0        0    11718 2023-05-01 19:22:05.810863 goatl-0.5.4/src/goatl/core.py
+-rw-r--r--   0        0        0     1478 2023-05-01 20:22:33.439577 goatl-0.5.4/src/goatl/utils.py
+-rw-r--r--   0        0        0     4312 2023-05-01 21:12:21.445271 goatl-0.5.4/setup.py
+-rw-r--r--   0        0        0     4432 2023-05-01 21:12:21.445271 goatl-0.5.4/PKG-INFO
```

### Comparing `goatl-0.5.3/LICENSE` & `goatl-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goatl-0.5.3/pyproject.toml` & `goatl-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-# Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "goatl"
-version = "0.5.3"
+version = "0.5.4"
 description = "Greatest of all time logger"
 readme = "README.md"
 authors = ["goatl <EytanDn@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/EytanDn/goatl"
 homepage = "https://github.com/EytanDn/goatl"
 
-# Keywords description https://python-poetry.org/docs/pyproject/#keywords
-keywords = []  #! Update me
+keywords = ["logging", "logger", "log", "goat", "goatl", "goatlogger", "goat-logger", "goat-logging", "goat-log"] 
 
-# Pypi classifiers: https://pypi.org/classifiers/
-classifiers = [  #! Update me
+classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 
 
-
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^23.3", allow-prereleases = true}
 darglint = "^1.8.1"
```

### Comparing `goatl-0.5.3/src/goatl/__init__.py` & `goatl-0.5.4/src/goatl/__init__.py`

 * *Files identical despite different names*

### Comparing `goatl-0.5.3/src/goatl/core.py` & `goatl-0.5.4/src/goatl/core.py`

 * *Files identical despite different names*

### Comparing `goatl-0.5.3/src/goatl/utils.py` & `goatl-0.5.4/src/goatl/utils.py`

 * *Files identical despite different names*

