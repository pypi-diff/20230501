# Comparing `tmp/yt_idefix-1.1.1.tar.gz` & `tmp/yt_idefix-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-1.1.1.tar", last modified: Tue Apr 18 15:42:55 2023, max compression
+gzip compressed data, was "yt_idefix-2.0.0.tar", last modified: Mon May  1 13:30:43 2023, max compression
```

## Comparing `yt_idefix-1.1.1.tar` & `yt_idefix-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 15:42:42.000000 yt_idefix-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 15:42:42.000000 yt_idefix-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-18 15:42:42.000000 yt_idefix-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 13:30:27.000000 yt_idefix-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-01 13:30:27.000000 yt_idefix-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-01 13:30:27.000000 yt_idefix-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34811 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:29.000000 yt_idefix-2.0.0/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:30:43.108076 yt_idefix-2.0.0/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 13:30:43.000000 yt_idefix-2.0.0/yt_idefix.egg-info/top_level.txt
```

### Comparing `yt_idefix-1.1.1/LICENSE` & `yt_idefix-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/pyproject.toml` & `yt_idefix-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_idefix"
-version = "1.1.1"
+version = "2.0.0"
 description = "An extension module for yt, adding a frontend for Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

### Comparing `yt_idefix-1.1.1/tests/test_C_io.py` & `yt_idefix-2.0.0/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/tests/test_dmp.py` & `yt_idefix-2.0.0/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/tests/test_loading.py` & `yt_idefix-2.0.0/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/tests/test_vtk.py` & `yt_idefix-2.0.0/tests/test_vtk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import re
+import shutil
+from pathlib import Path
 
 import pytest
 from more_itertools import distinct_combinations
 from unyt import Unit, assert_allclose_units
 
 import yt
 from yt_idefix.api import IdefixVtkDataset, PlutoVtkDataset
@@ -94,14 +96,31 @@
     # Pluto's velocity_unit should be overrided
     expect_velocity = ds.length_unit / ds.quan(*uo["time_unit"])
     expect_mass = ds.quan(*uo["density_unit"]) * ds.length_unit**3
     assert_allclose_units(ds.velocity_unit, expect_velocity)
     assert_allclose_units(ds.mass_unit, expect_mass)
 
 
+def test_missing_inifile(tmp_path):
+    tmpdir = tmp_path / "missing_inifile"
+    shutil.copytree(
+        Path(__file__).parent / "data" / "pluto_disk_planet",
+        tmpdir,
+        ignore=shutil.ignore_patterns("*.ini"),
+    )
+    with pytest.warns(UserWarning, match="Could not find inifile"):
+        yt.load(tmpdir / "data.0010.vtk")
+
+
+def test_incorrect_inifile():
+    file_dir = Path(__file__).parent / "data" / "pluto_disk_planet"
+    with pytest.warns(UserWarning, match=r"Cannot get the value of"):
+        yt.load(file_dir / "data.0010.vtk", inifile=file_dir / "incorrect_inifile")
+
+
 def test_pluto_invalid_units_override(pluto_vtk_file):
     for uo in PlutoVtkDataset.invalid_unit_combinations:
         with pytest.raises(ValueError, match=r".* cannot derive all units\n.*"):
             yt.load(
                 pluto_vtk_file["path"],
                 geometry=pluto_vtk_file["geometry"],
                 units_override=uo,
```

### Comparing `yt_idefix-1.1.1/tests/test_xdmf.py` & `yt_idefix-2.0.0/tests/test_xdmf.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/yt_idefix/_backports.py` & `yt_idefix-2.0.0/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/yt_idefix/_io/commons.py` & `yt_idefix-2.0.0/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.0.0/yt_idefix/_io/dmp_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/yt_idefix/_io/h5_io.py` & `yt_idefix-2.0.0/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.0.0/yt_idefix/_io/vtk_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -201,27 +201,30 @@
         array_shape = shape.to_cell_centered()
         assert data_type == "CELL_DATA"
 
     return Coordinates(coords[0], coords[1], coords[2], array_shape)
 
 
 def read_field_offset_index(
-    fh: BinaryIO, shape: Shape, *, upper_case_varnames: bool
+    fh: BinaryIO, shape: Shape, *, default_field_list: list[str]
 ) -> dict[str, int]:
     # assuming fh is correctly positioned (read_grid_coordinates must be called first)
     retv: dict[str, int] = {}
 
     while True:
         line = fh.readline()
         if len(line) < 2:
             break
         s = line.decode()
         datatype, varname, dtype = s.split()
 
-        if upper_case_varnames:
+        # some versions of Pluto define field names in lower case
+        # so we normalize standard output field names to upper case
+        # to avoid duplicating data in PlutoFields.known_other_fields
+        if varname.upper() in default_field_list:
             varname = varname.upper()
 
         if datatype == "SCALARS":
             next(fh)
             retv[varname] = fh.tell()
             read_single_field(fh, shape=shape, skip_data=True)
         elif datatype == "VECTORS":
```

### Comparing `yt_idefix-1.1.1/yt_idefix/data_structures.py` & `yt_idefix-2.0.0/yt_idefix/data_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,17 @@
 from yt_idefix._backports import removesuffix
 from yt_idefix._typing import UnitLike
 
 from ._io import C_io, dmp_io, h5_io, vtk_io
 from ._io.commons import IdefixFieldProperties, IdefixMetadata
 from .definitions import _PlutoBaseUnits, pluto_def_constants
 from .fields import (
-    BaseVtkFields,
     IdefixDmpFields,
     IdefixVtkFields,
-    PlutoVtkFields,
-    PlutoXdmfFields,
+    PlutoFields,
 )
 
 # import IO classes to ensure they are properly registered,
 # even though we don't call them directly
 from .io import IdefixDmpIO, IdefixVtkIO, PlutoVtkIO  # noqa
 
 if TYPE_CHECKING:
@@ -245,21 +243,14 @@
             fdata["x1"] * length_unit,
             fdata["x2"] * length_unit,
             fdata["x3"] * length_unit,
         )
 
 
 class PlutoXdmfHierarchy(GoodBoyHierarchy):
