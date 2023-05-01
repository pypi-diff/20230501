# Comparing `tmp/redmage-0.0.4.tar.gz` & `tmp/redmage-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.0.4.tar", max compression
+gzip compressed data, was "redmage-0.0.5.tar", max compression
```

## Comparing `redmage-0.0.4.tar` & `redmage-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.4/LICENSE
--rw-r--r--   0        0        0    14693 2023-04-30 22:37:22.299063 redmage-0.0.4/README.md
--rw-r--r--   0        0        0      624 2023-05-01 00:08:28.662989 redmage-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.4/redmage/__init__.py
--rw-r--r--   0        0        0     6371 2023-05-01 00:05:27.298095 redmage-0.0.4/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.4/redmage/convertors.py
--rw-r--r--   0        0        0     6979 2023-04-30 21:11:15.121820 redmage-0.0.4/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.4/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.4/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.4/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.4/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.4/redmage/triggers.py
--rw-r--r--   0        0        0      936 2023-04-04 02:55:52.571857 redmage-0.0.4/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.4/redmage/utils.py
--rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.5/LICENSE
+-rw-r--r--   0        0        0    14693 2023-04-30 22:37:22.299063 redmage-0.0.5/README.md
+-rw-r--r--   0        0        0      624 2023-05-01 01:05:35.169429 redmage-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.5/redmage/__init__.py
+-rw-r--r--   0        0        0     6371 2023-05-01 00:05:27.298095 redmage-0.0.5/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.5/redmage/convertors.py
+-rw-r--r--   0        0        0     6979 2023-04-30 21:11:15.121820 redmage-0.0.5/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.5/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.5/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.5/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.5/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.5/redmage/triggers.py
+-rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.0.5/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.5/redmage/utils.py
+-rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.0.5/PKG-INFO
```

### Comparing `redmage-0.0.4/LICENSE` & `redmage-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/README.md` & `redmage-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/pyproject.toml` & `redmage-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.0.4"
+version = "0.0.5"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.0.4/redmage/components.py` & `redmage-0.0.5/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/redmage/convertors.py` & `redmage-0.0.5/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/redmage/core.py` & `redmage-0.0.5/redmage/core.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/redmage/elements.py` & `redmage-0.0.5/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/redmage/targets.py` & `redmage-0.0.5/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/redmage/triggers.py` & `redmage-0.0.5/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/redmage/utils.py` & `redmage-0.0.5/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.4/PKG-INFO` & `redmage-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.0.4
+Version: 0.0.5
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

