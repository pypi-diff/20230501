# Comparing `tmp/croto-0.91.tar.gz` & `tmp/croto-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croto-0.91.tar", last modified: Mon May  1 16:52:18 2023, max compression
+gzip compressed data, was "croto-1.1.tar", last modified: Mon May  1 17:04:52 2023, max compression
```

## Comparing `croto-0.91.tar` & `croto-1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 16:52:18.102207 croto-0.91/
--rw-r--r--   0 defeee     (501) staff       (20)      231 2023-05-01 16:52:18.102274 croto-0.91/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-0.91/README.rst
--rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 16:52:18.102548 croto-0.91/setup.cfg
--rw-r--r--   0 defeee     (501) staff       (20)      320 2023-05-01 16:52:15.000000 croto-0.91/setup.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 16:52:18.101382 croto-0.91/src/
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 16:52:18.102095 croto-0.91/src/croto.egg-info/
--rw-r--r--   0 defeee     (501) staff       (20)      231 2023-05-01 16:52:18.000000 croto-0.91/src/croto.egg-info/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)      201 2023-05-01 16:52:18.000000 croto-0.91/src/croto.egg-info/SOURCES.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 16:52:18.000000 croto-0.91/src/croto.egg-info/dependency_links.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 16:52:18.000000 croto-0.91/src/croto.egg-info/top_level.txt
--rw-r--r--   0 defeee     (501) staff       (20)     8854 2023-05-01 15:45:53.000000 croto-0.91/src/croto.py
--rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-0.91/src/strings_with_arrows.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 17:04:52.060684 croto-1.1/
+-rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 17:04:52.060730 croto-1.1/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-1.1/README.rst
+-rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 17:04:52.060910 croto-1.1/setup.cfg
+-rw-r--r--   0 defeee     (501) staff       (20)      319 2023-05-01 17:04:49.000000 croto-1.1/setup.py
+-rw-r--r--   0 defeee     (501) staff       (20)      190 2023-05-01 15:45:53.000000 croto-1.1/shell.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 17:04:52.059890 croto-1.1/src/
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 17:04:52.060579 croto-1.1/src/croto.egg-info/
+-rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 17:04:52.000000 croto-1.1/src/croto.egg-info/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)      210 2023-05-01 17:04:52.000000 croto-1.1/src/croto.egg-info/SOURCES.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 17:04:52.000000 croto-1.1/src/croto.egg-info/dependency_links.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 17:04:52.000000 croto-1.1/src/croto.egg-info/top_level.txt
+-rw-r--r--   0 defeee     (501) staff       (20)     8854 2023-05-01 15:45:53.000000 croto-1.1/src/croto.py
+-rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-1.1/src/strings_with_arrows.py
```

### Comparing `croto-0.91/src/croto.py` & `croto-1.1/src/croto.py`

 * *Files identical despite different names*

### Comparing `croto-0.91/src/strings_with_arrows.py` & `croto-1.1/src/strings_with_arrows.py`

 * *Files identical despite different names*

