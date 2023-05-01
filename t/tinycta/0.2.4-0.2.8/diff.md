# Comparing `tmp/tinycta-0.2.4.tar.gz` & `tmp/tinycta-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinycta-0.2.4.tar", max compression
+gzip compressed data, was "tinycta-0.2.8.tar", max compression
```

## Comparing `tinycta-0.2.4.tar` & `tinycta-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-03-29 06:42:41.085632 tinycta-0.2.4/LICENSE
--rw-r--r--   0        0        0      241 2023-03-29 06:42:41.085632 tinycta-0.2.4/README.md
--rw-r--r--   0        0        0      416 2023-03-29 06:43:01.310791 tinycta-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 06:42:41.085632 tinycta-0.2.4/tinycta/__init__.py
--rw-r--r--   0        0        0     2439 2023-03-29 06:42:41.085632 tinycta-0.2.4/tinycta/linalg.py
--rw-r--r--   0        0        0     2635 2023-03-29 06:42:41.085632 tinycta-0.2.4/tinycta/portfolio.py
--rw-r--r--   0        0        0     1471 2023-03-29 06:42:41.085632 tinycta-0.2.4/tinycta/signal.py
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 tinycta-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-01 17:18:28.326201 tinycta-0.2.8/LICENSE
+-rw-r--r--   0        0        0      241 2023-05-01 17:18:28.326201 tinycta-0.2.8/README.md
+-rw-r--r--   0        0        0      416 2023-05-01 17:18:47.986483 tinycta-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/__init__.py
+-rw-r--r--   0        0        0     2439 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/linalg.py
+-rw-r--r--   0        0        0     2635 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/portfolio.py
+-rw-r--r--   0        0        0     1471 2023-05-01 17:18:28.326201 tinycta-0.2.8/tinycta/signal.py
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 tinycta-0.2.8/PKG-INFO
```

### Comparing `tinycta-0.2.4/LICENSE` & `tinycta-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.4/tinycta/linalg.py` & `tinycta-0.2.8/tinycta/linalg.py`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.4/tinycta/portfolio.py` & `tinycta-0.2.8/tinycta/portfolio.py`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.4/tinycta/signal.py` & `tinycta-0.2.8/tinycta/signal.py`

 * *Files identical despite different names*

### Comparing `tinycta-0.2.4/PKG-INFO` & `tinycta-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinycta
-Version: 0.2.4
+Version: 0.2.8
 Summary: ...
 Home-page: https://github.com/tschm/TinyCTA
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

