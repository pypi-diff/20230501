# Comparing `tmp/utils_easy-0.0.1.tar.gz` & `tmp/utils_easy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_easy-0.0.1.tar", last modified: Sun Apr 30 15:55:40 2023, max compression
+gzip compressed data, was "utils_easy-0.0.2.tar", last modified: Mon May  1 02:32:56 2023, max compression
```

## Comparing `utils_easy-0.0.1.tar` & `utils_easy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 15:55:40.341962 utils_easy-0.0.1/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-04-30 15:55:40.341962 utils_easy-0.0.1/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.1/README.md
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 15:55:40.341962 utils_easy-0.0.1/easy_logger/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-04-30 14:52:29.000000 utils_easy-0.0.1/easy_logger/__init__.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      636 2023-04-30 14:53:55.000000 utils_easy-0.0.1/easy_logger/logging_config.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1227 2023-04-30 14:55:02.000000 utils_easy-0.0.1/easy_logger/setup_logger.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-04-30 15:55:40.341962 utils_easy-0.0.1/setup.cfg
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      606 2023-04-30 15:07:34.000000 utils_easy-0.0.1/setup.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 15:55:40.341962 utils_easy-0.0.1/stringfyobject/
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.1/stringfyobject/__init__.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.1/stringfyobject/config.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.1/stringfyobject/registry.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 15:55:40.341962 utils_easy-0.0.1/utils_easy.egg-info/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-04-30 15:55:40.000000 utils_easy-0.0.1/utils_easy.egg-info/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      315 2023-04-30 15:55:40.000000 utils_easy-0.0.1/utils_easy.egg-info/SOURCES.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-04-30 15:55:40.000000 utils_easy-0.0.1/utils_easy.egg-info/dependency_links.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       27 2023-04-30 15:55:40.000000 utils_easy-0.0.1/utils_easy.egg-info/top_level.txt
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:32:56.165135 utils_easy-0.0.2/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.2/README.md
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/easy_logger/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-04-30 14:52:29.000000 utils_easy-0.0.2/easy_logger/__init__.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      636 2023-04-30 14:53:55.000000 utils_easy-0.0.2/easy_logger/logging_config.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1227 2023-04-30 14:55:02.000000 utils_easy-0.0.2/easy_logger/setup_logger.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-01 02:32:56.165135 utils_easy-0.0.2/setup.cfg
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      607 2023-05-01 02:32:21.000000 utils_easy-0.0.2/setup.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/stringfyobject/
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.2/stringfyobject/__init__.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.2/stringfyobject/config.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.2/stringfyobject/registry.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/utils_easy.egg-info/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      315 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       27 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/top_level.txt
```

### Comparing `utils_easy-0.0.1/easy_logger/logging_config.py` & `utils_easy-0.0.2/easy_logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `utils_easy-0.0.1/easy_logger/setup_logger.py` & `utils_easy-0.0.2/easy_logger/setup_logger.py`

 * *Files identical despite different names*

### Comparing `utils_easy-0.0.1/setup.py` & `utils_easy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="utils_easy",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
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
-)
+)
```

### Comparing `utils_easy-0.0.1/stringfyobject/registry.py` & `utils_easy-0.0.2/stringfyobject/registry.py`

 * *Files identical despite different names*

