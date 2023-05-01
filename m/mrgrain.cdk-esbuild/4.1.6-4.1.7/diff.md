# Comparing `tmp/mrgrain.cdk-esbuild-4.1.6.tar.gz` & `tmp/mrgrain.cdk-esbuild-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-4.1.6.tar", last modified: Sat Apr 15 05:06:13 2023, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-4.1.7.tar", last modified: Mon May  1 05:05:46 2023, max compression
```

## Comparing `mrgrain.cdk-esbuild-4.1.6.tar` & `mrgrain.cdk-esbuild-4.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.522446 mrgrain.cdk-esbuild-4.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.522446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (123)   393083 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81277 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.1.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:06:00.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:06:13.526446 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 05:06:13.000000 mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:05:46.880431 mrgrain.cdk-esbuild-4.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-05-01 05:05:46.880431 mrgrain.cdk-esbuild-4.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 05:05:46.880431 mrgrain.cdk-esbuild-4.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:05:46.876431 mrgrain.cdk-esbuild-4.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:05:46.876431 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:05:46.880431 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)   393083 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:05:46.880431 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81279 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.1.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:05:33.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:05:46.880431 mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-05-01 05:05:46.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-01 05:05:46.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:05:46.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 05:05:46.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 05:05:46.000000 mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-4.1.6/LICENSE` & `mrgrain.cdk-esbuild-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.6/PKG-INFO` & `mrgrain.cdk-esbuild-4.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.1.6
+Version: 4.1.7
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `mrgrain.cdk-esbuild-4.1.6/README.md` & `mrgrain.cdk-esbuild-4.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.6/setup.py` & `mrgrain.cdk-esbuild-4.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "4.1.6",
+    "version": "4.1.7",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@4.1.6.jsii.tgz"
+            "cdk-esbuild@4.1.7.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `mrgrain.cdk-esbuild-4.1.6/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-4.1.7/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.6/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-4.1.7/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.1.6
+Version: 4.1.7
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

