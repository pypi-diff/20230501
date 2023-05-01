# Comparing `tmp/croto-1.2.tar.gz` & `tmp/croto-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croto-1.2.tar", last modified: Mon May  1 17:24:17 2023, max compression
+gzip compressed data, was "croto-2.0.tar", last modified: Mon May  1 21:13:42 2023, max compression
```

## Comparing `croto-1.2.tar` & `croto-2.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 17:24:17.427785 croto-1.2/
--rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 17:24:17.427874 croto-1.2/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-1.2/README.rst
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 17:24:17.426643 croto-1.2/croto.egg-info/
--rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 17:24:17.000000 croto-1.2/croto.egg-info/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)      201 2023-05-01 17:24:17.000000 croto-1.2/croto.egg-info/SOURCES.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 17:24:17.000000 croto-1.2/croto.egg-info/dependency_links.txt
--rw-r--r--   0 defeee     (501) staff       (20)        4 2023-05-01 17:24:17.000000 croto-1.2/croto.egg-info/top_level.txt
--rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 17:24:17.428128 croto-1.2/setup.cfg
--rw-r--r--   0 defeee     (501) staff       (20)      277 2023-05-01 17:24:15.000000 croto-1.2/setup.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 17:24:17.427254 croto-1.2/src/
--rw-r--r--   0 defeee     (501) staff       (20)        0 2023-05-01 17:02:21.000000 croto-1.2/src/__init__.py
--rw-r--r--   0 defeee     (501) staff       (20)     8854 2023-05-01 15:45:53.000000 croto-1.2/src/croto.py
--rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-1.2/src/strings_with_arrows.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:13:42.379689 croto-2.0/
+-rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:13:42.379813 croto-2.0/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-2.0/README.rst
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:13:42.378297 croto-2.0/croto/
+-rw-r--r--   0 defeee     (501) staff       (20)     8854 2023-05-01 15:45:53.000000 croto-2.0/croto/croto.py
+-rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-2.0/croto/strings_with_arrows.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:13:42.379308 croto-2.0/croto.egg-info/
+-rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)      189 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/SOURCES.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/dependency_links.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        6 2023-05-01 21:13:42.000000 croto-2.0/croto.egg-info/top_level.txt
+-rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 21:13:42.380130 croto-2.0/setup.cfg
+-rw-r--r--   0 defeee     (501) staff       (20)      382 2023-05-01 21:13:34.000000 croto-2.0/setup.py
```

### Comparing `croto-1.2/src/croto.py` & `croto-2.0/croto/croto.py`

 * *Files identical despite different names*

### Comparing `croto-1.2/src/strings_with_arrows.py` & `croto-2.0/croto/strings_with_arrows.py`

 * *Files identical despite different names*

