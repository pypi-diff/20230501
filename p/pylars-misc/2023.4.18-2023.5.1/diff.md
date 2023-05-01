# Comparing `tmp/pylars_misc-2023.4.18.tar.gz` & `tmp/pylars_misc-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylars_misc-2023.4.18.tar", last modified: Tue Apr 18 10:22:51 2023, max compression
+gzip compressed data, was "pylars_misc-2023.5.1.tar", last modified: Mon May  1 20:00:07 2023, max compression
```

## Comparing `pylars_misc-2023.4.18.tar` & `pylars_misc-2023.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.381293 pylars_misc-2023.4.18/
--rw-r--r--   0 root         (0) root         (0)      229 2023-04-18 10:22:51.379299 pylars_misc-2023.4.18/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-18 10:22:10.000000 pylars_misc-2023.4.18/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 10:22:51.382295 pylars_misc-2023.4.18/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.250928 pylars_misc-2023.4.18/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.286963 pylars_misc-2023.4.18/src/pylars_misc/
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-14 19:18:37.000000 pylars_misc-2023.4.18/src/pylars_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-03-30 10:25:11.000000 pylars_misc-2023.4.18/src/pylars_misc/pylars_misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:22:51.358972 pylars_misc-2023.4.18/src/pylars_misc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      229 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      229 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-18 10:22:51.000000 pylars_misc-2023.4.18/src/pylars_misc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:00:07.555537 pylars_misc-2023.5.1/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-01 20:00:07.553534 pylars_misc-2023.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-01 19:58:42.000000 pylars_misc-2023.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:00:07.556537 pylars_misc-2023.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:00:07.426967 pylars_misc-2023.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:00:07.469308 pylars_misc-2023.5.1/src/pylars_misc/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-03-14 19:18:37.000000 pylars_misc-2023.5.1/src/pylars_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-05-01 19:56:05.000000 pylars_misc-2023.5.1/src/pylars_misc/pylars_misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:00:07.536104 pylars_misc-2023.5.1/src/pylars_misc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-01 20:00:07.000000 pylars_misc-2023.5.1/src/pylars_misc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-01 20:00:07.000000 pylars_misc-2023.5.1/src/pylars_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:00:07.000000 pylars_misc-2023.5.1/src/pylars_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-01 20:00:07.000000 pylars_misc-2023.5.1/src/pylars_misc.egg-info/top_level.txt
```

### Comparing `pylars_misc-2023.4.18/src/pylars_misc/pylars_misc.py` & `pylars_misc-2023.5.1/src/pylars_misc/pylars_misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,59 @@
 patched in.  It's all python specific so isn't really an improvement to the Rust
 based underlying polars package.
 """
 
 import polars as pl
 import fsspec
 import os
+import pyarrow.dataset as ds
+import numpy as np
 
 abfs = fsspec.filesystem('abfss', connection_string=os.environ['Synblob'])
 
 def write_pq(self, REMOTE_PATH, **kwargs):
     with abfs.open(REMOTE_PATH, "wb") as file_pointer:
         self.write_parquet(file_pointer, **kwargs)
         
 pl.DataFrame.write_pq=write_pq
 
 def read_pq(REMOTE_PATH, **kwargs):
     with abfs.open(REMOTE_PATH, "rb") as file_pointer:
         return pl.read_parquet(file_pointer, **kwargs)
 pl.read_pq=read_pq
+del read_pq
+
+def scan_ds(REMOTE_PATH, **kwargs):
+    return pl.scan_pyarrow_dataset(
+        ds.dataset(REMOTE_PATH, 
+                   filesystem=abfs,
+                   partitioning='hive'))
+pl.scan_ds=scan_ds
+
+def sortD(self, sortdict, **kwargs):
+    return self.sort(list(sortdict.keys()), descending=list(sortdict.values()), **kwargs)
+pl.DataFrame.sortD=sortD
+del sortD
+
+def to_np_yX(self):
+    npY=np.empty(
+        self.height, 
+        [(self.columns[0], self.head(0).get_column(self.columns[0]).to_numpy().dtype.str)]
+        )
+    npY[self.columns[0]]=self.get_column(self.columns[0]).to_numpy()
+    npX=np.empty(
+        self.height,
+        [(x, self.head(0).get_column(x).to_numpy().dtype.str) for x in self.columns[1:]]
+    )
+    for x in self.columns[1:]:
+        npX[x]=self.get_column(x).to_numpy()
+    return npY, npX
+pl.DataFrame.to_np_yX=to_np_yX
+
+
 try:
     import ipy_table as pt  
     def to_html(self):
         myL=[tuple(x for x in self.columns)]
         myL.extend(self.rows())
         return pt.IpyTable(myL)
     pl.DataFrame.to_html=to_html
```

