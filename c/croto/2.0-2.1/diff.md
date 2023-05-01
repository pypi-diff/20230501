# Comparing `tmp/croto-2.0.tar.gz` & `tmp/croto-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croto-2.0.tar", last modified: Mon May  1 21:13:42 2023, max compression
+gzip compressed data, was "croto-2.1.tar", last modified: Mon May  1 21:24:03 2023, max compression
```

## Comparing `croto-2.0.tar` & `croto-2.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:13:42.379689 croto-2.0/
--rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:13:42.379813 croto-2.0/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-2.0/README.rst
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:13:42.378297 croto-2.0/croto/
--rw-r--r--   0 defeee     (501) staff       (20)     8854 2023-05-01 15:45:53.000000 croto-2.0/croto/croto.py
--rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-2.0/croto/strings_with_arrows.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:13:42.379308 croto-2.0/croto.egg-info/
--rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)      189 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/SOURCES.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/dependency_links.txt
--rw-r--r--   0 defeee     (501) staff       (20)        6 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/top_level.txt
--rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 21:13:42.380130 croto-2.0/setup.cfg
--rw-r--r--   0 defeee     (501) staff       (20)      382 2023-05-01 21:13:34.000000 croto-2.0/setup.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.464523 croto-2.1/
+-rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:24:03.464587 croto-2.1/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-2.1/README.rst
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.463461 croto-2.1/coppado/
+-rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-2.1/coppado/strings_with_arrows.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.463818 croto-2.1/croto/
+-rw-r--r--   0 defeee     (501) staff       (20)        0 2023-05-01 21:20:56.000000 croto-2.1/croto/__init__.py
+-rw-r--r--   0 defeee     (501) staff       (20)     8858 2023-05-01 21:18:17.000000 croto-2.1/croto/croto.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.464412 croto-2.1/croto.egg-info/
+-rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)      209 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/SOURCES.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/dependency_links.txt
+-rw-r--r--   0 defeee     (501) staff       (20)       14 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/top_level.txt
+-rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 21:24:03.464794 croto-2.1/setup.cfg
+-rw-r--r--   0 defeee     (501) staff       (20)      394 2023-05-01 21:24:00.000000 croto-2.1/setup.py
```

### Comparing `croto-2.0/croto/croto.py` & `croto-2.1/croto/croto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.strings_with_arrows import *
+from coppado.strings_with_arrows import *
 
 ###################################################
 # CONSTANTES
 ###################################################
 
 DIGITS = '0123456789'
```

### Comparing `croto-2.0/croto/strings_with_arrows.py` & `croto-2.1/coppado/strings_with_arrows.py`

 * *Files identical despite different names*

