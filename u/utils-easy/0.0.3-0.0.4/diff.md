# Comparing `tmp/utils_easy-0.0.3.tar.gz` & `tmp/utils_easy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_easy-0.0.3.tar", last modified: Mon May  1 02:52:56 2023, max compression
+gzip compressed data, was "utils_easy-0.0.4.tar", last modified: Mon May  1 03:43:02 2023, max compression
```

## Comparing `utils_easy-0.0.3.tar` & `utils_easy-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:52:56.884932 utils_easy-0.0.3/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.3/README.md
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/easy_logger/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       39 2023-05-01 02:47:10.000000 utils_easy-0.0.3/easy_logger/__init__.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      637 2023-05-01 02:47:34.000000 utils_easy-0.0.3/easy_logger/logging_config.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1228 2023-05-01 02:48:02.000000 utils_easy-0.0.3/easy_logger/setup_logger.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-01 02:52:56.884932 utils_easy-0.0.3/setup.cfg
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      607 2023-05-01 02:52:51.000000 utils_easy-0.0.3/setup.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/stringfyobject/
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.3/stringfyobject/__init__.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.3/stringfyobject/config.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.3/stringfyobject/registry.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/utils_easy.egg-info/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      315 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/SOURCES.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/dependency_links.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       27 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/top_level.txt
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.745207 utils_easy-0.0.4/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 03:43:02.745207 utils_easy-0.0.4/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.4/README.md
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-01 03:43:02.745207 utils_easy-0.0.4/setup.cfg
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      660 2023-05-01 03:41:51.000000 utils_easy-0.0.4/setup.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy/
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy/easy_logger/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       39 2023-05-01 02:47:10.000000 utils_easy-0.0.4/utils_easy/easy_logger/__init__.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      637 2023-05-01 02:47:34.000000 utils_easy-0.0.4/utils_easy/easy_logger/logging_config.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1228 2023-05-01 02:48:02.000000 utils_easy-0.0.4/utils_easy/easy_logger/setup_logger.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy/stringfyobject/
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.4/utils_easy/stringfyobject/__init__.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.4/utils_easy/stringfyobject/config.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.4/utils_easy/stringfyobject/registry.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 03:43:02.741207 utils_easy-0.0.4/utils_easy.egg-info/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      381 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       11 2023-05-01 03:43:02.000000 utils_easy-0.0.4/utils_easy.egg-info/top_level.txt
```

### Comparing `utils_easy-0.0.3/easy_logger/logging_config.py` & `utils_easy-0.0.4/utils_easy/easy_logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `utils_easy-0.0.3/easy_logger/setup_logger.py` & `utils_easy-0.0.4/utils_easy/easy_logger/setup_logger.py`

 * *Files identical despite different names*

### Comparing `utils_easy-0.0.3/setup.py` & `utils_easy-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name="utils_easy",
-    version="0.0.3",
-    packages=find_packages(),
+    version="0.0.4",
+    packages=[
+         'utils_easy.easy_logger',
+         'utils_easy.stringfyobject'
+       ],
     install_requires=[],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
+
```

### Comparing `utils_easy-0.0.3/stringfyobject/registry.py` & `utils_easy-0.0.4/utils_easy/stringfyobject/registry.py`

 * *Files identical despite different names*

