# Comparing `tmp/denmune-1.15.9.tar.gz` & `tmp/denmune-1.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-1.15.9.tar", last modified: Mon May  1 19:14:37 2023, max compression
+gzip compressed data, was "denmune-1.16.0.tar", last modified: Mon May  1 19:19:36 2023, max compression
```

## Comparing `denmune-1.15.9.tar` & `denmune-1.16.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:14:37.700586 denmune-1.15.9/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.15.9/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.15.9/MANIFEST.in
--rw-rw-rw-   0        0        0    31200 2023-05-01 19:14:37.701568 denmune-1.15.9/PKG-INFO
--rw-rw-rw-   0        0        0    30529 2023-05-01 19:12:50.000000 denmune-1.15.9/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.15.9/pyproject.toml
--rw-rw-rw-   0        0        0      810 2023-05-01 19:14:37.704584 denmune-1.15.9/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-05-01 00:42:54.000000 denmune-1.15.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:14:37.634374 denmune-1.15.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 19:14:37.672688 denmune-1.15.9/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.15.9/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.15.9/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:14:37.697568 denmune-1.15.9/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    31200 2023-05-01 19:14:37.000000 denmune-1.15.9/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-01 19:14:37.000000 denmune-1.15.9/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:14:37.000000 denmune-1.15.9/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-05-01 19:14:37.000000 denmune-1.15.9/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 19:14:37.000000 denmune-1.15.9/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 19:19:36.438385 denmune-1.16.0/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    31197 2023-05-01 19:19:36.439379 denmune-1.16.0/PKG-INFO
+-rw-rw-rw-   0        0        0    30526 2023-05-01 19:19:01.000000 denmune-1.16.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.0/pyproject.toml
+-rw-rw-rw-   0        0        0      810 2023-05-01 19:19:36.441382 denmune-1.16.0/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-05-01 00:42:54.000000 denmune-1.16.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:19:36.383332 denmune-1.16.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 19:19:36.417352 denmune-1.16.0/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.0/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.16.0/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:19:36.435386 denmune-1.16.0/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    31197 2023-05-01 19:19:36.000000 denmune-1.16.0/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-01 19:19:36.000000 denmune-1.16.0/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:19:36.000000 denmune-1.16.0/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-05-01 19:19:36.000000 denmune-1.16.0/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 19:19:36.000000 denmune-1.16.0/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-1.15.9/LICENSE` & `denmune-1.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-1.15.9/PKG-INFO` & `denmune-1.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.15.9
+Version: 1.16.0
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,15 @@
 
 
 Collaborative Test Drive (New)
 ------------------------------
 
 Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using my capsule on CodeOcean, your collaborative test drive.
 
-https://codeocean.com/capsule/3560333/tree/v2
+https://codeocean.com/capsule/3560333/tree
 
 
 
 
 Scientific Work
 ---------------------
```

### Comparing `denmune-1.15.9/README.md` & `denmune-1.16.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 Collaborative Test Drive (New)
 ------------------------------
 
 Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using my capsule on CodeOcean, your collaborative test drive.
 
-https://codeocean.com/capsule/3560333/tree/v2
+https://codeocean.com/capsule/3560333/tree
 
 
 
 
 Scientific Work
 ---------------------
```

### Comparing `denmune-1.15.9/setup.cfg` & `denmune-1.16.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 312e 3135 2e39 0d0a 6175  ion = 1.15.9..au
+00000020: 696f 6e20 3d20 312e 3136 2e30 0d0a 6175  ion = 1.16.0..au
 00000030: 7468 6f72 203d 2044 722e 204d 6f68 616d  thor = Dr. Moham
 00000040: 6564 2041 6c69 2041 6262 6173 2026 2050  ed Ali Abbas & P
 00000050: 726f 662e 2041 6d69 6e20 2053 686f 756b  rof. Amin  Shouk
 00000060: 7279 0d0a 6175 7468 6f72 5f65 6d61 696c  ry..author_email
 00000070: 203d 206d 6f68 616d 6564 2e61 6c79 6162   = mohamed.alyab
 00000080: 6261 7340 6f75 746c 6f6f 6b2e 636f 6d0d  bas@outlook.com.
 00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
```

### Comparing `denmune-1.15.9/src/denmune/denmune.py` & `denmune-1.16.0/src/denmune/denmune.py`

 * *Files identical despite different names*

### Comparing `denmune-1.15.9/src/denmune.egg-info/PKG-INFO` & `denmune-1.16.0/src/denmune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.15.9
+Version: 1.16.0
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,15 @@
 
 
 Collaborative Test Drive (New)
 ------------------------------
 
 Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using my capsule on CodeOcean, your collaborative test drive.
 
-https://codeocean.com/capsule/3560333/tree/v2
+https://codeocean.com/capsule/3560333/tree
 
 
 
 
 Scientific Work
 ---------------------
```

