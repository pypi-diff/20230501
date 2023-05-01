# Comparing `tmp/croto-0.7.tar.gz` & `tmp/croto-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croto-0.7.tar", last modified: Mon May  1 15:37:34 2023, max compression
+gzip compressed data, was "croto-0.8.tar", last modified: Mon May  1 15:42:03 2023, max compression
```

## Comparing `croto-0.7.tar` & `croto-0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:37:34.179261 croto-0.7/
--rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:37:34.179315 croto-0.7/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-0.7/README.rst
--rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 15:37:34.179511 croto-0.7/setup.cfg
--rw-r--r--   0 defeee     (501) staff       (20)      319 2023-05-01 15:37:31.000000 croto-0.7/setup.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:37:34.178178 croto-0.7/src/
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:37:34.179149 croto-0.7/src/croto.egg-info/
--rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:37:34.000000 croto-0.7/src/croto.egg-info/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)      161 2023-05-01 15:37:34.000000 croto-0.7/src/croto.egg-info/SOURCES.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:37:34.000000 croto-0.7/src/croto.egg-info/dependency_links.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:37:34.000000 croto-0.7/src/croto.egg-info/top_level.txt
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:42:03.085269 croto-0.8/
+-rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:42:03.085376 croto-0.8/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-0.8/README.rst
+-rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 15:42:03.085707 croto-0.8/setup.cfg
+-rw-r--r--   0 defeee     (501) staff       (20)      319 2023-05-01 15:42:00.000000 croto-0.8/setup.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:42:03.084027 croto-0.8/src/
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:42:03.085073 croto-0.8/src/croto.egg-info/
+-rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)      161 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/SOURCES.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/dependency_links.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/top_level.txt
```

