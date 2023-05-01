# Comparing `tmp/OWR-0.3.0.tar.gz` & `tmp/OWR-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-0.3.0.tar", last modified: Mon May  1 14:26:13 2023, max compression
+gzip compressed data, was "OWR-0.4.0.tar", last modified: Mon May  1 14:27:54 2023, max compression
```

## Comparing `OWR-0.3.0.tar` & `OWR-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:26:13.534215 OWR-0.3.0/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-0.3.0/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:26:13.530215 OWR-0.3.0/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      278 2023-05-01 14:26:13.000000 OWR-0.3.0/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-01 14:26:13.000000 OWR-0.3.0/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-01 14:26:13.000000 OWR-0.3.0/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       81 2023-05-01 14:26:13.000000 OWR-0.3.0/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-01 14:26:13.000000 OWR-0.3.0/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      278 2023-05-01 14:26:13.534215 OWR-0.3.0/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-0.3.0/README.md
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:26:13.530215 OWR-0.3.0/owr/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6359 2023-05-01 12:02:13.000000 OWR-0.3.0/owr/__init__.py
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-01 14:26:13.534215 OWR-0.3.0/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      614 2023-05-01 14:25:45.000000 OWR-0.3.0/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:27:54.165679 OWR-0.4.0/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-0.4.0/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:27:54.165679 OWR-0.4.0/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      278 2023-05-01 14:27:54.000000 OWR-0.4.0/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-01 14:27:54.000000 OWR-0.4.0/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-01 14:27:54.000000 OWR-0.4.0/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       82 2023-05-01 14:27:54.000000 OWR-0.4.0/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-01 14:27:54.000000 OWR-0.4.0/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      278 2023-05-01 14:27:54.165679 OWR-0.4.0/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-0.4.0/README.md
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 14:27:54.165679 OWR-0.4.0/owr/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6359 2023-05-01 12:02:13.000000 OWR-0.4.0/owr/__init__.py
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-01 14:27:54.165679 OWR-0.4.0/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      615 2023-05-01 14:27:43.000000 OWR-0.4.0/setup.py
```

### Comparing `OWR-0.3.0/LICENSE` & `OWR-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-0.3.0/owr/__init__.py` & `OWR-0.4.0/owr/__init__.py`

 * *Files identical despite different names*

### Comparing `OWR-0.3.0/setup.py` & `OWR-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name='OWR',
-    version='0.3.0',
+    version='0.4.0',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['owr'],
     install_requires=['huggingsound',
-                      'librosa'
+                      'librosa',
                       'Levenshtein',
                       'soundfile',
                       'fonetika',
                       'numpy',
                       'playsound',
                       'pylcs',
                       'logging'],
```

