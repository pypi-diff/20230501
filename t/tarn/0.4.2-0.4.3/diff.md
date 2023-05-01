# Comparing `tmp/tarn-0.4.2.tar.gz` & `tmp/tarn-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.4.2.tar", last modified: Mon Apr 10 17:04:47 2023, max compression
+gzip compressed data, was "tarn-0.4.3.tar", last modified: Mon May  1 17:00:35 2023, max compression
```

## Comparing `tarn-0.4.2.tar` & `tarn-0.4.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-10 17:04:45.000000 tarn-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 17:04:45.000000 tarn-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 17:04:47.766092 tarn-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-10 17:04:45.000000 tarn-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-10 17:04:45.000000 tarn-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 17:04:45.000000 tarn-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:04:47.766092 tarn-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-10 17:04:45.000000 tarn-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.762092 tarn-0.4.2/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.766092 tarn-0.4.2/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-10 17:04:45.000000 tarn-0.4.2/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:04:47.762092 tarn-0.4.2/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 17:04:47.000000 tarn-0.4.2/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-10 17:04:47.000000 tarn-0.4.2/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:04:47.000000 tarn-0.4.2/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 17:04:47.000000 tarn-0.4.2/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 17:04:47.000000 tarn-0.4.2/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-01 17:00:33.000000 tarn-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 17:00:33.000000 tarn-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-01 17:00:35.760567 tarn-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-01 17:00:33.000000 tarn-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-01 17:00:33.000000 tarn-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 17:00:33.000000 tarn-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:00:35.760567 tarn-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-01 17:00:33.000000 tarn-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.760567 tarn-0.4.3/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-01 17:00:33.000000 tarn-0.4.3/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:00:35.756569 tarn-0.4.3/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 17:00:35.000000 tarn-0.4.3/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.4.2/LICENSE` & `tarn-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/PKG-INFO` & `tarn-0.4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.4.2
+Version: 0.4.3
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.2.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.3.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.4.2/README.md` & `tarn-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/pyproject.toml` & `tarn-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/setup.py` & `tarn-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/cache/storage.py` & `tarn-0.4.3/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/compat.py` & `tarn-0.4.3/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/config.py` & `tarn-0.4.3/tarn/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from typing import Any, Dict, Sequence, Tuple, Union
 
 import humanfriendly
 from pydantic import BaseModel, Extra, root_validator, validator
 from yaml import safe_dump, safe_load
 
 from .compat import get_path_group
+from .interface import PathOrStr
 from .tools import DummyLocker, DummySize, DummyUsage, Locker, SizeTracker, UsageTracker
