# Comparing `tmp/jmespath-community-1.1.1.tar.gz` & `tmp/jmespath-community-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmespath-community-1.1.1.tar", last modified: Fri Apr  7 15:27:58 2023, max compression
+gzip compressed data, was "jmespath-community-1.1.2.tar", last modified: Mon May  1 00:20:41 2023, max compression
```

## Comparing `jmespath-community-1.1.1.tar` & `jmespath-community-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1113 2023-04-07 14:59:05.000000 jmespath-community-1.1.1/LICENSE
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)       35 2023-04-07 14:59:05.000000 jmespath-community-1.1.1/MANIFEST.in
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)    10906 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/PKG-INFO
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     7884 2023-04-07 14:58:41.000000 jmespath-community-1.1.1/README.rst
-drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/bin/
--rwxr-xr-x   0 springcomp  (1000) springcomp  (1000)     1814 2023-04-07 14:58:41.000000 jmespath-community-1.1.1/bin/jp.py
-drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/jmespath/
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)      307 2023-04-07 15:26:59.000000 jmespath-community-1.1.1/jmespath/__init__.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     2736 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/ast.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)      369 2023-04-07 14:58:41.000000 jmespath-community-1.1.1/jmespath/compat.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     4794 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/exceptions.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)    19822 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/functions.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)    10614 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/lexer.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)    21644 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/parser.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1417 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/scope.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)    13551 2023-04-07 15:09:16.000000 jmespath-community-1.1.1/jmespath/visitor.py
-drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/jmespath_community.egg-info/
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)    10906 2023-04-07 15:27:58.000000 jmespath-community-1.1.1/jmespath_community.egg-info/PKG-INFO
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)      455 2023-04-07 15:27:58.000000 jmespath-community-1.1.1/jmespath_community.egg-info/SOURCES.txt
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)        1 2023-04-07 15:27:58.000000 jmespath-community-1.1.1/jmespath_community.egg-info/dependency_links.txt
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)       15 2023-04-07 15:27:58.000000 jmespath-community-1.1.1/jmespath_community.egg-info/top_level.txt
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)      102 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/setup.cfg
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1242 2023-04-07 15:26:59.000000 jmespath-community-1.1.1/setup.py
-drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/tests/
-drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-04-07 15:27:58.413715 jmespath-community-1.1.1/tests/legacy/
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)       16 2023-04-07 14:58:41.000000 jmespath-community-1.1.1/tests/legacy/__init__.py
--rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1301 2023-04-07 14:58:41.000000 jmespath-community-1.1.1/tests/legacy/test_lexer.py
+drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1113 2023-03-30 17:53:04.000000 jmespath-community-1.1.2/LICENSE
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)       35 2023-03-30 17:53:04.000000 jmespath-community-1.1.2/MANIFEST.in
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)    10906 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/PKG-INFO
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     7884 2023-02-26 10:33:47.000000 jmespath-community-1.1.2/README.rst
+drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/bin/
+-rwxr-xr-x   0 springcomp  (1000) springcomp  (1000)     1814 2023-02-26 18:24:57.000000 jmespath-community-1.1.2/bin/jp.py
+drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/jmespath/
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)      307 2023-04-30 23:55:03.000000 jmespath-community-1.1.2/jmespath/__init__.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     2736 2023-04-30 23:01:55.000000 jmespath-community-1.1.2/jmespath/ast.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)      369 2023-02-26 10:33:43.000000 jmespath-community-1.1.2/jmespath/compat.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     4794 2023-04-30 23:01:55.000000 jmespath-community-1.1.2/jmespath/exceptions.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)    19822 2023-04-30 23:01:55.000000 jmespath-community-1.1.2/jmespath/functions.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)    10614 2023-04-30 23:01:55.000000 jmespath-community-1.1.2/jmespath/lexer.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)    21644 2023-04-30 23:01:55.000000 jmespath-community-1.1.2/jmespath/parser.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1417 2023-04-30 23:01:55.000000 jmespath-community-1.1.2/jmespath/scope.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)    13710 2023-04-30 23:54:38.000000 jmespath-community-1.1.2/jmespath/visitor.py
+drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/jmespath_community.egg-info/
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)    10906 2023-05-01 00:20:41.000000 jmespath-community-1.1.2/jmespath_community.egg-info/PKG-INFO
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)      455 2023-05-01 00:20:41.000000 jmespath-community-1.1.2/jmespath_community.egg-info/SOURCES.txt
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)        1 2023-05-01 00:20:41.000000 jmespath-community-1.1.2/jmespath_community.egg-info/dependency_links.txt
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)       15 2023-05-01 00:20:41.000000 jmespath-community-1.1.2/jmespath_community.egg-info/top_level.txt
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)      102 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/setup.cfg
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1242 2023-04-30 23:55:03.000000 jmespath-community-1.1.2/setup.py
+drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/tests/
+drwxr-xr-x   0 springcomp  (1000) springcomp  (1000)        0 2023-05-01 00:20:41.414731 jmespath-community-1.1.2/tests/legacy/
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)       16 2023-02-26 10:33:43.000000 jmespath-community-1.1.2/tests/legacy/__init__.py
+-rw-r--r--   0 springcomp  (1000) springcomp  (1000)     1301 2023-02-26 10:33:43.000000 jmespath-community-1.1.2/tests/legacy/test_lexer.py
```

### Comparing `jmespath-community-1.1.1/LICENSE` & `jmespath-community-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/PKG-INFO` & `jmespath-community-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: jmespath-community
-Version: 1.1.1
+Version: 1.1.2
 Summary: JSON Matching Expressions
 Home-page: https://github.com/jmespath-community/jmespath.py
 Author: James Saryerwinnie, Springcomp
 Author-email: js@jamesls.com, springcomp@users.noreply.github.com
 License: MIT
 Description: JMESPath Community
         ==================
