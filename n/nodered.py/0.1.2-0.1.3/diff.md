# Comparing `tmp/nodered.py-0.1.2.tar.gz` & `tmp/nodered.py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.1.2.tar", last modified: Sun Apr 30 05:01:13 2023, max compression
+gzip compressed data, was "nodered.py-0.1.3.tar", last modified: Mon May  1 13:26:39 2023, max compression
```

## Comparing `nodered.py-0.1.2.tar` & `nodered.py-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.360000 nodered.py-0.1.2/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.2/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-04-30 05:01:13.450000 nodered.py-0.1.2/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1758 2023-04-30 04:58:00.000000 nodered.py-0.1.2/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.360000 nodered.py-0.1.2/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      435 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       37 2023-04-30 05:01:13.000000 nodered.py-0.1.2/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.2/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.360000 nodered.py-0.1.2/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      466 2023-04-30 03:51:45.000000 nodered.py-0.1.2/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7628 2023-04-30 04:22:32.000000 nodered.py-0.1.2/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3357 2023-04-30 04:55:12.000000 nodered.py-0.1.2/noderedpy/_property.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6410 2023-04-30 03:53:02.000000 nodered.py-0.1.2/noderedpy/_server.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    10303 2023-04-30 04:47:34.000000 nodered.py-0.1.2/noderedpy/_templates.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      805 2023-04-30 03:52:23.000000 nodered.py-0.1.2/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-30 05:01:13.370000 nodered.py-0.1.2/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.2/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.2/noderedpy/node-red-starter/package.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-04-30 05:01:13.450000 nodered.py-0.1.2/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1044 2023-04-28 05:53:24.000000 nodered.py-0.1.2/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.3/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-01 13:26:39.670000 nodered.py-0.1.3/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1758 2023-04-30 04:58:00.000000 nodered.py-0.1.3/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      543 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       57 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.3/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      466 2023-05-01 12:55:57.000000 nodered.py-0.1.3/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5580 2023-05-01 13:06:41.000000 nodered.py-0.1.3/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3457 2023-05-01 13:22:01.000000 nodered.py-0.1.3/noderedpy/_property.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6410 2023-04-30 03:53:02.000000 nodered.py-0.1.3/noderedpy/_server.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      805 2023-04-30 03:52:23.000000 nodered.py-0.1.3/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.3/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.3/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7123 2023-05-01 13:22:31.000000 nodered.py-0.1.3/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      971 2023-05-01 13:00:37.000000 nodered.py-0.1.3/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3212 2023-05-01 13:01:59.000000 nodered.py-0.1.3/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      269 2023-05-01 13:03:04.000000 nodered.py-0.1.3/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-01 13:26:39.670000 nodered.py-0.1.3/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1077 2023-05-01 12:49:35.000000 nodered.py-0.1.3/setup.py
```

### Comparing `nodered.py-0.1.2/LICENSE` & `nodered.py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.2/PKG-INFO` & `nodered.py-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.2 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.3 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.1.2/README.md` & `nodered.py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.2/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.1.3/nodered.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.2 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.3 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.1.2/noderedpy/_nodered.py` & `nodered.py-0.1.3/noderedpy/_nodered.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import os, sys, subprocess, threading, traceback, noderedpy
 from types import MethodType
-from typing import Type, Literal, Any, List
-from ._templates import package_json, node_html, node_js
+from typing import Type, List
+from .templates import package_json, node_html, node_js
 from ._property import Property
 from . import __path__
 
 
 class RED:
     """
     Node-RED manager class
@@ -123,67 +123,14 @@
         Stop Node-RED server
         """
         if os.path.exists(self.__started_file):
             os.remove(self.__started_file)
 
         self.__stop()
 
