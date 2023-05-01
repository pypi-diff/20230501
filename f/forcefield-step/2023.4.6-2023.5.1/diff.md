# Comparing `tmp/forcefield_step-2023.4.6.tar.gz` & `tmp/forcefield_step-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forcefield_step-2023.4.6.tar", last modified: Thu Apr  6 15:40:42 2023, max compression
+gzip compressed data, was "forcefield_step-2023.5.1.tar", last modified: Mon May  1 15:21:39 2023, max compression
```

## Comparing `forcefield_step-2023.4.6.tar` & `forcefield_step-2023.5.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.384149 forcefield_step-2023.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-06 15:40:42.384149 forcefield_step-2023.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.376150 forcefield_step-2023.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.376150 forcefield_step-2023.4.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.376150 forcefield_step-2023.4.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9604 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.376150 forcefield_step-2023.4.6/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/developer_guide/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.376150 forcefield_step-2023.4.6/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.376150 forcefield_step-2023.4.6/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.384149 forcefield_step-2023.4.6/forcefield_step/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-06 15:40:42.384149 forcefield_step-2023.4.6/forcefield_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.380149 forcefield_step-2023.4.6/forcefield_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/data/lithium_battery.frc
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/data/nacl_water.frc
--rw-r--r--   0 runner    (1001) docker     (123)   474898 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/data/oplsaa.frc
--rw-r--r--   0 runner    (1001) docker     (123)   361764 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/data/pcff2018.frc
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/forcefield_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/forcefield_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/forcefield_step/tk_forcefield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.380149 forcefield_step-2023.4.6/forcefield_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-06 15:40:42.000000 forcefield_step-2023.4.6/forcefield_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-06 15:40:42.000000 forcefield_step-2023.4.6/forcefield_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:40:42.000000 forcefield_step-2023.4.6/forcefield_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-06 15:40:42.000000 forcefield_step-2023.4.6/forcefield_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-06 15:40:42.000000 forcefield_step-2023.4.6/forcefield_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 15:40:42.000000 forcefield_step-2023.4.6/forcefield_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-06 15:40:42.384149 forcefield_step-2023.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:40:42.384149 forcefield_step-2023.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/tests/test_forcefield_step.py
--rw-r--r--   0 runner    (1001) docker     (123)   153001 2023-04-06 15:40:18.000000 forcefield_step-2023.4.6/tests/test_oplsaa_assignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.161509 forcefield_step-2023.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.161509 forcefield_step-2023.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.161509 forcefield_step-2023.5.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9604 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.165509 forcefield_step-2023.5.1/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.165509 forcefield_step-2023.5.1/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.165509 forcefield_step-2023.5.1/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/lithium_battery.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/nacl_water.frc
+-rw-r--r--   0 runner    (1001) docker     (123)   474899 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/oplsaa.frc
+-rw-r--r--   0 runner    (1001) docker     (123)   361764 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/pcff2018.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/forcefield_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/forcefield_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/tk_forcefield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/test_forcefield_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153001 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/test_oplsaa_assignment.py
```

### Comparing `forcefield_step-2023.4.6/CONTRIBUTING.rst` & `forcefield_step-2023.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/HISTORY.rst` & `forcefield_step-2023.5.1/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =======
 History
 =======
 
+2023.5.1 -- Fixed bug in Lithium battery forcefield
+  * Fixed a typo in the angle type unit line which caused a crash
+    
 2023.4.6 -- Added Lithium battery forcefield
   * An initial set of parameters for cathode materials, specifically LiCoO2.
 
 2023.2.13 -- Added OPLS-AA forcefield
   * Added parameters for OPLS-AA along with some extra parameters for ionic liquids
     * PF6-
     * ethylene carbonate (EC) and fluoronated EC (FEC)
```

### Comparing `forcefield_step-2023.4.6/LICENSE` & `forcefield_step-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/PKG-INFO` & `forcefield_step-2023.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcefield_step
-Version: 2023.4.6
+Version: 2023.5.1
 Summary: A SEAMM plug-in for setting up a forcefield or EAM potentials for subsequent simulations.
 Home-page: https://github.com/molssi-seam/forcefield_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM
 Platform: Linux
@@ -83,14 +83,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.5.1 -- Fixed bug in Lithium battery forcefield
+  * Fixed a typo in the angle type unit line which caused a crash
+    
 2023.4.6 -- Added Lithium battery forcefield
   * An initial set of parameters for cathode materials, specifically LiCoO2.
 
 2023.2.13 -- Added OPLS-AA forcefield
   * Added parameters for OPLS-AA along with some extra parameters for ionic liquids
     * PF6-
     * ethylene carbonate (EC) and fluoronated EC (FEC)
```

### Comparing `forcefield_step-2023.4.6/README.rst` & `forcefield_step-2023.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/Makefile` & `forcefield_step-2023.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/_static/SEAMM inverted.png` & `forcefield_step-2023.5.1/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/_static/SEAMM logo.png` & `forcefield_step-2023.5.1/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/_static/molssi_main_logo.png` & `forcefield_step-2023.5.1/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/_static/molssi_main_logo_inverted_white.png` & `forcefield_step-2023.5.1/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/_static/molssi_square.png` & `forcefield_step-2023.5.1/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/_static/nsf.png` & `forcefield_step-2023.5.1/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/conf.py` & `forcefield_step-2023.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/developer_guide/installation.rst` & `forcefield_step-2023.5.1/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/getting_started/index.rst` & `forcefield_step-2023.5.1/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/index.rst` & `forcefield_step-2023.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/docs/make.bat` & `forcefield_step-2023.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/__init__.py` & `forcefield_step-2023.5.1/forcefield_step/__init__.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/data/lithium_battery.frc` & `forcefield_step-2023.5.1/forcefield_step/data/lithium_battery.frc`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/data/nacl_water.frc` & `forcefield_step-2023.5.1/forcefield_step/data/nacl_water.frc`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/data/oplsaa.frc` & `forcefield_step-2023.5.1/forcefield_step/data/oplsaa.frc`

 * *Files 0% similar despite different names*

```diff
@@ -29497,186 +29497,186 @@
 00073380: 5020 2020 2020 2020 2020 4620 2020 2020  P         F     
 00073390: 2020 2020 312e 3630 3620 2020 2020 3331      1.606     31
 000733a0: 3030 2e30 0a0a 0a0a 2371 7561 6472 6174  00.0....#quadrat
 000733b0: 6963 5f61 6e67 6c65 2020 2020 2020 2043  ic_angle       C
 000733c0: 4c26 502d 6f70 6c73 6161 0a0a 3e20 4520  L&P-oplsaa..> E 
 000733d0: 3d20 4b32 202a 2028 5468 6574 6120 2d20  = K2 * (Theta - 
 000733e0: 5468 6574 6130 295e 320a 0a40 756e 6974  Theta0)^2..@unit
