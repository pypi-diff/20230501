# Comparing `tmp/toxicjasmine-0.2.1.tar.gz` & `tmp/toxicjasmine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toxicjasmine-0.2.1.tar", last modified: Mon May  1 03:10:09 2023, max compression
+gzip compressed data, was "toxicjasmine-0.2.2.tar", last modified: Mon May  1 03:36:24 2023, max compression
```

## Comparing `toxicjasmine-0.2.1.tar` & `toxicjasmine-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/
--rw-rw-r--   0 juca      (1001) juca      (1001)       70 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/MANIFEST.in
--rw-rw-r--   0 juca      (1001) juca      (1001)      594 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/PKG-INFO
--rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/setup.cfg
--rw-rw-r--   0 juca      (1001) juca      (1001)     1168 2023-05-01 03:09:29.000000 toxicjasmine-0.2.1/setup.py
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/toxicjasmine/
--rw-rw-r--   0 juca      (1001) juca      (1001)       26 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/README
--rw-rw-r--   0 juca      (1001) juca      (1001)     7914 2023-05-01 03:08:27.000000 toxicjasmine-0.2.1/toxicjasmine/__init__.py
--rw-rw-r--   0 juca      (1001) juca      (1001)     6227 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/boot.js
--rw-rw-r--   0 juca      (1001) juca      (1001)    20494 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine-clear.css
--rw-rw-r--   0 juca      (1001) juca      (1001)    20591 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine-dark.css
--rw-rw-r--   0 juca      (1001) juca      (1001)    23571 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine-html.js
--rw-rw-r--   0 juca      (1001) juca      (1001)    21115 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine.css
--rw-rw-r--   0 juca      (1001) juca      (1001)   232520 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/jasmine.js
--rw-rw-r--   0 juca      (1001) juca      (1001)    17569 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/json2.js
--rw-rw-r--   0 juca      (1001) juca      (1001)     2198 2023-05-01 03:07:50.000000 toxicjasmine-0.2.1/toxicjasmine/monkey.py
--rw-rw-r--   0 juca      (1001) juca      (1001)     1491 2023-05-01 02:54:26.000000 toxicjasmine-0.2.1/toxicjasmine/node_boot.js
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:10:09.582877 toxicjasmine-0.2.1/toxicjasmine.egg-info/
--rw-rw-r--   0 juca      (1001) juca      (1001)      594 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/PKG-INFO
--rw-rw-r--   0 juca      (1001) juca      (1001)      514 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/SOURCES.txt
--rw-rw-r--   0 juca      (1001) juca      (1001)        1 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/dependency_links.txt
--rw-rw-r--   0 juca      (1001) juca      (1001)       52 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/entry_points.txt
--rw-rw-r--   0 juca      (1001) juca      (1001)       68 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/requires.txt
--rw-rw-r--   0 juca      (1001) juca      (1001)       13 2023-05-01 03:10:09.000000 toxicjasmine-0.2.1/toxicjasmine.egg-info/top_level.txt
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:36:24.295376 toxicjasmine-0.2.2/
+-rw-rw-r--   0 juca      (1001) juca      (1001)       70 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/MANIFEST.in
+-rw-rw-r--   0 juca      (1001) juca      (1001)      594 2023-05-01 03:36:24.295376 toxicjasmine-0.2.2/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-05-01 03:36:24.295376 toxicjasmine-0.2.2/setup.cfg
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1168 2023-05-01 03:35:53.000000 toxicjasmine-0.2.2/setup.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:36:24.295376 toxicjasmine-0.2.2/toxicjasmine/
+-rw-rw-r--   0 juca      (1001) juca      (1001)       26 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/README
+-rw-rw-r--   0 juca      (1001) juca      (1001)     7917 2023-05-01 03:35:40.000000 toxicjasmine-0.2.2/toxicjasmine/__init__.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     6227 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/boot.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)    20494 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/jasmine-clear.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    20591 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/jasmine-dark.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    23571 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/jasmine-html.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)    21115 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/jasmine.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)   232520 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/jasmine.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)    17569 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/json2.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)     2198 2023-05-01 03:07:50.000000 toxicjasmine-0.2.2/toxicjasmine/monkey.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1491 2023-05-01 02:54:26.000000 toxicjasmine-0.2.2/toxicjasmine/node_boot.js
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-01 03:36:24.295376 toxicjasmine-0.2.2/toxicjasmine.egg-info/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      594 2023-05-01 03:36:24.000000 toxicjasmine-0.2.2/toxicjasmine.egg-info/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      514 2023-05-01 03:36:24.000000 toxicjasmine-0.2.2/toxicjasmine.egg-info/SOURCES.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)        1 2023-05-01 03:36:24.000000 toxicjasmine-0.2.2/toxicjasmine.egg-info/dependency_links.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       52 2023-05-01 03:36:24.000000 toxicjasmine-0.2.2/toxicjasmine.egg-info/entry_points.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       68 2023-05-01 03:36:24.000000 toxicjasmine-0.2.2/toxicjasmine.egg-info/requires.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       13 2023-05-01 03:36:24.000000 toxicjasmine-0.2.2/toxicjasmine.egg-info/top_level.txt
```

### Comparing `toxicjasmine-0.2.1/PKG-INFO` & `toxicjasmine-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toxicjasmine
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toxicjasmine: Nothing interresting here.
 Home-page: 
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: GPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
```

### Comparing `toxicjasmine-0.2.1/setup.py` & `toxicjasmine-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 DESCRIPTION = """
 Toxicjasmine: Nothing interresting here.
 """.strip()
 
 
 setup(name='toxicjasmine',
```

### Comparing `toxicjasmine-0.2.1/toxicjasmine/__init__.py` & `toxicjasmine-0.2.2/toxicjasmine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 import cherrypy
 from jasmine_core.core import Core
 from jasmine.config import Config
 from jasmine.entry_points import Command
 from jasmine.standalone import JasmineApp
 from jasmine.ci import CIRunner, TestServerThread
 
+from toxicjasmine.monkey import MonkeyPatcher
+
+monkey = MonkeyPatcher()
+monkey.patch_all()
+
+
 
 class ToxicjasmineApp(JasmineApp):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.jasmine_file = ToxicjasmineFile()
 
@@ -226,11 +232,8 @@
     else:
         args = sys.argv[1:]
 
     cmd.run(args)
 
 
 if __name__ == '__main__':
-    from .monkey import MonkeyPatcher
-    monkey = MonkeyPatcher()
-    monkey.patch_all()
     begin()
```

### Comparing `toxicjasmine-0.2.1/toxicjasmine/boot.js` & `toxicjasmine-0.2.2/toxicjasmine/boot.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/jasmine-clear.css` & `toxicjasmine-0.2.2/toxicjasmine/jasmine-clear.css`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/jasmine-dark.css` & `toxicjasmine-0.2.2/toxicjasmine/jasmine-dark.css`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/jasmine-html.js` & `toxicjasmine-0.2.2/toxicjasmine/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/jasmine.css` & `toxicjasmine-0.2.2/toxicjasmine/jasmine.css`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/jasmine.js` & `toxicjasmine-0.2.2/toxicjasmine/jasmine.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/json2.js` & `toxicjasmine-0.2.2/toxicjasmine/json2.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/monkey.py` & `toxicjasmine-0.2.2/toxicjasmine/monkey.py`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine/node_boot.js` & `toxicjasmine-0.2.2/toxicjasmine/node_boot.js`

 * *Files identical despite different names*

### Comparing `toxicjasmine-0.2.1/toxicjasmine.egg-info/PKG-INFO` & `toxicjasmine-0.2.2/toxicjasmine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toxicjasmine
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toxicjasmine: Nothing interresting here.
 Home-page: 
 Author: Juca Crispim
 Author-email: juca@poraodojuca.net
 License: GPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: No Input/Output (Daemon)
```

### Comparing `toxicjasmine-0.2.1/toxicjasmine.egg-info/SOURCES.txt` & `toxicjasmine-0.2.2/toxicjasmine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

