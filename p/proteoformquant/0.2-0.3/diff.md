# Comparing `tmp/proteoformquant-0.2.tar.gz` & `tmp/proteoformquant-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteoformquant-0.2.tar", last modified: Mon May  1 09:01:43 2023, max compression
+gzip compressed data, was "proteoformquant-0.3.tar", last modified: Mon May  1 09:01:50 2023, max compression
```

## Comparing `proteoformquant-0.2.tar` & `proteoformquant-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-05-01 09:01:43.884396 proteoformquant-0.2/
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        0 2023-03-17 14:28:03.000000 proteoformquant-0.2/MANIFEST.in
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1711 2023-05-01 09:01:43.884396 proteoformquant-0.2/PKG-INFO
-drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-05-01 09:01:43.884396 proteoformquant-0.2/proteoformquant.egg-info/
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1711 2023-05-01 09:01:43.000000 proteoformquant-0.2/proteoformquant.egg-info/PKG-INFO
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1070 2023-05-01 09:01:43.000000 proteoformquant-0.2/proteoformquant.egg-info/SOURCES.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        1 2023-05-01 09:01:43.000000 proteoformquant-0.2/proteoformquant.egg-info/dependency_links.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       57 2023-05-01 09:01:43.000000 proteoformquant-0.2/proteoformquant.egg-info/entry_points.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)      349 2023-05-01 09:01:43.000000 proteoformquant-0.2/proteoformquant.egg-info/requires.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       16 2023-05-01 09:01:43.000000 proteoformquant-0.2/proteoformquant.egg-info/top_level.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       38 2023-05-01 09:01:43.884396 proteoformquant-0.2/setup.cfg
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     3372 2023-03-20 10:27:03.000000 proteoformquant-0.2/setup.py
+drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-05-01 09:01:50.880375 proteoformquant-0.3/
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        0 2023-03-17 14:28:03.000000 proteoformquant-0.3/MANIFEST.in
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1711 2023-05-01 09:01:50.880375 proteoformquant-0.3/PKG-INFO
+drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-05-01 09:01:50.880375 proteoformquant-0.3/proteoformquant.egg-info/
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1711 2023-05-01 09:01:50.000000 proteoformquant-0.3/proteoformquant.egg-info/PKG-INFO
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1070 2023-05-01 09:01:50.000000 proteoformquant-0.3/proteoformquant.egg-info/SOURCES.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        1 2023-05-01 09:01:50.000000 proteoformquant-0.3/proteoformquant.egg-info/dependency_links.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       57 2023-05-01 09:01:50.000000 proteoformquant-0.3/proteoformquant.egg-info/entry_points.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)      349 2023-05-01 09:01:50.000000 proteoformquant-0.3/proteoformquant.egg-info/requires.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       16 2023-05-01 09:01:50.000000 proteoformquant-0.3/proteoformquant.egg-info/top_level.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       38 2023-05-01 09:01:50.884375 proteoformquant-0.3/setup.cfg
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     3372 2023-03-20 10:27:03.000000 proteoformquant-0.3/setup.py
```

### Comparing `proteoformquant-0.2/PKG-INFO` & `proteoformquant-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteoformquant
-Version: 0.2
+Version: 0.3
 Summary: A python command line tool for the quantification of peptidoform/proteoforms
 Home-page: 
 Author: Arthur Grimaud
 Author-email: arthur582@hotmail.fr
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `proteoformquant-0.2/proteoformquant.egg-info/PKG-INFO` & `proteoformquant-0.3/proteoformquant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteoformquant
-Version: 0.2
+Version: 0.3
 Summary: A python command line tool for the quantification of peptidoform/proteoforms
 Home-page: 
 Author: Arthur Grimaud
 Author-email: arthur582@hotmail.fr
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `proteoformquant-0.2/proteoformquant.egg-info/SOURCES.txt` & `proteoformquant-0.3/proteoformquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteoformquant-0.2/setup.py` & `proteoformquant-0.3/setup.py`

 * *Files identical despite different names*

