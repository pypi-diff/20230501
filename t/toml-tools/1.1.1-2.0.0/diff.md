# Comparing `tmp/toml_tools-1.1.1.tar.gz` & `tmp/toml_tools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_tools-1.1.1.tar", last modified: Sun Apr 30 21:27:57 2023, max compression
+gzip compressed data, was "toml_tools-2.0.0.tar", last modified: Mon May  1 19:01:01 2023, max compression
```

## Comparing `toml_tools-1.1.1.tar` & `toml_tools-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.933298 toml_tools-1.1.1/
--rw-rw-rw-   0        0        0     1093 2023-04-29 19:23:43.000000 toml_tools-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       88 2023-04-30 11:09:23.000000 toml_tools-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14844 2023-04-30 21:27:57.934291 toml_tools-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    13885 2023-04-30 21:27:23.000000 toml_tools-1.1.1/README.md
--rw-rw-rw-   0        0        0      115 2023-04-30 21:27:57.937300 toml_tools-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-04-30 21:22:49.000000 toml_tools-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.885291 toml_tools-1.1.1/tests/
--rw-rw-rw-   0        0        0      425 2023-04-30 13:19:52.000000 toml_tools-1.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     4292 2023-04-30 21:03:53.000000 toml_tools-1.1.1/tests/burntsushi.py
--rw-rw-rw-   0        0        0     2750 2023-04-30 14:27:16.000000 toml_tools-1.1.1/tests/test_data.py
--rw-rw-rw-   0        0        0     2290 2023-04-30 13:05:45.000000 toml_tools-1.1.1/tests/test_error.py
--rw-rw-rw-   0        0        0      910 2023-04-30 13:43:35.000000 toml_tools-1.1.1/tests/test_for_profiler.py
--rw-rw-rw-   0        0        0      439 2023-04-30 13:09:48.000000 toml_tools-1.1.1/tests/test_invalid.py
--rw-rw-rw-   0        0        0     3971 2023-04-30 15:41:55.000000 toml_tools-1.1.1/tests/test_misc.py
--rw-rw-rw-   0        0        0     5612 2023-04-30 13:11:25.000000 toml_tools-1.1.1/tests/test_style.py
--rw-rw-rw-   0        0        0      757 2023-04-30 09:56:38.000000 toml_tools-1.1.1/tests/test_types.py
--rw-rw-rw-   0        0        0     2075 2023-04-30 21:09:47.000000 toml_tools-1.1.1/tests/test_valid.py
--rw-rw-rw-   0        0        0      301 2023-04-30 09:56:56.000000 toml_tools-1.1.1/tests/test_write_file.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.901294 toml_tools-1.1.1/toml_tools/
--rw-rw-rw-   0        0        0      421 2023-04-30 21:27:55.000000 toml_tools-1.1.1/toml_tools/__init__.py
--rw-rw-rw-   0        0        0      444 2023-04-29 21:12:30.000000 toml_tools-1.1.1/toml_tools/_helpers.py
--rw-rw-rw-   0        0        0    23870 2023-04-30 15:19:52.000000 toml_tools-1.1.1/toml_tools/_parser.py
--rw-rw-rw-   0        0        0     4285 2023-04-30 14:29:54.000000 toml_tools-1.1.1/toml_tools/_re.py
--rw-rw-rw-   0        0        0     6509 2023-04-30 11:54:56.000000 toml_tools-1.1.1/toml_tools/_writer.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:27:57.931288 toml_tools-1.1.1/toml_tools.egg-info/
--rw-rw-rw-   0        0        0    14844 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 21:27:57.000000 toml_tools-1.1.1/toml_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1271 2023-04-30 21:11:20.000000 toml_tools-1.1.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-01 19:01:01.937484 toml_tools-2.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-04-29 19:23:43.000000 toml_tools-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-04-30 11:09:23.000000 toml_tools-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15227 2023-05-01 19:01:01.939487 toml_tools-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14268 2023-05-01 19:00:17.000000 toml_tools-2.0.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-01 19:01:01.942487 toml_tools-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-05-01 14:39:44.000000 toml_tools-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:01:01.895507 toml_tools-2.0.0/tests/
+-rw-rw-rw-   0        0        0      321 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     7042 2023-05-01 16:46:05.000000 toml_tools-2.0.0/tests/test_data.py
+-rw-rw-rw-   0        0        0     2283 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/test_error.py
+-rw-rw-rw-   0        0        0     1038 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/test_for_profiler.py
+-rw-rw-rw-   0        0        0      522 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/test_invalid.py
+-rw-rw-rw-   0        0        0     4083 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/test_misc.py
+-rw-rw-rw-   0        0        0     7342 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/test_style.py
+-rw-rw-rw-   0        0        0     1007 2023-05-01 14:39:44.000000 toml_tools-2.0.0/tests/test_types.py
+-rw-rw-rw-   0        0        0     3404 2023-05-01 18:50:04.000000 toml_tools-2.0.0/tests/test_valid.py
+-rw-rw-rw-   0        0        0      670 2023-05-01 16:46:05.000000 toml_tools-2.0.0/tests/test_write_file.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:01:01.909489 toml_tools-2.0.0/toml_tools/
+-rw-rw-rw-   0        0        0      449 2023-05-01 14:39:44.000000 toml_tools-2.0.0/toml_tools/__init__.py
+-rw-rw-rw-   0        0        0     1494 2023-05-01 18:13:23.000000 toml_tools-2.0.0/toml_tools/_helpers.py
+-rw-rw-rw-   0        0        0    24206 2023-05-01 16:46:05.000000 toml_tools-2.0.0/toml_tools/_parser.py
+-rw-rw-rw-   0        0        0     4391 2023-05-01 16:11:56.000000 toml_tools-2.0.0/toml_tools/_re.py
+-rw-rw-rw-   0        0        0     6687 2023-05-01 16:39:48.000000 toml_tools-2.0.0/toml_tools/_writer.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:01:01.936491 toml_tools-2.0.0/toml_tools.egg-info/
+-rw-rw-rw-   0        0        0    15227 2023-05-01 19:01:01.000000 toml_tools-2.0.0/toml_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-05-01 19:01:01.000000 toml_tools-2.0.0/toml_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:01:01.000000 toml_tools-2.0.0/toml_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 19:01:01.000000 toml_tools-2.0.0/toml_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1915 2023-05-01 14:47:48.000000 toml_tools-2.0.0/tox.ini
```

### Comparing `toml_tools-1.1.1/LICENSE` & `toml_tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.1/PKG-INFO` & `toml_tools-2.0.0/toml_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: toml_tools
-Version: 1.1.1
+Name: toml-tools
+Version: 2.0.0
 Summary: Tomli and Tomli-W for Python 2 and Iron Python
 Home-page: https://github.com/JamesParrott/toml_tools
 Author: Taneli Hukkinen
 Author-email: hukkin@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,19 +17,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