-
-# class NodeProperty:
-#     """
-#     Property for Node function
-#     """
-#     def __init__(self, name:str, type:Literal["str", "int", "float", "list", "dict"], default_value:Any = None, required:bool = False, display_icon:str = None):
-#         """
-#         Property information for Node function
-
-#         Parameters
-#         ----------
-#         name: str, required
-#             name of Property
-#         type: Literal["str", "int", "float"], required
-#             type of Property
-#         default_value: Any, default None
-#             default value of Property
-#         required: bool, default False
-#             set Property is required or not
-#         display_icon: str, default None
-#             icon for Node-RED node display
-#         """
-#         if " " in name.strip():
-#             raise NameError("Property name cannot contain space!")
-        
-#         if not type in ("str", "int", "float", "list", "dict"):
-#             raise TypeError("Currently supported types: [ 'str', 'int', 'float', 'list', 'dict' ]")
-        
-#         if default_value is not None and not isinstance(default_value, ( str, int, float, list, dict )):
-#             raise TypeError("Currently supported value types: [ str, int, float, list, dict ]")
-
-#         self.name, self.type, self.default_value, self.required =\
-#             name, type, default_value, required
-        
-#         if display_icon is None:
-#             if type in ( "int", "float" ):
-#                 self.display_icon = "fa fa-sort-numeric-asc"
-#             elif type == "str":
-#                 self.display_icon = "fa fa-font"
-#             elif type == "list":
-#                 self.display_icon = "fa fa-list"
-#             elif type == "dict":
-#                 self.display_icon = "fa fa-code"
-#         else:
-#             self.display_icon = display_icon
-        
-#     @property
-#     def display_name(self) -> str:
-#         return " ".join([
-#             item.capitalize()
-#             for item in self.name.split("_")
-#         ])
-
 class Node:
     def __init__(self, name:str, category:str, properties:List[Property], node_func:MethodType):
         if " " in name.strip():
             raise NameError("Node name cannot contain spaces!")
         
         if "-" in category.strip() or "," in category.strip():
             raise NameError("Category cannot contain '-' or ','!")
```

### Comparing `nodered.py-0.1.2/noderedpy/_property.py` & `nodered.py-0.1.3/noderedpy/_property.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,43 +36,45 @@
                 self.display_icon = "fa fa-sort-numeric-asc"
             else:
                 self.display_icon = "fa fa-font"
         else:
             self.display_icon = display_icon
 
 class ListProperty(Property):
-    def __init__(self, name:str, default:list = [], required:bool = False, display_icon:str = None):
+    def __init__(self, name:str, default:list = [], height:int = 250, required:bool = False, display_icon:str = None):
         if not isinstance(default, list):
             raise TypeError("ListProperty can accept type: 'list'")
 
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-list-ul")
+        self.height = height
 
 class DictProperty(Property):
-    def __init__(self, name:str, default:Union[dict, str] = {}, required:bool = False, display_icon:str = None):
+    def __init__(self, name:str, default:Union[dict, str] = {}, height:int = 250, required:bool = False, display_icon:str = None):
         if not isinstance(default, ( dict, str )):
             raise TypeError("DictProperty can accept types: [ 'dict', 'json string' ]")
         
         if isinstance(default, str):
             if not default.strip().startswith("{") or not default.strip().endswith("}"):
                 raise ValueError("DictProperty value must be 'dict' or 'json string'!")
 
             try:
                 json.loads(default)
             except:
                 raise ValueError("DictProperty value must be 'dict' or 'json string'!")
         
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-code")
+        self.height = height
 
 class SpinnerProperty(Property):
-    def __init__(self, name:str, default:float = 0, step:float = 1, min:float = 0, max:float = 1000, required:bool = False, display_icon:str = None):
+    def __init__(self, name:str, default:float = 0, step:float = None, min:float = None, max:float = None, required:bool = False, display_icon:str = None):
         if not isinstance(default, (int, float)):
             raise TypeError("SpinnerProperty can accept types: [ 'int', 'float' ]")
 
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-random")
-        self.setp, self.min, self.max =\
+        self.step, self.min, self.max =\
             step, min, max
 
 class ComboBoxProperty(Property):
     def __init__(self, name:str, items:List[Any], default:str = None, required:bool = False, display_icon:str = None):
         if not isinstance(items, list):
             raise TypeError("items of ComboBoxProperty must be type: 'list'")
```

### Comparing `nodered.py-0.1.2/noderedpy/_server.py` & `nodered.py-0.1.3/noderedpy/_server.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.2/noderedpy/decorator.py` & `nodered.py-0.1.3/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.2/noderedpy/node-red-starter/index.js` & `nodered.py-0.1.3/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.2/setup.py` & `nodered.py-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     setup_requires = requires,
     license = "MIT license",
     description = "make python function to Node-RED node",
     long_description = readme,
     long_description_content_type = "text/markdown",
     # package informations
     packages = [
-        "noderedpy", "noderedpy/node-red-starter"
+        "noderedpy", "noderedpy/templates", "noderedpy/node-red-starter"
     ],
     package_data = {
         "": [
-            "*.js", "*.json"
+            "*.html", "*.js", "*.json"
         ]
     },
     include_package_data = True,
     zip_safe = True
 )
```

