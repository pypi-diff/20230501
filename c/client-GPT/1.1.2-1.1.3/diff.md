# Comparing `tmp/client_GPT-1.1.2.tar.gz` & `tmp/client_GPT-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-1.1.2.tar", last modified: Mon May  1 12:51:25 2023, max compression
+gzip compressed data, was "client_GPT-1.1.3.tar", last modified: Mon May  1 12:57:09 2023, max compression
```

## Comparing `client_GPT-1.1.2.tar` & `client_GPT-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:51:25.326703 client_GPT-1.1.2/
--rw-rw-rw-   0        0        0      419 2023-05-01 12:51:25.326703 client_GPT-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 12:51:25.308704 client_GPT-1.1.2/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 12:51:24.000000 client_GPT-1.1.2/client_GPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 12:51:25.324701 client_GPT-1.1.2/client_gpt/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.2/client_gpt/__init__.py
--rw-rw-rw-   0        0        0     3925 2023-05-01 12:48:07.000000 client_GPT-1.1.2/client_gpt/client_gpt.py
--rw-rw-rw-   0        0        0       42 2023-05-01 12:51:25.327700 client_GPT-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-05-01 12:50:42.000000 client_GPT-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:57:09.970694 client_GPT-1.1.3/
+-rw-rw-rw-   0        0        0      419 2023-05-01 12:57:09.969706 client_GPT-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 12:57:09.961713 client_GPT-1.1.3/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 12:57:09.000000 client_GPT-1.1.3/client_GPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 12:57:09.965693 client_GPT-1.1.3/client_gpt/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.3/client_gpt/__init__.py
+-rw-rw-rw-   0        0        0     3925 2023-05-01 12:48:07.000000 client_GPT-1.1.3/client_gpt/client_gpt.py
+-rw-rw-rw-   0        0        0       42 2023-05-01 12:57:09.971709 client_GPT-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-05-01 12:56:47.000000 client_GPT-1.1.3/setup.py
```

### Comparing `client_GPT-1.1.2/client_gpt/client_gpt.py` & `client_GPT-1.1.3/client_gpt/client_gpt.py`

 * *Files identical despite different names*

### Comparing `client_GPT-1.1.2/setup.py` & `client_GPT-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="1.1.2",
+    version="1.1.3",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

