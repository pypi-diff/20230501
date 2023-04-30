# Comparing `tmp/repository-cli-0.5.0.tar.gz` & `tmp/repository-cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repository-cli-0.5.0.tar", last modified: Wed Mar  8 08:13:56 2023, max compression
+gzip compressed data, was "repository-cli-0.6.0.tar", last modified: Sun Apr 30 22:39:32 2023, max compression
```

## Comparing `repository-cli-0.5.0.tar` & `repository-cli-0.6.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.483411 repository-cli-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-08 08:13:49.000000 repository-cli-0.5.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.475411 repository-cli-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.479411 repository-cli-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-08 08:13:49.000000 repository-cli-0.5.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-08 08:13:49.000000 repository-cli-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-08 08:13:49.000000 repository-cli-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-08 08:13:49.000000 repository-cli-0.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-08 08:13:49.000000 repository-cli-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-08 08:13:49.000000 repository-cli-0.5.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-08 08:13:49.000000 repository-cli-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-08 08:13:49.000000 repository-cli-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-08 08:13:56.483411 repository-cli-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-08 08:13:49.000000 repository-cli-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.479411 repository-cli-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-08 08:13:49.000000 repository-cli-0.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.479411 repository-cli-0.5.0/repository_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/click_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/click_param_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-08 08:13:49.000000 repository-cli-0.5.0/repository_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.479411 repository-cli-0.5.0/repository_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 08:13:56.000000 repository-cli-0.5.0/repository_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-08 08:13:49.000000 repository-cli-0.5.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-03-08 08:13:49.000000 repository-cli-0.5.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-08 08:13:56.483411 repository-cli-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-08 08:13:49.000000 repository-cli-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 08:13:56.479411 repository-cli-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-08 08:13:49.000000 repository-cli-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-03-08 08:13:49.000000 repository-cli-0.5.0/tests/test_rdmrecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-08 08:13:49.000000 repository-cli-0.5.0/tests/test_rdmrecords_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-08 08:13:49.000000 repository-cli-0.5.0/tests/test_rdmrecords_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-08 08:13:49.000000 repository-cli-0.5.0/tests/test_repository_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 22:39:26.000000 repository-cli-0.6.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.196524 repository-cli-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.196524 repository-cli-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-30 22:39:26.000000 repository-cli-0.6.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 22:39:26.000000 repository-cli-0.6.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-30 22:39:26.000000 repository-cli-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-30 22:39:26.000000 repository-cli-0.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-30 22:39:26.000000 repository-cli-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-30 22:39:26.000000 repository-cli-0.6.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-30 22:39:26.000000 repository-cli-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-30 22:39:26.000000 repository-cli-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-30 22:39:32.200523 repository-cli-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-30 22:39:26.000000 repository-cli-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.196524 repository-cli-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-30 22:39:26.000000 repository-cli-0.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/repository_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/click_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-30 22:39:26.000000 repository-cli-0.6.0/repository_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/repository_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 22:39:32.000000 repository-cli-0.6.0/repository_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-30 22:39:26.000000 repository-cli-0.6.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-30 22:39:26.000000 repository-cli-0.6.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-30 22:39:32.200523 repository-cli-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-30 22:39:26.000000 repository-cli-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:39:32.200523 repository-cli-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_rdmrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_rdmrecords_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_rdmrecords_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-30 22:39:26.000000 repository-cli-0.6.0/tests/test_repository_cli.py
```

### Comparing `repository-cli-0.5.0/.github/workflows/tests.yml` & `repository-cli-0.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/CHANGES.rst` & `repository-cli-0.6.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.6.0 (release 2023-05-01)
+
+- cli: add command publish
+- cli: add record_id parameter to modify-access
+
+
 Version v0.5.0 (release 2023-03-08)
 
 - setup: remove python 3.11
 - records: add command modify-access
 - records: change add-file command to common pattern
```

### Comparing `repository-cli-0.5.0/CONTRIBUTING.rst` & `repository-cli-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/LICENSE` & `repository-cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/MANIFEST.in` & `repository-cli-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/PKG-INFO` & `repository-cli-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.5.0
+Version: 0.6.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.6.0 (release 2023-05-01)
+
+- cli: add command publish
+- cli: add record_id parameter to modify-access
+
+
 Version v0.5.0 (release 2023-03-08)
 
 - setup: remove python 3.11
 - records: add command modify-access
 - records: change add-file command to common pattern
