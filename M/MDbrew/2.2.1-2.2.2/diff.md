# Comparing `tmp/MDbrew-2.2.1.tar.gz` & `tmp/MDbrew-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.2.1.tar", last modified: Mon May  1 09:20:40 2023, max compression
+gzip compressed data, was "MDbrew-2.2.2.tar", last modified: Mon May  1 13:29:28 2023, max compression
```

## Comparing `MDbrew-2.2.1.tar` & `MDbrew-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,35 @@
-drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:17:26.632754 MDbrew-2.2.1/
--rw-------   0 minu928   (1216) minu928   (1216)       24 2023-05-01 06:01:04.000000 MDbrew-2.2.1/MANIFEST.in
-drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:17:26.626088 MDbrew-2.2.1/MDbrew/
--rw-------   0 minu928   (1216) minu928   (1216)      181 2023-05-01 09:12:21.000000 MDbrew-2.2.1/MDbrew/__init__.py
--rw-------   0 minu928   (1216) minu928   (1216)      265 2023-05-01 09:12:21.000000 MDbrew-2.2.1/MDbrew/_type.py
--rw-rw-r--   0 minu928   (1216) minu928   (1216)     2822 2023-05-01 09:12:21.000000 MDbrew-2.2.1/MDbrew/brewery.py
-drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 09:17:26.632754 MDbrew-2.2.1/MDbrew.egg-info/
--rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/PKG-INFO
--rw-------   0 minu928   (1216) minu928   (1216)      248 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/SOURCES.txt
--rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/dependency_links.txt
--rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 09:13:44.000000 MDbrew-2.2.1/MDbrew.egg-info/not-zip-safe
--rw-------   0 minu928   (1216) minu928   (1216)        7 2023-05-01 09:17:26.000000 MDbrew-2.2.1/MDbrew.egg-info/top_level.txt
--rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 09:17:26.632754 MDbrew-2.2.1/PKG-INFO
--rw-------   0 minu928   (1216) minu928   (1216)       58 2023-05-01 06:01:04.000000 MDbrew-2.2.1/requirement.txt
--rw-------   0 minu928   (1216) minu928   (1216)       79 2023-05-01 09:17:26.632754 MDbrew-2.2.1/setup.cfg
--rw-------   0 minu928   (1216) minu928   (1216)      631 2023-05-01 09:17:00.000000 MDbrew-2.2.1/setup.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.796932 MDbrew-2.2.2/
+-rw-------   0 minu928   (1216) minu928   (1216)       24 2023-05-01 11:46:47.000000 MDbrew-2.2.2/MANIFEST.in
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.770265 MDbrew-2.2.2/MDbrew/
+-rw-rw----   0 minu928   (1216) minu928   (1216)      225 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/__init__.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.783599 MDbrew-2.2.2/MDbrew/analysis/
+-rw-------   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:22:45.000000 MDbrew-2.2.2/MDbrew/analysis/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     4065 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/analysis/msd.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     5245 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/analysis/rdf.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.786932 MDbrew-2.2.2/MDbrew/application/
+-rw-------   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:22:46.000000 MDbrew-2.2.2/MDbrew/application/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     9051 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/application/brewcp2k.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     3657 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/brewery.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.790266 MDbrew-2.2.2/MDbrew/filetype/
+-rw-------   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:22:54.000000 MDbrew-2.2.2/MDbrew/filetype/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      741 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/filetype/lmps.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      979 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/filetype/openerinterface.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      791 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/filetype/pdb.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     1304 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/filetype/vasp.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      454 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/filetype/xyz.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.796932 MDbrew-2.2.2/MDbrew/tool/
+-rw-------   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:22:47.000000 MDbrew-2.2.2/MDbrew/tool/__init__.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     3545 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/tool/colorfont.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)      851 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/tool/decorator.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     1037 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/tool/doctor.py
+-rw-rw----   0 minu928   (1216) minu928   (1216)     1563 2023-05-01 13:18:31.000000 MDbrew-2.2.2/MDbrew/tool/spacer.py
+drwx--S---   0 minu928   (1216) minu928   (1216)        0 2023-05-01 13:26:13.776932 MDbrew-2.2.2/MDbrew.egg-info/
+-rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 13:26:13.000000 MDbrew-2.2.2/MDbrew.egg-info/PKG-INFO
+-rw-------   0 minu928   (1216) minu928   (1216)      643 2023-05-01 13:26:13.000000 MDbrew-2.2.2/MDbrew.egg-info/SOURCES.txt
+-rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 13:26:13.000000 MDbrew-2.2.2/MDbrew.egg-info/dependency_links.txt
+-rw-------   0 minu928   (1216) minu928   (1216)        1 2023-05-01 13:26:13.000000 MDbrew-2.2.2/MDbrew.egg-info/not-zip-safe
+-rw-------   0 minu928   (1216) minu928   (1216)        7 2023-05-01 13:26:13.000000 MDbrew-2.2.2/MDbrew.egg-info/top_level.txt
+-rw-------   0 minu928   (1216) minu928   (1216)      332 2023-05-01 13:26:13.796932 MDbrew-2.2.2/PKG-INFO
+-rw-------   0 minu928   (1216) minu928   (1216)       58 2023-05-01 11:46:47.000000 MDbrew-2.2.2/requirement.txt
+-rw-------   0 minu928   (1216) minu928   (1216)       79 2023-05-01 13:26:13.796932 MDbrew-2.2.2/setup.cfg
+-rw-------   0 minu928   (1216) minu928   (1216)      631 2023-05-01 13:25:30.000000 MDbrew-2.2.2/setup.py
```

### Comparing `MDbrew-2.2.1/MDbrew/brewery.py` & `MDbrew-2.2.2/MDbrew/brewery.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,74 @@
 import os
 import numpy as np
 import pandas as pd
