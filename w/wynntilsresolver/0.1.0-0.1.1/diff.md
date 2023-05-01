# Comparing `tmp/wynntilsresolver-0.1.0.tar.gz` & `tmp/wynntilsresolver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wynntilsresolver-0.1.0.tar", last modified: Mon May  1 15:03:50 2023, max compression
+gzip compressed data, was "wynntilsresolver-0.1.1.tar", last modified: Mon May  1 16:00:49 2023, max compression
```

## Comparing `wynntilsresolver-0.1.0.tar` & `wynntilsresolver-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      570 2023-05-01 15:03:50.193952 wynntilsresolver-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      817 2023-05-01 14:47:13.582040 wynntilsresolver-0.1.0/readme.md
--rw-r--r--   0        0        0      106 2023-05-01 13:36:20.127759 wynntilsresolver-0.1.0/wynntilsresolver/__init__.py
--rw-r--r--   0        0        0      105 2023-05-01 14:01:24.386186 wynntilsresolver-0.1.0/wynntilsresolver/exceptions.py
--rw-r--r--   0        0        0      305 2023-05-01 14:32:52.608390 wynntilsresolver-0.1.0/wynntilsresolver/model.py
--rw-r--r--   0        0        0     2481 2023-05-01 14:43:09.238131 wynntilsresolver-0.1.0/wynntilsresolver/resolver.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-01 15:17:38.959920 wynntilsresolver-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1182 2023-05-01 16:00:49.269107 wynntilsresolver-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      831 2023-05-01 15:33:12.782134 wynntilsresolver-0.1.1/readme.md
+-rw-r--r--   0        0        0      106 2023-05-01 13:36:20.127759 wynntilsresolver-0.1.1/src/wynntilsresolver/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 15:21:08.556117 wynntilsresolver-0.1.1/src/wynntilsresolver/cli.py
+-rw-r--r--   0        0        0      105 2023-05-01 14:01:24.386186 wynntilsresolver-0.1.1/src/wynntilsresolver/exceptions.py
+-rw-r--r--   0        0        0      553 2023-05-01 15:32:27.978149 wynntilsresolver-0.1.1/src/wynntilsresolver/model.py
+-rw-r--r--   0        0        0     2494 2023-05-01 15:30:04.642268 wynntilsresolver-0.1.1/src/wynntilsresolver/resolver.py
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.1/PKG-INFO
```

### Comparing `wynntilsresolver-0.1.0/readme.md` & `wynntilsresolver-0.1.1/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Wynntils Resolver
 ## A simple resolver to anaslyeze wynntils' coded equipment in chat.
 
 ### Built on
 [![Python 3.9](https://img.shields.io/badge/python%203.9-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
 
 ### Install
+```bash
 pip install wynntilsresolver
+```
 
 ### Usage
 
 Use as a package
 
 ```python
 from wynntilsresolver import resolver
```

### Comparing `wynntilsresolver-0.1.0/wynntilsresolver/resolver.py` & `wynntilsresolver-0.1.1/src/wynntilsresolver/resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Author       : FYWinds i@windis.cn
 Date         : 2023-05-01 09:08:08
 LastEditors  : FYWinds i@windis.cn
-LastEditTime : 2023-05-01 10:29:48
-FilePath     : /src/resolver.py
+LastEditTime : 2023-05-01 11:30:04
+FilePath     : /wynntilsresolver/resolver.py
 
 Copyright (c) 2023 by FYWinds
 All Rights Reserved.
 Any modifications or distributions of the file
 should mark the original author's name.
 """
+import dataclasses
+import math
 import re
+from re import Pattern
 
 from .exceptions import ItemNotValidError
-from re import Pattern
 from .model import Item, Powder
-import dataclasses
-import math
 
 _START = chr(0xF5FF0)
 _END = chr(0xF5FF1)
 _SEP = chr(0xF5FF2)
 _RANGE = "[" + chr(0xF5000) + "-" + chr(0xF5F00) + "]"
 _OFFSET = chr(0xF5000)
```

