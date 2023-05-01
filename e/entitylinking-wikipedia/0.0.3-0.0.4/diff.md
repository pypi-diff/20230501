# Comparing `tmp/entitylinking_wikipedia-0.0.3.tar.gz` & `tmp/entitylinking_wikipedia-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entitylinking_wikipedia-0.0.3.tar", last modified: Mon May  1 18:12:11 2023, max compression
+gzip compressed data, was "entitylinking_wikipedia-0.0.4.tar", last modified: Mon May  1 18:38:42 2023, max compression
```

## Comparing `entitylinking_wikipedia-0.0.3.tar` & `entitylinking_wikipedia-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 18:12:11.964292 entitylinking_wikipedia-0.0.3/
--rw-rw-rw-   0        0        0      518 2023-05-01 18:12:11.963292 entitylinking_wikipedia-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-01 13:15:19.000000 entitylinking_wikipedia-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 18:12:11.948265 entitylinking_wikipedia-0.0.3/Sources/
--rw-rw-rw-   0        0        0      147 2023-05-01 18:04:56.000000 entitylinking_wikipedia-0.0.3/Sources/__init__.py
--rw-rw-rw-   0        0        0       88 2023-05-01 11:57:59.000000 entitylinking_wikipedia-0.0.3/Sources/el_wikipedia.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:12:11.962381 entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/
--rw-rw-rw-   0        0        0      518 2023-05-01 18:12:11.000000 entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-01 18:12:11.000000 entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 18:12:11.000000 entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-01 18:12:11.000000 entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 18:12:11.000000 entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 18:12:11.965293 entitylinking_wikipedia-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-01 18:09:35.000000 entitylinking_wikipedia-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 18:38:42.701815 entitylinking_wikipedia-0.0.4/
+-rw-rw-rw-   0        0        0      518 2023-05-01 18:38:42.700820 entitylinking_wikipedia-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-01 13:15:19.000000 entitylinking_wikipedia-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 18:38:42.667899 entitylinking_wikipedia-0.0.4/Sources/
+-rw-rw-rw-   0        0        0      147 2023-05-01 18:04:56.000000 entitylinking_wikipedia-0.0.4/Sources/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-05-01 11:57:59.000000 entitylinking_wikipedia-0.0.4/Sources/el_wikipedia.py
+drwxrwxrwx   0        0        0        0 2023-05-01 18:38:42.698925 entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/
+-rw-rw-rw-   0        0        0      518 2023-05-01 18:38:42.000000 entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-01 18:38:42.000000 entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 18:38:42.000000 entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-01 18:38:42.000000 entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 18:38:42.000000 entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 18:38:42.702814 entitylinking_wikipedia-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-01 18:38:15.000000 entitylinking_wikipedia-0.0.4/setup.py
```

### Comparing `entitylinking_wikipedia-0.0.3/PKG-INFO` & `entitylinking_wikipedia-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entitylinking_wikipedia
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for Entity Linking using WikiPedia
 Author: Soumyadipta Maiti
 Author-email: soumya55555@gmail.com
 Keywords: Python,Entity Linking,NER,WikiPedia
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `entitylinking_wikipedia-0.0.3/entitylinking_wikipedia.egg-info/PKG-INFO` & `entitylinking_wikipedia-0.0.4/entitylinking_wikipedia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entitylinking-wikipedia
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for Entity Linking using WikiPedia
 Author: Soumyadipta Maiti
 Author-email: soumya55555@gmail.com
 Keywords: Python,Entity Linking,NER,WikiPedia
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `entitylinking_wikipedia-0.0.3/setup.py` & `entitylinking_wikipedia-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import codecs
 import os
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION='Package for Entity Linking using WikiPedia'
 
 #Setting Up
 setup(
     name='entitylinking_wikipedia',
     version=VERSION,
     author='Soumyadipta Maiti',
```

