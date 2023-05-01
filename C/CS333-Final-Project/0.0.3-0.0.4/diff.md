# Comparing `tmp/CS333-Final-Project-0.0.3.tar.gz` & `tmp/CS333-Final-Project-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CS333-Final-Project-0.0.3.tar", last modified: Mon May  1 02:51:14 2023, max compression
+gzip compressed data, was "CS333-Final-Project-0.0.4.tar", last modified: Mon May  1 03:00:20 2023, max compression
```

## Comparing `CS333-Final-Project-0.0.3.tar` & `CS333-Final-Project-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:51:14.940647 CS333-Final-Project-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:51:14.940647 CS333-Final-Project-0.0.3/CS333_Final_Project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 02:51:14.000000 CS333-Final-Project-0.0.3/CS333_Final_Project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 02:51:14.000000 CS333-Final-Project-0.0.3/CS333_Final_Project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:51:14.000000 CS333-Final-Project-0.0.3/CS333_Final_Project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:51:14.000000 CS333-Final-Project-0.0.3/CS333_Final_Project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 02:51:14.940647 CS333-Final-Project-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-05-01 02:51:00.000000 CS333-Final-Project-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:51:14.940647 CS333-Final-Project-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 02:51:00.000000 CS333-Final-Project-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-01 03:00:08.000000 CS333-Final-Project-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 03:00:08.000000 CS333-Final-Project-0.0.4/setup.py
```

### Comparing `CS333-Final-Project-0.0.3/README.md` & `CS333-Final-Project-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # CS333 Final Project
+
+[![image](https://img.shields.io/pypi/v/CS333-Final-Project)](https://pypi.org/project/CS333-Final-Project/)
+
 CS333 Testing and DevOps Final Project
 
 ## Technologies Used
 
 * Testing Framework
 
     * Python unittest
```

### Comparing `CS333-Final-Project-0.0.3/setup.py` & `CS333-Final-Project-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'CS333 Final Project'
 LONG_DESCRIPTION = 'CS333 Testing and DevOps Final Project @ University of Nevada, Reno.'
 
 # Setting up
 setup(
     name="CS333-Final-Project",
     version=VERSION,
```

