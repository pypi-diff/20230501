# Comparing `tmp/croto-0.8.tar.gz` & `tmp/croto-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croto-0.8.tar", last modified: Mon May  1 15:42:03 2023, max compression
+gzip compressed data, was "croto-0.9.tar", last modified: Mon May  1 15:47:13 2023, max compression
```

## Comparing `croto-0.8.tar` & `croto-0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:42:03.085269 croto-0.8/
--rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:42:03.085376 croto-0.8/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-0.8/README.rst
--rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 15:42:03.085707 croto-0.8/setup.cfg
--rw-r--r--   0 defeee     (501) staff       (20)      319 2023-05-01 15:42:00.000000 croto-0.8/setup.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:42:03.084027 croto-0.8/src/
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:42:03.085073 croto-0.8/src/croto.egg-info/
--rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)      161 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/SOURCES.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/dependency_links.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:42:03.000000 croto-0.8/src/croto.egg-info/top_level.txt
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:47:13.462955 croto-0.9/
+-rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:47:13.463011 croto-0.9/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-0.9/README.rst
+-rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 15:47:13.463209 croto-0.9/setup.cfg
+-rw-r--r--   0 defeee     (501) staff       (20)      319 2023-05-01 15:47:02.000000 croto-0.9/setup.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:47:13.461732 croto-0.9/src/
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 15:47:13.462825 croto-0.9/src/croto.egg-info/
+-rw-r--r--   0 defeee     (501) staff       (20)      230 2023-05-01 15:47:13.000000 croto-0.9/src/croto.egg-info/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)      161 2023-05-01 15:47:13.000000 croto-0.9/src/croto.egg-info/SOURCES.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:47:13.000000 croto-0.9/src/croto.egg-info/dependency_links.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 15:47:13.000000 croto-0.9/src/croto.egg-info/top_level.txt
```

