# Comparing `tmp/loopsso-0.0.1.tar.gz` & `tmp/loopsso-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopsso-0.0.1.tar", last modified: Sun Apr 30 21:02:52 2023, max compression
+gzip compressed data, was "dist/loopsso-0.0.2.tar", last modified: Mon May  1 20:59:06 2023, max compression
```

## Comparing `loopsso-0.0.1.tar` & `loopsso-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 omfriyad   (502) staff       (20)        0 2023-04-30 21:02:52.924875 loopsso-0.0.1/
--rw-r--r--   0 omfriyad   (502) staff       (20)     1073 2023-04-30 20:25:51.000000 loopsso-0.0.1/LICENSE
--rw-r--r--   0 omfriyad   (502) staff       (20)     1643 2023-04-30 21:02:52.924310 loopsso-0.0.1/PKG-INFO
--rw-r--r--   0 omfriyad   (502) staff       (20)      975 2023-04-30 20:56:36.000000 loopsso-0.0.1/README.md
-drwxr-xr-x   0 omfriyad   (502) staff       (20)        0 2023-04-30 21:02:52.922045 loopsso-0.0.1/loopsso.egg-info/
--rw-r--r--   0 omfriyad   (502) staff       (20)     1643 2023-04-30 21:02:52.000000 loopsso-0.0.1/loopsso.egg-info/PKG-INFO
--rw-r--r--   0 omfriyad   (502) staff       (20)      210 2023-04-30 21:02:52.000000 loopsso-0.0.1/loopsso.egg-info/SOURCES.txt
--rw-r--r--   0 omfriyad   (502) staff       (20)        1 2023-04-30 21:02:52.000000 loopsso-0.0.1/loopsso.egg-info/dependency_links.txt
--rw-r--r--   0 omfriyad   (502) staff       (20)        9 2023-04-30 21:02:52.000000 loopsso-0.0.1/loopsso.egg-info/requires.txt
--rw-r--r--   0 omfriyad   (502) staff       (20)        4 2023-04-30 21:02:52.000000 loopsso-0.0.1/loopsso.egg-info/top_level.txt
--rw-r--r--   0 omfriyad   (502) staff       (20)       38 2023-04-30 21:02:52.924992 loopsso-0.0.1/setup.cfg
--rw-r--r--   0 omfriyad   (502) staff       (20)     1185 2023-04-30 21:02:49.000000 loopsso-0.0.1/setup.py
-drwxr-xr-x   0 omfriyad   (502) staff       (20)        0 2023-04-30 21:02:52.923622 loopsso-0.0.1/src/
--rw-r--r--   0 omfriyad   (502) staff       (20)       30 2023-04-30 20:37:25.000000 loopsso-0.0.1/src/__init__.py
--rw-r--r--   0 omfriyad   (502) staff       (20)     2017 2023-04-30 21:00:27.000000 loopsso-0.0.1/src/client.py
+drwxr-xr-x   0 omfriyad   (502) staff       (20)        0 2023-05-01 20:59:06.000000 loopsso-0.0.2/
+-rw-r--r--   0 omfriyad   (502) staff       (20)     1073 2023-04-30 20:25:51.000000 loopsso-0.0.2/LICENSE
+-rw-r--r--   0 omfriyad   (502) staff       (20)     1731 2023-05-01 20:59:06.000000 loopsso-0.0.2/PKG-INFO
+-rw-r--r--   0 omfriyad   (502) staff       (20)     1062 2023-05-01 20:55:33.000000 loopsso-0.0.2/README.md
+drwxr-xr-x   0 omfriyad   (502) staff       (20)        0 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso/
+-rw-r--r--   0 omfriyad   (502) staff       (20)       31 2023-05-01 20:55:33.000000 loopsso-0.0.2/loopsso/__init__.py
+-rw-r--r--   0 omfriyad   (502) staff       (20)     2017 2023-04-30 21:00:27.000000 loopsso-0.0.2/loopsso/client.py
+drwxr-xr-x   0 omfriyad   (502) staff       (20)        0 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso.egg-info/
+-rw-r--r--   0 omfriyad   (502) staff       (20)     1731 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso.egg-info/PKG-INFO
+-rw-r--r--   0 omfriyad   (502) staff       (20)      218 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso.egg-info/SOURCES.txt
+-rw-r--r--   0 omfriyad   (502) staff       (20)        1 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso.egg-info/dependency_links.txt
+-rw-r--r--   0 omfriyad   (502) staff       (20)        9 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso.egg-info/requires.txt
+-rw-r--r--   0 omfriyad   (502) staff       (20)        8 2023-05-01 20:59:06.000000 loopsso-0.0.2/loopsso.egg-info/top_level.txt
+-rw-r--r--   0 omfriyad   (502) staff       (20)       38 2023-05-01 20:59:06.000000 loopsso-0.0.2/setup.cfg
+-rw-r--r--   0 omfriyad   (502) staff       (20)     1185 2023-05-01 20:55:33.000000 loopsso-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `loopsso-0.0.1/LICENSE` & `loopsso-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loopsso-0.0.1/PKG-INFO` & `loopsso-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopsso
-Version: 0.0.1
+Version: 0.0.2
 Summary: Api client for loops.so
 Author: Omar Faruk Riyad
 Author-email: <omfriyad@gmail.com>
 Keywords: python,loops.so,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
@@ -15,21 +15,25 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## Loops
+[PyPI 0.0.2](https://pypi.org/project/loopsso/0.0.2/)
 
 A convenient Python wrapper for the [Lopps](https://loops.so/) API.
 - API docs: [https://tryloops.notion.site/API-5b453a52dd7c4b419aa4647410de9770](https://tryloops.notion.site/API-5b453a52dd7c4b419aa4647410de9770)
 
-### Examples
-
 #### Setup
+```python
+pip install loopsso
+```
+#### Examples
+
 ```
 from loopsso import LoopsClient
 client = LoopsClinet('YOUR-API-KEY')
 
 ```
 ### Contacts Usage
 #### Create/Add
@@ -70,8 +74,7 @@
 ```
 
 #### Send
 ```
 client.send(email='adam@loops.so', event_name='conversion')
 
 ```
