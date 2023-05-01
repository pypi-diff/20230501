# Comparing `tmp/openedx-ledger-0.3.2.tar.gz` & `tmp/openedx-ledger-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-0.3.2.tar", last modified: Wed Apr 26 20:38:40 2023, max compression
+gzip compressed data, was "openedx-ledger-0.3.3.tar", last modified: Mon May  1 14:15:33 2023, max compression
```

## Comparing `openedx-ledger-0.3.2.tar` & `openedx-ledger-0.3.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15474 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.230926 openedx-ledger-0.3.2/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8484 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.598944 openedx-ledger-0.3.3/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15389 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.598944 openedx-ledger-0.3.3/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.598944 openedx-ledger-0.3.3/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8484 2023-05-01 14:15:33.000000 openedx-ledger-0.3.3/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-01 14:15:33.000000 openedx-ledger-0.3.3/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 14:15:33.000000 openedx-ledger-0.3.3/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 14:15:33.000000 openedx-ledger-0.3.3/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-01 14:15:33.000000 openedx-ledger-0.3.3/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-01 14:15:33.000000 openedx-ledger-0.3.3/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:15:33.602944 openedx-ledger-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-05-01 14:15:29.000000 openedx-ledger-0.3.3/tests/test_models.py
```

### Comparing `openedx-ledger-0.3.2/CHANGELOG.rst` & `openedx-ledger-0.3.3/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+
+[0.3.3]
+*******
+* drop `ExternalFulfillmentProvider` name constraints
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
   more details.
-  
+
 [0.2.2]
 *******
 * Add many help_text fields to model fields.
 * Add some useful composite table indices.
 * Add a "failed" transaction state.
 
 [0.2.0]
```

### Comparing `openedx-ledger-0.3.2/LICENSE.txt` & `openedx-ledger-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/PKG-INFO` & `openedx-ledger-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.3.2
+Version: 0.3.3
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -205,18 +205,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+
+[0.3.3]
+*******
+* drop `ExternalFulfillmentProvider` name constraints
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
   more details.
-  
+
 [0.2.2]
 *******
 * Add many help_text fields to model fields.
 * Add some useful composite table indices.
 * Add a "failed" transaction state.
 
 [0.2.0]
```

### Comparing `openedx-ledger-0.3.2/README.rst` & `openedx-ledger-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/admin.py` & `openedx-ledger-0.3.3/openedx_ledger/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/api.py` & `openedx-ledger-0.3.3/openedx_ledger/api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-0.3.3/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-0.3.3/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-0.3.3/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-0.3.3/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-0.3.3/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-0.3.3/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/models.py` & `openedx-ledger-0.3.3/openedx_ledger/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,18 +358,14 @@
         """
 
         verbose_name = 'External Fulfillment provider'
         verbose_name_plural = 'External fulfillment providers'
 
     name = models.CharField(
         max_length=255,
-        blank=False,
-        null=False,
-        unique=True,
-        db_index=True,
         help_text="The name of the external reference type.",
     )
     slug = models.SlugField(
         max_length=32,
         unique=True,
         help_text=(
             "The slug of the external reference type. This is typically the slugified name of the system that the "
```

### Comparing `openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html` & `openedx-ledger-0.3.3/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-0.3.3/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/test_utils/factories.py` & `openedx-ledger-0.3.3/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/utils.py` & `openedx-ledger-0.3.3/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger/views.py` & `openedx-ledger-0.3.3/openedx_ledger/views.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-0.3.3/openedx_ledger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.3.2
+Version: 0.3.3
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -205,18 +205,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+
+[0.3.3]
+*******
+* drop `ExternalFulfillmentProvider` name constraints
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
   more details.
-  
+
 [0.2.2]
 *******
 * Add many help_text fields to model fields.
 * Add some useful composite table indices.
 * Add a "failed" transaction state.
 
 [0.2.0]
```

### Comparing `openedx-ledger-0.3.2/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-0.3.3/openedx_ledger.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 openedx_ledger.egg-info/top_level.txt
 openedx_ledger/migrations/0001_initial.py
 openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
 openedx_ledger/migrations/0003_field_updates_20230216_1605.py
 openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
 openedx_ledger/migrations/0005_help_text_and_more_indices.py
 openedx_ledger/migrations/0006_auto_20230404_1744.py
+openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
 openedx_ledger/migrations/__init__.py
 openedx_ledger/signals/__init__.py
 openedx_ledger/signals/signals.py
 openedx_ledger/templates/edx_ledger/base.html
 openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
 openedx_ledger/test_utils/__init__.py
 openedx_ledger/test_utils/factories.py
```

### Comparing `openedx-ledger-0.3.2/requirements/constraints.txt` & `openedx-ledger-0.3.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/setup.py` & `openedx-ledger-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/tests/test_api.py` & `openedx-ledger-0.3.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.2/tests/test_models.py` & `openedx-ledger-0.3.3/tests/test_models.py`

 * *Files identical despite different names*

