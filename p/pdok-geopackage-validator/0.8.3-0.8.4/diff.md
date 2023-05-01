# Comparing `tmp/pdok-geopackage-validator-0.8.3.tar.gz` & `tmp/pdok-geopackage-validator-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdok-geopackage-validator-0.8.3.tar", last modified: Thu Feb 23 12:26:58 2023, max compression
+gzip compressed data, was "pdok-geopackage-validator-0.8.4.tar", last modified: Mon May  1 13:57:32 2023, max compression
```

## Comparing `pdok-geopackage-validator-0.8.3.tar` & `pdok-geopackage-validator-0.8.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.798764 pdok-geopackage-validator-0.8.3/geopackage_validator/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.798764 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/columnname_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/db_views_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/feature_id_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geom_column_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_ccw_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_dimension_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_valid_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layerfeature_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layername_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/name_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_present_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_valid_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/srs_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/table_definitions_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:57:32.637278 pdok-geopackage-validator-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-05-01 13:57:32.637278 pdok-geopackage-validator-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21581 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:57:32.633278 pdok-geopackage-validator-0.8.4/geopackage_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 13:57:22.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:57:32.633278 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/columnname_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/db_views_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/feature_id_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geom_column_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_ccw_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_dimension_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_valid_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/layerfeature_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/layername_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/name_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/rtree_present_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/rtree_valid_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/srs_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/table_definitions_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/geopackage_validator/validations/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:57:32.633278 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-05-01 13:57:32.000000 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-01 13:57:32.000000 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:57:32.000000 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 13:57:32.000000 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 13:57:32.000000 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 13:57:32.000000 pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 13:57:32.637278 pdok-geopackage-validator-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:57:32.637278 pdok-geopackage-validator-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-01 13:57:21.000000 pdok-geopackage-validator-0.8.4/tests/test_validate.py
```

### Comparing `pdok-geopackage-validator-0.8.3/CHANGES.md` & `pdok-geopackage-validator-0.8.4/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/LICENSE` & `pdok-geopackage-validator-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/PKG-INFO` & `pdok-geopackage-validator-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 Metadata-Version: 2.1
 Name: pdok-geopackage-validator