-
```

### Comparing `loopsso-0.0.1/README.md` & `loopsso-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 ## Loops
+[PyPI 0.0.2](https://pypi.org/project/loopsso/0.0.2/)
 
 A convenient Python wrapper for the [Lopps](https://loops.so/) API.
 - API docs: [https://tryloops.notion.site/API-5b453a52dd7c4b419aa4647410de9770](https://tryloops.notion.site/API-5b453a52dd7c4b419aa4647410de9770)
 
-### Examples
-
 #### Setup
+```python
+pip install loopsso
+```
+#### Examples
+
 ```
 from loopsso import LoopsClient
 client = LoopsClinet('YOUR-API-KEY')
 
 ```
 ### Contacts Usage
 #### Create/Add
@@ -49,9 +53,8 @@
 
 ```
 
 #### Send
 ```
 client.send(email='adam@loops.so', event_name='conversion')
 
-```
-
+```
```

### Comparing `loopsso-0.0.1/loopsso.egg-info/PKG-INFO` & `loopsso-0.0.2/loopsso.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopsso
-Version: 0.0.1
+Version: 0.0.2
 Summary: Api client for loops.so
 Author: Omar Faruk Riyad
 Author-email: <omfriyad@gmail.com>
 Keywords: python,loops.so,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
@@ -15,21 +15,25 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## Loops
+[PyPI 0.0.2](https://pypi.org/project/loopsso/0.0.2/)
 
 A convenient Python wrapper for the [Lopps](https://loops.so/) API.
 - API docs: [https://tryloops.notion.site/API-5b453a52dd7c4b419aa4647410de9770](https://tryloops.notion.site/API-5b453a52dd7c4b419aa4647410de9770)
 
-### Examples
-
 #### Setup
+```python
+pip install loopsso
+```
+#### Examples
+
 ```
 from loopsso import LoopsClient
 client = LoopsClinet('YOUR-API-KEY')
 
 ```
 ### Contacts Usage
 #### Create/Add
@@ -70,8 +74,7 @@
 ```
 
 #### Send
 ```
 client.send(email='adam@loops.so', event_name='conversion')
 
 ```
-
```

### Comparing `loopsso-0.0.1/setup.py` & `loopsso-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Api client for loops.so'
 LONG_DESCRIPTION = 'A package that allows to perform api operations on loops.so.'
 
 # Setting up
 setup(
     name="loopsso",
     version=VERSION,
```

### Comparing `loopsso-0.0.1/src/client.py` & `loopsso-0.0.2/loopsso/client.py`

 * *Files identical despite different names*

