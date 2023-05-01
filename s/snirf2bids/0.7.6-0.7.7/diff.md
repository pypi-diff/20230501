# Comparing `tmp/snirf2bids-0.7.6.tar.gz` & `tmp/snirf2bids-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snirf2bids-0.7.6.tar", last modified: Mon Mar 27 19:05:58 2023, max compression
+gzip compressed data, was "dist/snirf2bids-0.7.7.tar", last modified: Mon May  1 14:42:51 2023, max compression
```

## Comparing `snirf2bids-0.7.6.tar` & `snirf2bids-0.7.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/schema/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-27 19:05:57.000000 snirf2bids-0.7.6/schema/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/schema/channel_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/schema/time_units.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/snirf2bids/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/snirf2bids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/snirf2bids/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48068 2023-03-27 19:05:45.000000 snirf2bids-0.7.6/snirf2bids/snirf2bids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/snirf2bids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-03-27 19:05:57.000000 snirf2bids-0.7.6/snirf2bids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-27 19:05:58.000000 snirf2bids-0.7.6/snirf2bids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:05:57.000000 snirf2bids-0.7.6/snirf2bids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 19:05:57.000000 snirf2bids-0.7.6/snirf2bids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 19:05:57.000000 snirf2bids-0.7.6/snirf2bids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/schema/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/schema/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/schema/channel_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/schema/time_units.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/snirf2bids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/snirf2bids/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48133 2023-05-01 14:42:34.000000 snirf2bids-0.7.7/snirf2bids/snirf2bids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 14:42:51.000000 snirf2bids-0.7.7/snirf2bids.egg-info/top_level.txt
```

### Comparing `snirf2bids-0.7.6/LICENSE` & `snirf2bids-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snirf2bids-0.7.6/PKG-INFO` & `snirf2bids-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snirf2bids
-Version: 0.7.6
+Version: 0.7.7
 Summary: To convert snirf file to bids format.
 Home-page: https://github.com/andyzjc/snirf2bids
 Author: JC
 Author-email: andyzjc@bu.edu
 License: MIT
 Description: 
         ![python](https://img.shields.io/pypi/pyversions/snirf2bids?color=green)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snirf2bids Version: 0.7.6 Summary: To convert snirf
+Metadata-Version: 2.1 Name: snirf2bids Version: 0.7.7 Summary: To convert snirf
 file to bids format. Home-page: https://github.com/andyzjc/snirf2bids Author:
 JC Author-email: andyzjc@bu.edu License: MIT Description: ![python](https://
 img.shields.io/pypi/pyversions/snirf2bids?color=green) [![pypi](https://
 img.shields.io/pypi/v/snirf2bids?color=blue)](https://pypi.org/project/
 snirf2bids/) [![tests](https://github.com/BUNPC/snirf2bids/actions/workflows/
 test.yml/badge.svg)](https://github.com/BUNPC/snirf2bids/actions/workflows/
 test.yml) [![DOI](https://zenodo.org/badge/478632378.svg)](https://zenodo.org/
```

### Comparing `snirf2bids-0.7.6/README.md` & `snirf2bids-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `snirf2bids-0.7.6/schema/schema.json` & `snirf2bids-0.7.7/schema/schema.json`

 * *Files identical despite different names*

### Comparing `snirf2bids-0.7.6/setup.py` & `snirf2bids-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `snirf2bids-0.7.6/snirf2bids/snirf2bids.py` & `snirf2bids-0.7.7/snirf2bids/snirf2bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     if 'ses' in entities:
         name += '_ses-' + entities_dict['ses']
     if 'task' in entities  and key != 'optodes' and key != 'coordsystem' and key != 'scans':
         name += '_task-' + entities_dict['task']
     # Misc entities
     for entity in [entity for entity in entities if entity not in ['sub', 'ses', 'task', 'run']]:
         name += '_' + entity + entities_dict[entity]
-    if 'run' in entities:
+    if 'run' in entities and key != 'optodes' and key != 'coordsystem' and key != 'scans':
         name += '_run-' + entities_dict['run']
     return name
 
 
 def _pull_participant(field, fpath=None):
     """Obtains the value for specific fields in the participants.tsv file (minimum functionality)
```

### Comparing `snirf2bids-0.7.6/snirf2bids.egg-info/PKG-INFO` & `snirf2bids-0.7.7/snirf2bids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snirf2bids
-Version: 0.7.6
+Version: 0.7.7
 Summary: To convert snirf file to bids format.
 Home-page: https://github.com/andyzjc/snirf2bids
 Author: JC
 Author-email: andyzjc@bu.edu
 License: MIT
 Description: 
         ![python](https://img.shields.io/pypi/pyversions/snirf2bids?color=green)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snirf2bids Version: 0.7.6 Summary: To convert snirf
+Metadata-Version: 2.1 Name: snirf2bids Version: 0.7.7 Summary: To convert snirf
 file to bids format. Home-page: https://github.com/andyzjc/snirf2bids Author:
 JC Author-email: andyzjc@bu.edu License: MIT Description: ![python](https://
 img.shields.io/pypi/pyversions/snirf2bids?color=green) [![pypi](https://
 img.shields.io/pypi/v/snirf2bids?color=blue)](https://pypi.org/project/
 snirf2bids/) [![tests](https://github.com/BUNPC/snirf2bids/actions/workflows/
 test.yml/badge.svg)](https://github.com/BUNPC/snirf2bids/actions/workflows/
 test.yml) [![DOI](https://zenodo.org/badge/478632378.svg)](https://zenodo.org/
```

