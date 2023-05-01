# Comparing `tmp/pyzconf-0.1.0.tar.gz` & `tmp/pyzconf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzconf-0.1.0.tar", max compression
+gzip compressed data, was "pyzconf-0.1.2.tar", max compression
```

## Comparing `pyzconf-0.1.0.tar` & `pyzconf-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-05-01 10:12:12.618106 pyzconf-0.1.0/LICENSE
--rw-r--r--   0        0        0       73 2023-05-01 10:12:12.618266 pyzconf-0.1.0/README.md
--rw-r--r--   0        0        0      364 2023-05-01 10:31:30.793203 pyzconf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 10:13:01.855394 pyzconf-0.1.0/zconf/__init__.py
--rw-r--r--   0        0        0     2604 2023-05-01 10:21:27.894290 pyzconf-0.1.0/zconf/zconf.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pyzconf-0.1.0/setup.py
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 pyzconf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-01 10:12:12.618106 pyzconf-0.1.2/LICENSE
+-rw-r--r--   0        0        0       73 2023-05-01 10:12:12.618266 pyzconf-0.1.2/README.md
+-rw-r--r--   0        0        0      364 2023-05-01 10:53:32.617487 pyzconf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 10:13:01.855394 pyzconf-0.1.2/zconf/__init__.py
+-rw-r--r--   0        0        0     2569 2023-05-01 10:48:25.161711 pyzconf-0.1.2/zconf/zconf.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pyzconf-0.1.2/setup.py
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 pyzconf-0.1.2/PKG-INFO
```

### Comparing `pyzconf-0.1.0/LICENSE` & `pyzconf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzconf-0.1.0/zconf/zconf.py` & `pyzconf-0.1.2/zconf/zconf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-class zconf(object):
-    from typing import Tuple, Union
-    import os
+from typing import Tuple, Union
+import os
 
-    from dfl.dfl import dfl_tools
+from dfl.dfl import dfl_tools
+
+from dotenv import load_dotenv
+import omegaconf
+
+
+class zconf(object):
 
-    from dotenv import load_dotenv
-    import omegaconf
-    
-    
     def __init__(
         self,
         zconf_path: str="",
         zconf_id: str=""
     ) -> None:
         
         load_dotenv()
@@ -95,11 +96,11 @@
         target: any,
         name: str,
         other: any
     ) -> any:
         
         _ret = None
         
-        if name != None in target:
+        if name in target:
             _ret = target[name] if target[name] != None else other
             
         return _ret
```

### Comparing `pyzconf-0.1.0/setup.py` & `pyzconf-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['omegaconf>=2.3.0,<3.0.0',
  'pydfl>=0.1.0,<0.2.0',
  'python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyzconf',
-    'version': '0.1.0',
+    'version': '0.1.2',
     'description': '',
     'long_description': '# zconf\nEasy configurations to python classes variables with conf files.\n',
     'author': 'Doohoon Kim',
     'author_email': 'invi.dh.kim@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyzconf-0.1.0/PKG-INFO` & `pyzconf-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzconf
-Version: 0.1.0
+Version: 0.1.2
 Summary: 
 Author: Doohoon Kim
 Author-email: invi.dh.kim@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

