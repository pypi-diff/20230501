# Comparing `tmp/sppersist-0.1.0.tar.gz` & `tmp/sppersist-0.1.1.tar.gz`

## Comparing `sppersist-0.1.0.tar` & `sppersist-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.0/src/spPersist/__init__.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 sppersist-0.1.0/src/spPersist/read.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.0/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.0/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.1/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 sppersist-0.1.1/src/spPersist/read.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.1/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.1/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.1/PKG-INFO
```

### Comparing `sppersist-0.1.0/src/spPersist/read.py` & `sppersist-0.1.1/src/spPersist/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,20 +117,18 @@
     raise ValueError('ttype is not either Visium or MERFISH.')
 
   sampleids = [s.split('_')[0] for s in samplelist]
   
   # helper function for extracting a sample
   def extractsample(members, sampleid):
     for member in members:
-      if tarfile.is_tarfile(filename):
+      if member.isfile():
         fname = member.name
-      elif zipfile.is_zipfile(filename):
-        fname = member
       else:
-        raise ValueError('filename is not tar or zip file.')
+        fname = member
 
       if sampleid in fname:
         yield member
 
   # helper function for emptying a given directory
   def emptydir(folder):
     for filename in os.listdir(folder):
@@ -183,8 +181,8 @@
     else:
       adata = merfish(gex, pos)
 
     savefilename = sampleid + '.h5'
     adata.write_h5ad(h5_path+savefilename)
   
   # zip h5 files
-  shutil.make_archive(gse+'_h5', 'zip', h5_path)
+  shutil.make_archive('h5', 'zip', h5_path)
```

### Comparing `sppersist-0.1.0/LICENSE` & `sppersist-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.0/pyproject.toml` & `sppersist-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.1.0/PKG-INFO` & `sppersist-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.1.0
+Version: 0.1.1
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

