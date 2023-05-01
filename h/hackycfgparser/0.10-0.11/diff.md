# Comparing `tmp/hackycfgparser-0.10.tar.gz` & `tmp/hackycfgparser-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackycfgparser-0.10.tar", last modified: Sat Apr 29 11:05:14 2023, max compression
+gzip compressed data, was "hackycfgparser-0.11.tar", last modified: Mon May  1 02:02:08 2023, max compression
```

## Comparing `hackycfgparser-0.10.tar` & `hackycfgparser-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:05:14.354785 hackycfgparser-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-29 11:05:07.000000 hackycfgparser-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      145 2023-04-29 11:05:06.000000 hackycfgparser-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     5243 2023-04-29 11:05:14.355782 hackycfgparser-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     4542 2023-04-29 11:03:09.000000 hackycfgparser-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:05:14.346776 hackycfgparser-0.10/hackycfgparser/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 hackycfgparser-0.10/hackycfgparser/LICENSE
--rw-rw-rw-   0        0        0     4542 2023-04-29 11:03:09.000000 hackycfgparser-0.10/hackycfgparser/README.md
--rw-rw-rw-   0        0        0     9923 2023-04-29 10:36:55.000000 hackycfgparser-0.10/hackycfgparser/__init__.py
--rw-rw-rw-   0        0        0       73 2023-04-29 11:05:12.000000 hackycfgparser-0.10/hackycfgparser/requirements.txt
--rw-rw-rw-   0        0        0     1249 2023-04-29 11:05:12.000000 hackycfgparser-0.10/hackycfgparser/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-29 11:05:14.353862 hackycfgparser-0.10/hackycfgparser.egg-info/
--rw-rw-rw-   0        0        0     5243 2023-04-29 11:05:13.000000 hackycfgparser-0.10/hackycfgparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-04-29 11:05:14.000000 hackycfgparser-0.10/hackycfgparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:05:13.000000 hackycfgparser-0.10/hackycfgparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-29 11:05:13.000000 hackycfgparser-0.10/hackycfgparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 11:05:13.000000 hackycfgparser-0.10/hackycfgparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-29 11:05:14.356780 hackycfgparser-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1519 2023-04-29 11:05:12.000000 hackycfgparser-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:02:08.789382 hackycfgparser-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-01 02:01:56.000000 hackycfgparser-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      145 2023-05-01 02:01:55.000000 hackycfgparser-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     5243 2023-05-01 02:02:08.790379 hackycfgparser-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     4542 2023-04-29 11:11:28.000000 hackycfgparser-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 02:02:08.785376 hackycfgparser-0.11/hackycfgparser/
+-rw-rw-rw-   0        0        0     1148 2023-04-29 11:11:28.000000 hackycfgparser-0.11/hackycfgparser/LICENSE
+-rw-rw-rw-   0        0        0     4542 2023-04-29 11:11:28.000000 hackycfgparser-0.11/hackycfgparser/README.md
+-rw-rw-rw-   0        0        0    10177 2023-05-01 01:56:55.000000 hackycfgparser-0.11/hackycfgparser/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-05-01 02:02:06.000000 hackycfgparser-0.11/hackycfgparser/requirements.txt
+-rw-rw-rw-   0        0        0     1249 2023-05-01 02:02:06.000000 hackycfgparser-0.11/hackycfgparser/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-01 02:02:08.789382 hackycfgparser-0.11/hackycfgparser.egg-info/
+-rw-rw-rw-   0        0        0     5243 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-01 02:02:08.790379 hackycfgparser-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2023-05-01 02:02:06.000000 hackycfgparser-0.11/setup.py
```

### Comparing `hackycfgparser-0.10/LICENSE.rst` & `hackycfgparser-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.10/PKG-INFO` & `hackycfgparser-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackycfgparser
-Version: 0.10
+Version: 0.11
 Summary: Hacky config parser - parses ConfigParser-compatible files / sys.argv and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackycfgparser
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: hacky,config,parser,decorator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hackycfgparser-0.10/README.md` & `hackycfgparser-0.11/README.md`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.10/hackycfgparser/LICENSE` & `hackycfgparser-0.11/hackycfgparser/LICENSE`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.10/hackycfgparser/README.md` & `hackycfgparser-0.11/hackycfgparser/README.md`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.10/hackycfgparser/__init__.py` & `hackycfgparser-0.11/hackycfgparser/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import base64
 import importlib
 from collections import defaultdict
 from functools import reduce
 from configparser import ConfigParser
 import re
 from typing import Iterable
 from flatten_any_dict_iterable_or_whatsoever import fla_tu, set_in_original_iter
@@ -39,22 +40,22 @@
     pars2 = ConfigParser()
     pars2.read(cfgfile)
 
     (
         cfgdictcopy,
         cfgdictcopyaslist,
     ) = copy_dict_and_convert_values(pars2, onezeroasboolean=onezeroasboolean)
+
     if "sys" not in dct:
         dct["sys"] = importlib.import_module("sys")
     for key, item in cfgdictcopyaslist:
-        dct["sys"].argv.extend([f"--{item[-1]}", repr(key)])
+        dct["sys"].argv.extend([f"--{item[-1]}",  (base64.b16encode(ascii(str(key )).encode('utf-8')[1:-1]).decode('utf-8'))])
     config.allsysargs = [
-        ini for ini, x in enumerate(dct["sys"].argv) if x.startswith("-")
+        ini for ini, x in enumerate(dct["sys"].argv) if x.startswith("--")
     ]
-
     parse_ar()
 
 
 def convert_to_normal_dict(di: dict) -> dict:
     """
     Recursively converts the input dictionary to a normal dictionary (i.e., non-defaultdict) by copying its contents.
 
@@ -208,15 +209,21 @@
     finally:
         os._exit(1)
 
 
 def parse_ar() -> None:
     ges = list(iter_split_by_index(iterable=sys.argv, indexes=config.allsysargs))
     checkset = ("-?", "?", "-h", "--h", "help", "-help", "--help")
-    for ini, g in enumerate(ges[1:]):
+
+    for ini, gg in enumerate(ges[1:]):
+        g = [gg[0], base64.b16decode(gg[1]).decode('utf-8')]
+        try:
+            g = [g[0], ast.literal_eval(g[1])]
+        except Exception:
+            pass
         try:
             there = g[0] in checkset
             if there:
                 raise ValueError
             config.parsedargs[g[0].lstrip("- ")] = g[1]
         except Exception:
             show_and_exit()
```

### Comparing `hackycfgparser-0.10/hackycfgparser/thirdparty.json` & `hackycfgparser-0.11/hackycfgparser/thirdparty.json`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.10/hackycfgparser.egg-info/PKG-INFO` & `hackycfgparser-0.11/hackycfgparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackycfgparser
-Version: 0.10
+Version: 0.11
 Summary: Hacky config parser - parses ConfigParser-compatible files / sys.argv and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackycfgparser
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: hacky,config,parser,decorator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hackycfgparser-0.10/setup.py` & `hackycfgparser-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Hacky config parser - parses ConfigParser-compatible files / sys.argv and changes the defaults of functions'''
 
 # Setting up
 setup(
     name="hackycfgparser",
     version=VERSION,
     license='MIT',
```

