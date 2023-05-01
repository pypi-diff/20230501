# Comparing `tmp/entitylinking-wikipedia-0.0.6.tar.gz` & `tmp/entitylinking_wikipedia-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entitylinking-wikipedia-0.0.6.tar", last modified: Mon May  1 19:42:57 2023, max compression
+gzip compressed data, was "entitylinking_wikipedia-0.0.7.tar", last modified: Mon May  1 20:41:07 2023, max compression
```

## Comparing `entitylinking-wikipedia-0.0.6.tar` & `entitylinking_wikipedia-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:42:57.328392 entitylinking-wikipedia-0.0.6/
--rw-rw-rw-   0        0        0     1165 2023-05-01 19:42:57.326391 entitylinking-wikipedia-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-05-01 19:28:26.000000 entitylinking-wikipedia-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 19:42:57.310826 entitylinking-wikipedia-0.0.6/entitylinking-wikipedia/
--rw-rw-rw-   0        0        0     2009 2023-05-01 18:42:43.000000 entitylinking-wikipedia-0.0.6/entitylinking-wikipedia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:42:57.325392 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/
--rw-rw-rw-   0        0        0     1165 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 19:42:57.328392 entitylinking-wikipedia-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-01 19:42:08.000000 entitylinking-wikipedia-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:41:07.154068 entitylinking_wikipedia-0.0.7/
+-rw-rw-rw-   0        0        0     1165 2023-05-01 20:41:07.150064 entitylinking_wikipedia-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-05-01 19:28:26.000000 entitylinking_wikipedia-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 20:41:07.104998 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia/
+-rw-rw-rw-   0        0        0     2009 2023-05-01 18:42:43.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:41:07.144986 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/
+-rw-rw-rw-   0        0        0     1165 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:41:07.155067 entitylinking_wikipedia-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-01 20:07:35.000000 entitylinking_wikipedia-0.0.7/setup.py
```

### Comparing `entitylinking-wikipedia-0.0.6/PKG-INFO` & `entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entitylinking-wikipedia
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for Entity Linking using WikiPedia
 Home-page: https://github.com/pypa/sampleproject
 Author: Soumyadipta Maiti
 Author-email: soumya55555@gmail.com
 Keywords: Python,Entity Linking,NER,WikiPedia
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `entitylinking-wikipedia-0.0.6/README.md` & `entitylinking_wikipedia-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `entitylinking-wikipedia-0.0.6/entitylinking-wikipedia/__init__.py` & `entitylinking_wikipedia-0.0.7/entitylinking_wikipedia/__init__.py`

 * *Files identical despite different names*

### Comparing `entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/PKG-INFO` & `entitylinking_wikipedia-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: entitylinking-wikipedia
-Version: 0.0.6
+Name: entitylinking_wikipedia
+Version: 0.0.7
 Summary: Package for Entity Linking using WikiPedia
 Home-page: https://github.com/pypa/sampleproject
 Author: Soumyadipta Maiti
 Author-email: soumya55555@gmail.com
 Keywords: Python,Entity Linking,NER,WikiPedia
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `entitylinking-wikipedia-0.0.6/setup.py` & `entitylinking_wikipedia-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION_FILE = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION='Package for Entity Linking using WikiPedia'
 # LONG_DESCRIPTION = file:README.md
 URL = 'https://github.com/pypa/sampleproject'
 
 #Setting Up
 setup(
-    name='entitylinking-wikipedia',
+    name='entitylinking_wikipedia',
     version=VERSION,
     author='Soumyadipta Maiti',
     author_email='soumya55555@gmail.com',
     description=DESCRIPTION,
     long_description = LONG_DESCRIPTION_FILE,
     long_description_content_type = "text/markdown",
     url= URL,
```