-from .tool.colorfont import ColorFont
-from .tool.deco import color_print
+from .tool.colorfont import color
+from .tool.decorator import color_print
 from .filetype.lmps import lmpsOpener
 from .filetype.pdb import pdbOpener
 from .filetype.vasp import vaspOpener
 from .filetype.xyz import xyzOpener
 
 
-color = ColorFont()
-
 # Extractor of Something
 class Brewery(object):
     __support_fmt_opener__ = {"auto": None, "pdb": pdbOpener, "xyz": xyzOpener, "vasp": vaspOpener, "lmps": lmpsOpener}
-    __dtype__ = "float64"
-    __printing_option = {
-        "opener": f" #LOAD  {color.font_yellow}Opener{color.reset}",
-        "brew": f" #BREW  {color.font_yellow}DATA{color.reset}",
+    __printing_option__ = {
+        "opener": f" #LOAD  {color.font_yellow}Files      {color.reset}",
+        "b_brewing": f" #BREW  {color.font_yellow}Something  {color.reset}",
+        "b_coords": f" #BREW  {color.font_yellow}Coords     {color.reset}",
+        "b_atominfo": f" #BREW  {color.font_yellow}Atom Info  {color.reset}",
     }
 
-    def __init__(self, path: str, ordered: bool = True, fmt: str = "auto") -> None:
-        self.check_fmt(fmt=fmt)
-        self.check_path(path=path)
-        self.load_opener(path=path)
+    def __init__(self, path: str, fmt: str = "auto") -> None:
+        self.__check_fmt(fmt=fmt)
+        self.__check_path(path=path)
+        self.__load_opener(path=path)
 
-    @color_print(name=__printing_option["opener"])
-    def load_opener(self, path):
+    @color_print(name=__printing_option__["opener"])
+    def __load_opener(self, path):
         self._opener = self.__support_fmt_opener__[self.fmt](path=path)
         self.database = self._opener.database
         self.columns = self._opener.column
         self.box_size = self._opener.box_size
         self.frame_num = self._opener.frame_num
-        self.dim = 3
 
-    def check_fmt(self, fmt: str):
+    def __check_fmt(self, fmt: str):
         assert fmt in self.__support_fmt_opener__, f"fmt should be in {list(self.__support_fmt_opener__.keys())}"
         self.fmt = fmt
 
-    def check_path(self, path):
+    def __check_path(self, path):
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         if self.fmt == "auto":
             file_name = path.split("/")[-1]
             file_fmt = file_name.split(".")[-1]
             self.fmt = file_fmt
 
     def query(self, ment: str = None):
         for data in self.database:
             df_data = pd.DataFrame(data=data, columns=self.columns)
             yield df_data.query(ment) if ment is not None else df_data
 
-    @color_print(name=__printing_option["brew"])
-    def brew(self, ment: str = None, max_iter: str = None, xyz_list: list[str] = None):
+    @color_print(name=__printing_option__["b_brewing"])
+    def brew(self, ment: str = None, cols: list[str] = None, max_iter: int = None, dtype: str = "float32"):
+        return self.__brewing__(ment=ment, cols=cols, max_iter=max_iter, dtype=dtype)
+
+    @color_print(name=__printing_option__["b_coords"])
+    def brew_coords(self, ment: str = None, xyz_list: list[str] = None, max_iter: int = None, dtype: str = "float32"):
+        xyz_list = ["x", "y", "z"] if xyz_list is None else xyz_list
+        return self.__brewing__(ment=ment, cols=xyz_list, max_iter=max_iter, dtype=dtype)
+
+    @color_print(name=__printing_option__["b_atominfo"])
+    def brew_atom_info(self, cols: str = ["atom"], max_iter: int = 1, dtype: str = "str"):
+        return np.unique(self.__brewing__(ment=None, cols=cols, max_iter=max_iter, dtype=dtype), return_counts=True)
+
+    def __brewing__(self, ment: str = None, cols: list[str] = None, max_iter: int = None, dtype: str = "float32"):
         max_iter = self.frame_num if max_iter is None else max_iter
         assert max_iter <= self.frame_num, f"max_iter is larger than {self.frame_num}, not {max_iter}"
-        
-        xyz_list = ["x", "y", "z"] if xyz_list is None else xyz_list
-        assert xyz_list[0] in self.columns, f"Check your xyz_list in argument, not xyz_list = {xyz_list}"
-        
-        flatten_database = np.reshape(self.database, (-1, len(self.columns)))
+        assert set(cols) <= set(
+            self.columns
+        ), f"cols should be subset of columns, your cols: {cols} || columns: {self.columns}"
+        flatten_database = np.reshape(self.database[:max_iter], (-1, len(self.columns)))
         flatten_database = pd.DataFrame(data=flatten_database, columns=self.columns)
         flatten_database = flatten_database.query(ment) if ment is not None else flatten_database
-        flatten_position = flatten_database.loc[:, xyz_list].to_numpy(dtype=self.__dtype__)
-        flatten_position = flatten_position.reshape([self.frame_num, -1, self.dim])
-        return flatten_position
+        flatten_database = flatten_database.loc[:, cols].to_numpy(dtype=dtype)
+        return flatten_database.reshape([max_iter, -1, len(cols)])
```

### Comparing `MDbrew-2.2.1/setup.py` & `MDbrew-2.2.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.2.1",
+    version="2.2.2",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
-    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.1.6.tar.gz",
+    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.2.2.tar.gz",
     install_requies=[
         "numpy>=1.0.0",
         "pandas>=1.0.0",
         "matplotlib>=1.0.0",
         "tqdm>=1.0.0",
     ],
     description="Postprocessing tools for the MD simulation results (ex. lammps)",
```

