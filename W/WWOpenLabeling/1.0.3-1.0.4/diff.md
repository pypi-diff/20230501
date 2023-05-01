# Comparing `tmp/WWOpenLabeling-1.0.3.tar.gz` & `tmp/WWOpenLabeling-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/WWOpenLabeling-1.0.3.tar", last modified: Mon May  1 21:32:16 2023, max compression
+gzip compressed data, was "dist/WWOpenLabeling-1.0.4.tar", last modified: Mon May  1 21:38:12 2023, max compression
```

## Comparing `WWOpenLabeling-1.0.3.tar` & `WWOpenLabeling-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/
--rw-r--r--   0 nrozanov   (501) staff       (20)    11357 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/LICENSE
--rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/PKG-INFO
--rw-r--r--   0 nrozanov   (501) staff       (20)     5783 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/README.md
-drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/
--rwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 08:08:29.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/__init__.py
--rwxr-xr-x   0 nrozanov   (501) staff       (20)    52951 2023-05-01 20:30:07.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/annotator.py
--rw-r--r--   0 nrozanov   (501) staff       (20)     4277 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/dasiamrpn.py
--rwxr-xr-x   0 nrozanov   (501) staff       (20)     3428 2023-05-01 21:28:48.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/main.py
--rwxr-xr-x   0 nrozanov   (501) staff       (20)    30588 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.3/WWOpenLabeling/main_auto.py
-drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/
--rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/PKG-INFO
--rw-r--r--   0 nrozanov   (501) staff       (20)      349 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/SOURCES.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)        1 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/dependency_links.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)      127 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/requires.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)       15 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/WWOpenLabeling.egg-info/top_level.txt
--rw-r--r--   0 nrozanov   (501) staff       (20)       38 2023-05-01 21:32:16.000000 WWOpenLabeling-1.0.3/setup.cfg
--rw-r--r--   0 nrozanov   (501) staff       (20)      479 2023-05-01 21:32:07.000000 WWOpenLabeling-1.0.3/setup.py
+drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:38:12.000000 WWOpenLabeling-1.0.4/
+-rw-r--r--   0 nrozanov   (501) staff       (20)    11357 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.4/LICENSE
+-rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:38:12.000000 WWOpenLabeling-1.0.4/PKG-INFO
+-rw-r--r--   0 nrozanov   (501) staff       (20)     5783 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.4/README.md
+drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:38:12.000000 WWOpenLabeling-1.0.4/WWOpenLabeling/
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 08:08:29.000000 WWOpenLabeling-1.0.4/WWOpenLabeling/__init__.py
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)    52951 2023-05-01 20:30:07.000000 WWOpenLabeling-1.0.4/WWOpenLabeling/annotator.py
+-rw-r--r--   0 nrozanov   (501) staff       (20)     4277 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.4/WWOpenLabeling/dasiamrpn.py
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)     3398 2023-05-01 21:37:47.000000 WWOpenLabeling-1.0.4/WWOpenLabeling/main.py
+-rwxr-xr-x   0 nrozanov   (501) staff       (20)    30588 2023-05-01 07:41:37.000000 WWOpenLabeling-1.0.4/WWOpenLabeling/main_auto.py
+drwxr-xr-x   0 nrozanov   (501) staff       (20)        0 2023-05-01 21:38:12.000000 WWOpenLabeling-1.0.4/WWOpenLabeling.egg-info/
+-rw-r--r--   0 nrozanov   (501) staff       (20)      168 2023-05-01 21:38:11.000000 WWOpenLabeling-1.0.4/WWOpenLabeling.egg-info/PKG-INFO
+-rw-r--r--   0 nrozanov   (501) staff       (20)      349 2023-05-01 21:38:11.000000 WWOpenLabeling-1.0.4/WWOpenLabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)        1 2023-05-01 21:38:11.000000 WWOpenLabeling-1.0.4/WWOpenLabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)      127 2023-05-01 21:38:11.000000 WWOpenLabeling-1.0.4/WWOpenLabeling.egg-info/requires.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)       15 2023-05-01 21:38:11.000000 WWOpenLabeling-1.0.4/WWOpenLabeling.egg-info/top_level.txt
+-rw-r--r--   0 nrozanov   (501) staff       (20)       38 2023-05-01 21:38:12.000000 WWOpenLabeling-1.0.4/setup.cfg
+-rw-r--r--   0 nrozanov   (501) staff       (20)      479 2023-05-01 21:37:59.000000 WWOpenLabeling-1.0.4/setup.py
```

### Comparing `WWOpenLabeling-1.0.3/LICENSE` & `WWOpenLabeling-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.3/README.md` & `WWOpenLabeling-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.3/WWOpenLabeling/annotator.py` & `WWOpenLabeling-1.0.4/WWOpenLabeling/annotator.py`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.3/WWOpenLabeling/dasiamrpn.py` & `WWOpenLabeling-1.0.4/WWOpenLabeling/dasiamrpn.py`

 * *Files identical despite different names*

### Comparing `WWOpenLabeling-1.0.3/WWOpenLabeling/main.py` & `WWOpenLabeling-1.0.4/WWOpenLabeling/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
-from WWOpenLabeling.annotator import run
+from annotator import run
 
 import argparse
 import asyncio
-from WWOpenLabeling.helper_utils.annotation_file_manager import AnnotationFileManager
+from helper_utils.annotation_file_manager import AnnotationFileManager
 
 import os
 import shutil
 import subprocess
 from lxml import etree
 
 def prepare(input_folder_name, output_folder_name):
```

### Comparing `WWOpenLabeling-1.0.3/WWOpenLabeling/main_auto.py` & `WWOpenLabeling-1.0.4/WWOpenLabeling/main_auto.py`

 * *Files identical despite different names*

