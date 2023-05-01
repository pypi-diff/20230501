# Comparing `tmp/py_fumen_py-0.0.2.tar.gz` & `tmp/py_fumen_py-0.0.3.tar.gz`

## Comparing `py_fumen_py-0.0.2.tar` & `py_fumen_py-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/.field.py.swp
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/.operation.py.swp
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/__init__.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/action.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/comment.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/constant.py
--rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/field.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/fumen_buffer.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/fumen_codec.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/js_escape.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/operation.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/page.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/quiz.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/LICENSE
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/.field.py.swp
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/__init__.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/action.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/comment.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/constant.py
+-rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/field.py
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/fumen_buffer.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/fumen_codec.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/js_escape.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/operation.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/page.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/src/py_fumen_py/quiz.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/README.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 py_fumen_py-0.0.3/PKG-INFO
```

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/.field.py.swp` & `py_fumen_py-0.0.3/src/py_fumen_py/.field.py.swp`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 6230 5649 4d20 382e 3000 0000 0010 0000  b0VIM 8.0.......
-00000010: fc85 4f64 289d 3c00 ba3d 0000 6f63 7475  ..Od(.<..=..octu
+00000010: fc85 4f64 289d 3c00 524d 0000 6f63 7475  ..Od(.<.RM..octu
 00000020: 7075 7374 6561 0000 0000 0000 0000 0000  pustea..........
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 4f63 7475 7075 7354 6561 2d4d  ....OctupusTea-M
 00000050: 696e 7400 0000 0000 0000 0000 0000 0000  int.............
 00000060: 0000 0000 0000 0000 0000 0000 7e6f 6374  ............~oct
 00000070: 7570 7573 7465 612f 6769 742f 7079 2d66  upustea/git/py-f
 00000080: 756d 656e 2d70 792f 7372 632f 7079 5f66  umen-py/src/py_f
@@ -788,36 +788,36 @@
 00003130: b906 0000 b806 0000 a206 0000 8306 0000  ................
 00003140: 6906 0000 2206 0000 0a06 0000 f405 0000  i..."...........
 00003150: f305 0000 a505 0000 6205 0000 2b05 0000  ........b...+...
 00003160: 1505 0000 e904 0000 ca04 0000 9004 0000  ................
 00003170: 5b04 0000 5104 0000 5004 0000 0704 0000  [...Q...P.......
 00003180: c803 0000 9603 0000 9503 0000 7d03 0000  ............}...
 00003190: 3503 0000 3403 0000 1d03 0000 0003 0000  5...4...........
-000031a0: ff02 0000 bb02 0000 a302 0000 9e02 0000  ................
-000031b0: 8602 0000 7702 0000 0000 0000 0000 0000  ....w...........
+000031a0: ff02 0000 0000 0000 0000 0000 0000 0000  ................
+000031b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003240: 0000 0000 0000 0020 2020 2020 2020 2072  .......        r
-00003250: 6574 7572 6e20 7365 6c66 2e73 7472 696e  eturn self.strin
-00003260: 6728 2900 2020 2020 6465 6620 5f5f 7374  g().    def __st
-00003270: 725f 5f28 7365 6c20 2020 2020 2020 2072  r__(sel        r
-00003280: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00003290: 7475 726e 2073 656c 662e 7374 7269 2020  turn self.stri  
-000032a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000032b0: 6e20 7365 6c66 2e73 7472 6920 2020 2020  n self.stri     
-000032c0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
-000032d0: 7472 696e 6728 2900 2020 2020 6465 6620  tring().    def 
-000032e0: 5f5f 7374 725f 5f28 7365 6c66 293a 0000  __str__(self):..
-000032f0: 2020 2020 2020 2020 7265 7475 726e 2020          return  
+00003240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003300: 2020 2020 2020 2020 7265 7475 726e 2073          return s
 00003310: 656c 662e 7374 7269 6e67 2829 0020 2020  elf.string().   
 00003320: 2064 6566 205f 5f73 7472 5f5f 2873 656c   def __str__(sel
 00003330: 6629 3a00 0020 2020 2020 2020 2072 6574  f):..        ret
 00003340: 7572 6e20 6627 3c46 6965 6c64 3a7b 7365  urn f'<Field:{se
 00003350: 6c66 2e73 7472 696e 6728 7472 756e 6361  lf.string(trunca
 00003360: 7465 643d 4661 6c73 652c 2073 6570 6172  ted=False, separ
```

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/action.py` & `py_fumen_py-0.0.3/src/py_fumen_py/action.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/comment.py` & `py_fumen_py-0.0.3/src/py_fumen_py/comment.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/constant.py` & `py_fumen_py-0.0.3/src/py_fumen_py/constant.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/field.py` & `py_fumen_py-0.0.3/src/py_fumen_py/field.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/fumen_buffer.py` & `py_fumen_py-0.0.3/src/py_fumen_py/fumen_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     def move_field_buffer(self):
         self += self._field_repeat_buffer
         self._field_repeat_buffer.clear()
 
     def write_field(self, field):
         if field is None:
             diff = 0
+            prev_diff = 0
             length = self._consts.TOTAL_BLOCK_COUNT - 1
         else:
             prev_diff = self._field_diff(field, 0, 0)
             length = -1
             for y in range(self._consts.TOTAL_HEIGHT):
                 for x in range(self._consts.WIDTH):
                     diff = self._field_diff(field, x, y)
```

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/fumen_codec.py` & `py_fumen_py-0.0.3/src/py_fumen_py/fumen_codec.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/js_escape.py` & `py_fumen_py-0.0.3/src/py_fumen_py/js_escape.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/operation.py` & `py_fumen_py-0.0.3/src/py_fumen_py/operation.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/page.py` & `py_fumen_py-0.0.3/src/py_fumen_py/page.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/src/py_fumen_py/quiz.py` & `py_fumen_py-0.0.3/src/py_fumen_py/quiz.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/.gitignore` & `py_fumen_py-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/LICENSE` & `py_fumen_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/README.md` & `py_fumen_py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.2/pyproject.toml` & `py_fumen_py-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_py"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'tetris-fumen'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `py_fumen_py-0.0.2/PKG-INFO` & `py_fumen_py-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_fumen_py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of the JavaScript package 'tetris-fumen'
 Project-URL: Source, https://github.com/OctupusTea/py-fumen-py
 Author: Octupus Tea
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

