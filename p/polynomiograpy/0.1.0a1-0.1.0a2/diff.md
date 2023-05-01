# Comparing `tmp/polynomiograpy-0.1.0a1.tar.gz` & `tmp/polynomiograpy-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.1.0a1.tar", max compression
+gzip compressed data, was "polynomiograpy-0.1.0a2.tar", max compression
```

## Comparing `polynomiograpy-0.1.0a1.tar` & `polynomiograpy-0.1.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.1.0a1/LICENSE
--rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.1.0a1/README.md
--rw-r--r--   0        0        0     1998 2023-05-01 03:36:56.911460 polynomiograpy-0.1.0a1/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     2444 2023-05-01 03:32:22.349878 polynomiograpy-0.1.0a1/polynomiograpy/cli/__init__.py
--rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.1.0a1/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     1256 2023-05-01 02:27:18.245511 polynomiograpy-0.1.0a1/polynomiograpy/compute_screen.py
--rw-r--r--   0        0        0     2279 2023-05-01 03:18:42.322827 polynomiograpy-0.1.0a1/polynomiograpy/methods/iter.py
--rw-r--r--   0        0        0      803 2023-05-01 03:36:31.397676 polynomiograpy-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 polynomiograpy-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.1.0a2/README.md
+-rw-r--r--   0        0        0     1998 2023-05-01 03:42:21.865965 polynomiograpy-0.1.0a2/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     2444 2023-05-01 03:32:22.349878 polynomiograpy-0.1.0a2/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.1.0a2/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     1256 2023-05-01 02:27:18.245511 polynomiograpy-0.1.0a2/polynomiograpy/compute_screen.py
+-rw-r--r--   0        0        0     2279 2023-05-01 03:18:42.322827 polynomiograpy-0.1.0a2/polynomiograpy/methods/iter.py
+-rw-r--r--   0        0        0      738 2023-05-01 03:42:08.187485 polynomiograpy-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 polynomiograpy-0.1.0a2/PKG-INFO
```

### Comparing `polynomiograpy-0.1.0a1/LICENSE` & `polynomiograpy-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a1/polynomiograpy/__init__.py` & `polynomiograpy-0.1.0a2/polynomiograpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Callable
 from polynomiograpy.common.polynomial import Polynomial
 from polynomiograpy.compute_screen import compute_screen
 from polynomiograpy.methods import iter
 import numpy as np
 
-__version__ = "0.1.0.a1"
+__version__ = "0.1.0.a2"
 
 __all__ = ["compute_screen_for_single_poly", "Polynomial"]
 
 
 def compute_screen_for_single_poly(
     method: Literal["newton", "halley", "steffensen"],
     poly: Polynomial,
```

### Comparing `polynomiograpy-0.1.0a1/polynomiograpy/cli/__init__.py` & `polynomiograpy-0.1.0a2/polynomiograpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a1/polynomiograpy/common/polynomial.py` & `polynomiograpy-0.1.0a2/polynomiograpy/common/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a1/polynomiograpy/compute_screen.py` & `polynomiograpy-0.1.0a2/polynomiograpy/compute_screen.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a1/polynomiograpy/methods/iter.py` & `polynomiograpy-0.1.0a2/polynomiograpy/methods/iter.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.1.0a1/pyproject.toml` & `polynomiograpy-0.1.0a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.1.0.a1"
+version = "0.1.0.a2"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
@@ -13,18 +13,15 @@
     "Polynomiography",
     "Polynomials",
     "Visual Art"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-moderngl = "^5.8.1"
-moderngl-window = "^2.4.3"
 numpy = "^1.24.2"
-pyglet = "^2.0.5"
 pillow = "^9.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

