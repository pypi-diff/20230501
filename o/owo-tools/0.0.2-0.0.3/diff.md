# Comparing `tmp/owo_tools-0.0.2.tar.gz` & `tmp/owo_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\owo_tools-0.0.2.tar", last modified: Mon May  1 09:33:46 2023, max compression
+gzip compressed data, was "dist\owo_tools-0.0.3.tar", last modified: Mon May  1 09:46:37 2023, max compression
```

## Comparing `owo_tools-0.0.2.tar` & `owo_tools-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:33:46.193983 owo_tools-0.0.2/
--rw-rw-rw-   0        0        0      460 2023-05-01 09:33:46.191983 owo_tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-01 09:19:31.000000 owo_tools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 09:33:46.176664 owo_tools-0.0.2/owo_tools/
--rw-rw-rw-   0        0        0       23 2023-05-01 09:24:14.000000 owo_tools-0.0.2/owo_tools/__init__.py
--rw-rw-rw-   0        0        0      763 2023-05-01 09:19:31.000000 owo_tools-0.0.2/owo_tools/autoEDA.py
--rw-rw-rw-   0        0        0     1357 2023-05-01 09:29:11.000000 owo_tools-0.0.2/owo_tools/encrypt.py
--rw-rw-rw-   0        0        0     1689 2023-05-01 09:19:31.000000 owo_tools-0.0.2/owo_tools/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:33:46.187371 owo_tools-0.0.2/owo_tools.egg-info/
--rw-rw-rw-   0        0        0      460 2023-05-01 09:33:46.000000 owo_tools-0.0.2/owo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-01 09:33:46.000000 owo_tools-0.0.2/owo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:33:46.000000 owo_tools-0.0.2/owo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 09:33:46.000000 owo_tools-0.0.2/owo_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 09:33:46.193983 owo_tools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-05-01 09:25:35.000000 owo_tools-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:33:46.189976 owo_tools-0.0.2/test/
--rw-rw-rw-   0        0        0      722 2023-05-01 09:30:57.000000 owo_tools-0.0.2/test/test_encrypt.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:46:37.374003 owo_tools-0.0.3/
+-rw-rw-rw-   0        0        0      460 2023-05-01 09:46:37.296366 owo_tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-01 09:19:31.000000 owo_tools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 09:46:37.281350 owo_tools-0.0.3/owo_tools/
+-rw-rw-rw-   0        0        0       23 2023-05-01 09:45:19.000000 owo_tools-0.0.3/owo_tools/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-05-01 09:19:31.000000 owo_tools-0.0.3/owo_tools/autoEDA.py
+-rw-rw-rw-   0        0        0     1357 2023-05-01 09:29:11.000000 owo_tools-0.0.3/owo_tools/encrypt.py
+-rw-rw-rw-   0        0        0      726 2023-05-01 09:44:19.000000 owo_tools-0.0.3/owo_tools/notify.py
+-rw-rw-rw-   0        0        0     1689 2023-05-01 09:19:31.000000 owo_tools-0.0.3/owo_tools/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:46:37.292278 owo_tools-0.0.3/owo_tools.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-05-01 09:46:37.000000 owo_tools-0.0.3/owo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-05-01 09:46:37.000000 owo_tools-0.0.3/owo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:46:37.000000 owo_tools-0.0.3/owo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-01 09:46:37.000000 owo_tools-0.0.3/owo_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:46:37.376000 owo_tools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-05-01 09:45:13.000000 owo_tools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:46:37.294849 owo_tools-0.0.3/test/
+-rw-rw-rw-   0        0        0      722 2023-05-01 09:30:57.000000 owo_tools-0.0.3/test/test_encrypt.py
```

### Comparing `owo_tools-0.0.2/owo_tools/autoEDA.py` & `owo_tools-0.0.3/owo_tools/autoEDA.py`

 * *Files identical despite different names*

### Comparing `owo_tools-0.0.2/owo_tools/encrypt.py` & `owo_tools-0.0.3/owo_tools/encrypt.py`

 * *Files identical despite different names*

### Comparing `owo_tools-0.0.2/owo_tools/plot.py` & `owo_tools-0.0.3/owo_tools/plot.py`

 * *Files identical despite different names*

### Comparing `owo_tools-0.0.2/setup.py` & `owo_tools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="owo_tools",
-    version="0.0.2",
+    version="0.0.3",
     author="Ryan Liu",
     author_email="pm@owomail.cc",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Keycatowo/owo_tools",
     packages=setuptools.find_packages(),
```

### Comparing `owo_tools-0.0.2/test/test_encrypt.py` & `owo_tools-0.0.3/test/test_encrypt.py`

 * *Files identical despite different names*

