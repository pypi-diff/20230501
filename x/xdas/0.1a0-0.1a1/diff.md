# Comparing `tmp/xdas-0.1a0.tar.gz` & `tmp/xdas-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdas-0.1a0.tar", last modified: Mon May  1 19:09:18 2023, max compression
+gzip compressed data, was "xdas-0.1a1.tar", last modified: Mon May  1 19:12:55 2023, max compression
```

## Comparing `xdas-0.1a0.tar` & `xdas-0.1a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:09:18.369625 xdas-0.1a0/
--rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1a0/LICENSE.md
--rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-05-01 19:09:18.369476 xdas-0.1a0/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)     1352 2023-05-01 18:57:32.000000 xdas-0.1a0/README.md
--rw-r--r--   0 trabatto   (502) staff       (20)      454 2023-05-01 19:03:36.000000 xdas-0.1a0/pyproject.toml
--rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-05-01 19:09:18.369663 xdas-0.1a0/setup.cfg
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:09:18.367428 xdas-0.1a0/tests/
--rw-r--r--   0 trabatto   (502) staff       (20)    11180 2023-02-23 15:44:38.000000 xdas-0.1a0/tests/test_core.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2573 2023-02-23 15:50:41.000000 xdas-0.1a0/tests/test_signaltools.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:09:18.367896 xdas-0.1a0/xdas/
--rw-r--r--   0 trabatto   (502) staff       (20)      171 2023-02-23 09:32:18.000000 xdas-0.1a0/xdas/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)    21837 2023-03-13 16:30:29.000000 xdas-0.1a0/xdas/core.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:09:18.369254 xdas-0.1a0/xdas/io/
--rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1a0/xdas/io/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)      627 2023-02-23 09:32:18.000000 xdas-0.1a0/xdas/io/asn.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-02-23 09:32:18.000000 xdas-0.1a0/xdas/io/febus.py
--rw-r--r--   0 trabatto   (502) staff       (20)     5363 2023-03-10 10:53:44.000000 xdas-0.1a0/xdas/signaltools.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:09:18.368759 xdas-0.1a0/xdas.egg-info/
--rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-05-01 19:09:18.000000 xdas-0.1a0/xdas.egg-info/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)      321 2023-05-01 19:09:18.000000 xdas-0.1a0/xdas.egg-info/SOURCES.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-05-01 19:09:18.000000 xdas-0.1a0/xdas.egg-info/dependency_links.txt
--rw-r--r--   0 trabatto   (502) staff       (20)      101 2023-05-01 19:09:18.000000 xdas-0.1a0/xdas.egg-info/requires.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-05-01 19:09:18.000000 xdas-0.1a0/xdas.egg-info/top_level.txt
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.462263 xdas-0.1a1/
+-rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1a1/LICENSE.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-05-01 19:12:55.462129 xdas-0.1a1/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)     1352 2023-05-01 18:57:32.000000 xdas-0.1a1/README.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      455 2023-05-01 19:12:15.000000 xdas-0.1a1/pyproject.toml
+-rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-05-01 19:12:55.462299 xdas-0.1a1/setup.cfg
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.460608 xdas-0.1a1/tests/
+-rw-r--r--   0 trabatto   (502) staff       (20)    11180 2023-02-23 15:44:38.000000 xdas-0.1a1/tests/test_core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     2573 2023-02-23 15:50:41.000000 xdas-0.1a1/tests/test_signaltools.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.460991 xdas-0.1a1/xdas/
+-rw-r--r--   0 trabatto   (502) staff       (20)      171 2023-02-23 09:32:18.000000 xdas-0.1a1/xdas/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    21837 2023-03-13 16:30:29.000000 xdas-0.1a1/xdas/core.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.461961 xdas-0.1a1/xdas/io/
+-rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1a1/xdas/io/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      627 2023-02-23 09:32:18.000000 xdas-0.1a1/xdas/io/asn.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-02-23 09:32:18.000000 xdas-0.1a1/xdas/io/febus.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     5363 2023-03-10 10:53:44.000000 xdas-0.1a1/xdas/signaltools.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.461591 xdas-0.1a1/xdas.egg-info/
+-rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)      321 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/SOURCES.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/dependency_links.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)      101 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/requires.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/top_level.txt
```

### Comparing `xdas-0.1a0/LICENSE.md` & `xdas-0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/README.md` & `xdas-0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/tests/test_core.py` & `xdas-0.1a1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/tests/test_signaltools.py` & `xdas-0.1a1/tests/test_signaltools.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/xdas/core.py` & `xdas-0.1a1/xdas/core.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/xdas/io/asn.py` & `xdas-0.1a1/xdas/io/asn.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/xdas/io/febus.py` & `xdas-0.1a1/xdas/io/febus.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a0/xdas/signaltools.py` & `xdas-0.1a1/xdas/signaltools.py`

 * *Files identical despite different names*

