# Comparing `tmp/wynntilsresolver-0.1.1.tar.gz` & `tmp/wynntilsresolver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wynntilsresolver-0.1.1.tar", last modified: Mon May  1 16:00:49 2023, max compression
+gzip compressed data, was "wynntilsresolver-0.1.2.tar", last modified: Mon May  1 16:34:34 2023, max compression
```

## Comparing `wynntilsresolver-0.1.1.tar` & `wynntilsresolver-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1087 2023-05-01 15:17:38.959920 wynntilsresolver-0.1.1/LICENSE
--rw-r--r--   0        0        0     1182 2023-05-01 16:00:49.269107 wynntilsresolver-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      831 2023-05-01 15:33:12.782134 wynntilsresolver-0.1.1/readme.md
--rw-r--r--   0        0        0      106 2023-05-01 13:36:20.127759 wynntilsresolver-0.1.1/src/wynntilsresolver/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 15:21:08.556117 wynntilsresolver-0.1.1/src/wynntilsresolver/cli.py
--rw-r--r--   0        0        0      105 2023-05-01 14:01:24.386186 wynntilsresolver-0.1.1/src/wynntilsresolver/exceptions.py
--rw-r--r--   0        0        0      553 2023-05-01 15:32:27.978149 wynntilsresolver-0.1.1/src/wynntilsresolver/model.py
--rw-r--r--   0        0        0     2494 2023-05-01 15:30:04.642268 wynntilsresolver-0.1.1/src/wynntilsresolver/resolver.py
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-01 15:17:38.959920 wynntilsresolver-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1182 2023-05-01 16:34:34.821452 wynntilsresolver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1027 2023-05-01 16:34:03.990841 wynntilsresolver-0.1.2/readme.md
+-rw-r--r--   0        0        0      175 2023-05-01 16:22:08.595090 wynntilsresolver-0.1.2/src/wynntilsresolver/__init__.py
+-rw-r--r--   0        0        0       56 2023-05-01 16:22:26.308970 wynntilsresolver-0.1.2/src/wynntilsresolver/cli.py
+-rw-r--r--   0        0        0      105 2023-05-01 14:01:24.386186 wynntilsresolver-0.1.2/src/wynntilsresolver/exceptions.py
+-rw-r--r--   0        0        0     1353 2023-05-01 16:32:58.505158 wynntilsresolver-0.1.2/src/wynntilsresolver/model.py
+-rw-r--r--   0        0        0     2527 2023-05-01 16:31:02.130980 wynntilsresolver-0.1.2/src/wynntilsresolver/resolver.py
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.2/PKG-INFO
```

### Comparing `wynntilsresolver-0.1.1/LICENSE` & `wynntilsresolver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-0.1.1/pyproject.toml` & `wynntilsresolver-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "WynntilsResolver"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple resolver to analyze wynntils' encoded equipment in chat."
 authors = [
     { name = "FYWinds", email = "i@windis.cn" },
 ]
 dependencies = [
     "typer[all]==0.8.0",
 ]
```

### Comparing `wynntilsresolver-0.1.1/src/wynntilsresolver/resolver.py` & `wynntilsresolver-0.1.2/src/wynntilsresolver/resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 FilePath     : /wynntilsresolver/resolver.py
 
 Copyright (c) 2023 by FYWinds
 All Rights Reserved.
 Any modifications or distributions of the file
 should mark the original author's name.
 """
-import dataclasses
 import math
 import re
 from re import Pattern
+import json
 
 from .exceptions import ItemNotValidError
-from .model import Item, Powder
+from .model import Item, Powder, CustomeEncoder
 
 _START = chr(0xF5FF0)
 _END = chr(0xF5FF1)
 _SEP = chr(0xF5FF2)
 _RANGE = "[" + chr(0xF5000) + "-" + chr(0xF5F00) + "]"
 _OFFSET = chr(0xF5000)
 
@@ -56,15 +56,15 @@
             rerolls = self._decode_numbers(m.group("Rerolls"))[0]
             ids = [((i / 4) + 30) / 100 for i in ids]  # id rolls from 0.3 to 1.3
             return Item(name, ids, self._decode_powders(powders), rerolls)
         else:
             raise ItemNotValidError(f"Given text {text} is not a valid encoded item.")
 
     def decode_to_json(self, text) -> dict:
-        return dataclasses.asdict(self.decode(text))
+        return json.loads(json.dumps(self.decode(text), cls=CustomeEncoder))
 
     def _decode_powders(self, powders: list[int]) -> list[Powder]:
         powders.reverse()
         plist = []
         for powderNum in powders:
             while powderNum > 0:
                 plist.append(Powder(powderNum % 6 - 1))
```

### Comparing `wynntilsresolver-0.1.1/PKG-INFO` & `wynntilsresolver-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wynntilsresolver
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple resolver to analyze wynntils' encoded equipment in chat.
 Keywords: wynntils resolver wynncraft
 Author-Email: FYWinds <i@windis.cn>
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -34,15 +34,17 @@
 
 Use as a package
 
 ```python
 from wynntilsresolver import resolver
 
 print(resolver.decode("󵿰Warp󵿲󵃨󵄴󵁤󵀠󵁤󵂄󵅥󵀀󵃌󵿲󵃗󵀄󵿱"))
-# Item(name='Warp', ids=[0.88, 1.07, 0.55, 0.38, 0.55, 0.63, 1.1925, 0.3, 0.81], powders=[<Powder.AIR: 4>, <Powder.AIR: 4>, <Powder.AIR: 4>], rerolls=4)
+# Item(name='Warp', ids=[0.88, 1.07, 0.55, 0.38, 0.55, 0.63, 1.1925, 0.3, 0.81], powders=[AIR, AIR, AIR], rerolls=4)
+print(resolver.decode_to_json("󵿰Warp󵿲󵃨󵄴󵁤󵀠󵁤󵂄󵅥󵀀󵃌󵿲󵃗󵀄󵿱"))
+# {'name': 'Warp', 'ids': [0.88, 1.07, 0.55, 0.38, 0.55, 0.63, 1.1925, 0.3, 0.81], 'powders': ['AIR', 'AIR', 'AIR'], 'rerolls': 4}
 ```
 
 Or initialite your own match pattern
 ```python
 import re
 from wynntilsresolver import Resolver
```