+# toml_tools: Tomli and Tomli-W for Python 2 and Iron Python
 
-v1.1.1 - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+v2.0.0 
+ - dump and dumps now return an OrderedDict, in Pythons before 3.7 or in IronPython which should preserve the order of entries (other than listing the root table entries first).  
+ - integers and floats can have underscores in in Python 2
+ - Passes 312 tests in each of cPythons 2.7, and 3.7 to 3.12, and in Iron Pythons 2.7 and 3.4.
 
-v1.0.0 is a complete overhaul - toml_tools is now based on tomli and tomli-w.  Note, unlike toml_tools v0, toml and tomlkit, toml_tools v1 and tomli require files to be opened in bytes mode ('rb').
+v1.1.1
+ - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+
+v1.0.0 is a complete overhaul
+ - toml_tools is now based on tomli and tomli-w.  Note unlike toml_tools v0, toml and tomlkit, that both toml_tools v1 and tomli require files to be opened in bytes mode ('rb'), not text mode ('rt').
 
 
 # Parent Project number (1/2)'s Readme File (Tomli)
 
 > A lil' TOML parser
 
 **Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
```

### Comparing `toml_tools-1.1.1/README.md` & `toml_tools-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-# toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
+# toml_tools: Tomli and Tomli-W for Python 2 and Iron Python
 
-v1.1.1 - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+v2.0.0 
+ - dump and dumps now return an OrderedDict, in Pythons before 3.7 or in IronPython which should preserve the order of entries (other than listing the root table entries first).  
+ - integers and floats can have underscores in in Python 2
+ - Passes 312 tests in each of cPythons 2.7, and 3.7 to 3.12, and in Iron Pythons 2.7 and 3.4.
 
-v1.0.0 is a complete overhaul - toml_tools is now based on tomli and tomli-w.  Note, unlike toml_tools v0, toml and tomlkit, toml_tools v1 and tomli require files to be opened in bytes mode ('rb').
+v1.1.1
+ - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+
+v1.0.0 is a complete overhaul
+ - toml_tools is now based on tomli and tomli-w.  Note unlike toml_tools v0, toml and tomlkit, that both toml_tools v1 and tomli require files to be opened in bytes mode ('rb'), not text mode ('rt').
 
 
 # Parent Project number (1/2)'s Readme File (Tomli)
 
 > A lil' TOML parser
 
 **Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
```

### Comparing `toml_tools-1.1.1/setup.py` & `toml_tools-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `toml_tools-1.1.1/tests/test_error.py` & `toml_tools-2.0.0/tests/test_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Taneli Hukkinen
 # Licensed to PSF under a Contributor Agreement.
 
 import unittest
 
-from . import toml_tools
+import toml_tools
 
 
 class TestError(unittest.TestCase):
     def test_line_and_col(self):
         with self.assertRaises(toml_tools.TOMLDecodeError) as exc_info:
             toml_tools.loads("val=.")
         self.assertEqual(str(exc_info.exception), "Invalid value (at line 1, column 5)")
```

