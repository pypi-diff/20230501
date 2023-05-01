# Comparing `tmp/polynomiograpy-0.1.0.tar.gz` & `tmp/polynomiograpy-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.1.0.tar", max compression
+gzip compressed data, was "polynomiograpy-0.1.0a1.tar", max compression
```

## Comparing `polynomiograpy-0.1.0.tar` & `polynomiograpy-0.1.0a1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.1.0/LICENSE
--rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.1.0/README.md
--rw-r--r--   0        0        0     1399 2023-05-01 02:42:20.827237 polynomiograpy-0.1.0/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.1.0/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     1256 2023-05-01 02:27:18.245511 polynomiograpy-0.1.0/polynomiograpy/compute_screen.py
--rw-r--r--   0        0        0      689 2023-05-01 02:36:13.412823 polynomiograpy-0.1.0/polynomiograpy/methods/iter.py
--rw-r--r--   0        0        0      731 2023-05-01 02:44:31.679177 polynomiograpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 polynomiograpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1998 2023-05-01 03:36:56.911460 polynomiograpy-0.1.0a1/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     2444 2023-05-01 03:32:22.349878 polynomiograpy-0.1.0a1/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.1.0a1/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     1256 2023-05-01 02:27:18.245511 polynomiograpy-0.1.0a1/polynomiograpy/compute_screen.py
+-rw-r--r--   0        0        0     2279 2023-05-01 03:18:42.322827 polynomiograpy-0.1.0a1/polynomiograpy/methods/iter.py
+-rw-r--r--   0        0        0      803 2023-05-01 03:36:31.397676 polynomiograpy-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 polynomiograpy-0.1.0a1/PKG-INFO
```

### Comparing `polynomiograpy-0.1.0/LICENSE` & `polynomiograpy-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0/polynomiograpy/__init__.py` & `polynomiograpy-0.1.0a1/polynomiograpy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Literal, Callable
 from polynomiograpy.common.polynomial import Polynomial
 from polynomiograpy.compute_screen import compute_screen
 from polynomiograpy.methods import iter
 import numpy as np
 
-__version__ = "0.1.0"
+__version__ = "0.1.0.a1"
 
 __all__ = ["compute_screen_for_single_poly", "Polynomial"]
 
 
 def compute_screen_for_single_poly(
-    method: Literal["newton"],
+    method: Literal["newton", "halley", "steffensen"],
     poly: Polynomial,
     delta: float,
     width: int,
     height: int,
     screen: np.ndarray,
     screen_buffer: np.ndarray,
     *,
@@ -22,27 +22,49 @@
     scale_y: float = 1,
     shift_x: float = 0,
     shift_y: float = 0,
     max_value: int = 16,
     reverse_color=False,
     channel: int = 0,
 ):
-    assert method in {"newton"}, "Unknown method"
+    assert method in iter.available_methods, "Unknown method"
     func: Callable[[complex], int]
     if method == "newton":
 
         def func(val: complex) -> int:
             new_val, iter_count = iter.newton_method(
                 poly,
                 val,
                 delta,
                 max_iter_count=max_value,
             )
             return iter_count
 
+    elif method == "halley":
+
+        def func(val: complex) -> int:
+            new_val, iter_count = iter.halley_method(
+                poly,
+                val,
+                delta,
+                max_iter_count=max_value,
+            )
+            return iter_count
+
+    elif method == "steffensen":
+
+        def func(val: complex) -> int:
+            new_val, iter_count = iter.steffensen_method(
+                poly,
+                val,
+                delta,
+                max_iter_count=max_value,
+            )
+            return iter_count
+
     else:
         # cannot happen
         raise Exception("wtf")
     return compute_screen(
         func,
         width,
         height,
```

### Comparing `polynomiograpy-0.1.0/polynomiograpy/common/polynomial.py` & `polynomiograpy-0.1.0a1/polynomiograpy/common/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0/polynomiograpy/compute_screen.py` & `polynomiograpy-0.1.0a1/polynomiograpy/compute_screen.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0/polynomiograpy/methods/iter.py` & `polynomiograpy-0.1.0a1/polynomiograpy/methods/iter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from polynomiograpy import common
 
+available_methods = {"newton", "halley", "steffensen"}
+
 
 def newton_method(
     poly: common.polynomial.Polynomial,
     x: complex,
     delta: float,
     *,
     step: int = 0,
@@ -23,7 +25,67 @@
             poly,
             newton_res,
             delta,
             step=step + 1,
             max_iter_count=max_iter_count,
         )
         return new_res, count + 1
+
+
+def halley_method(
+    poly: common.polynomial.Polynomial,
+    x: complex,
+    delta: float,
+    *,
+    step: int = 0,
+    max_iter_count: int = 16,
+) -> tuple[complex, int]:
+    if step > max_iter_count:
+        return x, 0
+    res = poly.eval(x)
+    deriv_res = poly.eval_deriv(x)
+    deriv_deriv_res = poly.deriv().eval_deriv(x)
+    denom = -(res * deriv_deriv_res) + 2 * deriv_res * deriv_res
+    if denom == 0:
+        return x, max_iter_count - step
+    halley_res = x - 2 * (-deriv_res * res) / denom
+    if abs(halley_res - x) < delta:
+        return halley_res, 0
+    else:
+        new_res, count = halley_method(
+            poly,
+            halley_res,
+            delta,
+            step=step + 1,
+            max_iter_count=max_iter_count,
+        )
+        return new_res, count + 1
+
+
+def steffensen_method(
+    poly: common.polynomial.Polynomial,
+    x: complex,
+    delta: float,
+    *,
+    step: int = 0,
+    max_iter_count: int = 16,
+) -> tuple[complex, int]:
+    if step > max_iter_count:
+        return x, 0
+    res = poly.eval(x)
+    if res == 0:
+        return x, 0
+    denom = poly.eval(x + res) / res - 1
+    if denom == 0:
+        return x, max_iter_count - step
+    steffensen_res = x - res / denom
+    if abs(steffensen_res - x) < delta:
+        return steffensen_res, 0
+    else:
+        new_res, count = steffensen_method(
+            poly,
+            steffensen_res,
+            delta,
+            step=step + 1,
+            max_iter_count=max_iter_count,
+        )
+        return new_res, count + 1
```

### Comparing `polynomiograpy-0.1.0/pyproject.toml` & `polynomiograpy-0.1.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.1.0"
+version = "0.1.0.a1"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
@@ -24,13 +24,16 @@
 pillow = "^9.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 
+[tool.poetry.scripts]
+polynomiograpy_cli = 'polynomiograpy.cli:run'
+
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `polynomiograpy-0.1.0/PKG-INFO` & `polynomiograpy-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polynomiograpy
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: 
 Home-page: https://github.com/ismltpn/polynomiograpy/
 License: MIT
 Keywords: Polynomiography,Polynomials,Visual Art
 Author: İsmail Tapan
 Author-email: ismltpn@gmail.com
 Maintainer: İsmail Tapan
```

