# Comparing `tmp/sppersist-0.1.2.tar.gz` & `tmp/sppersist-0.1.3.tar.gz`

## Comparing `sppersist-0.1.2.tar` & `sppersist-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.2/src/spPersist/__init__.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 sppersist-0.1.2/src/spPersist/read.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.2/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.2/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppersist-0.1.3/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 sppersist-0.1.3/src/spPersist/read.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-0.1.3/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sppersist-0.1.3/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 sppersist-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 sppersist-0.1.3/PKG-INFO
```

### Comparing `sppersist-0.1.2/src/spPersist/read.py` & `sppersist-0.1.3/src/spPersist/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     
     # extract files for a given sample id to the visium foler
     repository.extractall(path=data_path,
                    members=extractsample(repository, sampleid))
 
     for filename in os.listdir(data_path):
       if ttype == 'Visium':
-        if filename.endswith('.h5'):
+        if 'filtered' in filename:
           gex = data_path + filename
         if 'positions' in filename:
           pos = data_path + filename
       elif ttype == 'MERFISH':
         if 'cell_by_gene' in filename:
           gex = data_path + filename
         if 'cell_metadata' in filename:
```

### Comparing `sppersist-0.1.2/LICENSE` & `sppersist-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-0.1.2/pyproject.toml` & `sppersist-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial analysis package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-0.1.2/PKG-INFO` & `sppersist-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.1.2
+Version: 0.1.3
 Summary: Spatial analysis package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