-000733f0: 7320 5468 6574 6120 6465 6772 6565 0a40  s Theta degree.@
-00073400: 756e 6974 7320 4b32 206b 4a2f 6d6f 6c2f  units K2 kJ/mol/
-00073410: 7261 6469 616e 5e32 0a0a 2120 5665 7273  radian^2..! Vers
-00073420: 696f 6e20 2020 5265 6620 2020 4920 2020  ion   Ref   I   
-00073430: 2020 2020 2020 4a20 2020 2020 2020 2020        J         
-00073440: 4b20 2020 2020 2020 2020 2020 5468 6574  K           Thet
-00073450: 6130 2020 2020 2020 2020 4b32 0a21 2d2d  a0        K2.!--
-00073460: 2d2d 2d2d 2d2d 2d20 202d 2d2d 2d20 202d  -------  ----  -
-00073470: 2d2d 2d2d 2d2d 2d20 202d 2d2d 2d2d 2d2d  -------  -------
-00073480: 2d20 202d 2d2d 2d2d 2d2d 2d20 202d 2d2d  -  --------  ---
-00073490: 2d2d 2d2d 2d20 202d 2d2d 2d2d 2d2d 2d0a  -----  --------.
-000734a0: 3230 3233 2e30 312e 3239 2020 3320 2020  2023.01.29  3   
-000734b0: 2020 4650 2020 2020 2020 2020 5020 2020    FP        P   
-000734c0: 2020 2020 2020 4650 2020 2020 2020 2020        FP        
-000734d0: 2020 3930 2e30 2020 2020 2020 3131 3635    90.0      1165
-000734e0: 2e30 0a0a 0a0a 2373 696d 706c 655f 666f  .0....#simple_fo
-000734f0: 7572 6965 725f 616e 676c 6520 2020 2020  urier_angle     
-00073500: 2020 434c 2650 2d6f 706c 7361 610a 0a3e    CL&P-oplsaa..>
-00073510: 2045 203d 204b 202a 205b 3120 2d20 636f   E = K * [1 - co
-00073520: 7328 6e2a 5468 6574 6129 5d0a 3e0a 3e20  s(n*Theta)].>.> 
-00073530: 2020 204b 203d 204b 3228 7175 6164 7261     K = K2(quadra
-00073540: 7469 6329 202f 2038 0a0a 4075 6e69 7473  tic) / 8..@units
-00073550: 204b 206b 4a2f 6d6f 6c0a 0a21 2056 6572   K kJ/mol..! Ver
-00073560: 7369 6f6e 2020 2052 6566 2020 2049 2020  sion   Ref   I  
-00073570: 2020 2020 2020 204a 2020 2020 2020 2020         J        
-00073580: 204b 2020 2020 2020 2020 2020 2020 4b20   K            K 
-00073590: 2020 2020 2020 2020 6e0a 212d 2d2d 2d2d          n.!-----
-000735a0: 2d2d 2d2d 2020 2d2d 2d2d 2020 2d2d 2d2d  ----  ----  ----
-000735b0: 2d2d 2d2d 2020 2d2d 2d2d 2d2d 2d2d 2020  ----  --------  
-000735c0: 2d2d 2d2d 2d2d 2d2d 2020 2d2d 2d2d 2d2d  --------  ------
-000735d0: 2d2d 2020 2020 2d2d 2d0a 3230 3233 2e30  --    ---.2023.0
-000735e0: 312e 3239 2020 3520 2020 2020 4650 2020  1.29  5     FP  
-000735f0: 2020 2020 2020 5020 2020 2020 2020 2020        P         
-00073600: 4650 2020 2020 2020 2020 2031 3435 2e36  FP         145.6
-00073610: 2020 2020 2020 2034 0a0a 2374 656d 706c         4..#templ
-00073620: 6174 6573 2043 4c26 502d 6f70 6c73 6161  ates CL&P-oplsaa
-00073630: 0a7b 0a20 2020 2022 5022 3a20 7b0a 2020  .{.    "P": {.  
-00073640: 2020 2020 2020 2232 3032 332e 3031 2e32        "2023.01.2
-00073650: 3922 3a20 7b0a 2020 2020 2020 2020 2020  9": {.          
-00073660: 2020 2273 6d61 7274 7322 3a20 5b0a 2020    "smarts": [.  
-00073670: 2020 2020 2020 2020 2020 2020 2020 225b                "[
-00073680: 503a 315d 2846 2928 4629 2846 2928 4629  P:1](F)(F)(F)(F)
-00073690: 2846 2946 220a 2020 2020 2020 2020 2020  (F)F".          
-000736a0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-000736b0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000736c0: 2250 686f 7370 686f 726f 7573 2069 6e20  "Phosphorous in 
-000736d0: 5046 362d 222c 0a20 2020 2020 2020 2020  PF6-",.         
-000736e0: 2020 2022 6f76 6572 7269 6465 7322 3a20     "overrides": 
-000736f0: 5b5d 0a20 2020 2020 2020 207d 0a20 2020  [].        }.   
-00073700: 207d 2c0a 2020 2020 2246 5022 3a20 7b0a   },.    "FP": {.
-00073710: 2020 2020 2020 2020 2232 3032 332e 3031          "2023.01
-00073720: 2e32 3922 3a20 7b0a 2020 2020 2020 2020  .29": {.        
-00073730: 2020 2020 2273 6d61 7274 7322 3a20 5b0a      "smarts": [.
-00073740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00073750: 225b 505d 285b 463a 315d 2928 5b46 3a32  "[P]([F:1])([F:2
-00073760: 5d29 285b 463a 335d 2928 5b46 3a34 5d29  ])([F:3])([F:4])
-00073770: 285b 463a 355d 295b 463a 365d 220a 2020  ([F:5])[F:6]".  
-00073780: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00073790: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-000737a0: 7074 696f 6e22 3a20 2246 6c75 6f72 696e  ption": "Fluorin
-000737b0: 6520 696e 2050 4636 2d22 2c0a 2020 2020  e in PF6-",.    
-000737c0: 2020 2020 2020 2020 226f 7665 7272 6964          "overrid
-000737d0: 6573 223a 205b 5d0a 2020 2020 2020 2020  es": [].        
-000737e0: 7d0a 2020 2020 7d0a 7d0a 0a23 7265 6665  }.    }.}..#refe
-000737f0: 7265 6e63 6520 310a 4041 7574 686f 7220  rence 1.@Author 
-00073800: 5061 756c 2053 6178 650a 4044 6174 6520  Paul Saxe.@Date 
-00073810: 3230 3233 2d30 312d 3239 0a4f 504c 5341  2023-01-29.OPLSA
-00073820: 4120 666f 7263 6566 6965 6c64 2074 7261  A forcefield tra
-00073830: 6e73 6c61 7465 6420 6672 6f6d 2054 696e  nslated from Tin
-00073840: 6b65 7220 7665 7273 696f 6e2e 0a23 656e  ker version..#en
-00073850: 640a 0a23 7265 6665 7265 6e63 6520 320a  d..#reference 2.
-00073860: 4041 7574 686f 7220 5061 756c 2053 6178  @Author Paul Sax
-00073870: 650a 4044 6174 6520 3230 3233 2d30 312d  e.@Date 2023-01-
-00073880: 3239 0a0a 4c6f 7065 732c 204a 2e20 4e2e  29..Lopes, J. N.
-00073890: 2043 2e3b 2044 6573 6368 616d 7073 2c20   C.; Deschamps, 
-000738a0: 4a2e 3b20 50c3 a164 7561 2c20 412e 2041  J.; P..dua, A. A
-000738b0: 2e20 482e 0a4d 6f64 656c 696e 6720 496f  . H..Modeling Io
-000738c0: 6e69 6320 4c69 7175 6964 7320 5573 696e  nic Liquids Usin
-000738d0: 6720 6120 5379 7374 656d 6174 6963 2041  g a Systematic A
-000738e0: 6c6c 2d41 746f 6d20 466f 7263 6520 4669  ll-Atom Force Fi
-000738f0: 656c 642e 0a4a 2050 6879 7320 4368 656d  eld..J Phys Chem
-00073900: 2042 2032 3030 342c 2031 3038 2028 3629   B 2004, 108 (6)
-00073910: 2c20 3230 3338 e280 9332 3034 372e 0a68  , 2038...2047..h
-00073920: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00073930: 302e 3130 3231 2f6a 7030 3336 3231 3333  0.1021/jp0362133
-00073940: 2e0a 0a0a 4061 7274 6963 6c65 7b31 302e  ....@article{10.
-00073950: 3130 3231 2f6a 7030 3336 3231 3333 2c20  1021/jp0362133, 
-00073960: 0d0a 7965 6172 203d 207b 3230 3034 7d2c  ..year = {2004},
-00073970: 200d 0a74 6974 6c65 203d 207b 7b4d 6f64   ..title = {{Mod
-00073980: 656c 696e 6720 496f 6e69 6320 4c69 7175  eling Ionic Liqu
-00073990: 6964 7320 5573 696e 6720 6120 5379 7374  ids Using a Syst
-000739a0: 656d 6174 6963 2041 6c6c 2d41 746f 6d20  ematic All-Atom 
-000739b0: 466f 7263 6520 4669 656c 647d 7d2c 200d  Force Field}}, .
-000739c0: 0a61 7574 686f 7220 3d20 7b4c 6f70 6573  .author = {Lopes
-000739d0: 2c20 4a6f 73c3 a920 4e2e 2043 616e 6f6e  , Jos.. N. Canon
-000739e0: 6769 6120 616e 6420 4465 7363 6861 6d70  gia and Deschamp
-000739f0: 732c 204a 6f68 6e6e 7920 616e 6420 50c3  s, Johnny and P.
-00073a00: a164 7561 2c20 4167 c3ad 6c69 6f20 412e  .dua, Ag..lio A.
-00073a10: 2048 2e7d 2c20 0d0a 6a6f 7572 6e61 6c20   H.}, ..journal 
-00073a20: 3d20 7b54 6865 204a 6f75 726e 616c 206f  = {The Journal o
-00073a30: 6620 5068 7973 6963 616c 2043 6865 6d69  f Physical Chemi
-00073a40: 7374 7279 2042 7d2c 200d 0a69 7373 6e20  stry B}, ..issn 
-00073a50: 3d20 7b31 3532 302d 3631 3036 7d2c 200d  = {1520-6106}, .
-00073a60: 0a64 6f69 203d 207b 3130 2e31 3032 312f  .doi = {10.1021/
-00073a70: 6a70 3033 3632 3133 337d 2c20 0d0a 7061  jp0362133}, ..pa
-00073a80: 6765 7320 3d20 7b32 3033 382d 2d32 3034  ges = {2038--204
-00073a90: 377d 2c20 0d0a 6e75 6d62 6572 203d 207b  7}, ..number = {
-00073aa0: 367d 2c20 0d0a 766f 6c75 6d65 203d 207b  6}, ..volume = {
-00073ab0: 3130 387d 2c20 0d0a 7d0a 0a0a 2372 6566  108}, ..}...#ref
-00073ac0: 6572 656e 6365 2033 0a40 4175 7468 6f72  erence 3.@Author
-00073ad0: 2050 6175 6c20 5361 7865 0a40 4461 7465   Paul Saxe.@Date
-00073ae0: 2032 3032 332d 3031 2d32 390a 0a4c 6f70   2023-01-29..Lop
-00073af0: 6573 2c20 4a2e 204e 2e20 432e 3b20 50c3  es, J. N. C.; P.
-00073b00: a164 7561 2c20 412e 2041 2e20 482e 0a4d  .dua, A. A. H..M
-00073b10: 6f6c 6563 756c 6172 2046 6f72 6365 2046  olecular Force F
-00073b20: 6965 6c64 2066 6f72 2049 6f6e 6963 204c  ield for Ionic L
-00073b30: 6971 7569 6473 2043 6f6d 706f 7365 6420  iquids Composed 
-00073b40: 6f66 2054 7269 666c 6174 6520 6f72 2042  of Triflate or B
-00073b50: 6973 7472 6966 6c79 6c69 6d69 6465 2041  istriflylimide A
-00073b60: 6e69 6f6e 732e 0a4a 2050 6879 7320 4368  nions..J Phys Ch
-00073b70: 656d 2042 2032 3030 342c 2031 3038 2028  em B 2004, 108 (
-00073b80: 3433 292c 2031 3638 3933 e280 9331 3638  43), 16893...168
-00073b90: 3938 2e0a 6874 7470 733a 2f2f 646f 692e  98..https://doi.
-00073ba0: 6f72 672f 3130 2e31 3032 312f 6a70 3034  org/10.1021/jp04
-00073bb0: 3736 3534 352e 0a0a 0a40 6172 7469 636c  76545....@articl
-00073bc0: 657b 3130 2e31 3032 312f 6a70 3034 3736  e{10.1021/jp0476
-00073bd0: 3534 352c 200d 0a79 6561 7220 3d20 7b32  545, ..year = {2
-00073be0: 3030 347d 2c20 0d0a 7469 746c 6520 3d20  004}, ..title = 
-00073bf0: 7b7b 4d6f 6c65 6375 6c61 7220 466f 7263  {{Molecular Forc
-00073c00: 6520 4669 656c 6420 666f 7220 496f 6e69  e Field for Ioni
-00073c10: 6320 4c69 7175 6964 7320 436f 6d70 6f73  c Liquids Compos
-00073c20: 6564 206f 6620 5472 6966 6c61 7465 206f  ed of Triflate o
-00073c30: 7220 4269 7374 7269 666c 796c 696d 6964  r Bistriflylimid
-00073c40: 6520 416e 696f 6e73 7d7d 2c20 0d0a 6175  e Anions}}, ..au
-00073c50: 7468 6f72 203d 207b 4c6f 7065 732c 204a  thor = {Lopes, J
-00073c60: 6f73 c3a9 204e 2e20 4361 6e6f 6e67 6961  os.. N. Canongia
-00073c70: 2061 6e64 2050 c3a1 6475 612c 2041 67c3   and P..dua, Ag.
-00073c80: ad6c 696f 2041 2e20 482e 7d2c 200d 0a6a  .lio A. H.}, ..j
-00073c90: 6f75 726e 616c 203d 207b 5468 6520 4a6f  ournal = {The Jo
-00073ca0: 7572 6e61 6c20 6f66 2050 6879 7369 6361  urnal of Physica
-00073cb0: 6c20 4368 656d 6973 7472 7920 427d 2c20  l Chemistry B}, 
-00073cc0: 0d0a 6973 736e 203d 207b 3135 3230 2d36  ..issn = {1520-6
-00073cd0: 3130 367d 2c20 0d0a 646f 6920 3d20 7b31  106}, ..doi = {1
-00073ce0: 302e 3130 3231 2f6a 7030 3437 3635 3435  0.1021/jp0476545
-00073cf0: 7d2c 200d 0a70 6167 6573 203d 207b 3136  }, ..pages = {16
-00073d00: 3839 332d 2d31 3638 3938 7d2c 200d 0a6e  893--16898}, ..n
-00073d10: 756d 6265 7220 3d20 7b34 337d 2c20 0d0a  umber = {43}, ..
-00073d20: 766f 6c75 6d65 203d 207b 3130 387d 2c20  volume = {108}, 
-00073d30: 0d0a 7d0a 0a23 7265 6665 7265 6e63 6520  ..}..#reference 
-00073d40: 340a 4041 7574 686f 7220 5061 756c 2053  4.@Author Paul S
-00073d50: 6178 650a 4044 6174 6520 3230 3233 2d30  axe.@Date 2023-0
-00073d60: 312d 3239 0a0a 6164 6465 6420 6d69 7373  1-29..added miss
-00073d70: 696e 6720 616e 676c 6520 7061 7261 6d65  ing angle parame
-00073d80: 7465 7273 0a20 2020 2020 204f 2d43 283d  ters.      O-C(=
-00073d90: 4f29 2d4f 2066 6f72 2063 6172 626f 6e61  O)-O for carbona
-00073da0: 7465 730a 2020 2020 2020 462d 432d 4f20  tes.      F-C-O 
-00073db0: 7768 6572 6520 4f20 6973 2063 6172 626f  where O is carbo
-00073dc0: 6e61 7465 2065 7374 6572 206f 7879 6765  nate ester oxyge
-00073dd0: 6e0a 2020 2020 2020 4f2d 432d 4f2d 4320  n.      O-C-O-C 
-00073de0: 7768 6572 6520 3173 7420 7468 7265 6520  where 1st three 
-00073df0: 6174 6f6d 7320 6172 6520 6163 726f 7373  atoms are across
-00073e00: 2063 6172 626f 6e61 7465 2061 6e64 206c   carbonate and l
-00073e10: 6173 7420 4320 6973 2043 2069 6e20 6574  ast C is C in et
-00073e20: 6879 6c65 6e65 206d 6f69 6574 790a 0a20  hylene moiety.. 
-00073e30: 2020 2020 2054 6f72 7369 6f6e 2037 3134       Torsion 714
-00073e40: 2d38 312d 3832 2d37 3836 0a20 2020 2020  -81-82-786.     
-00073e50: 204f 2d43 4832 2d43 482d 4620 696e 2046   O-CH2-CH-F in F
-00073e60: 4543 202d 2d3e 2034 312d 3138 2d31 382d  EC --> 41-18-18-
-00073e70: 310a 0a20 2020 2020 2054 6f72 7369 6f6e  1..      Torsion
-00073e80: 2037 3836 2d38 322d 3731 342d 3731 3320   786-82-714-713 
-00073e90: 2d3e 2031 2d31 382d 3431 2d33 0a20 2020  -> 1-18-41-3.   
-00073ea0: 2020 2046 2d43 482d 4f2d 4328 3d4f 2920     F-CH-O-C(=O) 
-00073eb0: 696e 2046 4543 0a20 2020 2020 200a 6672  in FEC.      .fr
-00073ec0: 6f6d 204c 6962 5061 7247 656e 206f 6e20  om LibParGen on 
-00073ed0: 4543 2061 6e64 2046 4543 2028 6574 6879  EC and FEC (ethy
-00073ee0: 6c65 6e65 2063 6172 626f 6e61 7465 2061  lene carbonate a
-00073ef0: 6e64 2066 6c75 6f72 6f65 7468 796c 656e  nd fluoroethylen
-00073f00: 6520 6361 7262 6f6e 6174 6529 0a23 656e  e carbonate).#en
-00073f10: 640a                                     d.
+000733f0: 7320 5468 6574 6130 2064 6567 7265 650a  s Theta0 degree.
+00073400: 4075 6e69 7473 204b 3220 6b4a 2f6d 6f6c  @units K2 kJ/mol
+00073410: 2f72 6164 6961 6e5e 320a 0a21 2056 6572  /radian^2..! Ver
+00073420: 7369 6f6e 2020 2052 6566 2020 2049 2020  sion   Ref   I  
+00073430: 2020 2020 2020 204a 2020 2020 2020 2020         J        
+00073440: 204b 2020 2020 2020 2020 2020 2054 6865   K           The
+00073450: 7461 3020 2020 2020 2020 204b 320a 212d  ta0        K2.!-
+00073460: 2d2d 2d2d 2d2d 2d2d 2020 2d2d 2d2d 2020  --------  ----  
+00073470: 2d2d 2d2d 2d2d 2d2d 2020 2d2d 2d2d 2d2d  --------  ------
+00073480: 2d2d 2020 2d2d 2d2d 2d2d 2d2d 2020 2d2d  --  --------  --
+00073490: 2d2d 2d2d 2d2d 2020 2d2d 2d2d 2d2d 2d2d  ------  --------
+000734a0: 0a32 3032 332e 3031 2e32 3920 2033 2020  .2023.01.29  3  
+000734b0: 2020 2046 5020 2020 2020 2020 2050 2020     FP        P  
+000734c0: 2020 2020 2020 2046 5020 2020 2020 2020         FP       
+000734d0: 2020 2039 302e 3020 2020 2020 2031 3136     90.0      116
+000734e0: 352e 300a 0a0a 0a23 7369 6d70 6c65 5f66  5.0....#simple_f
+000734f0: 6f75 7269 6572 5f61 6e67 6c65 2020 2020  ourier_angle    
+00073500: 2020 2043 4c26 502d 6f70 6c73 6161 0a0a     CL&P-oplsaa..
+00073510: 3e20 4520 3d20 4b20 2a20 5b31 202d 2063  > E = K * [1 - c
+00073520: 6f73 286e 2a54 6865 7461 295d 0a3e 0a3e  os(n*Theta)].>.>
+00073530: 2020 2020 4b20 3d20 4b32 2871 7561 6472      K = K2(quadr
+00073540: 6174 6963 2920 2f20 380a 0a40 756e 6974  atic) / 8..@unit
+00073550: 7320 4b20 6b4a 2f6d 6f6c 0a0a 2120 5665  s K kJ/mol..! Ve
+00073560: 7273 696f 6e20 2020 5265 6620 2020 4920  rsion   Ref   I 
+00073570: 2020 2020 2020 2020 4a20 2020 2020 2020          J       
+00073580: 2020 4b20 2020 2020 2020 2020 2020 204b    K            K
+00073590: 2020 2020 2020 2020 206e 0a21 2d2d 2d2d           n.!----
+000735a0: 2d2d 2d2d 2d20 202d 2d2d 2d20 202d 2d2d  -----  ----  ---
+000735b0: 2d2d 2d2d 2d20 202d 2d2d 2d2d 2d2d 2d20  -----  -------- 
+000735c0: 202d 2d2d 2d2d 2d2d 2d20 202d 2d2d 2d2d   --------  -----
+000735d0: 2d2d 2d20 2020 202d 2d2d 0a32 3032 332e  ---    ---.2023.
+000735e0: 3031 2e32 3920 2035 2020 2020 2046 5020  01.29  5     FP 
+000735f0: 2020 2020 2020 2050 2020 2020 2020 2020         P        
+00073600: 2046 5020 2020 2020 2020 2020 3134 352e   FP         145.
+00073610: 3620 2020 2020 2020 340a 0a23 7465 6d70  6       4..#temp
+00073620: 6c61 7465 7320 434c 2650 2d6f 706c 7361  lates CL&P-oplsa
+00073630: 610a 7b0a 2020 2020 2250 223a 207b 0a20  a.{.    "P": {. 
+00073640: 2020 2020 2020 2022 3230 3233 2e30 312e         "2023.01.
+00073650: 3239 223a 207b 0a20 2020 2020 2020 2020  29": {.         
+00073660: 2020 2022 736d 6172 7473 223a 205b 0a20     "smarts": [. 
+00073670: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00073680: 5b50 3a31 5d28 4629 2846 2928 4629 2846  [P:1](F)(F)(F)(F
+00073690: 2928 4629 4622 0a20 2020 2020 2020 2020  )(F)F".         
+000736a0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+000736b0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+000736c0: 2022 5068 6f73 7068 6f72 6f75 7320 696e   "Phosphorous in
+000736d0: 2050 4636 2d22 2c0a 2020 2020 2020 2020   PF6-",.        
+000736e0: 2020 2020 226f 7665 7272 6964 6573 223a      "overrides":
+000736f0: 205b 5d0a 2020 2020 2020 2020 7d0a 2020   [].        }.  
+00073700: 2020 7d2c 0a20 2020 2022 4650 223a 207b    },.    "FP": {
+00073710: 0a20 2020 2020 2020 2022 3230 3233 2e30  .        "2023.0
+00073720: 312e 3239 223a 207b 0a20 2020 2020 2020  1.29": {.       
+00073730: 2020 2020 2022 736d 6172 7473 223a 205b       "smarts": [
+00073740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00073750: 2022 5b50 5d28 5b46 3a31 5d29 285b 463a   "[P]([F:1])([F:
+00073760: 325d 2928 5b46 3a33 5d29 285b 463a 345d  2])([F:3])([F:4]
+00073770: 2928 5b46 3a35 5d29 5b46 3a36 5d22 0a20  )([F:5])[F:6]". 
+00073780: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00073790: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000737a0: 6970 7469 6f6e 223a 2022 466c 756f 7269  iption": "Fluori
+000737b0: 6e65 2069 6e20 5046 362d 222c 0a20 2020  ne in PF6-",.   
+000737c0: 2020 2020 2020 2020 2022 6f76 6572 7269           "overri
+000737d0: 6465 7322 3a20 5b5d 0a20 2020 2020 2020  des": [].       
+000737e0: 207d 0a20 2020 207d 0a7d 0a0a 2372 6566   }.    }.}..#ref
+000737f0: 6572 656e 6365 2031 0a40 4175 7468 6f72  erence 1.@Author
+00073800: 2050 6175 6c20 5361 7865 0a40 4461 7465   Paul Saxe.@Date
+00073810: 2032 3032 332d 3031 2d32 390a 4f50 4c53   2023-01-29.OPLS
+00073820: 4141 2066 6f72 6365 6669 656c 6420 7472  AA forcefield tr
+00073830: 616e 736c 6174 6564 2066 726f 6d20 5469  anslated from Ti
+00073840: 6e6b 6572 2076 6572 7369 6f6e 2e0a 2365  nker version..#e
+00073850: 6e64 0a0a 2372 6566 6572 656e 6365 2032  nd..#reference 2
+00073860: 0a40 4175 7468 6f72 2050 6175 6c20 5361  .@Author Paul Sa
+00073870: 7865 0a40 4461 7465 2032 3032 332d 3031  xe.@Date 2023-01
+00073880: 2d32 390a 0a4c 6f70 6573 2c20 4a2e 204e  -29..Lopes, J. N
+00073890: 2e20 432e 3b20 4465 7363 6861 6d70 732c  . C.; Deschamps,
+000738a0: 204a 2e3b 2050 c3a1 6475 612c 2041 2e20   J.; P..dua, A. 
+000738b0: 412e 2048 2e0a 4d6f 6465 6c69 6e67 2049  A. H..Modeling I
+000738c0: 6f6e 6963 204c 6971 7569 6473 2055 7369  onic Liquids Usi
+000738d0: 6e67 2061 2053 7973 7465 6d61 7469 6320  ng a Systematic 
+000738e0: 416c 6c2d 4174 6f6d 2046 6f72 6365 2046  All-Atom Force F
+000738f0: 6965 6c64 2e0a 4a20 5068 7973 2043 6865  ield..J Phys Che
+00073900: 6d20 4220 3230 3034 2c20 3130 3820 2836  m B 2004, 108 (6
+00073910: 292c 2032 3033 38e2 8093 3230 3437 2e0a  ), 2038...2047..
+00073920: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00073930: 3130 2e31 3032 312f 6a70 3033 3632 3133  10.1021/jp036213
+00073940: 332e 0a0a 0a40 6172 7469 636c 657b 3130  3....@article{10
+00073950: 2e31 3032 312f 6a70 3033 3632 3133 332c  .1021/jp0362133,
+00073960: 200d 0a79 6561 7220 3d20 7b32 3030 347d   ..year = {2004}
+00073970: 2c20 0d0a 7469 746c 6520 3d20 7b7b 4d6f  , ..title = {{Mo
+00073980: 6465 6c69 6e67 2049 6f6e 6963 204c 6971  deling Ionic Liq
+00073990: 7569 6473 2055 7369 6e67 2061 2053 7973  uids Using a Sys
+000739a0: 7465 6d61 7469 6320 416c 6c2d 4174 6f6d  tematic All-Atom
+000739b0: 2046 6f72 6365 2046 6965 6c64 7d7d 2c20   Force Field}}, 
+000739c0: 0d0a 6175 7468 6f72 203d 207b 4c6f 7065  ..author = {Lope
+000739d0: 732c 204a 6f73 c3a9 204e 2e20 4361 6e6f  s, Jos.. N. Cano
+000739e0: 6e67 6961 2061 6e64 2044 6573 6368 616d  ngia and Descham
+000739f0: 7073 2c20 4a6f 686e 6e79 2061 6e64 2050  ps, Johnny and P
+00073a00: c3a1 6475 612c 2041 67c3 ad6c 696f 2041  ..dua, Ag..lio A
+00073a10: 2e20 482e 7d2c 200d 0a6a 6f75 726e 616c  . H.}, ..journal
+00073a20: 203d 207b 5468 6520 4a6f 7572 6e61 6c20   = {The Journal 
+00073a30: 6f66 2050 6879 7369 6361 6c20 4368 656d  of Physical Chem
+00073a40: 6973 7472 7920 427d 2c20 0d0a 6973 736e  istry B}, ..issn
+00073a50: 203d 207b 3135 3230 2d36 3130 367d 2c20   = {1520-6106}, 
+00073a60: 0d0a 646f 6920 3d20 7b31 302e 3130 3231  ..doi = {10.1021
+00073a70: 2f6a 7030 3336 3231 3333 7d2c 200d 0a70  /jp0362133}, ..p
+00073a80: 6167 6573 203d 207b 3230 3338 2d2d 3230  ages = {2038--20
+00073a90: 3437 7d2c 200d 0a6e 756d 6265 7220 3d20  47}, ..number = 
+00073aa0: 7b36 7d2c 200d 0a76 6f6c 756d 6520 3d20  {6}, ..volume = 
+00073ab0: 7b31 3038 7d2c 200d 0a7d 0a0a 0a23 7265  {108}, ..}...#re
+00073ac0: 6665 7265 6e63 6520 330a 4041 7574 686f  ference 3.@Autho
+00073ad0: 7220 5061 756c 2053 6178 650a 4044 6174  r Paul Saxe.@Dat
+00073ae0: 6520 3230 3233 2d30 312d 3239 0a0a 4c6f  e 2023-01-29..Lo
+00073af0: 7065 732c 204a 2e20 4e2e 2043 2e3b 2050  pes, J. N. C.; P
+00073b00: c3a1 6475 612c 2041 2e20 412e 2048 2e0a  ..dua, A. A. H..
+00073b10: 4d6f 6c65 6375 6c61 7220 466f 7263 6520  Molecular Force 
+00073b20: 4669 656c 6420 666f 7220 496f 6e69 6320  Field for Ionic 
+00073b30: 4c69 7175 6964 7320 436f 6d70 6f73 6564  Liquids Composed
+00073b40: 206f 6620 5472 6966 6c61 7465 206f 7220   of Triflate or 
+00073b50: 4269 7374 7269 666c 796c 696d 6964 6520  Bistriflylimide 
+00073b60: 416e 696f 6e73 2e0a 4a20 5068 7973 2043  Anions..J Phys C
+00073b70: 6865 6d20 4220 3230 3034 2c20 3130 3820  hem B 2004, 108 
+00073b80: 2834 3329 2c20 3136 3839 33e2 8093 3136  (43), 16893...16
+00073b90: 3839 382e 0a68 7474 7073 3a2f 2f64 6f69  898..https://doi
+00073ba0: 2e6f 7267 2f31 302e 3130 3231 2f6a 7030  .org/10.1021/jp0
+00073bb0: 3437 3635 3435 2e0a 0a0a 4061 7274 6963  476545....@artic
+00073bc0: 6c65 7b31 302e 3130 3231 2f6a 7030 3437  le{10.1021/jp047
+00073bd0: 3635 3435 2c20 0d0a 7965 6172 203d 207b  6545, ..year = {
+00073be0: 3230 3034 7d2c 200d 0a74 6974 6c65 203d  2004}, ..title =
+00073bf0: 207b 7b4d 6f6c 6563 756c 6172 2046 6f72   {{Molecular For
+00073c00: 6365 2046 6965 6c64 2066 6f72 2049 6f6e  ce Field for Ion
+00073c10: 6963 204c 6971 7569 6473 2043 6f6d 706f  ic Liquids Compo
+00073c20: 7365 6420 6f66 2054 7269 666c 6174 6520  sed of Triflate 
+00073c30: 6f72 2042 6973 7472 6966 6c79 6c69 6d69  or Bistriflylimi
+00073c40: 6465 2041 6e69 6f6e 737d 7d2c 200d 0a61  de Anions}}, ..a
+00073c50: 7574 686f 7220 3d20 7b4c 6f70 6573 2c20  uthor = {Lopes, 
+00073c60: 4a6f 73c3 a920 4e2e 2043 616e 6f6e 6769  Jos.. N. Canongi
+00073c70: 6120 616e 6420 50c3 a164 7561 2c20 4167  a and P..dua, Ag
+00073c80: c3ad 6c69 6f20 412e 2048 2e7d 2c20 0d0a  ..lio A. H.}, ..
+00073c90: 6a6f 7572 6e61 6c20 3d20 7b54 6865 204a  journal = {The J
+00073ca0: 6f75 726e 616c 206f 6620 5068 7973 6963  ournal of Physic
+00073cb0: 616c 2043 6865 6d69 7374 7279 2042 7d2c  al Chemistry B},
+00073cc0: 200d 0a69 7373 6e20 3d20 7b31 3532 302d   ..issn = {1520-
+00073cd0: 3631 3036 7d2c 200d 0a64 6f69 203d 207b  6106}, ..doi = {
+00073ce0: 3130 2e31 3032 312f 6a70 3034 3736 3534  10.1021/jp047654
+00073cf0: 357d 2c20 0d0a 7061 6765 7320 3d20 7b31  5}, ..pages = {1
+00073d00: 3638 3933 2d2d 3136 3839 387d 2c20 0d0a  6893--16898}, ..
+00073d10: 6e75 6d62 6572 203d 207b 3433 7d2c 200d  number = {43}, .
+00073d20: 0a76 6f6c 756d 6520 3d20 7b31 3038 7d2c  .volume = {108},
+00073d30: 200d 0a7d 0a0a 2372 6566 6572 656e 6365   ..}..#reference
+00073d40: 2034 0a40 4175 7468 6f72 2050 6175 6c20   4.@Author Paul 
+00073d50: 5361 7865 0a40 4461 7465 2032 3032 332d  Saxe.@Date 2023-
+00073d60: 3031 2d32 390a 0a61 6464 6564 206d 6973  01-29..added mis
+00073d70: 7369 6e67 2061 6e67 6c65 2070 6172 616d  sing angle param
+00073d80: 6574 6572 730a 2020 2020 2020 4f2d 4328  eters.      O-C(
+00073d90: 3d4f 292d 4f20 666f 7220 6361 7262 6f6e  =O)-O for carbon
+00073da0: 6174 6573 0a20 2020 2020 2046 2d43 2d4f  ates.      F-C-O
+00073db0: 2077 6865 7265 204f 2069 7320 6361 7262   where O is carb
+00073dc0: 6f6e 6174 6520 6573 7465 7220 6f78 7967  onate ester oxyg
+00073dd0: 656e 0a20 2020 2020 204f 2d43 2d4f 2d43  en.      O-C-O-C
+00073de0: 2077 6865 7265 2031 7374 2074 6872 6565   where 1st three
+00073df0: 2061 746f 6d73 2061 7265 2061 6372 6f73   atoms are acros
+00073e00: 7320 6361 7262 6f6e 6174 6520 616e 6420  s carbonate and 
+00073e10: 6c61 7374 2043 2069 7320 4320 696e 2065  last C is C in e
+00073e20: 7468 796c 656e 6520 6d6f 6965 7479 0a0a  thylene moiety..
+00073e30: 2020 2020 2020 546f 7273 696f 6e20 3731        Torsion 71
+00073e40: 342d 3831 2d38 322d 3738 360a 2020 2020  4-81-82-786.    
+00073e50: 2020 4f2d 4348 322d 4348 2d46 2069 6e20    O-CH2-CH-F in 
+00073e60: 4645 4320 2d2d 3e20 3431 2d31 382d 3138  FEC --> 41-18-18
+00073e70: 2d31 0a0a 2020 2020 2020 546f 7273 696f  -1..      Torsio
+00073e80: 6e20 3738 362d 3832 2d37 3134 2d37 3133  n 786-82-714-713
+00073e90: 202d 3e20 312d 3138 2d34 312d 330a 2020   -> 1-18-41-3.  
+00073ea0: 2020 2020 462d 4348 2d4f 2d43 283d 4f29      F-CH-O-C(=O)
+00073eb0: 2069 6e20 4645 430a 2020 2020 2020 0a66   in FEC.      .f
+00073ec0: 726f 6d20 4c69 6250 6172 4765 6e20 6f6e  rom LibParGen on
+00073ed0: 2045 4320 616e 6420 4645 4320 2865 7468   EC and FEC (eth
+00073ee0: 796c 656e 6520 6361 7262 6f6e 6174 6520  ylene carbonate 
+00073ef0: 616e 6420 666c 756f 726f 6574 6879 6c65  and fluoroethyle
+00073f00: 6e65 2063 6172 626f 6e61 7465 290a 2365  ne carbonate).#e
+00073f10: 6e64 0a                                  nd.
```

### Comparing `forcefield_step-2023.4.6/forcefield_step/data/pcff2018.frc` & `forcefield_step-2023.5.1/forcefield_step/data/pcff2018.frc`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/forcefield.py` & `forcefield_step-2023.5.1/forcefield_step/forcefield.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/forcefield_parameters.py` & `forcefield_step-2023.5.1/forcefield_step/forcefield_parameters.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/forcefield_step.py` & `forcefield_step-2023.5.1/forcefield_step/forcefield_step.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step/tk_forcefield.py` & `forcefield_step-2023.5.1/forcefield_step/tk_forcefield.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/forcefield_step.egg-info/PKG-INFO` & `forcefield_step-2023.5.1/forcefield_step.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcefield-step
-Version: 2023.4.6
+Version: 2023.5.1
 Summary: A SEAMM plug-in for setting up a forcefield or EAM potentials for subsequent simulations.
 Home-page: https://github.com/molssi-seam/forcefield_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM
 Platform: Linux
@@ -83,14 +83,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.5.1 -- Fixed bug in Lithium battery forcefield
+  * Fixed a typo in the angle type unit line which caused a crash
+    
 2023.4.6 -- Added Lithium battery forcefield
   * An initial set of parameters for cathode materials, specifically LiCoO2.
 
 2023.2.13 -- Added OPLS-AA forcefield
   * Added parameters for OPLS-AA along with some extra parameters for ionic liquids
     * PF6-
     * ethylene carbonate (EC) and fluoronated EC (FEC)
```

### Comparing `forcefield_step-2023.4.6/forcefield_step.egg-info/SOURCES.txt` & `forcefield_step-2023.5.1/forcefield_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/setup.py` & `forcefield_step-2023.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/tests/conftest.py` & `forcefield_step-2023.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/tests/test_forcefield_step.py` & `forcefield_step-2023.5.1/tests/test_forcefield_step.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.4.6/tests/test_oplsaa_assignment.py` & `forcefield_step-2023.5.1/tests/test_oplsaa_assignment.py`

 * *Files identical despite different names*

