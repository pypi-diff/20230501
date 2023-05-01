# Comparing `tmp/envname-0.0.2.tar.gz` & `tmp/envname-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envname-0.0.2.tar", last modified: Mon May  1 16:32:23 2023, max compression
+gzip compressed data, was "envname-1.0.tar", last modified: Mon May  1 16:40:11 2023, max compression
```

## Comparing `envname-0.0.2.tar` & `envname-1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 envname-0.0.2/LICENSE
--rw-r--r--   0        0        0     1765 2023-05-01 15:47:23.102653 envname-0.0.2/README.md
--rw-r--r--   0        0        0      645 2023-05-01 16:30:31.499496 envname-0.0.2/envname/__init__.py
--rw-r--r--   0        0        0       49 2023-05-01 16:24:22.924576 envname-0.0.2/envname/_envname.py
--rw-r--r--   0        0        0      583 2023-05-01 16:30:47.105702 envname-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 envname-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 envname-1.0/LICENSE
+-rw-r--r--   0        0        0     1765 2023-05-01 15:47:23.102653 envname-1.0/README.md
+-rw-r--r--   0        0        0      645 2023-05-01 16:30:31.499496 envname-1.0/envname/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-01 16:24:22.924576 envname-1.0/envname/_envname.py
+-rw-r--r--   0        0        0      581 2023-05-01 16:36:21.492222 envname-1.0/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 envname-1.0/PKG-INFO
```

### Comparing `envname-0.0.2/LICENSE` & `envname-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `envname-0.0.2/README.md` & `envname-1.0/README.md`

 * *Files identical despite different names*

### Comparing `envname-0.0.2/envname/__init__.py` & `envname-1.0/envname/__init__.py`

 * *Files identical despite different names*

### Comparing `envname-0.0.2/pyproject.toml` & `envname-1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "envname"
-version = "0.0.2"
+version = "1.0"
 description = "为运行环境设置名称"
 dependencies = []
 keywords = []
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `envname-0.0.2/PKG-INFO` & `envname-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envname
-Version: 0.0.2
+Version: 1.0
 Summary: 为运行环境设置名称
 Keywords: 
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/envname#readme
```

