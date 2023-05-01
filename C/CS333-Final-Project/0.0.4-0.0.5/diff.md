# Comparing `tmp/CS333-Final-Project-0.0.4.tar.gz` & `tmp/CS333-Final-Project-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CS333-Final-Project-0.0.4.tar", last modified: Mon May  1 03:00:20 2023, max compression
+gzip compressed data, was "CS333-Final-Project-0.0.5.tar", last modified: Mon May  1 05:06:54 2023, max compression
```

## Comparing `CS333-Final-Project-0.0.4.tar` & `CS333-Final-Project-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 03:00:20.000000 CS333-Final-Project-0.0.4/CS333_Final_Project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-01 03:00:08.000000 CS333-Final-Project-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 03:00:20.773066 CS333-Final-Project-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 03:00:08.000000 CS333-Final-Project-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:06:54.698868 CS333-Final-Project-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:06:54.698868 CS333-Final-Project-0.0.5/CS333_Final_Project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 05:06:54.000000 CS333-Final-Project-0.0.5/CS333_Final_Project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 05:06:54.000000 CS333-Final-Project-0.0.5/CS333_Final_Project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:06:54.000000 CS333-Final-Project-0.0.5/CS333_Final_Project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:06:54.000000 CS333-Final-Project-0.0.5/CS333_Final_Project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 05:06:54.698868 CS333-Final-Project-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-01 05:06:43.000000 CS333-Final-Project-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 05:06:54.698868 CS333-Final-Project-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 05:06:43.000000 CS333-Final-Project-0.0.5/setup.py
```

### Comparing `CS333-Final-Project-0.0.4/README.md` & `CS333-Final-Project-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # CS333 Final Project
 
-[![image](https://img.shields.io/pypi/v/CS333-Final-Project)](https://pypi.org/project/CS333-Final-Project/)
+[![image](https://img.shields.io/badge/-PyPI-brightgreen)](https://pypi.org/project/CS333-Final-Project/)
 
 CS333 Testing and DevOps Final Project
 
+Author: Colin Martires
+
+Date: 4/30/2023
+
 ## Technologies Used
 
 * Testing Framework
 
     * Python unittest
 
 * Source Control
@@ -18,30 +22,72 @@
 
     * PyPi
 
 * Automated Testing and Deployment
 
     * GitHub Actions
 
-## CS457 Programming Assignment 1: Metadata Management
+## Manual Testing
+
+* Install coverage.py to view code coverage report
+
+    * `pip install coverage`
+
+* To run tests manually
+
+    * `python test_suite.py -b` or `coverage run test_suite.py -b`
+
+    ```
+    .........................................
+    ----------------------------------------------------------------------
+    Ran 41 tests in 0.063s
+
+    OK
+    ```
+
+* To view code coverage
+
+    * `coverage report`
+
+    ```
+    Name             Stmts   Miss  Cover
+    ------------------------------------
+    Functions.py       114     11    90%
+    TokenParser.py      12      0   100%
+    test_suite.py      372      4    99%
+    ------------------------------------
+    TOTAL              498     15    97%
+    ```
+
+## Automated Testing and Deployment
+
+* Tests will be automatically ran once code is pushed to the repository
+
+* The automatic deployment script will only be run if the test script passes
+
+    * Ensure you update the `VERSION` variable in `setup.py` to prevent deployment errors.
+
+---
+
+### CS457 Programming Assignment 1: Metadata Management
 
 Author: Colin Martires
 
 Date: 2/13/2023
 
-## Prerequisites
+### Prerequisites
 
 * Python 3.10.6
 
 * Modules used:
 
     * os
     * shutil
 
-## Usage
+### Usage
 * Run main.py
 
     `python3 main.py`
 
 * To create a database
 
     `CREATE DATABASE <database name>;`
```

### Comparing `CS333-Final-Project-0.0.4/setup.py` & `CS333-Final-Project-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'CS333 Final Project'
 LONG_DESCRIPTION = 'CS333 Testing and DevOps Final Project @ University of Nevada, Reno.'
 
 # Setting up
 setup(
     name="CS333-Final-Project",
     version=VERSION,
```

