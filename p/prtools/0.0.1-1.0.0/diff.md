# Comparing `tmp/prtools-0.0.1.tar.gz` & `tmp/prtools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prtools-0.0.1.tar", last modified: Sun Mar 12 23:46:49 2023, max compression
+gzip compressed data, was "prtools-1.0.0.tar", last modified: Mon May  1 02:59:20 2023, max compression
```

## Comparing `prtools-0.0.1.tar` & `prtools-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
-drwxr-xr-x   0 akee       (504) staff       (20)        0 2023-03-12 23:46:49.256060 prtools-0.0.1/
--rw-r--r--   0 akee       (504) staff       (20)      790 2023-03-12 23:46:49.256123 prtools-0.0.1/PKG-INFO
-drwxr-xr-x   0 akee       (504) staff       (20)        0 2023-03-12 23:46:49.255260 prtools-0.0.1/prtools/
--rw-r--r--   0 akee       (504) staff       (20)       23 2023-03-12 23:46:33.000000 prtools-0.0.1/prtools/__init__.py
-drwxr-xr-x   0 akee       (504) staff       (20)        0 2023-03-12 23:46:49.255910 prtools-0.0.1/prtools.egg-info/
--rw-r--r--   0 akee       (504) staff       (20)      790 2023-03-12 23:46:49.000000 prtools-0.0.1/prtools.egg-info/PKG-INFO
--rw-r--r--   0 akee       (504) staff       (20)      162 2023-03-12 23:46:49.000000 prtools-0.0.1/prtools.egg-info/SOURCES.txt
--rw-r--r--   0 akee       (504) staff       (20)        1 2023-03-12 23:46:49.000000 prtools-0.0.1/prtools.egg-info/dependency_links.txt
--rw-r--r--   0 akee       (504) staff       (20)        8 2023-03-12 23:46:49.000000 prtools-0.0.1/prtools.egg-info/top_level.txt
--rw-r--r--   0 akee       (504) staff       (20)      729 2023-03-12 23:46:49.256399 prtools-0.0.1/setup.cfg
--rw-r--r--   0 akee       (504) staff       (20)       71 2023-03-12 23:45:24.000000 prtools-0.0.1/setup.py
+drwxr-xr-x   0 akee       (504) staff       (20)        0 2023-05-01 02:59:20.599107 prtools-1.0.0/
+-rw-r--r--   0 akee       (504) staff       (20)     1064 2023-05-01 02:55:49.000000 prtools-1.0.0/LICENSE
+-rw-r--r--   0 akee       (504) staff       (20)     2046 2023-04-07 21:04:38.000000 prtools-1.0.0/NOTICE
+-rw-r--r--   0 akee       (504) staff       (20)      833 2023-05-01 02:59:20.599170 prtools-1.0.0/PKG-INFO
+-rw-r--r--   0 akee       (504) staff       (20)      858 2023-04-07 17:17:48.000000 prtools-1.0.0/README.rst
+drwxr-xr-x   0 akee       (504) staff       (20)        0 2023-05-01 02:59:20.598122 prtools-1.0.0/prtools/
+-rw-r--r--   0 akee       (504) staff       (20)      469 2023-05-01 02:54:37.000000 prtools-1.0.0/prtools/__init__.py
+-rw-r--r--   0 akee       (504) staff       (20)    14102 2023-05-01 02:54:37.000000 prtools-1.0.0/prtools/array.py
+-rw-r--r--   0 akee       (504) staff       (20)     1071 2023-03-14 00:55:56.000000 prtools-1.0.0/prtools/misc.py
+-rw-r--r--   0 akee       (504) staff       (20)     7674 2023-03-01 22:21:25.000000 prtools-1.0.0/prtools/shapes.py
+-rw-r--r--   0 akee       (504) staff       (20)     4264 2023-05-01 02:54:37.000000 prtools-1.0.0/prtools/stats.py
+-rw-r--r--   0 akee       (504) staff       (20)    11208 2023-03-14 15:57:47.000000 prtools-1.0.0/prtools/zernike.py
+drwxr-xr-x   0 akee       (504) staff       (20)        0 2023-05-01 02:59:20.598986 prtools-1.0.0/prtools.egg-info/
+-rw-r--r--   0 akee       (504) staff       (20)      833 2023-05-01 02:59:20.000000 prtools-1.0.0/prtools.egg-info/PKG-INFO
+-rw-r--r--   0 akee       (504) staff       (20)      305 2023-05-01 02:59:20.000000 prtools-1.0.0/prtools.egg-info/SOURCES.txt
+-rw-r--r--   0 akee       (504) staff       (20)        1 2023-05-01 02:59:20.000000 prtools-1.0.0/prtools.egg-info/dependency_links.txt
+-rw-r--r--   0 akee       (504) staff       (20)       12 2023-05-01 02:59:20.000000 prtools-1.0.0/prtools.egg-info/requires.txt
+-rw-r--r--   0 akee       (504) staff       (20)        8 2023-05-01 02:59:20.000000 prtools-1.0.0/prtools.egg-info/top_level.txt
+-rw-r--r--   0 akee       (504) staff       (20)      729 2023-05-01 02:59:20.599486 prtools-1.0.0/setup.cfg
+-rw-r--r--   0 akee       (504) staff       (20)      122 2023-04-07 17:18:18.000000 prtools-1.0.0/setup.py
```

### Comparing `prtools-0.0.1/PKG-INFO` & `prtools-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prtools
-Version: 0.0.1
+Version: 1.0.0
 Summary: Utility functions for image-based phase retrieval
 Author: Andy Kee
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,9 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: NOTICE
```

### Comparing `prtools-0.0.1/prtools.egg-info/PKG-INFO` & `prtools-1.0.0/prtools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prtools
-Version: 0.0.1
+Version: 1.0.0
 Summary: Utility functions for image-based phase retrieval
 Author: Andy Kee
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,9 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: NOTICE
```

### Comparing `prtools-0.0.1/setup.cfg` & `prtools-1.0.0/setup.cfg`

 * *Files identical despite different names*

