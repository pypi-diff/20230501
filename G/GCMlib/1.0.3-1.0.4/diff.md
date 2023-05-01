# Comparing `tmp/GCMlib-1.0.3.tar.gz` & `tmp/GCMlib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GCMlib-1.0.3.tar", last modified: Sat Feb 25 01:19:22 2023, max compression
+gzip compressed data, was "GCMlib-1.0.4.tar", last modified: Mon May  1 20:15:52 2023, max compression
```

## Comparing `GCMlib-1.0.3.tar` & `GCMlib-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:19:22.151542 GCMlib-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:19:22.151542 GCMlib-1.0.3/GCMlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-02-25 01:19:22.000000 GCMlib-1.0.3/GCMlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-25 01:19:22.000000 GCMlib-1.0.3/GCMlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 01:19:22.000000 GCMlib-1.0.3/GCMlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-25 01:19:22.000000 GCMlib-1.0.3/GCMlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-25 01:19:22.000000 GCMlib-1.0.3/GCMlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-25 01:19:12.000000 GCMlib-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-02-25 01:19:22.151542 GCMlib-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-02-25 01:19:12.000000 GCMlib-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-02-25 01:19:12.000000 GCMlib-1.0.3/gcm.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 01:19:22.151542 GCMlib-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-25 01:19:12.000000 GCMlib-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:15:52.091858 GCMlib-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:15:52.091858 GCMlib-1.0.4/GCMlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-01 20:15:52.000000 GCMlib-1.0.4/GCMlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 20:15:52.000000 GCMlib-1.0.4/GCMlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:15:52.000000 GCMlib-1.0.4/GCMlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 20:15:52.000000 GCMlib-1.0.4/GCMlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-01 20:15:52.000000 GCMlib-1.0.4/GCMlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 20:15:41.000000 GCMlib-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-01 20:15:52.091858 GCMlib-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-01 20:15:41.000000 GCMlib-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-01 20:15:41.000000 GCMlib-1.0.4/gcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:15:52.091858 GCMlib-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-01 20:15:41.000000 GCMlib-1.0.4/setup.py
```

### Comparing `GCMlib-1.0.3/GCMlib.egg-info/PKG-INFO` & `GCMlib-1.0.4/GCMlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCMlib
-Version: 1.0.3
+Version: 1.0.4
 Summary: A minimalistic and simple encryption library. For encrypting data using AES GCM mode.
 Home-page: https://github.com/therealOri/GCMlib
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GCMlib-1.0.3/LICENSE` & `GCMlib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GCMlib-1.0.3/PKG-INFO` & `GCMlib-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCMlib
-Version: 1.0.3
+Version: 1.0.4
 Summary: A minimalistic and simple encryption library. For encrypting data using AES GCM mode.
 Home-page: https://github.com/therealOri/GCMlib
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `GCMlib-1.0.3/README.md` & `GCMlib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `GCMlib-1.0.3/gcm.py` & `GCMlib-1.0.4/gcm.py`

 * *Files identical despite different names*

### Comparing `GCMlib-1.0.3/setup.py` & `GCMlib-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GCMlib",
-    version="1.0.3",
+    version="1.0.4",
     author="therealOri",
     license="GPL-3.0",
     install_requires=[
-        "alive-progress==2.4.1",
-        "pycryptodome==3.17",
-        "argon2-cffi==21.3.0"
+        "alive-progress",
+        "pycryptodome",
+        "argon2-cffi"
     ],
     author_email="therealOri@duck.com",
     description="A minimalistic and simple encryption library. For encrypting data using AES GCM mode.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/therealOri/GCMlib",
 )
```

