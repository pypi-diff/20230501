# Comparing `tmp/wallabag2readwise-1.4.6.tar.gz` & `tmp/wallabag2readwise-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallabag2readwise-1.4.6.tar", last modified: Wed Apr  5 21:44:50 2023, max compression
+gzip compressed data, was "wallabag2readwise-1.4.7.tar", last modified: Mon May  1 20:01:11 2023, max compression
```

## Comparing `wallabag2readwise-1.4.6.tar` & `wallabag2readwise-1.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:44:50.631111 wallabag2readwise-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-05 21:44:50.631111 wallabag2readwise-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 21:44:50.631111 wallabag2readwise-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:44:50.631111 wallabag2readwise-1.4.6/wallabag2readwise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-05 21:44:47.000000 wallabag2readwise-1.4.6/wallabag2readwise/wallabag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 21:44:50.631111 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-05 21:44:50.000000 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-05 21:44:50.000000 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 21:44:50.000000 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-05 21:44:50.000000 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 21:44:50.000000 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 21:44:50.000000 wallabag2readwise-1.4.6/wallabag2readwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:11.018897 wallabag2readwise-1.4.7/wallabag2readwise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-01 20:01:08.000000 wallabag2readwise-1.4.7/wallabag2readwise/wallabag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:01:11.022897 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 20:01:11.000000 wallabag2readwise-1.4.7/wallabag2readwise.egg-info/top_level.txt
```

### Comparing `wallabag2readwise-1.4.6/LICENSE` & `wallabag2readwise-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/PKG-INFO` & `wallabag2readwise-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallabag2readwise
-Version: 1.4.6
+Version: 1.4.7
 Summary: Push wallabag annotations to Readwise highlights
 Home-page: https://github.com/rwxd/wallabag2readwise
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wallabag2readwise-1.4.6/README.md` & `wallabag2readwise-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/setup.py` & `wallabag2readwise-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/wallabag2readwise/cli.py` & `wallabag2readwise-1.4.7/wallabag2readwise/cli.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/wallabag2readwise/misc.py` & `wallabag2readwise-1.4.7/wallabag2readwise/misc.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/wallabag2readwise/models.py` & `wallabag2readwise-1.4.7/wallabag2readwise/models.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/wallabag2readwise/wallabag.py` & `wallabag2readwise-1.4.7/wallabag2readwise/wallabag.py`

 * *Files identical despite different names*

### Comparing `wallabag2readwise-1.4.6/wallabag2readwise.egg-info/PKG-INFO` & `wallabag2readwise-1.4.7/wallabag2readwise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallabag2readwise
-Version: 1.4.6
+Version: 1.4.7
 Summary: Push wallabag annotations to Readwise highlights
 Home-page: https://github.com/rwxd/wallabag2readwise
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `wallabag2readwise-1.4.6/wallabag2readwise.egg-info/SOURCES.txt` & `wallabag2readwise-1.4.7/wallabag2readwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

