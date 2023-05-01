# Comparing `tmp/sppersist-0.1.1.tar.gz` & `tmp/sppersist-0.1.2.tar.gz`

## Comparing `sppersist-0.1.1.tar` & `sppersist-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.1/src/spPersist/__init__.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 sppersist-0.1.1/src/spPersist/read.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.1/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.1/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.2/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 sppersist-0.1.2/src/spPersist/read.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.2/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.2/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.2/PKG-INFO
```

### Comparing `sppersist-0.1.1/src/spPersist/read.py` & `sppersist-0.1.2/src/spPersist/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 import anndata
 
 
 
 def visium(gex: str, pos: str):
   '''
   visium takes cell by gene count file name gex and tissue position lists pos, 
-  and return an annotated data object with spatial coordinates.
+  and return an annotated data object with spatial coordinates in obsm.
   Note that gex and pos should be formatted as Spance Ranger outputs.
   '''
   ad = sc.read_10x_h5(gex)
   coords = pd.read_csv(pos,index_col=0)
   coords.columns = ["in_tissue", "array_row", "array_col", "pxl_col_in_fullres", "pxl_row_in_fullres"]
   ad.obs = pd.merge(ad.obs, coords, how="left", left_index=True, right_index=True)
   ad.obsm['spatial'] = ad.obs[["pxl_row_in_fullres", "pxl_col_in_fullres"]].values
   ad.obs.drop(columns=["pxl_row_in_fullres", "pxl_col_in_fullres"], inplace=True)
   return ad
 
 def merfish(gex: str, pos: str):
   '''
   merfish takes cell by gene count file name gex and
   metadata file pos that contains spatial coordinates, 
-  and return an annotated data object with spatial coordinates.
+  and return an annotated data object with spatial coordinates in obsm.
   Note that gex and pos should be formatted as Vizgen outputs.
   '''
   adata = anndata.AnnData(pd.read_csv(gex, header=0, index_col=0))
   
 
   # fmt: off
   coords = pd.read_csv(pos, header=0, index_col=0)
```

### Comparing `sppersist-0.1.1/LICENSE` & `sppersist-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.1/pyproject.toml` & `sppersist-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.1.1/PKG-INFO` & `sppersist-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.1.1
+Version: 0.1.2
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

