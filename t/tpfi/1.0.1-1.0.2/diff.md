# Comparing `tmp/tpfi-1.0.1.tar.gz` & `tmp/tpfi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.0.1.tar", max compression
+gzip compressed data, was "tpfi-1.0.2.tar", max compression
```

## Comparing `tpfi-1.0.1.tar` & `tpfi-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-28 16:03:14.851920 tpfi-1.0.1/LICENSE
--rw-r--r--   0        0        0     2251 2023-04-28 16:03:14.851920 tpfi-1.0.1/README.md
--rw-r--r--   0        0        0      417 2023-04-28 16:03:14.859920 tpfi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    14657 2023-04-28 16:03:14.859920 tpfi-1.0.1/tpfi.py
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 tpfi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 13:22:49.013242 tpfi-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2251 2023-05-01 13:22:49.013242 tpfi-1.0.2/README.md
+-rw-r--r--   0        0        0      417 2023-05-01 13:22:49.021242 tpfi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-05-01 13:22:49.021242 tpfi-1.0.2/src/tpfi/__init__.py
+-rw-r--r--   0        0        0    14658 2023-05-01 13:22:49.021242 tpfi-1.0.2/src/tpfi/tpfi.py
+-rw-r--r--   0        0        0     5167 2023-05-01 13:22:49.021242 tpfi-1.0.2/src/tpfi/utils.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 tpfi-1.0.2/PKG-INFO
```

### Comparing `tpfi-1.0.1/LICENSE` & `tpfi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.1/README.md` & `tpfi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.1/tpfi.py` & `tpfi-1.0.2/src/tpfi/tpfi.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from matplotlib import patches
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.colorbar import Colorbar
 from matplotlib.offsetbox import AnchoredText
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
-from utils import add_orientation, add_scalebar, calculate_theta, query_sky_img
+from .utils import add_orientation, add_scalebar, calculate_theta, query_sky_img
 
 Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
 Gaia.ROW_LIMIT = -1
 
 CUSTOM_SIMBAD = Simbad()
 CUSTOM_SIMBAD.add_votable_fields("ids")
```

### Comparing `tpfi-1.0.1/PKG-INFO` & `tpfi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

