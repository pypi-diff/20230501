# Comparing `tmp/WWOpenLabeling-1.0.1.tar.gz` & `tmp/WWOpenLabeling-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/WWOpenLabeling-1.0.1.tar", last modified: Mon May  1 21:21:45 2023, max compression
+gzip compressed data, was "dist/WWOpenLabeling-1.0.3.tar", last modified: Mon May  1 21:32:16 2023, max compression
```

## Comparing `WWOpenLabeling-1.0.1.tar` & `WWOpenLabeling-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/
--rw-r--r--   0 nrozanov   (501) staff       (20)    11357 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.1/LICENSE
--rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/PKG-INFO
--rw-r--r--   0 nrozanov   (501) staff       (20)     5783 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.1/README.md
-drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling/
--rwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 08:08:29.000000 WWOpenLabeling-1.0.1/WWOpenLabeling/__init__.py
--rwxr-xr-x   0 nrozanov   (501) staff       (20)    52951 2023-05-01 20:30:07.000000 WWOpenLabeling-1.0.1/WWOpenLabeling/annotator.py
--rw-r--r--   0 nrozanov   (501) staff       (20)     4277 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.1/WWOpenLabeling/dasiamrpn.py
--rwxr-xr-x   0 nrozanov   (501) staff       (20)     3451 2023-05-01 21:20:32.000000 WWOpenLabeling-1.0.1/WWOpenLabeling/main.py
--rwxr-xr-x   0 nrozanov   (501) staff       (20)    30588 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.1/WWOpenLabeling/main_auto.py
-drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling.egg-info/
--rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling.egg-info/PKG-INFO
--rw-r--r--   0 nrozanov   (501) staff       (20)      349 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling.egg-info/SOURCES.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)        1 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling.egg-info/dependency_links.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)      127 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling.egg-info/requires.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)       15 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/WWOpenLabeling.egg-info/top_level.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)       38 2023-05-01 21:21:45.000000 WWOpenLabeling-1.0.1/setup.cfg
--rw-r--r--   0 nrozanov   (501) staff       (20)      479 2023-05-01 21:21:39.000000 WWOpenLabeling-1.0.1/setup.py
+drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/
+-rw-r--r--   0 nrozanov   (501) staff       (20)    11357 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/LICENSE
+-rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/PKG-INFO
+-rw-r--r--   0 nrozanov   (501) staff       (20)     5783 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/README.md
+drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 08:08:29.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/__init__.py
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)    52951 2023-05-01 20:30:07.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/annotator.py
+-rw-r--r--   0 nrozanov   (501) staff       (20)     4277 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/dasiamrpn.py
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)     3428 2023-05-01 21:28:48.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/main.py
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)    30588 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/main_auto.py
+drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/
+-rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/PKG-INFO
+-rw-r--r--   0 nrozanov   (501) staff       (20)      349 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)        1 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)      127 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/requires.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)       15 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/top_level.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)       38 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/setup.cfg
+-rw-r--r--   0 nrozanov   (501) staff       (20)      479 2023-05-01 21:32:07.000000 WWOpenLabeling-1.0.3/setup.py
```

### Comparing `WWOpenLabeling-1.0.1/LICENSE` & `WWOpenLabeling-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.1/README.md` & `WWOpenLabeling-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.1/WWOpenLabeling/annotator.py` & `WWOpenLabeling-1.0.3/WWOpenLabeling/annotator.py`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.1/WWOpenLabeling/dasiamrpn.py` & `WWOpenLabeling-1.0.3/WWOpenLabeling/dasiamrpn.py`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.1/WWOpenLabeling/main.py` & `WWOpenLabeling-1.0.3/WWOpenLabeling/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 
-import setuptools
-print(setuptools.find_packages())
-
-from annotator import run
+from WWOpenLabeling.annotator import run
 
 import argparse
 import asyncio
-from helper_utils.annotation_file_manager import AnnotationFileManager
+from WWOpenLabeling.helper_utils.annotation_file_manager import AnnotationFileManager
 
 import os
 import shutil
 import subprocess
 from lxml import etree
 
 def prepare(input_folder_name, output_folder_name):
```

### Comparing `WWOpenLabeling-1.0.1/WWOpenLabeling/main_auto.py` & `WWOpenLabeling-1.0.3/WWOpenLabeling/main_auto.py`

 * *Files identical despite different names*

