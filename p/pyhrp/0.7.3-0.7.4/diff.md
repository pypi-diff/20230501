# Comparing `tmp/pyhrp-0.7.3.tar.gz` & `tmp/pyhrp-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhrp-0.7.3.tar", max compression
+gzip compressed data, was "pyhrp-0.7.4.tar", max compression
```

## Comparing `pyhrp-0.7.3.tar` & `pyhrp-0.7.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1083 2023-04-30 13:47:32.430232 pyhrp-0.7.3/LICENSE.txt
--rw-r--r--   0        0        0     1515 2023-04-30 13:47:32.430232 pyhrp-0.7.3/README.md
--rwxr-xr-x   0        0        0        0 2023-04-30 13:47:32.430232 pyhrp-0.7.3/pyhrp/__init__.py
--rw-r--r--   0        0        0     3047 2023-04-30 13:47:32.430232 pyhrp-0.7.3/pyhrp/cluster.py
--rw-r--r--   0        0        0      309 2023-04-30 13:47:32.430232 pyhrp-0.7.3/pyhrp/graph.py
--rw-r--r--   0        0        0     2559 2023-04-30 13:47:32.430232 pyhrp-0.7.3/pyhrp/hrp.py
--rw-r--r--   0        0        0     2250 2023-04-30 13:47:32.430232 pyhrp-0.7.3/pyhrp/marcos.py
--rw-r--r--   0        0        0      479 2023-04-30 13:47:58.082420 pyhrp-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.7.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2023-05-01 00:59:27.025410 pyhrp-0.7.4/LICENSE.txt
+-rw-r--r--   0        0        0     1515 2023-05-01 00:59:27.025410 pyhrp-0.7.4/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-01 00:59:27.025410 pyhrp-0.7.4/pyhrp/__init__.py
+-rw-r--r--   0        0        0     3047 2023-05-01 00:59:27.025410 pyhrp-0.7.4/pyhrp/cluster.py
+-rw-r--r--   0        0        0      309 2023-05-01 00:59:27.025410 pyhrp-0.7.4/pyhrp/graph.py
+-rw-r--r--   0        0        0     2559 2023-05-01 00:59:27.025410 pyhrp-0.7.4/pyhrp/hrp.py
+-rw-r--r--   0        0        0     2250 2023-05-01 00:59:27.025410 pyhrp-0.7.4/pyhrp/marcos.py
+-rw-r--r--   0        0        0      479 2023-05-01 00:59:52.169759 pyhrp-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 pyhrp-0.7.4/PKG-INFO
```

### Comparing `pyhrp-0.7.3/LICENSE.txt` & `pyhrp-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhrp-0.7.3/README.md` & `pyhrp-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhrp-0.7.3/pyhrp/cluster.py` & `pyhrp-0.7.4/pyhrp/cluster.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.7.3/pyhrp/hrp.py` & `pyhrp-0.7.4/pyhrp/hrp.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.7.3/pyhrp/marcos.py` & `pyhrp-0.7.4/pyhrp/marcos.py`

 * *Files identical despite different names*

### Comparing `pyhrp-0.7.3/PKG-INFO` & `pyhrp-0.7.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhrp
-Version: 0.7.3
+Version: 0.7.4
 Summary: ...
 Home-page: https://github.com/tschm/pyhrp
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

