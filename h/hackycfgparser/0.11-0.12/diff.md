# Comparing `tmp/hackycfgparser-0.11.tar.gz` & `tmp/hackycfgparser-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackycfgparser-0.11.tar", last modified: Mon May  1 02:02:08 2023, max compression
+gzip compressed data, was "hackycfgparser-0.12.tar", last modified: Mon May  1 02:46:46 2023, max compression
```

## Comparing `hackycfgparser-0.11.tar` & `hackycfgparser-0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 02:02:08.789382 hackycfgparser-0.11/
--rw-rw-rw-   0        0        0     1148 2023-05-01 02:01:56.000000 hackycfgparser-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      145 2023-05-01 02:01:55.000000 hackycfgparser-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     5243 2023-05-01 02:02:08.790379 hackycfgparser-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     4542 2023-04-29 11:11:28.000000 hackycfgparser-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 02:02:08.785376 hackycfgparser-0.11/hackycfgparser/
--rw-rw-rw-   0        0        0     1148 2023-04-29 11:11:28.000000 hackycfgparser-0.11/hackycfgparser/LICENSE
--rw-rw-rw-   0        0        0     4542 2023-04-29 11:11:28.000000 hackycfgparser-0.11/hackycfgparser/README.md
--rw-rw-rw-   0        0        0    10177 2023-05-01 01:56:55.000000 hackycfgparser-0.11/hackycfgparser/__init__.py
--rw-rw-rw-   0        0        0       73 2023-05-01 02:02:06.000000 hackycfgparser-0.11/hackycfgparser/requirements.txt
--rw-rw-rw-   0        0        0     1249 2023-05-01 02:02:06.000000 hackycfgparser-0.11/hackycfgparser/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-01 02:02:08.789382 hackycfgparser-0.11/hackycfgparser.egg-info/
--rw-rw-rw-   0        0        0     5243 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-01 02:02:08.000000 hackycfgparser-0.11/hackycfgparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-01 02:02:08.790379 hackycfgparser-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1519 2023-05-01 02:02:06.000000 hackycfgparser-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:46:46.683095 hackycfgparser-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-05-01 02:46:39.000000 hackycfgparser-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      145 2023-05-01 02:46:39.000000 hackycfgparser-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     5243 2023-05-01 02:46:46.683095 hackycfgparser-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     4542 2023-05-01 02:04:50.000000 hackycfgparser-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 02:46:46.678107 hackycfgparser-0.12/hackycfgparser/
+-rw-rw-rw-   0        0        0     1148 2023-05-01 02:04:50.000000 hackycfgparser-0.12/hackycfgparser/LICENSE
+-rw-rw-rw-   0        0        0     4542 2023-05-01 02:04:50.000000 hackycfgparser-0.12/hackycfgparser/README.md
+-rw-rw-rw-   0        0        0    10562 2023-05-01 02:45:50.000000 hackycfgparser-0.12/hackycfgparser/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-05-01 02:46:45.000000 hackycfgparser-0.12/hackycfgparser/requirements.txt
+-rw-rw-rw-   0        0        0     1249 2023-05-01 02:46:45.000000 hackycfgparser-0.12/hackycfgparser/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-01 02:46:46.682097 hackycfgparser-0.12/hackycfgparser.egg-info/
+-rw-rw-rw-   0        0        0     5243 2023-05-01 02:46:46.000000 hackycfgparser-0.12/hackycfgparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-05-01 02:46:46.000000 hackycfgparser-0.12/hackycfgparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:46:46.000000 hackycfgparser-0.12/hackycfgparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-01 02:46:46.000000 hackycfgparser-0.12/hackycfgparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-01 02:46:46.000000 hackycfgparser-0.12/hackycfgparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-01 02:46:46.684091 hackycfgparser-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2023-05-01 02:46:45.000000 hackycfgparser-0.12/setup.py
```

### Comparing `hackycfgparser-0.11/LICENSE.rst` & `hackycfgparser-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.11/PKG-INFO` & `hackycfgparser-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackycfgparser
-Version: 0.11
+Version: 0.12
 Summary: Hacky config parser - parses ConfigParser-compatible files / sys.argv and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackycfgparser
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: hacky,config,parser,decorator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hackycfgparser-0.11/README.md` & `hackycfgparser-0.12/README.md`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.11/hackycfgparser/LICENSE` & `hackycfgparser-0.12/hackycfgparser/LICENSE`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.11/hackycfgparser/README.md` & `hackycfgparser-0.12/hackycfgparser/README.md`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.11/hackycfgparser/__init__.py` & `hackycfgparser-0.12/hackycfgparser/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 from tolerant_isinstance import isinstance_tolerant
 from deepcopyall import deepcopy
 import os
 import sys
 from ast import literal_eval
 from functools import wraps
 from itertools import tee
-
 nested_dict = lambda: defaultdict(nested_dict)
 config = sys.modules[__name__]
 config.parsedargs = {}
 config.helptext = ""
 config.stop_after_kill = True
-
+config.sysargvcopy = []
 
 def load_config_file_vars(cfgfile: str, onezeroasboolean: bool = False) -> None:
     """
     Loads the variables in the specified configuration file and sets them as global variables.
 
     Args:
     - cfgfile (str): The path of the configuration file to load.
@@ -32,27 +31,36 @@
         respectively (default False).
 
     Returns:
     - None
     """
     f = sys._getframe(1)
     dct = f.f_globals
-
     pars2 = ConfigParser()
     pars2.read(cfgfile)
 
     (
         cfgdictcopy,
         cfgdictcopyaslist,
     ) = copy_dict_and_convert_values(pars2, onezeroasboolean=onezeroasboolean)
 
     if "sys" not in dct:
         dct["sys"] = importlib.import_module("sys")
+    config.sysargvcopy.extend(dct['sys'].argv)
     for key, item in cfgdictcopyaslist:
-        dct["sys"].argv.extend([f"--{item[-1]}",  (base64.b16encode(ascii(str(key )).encode('utf-8')[1:-1]).decode('utf-8'))])
+        dct["sys"].argv.extend(
+            [
+                f"--{item[-1]}",
+                (
+                    base64.b16encode(ascii(str(key)).encode("utf-8")[1:-1]).decode(
+                        "utf-8"
+                    )
+                ),
+            ]
+        )
     config.allsysargs = [
         ini for ini, x in enumerate(dct["sys"].argv) if x.startswith("--")
     ]
     parse_ar()
 
 
 def convert_to_normal_dict(di: dict) -> dict:
@@ -211,19 +219,22 @@
 
 
 def parse_ar() -> None:
     ges = list(iter_split_by_index(iterable=sys.argv, indexes=config.allsysargs))
     checkset = ("-?", "?", "-h", "--h", "help", "-help", "--help")
 
     for ini, gg in enumerate(ges[1:]):
-        g = [gg[0], base64.b16decode(gg[1]).decode('utf-8')]
         try:
-            g = [g[0], ast.literal_eval(g[1])]
+            g = [gg[0], base64.b16decode(gg[1]).decode("utf-8")]
+            try:
+                g = [g[0], ast.literal_eval(g[1])]
+            except Exception:
+                pass
         except Exception:
-            pass
+            g = gg
         try:
             there = g[0] in checkset
             if there:
                 raise ValueError
             config.parsedargs[g[0].lstrip("- ")] = g[1]
         except Exception:
             show_and_exit()
@@ -290,8 +301,10 @@
                 "__defaults__",
                 tuple(newargs),
             )
             return func(*args, **kwargs)
 
         return wrapper
 
+    dct['sys'].argv.clear()
+    dct['sys'].argv.extend(config.sysargvcopy)
     return _decorator(f_py) if callable(f_py) else _decorator
```

### Comparing `hackycfgparser-0.11/hackycfgparser/thirdparty.json` & `hackycfgparser-0.12/hackycfgparser/thirdparty.json`

 * *Files identical despite different names*

### Comparing `hackycfgparser-0.11/hackycfgparser.egg-info/PKG-INFO` & `hackycfgparser-0.12/hackycfgparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackycfgparser
-Version: 0.11
+Version: 0.12
 Summary: Hacky config parser - parses ConfigParser-compatible files / sys.argv and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackycfgparser
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: hacky,config,parser,decorator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hackycfgparser-0.11/setup.py` & `hackycfgparser-0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Hacky config parser - parses ConfigParser-compatible files / sys.argv and changes the defaults of functions'''
 
 # Setting up
 setup(
     name="hackycfgparser",
     version=VERSION,
     license='MIT',
```