-Version: 0.8.3
+Version: 0.8.4
 Summary: Validate Geopackage files according to PDOK requirements and recommendations
 License: MIT
 Keywords: geopackage-validator,geopackage,pdok
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# geopackage-validator
+# PDOK geopackage-validator
 
 [![Tests](https://github.com/pdok/geopackage-validator/actions/workflows/pytest.yml/badge.svg)](https://github.com/pdok/geopackage-validator/actions/workflows/pytest.yml)[![PyPI version](https://badge.fury.io/py/pdok-geopackage-validator.svg)](https://pypi.org/project/pdok-geopackage-validator/)
 
+Geopackages are a data format that have a deliberately broad application, so many of the requirements are dependend on your use.
+
+The PDOK geopackage validator is used by [PDOK](https://www.pdok.nl/). PDOK is part of the Dutch government. This geopackage validator is used to validate a [set of requirements](#what-does-it-do) to make sure geopackages adhere to our standardized ETL pipeline. It is possible to use this for your own purposes as described [here](https://github.com/PDOK/geopackage-validator/issues/115#issuecomment-1529488733). The validations will not change (except for bugfixes); **new validations are always added to the list**. 
+
+
 ## Table of Contents
 
 - [geopackage-validator](#geopackage-validator)
   - [Table of Contents](#table-of-contents)
   - [What does it do](#what-does-it-do)
   - [Geopackage versions](#geopackage-versions)
   - [Installation](#installation)
-    - [Docker](#docker)
+    - [Docker](#docker-installation)
   - [Usage](#usage)
-    - [RQ8 Validation](#rq8-validation)
-    - [Show validations](#show-validations)
-    - [Generate table definitions](#generate-table-definitions)
+    - [RQ8 Validation](#local-rq8-validation)
+    - [Show validations](#local-show-validations)
+    - [Generate table definitions](#local-generate-table-definitions)
   - [Local development](#local-development)
     - [Usage](#usage-1)
     - [Python console](#python-console)
     - [Code style](#code-style)
     - [Tests](#tests)
     - [Releasing](#releasing)
 
 ## TL;DR Commands
 
+Either run through [docker](#docker) or [locally](#local). 
+
+### Docker
 Validate a GeoPackage with the default set of validation rules:
 
 ```sh
 gpkg_path=relative/path/to/the.gpkg
 docker run -v "$(pwd)":/gpkg --rm pdok/geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" 
 ```
 
@@ -59,14 +67,39 @@
 
 ```sh
 schema_path=relative/path/to/the/schema.json
 gpkg_path=relative/path/to/the.gpkg
 docker run -v "$(pwd)":/gpkg --rm pdok/geopackage-validator generate-definitions --gpkg-path "/gpkg/${gpkg_path}" > "$schema_path" 
 ```
 
+### Local
+
+For a local setup we require/tested against python > 3.6 and gdal = 3.4.
+
+```sh
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" 
+```
+
+Validate a GeoPackage with the default set of validation rules including a schema:
+
+```sh
+schema_path=relative/path/to/the/schema.json
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" --table-definitions-path "/gpkg/${schema_path}" 
+```
+
+Generate a schema: 
+
+```sh
+schema_path=relative/path/to/the/schema.json
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator generate-definitions --gpkg-path "/gpkg/${gpkg_path}" > "$schema_path" 
+```
+
 ## What does it do
 
 The Geopackage validator can validate .gkpg files to see if they conform to a set of standards.
 The current checks are (see also the 'show-validations' command):
 
 | Validation code** | Description                                                                                                                                                                                         |
 |:-----------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
@@ -111,15 +144,15 @@
 This package requires:
 - [GDAL](https://gdal.org/) version >= 3.2.1.
 - [Spatialite](https://www.gaia-gis.it/fossil/libspatialite/index) version >= 5.0.0
 - And python >= 3.8 to run.
 
 We recommend using the docker image. When above requirements are met the package can be installed using pip (`pip install pdok-geopackage-validator`).  
 
-### Docker
+### Docker Installation
 
 Pull the latest version of the Docker image (only once needed, or after an update)
 
 ```bash
 docker pull pdok/geopackage-validator:latest
 ```
 
@@ -415,8 +448,8 @@
 
 ```bash
 docker-compose run --rm validator pytest
 ```
 
 ### Releasing
 
-Release in github by bumping the `__version__` in [`geopackage_validator.constants.py`](geopackage_validator/constants.py) and by creating and pushing a new tag to master and create a new release in github.  
+Release in github by creating a new release in github.
```

### Comparing `pdok-geopackage-validator-0.8.3/README.md` & `pdok-geopackage-validator-0.8.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-# geopackage-validator
+# PDOK geopackage-validator
 
 [![Tests](https://github.com/pdok/geopackage-validator/actions/workflows/pytest.yml/badge.svg)](https://github.com/pdok/geopackage-validator/actions/workflows/pytest.yml)[![PyPI version](https://badge.fury.io/py/pdok-geopackage-validator.svg)](https://pypi.org/project/pdok-geopackage-validator/)
 
+Geopackages are a data format that have a deliberately broad application, so many of the requirements are dependend on your use.
+
+The PDOK geopackage validator is used by [PDOK](https://www.pdok.nl/). PDOK is part of the Dutch government. This geopackage validator is used to validate a [set of requirements](#what-does-it-do) to make sure geopackages adhere to our standardized ETL pipeline. It is possible to use this for your own purposes as described [here](https://github.com/PDOK/geopackage-validator/issues/115#issuecomment-1529488733). The validations will not change (except for bugfixes); **new validations are always added to the list**. 
+
+
 ## Table of Contents
 
 - [geopackage-validator](#geopackage-validator)
   - [Table of Contents](#table-of-contents)
   - [What does it do](#what-does-it-do)
   - [Geopackage versions](#geopackage-versions)
   - [Installation](#installation)
-    - [Docker](#docker)
+    - [Docker](#docker-installation)
   - [Usage](#usage)
-    - [RQ8 Validation](#rq8-validation)
-    - [Show validations](#show-validations)
-    - [Generate table definitions](#generate-table-definitions)
+    - [RQ8 Validation](#local-rq8-validation)
+    - [Show validations](#local-show-validations)
+    - [Generate table definitions](#local-generate-table-definitions)
   - [Local development](#local-development)
     - [Usage](#usage-1)
     - [Python console](#python-console)
     - [Code style](#code-style)
     - [Tests](#tests)
     - [Releasing](#releasing)
 
 ## TL;DR Commands
 
+Either run through [docker](#docker) or [locally](#local). 
+
+### Docker
 Validate a GeoPackage with the default set of validation rules:
 
 ```sh
 gpkg_path=relative/path/to/the.gpkg
 docker run -v "$(pwd)":/gpkg --rm pdok/geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" 
 ```
 
@@ -42,14 +50,39 @@
 
 ```sh
 schema_path=relative/path/to/the/schema.json
 gpkg_path=relative/path/to/the.gpkg
 docker run -v "$(pwd)":/gpkg --rm pdok/geopackage-validator generate-definitions --gpkg-path "/gpkg/${gpkg_path}" > "$schema_path" 
 ```
 
+### Local
+
+For a local setup we require/tested against python > 3.6 and gdal = 3.4.
+
+```sh
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" 
+```
+
+Validate a GeoPackage with the default set of validation rules including a schema:
+
+```sh
+schema_path=relative/path/to/the/schema.json
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" --table-definitions-path "/gpkg/${schema_path}" 
+```
+
+Generate a schema: 
+
+```sh
+schema_path=relative/path/to/the/schema.json
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator generate-definitions --gpkg-path "/gpkg/${gpkg_path}" > "$schema_path" 
+```
+
 ## What does it do
 
 The Geopackage validator can validate .gkpg files to see if they conform to a set of standards.
 The current checks are (see also the 'show-validations' command):
 
 | Validation code** | Description                                                                                                                                                                                         |
 |:-----------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
@@ -94,15 +127,15 @@
 This package requires:
 - [GDAL](https://gdal.org/) version >= 3.2.1.
 - [Spatialite](https://www.gaia-gis.it/fossil/libspatialite/index) version >= 5.0.0
 - And python >= 3.8 to run.
 
 We recommend using the docker image. When above requirements are met the package can be installed using pip (`pip install pdok-geopackage-validator`).  
 
-### Docker
+### Docker Installation
 
 Pull the latest version of the Docker image (only once needed, or after an update)
 
 ```bash
 docker pull pdok/geopackage-validator:latest
 ```
 
@@ -398,8 +431,8 @@
 
 ```bash
 docker-compose run --rm validator pytest
 ```
 
 ### Releasing
 
-Release in github by bumping the `__version__` in [`geopackage_validator.constants.py`](geopackage_validator/constants.py) and by creating and pushing a new tag to master and create a new release in github.  
+Release in github by creating a new release in github.
```

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/cli.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/cli.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/generate.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/generate.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/output.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/output.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/s3.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/s3.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/utils.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/utils.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validate.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validate.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/__init__.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/columnname_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/columnname_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/db_views_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/db_views_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/feature_id_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/feature_id_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geom_column_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geom_column_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_ccw_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_ccw_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_dimension_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_dimension_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_type_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_type_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_valid_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/geometry_valid_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layerfeature_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/layerfeature_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layername_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/layername_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/name_length_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/name_length_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_present_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/rtree_present_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_valid_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/rtree_valid_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/srs_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/srs_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/table_definitions_check.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/table_definitions_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/validator.py` & `pdok-geopackage-validator-0.8.4/geopackage_validator/validations/validator.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/PKG-INFO` & `pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 Metadata-Version: 2.1
 Name: pdok-geopackage-validator
-Version: 0.8.3
+Version: 0.8.4
 Summary: Validate Geopackage files according to PDOK requirements and recommendations
 License: MIT
 Keywords: geopackage-validator,geopackage,pdok
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# geopackage-validator
+# PDOK geopackage-validator
 
 [![Tests](https://github.com/pdok/geopackage-validator/actions/workflows/pytest.yml/badge.svg)](https://github.com/pdok/geopackage-validator/actions/workflows/pytest.yml)[![PyPI version](https://badge.fury.io/py/pdok-geopackage-validator.svg)](https://pypi.org/project/pdok-geopackage-validator/)
 
+Geopackages are a data format that have a deliberately broad application, so many of the requirements are dependend on your use.
+
+The PDOK geopackage validator is used by [PDOK](https://www.pdok.nl/). PDOK is part of the Dutch government. This geopackage validator is used to validate a [set of requirements](#what-does-it-do) to make sure geopackages adhere to our standardized ETL pipeline. It is possible to use this for your own purposes as described [here](https://github.com/PDOK/geopackage-validator/issues/115#issuecomment-1529488733). The validations will not change (except for bugfixes); **new validations are always added to the list**. 
+
+
 ## Table of Contents
 
 - [geopackage-validator](#geopackage-validator)
   - [Table of Contents](#table-of-contents)
   - [What does it do](#what-does-it-do)
   - [Geopackage versions](#geopackage-versions)
   - [Installation](#installation)
-    - [Docker](#docker)
+    - [Docker](#docker-installation)
   - [Usage](#usage)
-    - [RQ8 Validation](#rq8-validation)
-    - [Show validations](#show-validations)
-    - [Generate table definitions](#generate-table-definitions)
+    - [RQ8 Validation](#local-rq8-validation)
+    - [Show validations](#local-show-validations)
+    - [Generate table definitions](#local-generate-table-definitions)
   - [Local development](#local-development)
     - [Usage](#usage-1)
     - [Python console](#python-console)
     - [Code style](#code-style)
     - [Tests](#tests)
     - [Releasing](#releasing)
 
 ## TL;DR Commands
 
+Either run through [docker](#docker) or [locally](#local). 
+
+### Docker
 Validate a GeoPackage with the default set of validation rules:
 
 ```sh
 gpkg_path=relative/path/to/the.gpkg
 docker run -v "$(pwd)":/gpkg --rm pdok/geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" 
 ```
 
@@ -59,14 +67,39 @@
 
 ```sh
 schema_path=relative/path/to/the/schema.json
 gpkg_path=relative/path/to/the.gpkg
 docker run -v "$(pwd)":/gpkg --rm pdok/geopackage-validator generate-definitions --gpkg-path "/gpkg/${gpkg_path}" > "$schema_path" 
 ```
 
+### Local
+
+For a local setup we require/tested against python > 3.6 and gdal = 3.4.
+
+```sh
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" 
+```
+
+Validate a GeoPackage with the default set of validation rules including a schema:
+
+```sh
+schema_path=relative/path/to/the/schema.json
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator validate --gpkg-path "/gpkg/${gpkg_path}" --table-definitions-path "/gpkg/${schema_path}" 
+```
+
+Generate a schema: 
+
+```sh
+schema_path=relative/path/to/the/schema.json
+gpkg_path=relative/path/to/the.gpkg
+geopackage-validator generate-definitions --gpkg-path "/gpkg/${gpkg_path}" > "$schema_path" 
+```
+
 ## What does it do
 
 The Geopackage validator can validate .gkpg files to see if they conform to a set of standards.
 The current checks are (see also the 'show-validations' command):
 
 | Validation code** | Description                                                                                                                                                                                         |
 |:-----------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
@@ -111,15 +144,15 @@
 This package requires:
 - [GDAL](https://gdal.org/) version >= 3.2.1.
 - [Spatialite](https://www.gaia-gis.it/fossil/libspatialite/index) version >= 5.0.0
 - And python >= 3.8 to run.
 
 We recommend using the docker image. When above requirements are met the package can be installed using pip (`pip install pdok-geopackage-validator`).  
 
-### Docker
+### Docker Installation
 
 Pull the latest version of the Docker image (only once needed, or after an update)
 
 ```bash
 docker pull pdok/geopackage-validator:latest
 ```
 
@@ -415,8 +448,8 @@
 
 ```bash
 docker-compose run --rm validator pytest
 ```
 
 ### Releasing
 
-Release in github by bumping the `__version__` in [`geopackage_validator.constants.py`](geopackage_validator/constants.py) and by creating and pushing a new tag to master and create a new release in github.  
+Release in github by creating a new release in github.
```

### Comparing `pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/SOURCES.txt` & `pdok-geopackage-validator-0.8.4/pdok_geopackage_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/pyproject.toml` & `pdok-geopackage-validator-0.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 dynamic = ["version", "readme", "requires-python"]
 
 [project.scripts]
 geopackage-validator = "geopackage_validator.cli:cli"
 
 [tool.setuptools.dynamic]
-version = {attr = "geopackage_validator.constants.__version__"}
+version = {attr = "geopackage_validator.__version__"}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [tool.setuptools.packages.find]
 include = ["geopackage_validator*"]  # package names should match these glob patterns (["*"] by default)
 exclude = ["tests*"]  # exclude packages matching these glob patterns (empty by default)
 
 [tool.pytest.ini_options]
```

### Comparing `pdok-geopackage-validator-0.8.3/setup.cfg` & `pdok-geopackage-validator-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/tests/test_cli.py` & `pdok-geopackage-validator-0.8.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/tests/test_utils.py` & `pdok-geopackage-validator-0.8.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.3/tests/test_validate.py` & `pdok-geopackage-validator-0.8.4/tests/test_validate.py`

 * *Files identical despite different names*

