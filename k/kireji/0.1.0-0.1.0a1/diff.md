# Comparing `tmp/kireji-0.1.0.tar.gz` & `tmp/kireji-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kireji-0.1.0.tar", last modified: Mon May  1 01:16:12 2023, max compression
+gzip compressed data, was "kireji-0.1.0a1.tar", last modified: Sun Apr 30 23:49:42 2023, max compression
```

## Comparing `kireji-0.1.0.tar` & `kireji-0.1.0a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:16:12.208960 kireji-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-01 01:16:12.208960 kireji-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:16:12.208960 kireji-0.1.0/kireji/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-01 01:15:37.000000 kireji-0.1.0/kireji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 01:15:37.000000 kireji-0.1.0/kireji/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:16:12.208960 kireji-0.1.0/kireji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-01 01:16:12.000000 kireji-0.1.0/kireji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 01:16:12.000000 kireji-0.1.0/kireji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 01:16:12.000000 kireji-0.1.0/kireji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 01:16:12.000000 kireji-0.1.0/kireji.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 01:16:12.000000 kireji-0.1.0/kireji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 01:16:12.000000 kireji-0.1.0/kireji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-01 01:15:37.000000 kireji-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-01 01:15:37.000000 kireji-0.1.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 01:16:12.208960 kireji-0.1.0/setup.cfg
+drwxr-xr-x   0 stv       (1000) stv       (1000)        0 2023-04-30 23:49:42.708711 kireji-0.1.0a1/
+-rw-r--r--   0 stv       (1000) stv       (1000)     3405 2023-04-30 23:49:42.708711 kireji-0.1.0a1/PKG-INFO
+drwxr-xr-x   0 stv       (1000) stv       (1000)        0 2023-04-30 23:49:42.708711 kireji-0.1.0a1/kireji/
+-rw-r--r--   0 stv       (1000) stv       (1000)      161 2023-04-30 23:48:39.000000 kireji-0.1.0a1/kireji/__init__.py
+-rw-r--r--   0 stv       (1000) stv       (1000)      244 2023-04-30 21:34:55.000000 kireji-0.1.0a1/kireji/__main__.py
+drwxr-xr-x   0 stv       (1000) stv       (1000)        0 2023-04-30 23:49:42.708711 kireji-0.1.0a1/kireji.egg-info/
+-rw-r--r--   0 stv       (1000) stv       (1000)     3405 2023-04-30 23:49:42.000000 kireji-0.1.0a1/kireji.egg-info/PKG-INFO
+-rw-r--r--   0 stv       (1000) stv       (1000)      244 2023-04-30 23:49:42.000000 kireji-0.1.0a1/kireji.egg-info/SOURCES.txt
+-rw-r--r--   0 stv       (1000) stv       (1000)        1 2023-04-30 23:49:42.000000 kireji-0.1.0a1/kireji.egg-info/dependency_links.txt
+-rw-r--r--   0 stv       (1000) stv       (1000)       48 2023-04-30 23:49:42.000000 kireji-0.1.0a1/kireji.egg-info/entry_points.txt
+-rw-r--r--   0 stv       (1000) stv       (1000)       11 2023-04-30 23:49:42.000000 kireji-0.1.0a1/kireji.egg-info/requires.txt
+-rw-r--r--   0 stv       (1000) stv       (1000)        7 2023-04-30 23:49:42.000000 kireji-0.1.0a1/kireji.egg-info/top_level.txt
+-rw-r--r--   0 stv       (1000) stv       (1000)      931 2023-04-30 23:37:19.000000 kireji-0.1.0a1/pyproject.toml
+-rw-r--r--   0 stv       (1000) stv       (1000)     2784 2023-04-30 23:49:29.000000 kireji-0.1.0a1/readme.md
+-rw-r--r--   0 stv       (1000) stv       (1000)       38 2023-04-30 23:49:42.708711 kireji-0.1.0a1/setup.cfg
```

### Comparing `kireji-0.1.0/PKG-INFO` & `kireji-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kireji
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: A plaintext note-taking CLI in Python.
 Author-email: Stephen Malone <mail@wirehaiku.org>
 License: BSD-3-Clause
 Keywords: note,notes,note-taking,cli
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `kireji-0.1.0/kireji.egg-info/PKG-INFO` & `kireji-0.1.0a1/kireji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kireji
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: A plaintext note-taking CLI in Python.
 Author-email: Stephen Malone <mail@wirehaiku.org>
 License: BSD-3-Clause
 Keywords: note,notes,note-taking,cli
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `kireji-0.1.0/pyproject.toml` & `kireji-0.1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kireji-0.1.0/readme.md` & `kireji-0.1.0a1/readme.md`

 * *Files identical despite different names*

