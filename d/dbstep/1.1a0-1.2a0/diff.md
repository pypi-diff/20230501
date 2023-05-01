# Comparing `tmp/dbstep-1.1a0.tar.gz` & `tmp/dbstep-1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbstep-1.1a0.tar", last modified: Thu Apr  1 21:25:29 2021, max compression
+gzip compressed data, was "dist/dbstep-1.2a0.tar", last modified: Mon Apr 19 21:59:43 2021, max compression
```

## Comparing `dbstep-1.1a0.tar` & `dbstep-1.2a0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-01 21:25:29.832144 dbstep-1.1a0/
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1099 2020-11-30 20:47:12.000000 dbstep-1.1a0/LICENSE.txt
--rw-r--r--   0 guilianluchini   (501) staff       (20)       73 2020-11-30 17:57:24.000000 dbstep-1.1a0/MANIFEST.in
--rw-r--r--   0 guilianluchini   (501) staff       (20)    12295 2021-04-01 21:25:29.832303 dbstep-1.1a0/PKG-INFO
--rw-r--r--   0 guilianluchini   (501) staff       (20)    10257 2021-04-01 21:12:29.000000 dbstep-1.1a0/README.md
-drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-01 21:25:29.814152 dbstep-1.1a0/dbstep/
--rw-r--r--   0 guilianluchini   (501) staff       (20)    28187 2021-04-01 21:13:36.000000 dbstep-1.1a0/dbstep/Dbstep.py
--rw-r--r--   0 guilianluchini   (501) staff       (20)      138 2020-08-25 17:52:43.000000 dbstep-1.1a0/dbstep/__init__.py
--rw-r--r--   0 guilianluchini   (501) staff       (20)      407 2019-11-06 21:12:25.000000 dbstep-1.1a0/dbstep/__main__.py
--rw-r--r--   0 guilianluchini   (501) staff       (20)     9543 2020-09-11 17:13:17.000000 dbstep-1.1a0/dbstep/calculator.py
-drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-01 21:25:29.831558 dbstep-1.1a0/dbstep/examples/
--rw-r--r--   0 guilianluchini   (501) staff       (20)     6148 2021-04-01 21:00:29.000000 dbstep-1.1a0/dbstep/examples/.DS_Store
--rw-r--r--   0 guilianluchini   (501) staff       (20)      351 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/1Nap.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      922 2019-08-16 22:44:08.000000 dbstep-1.1a0/dbstep/examples/35diMePh.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      625 2019-08-16 22:44:43.000000 dbstep-1.1a0/dbstep/examples/4ClPh.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      822 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/4MeOPh.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      772 2019-08-16 22:44:25.000000 dbstep-1.1a0/dbstep/examples/4MePh.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1308 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/Ad.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1239 2019-11-06 20:30:02.000000 dbstep-1.1a0/dbstep/examples/Benchmark.csv
--rw-r--r--   0 guilianluchini   (501) staff       (20)      769 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/Bn.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1163 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/CEt3.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      724 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/CH2iPr.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      871 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/CH2tBu.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      870 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/CHEt2.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1164 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/CHPr2.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1165 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/CHiPr2.xyz
--rwxr-xr-x   0 guilianluchini   (501) staff       (20)      114 2019-11-07 16:42:00.000000 dbstep-1.1a0/dbstep/examples/DBLOOP
--rw-r--r--   0 guilianluchini   (501) staff       (20)      164 2020-08-24 22:14:57.000000 dbstep-1.1a0/dbstep/examples/Et.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      130 2019-08-16 22:46:19.000000 dbstep-1.1a0/dbstep/examples/H.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      108 2019-08-18 19:31:02.000000 dbstep-1.1a0/dbstep/examples/Me.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      622 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/Ph.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      918 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/cHex.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      574 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/iPr.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      246 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/nBu.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)      574 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/nPr.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)       64 2021-04-01 21:14:13.000000 dbstep-1.1a0/dbstep/examples/smiles.txt
--rw-r--r--   0 guilianluchini   (501) staff       (20)      721 2019-08-16 22:27:23.000000 dbstep-1.1a0/dbstep/examples/tBu.xyz
--rw-r--r--   0 guilianluchini   (501) staff       (20)     6761 2021-04-01 20:51:34.000000 dbstep-1.1a0/dbstep/graph.py
--rw-r--r--   0 guilianluchini   (501) staff       (20)     9747 2020-09-17 17:39:04.000000 dbstep-1.1a0/dbstep/parse_data.py
--rw-r--r--   0 guilianluchini   (501) staff       (20)    15058 2020-10-20 23:56:09.000000 dbstep-1.1a0/dbstep/sterics.py
--rw-r--r--   0 guilianluchini   (501) staff       (20)     3931 2020-01-17 22:34:22.000000 dbstep-1.1a0/dbstep/writer.py
-drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-01 21:25:29.816525 dbstep-1.1a0/dbstep.egg-info/
--rw-r--r--   0 guilianluchini   (501) staff       (20)    12295 2021-04-01 21:25:29.000000 dbstep-1.1a0/dbstep.egg-info/PKG-INFO
--rw-r--r--   0 guilianluchini   (501) staff       (20)     1004 2021-04-01 21:25:29.000000 dbstep-1.1a0/dbstep.egg-info/SOURCES.txt
--rw-r--r--   0 guilianluchini   (501) staff       (20)        1 2021-04-01 21:25:29.000000 dbstep-1.1a0/dbstep.egg-info/dependency_links.txt
--rw-r--r--   0 guilianluchini   (501) staff       (20)       24 2021-04-01 21:25:29.000000 dbstep-1.1a0/dbstep.egg-info/requires.txt
--rw-r--r--   0 guilianluchini   (501) staff       (20)        7 2021-04-01 21:25:29.000000 dbstep-1.1a0/dbstep.egg-info/top_level.txt
--rw-r--r--   0 guilianluchini   (501) staff       (20)      108 2021-04-01 21:25:29.832616 dbstep-1.1a0/setup.cfg
--rw-r--r--   0 guilianluchini   (501) staff       (20)      972 2021-04-01 21:24:46.000000 dbstep-1.1a0/setup.py
+drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-19 21:59:43.898281 dbstep-1.2a0/
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1099 2020-11-30 20:47:12.000000 dbstep-1.2a0/LICENSE.txt
+-rw-r--r--   0 guilianluchini   (501) staff       (20)       73 2020-11-30 17:57:24.000000 dbstep-1.2a0/MANIFEST.in
+-rw-r--r--   0 guilianluchini   (501) staff       (20)    12407 2021-04-19 21:59:43.898439 dbstep-1.2a0/PKG-INFO
+-rw-r--r--   0 guilianluchini   (501) staff       (20)    10353 2021-04-19 21:57:22.000000 dbstep-1.2a0/README.md
+drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-19 21:59:43.891838 dbstep-1.2a0/dbstep/
+-rw-r--r--   0 guilianluchini   (501) staff       (20)    28211 2021-04-14 20:35:49.000000 dbstep-1.2a0/dbstep/Dbstep.py
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      138 2020-08-25 17:52:43.000000 dbstep-1.2a0/dbstep/__init__.py
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      407 2019-11-06 21:12:25.000000 dbstep-1.2a0/dbstep/__main__.py
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     9543 2020-09-11 17:13:17.000000 dbstep-1.2a0/dbstep/calculator.py
+drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-19 21:59:43.898120 dbstep-1.2a0/dbstep/examples/
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     6148 2021-04-06 22:23:59.000000 dbstep-1.2a0/dbstep/examples/.DS_Store
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      351 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/1Nap.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      922 2019-08-16 22:44:08.000000 dbstep-1.2a0/dbstep/examples/35diMePh.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      625 2019-08-16 22:44:43.000000 dbstep-1.2a0/dbstep/examples/4ClPh.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      822 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/4MeOPh.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      772 2019-08-16 22:44:25.000000 dbstep-1.2a0/dbstep/examples/4MePh.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1308 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/Ad.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1239 2019-11-06 20:30:02.000000 dbstep-1.2a0/dbstep/examples/Benchmark.csv
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      769 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/Bn.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1163 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/CEt3.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      724 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/CH2iPr.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      871 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/CH2tBu.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      870 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/CHEt2.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1164 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/CHPr2.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1165 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/CHiPr2.xyz
+-rwxr-xr-x   0 guilianluchini   (501) staff       (20)      110 2021-04-06 15:47:09.000000 dbstep-1.2a0/dbstep/examples/DBLOOP
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      164 2020-08-24 22:14:57.000000 dbstep-1.2a0/dbstep/examples/Et.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      130 2019-08-16 22:46:19.000000 dbstep-1.2a0/dbstep/examples/H.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      108 2019-08-18 19:31:02.000000 dbstep-1.2a0/dbstep/examples/Me.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      622 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/Ph.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      918 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/cHex.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      574 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/iPr.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      246 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/nBu.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      574 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/nPr.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)       64 2021-04-01 21:14:13.000000 dbstep-1.2a0/dbstep/examples/smiles.txt
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      721 2019-08-16 22:27:23.000000 dbstep-1.2a0/dbstep/examples/tBu.xyz
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     7040 2021-04-07 17:14:32.000000 dbstep-1.2a0/dbstep/graph.py
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     9867 2021-04-14 20:40:03.000000 dbstep-1.2a0/dbstep/parse_data.py
+-rw-r--r--   0 guilianluchini   (501) staff       (20)    15058 2020-10-20 23:56:09.000000 dbstep-1.2a0/dbstep/sterics.py
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     3931 2020-01-17 22:34:22.000000 dbstep-1.2a0/dbstep/writer.py
+drwxr-xr-x   0 guilianluchini   (501) staff       (20)        0 2021-04-19 21:59:43.892612 dbstep-1.2a0/dbstep.egg-info/
+-rw-r--r--   0 guilianluchini   (501) staff       (20)    12407 2021-04-19 21:59:43.000000 dbstep-1.2a0/dbstep.egg-info/PKG-INFO
+-rw-r--r--   0 guilianluchini   (501) staff       (20)     1004 2021-04-19 21:59:43.000000 dbstep-1.2a0/dbstep.egg-info/SOURCES.txt
+-rw-r--r--   0 guilianluchini   (501) staff       (20)        1 2021-04-19 21:59:43.000000 dbstep-1.2a0/dbstep.egg-info/dependency_links.txt
+-rw-r--r--   0 guilianluchini   (501) staff       (20)       24 2021-04-19 21:59:43.000000 dbstep-1.2a0/dbstep.egg-info/requires.txt
+-rw-r--r--   0 guilianluchini   (501) staff       (20)        7 2021-04-19 21:59:43.000000 dbstep-1.2a0/dbstep.egg-info/top_level.txt
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      108 2021-04-19 21:59:43.898779 dbstep-1.2a0/setup.cfg
+-rw-r--r--   0 guilianluchini   (501) staff       (20)      972 2021-04-19 21:58:50.000000 dbstep-1.2a0/setup.py
```

### Comparing `dbstep-1.1a0/LICENSE.txt` & `dbstep-1.2a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/PKG-INFO` & `dbstep-1.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dbstep
-Version: 1.1a0
+Version: 1.2a0
 Summary: DFT Based Steric Parameters
 Home-page: https://github.com/bobbypaton/DBSTEP
 Author: Guilian Luchini, Robert Paton
 Author-email: patonlab@colostate.edu
 License: MIT
