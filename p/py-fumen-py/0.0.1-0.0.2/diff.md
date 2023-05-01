# Comparing `tmp/py_fumen_py-0.0.1.tar.gz` & `tmp/py_fumen_py-0.0.2.tar.gz`

## Comparing `py_fumen_py-0.0.1.tar` & `py_fumen_py-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/test2.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/__init__.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/action.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/comment.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/constant.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/field.py
--rw-r--r--   0        0        0   116321 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/fumen.js
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/fumen_buffer.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/fumen_codec.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/js_escape.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/operation.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/page.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/quiz.py
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/src/py_fumen_py/quiz.py.old
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/LICENSE
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 py_fumen_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/.field.py.swp
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/.operation.py.swp
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/__init__.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/action.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/comment.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/constant.py
+-rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/field.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/fumen_buffer.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/fumen_codec.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/js_escape.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/operation.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/page.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/src/py_fumen_py/quiz.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/README.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 py_fumen_py-0.0.2/PKG-INFO
```

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/action.py` & `py_fumen_py-0.0.2/src/py_fumen_py/action.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/comment.py` & `py_fumen_py-0.0.2/src/py_fumen_py/comment.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/constant.py` & `py_fumen_py-0.0.2/src/py_fumen_py/constant.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/field.py` & `py_fumen_py-0.0.2/src/py_fumen_py/field.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,21 @@
             1 if slice_.step is None else slice_.step
         )
 
     @classmethod
     def _field_init(cls, height, field=None):
         if field:
             if isinstance(field, str):
-                lines = [[Mino.parse_name(mino) for mino in line]
-                         for line in field.splitlines()[::-1]]
-            else:
+                field = field.splitlines()
+
+            if isinstance(field[0], list):
                 lines = [line[:] for line in field]
+            elif isinstance(field[0], str):
+                lines = [[Mino.parse_name(mino) for mino in line]
+                        for line in field[::-1]]
             lines[-1] += [Mino._ for x in range(Consts.WIDTH-len(lines[-1]))]
             lines += cls._empty_lines(height-len(lines))
             return lines
         else:
             return cls._empty_lines(height)
 
     def __init__(self, field=None, garbage=None):
@@ -138,45 +141,49 @@
 
     def shift_right(self, amount=1, warp=False):
         for line in self:
             line[:] = ((line[-amount:] if warp else [Mino._]*amount)
                        + line[:-amount])
 
     def is_lineclear_at(self, y):
-        return not Mino._ in self[y]
+        return Mino._ not in self[y]
 
     def clear_line(self):
         lines = []
         n_lineclear = 0
         for line in self:
             if Mino._ in line:
                 lines.append(line)
             else:
                 n_lineclear += 1
-        self._field = lines + [[Mino._ for x in range(Consts.WIDTH)]
-                               for y in range(n_lineclear)]
+        self._field = lines + self._empty_lines(n_lineclear)
         return n_lineclear
 
     def apply_action(self, action):
         if action.lock:
             if action.operation.mino.is_colored():
                 self.lock(action.operation)
             self.clear_line()
             if action.rise:
                 self.rise()
             if action.mirror:
                 self.mirror()
 
+    def height(self):
+        height = Consts.HEIGHT
+        while (height > 0
+                and all(mino is Mino._ for mino in self[height - 1])):
+            height -= 1
+        return height
+
     def _string(self, start=None, stop=None, truncated=True, separator='\n'):
         start = -Consts.GARBAGE_HEIGHT if start is None else start
         stop = Consts.HEIGHT if stop is None else stop
         if truncated:
-            while (stop > start
-                    and all(mino is Mino._ for mino in self[stop-1])):
-                stop -= 1
+            stop = min(stop, self.height())
         return separator.join(
             reversed([''.join(mino.name for mino in line)
                       for line in self[start:stop]])
         )
 
     def string(self, truncated=True, separator='\n', with_garbage=True):
         return self._string(None if with_garbage else 0, None,
```

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/fumen_buffer.py` & `py_fumen_py-0.0.2/src/py_fumen_py/fumen_buffer.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/fumen_codec.py` & `py_fumen_py-0.0.2/src/py_fumen_py/fumen_codec.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/js_escape.py` & `py_fumen_py-0.0.2/src/py_fumen_py/js_escape.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/operation.py` & `py_fumen_py-0.0.2/src/py_fumen_py/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     L = 2
     O = 3
     Z = 4
     T = 5
     J = 6
     S = 7
     X = 8
+    G = 8
     GRAY = 8
 
     @staticmethod
     def parse_name(name):
     # parse_name() is added to support parsing of ' ' and lowercase names.
         if name == ' ':
             return Mino._
```

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/page.py` & `py_fumen_py-0.0.2/src/py_fumen_py/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 @dataclass
 class Refs():
     field: Optional[int] = None
     comment: Optional[int] = None
 
 @dataclass
 class Page():
-    field: Optional[Field]
-    operation: Optional[Operation]
-    comment: Optional[str]
-    flags: Optional[Flags]
-    refs: Optional[Refs]
+    field: Optional[Field] = None
+    operation: Optional[Operation] = None
+    comment: Optional[str] = None
+    flags: Optional[Flags] = None
+    refs: Optional[Refs] = None
 
     def __repr__(self):
-        return (f'{{field:\n{self.field}, operation: {self.operation}, '
-                f'comment:{self.comment}, flags: {self.flags}, '
-                f'refs: {self.refs}}}')
+        field_separator = '\n' if self.field else ' '
+        return (f'{{field:{field_separator}{self.field}, '
+                f'operation: {self.operation}, comment: {self.comment}, '
+                f'flags: {self.flags}, refs: {self.refs}}}')
```

### Comparing `py_fumen_py-0.0.1/src/py_fumen_py/quiz.py` & `py_fumen_py-0.0.2/src/py_fumen_py/quiz.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/.gitignore` & `py_fumen_py-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/LICENSE` & `py_fumen_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/README.md` & `py_fumen_py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.1/pyproject.toml` & `py_fumen_py-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_py"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'tetris-fumen'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `py_fumen_py-0.0.1/PKG-INFO` & `py_fumen_py-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_fumen_py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of the JavaScript package 'tetris-fumen'
 Project-URL: Source, https://github.com/OctupusTea/py-fumen-py
 Author: Octupus Tea
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