-    def _detect_output_fields(self):
-        with h5py.File(self.index_filename, mode="r") as h5f:
-            root = list(h5f.keys())[0]
-            self.field_list = [
-                (self.ds._dataset_type, str(k)) for k in list(h5f[f"{root}/vars/"])
-            ]
-
     @cached_property
     def _cell_widths(self) -> tuple[XSpans, YSpans, ZSpans]:
         cell_edges = h5_io.read_grid_coordinates(
             self.index_filename, geometry=self.ds.geometry
         )
 
         dims = self.ds.domain_dimensions
@@ -507,14 +498,15 @@
 
 class StaticPlutoDataset(GoodboyDataset, ABC):
     # PlutoDataset is already used as a class name in yt.frontends.chombo
     # the key difference being that, in this extension frontend
     # we only support static grid formats (as opposed to chombo-pluto, which is AMR)
     _default_inifile = "pluto.ini"
     _default_definitions_header = "definitions.h"
+    _field_info_class = PlutoFields
     _version_regexp = re.compile(r"\d+\.\d+\.?\d*[-\w+]*")
 
     @abstractmethod
     def _get_log_file(self) -> str:
         pass
 
     def _parse_parameter_file(self):
@@ -657,14 +649,31 @@
                 expr = re.sub(r"sqrt", "np.sqrt", expr)
                 expr = re.sub(r"log", "np.log", expr)
                 self.parameters["definitions"][unit] = eval(expr)
 
     def _get_input_parameter(self, match: re.Match) -> str:
         """Replace matched input parameters with its value"""
         key = match.group(1)
+        if key not in self.parameters.get("Parameters", {}):
+            if not os.path.exists(self._inifile):
+                warnings.warn(
+                    f"Could not find inifile ({self._inifile}). "
+                    "Inferred code units might be inaccurate\n"
+                    "To silence this warning, specify the inifile keyword argument to yt.load, "
+                    "as a path (either absolute or relative to the data file's parent directory). "
+                    f"Default is {self._default_inifile!r}. ",
+                    stacklevel=2,
+                )
+            else:
+                warnings.warn(
+                    f"Cannot get the value of {key} from {self._inifile}."
+                    "Make sure that all fields are in code units!",
+                    stacklevel=2,
+                )
+            return "1.0"
         return str(self.parameters["Parameters"][key])
 
     def _get_unit(self, match: re.Match) -> str:
         """Replace matched unit with its value"""
         key = match.group(1).lower() + "_unit"
         return str(self.parameters["definitions"].get(key, 1.0))
 
@@ -721,24 +730,23 @@
         with open(self.filename, "rb") as fh:
             md = vtk_io.read_metadata(fh)
         self.parameters.update(md)
 
         super()._parse_parameter_file()
         # from here self.geometry is assumed to be set
 
-        # some versions of Pluto define field names in lower case
-        # so we normalize to upper case to avoid duplicating data
-        # in BaseVtkFields.known_other_fields
-        normalize_varnames = self.dataset_type == "pluto-vtk"
-
         # parse the grid
         with open(self.filename, "rb") as fh:
             coords = vtk_io.read_grid_coordinates(fh, geometry=self.geometry)
             self._field_offset_index = vtk_io.read_field_offset_index(
-                fh, coords.array_shape, upper_case_varnames=normalize_varnames
+                fh,
+                coords.array_shape,
+                default_field_list=[
+                    f[0] for f in self._field_info_class.known_other_fields
+                ],
             )
         self._detected_field_list = list(self._field_offset_index.keys())
 
         self.domain_dimensions = np.array(coords.array_shape)
         self.dimensionality = np.count_nonzero(self.domain_dimensions - 1)
 
         dle = np.array([arr.min() for arr in coords.arrays], dtype="float64")
