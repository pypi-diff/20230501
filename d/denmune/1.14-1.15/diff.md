# Comparing `tmp/denmune-1.14.tar.gz` & `tmp/denmune-1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-1.14.tar", last modified: Sat Apr 29 23:37:29 2023, max compression
+gzip compressed data, was "denmune-1.15.tar", last modified: Sun Apr 30 00:21:58 2023, max compression
```

## Comparing `denmune-1.14.tar` & `denmune-1.15.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:37:29.751662 denmune-1.14/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.14/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.14/MANIFEST.in
--rw-rw-rw-   0        0        0    31198 2023-04-29 23:37:29.752666 denmune-1.14/PKG-INFO
--rw-rw-rw-   0        0        0    30529 2023-04-29 21:17:35.000000 denmune-1.14/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.14/pyproject.toml
--rw-rw-rw-   0        0        0      808 2023-04-29 23:37:29.754662 denmune-1.14/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-04-29 23:36:12.000000 denmune-1.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:37:29.670793 denmune-1.14/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 23:37:29.719783 denmune-1.14/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.14/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39275 2022-05-12 03:42:03.000000 denmune-1.14/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:37:29.747538 denmune-1.14/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    31198 2023-04-29 23:37:29.000000 denmune-1.14/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-29 23:37:29.000000 denmune-1.14/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 23:37:29.000000 denmune-1.14/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-04-29 23:37:29.000000 denmune-1.14/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 23:37:29.000000 denmune-1.14/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 00:21:58.287160 denmune-1.15/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.15/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.15/MANIFEST.in
+-rw-rw-rw-   0        0        0    31198 2023-04-30 00:21:58.289164 denmune-1.15/PKG-INFO
+-rw-rw-rw-   0        0        0    30529 2023-04-29 21:17:35.000000 denmune-1.15/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.15/pyproject.toml
+-rw-rw-rw-   0        0        0      808 2023-04-30 00:21:58.297917 denmune-1.15/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-04-29 23:36:12.000000 denmune-1.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:21:58.152764 denmune-1.15/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 00:21:58.205735 denmune-1.15/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.15/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.15/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-04-30 00:21:58.280715 denmune-1.15/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    31198 2023-04-30 00:21:57.000000 denmune-1.15/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-30 00:21:58.000000 denmune-1.15/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 00:21:57.000000 denmune-1.15/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-04-30 00:21:57.000000 denmune-1.15/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 00:21:58.000000 denmune-1.15/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-1.14/LICENSE` & `denmune-1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-1.14/PKG-INFO` & `denmune-1.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.14
+Version: 1.15
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `denmune-1.14/README.md` & `denmune-1.15/README.md`

 * *Files identical despite different names*

### Comparing `denmune-1.14/setup.cfg` & `denmune-1.15/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 312e 3134 0d0a 6175 7468  ion = 1.14..auth
+00000020: 696f 6e20 3d20 312e 3135 0d0a 6175 7468  ion = 1.15..auth
 00000030: 6f72 203d 2044 722e 204d 6f68 616d 6564  or = Dr. Mohamed
 00000040: 2041 6c69 2041 6262 6173 2026 2050 726f   Ali Abbas & Pro
 00000050: 662e 2041 6d69 6e20 2053 686f 756b 7279  f. Amin  Shoukry
 00000060: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000070: 206d 6f68 616d 6564 2e61 6c79 6162 6261   mohamed.alyabba
 00000080: 7340 6f75 746c 6f6f 6b2e 636f 6d0d 0a64  s@outlook.com..d
 00000090: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
```

### Comparing `denmune-1.14/src/denmune/denmune.py` & `denmune-1.15/src/denmune/denmune.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
               train_truth = train_truth.to_numpy()
               train_truth = train_truth.copy(order='C')
           elif type(train_truth == np.ndarray and not train_truth.data.c_contiguous):  
             train_truth = train_truth.copy(order='C')   
 
         if test_data is not None:
           if isinstance(test_data, pd.DataFrame):
-            print ('I am in One')
             test_data = test_data.to_numpy()
             test_data = test_data.copy(order='C')
           elif type(test_data == np.ndarray and not test_data.data.c_contiguous): 
             print ('I am in two') 
             test_data = test_data.copy(order='C')
     
         if test_truth is not None:
```

### Comparing `denmune-1.14/src/denmune.egg-info/PKG-INFO` & `denmune-1.15/src/denmune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.14
+Version: 1.15
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