```

### Comparing `jmespath-community-1.1.1/README.rst` & `jmespath-community-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/bin/jp.py` & `jmespath-community-1.1.2/bin/jp.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/ast.py` & `jmespath-community-1.1.2/jmespath/ast.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/exceptions.py` & `jmespath-community-1.1.2/jmespath/exceptions.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/functions.py` & `jmespath-community-1.1.2/jmespath/functions.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/lexer.py` & `jmespath-community-1.1.2/jmespath/lexer.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/parser.py` & `jmespath-community-1.1.2/jmespath/parser.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/scope.py` & `jmespath-community-1.1.2/jmespath/scope.py`

 * *Files identical despite different names*

### Comparing `jmespath-community-1.1.1/jmespath/visitor.py` & `jmespath-community-1.1.2/jmespath/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,17 @@
         first_child = node['children'][0]
         if first_child['type'] == 'index_expression':
             nested_children = first_child['children']
             if len(nested_children) > 1 and nested_children[1]['type'] == 'slice':
                 allow_string = True
 
         if isinstance(base, string_type) and allow_string:
-            return base
+            ## projections are really sub-expressions in disguise
+            ## evaluate the rhs when lhs is a sliced string
+            return self.visit(node['children'][1], base)
 
         if not isinstance(base, list):
             return None
         collected = []
         for element in base:
             current = self.visit(node['children'][1], element)
             if current is not None:
```

### Comparing `jmespath-community-1.1.1/jmespath_community.egg-info/PKG-INFO` & `jmespath-community-1.1.2/jmespath_community.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: jmespath-community
-Version: 1.1.1
+Version: 1.1.2
 Summary: JSON Matching Expressions
 Home-page: https://github.com/jmespath-community/jmespath.py
 Author: James Saryerwinnie, Springcomp
 Author-email: js@jamesls.com, springcomp@users.noreply.github.com
 License: MIT
 Description: JMESPath Community
         ==================
```

### Comparing `jmespath-community-1.1.1/setup.py` & `jmespath-community-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='jmespath-community',
-    version='1.1.1',
+    version='1.1.2',
     description='JSON Matching Expressions',
     long_description=io.open('README.rst', encoding='utf-8').read(),
     author='James Saryerwinnie, Springcomp',
     author_email='js@jamesls.com, springcomp@users.noreply.github.com',
     url='https://github.com/jmespath-community/jmespath.py',
     scripts=['bin/jp.py'],
     packages=find_packages(exclude=['tests']),
```

### Comparing `jmespath-community-1.1.1/tests/legacy/test_lexer.py` & `jmespath-community-1.1.2/tests/legacy/test_lexer.py`

 * *Files identical despite different names*