-from .utils import PathLike, mkdir
+from .utils import mkdir
 
 CONFIG_NAME = 'config.yml'
 
 
 class _NoExtra(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -111,15 +112,15 @@
     return stat.st_mode & 0o777, get_path_group(root)
 
 
 def load_config_buffer(data: str) -> StorageConfig:
     return StorageConfig.parse_obj(safe_load(io.StringIO(data)))
 
 
-def load_config(root: PathLike) -> StorageConfig:
+def load_config(root: PathOrStr) -> StorageConfig:
     with open(Path(root) / CONFIG_NAME) as file:
         return StorageConfig.parse_obj(safe_load(file))
 
 
 def parse_size(x):
     if isinstance(x, int):
         return x
@@ -133,14 +134,14 @@
     for cls in base.__subclasses__():
         if cls.__name__ == name:
             return cls
 
     raise ValueError(f'Could not find a {base.__name__} named {name}')
 
 
-def init_storage(config: StorageConfig, root: PathLike, *,
+def init_storage(config: StorageConfig, root: PathOrStr, *,
                  permissions: Union[int, None] = None, group: Union[str, int, None] = None, exist_ok: bool = False):
     root = Path(root)
     mkdir(root, permissions, group, parents=True, exist_ok=exist_ok)
 
     with open(root / CONFIG_NAME, 'w') as file:
         safe_dump(config.dict(), file)
```

### Comparing `tarn-0.4.2/tarn/digest.py` & `tarn-0.4.3/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/interface.py` & `tarn-0.4.3/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/local/storage.py` & `tarn-0.4.3/tarn/local/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import logging
 import warnings
 from pathlib import Path
 from typing import Iterable, Optional, Sequence, Union
 
-from ..interface import Key
+from ..interface import Key, PathOrStr
 from ..location import Fanout, Level, Levels, Location
 from ..pool import HashKeyStorage
 from ..pool.hash_key import resolve_location
-from ..utils import PathLike
 from .disk import Disk
 
 logger = logging.getLogger(__name__)
 
 
 class Storage(HashKeyStorage):
-    def __init__(self, *local: Union[Level, Sequence[Disk], Disk, Sequence[PathLike], PathLike],
+    def __init__(self, *local: Union[Level, Sequence[Disk], Disk, Sequence[PathOrStr], PathOrStr],
                  remote: Sequence[Location] = ()):
         warnings.warn('This interface is deprecated. Use `HashKeyStorage` instead', UserWarning)
         warnings.warn('This interface is deprecated. Use `HashKeyStorage` instead', DeprecationWarning)
         super().__init__(Levels(*map(_resolve, local)), remote)
 
     @property
     def levels(self):
```

### Comparing `tarn-0.4.2/tarn/location/disk_dict.py` & `tarn-0.4.3/tarn/location/disk_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         self.levels = config.levels
         self.hash = config.hash.build()
         assert self.hash().digest_size == sum(self.levels)
 
         self.root = root
         self.permissions, self.group = root_params(self.root)
         usage_folder = self.root / 'tools/usage'
-        # FIXME: race condition
         create_folders(usage_folder, self.permissions, self.group)
 
         self.locker: Locker = config.make_locker()
         self.size_tracker: SizeTracker = config.make_size()
         self.usage_tracker: UsageTracker = config.make_usage(usage_folder)
         self.min_free_size = config.free_disk_size
         self.max_size = config.max_size
@@ -77,39 +76,43 @@
             try:
                 # if already stored
                 if file.exists():
                     # TODO: legacy
                     if file.is_dir():
                         file = file / 'data'
 
-                    if _is_pathlike(value):
-                        match_files(value, file)
-                    else:
-                        with open(file, 'rb') as dst:
-                            match_buffers(value, dst, context=key.hex())
-
+                    _match(value, file, key)
                     yield file
                     return
 
                 # make sure we can write
                 if not self._writeable():
                     yield
                     return
 
                 try:
                     # create base folders
                     create_folders(file.parent, self.permissions, self.group)
                     # populate the folder
-                    if _is_pathlike(value):
-                        copy_file(value, file)
-                    else:
-                        with open(file, 'wb') as dst:
-                            shutil.copyfileobj(value, dst)
+                    # TODO: make this an atomic operation
+                    #  now this is just an ugly crutch
+                    try:
+                        if _is_pathlike(value):
+                            copy_file(value, file)
+                        else:
+                            with open(file, 'wb') as dst:
+                                shutil.copyfileobj(value, dst)
+
+                    except PermissionError:
+                        if not file.exists():
+                            raise
+                        _match(value, file, key)
 
-                    adjust_permissions(file, self.permissions, self.group, read_only=True)
+                    else:
+                        adjust_permissions(file, self.permissions, self.group, read_only=True)
 
                 except BaseException as e:
                     if file.exists():
                         remove_file(file)
                     raise RuntimeError('An error occurred while copying the file') from e
 
                 # metadata
@@ -155,7 +158,15 @@
             result = result and self.size_tracker.get(self.root) <= self.max_size
 
         return result
 
 
 def _is_pathlike(x):
     return isinstance(x, (os.PathLike, str))
+
+
+def _match(value, file, key):
+    if _is_pathlike(value):
+        match_files(value, file)
+    else:
+        with open(file, 'rb') as dst:
+            match_buffers(value, dst, context=key.hex())
```

### Comparing `tarn-0.4.2/tarn/location/fanout.py` & `tarn-0.4.3/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/location/interface.py` & `tarn-0.4.3/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/location/levels.py` & `tarn-0.4.3/tarn/location/levels.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     replicate: bool = True
     name: Optional[str] = None
 
 
 class Levels(Writable):
     def __init__(self, *levels: Union[Level, Location]):
         levels = [
-            Level(level, write=True, replicate=True) if isinstance(level, Location) else level
+            level if isinstance(level, Level) else Level(level, write=True, replicate=True)
             for level in levels
         ]
         sizes = {level.location.key_size for level in levels if level.location.key_size is not None}
         hashes = {level.location.hash for level in levels if level.location.hash is not None}
         assert len(sizes) <= 1, sizes
         assert len(hashes) <= 1, hashes
```

### Comparing `tarn-0.4.2/tarn/location/nginx.py` & `tarn-0.4.3/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/location/scp.py` & `tarn-0.4.3/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/pickler/compat.py` & `tarn-0.4.3/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/pickler/interface.py` & `tarn-0.4.3/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/pool/hash_key.py` & `tarn-0.4.3/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/pool/pickle_key.py` & `tarn-0.4.3/tarn/pool/pickle_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
                 if file.is_dir():
                     continue
 
                 relative = str(file.relative_to(temp_folder))
                 assert relative not in mapping
                 mapping[relative] = self.storage.write(file).hex()
 
+        # we want a reproducible mapping each time
+        mapping = {k: mapping[k] for k in sorted(mapping)}
         logger.info('Saving to index %s', digest)
         with self.index.write(digest, BytesIO(json.dumps(mapping).encode())) as written:
             if written is None:
                 if error:
                     raise WriteError('The index could not be written to any storage')
                 return None
```

### Comparing `tarn-0.4.2/tarn/serializers.py` & `tarn-0.4.3/tarn/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,19 +164,19 @@
 
     def save(self, data: dict, folder: Path):
         if not isinstance(data, dict):
             raise SerializerError
 
         try:
             keys_to_folder = {}
-            for index, (key, value) in enumerate(data.items()):
+            for index, key in enumerate(sorted(data)):
                 keys_to_folder[index] = key
                 sub_folder = folder / str(index)
                 sub_folder.mkdir()
-                self.serializer.save(value, sub_folder)
+                self.serializer.save(data[key], sub_folder)
 
         except SerializerError:
             # remove the partially saved object
             for sub_folder in folder.iterdir():
                 rmtree(sub_folder)
 
             raise
```

### Comparing `tarn-0.4.2/tarn/tools/locker.py` & `tarn-0.4.3/tarn/tools/locker.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,36 +80,41 @@
         sleep_time = 0.1
         sleep_iters = int(self._expire / sleep_time) or 1
         wait_for_true(self._start_reading, key, sleep_time, sleep_iters)
 
         try:
             yield
         finally:
-            self._safe_eval(self._stop_reading_script, 1, self._prefix + key)
+            success = self._safe_eval(self._stop_reading_script, 1, self._prefix + key)
+        if not success:
+            raise RuntimeError('The locker is in a wrong state. Did it expire?')
 
     @contextmanager
     def write(self, key: Key) -> ContextManager[None]:
         sleep_time = 0.1
         sleep_iters = int(self._expire / sleep_time) or 1
         wait_for_true(self._start_writing, key, sleep_time, sleep_iters)
 
         try:
             yield
         finally:
-            self._safe_eval(self._stop_writing_script, 1, self._prefix + key)
+            success = self._safe_eval(self._stop_writing_script, 1, self._prefix + key)
+        if not success:
+            raise RuntimeError('The locker is in a wrong state. Did it expire?')
 
     def _update_scripts(self):
         expire = self._expire
         # TODO: how slow are these checks?
         # language=Lua
         self._stop_writing_script = self._redis.script_load('''
         if redis.call('get', KEYS[1]) == '-1' then
             redis.call('del', KEYS[1])
+            return 1
         else
-            error('')
+            return 0
         end''')
         # language=Lua
         self._start_reading_script = self._redis.script_load(f'''
         local lock = redis.call('get', KEYS[1])
         if lock == '-1' then
             return 0
         elseif lock == false then
@@ -118,28 +123,34 @@
         else
             redis.call('set', KEYS[1], lock + 1, 'EX', {expire})
             return 1
         end''')
         # language=Lua
         self._stop_reading_script = self._redis.script_load(f'''
         local lock = redis.call('get', KEYS[1])
-        if lock == '1' then
+        if lock == false then 
+            return 0
+        elseif lock == '1' then
             redis.call('del', KEYS[1])
+            return 1
         elseif tonumber(lock) < 1 then
-            error('')
+            return 0
         else
             redis.call('set', KEYS[1], lock - 1, 'EX', {expire})
+            return 1
         end''')
 
     def _safe_eval(self, *args):
         try:
             return self._redis.evalsha(*args)
         except NoScriptError:
-            self._update_scripts()
-            return self._redis.evalsha(*args)
+            pass
+
+        self._update_scripts()
+        return self._redis.evalsha(*args)
 
     def _start_writing(self, key: Key) -> bool:
         return bool(self._redis.set(self._prefix + key, -1, nx=True, ex=self._expire))
 
     def _start_reading(self, key: Key) -> bool:
         return bool(self._safe_eval(self._start_reading_script, 1, self._prefix + key))
```

### Comparing `tarn-0.4.2/tarn/tools/size.py` & `tarn-0.4.3/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.2/tarn/tools/usage.py` & `tarn-0.4.3/tarn/tools/usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,10 +54,15 @@
         if mark.exists():
             remove_file(mark)
 
     def get(self, key: Key, path: Path) -> Optional[datetime]:
         mark = self._mark(key)
         if mark.exists():
             return datetime.fromtimestamp(mark.stat().st_mtime)
+        # TODO: legacy
+        if path.exists() and path.is_dir():
+            mark = path / '.time'
+            if mark.exists():
+                return datetime.fromtimestamp(mark.stat().st_mtime)
 
     def _mark(self, key):
         return self.root / key_to_relative(key, (1, len(key) - 1))
```

### Comparing `tarn-0.4.2/tarn/utils.py` & `tarn-0.4.3/tarn/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import filecmp
 from pathlib import Path
 from typing import BinaryIO, Union
 
 from .compat import set_path_attrs
 from .interface import Key  # noqa
 
+# TODO: legacy
 PathLike = Union[Path, str]
 
 
 def to_read_only(path: Path, permissions, group):
     adjust_permissions(path, permissions, group, read_only=True)
```

### Comparing `tarn-0.4.2/tarn.egg-info/PKG-INFO` & `tarn-0.4.3/tarn.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.4.2
+Version: 0.4.3
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.2.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.3.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.4.2/tarn.egg-info/SOURCES.txt` & `tarn-0.4.3/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

