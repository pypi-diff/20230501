# Comparing `tmp/nocasedict-2.0.0.tar.gz` & `tmp/nocasedict-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nocasedict-2.0.0.tar", last modified: Sun Feb 26 07:18:58 2023, max compression
+gzip compressed data, was "nocasedict-2.0.1.tar", last modified: Mon May  1 07:11:19 2023, max compression
```

## Comparing `nocasedict-2.0.0.tar` & `nocasedict-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.560507 nocasedict-2.0.0/
--rw-r--r--   0 maiera     (501) staff       (20)      424 2023-02-25 11:05:20.000000 nocasedict-2.0.0/INSTALL.md
--rw-r--r--   0 maiera     (501) staff       (20)    26526 2023-02-25 11:05:20.000000 nocasedict-2.0.0/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      263 2023-02-26 07:18:58.000000 nocasedict-2.0.0/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     5596 2023-02-26 07:18:58.560026 nocasedict-2.0.0/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     4256 2023-02-26 06:22:27.000000 nocasedict-2.0.0/README.rst
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.546461 nocasedict-2.0.0/nocasedict/
--rw-r--r--   0 maiera     (501) staff       (20)      294 2023-02-25 11:05:20.000000 nocasedict-2.0.0/nocasedict/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     2151 2023-02-26 06:22:27.000000 nocasedict-2.0.0/nocasedict/_hashable.py
--rw-r--r--   0 maiera     (501) staff       (20)     1470 2023-02-26 06:22:27.000000 nocasedict-2.0.0/nocasedict/_keyableby.py
--rw-r--r--   0 maiera     (501) staff       (20)    27740 2023-02-26 06:22:27.000000 nocasedict-2.0.0/nocasedict/_nocasedict.py
--rw-r--r--   0 maiera     (501) staff       (20)     1141 2023-02-26 06:22:27.000000 nocasedict-2.0.0/nocasedict/_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)      326 2023-02-26 07:15:01.000000 nocasedict-2.0.0/nocasedict/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)        0 2023-02-26 06:22:27.000000 nocasedict-2.0.0/nocasedict/py.typed
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.549821 nocasedict-2.0.0/nocasedict.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     5596 2023-02-26 07:18:58.000000 nocasedict-2.0.0/nocasedict.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)      754 2023-02-26 07:18:58.000000 nocasedict-2.0.0/nocasedict.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-02-26 07:18:58.000000 nocasedict-2.0.0/nocasedict.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)       84 2023-02-26 07:18:58.000000 nocasedict-2.0.0/nocasedict.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       11 2023-02-26 07:18:58.000000 nocasedict-2.0.0/nocasedict.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-02-26 07:18:58.000000 nocasedict-2.0.0/nocasedict.egg-info/zip-safe
--rw-r--r--   0 maiera     (501) staff       (20)      506 2023-02-26 06:22:27.000000 nocasedict-2.0.0/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2023-02-26 07:18:58.560656 nocasedict-2.0.0/setup.cfg
--rwxr-xr-x   0 maiera     (501) staff       (20)     6663 2023-02-26 06:22:27.000000 nocasedict-2.0.0/setup.py
--rw-r--r--   0 maiera     (501) staff       (20)     1070 2023-02-26 06:22:27.000000 nocasedict-2.0.0/test-requirements.txt
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.550737 nocasedict-2.0.0/tests/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.0/tests/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.551168 nocasedict-2.0.0/tests/installtest/
--rwxr-xr-x   0 maiera     (501) staff       (20)    12821 2023-02-25 11:05:21.000000 nocasedict-2.0.0/tests/installtest/test_install.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.557392 nocasedict-2.0.0/tests/unittest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.0/tests/unittest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     9210 2023-02-26 06:22:27.000000 nocasedict-2.0.0/tests/unittest/test_hashable.py
--rw-r--r--   0 maiera     (501) staff       (20)     4067 2023-02-26 06:22:27.000000 nocasedict-2.0.0/tests/unittest/test_keyableby.py
--rwxr-xr-x   0 maiera     (501) staff       (20)    90763 2023-02-26 06:22:27.000000 nocasedict-2.0.0/tests/unittest/test_nocasedict.py
--rw-r--r--   0 maiera     (501) staff       (20)      401 2023-02-25 11:05:21.000000 nocasedict-2.0.0/tests/unittest/test_package.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 07:18:58.559120 nocasedict-2.0.0/tests/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.0/tests/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3444 2023-02-25 11:05:21.000000 nocasedict-2.0.0/tests/utils/import_installed.py
--rw-r--r--   0 maiera     (501) staff       (20)     7138 2023-02-26 06:22:27.000000 nocasedict-2.0.0/tests/utils/simplified_test_function.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.464289 nocasedict-2.0.1/
+-rw-r--r--   0 maiera     (501) staff       (20)      424 2023-04-30 18:32:10.000000 nocasedict-2.0.1/INSTALL.md
+-rw-r--r--   0 maiera     (501) staff       (20)    26526 2023-04-30 18:32:10.000000 nocasedict-2.0.1/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      263 2023-05-01 07:11:18.000000 nocasedict-2.0.1/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)     5596 2023-05-01 07:11:19.463941 nocasedict-2.0.1/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     4256 2023-05-01 07:11:07.000000 nocasedict-2.0.1/README.rst
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.455568 nocasedict-2.0.1/nocasedict/
+-rw-r--r--   0 maiera     (501) staff       (20)      294 2023-04-30 18:32:10.000000 nocasedict-2.0.1/nocasedict/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2151 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_hashable.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1470 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_keyableby.py
+-rw-r--r--   0 maiera     (501) staff       (20)    27740 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_nocasedict.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1141 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)      326 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:07.000000 nocasedict-2.0.1/nocasedict/py.typed
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.458410 nocasedict-2.0.1/nocasedict.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)     5596 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)      754 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       84 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       11 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2023-05-01 07:11:19.000000 nocasedict-2.0.1/nocasedict.egg-info/zip-safe
+-rw-r--r--   0 maiera     (501) staff       (20)      506 2023-05-01 07:11:07.000000 nocasedict-2.0.1/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2023-05-01 07:11:19.464421 nocasedict-2.0.1/setup.cfg
+-rwxr-xr-x   0 maiera     (501) staff       (20)     6663 2023-05-01 07:11:07.000000 nocasedict-2.0.1/setup.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1070 2023-05-01 07:11:07.000000 nocasedict-2.0.1/test-requirements.txt
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.458957 nocasedict-2.0.1/tests/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.1/tests/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.459352 nocasedict-2.0.1/tests/installtest/
+-rwxr-xr-x   0 maiera     (501) staff       (20)    12821 2023-04-30 18:32:10.000000 nocasedict-2.0.1/tests/installtest/test_install.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.462124 nocasedict-2.0.1/tests/unittest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.1/tests/unittest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     9210 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/unittest/test_hashable.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4067 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/unittest/test_keyableby.py
+-rwxr-xr-x   0 maiera     (501) staff       (20)    90763 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/unittest/test_nocasedict.py
+-rw-r--r--   0 maiera     (501) staff       (20)      401 2023-04-30 18:32:10.000000 nocasedict-2.0.1/tests/unittest/test_package.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-05-01 07:11:19.463503 nocasedict-2.0.1/tests/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 05:09:05.000000 nocasedict-2.0.1/tests/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3444 2023-04-30 18:32:10.000000 nocasedict-2.0.1/tests/utils/import_installed.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7138 2023-05-01 07:11:07.000000 nocasedict-2.0.1/tests/utils/simplified_test_function.py
```

### Comparing `nocasedict-2.0.0/LICENSE` & `nocasedict-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/PKG-INFO` & `nocasedict-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocasedict
-Version: 2.0.0
+Version: 2.0.1
 Summary: A case-insensitive ordered dictionary for Python
 Home-page: https://github.com/pywbem/nocasedict
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `nocasedict-2.0.0/README.rst` & `nocasedict-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/nocasedict/_hashable.py` & `nocasedict-2.0.1/nocasedict/_hashable.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/nocasedict/_keyableby.py` & `nocasedict-2.0.1/nocasedict/_keyableby.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/nocasedict/_nocasedict.py` & `nocasedict-2.0.1/nocasedict/_nocasedict.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/nocasedict/_utils.py` & `nocasedict-2.0.1/nocasedict/_utils.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/nocasedict.egg-info/PKG-INFO` & `nocasedict-2.0.1/nocasedict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocasedict
-Version: 2.0.0
+Version: 2.0.1
 Summary: A case-insensitive ordered dictionary for Python
 Home-page: https://github.com/pywbem/nocasedict
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `nocasedict-2.0.0/nocasedict.egg-info/SOURCES.txt` & `nocasedict-2.0.1/nocasedict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/setup.py` & `nocasedict-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/test-requirements.txt` & `nocasedict-2.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/tests/installtest/test_install.sh` & `nocasedict-2.0.1/tests/installtest/test_install.sh`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/tests/unittest/test_hashable.py` & `nocasedict-2.0.1/tests/unittest/test_hashable.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/tests/unittest/test_keyableby.py` & `nocasedict-2.0.1/tests/unittest/test_keyableby.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/tests/unittest/test_nocasedict.py` & `nocasedict-2.0.1/tests/unittest/test_nocasedict.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/tests/utils/import_installed.py` & `nocasedict-2.0.1/tests/utils/import_installed.py`

 * *Files identical despite different names*

### Comparing `nocasedict-2.0.0/tests/utils/simplified_test_function.py` & `nocasedict-2.0.1/tests/utils/simplified_test_function.py`

 * *Files identical despite different names*