### Comparing `toml_tools-1.1.1/tests/test_for_profiler.py` & `toml_tools-2.0.0/tests/test_for_profiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 This test can be useful for profiling, as most of the execution time
 will be spent writing TOML instead of managing pytest execution
 environment. To get and read profiler results:
   - `tox -e profile`
   - `firefox .tox/prof/combined.svg`
 """
 import os
-
-from . import toml_tools
+import unittest
+import toml_tools
 
 
 path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "benchmark", "data.toml")
 with open(path, 'rb') as f:
     benchmark_toml = f.read().decode('utf8')
 data = toml_tools.loads(benchmark_toml)
 
-
-def test_for_profiler():
-    # increase the count here to reduce the impact of
-    # setting up pytest execution environment. Let's keep
-    # the count low by default because this is part of the
-    # standard test suite.
-    iterations = int(os.environ.get("PROFILER_ITERATIONS", 1))
-    for _ in range(iterations):
-        toml_tools.dumps(data)
+class ProfilerTests(unittest.TestCase):
+    def test_for_profiler(self):
+        # increase the count here to reduce the impact of
+        # setting up pytest execution environment. Let's keep
+        # the count low by default because this is part of the
+        # standard test suite.
+        iterations = int(os.environ.get("PROFILER_ITERATIONS", 1))
+        for _ in range(iterations):
+            toml_tools.dumps(data)
+            
+        self.assertTrue(True)
```

### Comparing `toml_tools-1.1.1/tests/test_misc.py` & `toml_tools-2.0.0/tests/test_misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,59 +5,58 @@
 
 import os
 import copy
 import datetime
 from decimal import Decimal as D
 import tempfile
 import unittest
-import io
 
-from . import toml_tools
+import toml_tools
 
-from toml_tools._re import timezone
+timezone = toml_tools._re.timezone
+
+TMP_DIR_PATH = os.path.join(tempfile.gettempdir(), 'toml_tools_file_loading_tests')
+
+if not os.path.isdir(TMP_DIR_PATH):
+    os.mkdir(TMP_DIR_PATH)
 
 class TestMiscellaneous(unittest.TestCase):
+
+
     def test_load(self):
         content = "one=1 \n two='two' \n arr=[]"
         expected = {"one": 1, "two": "two", "arr": []}
-        tmp_dir_path = os.path.join(tempfile.gettempdir(), 'toml_tools_test_incorrect_load')
 
-        if not os.path.isdir(tmp_dir_path):
-            os.mkdir(tmp_dir_path)
+
         
-        file_path = os.path.join(tmp_dir_path, "test.toml")
+        file_path = os.path.join(TMP_DIR_PATH, "toml_tools_test_correct_load.toml")
         with open(file_path, 'wt') as f:
             f.write(content)
 
         with open(file_path, "rb") as bin_f:
             actual = toml_tools.load(bin_f)
         self.assertEqual(actual, expected)
 
         os.unlink(file_path)
-        os.rmdir(tmp_dir_path)
 
     @unittest.skipIf(hasattr(str, 'decode'), reason = "str can be decoded, so won't trip error (Python 2 or Iron Python 2)")
     def test_incorrect_load(self):
 
         content = "one=1"
-        tmp_dir_path = os.path.join(tempfile.gettempdir(), 'toml_tools_test_incorrect_load')
 
-        if not os.path.isdir(tmp_dir_path):
-            os.mkdir(tmp_dir_path)
 
-        file_path = os.path.join(tmp_dir_path, "test.toml")
+        file_path = os.path.join(TMP_DIR_PATH, "toml_tools_test_incorrect_load.toml")
         with open(file_path, 'wt') as f:
             f.write(content)
 
         with open(file_path, "rt") as txt_f:
             with self.assertRaises(TypeError):
                 toml_tools.load(txt_f)  # type: ignore[arg-type]
 
         os.unlink(file_path)
-        os.rmdir(tmp_dir_path)
 
     def test_parse_float(self):
         doc = """
               val=0.1
               biggest1=inf
               biggest2=+inf
               smallest=-inf
@@ -110,13 +109,29 @@
             }
         }
         self.assertEqual(obj_copy, expected_obj)
 
     def test_inline_array_recursion_limit(self):
         nest_count = 470
         recursive_array_toml = "arr = " + nest_count * "[" + nest_count * "]"
-        toml_tools.loads(recursive_array_toml)
+        dict_ = toml_tools.loads(recursive_array_toml)
+
+        list_ = dict_['arr']
+
+        i = 1
+        while len(list_) >= 1:
+            list_ = list_[0]
+            i += 1
+
+        self.assertEqual(i, nest_count)
 
     def test_inline_table_recursion_limit(self):
         nest_count = 310
         recursive_table_toml = nest_count * "key = {" + nest_count * "}"
-        toml_tools.loads(recursive_table_toml)
+        dict_ = toml_tools.loads(recursive_table_toml)
+
+        i = 0
+        while 'key' in dict_:
+            dict_ = dict_['key']
+            i += 1
+
+        self.assertEqual(i, nest_count)
```

### Comparing `toml_tools-1.1.1/tests/test_style.py` & `toml_tools-2.0.0/tests/test_style.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,142 @@
 # -*- coding: utf-8 -*-
 