-Download-URL: https://github.com/bobbypaton/DBSTEP/archive/refs/tags/1.1-alpha.tar.gz
+Download-URL: https://github.com/bobbypaton/DBSTEP/archive/refs/tags/1.2-alpha.tar.gz
 Description: ![DBSTEP](DBSTEP_banner.png)
         ===
         
         # DBSTEP
         DFT-based Steric Parameters 
         
+        [![DOI](https://zenodo.org/badge/198946518.svg)](https://zenodo.org/badge/latestdoi/198946518)
+        
         Allows a user to compute steric parameters from chemical structures. 
         
         Calculate Sterimol parameters<sup>1</sup> (L, Bmin, Bmax), %Buried Volume<sup>2</sup>, Sterimol2Vec and Vol2Vec parameters
         
         ## Features
         * Compute requested steric parameters from molecular structure files with input options:
             * `-s` or `--sterimol` - Sterimol Parameters (L, Bmin, Bmax)
```

### Comparing `dbstep-1.1a0/README.md` & `dbstep-1.2a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ![DBSTEP](DBSTEP_banner.png)
 ===
 
 # DBSTEP
 DFT-based Steric Parameters 
 
+[![DOI](https://zenodo.org/badge/198946518.svg)](https://zenodo.org/badge/latestdoi/198946518)
+
 Allows a user to compute steric parameters from chemical structures. 
 
 Calculate Sterimol parameters<sup>1</sup> (L, Bmin, Bmax), %Buried Volume<sup>2</sup>, Sterimol2Vec and Vol2Vec parameters
 
 ## Features
 * Compute requested steric parameters from molecular structure files with input options:
     * `-s` or `--sterimol` - Sterimol Parameters (L, Bmin, Bmax)
```

### Comparing `dbstep-1.1a0/dbstep/Dbstep.py` & `dbstep-1.2a0/dbstep/Dbstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 			 
 		#Parse coordinate/volumetric information
 		if ext == '.cube':
 			options.surface = 'density'
 			mol = parse_data.GetCubeData(name)
 		elif ext == 'rdkit':
 			mol = parse_data.GetData_RDKit(name, options.noH, options.spec_atom_1, options.spec_atom_2)
-		elif ext == ".xyz":
+		elif ext in [".xyz",'.com','.gjf']:
 			mol = parse_data.GetXYZData(name, ext, options.noH,options.spec_atom_1, options.spec_atom_2)
 			if options.noH:
 				options.spec_atom_1 = mol.spec_atom_1
 				options.spec_atom_2 = mol.spec_atom_2
 		else:
 			mol = parse_data.GetData_cclib(name, ext, options.noH,options.spec_atom_1, options.spec_atom_2)
 			if options.noH:
@@ -490,15 +490,15 @@
 	parser.add_option("--noH", dest="noH", action="store_true", help="Neglect hydrogen atoms (by default these are included)", default=False, metavar="noH")
 	parser.add_option("--addmetals", dest="add_metals", action="store_true", help="By default, the VDW radii of metals are not considered. This will include them", default=False, metavar="add_metals")
 	parser.add_option("--norot",dest='norot',action="store_true",help="Do not rotate the molecules (use if structures have been pre-aligned)",default=False)
 	parser.add_option("--grid", dest="grid", action="store", help="Specify how grid point spacing used to compute spatial occupancy", default=0.05, type=float, metavar="grid")
 	parser.add_option("--2d", dest="graph",action="store_true", help="[2D sterics only] Specify input text file containing SMILES strings to analyze 2D contributions",default=False)
 	parser.add_option("--fg",  dest="shared_fg", action="store", default=False, help="[2D sterics only] SMILES pattern (e.g. 'C(O)=O') of a shared functional group or atom - this is used to define the origin")
 	parser.add_option("--maxpath", dest="max_path_length", type=int, action="store", default=9, help="[2D sterics only] Maximum path length (bonds) along which to include steric contributions (Default: 9)")
-	parser.add_option("--2d-type", dest="voltype", action="store", default="crippen",choices=['crippen','mcgowan'], help="[2D sterics only] Method for determining atomic contribution to total volume. Options include 'crippen' or 'mcgowan' (Default: crippen)")
+	parser.add_option("--2d-type", dest="voltype", action="store", default="crippen",choices=['crippen','mcgowan','degree'], help="[2D sterics only] Method for determining atomic contribution to total volume. Options include 'crippen'=default,'mcgowan', or 'degree'")
 	parser.add_option("--pos", dest="pos", action="store_true", help="Measure Sterimol parameters in postive direction (from atom1 toward atom2). ", default=False, metavar="pos")
 	parser.add_option("--isoval", dest="isoval", action="store", help="Density isovalue cutoff (default = 0.002)", type="float", default=0.002, metavar="isoval")
 	parser.add_option("--vshell",dest="vshell",action="store",help="Calculate buried volume of hollow sphere. Input: shell width, use '-r' option to adjust radius'", default=False,type=float, metavar="radius")
 	parser.add_option("--qsar", dest="qsar", action="store_true", help="Construct a grid with probe atom at each point for QSAR study (this generates a lot of files!)", default=False, metavar="qsar")
 	parser.add_option("--gridsize", dest="gridsize", action="store",help="Set size of grid to analyze molecule centered at origin 'xmin,xmax:ymin,ymax:zmin,zmax'",default=False)
 	parser.add_option("--scalevdw", dest="SCALE_VDW", action="store", help="Scaling factor for VDW radii (default = 1.0)", type=float, default=1.0, metavar="SCALE_VDW")
 	parser.add_option("-t", "--timing",dest="timing",action="store_true", help="Request timing information", default=False)
```

### Comparing `dbstep-1.1a0/dbstep/calculator.py` & `dbstep-1.2a0/dbstep/calculator.py`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/.DS_Store` & `dbstep-1.2a0/dbstep/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/35diMePh.xyz` & `dbstep-1.2a0/dbstep/examples/35diMePh.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/4ClPh.xyz` & `dbstep-1.2a0/dbstep/examples/4ClPh.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/4MeOPh.xyz` & `dbstep-1.2a0/dbstep/examples/4MeOPh.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/4MePh.xyz` & `dbstep-1.2a0/dbstep/examples/4MePh.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/Ad.xyz` & `dbstep-1.2a0/dbstep/examples/Ad.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/Benchmark.csv` & `dbstep-1.2a0/dbstep/examples/Benchmark.csv`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/Bn.xyz` & `dbstep-1.2a0/dbstep/examples/Bn.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/CEt3.xyz` & `dbstep-1.2a0/dbstep/examples/CEt3.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/CH2iPr.xyz` & `dbstep-1.2a0/dbstep/examples/CH2iPr.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/CH2tBu.xyz` & `dbstep-1.2a0/dbstep/examples/CH2tBu.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/CHEt2.xyz` & `dbstep-1.2a0/dbstep/examples/CHEt2.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/CHPr2.xyz` & `dbstep-1.2a0/dbstep/examples/CHPr2.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/CHiPr2.xyz` & `dbstep-1.2a0/dbstep/examples/CHiPr2.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/Ph.xyz` & `dbstep-1.2a0/dbstep/examples/Ph.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/cHex.xyz` & `dbstep-1.2a0/dbstep/examples/cHex.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/iPr.xyz` & `dbstep-1.2a0/dbstep/examples/iPr.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/nPr.xyz` & `dbstep-1.2a0/dbstep/examples/nPr.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/examples/tBu.xyz` & `dbstep-1.2a0/dbstep/examples/tBu.xyz`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/graph.py` & `dbstep-1.2a0/dbstep/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,21 @@
             for nbr in at.GetNeighbors(): 
                 if nbr.GetAtomicNum()==1: #look at attached hydrogens
                     contrib += contribs[nbr.GetIdx()]
             res += contrib
             ccontribs.append(contrib)
     return res,ccontribs
     
+def degreeContribs(mol):
+    contribs = []
+    for i,at in enumerate(mol.GetAtoms()): #grab all atom contributions
+        deg = at.GetDegree()
+        contribs.append(deg)
+    return contribs
+    
 def load_mcgowan():
     stream = pkg_resources.resource_stream(__name__, 'mcgowan.csv')
     return pd.read_csv(stream)
 
 def mcgowanHContribs(molH): 
     """Adds McGowan volume atomic contributions from hydrogen to a heavy atoms contribution"""
     #Read mcgowan volumes 
@@ -128,14 +135,16 @@
             # condense H atom contributions to attached heavy atom
             mr, apolsCondensed = crippenHContribs(molH,mrs)
             vols = apolsCondensed
         elif voltype.lower() == 'mcgowan':
             #grab mcgowan volumes 
             molH = Chem.AddHs(mol)
             vols = mcgowanHContribs(molH)
+        elif voltype.lower() == 'degree':
+            vols = degreeContribs(mol)
         
         # this is the radial count up to the max_path_length
         for level in range(0,max_path_length):
             mol2vec.append(0)
             for at, dist in enumerate(dist_from_base):
                 # This will try to exclude the other atoms in the defined FG apart from the base
                 if dist == level and at not in fg_atoms:
```

### Comparing `dbstep-1.1a0/dbstep/parse_data.py` & `dbstep-1.2a0/dbstep/parse_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,26 +117,35 @@
 						except ValueError: pass
 					if len(coord) == 4:
 						if isinstance(coord[1],float) and isinstance(coord[2],float) and isinstance(coord[3],float):
 							[atom, x,y,z] = [coord[0], coord[1], coord[2], coord[3]]
 							self.ATOMTYPES.append(atom)
 							self.CARTESIANS.append([x,y,z])
 				except: pass
-		elif self.FORMAT == '.log':
-			for i, oline in enumerate(outlines):
-				if "Input orientation" in oline or "Standard orientation" in oline:
-					self.ATOMTYPES, self.CARTESIANS, carts = [], [], outlines[i + 5:]
-					for j, line in enumerate(carts):
-						if "-------" in line:
-							break
-						self.ATOMTYPES.append(element_id(int(line.split()[1])))
-						if len(line.split()) > 5:
-							self.CARTESIANS.append([float(line.split()[3]), float(line.split()[4]), float(line.split()[5])])
-						else:
-							self.CARTESIANS.append([float(line.split()[2]), float(line.split()[3]), float(line.split()[4])])
+		elif self.FORMAT == '.com' or self.FORMAT == '.gjf':
+			for i in range(0,len(outlines)):
+				if outlines[i].find("#") > -1:
+					if len(outlines[i+1].split()) == 0: 
+						start = i+5
+					if len(outlines[i+2].split()) == 0: 
+						start = i+6
+					break
+			for i in range(start,len(outlines)):
+				try:
+					coord = outlines[i].split()
+					for i in range(len(coord)):
+						try:
+							coord[i] = float(coord[i])
+						except ValueError: pass
+					if len(coord) == 4:
+						if isinstance(coord[1],float) and isinstance(coord[2],float) and isinstance(coord[3],float):
+							[atom, x,y,z] = [coord[0], coord[1], coord[2], coord[3]]
+							self.ATOMTYPES.append(atom)
+							self.CARTESIANS.append([x,y,z])
+				except: pass
 		self.ATOMTYPES = np.array(self.ATOMTYPES)
 		self.CARTESIANS = np.array(self.CARTESIANS)
 		#remove hydrogens if requested, update spec_atom numbering if necessary
 		if noH:
 			atom1_id,atom2_id = -1,-1
 			for n,atom in enumerate(self.ATOMTYPES):
 				if atom+str(n+1) == spec_atom_1:
```

### Comparing `dbstep-1.1a0/dbstep/sterics.py` & `dbstep-1.2a0/dbstep/sterics.py`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep/writer.py` & `dbstep-1.2a0/dbstep/writer.py`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/dbstep.egg-info/PKG-INFO` & `dbstep-1.2a0/dbstep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dbstep
-Version: 1.1a0
+Version: 1.2a0
 Summary: DFT Based Steric Parameters
 Home-page: https://github.com/bobbypaton/DBSTEP
 Author: Guilian Luchini, Robert Paton
 Author-email: patonlab@colostate.edu
 License: MIT
-Download-URL: https://github.com/bobbypaton/DBSTEP/archive/refs/tags/1.1-alpha.tar.gz
+Download-URL: https://github.com/bobbypaton/DBSTEP/archive/refs/tags/1.2-alpha.tar.gz
 Description: ![DBSTEP](DBSTEP_banner.png)
         ===
         
         # DBSTEP
         DFT-based Steric Parameters 
         
+        [![DOI](https://zenodo.org/badge/198946518.svg)](https://zenodo.org/badge/latestdoi/198946518)
+        
         Allows a user to compute steric parameters from chemical structures. 
         
         Calculate Sterimol parameters<sup>1</sup> (L, Bmin, Bmax), %Buried Volume<sup>2</sup>, Sterimol2Vec and Vol2Vec parameters
         
         ## Features
         * Compute requested steric parameters from molecular structure files with input options:
             * `-s` or `--sterimol` - Sterimol Parameters (L, Bmin, Bmax)
```

### Comparing `dbstep-1.1a0/dbstep.egg-info/SOURCES.txt` & `dbstep-1.2a0/dbstep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbstep-1.1a0/setup.py` & `dbstep-1.2a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name='dbstep',
   packages=['dbstep'],
-  version='1.1-alpha',
+  version='1.2-alpha',
   description='DFT Based Steric Parameters',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author='Guilian Luchini, Robert Paton',
   author_email='patonlab@colostate.edu',
   url = 'https://github.com/bobbypaton/DBSTEP',
-  download_url = 'https://github.com/bobbypaton/DBSTEP/archive/refs/tags/1.1-alpha.tar.gz',  
+  download_url = 'https://github.com/bobbypaton/DBSTEP/archive/refs/tags/1.2-alpha.tar.gz',  
   keywords=['compchem', 'steric', 'sterimol', 'informatics'],
   license="MIT",
   classifiers=['License :: OSI Approved :: MIT License',],
   install_requires=["numpy",'numba','scipy','cclib'],
   python_requires='>=3.6',
   include_package_data=True,
   package_data={'': ['*.csv']},
```

