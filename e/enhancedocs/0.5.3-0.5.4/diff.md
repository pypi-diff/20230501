# Comparing `tmp/enhancedocs-0.5.3.tar.gz` & `tmp/enhancedocs-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.3.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.4.tar", max compression
```

## Comparing `enhancedocs-0.5.3.tar` & `enhancedocs-0.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/LICENSE
--rw-r--r--   0        0        0     1030 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/README.md
--rw-r--r--   0        0        0      474 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      778 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0     1315 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/build.py
--rw-r--r--   0        0        0     1842 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/commands/push.py
--rw-r--r--   0        0        0     1151 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/config.py
--rw-r--r--   0        0        0      611 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/main.py
--rw-r--r--   0        0        0     1212 2023-04-28 15:37:31.662551 enhancedocs-0.5.3/src/enhancedocs/utils.py
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/README.md
+-rw-r--r--   0        0        0      478 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0     1150 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0     1842 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0     1151 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/config.py
+-rw-r--r--   0        0        0      611 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/main.py
+-rw-r--r--   0        0        0     1212 2023-05-01 14:49:12.426057 enhancedocs-0.5.4/src/enhancedocs/utils.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 enhancedocs-0.5.4/PKG-INFO
```

### Comparing `enhancedocs-0.5.3/LICENSE` & `enhancedocs-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/README.md` & `enhancedocs-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/src/enhancedocs/commands/build.py` & `enhancedocs-0.5.4/src/enhancedocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/src/enhancedocs/commands/push.py` & `enhancedocs-0.5.4/src/enhancedocs/commands/push.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/src/enhancedocs/config.py` & `enhancedocs-0.5.4/src/enhancedocs/config.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/src/enhancedocs/main.py` & `enhancedocs-0.5.4/src/enhancedocs/main.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/src/enhancedocs/utils.py` & `enhancedocs-0.5.4/src/enhancedocs/utils.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.3/PKG-INFO` & `enhancedocs-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.3
+Version: 0.5.4
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

