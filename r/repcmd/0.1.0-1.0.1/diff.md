# Comparing `tmp/repcmd-0.1.0.tar.gz` & `tmp/repcmd-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repcmd-0.1.0.tar", max compression
+gzip compressed data, was "repcmd-1.0.1.tar", max compression
```

## Comparing `repcmd-0.1.0.tar` & `repcmd-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-04-24 02:03:16.111352 repcmd-0.1.0/LICENSE-MIT.txt
--rw-r--r--   0        0        0      154 2023-04-29 05:40:31.112335 repcmd-0.1.0/README.md
--rw-r--r--   0        0        0      323 2023-04-29 05:32:54.054085 repcmd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       52 2023-04-29 05:31:54.470770 repcmd-0.1.0/repcmd/__init__.py
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 repcmd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-24 02:03:16.111352 repcmd-1.0.1/LICENSE-MIT.txt
+-rw-r--r--   0        0        0      154 2023-04-29 05:40:31.112335 repcmd-1.0.1/README.md
+-rw-r--r--   0        0        0      335 2023-05-01 00:29:52.579097 repcmd-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      311 2023-05-01 00:30:03.159094 repcmd-1.0.1/repcmd/__init__.py
+-rw-r--r--   0        0        0      419 2023-05-01 00:30:12.629092 repcmd-1.0.1/repcmd/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 repcmd-1.0.1/PKG-INFO
```

### Comparing `repcmd-0.1.0/LICENSE-MIT.txt` & `repcmd-1.0.1/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `repcmd-0.1.0/PKG-INFO` & `repcmd-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: repcmd
-Version: 0.1.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: tamuto
-Author-email: mutomob@infodb.jp
+Author-email: tamuto@infodb.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

