# Comparing `tmp/twarc2sql-0.2.2.tar.gz` & `tmp/twarc2sql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twarc2sql-0.2.2.tar", last modified: Sun Apr 23 14:58:43 2023, max compression
+gzip compressed data, was "twarc2sql-1.0.0.tar", last modified: Mon May  1 21:15:17 2023, max compression
```

## Comparing `twarc2sql-0.2.2.tar` & `twarc2sql-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.870145 twarc2sql-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/twarc2sql.db_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/twarc2sql.db_utils.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/twarc2sql.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.870145 twarc2sql-0.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-23 14:58:43.878145 twarc2sql-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.870145 twarc2sql-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.870145 twarc2sql-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/tests/data/.testenv
--rw-r--r--   0 runner    (1001) docker     (123)   521810 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/tests/data/example.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  3779875 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/tests/data/search_example.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/tests/test_twarc2sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/twarc2sql/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/twarc2sql/db_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/db_utils/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/db_utils/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/twarc2sql/db_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/db_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/db_utils/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/db_utils/tests/test_db_access.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/twarc2sql/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/file_utils/file_to_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/file_utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/file_utils/object_to_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 14:58:35.000000 twarc2sql-0.2.2/twarc2sql/twarc2sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:58:43.874145 twarc2sql-0.2.2/twarc2sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-23 14:58:43.000000 twarc2sql-0.2.2/twarc2sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 14:58:43.000000 twarc2sql-0.2.2/twarc2sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:58:43.000000 twarc2sql-0.2.2/twarc2sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:58:43.000000 twarc2sql-0.2.2/twarc2sql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-23 14:58:43.000000 twarc2sql-0.2.2/twarc2sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 14:58:43.000000 twarc2sql-0.2.2/twarc2sql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.167832 twarc2sql-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-01 21:15:17.167832 twarc2sql-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.155831 twarc2sql-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/twarc2sql.db_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/twarc2sql.db_utils.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/twarc2sql.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.155831 twarc2sql-1.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 21:15:17.167832 twarc2sql-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.155831 twarc2sql-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.155831 twarc2sql-1.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/tests/data/.testenv
+-rw-r--r--   0 runner    (1001) docker     (123)   521810 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/tests/data/example.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  3779875 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/tests/data/search_example.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/tests/test_twarc2sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.163832 twarc2sql-1.0.0/twarc2sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.163832 twarc2sql-1.0.0/twarc2sql/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/db_utils/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/db_utils/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.163832 twarc2sql-1.0.0/twarc2sql/db_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/db_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/db_utils/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/db_utils/tests/test_db_access.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.167832 twarc2sql-1.0.0/twarc2sql/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/file_utils/file_to_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/file_utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/file_utils/object_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 21:15:06.000000 twarc2sql-1.0.0/twarc2sql/twarc2sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:17.163832 twarc2sql-1.0.0/twarc2sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-01 21:15:17.000000 twarc2sql-1.0.0/twarc2sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-01 21:15:17.000000 twarc2sql-1.0.0/twarc2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:15:17.000000 twarc2sql-1.0.0/twarc2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:15:16.000000 twarc2sql-1.0.0/twarc2sql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 21:15:17.000000 twarc2sql-1.0.0/twarc2sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 21:15:17.000000 twarc2sql-1.0.0/twarc2sql.egg-info/top_level.txt
```

### Comparing `twarc2sql-0.2.2/CONTRIBUTING.rst` & `twarc2sql-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/LICENSE` & `twarc2sql-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/PKG-INFO` & `twarc2sql-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twarc2sql
-Version: 0.2.2
+Version: 1.0.0
 Summary: This package converts jsonl file generated by twarc2 to sql database in an opnionated way.
 Home-page: https://github.com/unna97/twarc2sql
 Author: Unnati Patel
 Author-email: unnati97@gmail.com
 License: MIT license
 Keywords: twarc2sql
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `twarc2sql-0.2.2/README.rst` & `twarc2sql-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/docs/Makefile` & `twarc2sql-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/docs/conf.py` & `twarc2sql-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/docs/installation.rst` & `twarc2sql-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/docs/make.bat` & `twarc2sql-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/docs/twarc2sql.db_utils.rst` & `twarc2sql-1.0.0/docs/twarc2sql.db_utils.rst`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/setup.py` & `twarc2sql-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,11 +49,11 @@
     include_package_data=True,
     keywords="twarc2sql",
     name="twarc2sql",
     packages=find_packages(include=["twarc2sql", "twarc2sql.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/unna97/twarc2sql",
-    version="0.2.2",
+    version="1.0.0",
     zip_safe=False,
     extras_require=extras_require,
 )
```

### Comparing `twarc2sql-0.2.2/tests/data/example.jsonl` & `twarc2sql-1.0.0/tests/data/example.jsonl`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/tests/data/search_example.jsonl` & `twarc2sql-1.0.0/tests/data/search_example.jsonl`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/tests/test_twarc2sql.py` & `twarc2sql-1.0.0/tests/test_twarc2sql.py`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/twarc2sql/db_utils/db_access.py` & `twarc2sql-1.0.0/twarc2sql/db_utils/db_access.py`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/twarc2sql/db_utils/tests/conftest.py` & `twarc2sql-1.0.0/twarc2sql/db_utils/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,17 @@
             "in_reply_to_user_id",
             "tweet_type",
             "retweet_count",
             "reply_count",
             "like_count",
             "quote_count",
             "impression_count",
-            "edits_remaining",
-            "is_edit_eligible",
-            "editable_until",
+            # "edits_remaining",
+            # "is_edit_eligible",
+            # "editable_until",
         ],
         "author": [
             "id",
             "name",
             "username",
             "created_at",
             "description",
```

### Comparing `twarc2sql-0.2.2/twarc2sql/db_utils/tests/test_db_access.py` & `twarc2sql-1.0.0/twarc2sql/db_utils/tests/test_db_access.py`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/twarc2sql/file_utils/file_to_object.py` & `twarc2sql-1.0.0/twarc2sql/file_utils/file_to_object.py`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/twarc2sql/file_utils/file_utils.py` & `twarc2sql-1.0.0/twarc2sql/file_utils/file_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,33 @@
 import pandas as pd
 from sqlalchemy.dialects.postgresql import insert
 
 from twarc2sql.db_utils.db_access import create_db_with_tables, get_engine
 
 from . import objects
 from .file_to_object import get_object_for_search
-from .object_to_table import tweet_object, user_object
+from .object_to_table import tweet_object_to_table, user_object_to_table
 
-table_priority = ["meta", "author", "tweet", "media", "places", "polls", "errors"]
+table_priority = [
+    "meta",
+    "author",
+    "tweet",
+    "retweeted_tweet_mapping",
+    "quoted_tweet_mapping",
+    "replied_to_tweet_mapping",
+    "mentions_tweet_mapping",
+    "urls_tweet_mapping",
+    "hashtags_tweet_mapping",
+    "annotations_tweet_mapping",
+    "cashtags_tweet_mapping",
+    "media",
+    "places",
+    "polls",
+    "errors",
+]
 
 
 def upload_to_database(tables: Dict[str, pd.DataFrame], engine: Any) -> None:
     """
     upload_to_database uploads the tables to the database.
 
     Parameters
@@ -26,14 +42,15 @@
     engine : Any
         the engine to connect to the database
     """
     for table in table_priority:
         current_table = tables[table]
         if len(current_table) > 0:
             current_table = pd.concat(current_table)
+            current_table = current_table.drop_duplicates()
             print(f"Uploading {len(current_table)} rows to {table}")
 
             current_table.to_sql(
                 table,
                 engine,
                 if_exists="append",
                 index=False,
@@ -72,29 +89,41 @@
     -------
     Dict[str, Any]
         the objects to uploaded to the database
 
     """
     # read the file in chunks:
     file_path: str = folder_path + file_name
-    chunks = pd.read_json(file_path, lines=True, chunksize=1000)
+    chunksize = 100
+    chunks = pd.read_json(file_path, lines=True, chunksize=chunksize)
 
     task_types = {"search": get_object_for_search}
-    # create empty tables:
-    tables = {table: [] for table in table_priority}
+
+    # Number of lines in the file:
+    num_lines = sum(1 for line in open(file_path))
+    num_chunks = num_lines / chunksize
+    i = 0
 
     for chunk in chunks:
+        print(f"Processing chunk {i} of {num_chunks}")
+        i += 1
+        # create empty tables for each chunk:
+        tables = {table: [] for table in table_priority}
         # get objects from chunk:
-        objects = task_types[task_type](chunk, objects)
+        current_objects = {key: [] for key in objects.keys()}
+        current_objects = task_types[task_type](chunk, current_objects)
         # TODO:Object processing is task specific i.e diff for tasks
         # convert objects to tables:
-        tables = tweet_object(pd.concat(objects["tweets_object"]), tables)
-        tables = user_object(pd.concat(objects["users_object"]), tables)
+        current_objects["tweets_object"] = pd.concat(current_objects["tweets_object"])
+        tables = tweet_object_to_table(current_objects["tweets_object"], tables)
+        current_objects["users_object"] = pd.concat(current_objects["users_object"])
+        tables = user_object_to_table(current_objects["users_object"], tables)
         # upload tables to database:
         upload_to_database(tables, engine)
+
     return tables
 
 
 # TODO: this function should be moved to the db_utils folder
 def on_duplicate_do_nothing(table, conn, keys, data_iter) -> None:
     """on_duplicate_do_nothing uploads data to the database without duplicates.
 
@@ -137,14 +166,13 @@
     file_name : str
         the name of the file
     task_type : str, optional
         the type of task that was run, by default "search"
     """
     try:
         engine = get_engine(config_file_path)
-    # catch exception if database does not exist:
     except Exception as e:
         print(e)
         print("Creating database")
         engine = create_db_with_tables(config_file_path)
     tables = read_and_upload_file(folder_path, file_name, task_type, engine, objects)
     return tables
```

### Comparing `twarc2sql-0.2.2/twarc2sql.egg-info/PKG-INFO` & `twarc2sql-1.0.0/twarc2sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twarc2sql
-Version: 0.2.2
+Version: 1.0.0
 Summary: This package converts jsonl file generated by twarc2 to sql database in an opnionated way.
 Home-page: https://github.com/unna97/twarc2sql
 Author: Unnati Patel
 Author-email: unnati97@gmail.com
 License: MIT license
 Keywords: twarc2sql
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `twarc2sql-0.2.2/twarc2sql.egg-info/SOURCES.txt` & `twarc2sql-1.0.0/twarc2sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twarc2sql-0.2.2/twarc2sql.egg-info/requires.txt` & `twarc2sql-1.0.0/twarc2sql.egg-info/requires.txt`

 * *Files identical despite different names*

