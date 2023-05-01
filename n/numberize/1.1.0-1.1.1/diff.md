# Comparing `tmp/numberize-1.1.0.tar.gz` & `tmp/numberize-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numberize-1.1.0.tar", last modified: Mon May  1 12:56:31 2023, max compression
+gzip compressed data, was "numberize-1.1.1.tar", last modified: Mon May  1 13:03:33 2023, max compression
```

## Comparing `numberize-1.1.0.tar` & `numberize-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:56:31.793541 numberize-1.1.0/
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1073 2023-05-01 11:12:42.000000 numberize-1.1.0/LICENSE
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1185 2023-05-01 12:56:31.793541 numberize-1.1.0/PKG-INFO
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      630 2023-05-01 11:12:42.000000 numberize-1.1.0/README.md
-drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:56:31.789540 numberize-1.1.0/numberize/
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      105 2023-05-01 11:12:42.000000 numberize-1.1.0/numberize/__init__.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1646 2023-05-01 11:12:42.000000 numberize-1.1.0/numberize/calculators.py
-drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:56:31.793541 numberize-1.1.0/numberize/dicts/
--rw-rw-r--   0 danylo    (1000) danylo    (1000)       91 2023-05-01 11:12:42.000000 numberize-1.1.0/numberize/dicts/__init__.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      479 2023-05-01 11:51:54.000000 numberize-1.1.0/numberize/dicts/en.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      981 2023-05-01 11:51:54.000000 numberize-1.1.0/numberize/dicts/ru.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      965 2023-05-01 11:51:54.000000 numberize-1.1.0/numberize/dicts/uk.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     2150 2023-05-01 12:51:11.000000 numberize-1.1.0/numberize/linguists.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      507 2023-05-01 11:12:42.000000 numberize-1.1.0/numberize/numberizer.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     2339 2023-05-01 12:51:13.000000 numberize-1.1.0/numberize/replacers.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     2951 2023-05-01 11:12:42.000000 numberize-1.1.0/numberize/tokenizers.py
-drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:56:31.789540 numberize-1.1.0/numberize.egg-info/
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1185 2023-05-01 12:56:31.000000 numberize-1.1.0/numberize.egg-info/PKG-INFO
--rw-rw-r--   0 danylo    (1000) danylo    (1000)      500 2023-05-01 12:56:31.000000 numberize-1.1.0/numberize.egg-info/SOURCES.txt
--rw-rw-r--   0 danylo    (1000) danylo    (1000)        1 2023-05-01 12:56:31.000000 numberize-1.1.0/numberize.egg-info/dependency_links.txt
--rw-rw-r--   0 danylo    (1000) danylo    (1000)       40 2023-05-01 12:56:31.000000 numberize-1.1.0/numberize.egg-info/requires.txt
--rw-rw-r--   0 danylo    (1000) danylo    (1000)       10 2023-05-01 12:56:31.000000 numberize-1.1.0/numberize.egg-info/top_level.txt
--rw-rw-r--   0 danylo    (1000) danylo    (1000)       38 2023-05-01 12:56:31.793541 numberize-1.1.0/setup.cfg
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1018 2023-05-01 12:56:23.000000 numberize-1.1.0/setup.py
-drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 12:56:31.793541 numberize-1.1.0/tests/
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1005 2023-05-01 11:12:42.000000 numberize-1.1.0/tests/test_calculators.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     1482 2023-05-01 12:54:45.000000 numberize-1.1.0/tests/test_linguists.py
--rw-rw-r--   0 danylo    (1000) danylo    (1000)     2536 2023-05-01 11:12:42.000000 numberize-1.1.0/tests/test_numberizer.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 13:03:33.675917 numberize-1.1.1/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1073 2023-05-01 11:12:42.000000 numberize-1.1.1/LICENSE
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1185 2023-05-01 13:03:33.675917 numberize-1.1.1/PKG-INFO
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      630 2023-05-01 11:12:42.000000 numberize-1.1.1/README.md
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 13:03:33.675917 numberize-1.1.1/numberize/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      105 2023-05-01 11:12:42.000000 numberize-1.1.1/numberize/__init__.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1646 2023-05-01 11:12:42.000000 numberize-1.1.1/numberize/calculators.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 13:03:33.675917 numberize-1.1.1/numberize/dicts/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       91 2023-05-01 11:12:42.000000 numberize-1.1.1/numberize/dicts/__init__.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      479 2023-05-01 11:51:54.000000 numberize-1.1.1/numberize/dicts/en.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      981 2023-05-01 11:51:54.000000 numberize-1.1.1/numberize/dicts/ru.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      965 2023-05-01 11:51:54.000000 numberize-1.1.1/numberize/dicts/uk.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2150 2023-05-01 12:51:11.000000 numberize-1.1.1/numberize/linguists.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      507 2023-05-01 11:12:42.000000 numberize-1.1.1/numberize/numberizer.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2339 2023-05-01 12:51:13.000000 numberize-1.1.1/numberize/replacers.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2951 2023-05-01 11:12:42.000000 numberize-1.1.1/numberize/tokenizers.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 13:03:33.675917 numberize-1.1.1/numberize.egg-info/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1185 2023-05-01 13:03:33.000000 numberize-1.1.1/numberize.egg-info/PKG-INFO
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)      500 2023-05-01 13:03:33.000000 numberize-1.1.1/numberize.egg-info/SOURCES.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)        1 2023-05-01 13:03:33.000000 numberize-1.1.1/numberize.egg-info/dependency_links.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       40 2023-05-01 13:03:33.000000 numberize-1.1.1/numberize.egg-info/requires.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       10 2023-05-01 13:03:33.000000 numberize-1.1.1/numberize.egg-info/top_level.txt
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)       38 2023-05-01 13:03:33.675917 numberize-1.1.1/setup.cfg
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1018 2023-05-01 13:03:19.000000 numberize-1.1.1/setup.py
+drwxrwxr-x   0 danylo    (1000) danylo    (1000)        0 2023-05-01 13:03:33.675917 numberize-1.1.1/tests/
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1005 2023-05-01 11:12:42.000000 numberize-1.1.1/tests/test_calculators.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     1482 2023-05-01 12:54:45.000000 numberize-1.1.1/tests/test_linguists.py
+-rw-rw-r--   0 danylo    (1000) danylo    (1000)     2536 2023-05-01 11:12:42.000000 numberize-1.1.1/tests/test_numberizer.py
```

### Comparing `numberize-1.1.0/LICENSE` & `numberize-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/PKG-INFO` & `numberize-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numberize
-Version: 1.1.0
+Version: 1.1.1
 Summary: Replace numerals with numbers
 Home-page: https://github.com/DanATW/numberize.git
 Author: YemchenkoDS
 Author-email: emchenko@dlit.dp.ua
 Project-URL: Bug Tracker, https://github.com/DanATW/numberize/issues
 Keywords: text replace numerals words numbers morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numberize-1.1.0/README.md` & `numberize-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize/calculators.py` & `numberize-1.1.1/numberize/calculators.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize/dicts/ru.py` & `numberize-1.1.1/numberize/dicts/ru.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize/dicts/uk.py` & `numberize-1.1.1/numberize/dicts/uk.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize/linguists.py` & `numberize-1.1.1/numberize/linguists.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize/replacers.py` & `numberize-1.1.1/numberize/replacers.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize/tokenizers.py` & `numberize-1.1.1/numberize/tokenizers.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/numberize.egg-info/PKG-INFO` & `numberize-1.1.1/numberize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numberize
-Version: 1.1.0
+Version: 1.1.1
 Summary: Replace numerals with numbers
 Home-page: https://github.com/DanATW/numberize.git
 Author: YemchenkoDS
 Author-email: emchenko@dlit.dp.ua
 Project-URL: Bug Tracker, https://github.com/DanATW/numberize/issues
 Keywords: text replace numerals words numbers morphology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `numberize-1.1.0/setup.py` & `numberize-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="numberize",
-    version="1.1.0",
+    version="1.1.1",
     author="YemchenkoDS",
     author_email="emchenko@dlit.dp.ua",
     description="Replace numerals with numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanATW/numberize.git",
     project_urls={
```

### Comparing `numberize-1.1.0/tests/test_calculators.py` & `numberize-1.1.1/tests/test_calculators.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/tests/test_linguists.py` & `numberize-1.1.1/tests/test_linguists.py`

 * *Files identical despite different names*

### Comparing `numberize-1.1.0/tests/test_numberizer.py` & `numberize-1.1.1/tests/test_numberizer.py`

 * *Files identical despite different names*