-from . import toml_tools
-
-
-
-def test_newline_before_table():
-    actual = toml_tools.dumps({"table": {}})
-    expected = "[table]\n"
-    assert actual == expected
-
-    actual = toml_tools.dumps({"table": {"nested": {}, "val3": 3}, "val2": 2, "val1": 1})
-    expected = """\
+import toml_tools
+import unittest
+from collections import OrderedDict
+
+class TableWritingTests(unittest.TestCase):
+    def test_table_with_empty_array(self):
+        # Empty arrays should never be AoTs
+        example = {"table": {"array": []}}
+        expected = """\
+[table]
+array = []
+"""
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+
+    def test_newline_before_table(self):
+        actual = toml_tools.dumps({"table": {}})
+        expected = "[table]\n"
+        self.assertEqual(actual, expected)
+
+        example = OrderedDict([("table", {"nested": {}, "val3": 3}), 
+                               ("val2", 2), 
+                               ("val1", 1)])
+        
+        actual = toml_tools.dumps(example)
+        expected = """\
 val2 = 2
 val1 = 1
 
 [table]
 val3 = 3
 
 [table.nested]
 """
-    assert actual == expected
+        self.assertEqual(actual, expected)
 
 
-def test_empty_doc():
-    assert toml_tools.dumps({}) == ""
+    def test_empty_doc(self):
+        self.assertEqual(toml_tools.dumps({}), "")
 
 
-def test_dont_write_redundant_tables():
-    actual = toml_tools.dumps({"tab1": {"tab2": {"tab3": {}}}})
-    expected = "[tab1.tab2.tab3]\n"
-    assert actual == expected
+    def test_dont_write_redundant_tables(self):
+        actual = toml_tools.dumps({"tab1": {"tab2": {"tab3": {}}}})
+        expected = "[tab1.tab2.tab3]\n"
+        self.assertEqual(actual, expected)
 
 
-def test_multiline():
-    multiline_string = (
-        "This is longer than threshold!\n"
-        "Should be formatted as a multiline basic string"
-    )
-    actual = toml_tools.dumps({"ml_string": multiline_string}, multiline_strings=True)
-    expected = '''\
+    def test_multiline(self):
+        multiline_string = (
+            "This is longer than threshold!\n"
+            "Should be formatted as a multiline basic string"
+        )
+        actual = toml_tools.dumps({"ml_string": multiline_string}, multiline_strings=True)
+        expected = '''\
 ml_string = """
 This is longer than threshold!
 Should be formatted as a multiline basic string"""
 '''
-    assert actual == expected
+        self.assertEqual(actual, expected)
 
 
-def test_only_tables():
-    actual = toml_tools.dumps({"tab1": {}, "tab2": {}})
-    expected = """\
+    def test_only_tables(self):
+        actual = toml_tools.dumps(OrderedDict([("tab1", {}), 
+                                               ("tab2", {})]))
+        expected = """\
 [tab1]
 
 [tab2]
 """
-    assert actual == expected
+        self.assertEqual(actual, expected)
+
+
 
+class KeysTests(unittest.TestCase):
 
-def test_tricky_keys():
-    actual = toml_tools.dumps({"f": 1, "tab1": {}, "": {"f": 2, "": {"": 1}}, "tab3": {}})
-    expected = """\
+    def test_tricky_keys(self):
+        example = OrderedDict([("f", 1), 
+                               ("tab1", {}), 
+                               ("", {"f": 2, "": {"": 1}}), 
+                               ("tab3", {})])
+        actual = toml_tools.dumps(example)
+        expected = """\
 f = 1
 
 [tab1]
 
 [""]
 f = 2
 
 ["".""]
 "" = 1
 
 [tab3]
 """
-    assert actual == expected
+        self.assertEqual(actual, expected)
 
 
-def test_nested_keys():
-    actual = toml_tools.dumps(
-        {
-            "k": 1,
-            "a": {"b": {"c": {"d": {"e": {"f": {}}, "e2": {"f2": {}}}, "d_key1": 1}}},
-        }
-    )
-    expected = """\
+    def test_nested_keys(self):
+        actual = toml_tools.dumps(
+            {
+                "k": 1,
+                "a": {"b": {"c": {"d": {"e": {"f": {}}, "e2": {"f2": {}}}, "d_key1": 1}}},
+            }
+        )
+        expected = """\
 k = 1
 
 [a.b.c]
 d_key1 = 1
 
 [a.b.c.d.e.f]
 
 [a.b.c.d.e2.f2]
 """
-    assert actual == expected
-
-
-def test_array_of_tables_containing_lists():
-    example = {"aot": [{"a": [0, 1, 2, 3]}]}
-    expected = """\
-[[aot]]
-a = [
-    0,
-    1,
-    2,
-    3,
-]
-"""
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-    assert toml_tools.loads(actual) == example
-
-    example = {"a": {"nested": example}}
-    expected = """\
-[[a.nested.aot]]
-a = [
-    0,
-    1,
-    2,
-    3,
-]
-"""
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-
-
-def test_array_of_long_tables():
-    long_dict = {
-        "long-value": "Lorem ipsum sith",
-        "another-long-value": "consectetur adipis",
-        "simple-value": 3,
-    }
-    example = {"table": {"nested-array": [{"a": 42}, long_dict]}}
-    expected = """\
-[[table.nested-array]]
-a = 42
-
-[[table.nested-array]]
-long-value = "Lorem ipsum sith"
-another-long-value = "consectetur adipis"
-simple-value = 3
-"""
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-    assert toml_tools.loads(actual) == example
+        self.assertEqual(actual, expected)
+    
 
 
-def test_array_of_short_tables():
-    long_name = "a" * 87
-    example = {"table": {"nested-array": [{long_name: 0}, {"b": 1}, {"c": 2}]}}
-    expected = """\
-[table]
-nested-array = [
-    { %s = 0 },
-    { b = 1 },
-    { c = 2 },
-]
-""" % long_name
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-
+class ArrayOfTablesTests(unittest.TestCase):
 