@@ -802,29 +810,28 @@
         self._periodicity = tuple(bool(p) for p in fdata["periodicity"])
 
         super()._parse_parameter_file()
 
 
 class IdefixVtkDataset(VtkMixin, IdefixDataset):
     _dataset_type = "idefix-vtk"
-    _field_info_class: type[BaseVtkFields] = IdefixVtkFields
+    _field_info_class = IdefixVtkFields
 
     @classmethod
     def _is_valid(cls, filename: str, *args, **kwargs) -> bool:
         try:
             header = vtk_io.read_header(filename)
         except Exception:
             return False
         else:
             return "Idefix" in header
 
 
 class PlutoVtkDataset(VtkMixin, StaticPlutoDataset):
     _dataset_type = "pluto-vtk"
-    _field_info_class = PlutoVtkFields
 
     @classmethod
     def _is_valid(cls, filename: str, *args, **kwargs) -> bool:
         try:
             header = vtk_io.read_header(filename)
         except Exception:
             return False
@@ -834,15 +841,14 @@
     def _get_log_file(self) -> str:
         return os.path.join(self.directory, "vtk.out")
 
 
 class PlutoXdmfDataset(StaticPlutoDataset):
     _dataset_type = "pluto-xdmf"
     _index_class = PlutoXdmfHierarchy
-    _field_info_class = PlutoXdmfFields
 
     def _get_log_file(self) -> str:
         if (suffix := re.search(r"(flt|dbl)\.h5$", self.filename)) is not None:
             return os.path.join(self.directory, f"{suffix.group()}.out")
         else:
             raise RuntimeError(
                 f"Failed to detect log file associated with {self.filename}"
@@ -864,42 +870,45 @@
         super()._parse_parameter_file()
 
         # parse the grid
         coords = h5_io.read_grid_coordinates(
             self.filename, geometry=self.parameters["definitions"]["geometry"]
         )
 
+        _default_field_list = [f[0] for f in self._field_info_class.known_other_fields]
+        with h5py.File(self.filename, mode="r") as h5f:
+            root = list(h5f.keys())[0]
+            self._detected_field_list = list(h5f[f"{root}/vars/"])
+            self._field_name_map = {}
+            # some versions of Pluto define field names in lower case
+            # so we normalize standard output field names to upper case
+            # to avoid duplicating data in PlutoFields.known_other_fields
+            for varname in self._detected_field_list:
+                if varname.upper() in _default_field_list:
+                    # The key in hdf5 is case sensitive, so we have to preserve
+                    # the info of original field names for reading data
+                    self._field_name_map[varname.upper()] = varname
+                else:
+                    self._field_name_map[varname] = varname
+
+            self._detected_field_list = self._field_name_map.keys()
+
         self.domain_dimensions = np.array(coords.array_shape)
         self.dimensionality = np.count_nonzero(self.domain_dimensions - 1)
 
         dle = np.array([arr.min() for arr in coords.arrays], dtype="float64")
         dre = np.array([arr.max() for arr in coords.arrays], dtype="float64")
 
         # temporary hack to prevent 0-width dimensions for 2D data
         dre = np.where(dre == dle, dle + 1, dre)
         self.domain_left_edge = dle
         self.domain_right_edge = dre
 
         self._periodicity = (True, True, True)
 
-    def _count_tracers(self) -> int:
-        with open(self._get_log_file()) as fh:
-            txt = fh.readlines()
-            if (match := re.search(r"\d{4}", self.filename)) is not None:
-                entry = int(match.group())
-            else:
-                raise RuntimeError(f"Failed to parse entry number from {self.filename}")
-
-            count = 0
-            # Passive tracer names in PLUTO are tr1, tr2, tr3 and so on by default
-            while f"tr{count + 1}" in txt[entry].split():
-                count += 1
-
-        return count
-
     def _read_data_header(self) -> str:
         grid_file = os.path.join(self.directory, "grid.out")
         if not os.path.isfile(grid_file):
             return ""
 
         with open(grid_file) as fh:
             body = fh.read()
```

### Comparing `yt_idefix-1.1.1/yt_idefix/definitions.py` & `yt_idefix-2.0.0/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.1/yt_idefix/io.py` & `yt_idefix-2.0.0/yt_idefix/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,18 @@
 
         with h5py.File(self.ds.filename, "r") as fh:
             ind = 0
             for chunk in chunks:
                 for grid in chunk.objs:
                     nd = 0
                     for field in fields:
-                        ftype, fname = field
-                        position = f"/Timestep_{entry}/vars/{fname}"
+                        _, fname = field
+                        position = (
+                            f"/Timestep_{entry}/vars/{self.ds._field_name_map[fname]}"
+                        )
                         field_data = fh[position][:].astype("=f8")
 
                         while field_data.ndim < 3:
                             field_data = np.expand_dims(field_data, axis=0)
 
                         # X3 X2 X1 orderding of fields in PLUTO needs to rearranged to X1 X2 X3 order in yt.
                         values = np.transpose(field_data, axes=(2, 1, 0))
```

### Comparing `yt_idefix-1.1.1/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.0.0/yt_idefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

