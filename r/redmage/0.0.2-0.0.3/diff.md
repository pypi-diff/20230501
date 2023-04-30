# Comparing `tmp/redmage-0.0.2.tar.gz` & `tmp/redmage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.0.2.tar", max compression
+gzip compressed data, was "redmage-0.0.3.tar", max compression
```

## Comparing `redmage-0.0.2.tar` & `redmage-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.2/LICENSE
--rw-r--r--   0        0        0    14693 2023-04-30 22:37:22.299063 redmage-0.0.2/README.md
--rw-r--r--   0        0        0      624 2023-04-30 22:38:41.524069 redmage-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.2/redmage/__init__.py
--rw-r--r--   0        0        0     6164 2023-04-30 22:25:43.512248 redmage-0.0.2/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.2/redmage/convertors.py
--rw-r--r--   0        0        0     6979 2023-04-30 21:11:15.121820 redmage-0.0.2/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.2/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.2/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.2/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.2/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.2/redmage/triggers.py
--rw-r--r--   0        0        0      936 2023-04-04 02:55:52.571857 redmage-0.0.2/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.2/redmage/utils.py
--rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.3/LICENSE
+-rw-r--r--   0        0        0    14693 2023-04-30 22:37:22.299063 redmage-0.0.3/README.md
+-rw-r--r--   0        0        0      625 2023-04-30 22:57:19.087414 redmage-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.3/redmage/__init__.py
+-rw-r--r--   0        0        0     6164 2023-04-30 22:25:43.512248 redmage-0.0.3/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.3/redmage/convertors.py
+-rw-r--r--   0        0        0     6979 2023-04-30 21:11:15.121820 redmage-0.0.3/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.3/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.3/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.3/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.3/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.3/redmage/triggers.py
+-rw-r--r--   0        0        0      936 2023-04-04 02:55:52.571857 redmage-0.0.3/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.3/redmage/utils.py
+-rw-r--r--   0        0        0    15295 1970-01-01 00:00:00.000000 redmage-0.0.3/PKG-INFO
```

### Comparing `redmage-0.0.2/LICENSE` & `redmage-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/README.md` & `redmage-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/pyproject.toml` & `redmage-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "redmage"
-version = "0.0.2"
+version = "0.0.3"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 starlette = "^0.26.1"
 hype-html = "^1.1.3"
 python-multipart = "^0.0.6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `redmage-0.0.2/redmage/components.py` & `redmage-0.0.3/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/convertors.py` & `redmage-0.0.3/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/core.py` & `redmage-0.0.3/redmage/core.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/elements.py` & `redmage-0.0.3/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/targets.py` & `redmage-0.0.3/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/triggers.py` & `redmage-0.0.3/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/types.py` & `redmage-0.0.3/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/redmage/utils.py` & `redmage-0.0.3/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.2/PKG-INFO` & `redmage-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.0.2
+Version: 0.0.3
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hype-html (>=1.1.3,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: starlette (>=0.26.1,<0.27.0)
 Description-Content-Type: text/markdown
```