-def test_example_issue_12():
-    example = {
-        "table": {
-            "nested_table": [
-                {"array_options": [1, 2, 3]},
-                {"another_array": [1, 2]},
-                {"c": 3},
-            ]
+    def test_example_issue_12(self):
+        example = {
+            "table": {
+                "nested_table": [
+                    {"array_options": [1, 2, 3]},
+                    {"another_array": [1, 2]},
+                    {"c": 3},
+                ]
+            }
         }
-    }
-    expected = """\
+        expected = """\
 [[table.nested_table]]
 array_options = [
     1,
     2,
     3,
 ]
 
@@ -182,48 +145,42 @@
     1,
     2,
 ]
 
 [[table.nested_table]]
 c = 3
 """
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-    assert toml_tools.loads(actual) == example
-
-
-def test_table_with_empty_array():
-    # Empty arrays should never be AoTs
-    example = {"table": {"array": []}}
-    expected = """\
-[table]
-array = []
-"""
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-    assert toml_tools.loads(actual) == example
-
-
-def test_non_trivial_nesting():
-    long = {
-        "long-value": "Lorem ipsum dolor sit amet",
-        "another-long-value": "consectetur adipiscing elit",
-        "a-third-one": "sed do eiusmod tempor incididunt ut labore et dolore magna",
-        "simple-value": 3,
-    }
-    example = {
-        "table": {
-            "aot": [
-                {"nested-table": {"nested_aot": [{"a": [0, 1]}, {"b": 2}, {"c": 3}]}},
-                {"other-nested-table": {"d": 4, "e": 5, "f": [{"g": 6}], "h": [long]}},
-            ]
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+
+    def test_non_trivial_nesting(self):
+
+        # Use OrderedDict for dicts with more than one key, if the
+        # test requires equality to a string literal.
+        long = OrderedDict([
+            ("long-value", "Lorem ipsum dolor sit amet"),
+            ("another-long-value", "consectetur adipiscing elit"),
+            ("a-third-one", "sed do eiusmod tempor incididunt ut labore et dolore magna"),
+            ("simple-value", 3)
+        ])
+        example = {
+            "table": {
+                "aot": [
+                    {"nested-table": {"nested_aot": [{"a": [0, 1]}, {"b": 2}, {"c": 3}]}},
+                    {"other-nested-table": OrderedDict([("d", 4), 
+                                                        ("e", 5), 
+                                                        ("f", [{"g": 6}]), 
+                                                        ("h", [long])])},
+                ]
+            }
         }
-    }
 
-    expected = """\
+        expected = """\
 [[table.aot]]
 
 [[table.aot.nested-table.nested_aot]]
 a = [
     0,
     1,
 ]
@@ -245,31 +202,105 @@
 
 [[table.aot.other-nested-table.h]]
 long-value = "Lorem ipsum dolor sit amet"
 another-long-value = "consectetur adipiscing elit"
 a-third-one = "sed do eiusmod tempor incididunt ut labore et dolore magna"
 simple-value = 3
 """
