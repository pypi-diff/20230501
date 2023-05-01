# Comparing `tmp/insidecouchbase-0.1.0.tar.gz` & `tmp/insidecouchbase-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidecouchbase-0.1.0.tar", last modified: Fri Apr 21 23:15:57 2023, max compression
+gzip compressed data, was "insidecouchbase-1.0.0.tar", last modified: Mon May  1 12:39:51 2023, max compression
```

## Comparing `insidecouchbase-0.1.0.tar` & `insidecouchbase-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-21 20:42:51.000000 insidecouchbase-0.1.0/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     9451 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     8871 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-21 20:42:51.000000 insidecouchbase-0.1.0/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/src/couchbase/
--rw-rw-r--   0 demir     (1000) demir     (1000)       36 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/src/couchbase/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    19737 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/src/couchbase/couchbase.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     9451 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 12:39:51.421587 insidecouchbase-1.0.0/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-21 20:42:51.000000 insidecouchbase-1.0.0/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4557 2023-05-01 12:39:51.421587 insidecouchbase-1.0.0/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3977 2023-05-01 12:39:43.000000 insidecouchbase-1.0.0/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-21 20:42:51.000000 insidecouchbase-1.0.0/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-05-01 12:39:51.421587 insidecouchbase-1.0.0/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-05-01 12:39:43.000000 insidecouchbase-1.0.0/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 12:39:51.421587 insidecouchbase-1.0.0/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 12:39:51.421587 insidecouchbase-1.0.0/src/couchbase/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       36 2023-04-21 23:15:49.000000 insidecouchbase-1.0.0/src/couchbase/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    14624 2023-05-01 12:39:43.000000 insidecouchbase-1.0.0/src/couchbase/couchbase.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 12:39:51.421587 insidecouchbase-1.0.0/src/insidecouchbase.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4557 2023-05-01 12:39:51.000000 insidecouchbase-1.0.0/src/insidecouchbase.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-05-01 12:39:51.000000 insidecouchbase-1.0.0/src/insidecouchbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-01 12:39:51.000000 insidecouchbase-1.0.0/src/insidecouchbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-05-01 12:39:51.000000 insidecouchbase-1.0.0/src/insidecouchbase.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-05-01 12:39:51.000000 insidecouchbase-1.0.0/src/insidecouchbase.egg-info/top_level.txt
```

### Comparing `insidecouchbase-0.1.0/LICENSE` & `insidecouchbase-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.1.0/setup.cfg` & `insidecouchbase-1.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = insidecocuhbase
-version = 0.1.0
+version = 1.0.0
 author = Huseyin Demir
 author_email = huseyin.d3r@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/adiosamig/insidecocuhbase
 project_urls =
```

### Comparing `insidecouchbase-0.1.0/setup.py` & `insidecouchbase-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidecouchbase",
-    version = "0.1.0",
+    version = "1.0.0",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidecocuhbase",
     install_requires=[
```

