# Comparing `tmp/MDbrew-2.2.0.tar.gz` & `tmp/MDbrew-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.2.0.tar", last modified: Mon May  1 09:16:58 2023, max compression
+gzip compressed data, was "MDbrew-2.2.1.tar", last modified: Mon May  1 09:20:40 2023, max compression
```

## Comparing `MDbrew-2.2.0.tar` & `MDbrew-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:13:44.175981 MDbrew-2.2.0/
--rw-------   0 minu928   (1216) minu928   (1216)       24 2023-05-01 06:01:04.000000 MDbrew-2.2.0/MANIFEST.in
-drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:13:44.172648 MDbrew-2.2.0/MDbrew/
--rw-------   0 minu928   (1216) minu928   (1216)      181 2023-05-01 09:12:21.000000 MDbrew-2.2.0/MDbrew/__init__.py
--rw-------   0 minu928   (1216) minu928   (1216)      265 2023-05-01 09:12:21.000000 MDbrew-2.2.0/MDbrew/_type.py
--rw-rw-r--   0 minu928   (1216) minu928   (1216)     2822 2023-05-01 09:12:21.000000 MDbrew-2.2.0/MDbrew/brewery.py
-drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:13:44.175981 MDbrew-2.2.0/MDbrew.egg-info/
--rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 09:13:44.000000 MDbrew-2.2.0/MDbrew.egg-info/PKG-INFO
--rw-------   0 minu928   (1216) minu928   (1216)      248 2023-05-01 09:13:44.000000 MDbrew-2.2.0/MDbrew.egg-info/SOURCES.txt
--rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 09:13:44.000000 MDbrew-2.2.0/MDbrew.egg-info/dependency_links.txt
--rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 09:13:44.000000 MDbrew-2.2.0/MDbrew.egg-info/not-zip-safe
--rw-------   0 minu928   (1216) minu928   (1216)        7 2023-05-01 09:13:44.000000 MDbrew-2.2.0/MDbrew.egg-info/top_level.txt
--rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 09:13:44.175981 MDbrew-2.2.0/PKG-INFO
--rw-------   0 minu928   (1216) minu928   (1216)       58 2023-05-01 06:01:04.000000 MDbrew-2.2.0/requirement.txt
--rw-------   0 minu928   (1216) minu928   (1216)       79 2023-05-01 09:13:44.175981 MDbrew-2.2.0/setup.cfg
--rw-------   0 minu928   (1216) minu928   (1216)      631 2023-05-01 09:12:30.000000 MDbrew-2.2.0/setup.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:17:26.632754 MDbrew-2.2.1/
+-rw-------   0 minu928   (1216) minu928   (1216)       24 2023-05-01 06:01:04.000000 MDbrew-2.2.1/MANIFEST.in
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:17:26.626088 MDbrew-2.2.1/MDbrew/
+-rw-------   0 minu928   (1216) minu928   (1216)      181 2023-05-01 09:12:21.000000 MDbrew-2.2.1/MDbrew/__init__.py
+-rw-------   0 minu928   (1216) minu928   (1216)      265 2023-05-01 09:12:21.000000 MDbrew-2.2.1/MDbrew/_type.py
+-rw-rw-r--   0 minu928   (1216) minu928   (1216)     2822 2023-05-01 09:12:21.000000 MDbrew-2.2.1/MDbrew/brewery.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:17:26.632754 MDbrew-2.2.1/MDbrew.egg-info/
+-rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/PKG-INFO
+-rw-------   0 minu928   (1216) minu928   (1216)      248 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/SOURCES.txt
+-rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/dependency_links.txt
+-rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 09:13:44.000000 MDbrew-2.2.1/MDbrew.egg-info/not-zip-safe
+-rw-------   0 minu928   (1216) minu928   (1216)        7 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/top_level.txt
+-rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 09:17:26.632754 MDbrew-2.2.1/PKG-INFO
+-rw-------   0 minu928   (1216) minu928   (1216)       58 2023-05-01 06:01:04.000000 MDbrew-2.2.1/requirement.txt
+-rw-------   0 minu928   (1216) minu928   (1216)       79 2023-05-01 09:17:26.632754 MDbrew-2.2.1/setup.cfg
+-rw-------   0 minu928   (1216) minu928   (1216)      631 2023-05-01 09:17:00.000000 MDbrew-2.2.1/setup.py
```

### Comparing `MDbrew-2.2.0/MDbrew/brewery.py` & `MDbrew-2.2.1/MDbrew/brewery.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.2.0/setup.py` & `MDbrew-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.2.0",
+    version="2.2.1",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
     download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.1.6.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
```

