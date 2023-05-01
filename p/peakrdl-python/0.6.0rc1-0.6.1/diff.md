# Comparing `tmp/peakrdl-python-0.6.0rc1.tar.gz` & `tmp/peakrdl-python-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-python-0.6.0rc1.tar", last modified: Sun Apr 16 18:46:48 2023, max compression
+gzip compressed data, was "peakrdl-python-0.6.1.tar", last modified: Mon May  1 18:55:38 2023, max compression
```

## Comparing `peakrdl-python-0.6.0rc1.tar` & `peakrdl-python-0.6.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/_node_walkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/peakpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/safe_name_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/systemrdl_node_utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.203227 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_field.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_memory.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_register.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_simulation.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/baseclass_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-16 18:46:47.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/reg_definitions.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:46:48.199227 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 18:46:48.000000 peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.249189 peakrdl-python-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.253189 peakrdl-python-0.6.1/src/peakrdl_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/_node_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.253189 peakrdl-python-0.6.1/src/peakrdl_python/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/peakpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/safe_name_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/systemrdl_node_utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/src/peakrdl_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_field.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_memory.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_register.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_simulation.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/baseclass_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/reg_definitions.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.253189 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-01 18:55:38.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/top_level.txt
```

### Comparing `peakrdl-python-0.6.0rc1/LICENSE` & `peakrdl-python-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/PKG-INFO` & `peakrdl-python-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.6.0rc1
+Version: 0.6.1
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
 Description: ![CI](https://github.com/krcb197/PeakRDL-python/actions/workflows/action.yaml/badge.svg)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-python.svg)](https://pypi.org/project/peakrdl-python)
         [![Documentation Status](https://readthedocs.org/projects/peakrdl-python/badge/?version=latest)](https://peakrdl-python.readthedocs.io/en/latest/?badge=latest)
+        [![Downloads](https://static.pepy.tech/badge/peakrdl-python)](https://pepy.tech/project/peakrdl-python)
         
         # PeakRDL-python
         Generate Python wrapper for a register model compiled SystemRDL input
         
         ## Documentation
         See the [PeakRDL Python Documentation](https://peakrdl-python.readthedocs.io/) for more details
```

### Comparing `peakrdl-python-0.6.0rc1/setup.py` & `peakrdl-python-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,14 @@
                     "peakrdl.exporters": [
                         'python = peakrdl_python.__peakrdl__:Exporter'
                     ]
                     },
     install_requires=[
         "systemrdl-compiler>=1.24.0",
         "autopep8",
-        "pylint",
-        "coverage",
         "jinja2",
         "asynctest;python_version<'3.8'",
         "peakrdl-ipxact"
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
```

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/__peakrdl__.py` & `peakrdl-python-0.6.1/src/peakrdl_python/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/_node_walkers.py` & `peakrdl-python-0.6.1/src/peakrdl_python/_node_walkers.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/exporter.py` & `peakrdl-python-0.6.1/src/peakrdl_python/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Main Classes for the PeakRDL Python
 """
 import os
+import warnings
 from pathlib import Path
 from shutil import copyfile
 from typing import List, NoReturn, Iterable, Tuple
 from glob import glob
 
 import autopep8 # type: ignore
 import jinja2 as jj
@@ -118,14 +119,20 @@
 
         # If it is the root node, skip to top addrmap
         if isinstance(node, RootNode):
             top_block = node.top
         else:
             top_block = node
 
+        # support for autopep8 will be removed from a future release
+        if autoformatoutputs is True:
+            warnings.warn('Autoformating the generated code in the export will be deprecated in a'
+                          'future release. It is recommended this is do outside of peakrdl python',
+                          category=PendingDeprecationWarning)
+
         package_path = os.path.join(path, node.inst_name)
         self._create_empty_package(package_path=package_path,
                                    skip_test_case_generation=skip_test_case_generation)
 
         self._build_node_type_table(top_block)
 
         context = {
```

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/__init__.py` & `peakrdl-python-0.6.1/src/peakrdl_python/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/base.py` & `peakrdl-python-0.6.1/src/peakrdl_python/lib/base.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/callbacks.py` & `peakrdl-python-0.6.1/src/peakrdl_python/lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/fields.py` & `peakrdl-python-0.6.1/src/peakrdl_python/lib/fields.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/memory.py` & `peakrdl-python-0.6.1/src/peakrdl_python/lib/memory.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/lib/register.py` & `peakrdl-python-0.6.1/src/peakrdl_python/lib/register.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,19 +180,25 @@
     @property
     @abstractmethod
     def readable_fields(self) -> Iterator[Union['FieldReadOnly', 'FieldReadWrite']]:
         """
         generator that produces has all the readable fields within the register
         """
 
-    @abstractmethod
     def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
         """
         read the register and return a dictionary of the field values
         """
+        return_dict: Dict['str', Union[bool, Enum, int]] = {}
+        with self.single_read() as reg:
+            for field in reg.readable_fields:
+                return_dict[field.inst_name] = field.read()
+
+        return return_dict
+
 
 
 class RegWriteOnly(Reg, ABC):
     """
     class for a write only register
     """
 
@@ -374,20 +380,40 @@
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             return self.__register_state
 
         return super().read()
 
-    @abstractmethod
     def write_fields(self, **kwargs) -> None: # type: ignore[no-untyped-def]
         """
         Do a read-modify-write to the register, updating any field included in
         the arguments
         """
+        if len(kwargs) == 0:
+            raise ValueError('no command args')
+
+        with self.single_read_modify_write() as reg:
+            for field_name, field_value in kwargs.items():
+                if field_name not in reg.systemrdl_python_child_name_map.values():
+                    raise ValueError(f'{field_name} is not a member of the register')
+
+                field = getattr(reg, field_name)
+                field.write(field_value)
+
+    def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
+        """
+        read the register and return a dictionary of the field values
+        """
+        return_dict: Dict['str', Union[bool, Enum, int]] = {}
+        with self.single_read_modify_write(skip_write=True) as reg:
+            for field in reg.readable_fields:
+                return_dict[field.inst_name] = field.read()
+
+        return return_dict
 
 
 class RegAsyncReadOnly(Reg, ABC):
     """
     class for an async read only register
 
     Args:
@@ -482,19 +508,24 @@
     @property
     @abstractmethod
     def readable_fields(self) -> Iterator[Union['FieldAsyncReadOnly', 'FieldAsyncReadWrite']]:
         """
         generator that produces has all the readable fields within the register
         """
 
-    @abstractmethod
-    async def read_fields(self) -> Dict[str, Union[int, Enum, bool]]:
+    async def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
         """
         asynchronously read the register and return a dictionary of the field values
         """
+        return_dict: Dict['str', Union[bool, Enum, int]] = {}
+        async with self.single_read() as reg:
+            for field in reg.readable_fields:
+                return_dict[field.inst_name] = await field.read()
+
+        return return_dict
 
 
 class RegAsyncWriteOnly(Reg, ABC):
     """
     class for an asynchronous write only register
     """
 
@@ -677,14 +708,41 @@
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             return self.__register_state
 
         return await super().read()
 
+    async def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
+        """
+        asynchronously read the register and return a dictionary of the field values
+        """
+        return_dict: Dict['str', Union[bool, Enum, int]] = {}
+        async with self.single_read_modify_write(skip_write=True) as reg:
+            for field in reg.readable_fields:
+                return_dict[field.inst_name] = await field.read()
+
+        return return_dict
+
+    async def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
+        """
+        asynchronously read-modify-write to the register, updating any field included in
+        the arguments
+        """
+        if len(kwargs) == 0:
+            raise ValueError('no command args')
+
+        async with self.single_read_modify_write() as reg:
+            for field_name, field_value in kwargs.items():
+                if field_name not in reg.systemrdl_python_child_name_map.values():
+                    raise ValueError(f'{field_name} is not a member of the register')
+
+                field = getattr(reg, field_name)
+                await field.write(field_value)
+
 
 ReadableRegister = Union[RegReadOnly, RegReadWrite]
 WritableRegister = Union[RegWriteOnly, RegReadWrite]
 ReadableAsyncRegister = Union[RegAsyncReadOnly, RegAsyncReadWrite]
 WritableAsyncRegister = Union[RegAsyncWriteOnly, RegAsyncReadWrite]
```

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/peakpython.py` & `peakrdl-python-0.6.1/src/peakrdl_python/peakpython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 Command Line tool for the PeakRDL Python
 """
 
 #!/usr/bin/env python3
 import argparse
 import os
-import subprocess
 import unittest.loader
+import warnings
 from typing import List, Optional
 import pathlib
 
-import coverage # type: ignore
-
 from systemrdl import RDLCompiler # type: ignore
 from systemrdl.node import Node, AddrmapNode # type: ignore
 from peakrdl_ipxact import IPXACTImporter # type: ignore
 
 from .exporter import PythonExporter
 
 
@@ -47,21 +45,19 @@
                         help='builds the register model using the async callbacks')
     parser.add_argument('--ipxact', dest='ipxact', nargs='*',
                         type=str)
     parser.add_argument('--user_template_dir', action='store', type=pathlib.Path,
                            help='directory of user templates to override the default ones')
     checker = parser.add_argument_group('post-generate checks')
     checker.add_argument('--lint', action='store_true',
-                         help='run pylint on the generated python')
+                         help='run pylint on the generated python (support removed at 0.6.1)')
     checker.add_argument('--test', action='store_true',
                          help='run unittests for the created')
     checker.add_argument('--coverage', action='store_true',
-                         help='run a coverage report on the unittests')
-    checker.add_argument('--html_coverage_out',
-                         help='output director (default: %(default)s)')
+                         help='run a coverage report on the unittests (support removed at 0.6.1)')
     parser.add_argument('--skip_test_case_generation', action='store_true',
                         help='skip the generation of the test cases')
 
     return parser
 
 
 def compile_rdl(infile:str,
@@ -117,30 +113,14 @@
     modules = PythonExporter().export(root, outdir, # type: ignore[no-untyped-call]
                                       autoformatoutputs=autoformatoutputs,
                                       asyncoutput=asyncoutput,
                                       skip_test_case_generation=skip_test_case_generation)
 
     return modules
 
-def run_lint(root:str, outdir:str) -> None:
-    """
-    Run the lint checks using pylint on a directory
-
-    Args:
-        root: name of the generated package (directory)
-        outdir: location where the package has been written
-
-    Returns:
-
-    """
-    subprocess.run(['pylint', '--rcfile',
-                    os.path.join('tests','pylint.rc'),
-                    os.path.join(outdir, root)],
-                   check=False)
-
 def main_function() -> None:
     """
     Main function for the Command Line tool, this needs to be separated out so that it can be
     referenced in setup.py
 
     Returns:
         None
@@ -161,37 +141,31 @@
 
     print('***************************************************************')
     print('* Generate the Python Package                                 *')
     print('***************************************************************')
     generate(spec, args.outdir, autoformatoutputs=args.autoformat,
              skip_test_case_generation=args.skip_test_case_generation,
              asyncoutput=args.asyncoutput)
-
     if args.lint:
-        print('***************************************************************')
-        print('* Lint Checks                                                 *')
-        print('***************************************************************')
-        run_lint(outdir=args.outdir, root=spec.inst_name)
+        raise NotImplementedError('Support for running linting checks was removed at 0.6.1, '
+                                  'pylint can be run seperatly on the generated code if needed')
     if args.test:
         print('***************************************************************')
         print('* Unit Test Run                                               *')
         print('***************************************************************')
         if args.coverage:
-            cov = coverage.Coverage(
-                include=[f'*\\{spec.inst_name}\\reg_model\\*.py',
-                         f'*\\{spec.inst_name}\\tests\\*.py'])
-            cov.start()
+            raise NotImplementedError('Support for geneating a coverage report was removed at '
+                                      '0.6.1, this can be done separately if needed')
         tests = unittest.TestLoader().discover(
             start_dir=os.path.join(args.outdir, spec.inst_name, 'tests'),
             top_level_dir=args.outdir)
         runner = unittest.TextTestRunner()
         runner.run(tests)
 
-        if args.coverage:
-            cov.stop()
-
-        if args.html_coverage_out is not None:
-            cov.html_report(directory=args.html_coverage_out)
+if __name__ == '__main__':
 
+    warnings.warn('The peakpython command line option will be removed in a future release. '
+                  'Command line functionality should be used via the see '
+                  'https://peakrdl-python.readthedocs.io/en/latest/command_line.html',
+                  category=PendingDeprecationWarning)
 
-if __name__ == '__main__':
     main_function()
```

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/safe_name_utility.py` & `peakrdl-python-0.6.1/src/peakrdl_python/safe_name_utility.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/systemrdl_node_utility_functions.py` & `peakrdl-python-0.6.1/src/peakrdl_python/systemrdl_node_utility_functions.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_field.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_field.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_memory.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_memory.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_register.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_register.py.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -46,32 +46,14 @@
                 is_volatile={{child_node.is_hw_writable}}),
             logger_handle=logger_handle+'.{{child_node.inst_name}}',
             inst_name='{{child_node.inst_name}}')
             {%- endif -%}
         {%- endfor %}
 
     {% if node.has_sw_readable %}
-    {% if asyncoutput %}async {% endif %}def read_fields(self) -> Dict[str, Union[bool, {% if uses_enum %}IntEnum, {% endif %} int]]: # type: ignore[override]
-        """
-        read the register and return a dictionary of the field values
-        """
-        {% if node.has_sw_writable %}
-        {% if asyncoutput %}async {% endif %}with self.single_read_modify_write(skip_write=True) as reg:
-        {% else %}
-        {% if asyncoutput %}async {% endif %}with self.single_read() as reg:
-        {% endif %}
-            return_dict:Dict[str, Union[bool, {% if uses_enum %}IntEnum, {% endif %} int]] = {
-                            {%- for child_node in get_reg_readable_fields(node) %}
-                            '{{child_node.inst_name}}' : {% if asyncoutput %}await {% endif %}reg.{{safe_node_name(child_node)}}.read()
-                            {%- if not loop.last -%} ,  {%- endif -%}
-                            {% endfor %}
-                          }
-
-        return return_dict
-
     @property
     def readable_fields(self) -> Iterator[Union[Field{% if asyncoutput %}Async{% endif %}ReadOnly, Field{% if asyncoutput %}Async{% endif %}ReadWrite]]:
         """
         generator that produces has all the readable fields within the register
         """
         {% for child_node in get_reg_readable_fields(node) -%}
         yield self.{{safe_node_name(child_node)}}
@@ -105,35 +87,16 @@
         """
         generator that produces has all the writable fields within the register
         """
         {% for child_node in get_reg_writable_fields(node) -%}
         yield self.{{safe_node_name(child_node)}}
         {% endfor %}
 
-    {% if node.has_sw_readable %}
-    {% if asyncoutput %}async {% endif %}def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
-        """
-        Do a read-modify-write to the register, updating any field included in
-        the arguments
-        """
-        if len(kwargs) == 0:
-            raise ValueError('no command args')
-
-        {% if asyncoutput %}async {% endif %}with self.single_read_modify_write() as reg:
-        {%- for child_node in get_reg_writable_fields(node) %}
-            if '{{safe_node_name(child_node)}}' in kwargs:
-                {% if asyncoutput %}await {% endif %}self.{{safe_node_name(child_node)}}.write(kwargs['{{safe_node_name(child_node)}}'])
-                kwargs.pop('{{safe_node_name(child_node)}}')
-        {%- endfor %}
-            if len(kwargs) != 0:
-                # left over unhandled arguments
-                raise ValueError('unrecognised arguments in field')
-
-
-    {% else %}
+    {% if not node.has_sw_readable %}
+    {# if the register has no readable components, all the fields must be writen as one #}
     {% if asyncoutput %}async {% endif %}def write_fields(self, {%- for child_node in node.fields() -%} {{safe_node_name(child_node)}} : {%- if 'encode' in child_node.list_properties() %}{{get_fully_qualified_enum_type(child_node.get_property('encode'), top_node.parent, child_node)}}_enumcls{% else %}int{% endif %}{%- if not loop.last -%},{%- endif -%}{%- endfor -%}) -> None: # type: ignore[override]
         """
         Do a write to the register, updating all fields
         """
         reg_value = 0
         {%- for child_node in node.fields() %}
         reg_value |= self.{{safe_node_name(child_node)}}.encode_write_value({{safe_node_name(child_node)}})
```

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/addrmap_tb.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/baseclass_tb.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/baseclass_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python/templates/reg_definitions.py.jinja` & `peakrdl-python-0.6.1/src/peakrdl_python/templates/reg_definitions.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/PKG-INFO` & `peakrdl-python-0.6.1/src/peakrdl_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.6.0rc1
+Version: 0.6.1
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
 Description: ![CI](https://github.com/krcb197/PeakRDL-python/actions/workflows/action.yaml/badge.svg)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-python.svg)](https://pypi.org/project/peakrdl-python)
         [![Documentation Status](https://readthedocs.org/projects/peakrdl-python/badge/?version=latest)](https://peakrdl-python.readthedocs.io/en/latest/?badge=latest)
+        [![Downloads](https://static.pepy.tech/badge/peakrdl-python)](https://pepy.tech/project/peakrdl-python)
         
         # PeakRDL-python
         Generate Python wrapper for a register model compiled SystemRDL input
         
         ## Documentation
         See the [PeakRDL Python Documentation](https://peakrdl-python.readthedocs.io/) for more details
```

### Comparing `peakrdl-python-0.6.0rc1/src/peakrdl_python.egg-info/SOURCES.txt` & `peakrdl-python-0.6.1/src/peakrdl_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

