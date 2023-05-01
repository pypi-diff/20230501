# Comparing `tmp/utils_easy-0.0.2.tar.gz` & `tmp/utils_easy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_easy-0.0.2.tar", last modified: Mon May  1 02:32:56 2023, max compression
+gzip compressed data, was "utils_easy-0.0.3.tar", last modified: Mon May  1 02:52:56 2023, max compression
```

## Comparing `utils_easy-0.0.2.tar` & `utils_easy-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:32:56.165135 utils_easy-0.0.2/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.2/README.md
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/easy_logger/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-04-30 14:52:29.000000 utils_easy-0.0.2/easy_logger/__init__.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      636 2023-04-30 14:53:55.000000 utils_easy-0.0.2/easy_logger/logging_config.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1227 2023-04-30 14:55:02.000000 utils_easy-0.0.2/easy_logger/setup_logger.py
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-01 02:32:56.165135 utils_easy-0.0.2/setup.cfg
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      607 2023-05-01 02:32:21.000000 utils_easy-0.0.2/setup.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/stringfyobject/
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.2/stringfyobject/__init__.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.2/stringfyobject/config.py
--rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.2/stringfyobject/registry.py
-drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:32:56.165135 utils_easy-0.0.2/utils_easy.egg-info/
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/PKG-INFO
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      315 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/SOURCES.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/dependency_links.txt
--rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       27 2023-05-01 02:32:56.000000 utils_easy-0.0.2/utils_easy.egg-info/top_level.txt
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:52:56.884932 utils_easy-0.0.3/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       62 2023-04-30 15:03:42.000000 utils_easy-0.0.3/README.md
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/easy_logger/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       39 2023-05-01 02:47:10.000000 utils_easy-0.0.3/easy_logger/__init__.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      637 2023-05-01 02:47:34.000000 utils_easy-0.0.3/easy_logger/logging_config.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)     1228 2023-05-01 02:48:02.000000 utils_easy-0.0.3/easy_logger/setup_logger.py
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       38 2023-05-01 02:52:56.884932 utils_easy-0.0.3/setup.cfg
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      607 2023-05-01 02:52:51.000000 utils_easy-0.0.3/setup.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/stringfyobject/
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)        0 2023-04-30 01:39:44.000000 utils_easy-0.0.3/stringfyobject/__init__.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      404 2023-04-30 12:00:32.000000 utils_easy-0.0.3/stringfyobject/config.py
+-rw-r--r--   0 cybercore  (1000) cybercore  (1000)      645 2023-04-30 14:55:26.000000 utils_easy-0.0.3/stringfyobject/registry.py
+drwxrwxr-x   0 cybercore  (1000) cybercore  (1000)        0 2023-05-01 02:52:56.884932 utils_easy-0.0.3/utils_easy.egg-info/
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      492 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/PKG-INFO
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)      315 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)        1 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cybercore  (1000) cybercore  (1000)       27 2023-05-01 02:52:56.000000 utils_easy-0.0.3/utils_easy.egg-info/top_level.txt
```

### Comparing `utils_easy-0.0.2/easy_logger/logging_config.py` & `utils_easy-0.0.3/easy_logger/logging_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         "file": {
             "class": "logging.FileHandler",
             "level": "WARNING",
             "formatter": "default",
             "filename": "",
         },
     },
-}
+}
```

### Comparing `utils_easy-0.0.2/easy_logger/setup_logger.py` & `utils_easy-0.0.3/easy_logger/setup_logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         file_handler.setFormatter(logging.Formatter(LOGGING_CONFIG["formatters"]["default"]["format"]))
         
 
         logger.addHandler(console_handler)
         logger.addHandler(file_handler)
         logger.propagate = False
 
-    return logger
+    return logger
```

### Comparing `utils_easy-0.0.2/setup.py` & `utils_easy-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="utils_easy",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     install_requires=[],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `utils_easy-0.0.2/stringfyobject/registry.py` & `utils_easy-0.0.3/stringfyobject/registry.py`

 * *Files identical despite different names*

