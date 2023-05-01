# Comparing `tmp/pdok-geopackage-validator-0.8.2.tar.gz` & `tmp/pdok-geopackage-validator-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdok-geopackage-validator-0.8.2.tar", last modified: Tue Jan 10 12:52:14 2023, max compression
+gzip compressed data, was "pdok-geopackage-validator-0.8.3.tar", last modified: Thu Feb 23 12:26:58 2023, max compression
```

## Comparing `pdok-geopackage-validator-0.8.2.tar` & `pdok-geopackage-validator-0.8.3.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:52:14.804988 pdok-geopackage-validator-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-01-10 12:52:14.808987 pdok-geopackage-validator-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:52:14.804988 pdok-geopackage-validator-0.8.2/geopackage_validator/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:52:14.804988 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/columnname_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/db_views_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/feature_id_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geom_column_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_ccw_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_dimension_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_valid_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/layerfeature_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/layername_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/name_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/rtree_present_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/rtree_valid_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/srs_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/table_definitions_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/geopackage_validator/validations/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:52:14.804988 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-01-10 12:52:14.000000 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-10 12:52:14.000000 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 12:52:14.000000 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-10 12:52:14.000000 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-10 12:52:14.000000 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-10 12:52:14.000000 pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-10 12:52:14.808987 pdok-geopackage-validator-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-10 12:52:03.000000 pdok-geopackage-validator-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.798764 pdok-geopackage-validator-0.8.3/geopackage_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.798764 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/columnname_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/db_views_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/feature_id_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geom_column_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_ccw_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_dimension_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_valid_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layerfeature_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layername_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/name_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_present_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_valid_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/srs_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/table_definitions_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/geopackage_validator/validations/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 12:26:58.000000 pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:26:58.802764 pdok-geopackage-validator-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-23 12:26:45.000000 pdok-geopackage-validator-0.8.3/tests/test_validate.py
```

### Comparing `pdok-geopackage-validator-0.8.2/CHANGES.md` & `pdok-geopackage-validator-0.8.3/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/LICENSE` & `pdok-geopackage-validator-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/PKG-INFO` & `pdok-geopackage-validator-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdok-geopackage-validator
-Version: 0.8.2
+Version: 0.8.3
 Summary: Validate Geopackage files according to PDOK requirements and recommendations
 License: MIT
 Keywords: geopackage-validator,geopackage,pdok
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pdok-geopackage-validator-0.8.2/README.md` & `pdok-geopackage-validator-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/cli.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/cli.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/generate.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/generate.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/output.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/output.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/s3.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/s3.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/utils.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/utils.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validate.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validate.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/__init__.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/columnname_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/columnname_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/db_views_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/db_views_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/feature_id_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/feature_id_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geom_column_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geom_column_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_ccw_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_ccw_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_dimension_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_dimension_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_type_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_type_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/geometry_valid_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/geometry_valid_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/layerfeature_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layerfeature_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/layername_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/layername_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/name_length_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/name_length_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/rtree_present_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_present_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/rtree_valid_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/rtree_valid_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/srs_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/srs_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/table_definitions_check.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/table_definitions_check.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/geopackage_validator/validations/validator.py` & `pdok-geopackage-validator-0.8.3/geopackage_validator/validations/validator.py`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/PKG-INFO` & `pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdok-geopackage-validator
-Version: 0.8.2
+Version: 0.8.3
 Summary: Validate Geopackage files according to PDOK requirements and recommendations
 License: MIT
 Keywords: geopackage-validator,geopackage,pdok
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pdok-geopackage-validator-0.8.2/pdok_geopackage_validator.egg-info/SOURCES.txt` & `pdok-geopackage-validator-0.8.3/pdok_geopackage_validator.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -31,8 +31,11 @@
 geopackage_validator/validations/table_definitions_check.py
 geopackage_validator/validations/validator.py
 pdok_geopackage_validator.egg-info/PKG-INFO
 pdok_geopackage_validator.egg-info/SOURCES.txt
 pdok_geopackage_validator.egg-info/dependency_links.txt
 pdok_geopackage_validator.egg-info/entry_points.txt
 pdok_geopackage_validator.egg-info/requires.txt
-pdok_geopackage_validator.egg-info/top_level.txt
+pdok_geopackage_validator.egg-info/top_level.txt
+tests/test_cli.py
+tests/test_utils.py
+tests/test_validate.py
```

### Comparing `pdok-geopackage-validator-0.8.2/pyproject.toml` & `pdok-geopackage-validator-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdok-geopackage-validator-0.8.2/setup.cfg` & `pdok-geopackage-validator-0.8.3/setup.cfg`

 * *Files identical despite different names*