```

### Comparing `repository-cli-0.5.0/README.rst` & `repository-cli-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/docs/Makefile` & `repository-cli-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/docs/api.rst` & `repository-cli-0.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/docs/conf.py` & `repository-cli-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/docs/index.rst` & `repository-cli-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/docs/make.bat` & `repository-cli-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/cli.py` & `repository-cli-0.6.0/repository_cli/cli.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/click_options.py` & `repository-cli-0.6.0/repository_cli/click_options.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/click_param_types.py` & `repository-cli-0.6.0/repository_cli/click_param_types.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/ext.py` & `repository-cli-0.6.0/repository_cli/ext.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/records.py` & `repository-cli-0.6.0/repository_cli/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -551,31 +551,57 @@
         secho("File added successfully.", fg=Color.success)
     else:
         secho("File addition aborted.", fg=Color.abort)
 
 
 @group_records.command("modify-access")
 @option_data_model
-@option_input_file(type_=JSON(), name="record_ids", help_="json array of ids")
+@option_input_file(
+    type_=JSON(), name="record_ids", help_="json array of ids", required=False
+)
+@click.option("--record-id", type=click.STRING)
 @click.option(
     "--access-record", default=None, type=click.Choice(["public", "restricted"])
 )
 @click.option(
     "--access-file", default=None, type=click.Choice(["public", "restricted"])
 )
 @with_appcontext
-def modify_access(data_model, record_ids, access_record, access_file):
+def modify_access(data_model, record_ids, record_id, access_record, access_file):
     """Modify the access object within the record."""
     identity = get_identity("system_process", role_name="admin")
     service = get_records_service(data_model=data_model)
 
-    for record_id in record_ids:
-        data = service.read(id_=record_id, identity=identity).data
+    if not record_ids and record_id:
+        record_ids = [record_id]
+
+    for rec_id in record_ids:
+        data = service.read(id_=rec_id, identity=identity).data
 
         if access_record:
             data["access"]["record"] = access_record
         if access_file:
             data["access"]["files"] = access_file
 
-        service.edit(id_=record_id, identity=identity)
-        service.update_draft(id_=record_id, identity=identity, data=data)
-        service.publish(id_=record_id, identity=identity)
+        service.edit(id_=rec_id, identity=identity)
+        service.update_draft(id_=rec_id, identity=identity, data=data)
+        service.publish(id_=rec_id, identity=identity)
+
+
+@group_records.command("publish")
+@option_data_model
+@option_input_file(
+    type_=JSON(), name="record_ids", help_="json array of ids", required=False
+)
+@click.option("--record-id", type=click.STRING)
+@with_appcontext
+def publish(data_model, record_ids, record_id):
+    """Publish all records."""
+    identity = get_identity("system_process", role_name="admin")
+    service = get_records_service(data_model=data_model)
+
+    if not record_ids and record_id:
+        record_ids = [record_id]
+
+    for rec_id in record_ids:
+        record = service.publish(id_=rec_id, identity=identity)
+        secho(f"record ({record.id}) published", fg=Color.success)
```

### Comparing `repository-cli-0.5.0/repository_cli/types.py` & `repository-cli-0.6.0/repository_cli/types.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/users.py` & `repository-cli-0.6.0/repository_cli/users.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli/utils.py` & `repository-cli-0.6.0/repository_cli/utils.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/repository_cli.egg-info/PKG-INFO` & `repository-cli-0.6.0/repository_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.5.0
+Version: 0.6.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,20 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.6.0 (release 2023-05-01)
+
+- cli: add command publish
+- cli: add record_id parameter to modify-access
+
+
 Version v0.5.0 (release 2023-03-08)
 
 - setup: remove python 3.11
 - records: add command modify-access
 - records: change add-file command to common pattern
```

### Comparing `repository-cli-0.5.0/repository_cli.egg-info/SOURCES.txt` & `repository-cli-0.6.0/repository_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/run-tests.sh` & `repository-cli-0.6.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/setup.cfg` & `repository-cli-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/tests/conftest.py` & `repository-cli-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/tests/test_rdmrecords.py` & `repository-cli-0.6.0/tests/test_rdmrecords.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/tests/test_rdmrecords_identifiers.py` & `repository-cli-0.6.0/tests/test_rdmrecords_identifiers.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/tests/test_rdmrecords_pids.py` & `repository-cli-0.6.0/tests/test_rdmrecords_pids.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.5.0/tests/test_repository_cli.py` & `repository-cli-0.6.0/tests/test_repository_cli.py`

 * *Files identical despite different names*