-    actual = toml_tools.dumps(example)
-    assert actual == expected
-    assert toml_tools.loads(actual) == example
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+
 
 
-def test_multiline_in_aot():
-    data = {"aot": [{"multiline_string": "line1\nline2"}]}
-    assert (
-        toml_tools.dumps(data, multiline_strings=True)
-        == '''\
+    def test_array_of_tables_containing_lists(self):
+        example = {"aot": [{"a": [0, 1, 2, 3]}]}
+        expected = """\
+[[aot]]
+a = [
+    0,
+    1,
+    2,
+    3,
+]
+"""
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+        example = {"a": {"nested": example}}
+        expected = """\
+[[a.nested.aot]]
+a = [
+    0,
+    1,
+    2,
+    3,
+]
+"""
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+
+    def test_array_of_long_tables(self):
+
+        long_dict = OrderedDict([
+            ("long-value", "Lorem ipsum sith"),
+            ("another-long-value", "consectetur adipis"),
+            ("simple-value", 3)
+        ])
+        example = {"table": {"nested-array": [{"a": 42}, long_dict]}}
+        expected = """\
+[[table.nested-array]]
+a = 42
+
+[[table.nested-array]]
+long-value = "Lorem ipsum sith"
+another-long-value = "consectetur adipis"
+simple-value = 3
+"""
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+
+    def test_array_of_short_tables(self):
+        long_name = "a" * 87
+        example = {"table": {"nested-array": [{long_name: 0}, {"b": 1}, {"c": 2}]}}
+        expected = """\
+[table]
+nested-array = [
+    { %s = 0 },
+    { b = 1 },
+    { c = 2 },
+]
+""" % long_name
+        
+        actual = toml_tools.dumps(example)
+        self.assertEqual(actual, expected)
+        self.assertEqual(toml_tools.loads(actual), example)
+
+
+
+
+    def test_multiline_in_aot(self):
+        data = {"aot": [{"multiline_string": "line1\nline2"}]}
+        self.assertEqual(
+            toml_tools.dumps(data, multiline_strings=True),
+            '''\
 [[aot]]
 multiline_string = """
 line1
 line2"""
 '''
-    )
-    assert (
-        toml_tools.dumps(data, multiline_strings=False)
-        == """\
+        )
+        self.assertEqual(
+            toml_tools.dumps(data, multiline_strings=False),
+            """\
 aot = [
     { multiline_string = "line1\\nline2" },
 ]
 """
-    )
+        )
+
```

### Comparing `toml_tools-1.1.1/tests/test_types.py` & `toml_tools-2.0.0/tests/test_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # -*- coding: utf-8 -*-
 
+from collections import OrderedDict
 from decimal import Decimal
+import unittest
 
-from . import toml_tools
+import toml_tools
 
-
-def test_decimal():
-    obj = {
-        "decimal-0": Decimal(0),
-        "decimal-pi": Decimal("3.14159"),
-        "decimal-inf": Decimal("inf"),
-        "decimal-minus-inf": Decimal("-inf"),
-        "decimal-nan": Decimal("nan"),
-    }
-    assert (
-        toml_tools.dumps(obj)
-        == """\
+class TypeWriterTests(unittest.TestCase):
+    def test_decimal(self):
+        obj = OrderedDict([
+            ("decimal-0", Decimal(0)),
+            ("decimal-pi", Decimal("3.14159")),
+            ("decimal-inf", Decimal("inf")),
+            ("decimal-minus-inf", Decimal("-inf")),
+            ("decimal-nan", Decimal("nan")),
+        ])
+        self.assertEqual(
+            toml_tools.dumps(obj),
+            """\
 decimal-0 = 0
 decimal-pi = 3.14159
 decimal-inf = inf
 decimal-minus-inf = -inf
 decimal-nan = nan
 """
-    )
+        )
 
 
-def test_tuple():
-    obj = {"empty-tuple": (), "non-empty-tuple": (1, (2, 3))}
-    assert (
-        toml_tools.dumps(obj)
-        == """\
+    def test_tuple(self):
+        obj = OrderedDict([("empty-tuple", ()),
+                           ("non-empty-tuple", (1, (2, 3)))])
+        self.assertEqual(
+            toml_tools.dumps(obj),
+            """\
 empty-tuple = []
 non-empty-tuple = [
     1,
     [
         2,
         3,
     ],
 ]
 """
-    )
+        )
```

### Comparing `toml_tools-1.1.1/toml_tools/_parser.py` & `toml_tools-2.0.0/toml_tools/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 # SPDX-FileCopyrightText: 2021 Taneli Hukkinen
 # Licensed to PSF under a Contributor Agreement.
 
 import sys
-from collections import namedtuple
+import collections
 import string
 import struct
 
 from ._re import (
     RE_DATETIME,
     RE_LOCALTIME,
     RE_NUMBER,
     match_to_datetime,
     match_to_localtime,
     match_to_number,
 )
 
-from ._helpers import ReadOnlyDict
+from ._helpers import ReadOnlyDict, Dict, parse_float
 
 if sys.version_info < (3,):
+
     def unichar(i):
         """https://stackoverflow.com/a/28326717/20785734
         """
         try:
             return unichr(i)
         except ValueError:
             return struct.pack('i', i).decode('utf-32')
@@ -45,44 +46,44 @@
 TOML_WS = frozenset(" \t")
 TOML_WS_AND_NEWLINE = TOML_WS | frozenset("\n")
 BARE_KEY_CHARS = frozenset(string.ascii_letters + string.digits + "-_")
 KEY_INITIAL_CHARS = BARE_KEY_CHARS | frozenset("\"'")
 HEXDIGIT_CHARS = frozenset(string.hexdigits)
 
 BASIC_STR_ESCAPE_REPLACEMENTS = ReadOnlyDict(
-    {
-        "\\b": "\u0008",  # backspace
-        "\\t": "\u0009",  # tab
-        "\\n": "\u000A",  # linefeed
-        "\\f": "\u000C",  # form feed
-        "\\r": "\u000D",  # carriage return
-        '\\"': "\u0022",  # quote
-        "\\\\": "\u005C",  # backslash
-    }
+    [
+        ("\\b", u"\u0008"),  # backspace
+        ("\\t", u"\u0009"),  # tab
+        ("\\n", u"\u000A"),  # linefeed
+        ("\\f", u"\u000C"),  # form feed
+        ("\\r", u"\u000D"),  # carriage return
+        ('\\"', u"\u0022"),  # quote
+        ("\\\\", u"\u005C")  # backslash
+    ]
 )
 
 
 class TOMLDecodeError(ValueError):
     """An error raised if a document is not valid TOML."""
 
 
-def load(__fp, parse_float = float):
+def load(__fp, parse_float = parse_float):
     #type(IO[bytes], Callable[[str], type(any)])) -> dict[str, Any]
     """Parse TOML from a binary file object."""
     b = __fp.read()
     try:
-        s = b.decode()
+        s = b.decode(encoding = 'utf8')
     except AttributeError:
         raise TypeError("File must be opened in binary mode"
                         ", e.g. use `open('foo.toml', 'rb')`"
                        )
     return loads(s, parse_float=parse_float)
 
 
-def loads(__s, parse_float = float):
+def loads(__s, parse_float = parse_float):
     #type(str, Callable[[str], type(any)])) -> dict[str, Any]
     """Parse TOML from a string."""
 
     # The spec allows converting "\r\n" to "\n", even in string
     # literals. Let's do so to simplify parsing.
     src = __s.replace("\r\n", "\n")
     pos = 0
@@ -207,22 +208,22 @@
             return flag in cont["flags"] or flag in cont["recursive_flags"]
         return False
 
 
 class NestedDict:
     def __init__(self):
         # The parsed content of the TOML document
-        self.dict = {} # : dict[str, Any]
+        self.dict = Dict() # : dict[str, Any]
 
     def get_or_create_nest(self, key, access_lists = True):
         #type(Tuple[str, ...], bool) -> dict
         cont = self.dict 
         for k in key:
             if k not in cont:
-                cont[k] = {}
+                cont[k] = Dict()
             cont = cont[k]
             if access_lists and isinstance(cont, list):
                 cont = cont[-1]
             if not isinstance(cont, dict):
                 raise KeyError("There is no nest behind this key")
         return cont
 
@@ -230,20 +231,20 @@
         #type(Tuple[str, ...]) -> None
         cont = self.get_or_create_nest(key[:-1])
         last_key = key[-1]
         if last_key in cont:
             list_ = cont[last_key]
             if not isinstance(list_, list):
                 raise KeyError("An object other than list found behind this key")
-            list_.append({})
+            list_.append(Dict())
         else:
-            cont[last_key] = [{}]
+            cont[last_key] = [Dict()]
 
 
-Output = namedtuple('Output', ('data', 'flags'))
+Output = collections.namedtuple('Output', ('data', 'flags'))
 
 
 def skip_chars(src, pos, chars):
     #type(str, int, ITerable[str]) -> int
     try:
         while src[pos] in chars:
             pos += 1
@@ -648,14 +649,17 @@
     localtime_match = RE_LOCALTIME.match(src, pos)
     if localtime_match:
         return localtime_match.end(), match_to_localtime(localtime_match)
 
     # Integers and "normal" floats.
     # The regex will greedily match any type starting with a decimal
     # char, so needs to be located after handling of dates and times.
+    # 
+    # In < Python 3.6, if the default value for parse_float is float
+    # underscores are stripped out before calling float.
     number_match = RE_NUMBER.match(src, pos)
     if number_match:
         return number_match.end(), match_to_number(number_match, parse_float)
 
     # Special floats
     first_three = src[pos : pos + 3]
     if first_three in {"inf", "nan"}:
@@ -687,28 +691,32 @@
 
 
 def is_unicode_scalar_value(codepoint):
     #type(int) -> bool
     return (0 <= codepoint <= 55295) or (57344 <= codepoint <= 1114111)
 
 
-def make_safe_parse_float(parse_float):
+def make_safe_parse_float(user_parse_float):
     #type(Callable[[str], type(any)])) -> Callable[[str], type(any)])
     """A decorator to make `parse_float` safe.
 
     `parse_float` must not return dicts or lists, because these types
     would be mixed with parsed TOML tables and arrays, thus confusing
     the parser. The returned decorated callable raises `ValueError`
     instead of returning illegal types.
     """
     # The default `float` callable never returns illegal types. Optimize it.
-    if parse_float is float:
-        return float
+    
+
+    if user_parse_float is parse_float:
+        return parse_float
+        
 
     def safe_parse_float(float_str):
         #type(str) -> Any:
-        float_value = parse_float(float_str)
+        """ This only accepts underscores if user_parse_float does. """
+        float_value = user_parse_float(float_str)
         if isinstance(float_value, (dict, list)):
             raise ValueError("parse_float must not return dicts or lists")
         return float_value
 
     return safe_parse_float
```

### Comparing `toml_tools-1.1.1/toml_tools/_re.py` & `toml_tools-2.0.0/toml_tools/_re.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Licensed to PSF under a Contributor Agreement.
 
 
 from datetime import date, datetime, time, timedelta, tzinfo
 import re
 import copy
 
+from ._helpers import parse_int, parse_float
+
 try:
     from datetime import timezone
 except ImportError:
     # https://docs.python.org/2.7/library/datetime.html#tzinfo-objects
     ZERO = timedelta(0)
 
     class UTC(tzinfo):
@@ -143,12 +145,16 @@
 def match_to_localtime(match):
     #type(re.Match) -> time
     hour_str, minute_str, sec_str, micros_str = match.groups()
     micros = int(micros_str.ljust(6, "0")) if micros_str else 0
     return time(int(hour_str), int(minute_str), int(sec_str), micros)
 
 
-def match_to_number(match, parse_float):
+
+def match_to_number(match, parse_float = parse_float):
     #type(re.Match, Callable[[str], type(any)]) -> type(any)
     if match.group("floatpart"):
-        return parse_float(match.group())
-    return int(match.group(), 0)
+        float_str = match.group()
+        return parse_float(float_str)
+    
+
+    return parse_int(match.group())
```

### Comparing `toml_tools-1.1.1/toml_tools/_writer.py` & `toml_tools-2.0.0/toml_tools/_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 
 
 from collections import namedtuple
 from datetime import date, datetime, time
 from decimal import Decimal
 import string
 
-from ._helpers import ReadOnlyDict
+from ._helpers import ReadOnlyDict, long
+
+try:
+    basestring #type: ignore
+except NameError:
+    basestring = str
+
 
 ASCII_CTRL = frozenset(chr(i) for i in range(32)) | frozenset(chr(127))
 ILLEGAL_BASIC_STR_CHARS = frozenset('"\\') | ASCII_CTRL - frozenset("\t")
 BARE_KEY_CHARS = frozenset(string.ascii_letters + string.digits + "-_")
 ARRAY_TYPES = (list, tuple)
 ARRAY_INDENT = " " * 4
 MAX_LINE_LENGTH = 100
 
-COMPACT_ESCAPES = ReadOnlyDict({"\u0008": "\\b",  # backspace
-                                "\u000A": "\\n",  # linefeed
-                                "\u000C": "\\f",  # form feed
-                                "\u000D": "\\r",  # carriage return
-                                "\u0022": '\\"',  # quote
-                                "\u005C": "\\\\",  # backslash
-                               }
+COMPACT_ESCAPES = ReadOnlyDict([(u"\u0008", r"\b"),  # backspace
+                                (u"\u000A", r"\n"),  # linefeed
+                                (u"\u000C", r"\f"),  # form feed
+                                (u"\u000D", r"\r"),  # carriage return
+                                (u"\u0022", r'\"'),  # quote
+                                (u"\u005C", r"\\")  # backslash
+                               ]
                               )
 
 
 def dump(__obj, __fp, multiline_strings = False):
     #type(dict, BinaryIO, bool) -> None
     ctx = Context(multiline_strings, {})
     for chunk in gen_table_chunks(__obj, ctx, name=""):
@@ -79,29 +85,34 @@
             yield chunk
 
 
 def format_literal(obj, ctx, nest_level= 0):
     #type(type[any], Context, int) -> str
     if isinstance(obj, bool):
         return "true" if obj else "false"
-    if isinstance(obj, (int, float, date, datetime)):
+    if isinstance(obj, (int, long, date, datetime)):
         return str(obj)
+    
+    # repr of floats Makes Python 2 behaviour consistent
+    # https://stackoverflow.com/questions/25898733/why-does-strfloat-return-more-digits-in-python-3-than-python-2
+    if isinstance(obj, float):
+        return repr(obj)
     if isinstance(obj, Decimal):
         return format_decimal(obj)
     if isinstance(obj, time):
         if obj.tzinfo:
             raise ValueError("TOML does not support offset times")
         return str(obj)
-    if isinstance(obj, str):
+    if isinstance(obj, basestring):
         return format_string(obj, allow_multiline=ctx.allow_multiline)
     if isinstance(obj, ARRAY_TYPES):
         return format_inline_array(obj, ctx, nest_level)
     if isinstance(obj, dict):
         return format_inline_table(obj, ctx)
-    raise TypeError("Object of type %s is not TOML serializable" % type(obj))
+    raise TypeError("Object: %s of type %s is not TOML serializable" % (obj, type(obj)))
 
 
 def format_decimal(obj):
     #type(Decimal) -> str
     if obj.is_nan():
         return "nan"
     if obj == Decimal("inf"):
@@ -162,35 +173,32 @@
     do_multiline = allow_multiline and "\n" in s
     if do_multiline:
         result = '"""\n'
         s = s.replace("\r\n", "\n")
     else:
         result = '"'
 
-    pos = seq_start = 0
-    while True:
-        try:
-            char = s[pos]
-        except IndexError:
-            result += s[seq_start:pos]
-            if do_multiline:
-                return result + '"""'
-            return result + '"'
+    for char in s:
         if char in ILLEGAL_BASIC_STR_CHARS:
-            result += s[seq_start:pos]
             if char in COMPACT_ESCAPES:
                 if do_multiline and char == "\n":
                     result += "\n"
                 else:
                     result += COMPACT_ESCAPES[char]
             else:
                 result += "\\u" + hex(ord(char))[2:].rjust(4, "0")
-            seq_start = pos + 1
-        pos += 1
+        else:
+            result += char
+
+    if do_multiline:
+        result += '"""'
+    else:
+        result += '"'
 
+    return result
 
 def is_aot(obj):
     #type(type[Any]) -> bool
     """Decides if an object behaves as an array of tables (i.e. a nonempty list
     of dicts)."""
     return bool(
         isinstance(obj, ARRAY_TYPES) and obj and all(isinstance(v, dict) for v in obj)
```

### Comparing `toml_tools-1.1.1/toml_tools.egg-info/PKG-INFO` & `toml_tools-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: toml-tools
-Version: 1.1.1
+Name: toml_tools
+Version: 2.0.0
 Summary: Tomli and Tomli-W for Python 2 and Iron Python
 Home-page: https://github.com/JamesParrott/toml_tools
 Author: Taneli Hukkinen
 Author-email: hukkin@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,19 +17,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# toml_tools, Tomli and Tomli-W for Python 2 and Iron Python
+# toml_tools: Tomli and Tomli-W for Python 2 and Iron Python
 
-v1.1.1 - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+v2.0.0 
+ - dump and dumps now return an OrderedDict, in Pythons before 3.7 or in IronPython which should preserve the order of entries (other than listing the root table entries first).  
+ - integers and floats can have underscores in in Python 2
+ - Passes 312 tests in each of cPythons 2.7, and 3.7 to 3.12, and in Iron Pythons 2.7 and 3.4.
 
-v1.0.0 is a complete overhaul - toml_tools is now based on tomli and tomli-w.  Note, unlike toml_tools v0, toml and tomlkit, toml_tools v1 and tomli require files to be opened in bytes mode ('rb').
+v1.1.1
+ - fit for purpose!  Passes 52 of Hukkin's unittest tests, in Python 2 and Iron Python 2.7
+
+v1.0.0 is a complete overhaul
+ - toml_tools is now based on tomli and tomli-w.  Note unlike toml_tools v0, toml and tomlkit, that both toml_tools v1 and tomli require files to be opened in bytes mode ('rb'), not text mode ('rt').
 
 
 # Parent Project number (1/2)'s Readme File (Tomli)
 
 > A lil' TOML parser
 
 **Table of Contents**  *generated with [mdformat-toc](https://github.com/hukkin/mdformat-toc)*
```

