# Comparing `tmp/mpc_orb-0.1.8.tar.gz` & `tmp/mpc_orb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_orb-0.1.8.tar", last modified: Sun Apr 30 23:20:13 2023, max compression
+gzip compressed data, was "mpc_orb-0.1.9.tar", last modified: Sun Apr 30 23:51:36 2023, max compression
```

## Comparing `mpc_orb-0.1.8.tar` & `mpc_orb-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb/demo_json/
--rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     8429 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb/schema_json/
--rw-r--r--   0 runner    (1001) docker     (122)    36424 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_latest.json
--rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.1.json
--rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.2.json
--rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.3.json
--rw-r--r--   0 runner    (1001) docker     (122)    36424 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.4.json
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/mpc_orb/validate_mpcorb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.176831 mpc_orb-0.1.8/mpc_orb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-30 23:20:13.000000 mpc_orb-0.1.8/mpc_orb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:20:13.180831 mpc_orb-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/filepaths_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-30 23:19:56.000000 mpc_orb-0.1.8/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/mpc_orb/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/mpc_orb/demo_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8429 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/mpc_orb/schema_json/
+-rw-r--r--   0 runner    (1001) docker     (122)    36424 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_latest.json
+-rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)    36424 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.4.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/mpc_orb/validate_mpcorb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/mpc_orb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-04-30 23:51:36.000000 mpc_orb-0.1.9/mpc_orb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-30 23:51:36.000000 mpc_orb-0.1.9/mpc_orb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 23:51:36.000000 mpc_orb-0.1.9/mpc_orb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 23:51:36.000000 mpc_orb-0.1.9/mpc_orb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-30 23:51:36.000000 mpc_orb-0.1.9/mpc_orb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-30 23:51:36.000000 mpc_orb-0.1.9/mpc_orb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:36.269741 mpc_orb-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/tests/filepaths_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/tests/test_filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/tests/test_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-30 23:51:18.000000 mpc_orb-0.1.9/tests/test_validation.py
```

### Comparing `mpc_orb-0.1.8/LICENSE` & `mpc_orb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/PKG-INFO` & `mpc_orb-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_orb
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/Smithsonian/mpc-public
 Author: MJP:MPC
 Author-email: mpayne@cfa.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpc-public/mpc_orb
```

### Comparing `mpc_orb-0.1.8/README.md` & `mpc_orb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/demo.py` & `mpc_orb-0.1.9/mpc_orb/demo.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json` & `mpc_orb-0.1.9/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/filepaths.py` & `mpc_orb-0.1.9/mpc_orb/filepaths.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/interpret.py` & `mpc_orb-0.1.9/mpc_orb/interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/parse.py` & `mpc_orb-0.1.9/mpc_orb/parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_latest.json` & `mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_latest.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.1.json` & `mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.1.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.2.json` & `mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.2.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.3.json` & `mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.3.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/schema_json/mpcorb_schema_v0.4.json` & `mpc_orb-0.1.9/mpc_orb/schema_json/mpcorb_schema_v0.4.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb/validate_mpcorb.py` & `mpc_orb-0.1.9/mpc_orb/validate_mpcorb.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/mpc_orb.egg-info/PKG-INFO` & `mpc_orb-0.1.9/mpc_orb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-orb
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/Smithsonian/mpc-public
 Author: MJP:MPC
 Author-email: mpayne@cfa.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpc-public/mpc_orb
```

### Comparing `mpc_orb-0.1.8/mpc_orb.egg-info/SOURCES.txt` & `mpc_orb-0.1.9/mpc_orb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/setup.py` & `mpc_orb-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mpc_orb',
-    version='0.1.8',
+    version='0.1.9',
     long_description=long_description,  
     long_description_content_type="text/markdown",
     author='MJP:MPC',
     author_email='mpayne@cfa.harvard.edu',
     url='https://github.com/Smithsonian/mpc-public',
     install_requires=[
         'jsonschema',
```

### Comparing `mpc_orb-0.1.8/tests/test_interpret.py` & `mpc_orb-0.1.9/tests/test_interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/tests/test_parse.py` & `mpc_orb-0.1.9/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.8/tests/test_validation.py` & `mpc_orb-0.1.9/tests/test_validation.py`

 * *Files identical despite different names*

