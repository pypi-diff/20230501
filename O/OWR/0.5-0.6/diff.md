# Comparing `tmp/OWR-0.5.tar.gz` & `tmp/OWR-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-0.5.tar", last modified: Mon May  1 14:41:29 2023, max compression
+gzip compressed data, was "OWR-0.6.tar", last modified: Mon May  1 14:45:15 2023, max compression
```

## Comparing `OWR-0.5.tar` & `OWR-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:41:29.129683 OWR-0.5/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-0.5/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:41:29.125683 OWR-0.5/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6359 2023-05-01 12:02:13.000000 OWR-0.5/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:41:29.129683 OWR-0.5/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-01 14:41:29.000000 OWR-0.5/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-01 14:41:29.000000 OWR-0.5/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-01 14:41:29.000000 OWR-0.5/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       82 2023-05-01 14:41:29.000000 OWR-0.5/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-01 14:41:29.000000 OWR-0.5/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-01 14:41:29.129683 OWR-0.5/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-0.5/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-01 14:41:29.129683 OWR-0.5/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      627 2023-05-01 14:41:22.000000 OWR-0.5/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:45:15.170353 OWR-0.6/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-0.6/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:45:15.166353 OWR-0.6/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6359 2023-05-01 12:02:13.000000 OWR-0.6/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:45:15.166353 OWR-0.6/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-01 14:45:15.000000 OWR-0.6/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-01 14:45:15.000000 OWR-0.6/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-01 14:45:15.000000 OWR-0.6/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       74 2023-05-01 14:45:15.000000 OWR-0.6/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-01 14:45:15.000000 OWR-0.6/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-01 14:45:15.170353 OWR-0.6/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-0.6/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-01 14:45:15.170353 OWR-0.6/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      594 2023-05-01 14:45:05.000000 OWR-0.6/setup.py
```

### Comparing `OWR-0.5/LICENSE` & `OWR-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-0.5/OWR/__init__.py` & `OWR-0.6/OWR/__init__.py`

 * *Files identical despite different names*

### Comparing `OWR-0.5/setup.py` & `OWR-0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='0.5',
+    version='0.6',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     install_requires=['huggingsound',
                       'librosa',
                       'Levenshtein',
                       'soundfile',
                       'fonetika',
                       'numpy',
                       'playsound',
-                      'pylcs',
-                      'logging'],
+                      'pylcs'],
 )
```

