# Comparing `tmp/entitylinking_wikipedia-0.0.5.tar.gz` & `tmp/entitylinking-wikipedia-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entitylinking_wikipedia-0.0.5.tar", last modified: Mon May  1 18:44:05 2023, max compression
+gzip compressed data, was "entitylinking-wikipedia-0.0.6.tar", last modified: Mon May  1 19:42:57 2023, max compression
```

## Comparing `entitylinking_wikipedia-0.0.5.tar` & `entitylinking-wikipedia-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 18:44:05.973976 entitylinking_wikipedia-0.0.5/
--rw-rw-rw-   0        0        0      518 2023-05-01 18:44:05.971971 entitylinking_wikipedia-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-01 13:15:19.000000 entitylinking_wikipedia-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 18:44:05.952976 entitylinking_wikipedia-0.0.5/Sources/
--rw-rw-rw-   0        0        0     2009 2023-05-01 18:42:43.000000 entitylinking_wikipedia-0.0.5/Sources/__init__.py
--rw-rw-rw-   0        0        0       88 2023-05-01 11:57:59.000000 entitylinking_wikipedia-0.0.5/Sources/el_wikipedia.py
-drwxrwxrwx   0        0        0        0 2023-05-01 18:44:05.969984 entitylinking_wikipedia-0.0.5/entitylinking_wikipedia.egg-info/
--rw-rw-rw-   0        0        0      518 2023-05-01 18:44:05.000000 entitylinking_wikipedia-0.0.5/entitylinking_wikipedia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-01 18:44:05.000000 entitylinking_wikipedia-0.0.5/entitylinking_wikipedia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 18:44:05.000000 entitylinking_wikipedia-0.0.5/entitylinking_wikipedia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-01 18:44:05.000000 entitylinking_wikipedia-0.0.5/entitylinking_wikipedia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 18:44:05.000000 entitylinking_wikipedia-0.0.5/entitylinking_wikipedia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 18:44:05.973976 entitylinking_wikipedia-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-01 18:43:07.000000 entitylinking_wikipedia-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:42:57.328392 entitylinking-wikipedia-0.0.6/
+-rw-rw-rw-   0        0        0     1165 2023-05-01 19:42:57.326391 entitylinking-wikipedia-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-05-01 19:28:26.000000 entitylinking-wikipedia-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 19:42:57.310826 entitylinking-wikipedia-0.0.6/entitylinking-wikipedia/
+-rw-rw-rw-   0        0        0     2009 2023-05-01 18:42:43.000000 entitylinking-wikipedia-0.0.6/entitylinking-wikipedia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:42:57.325392 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/
+-rw-rw-rw-   0        0        0     1165 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-01 19:42:57.000000 entitylinking-wikipedia-0.0.6/entitylinking_wikipedia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 19:42:57.328392 entitylinking-wikipedia-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-01 19:42:08.000000 entitylinking-wikipedia-0.0.6/setup.py
```

### Comparing `entitylinking_wikipedia-0.0.5/Sources/__init__.py` & `entitylinking-wikipedia-0.0.6/entitylinking-wikipedia/__init__.py`

 * *Files identical despite different names*

