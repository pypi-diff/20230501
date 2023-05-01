# Comparing `tmp/astartes-1.0.0b2.tar.gz` & `tmp/astartes-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astartes-1.0.0b2.tar", last modified: Wed Mar 15 17:10:05 2023, max compression
+gzip compressed data, was "astartes-1.0.0rc1.tar", last modified: Fri Mar 24 18:57:30 2023, max compression
```

## Comparing `astartes-1.0.0b2.tar` & `astartes-1.0.0rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.349701 astartes-1.0.0b2/
--rw-r--r--   0 jackson    (501) staff       (20)     1070 2023-03-02 01:08:02.000000 astartes-1.0.0b2/LICENSE
--rw-r--r--   0 jackson    (501) staff       (20)    13188 2023-03-15 17:10:05.348291 astartes-1.0.0b2/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)    12664 2023-03-15 16:22:42.000000 astartes-1.0.0b2/README.md
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.236749 astartes-1.0.0b2/astartes/
--rw-r--r--   0 jackson    (501) staff       (20)      290 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)    16611 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/main.py
--rw-r--r--   0 jackson    (501) staff       (20)     5461 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/molecules.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.284976 astartes-1.0.0b2/astartes/samplers/
--rw-r--r--   0 jackson    (501) staff       (20)      595 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/samplers/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)     4105 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/abstract_sampler.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.305699 astartes-1.0.0b2/astartes/samplers/extrapolation/
--rw-r--r--   0 jackson    (501) staff       (20)      160 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/extrapolation/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)      957 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/samplers/extrapolation/dbscan.py
--rw-r--r--   0 jackson    (501) staff       (20)     1095 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/samplers/extrapolation/kmeans.py
--rw-r--r--   0 jackson    (501) staff       (20)     7633 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/extrapolation/optisim.py
--rw-r--r--   0 jackson    (501) staff       (20)     4352 2023-03-15 17:08:10.000000 astartes-1.0.0b2/astartes/samplers/extrapolation/scaffold.py
--rw-r--r--   0 jackson    (501) staff       (20)     2915 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/extrapolation/sphere_exclusion.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.333743 astartes-1.0.0b2/astartes/samplers/interpolation/
--rw-r--r--   0 jackson    (501) staff       (20)      176 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/samplers/interpolation/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)       90 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/interpolation/doptimal.py
--rw-r--r--   0 jackson    (501) staff       (20)       88 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/interpolation/duplex.py
--rw-r--r--   0 jackson    (501) staff       (20)      883 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/interpolation/kennardstone.py
--rw-r--r--   0 jackson    (501) staff       (20)       86 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/interpolation/mtsd.py
--rw-r--r--   0 jackson    (501) staff       (20)      690 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/samplers/interpolation/random_split.py
--rw-r--r--   0 jackson    (501) staff       (20)     2984 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/samplers/interpolation/spxy.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.338948 astartes-1.0.0b2/astartes/utils/
--rw-r--r--   0 jackson    (501) staff       (20)        0 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/utils/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)      711 2023-03-02 01:08:02.000000 astartes-1.0.0b2/astartes/utils/exceptions.py
--rw-r--r--   0 jackson    (501) staff       (20)     2230 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/utils/sampler_factory.py
--rw-r--r--   0 jackson    (501) staff       (20)      718 2023-03-15 16:22:42.000000 astartes-1.0.0b2/astartes/utils/warnings.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.268915 astartes-1.0.0b2/astartes.egg-info/
--rw-r--r--   0 jackson    (501) staff       (20)    13188 2023-03-15 17:10:05.000000 astartes-1.0.0b2/astartes.egg-info/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)     1054 2023-03-15 17:10:05.000000 astartes-1.0.0b2/astartes.egg-info/SOURCES.txt
--rw-r--r--   0 jackson    (501) staff       (20)        1 2023-03-15 17:10:05.000000 astartes-1.0.0b2/astartes.egg-info/dependency_links.txt
--rw-r--r--   0 jackson    (501) staff       (20)       85 2023-03-15 17:10:05.000000 astartes-1.0.0b2/astartes.egg-info/requires.txt
--rw-r--r--   0 jackson    (501) staff       (20)        9 2023-03-15 17:10:05.000000 astartes-1.0.0b2/astartes.egg-info/top_level.txt
--rw-r--r--   0 jackson    (501) staff       (20)     1023 2023-03-15 17:09:45.000000 astartes-1.0.0b2/pyproject.toml
--rw-r--r--   0 jackson    (501) staff       (20)       38 2023-03-15 17:10:05.349839 astartes-1.0.0b2/setup.cfg
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-15 17:10:05.347130 astartes-1.0.0b2/test/
--rw-r--r--   0 jackson    (501) staff       (20)    15967 2023-03-15 16:22:42.000000 astartes-1.0.0b2/test/test_astartes.py
--rw-r--r--   0 jackson    (501) staff       (20)     4842 2023-03-15 16:22:42.000000 astartes-1.0.0b2/test/test_molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.714463 astartes-1.0.0rc1/astartes/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17498 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.714463 astartes-1.0.0rc1/astartes/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/abstract_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/astartes/samplers/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/optisim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/extrapolation/sphere_exclusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/astartes/samplers/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/doptimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/duplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/kennardstone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/mtsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/random_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/samplers/interpolation/spxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/astartes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/astartes/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.714463 astartes-1.0.0rc1/astartes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 18:57:30.000000 astartes-1.0.0rc1/astartes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:57:30.718463 astartes-1.0.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/test/test_astartes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-03-24 18:57:22.000000 astartes-1.0.0rc1/test/test_molecules.py
```

### Comparing `astartes-1.0.0b2/LICENSE` & `astartes-1.0.0rc1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Jackson Burns
+Copyright (c) 2023 Jackson Burns
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `astartes-1.0.0b2/PKG-INFO` & `astartes-1.0.0rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-Metadata-Version: 2.1
-Name: astartes
-Version: 1.0.0b2
-Summary: Train:Test Algorithmic Sampling for Molecules, Images, and Arbitrary Arrays
-Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/JacksonBurns/astartes
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: molecules
-Provides-Extra: dev
-License-File: LICENSE
-
 <h1 align="center">astartes</h1> 
-<h3 align="center">Train:Test Algorithmic Sampling for Molecules, Images, and Arbitrary Arrays</h3>
+<h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
   <img alt="astarteslogo" src="https://github.com/JacksonBurns/astartes/blob/main/astartes_logo.png">
 </p> 
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/astartes?style=social">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/astartes">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/astartes">
+  <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/astartes?style=plastic">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/astartes">
   <img alt="Test Status" src="https://github.com/JacksonBurns/astartes/actions/workflows/run_tests.yml/badge.svg?branch=main&event=schedule">
 </p>
 
 ## Installing `astartes`
-We reccomend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management.
+We recommend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management. Python versions 3.7, 3.8, 3.9, 3.10, and 3.11 are supported on all platforms.
 
-`astartes` is availble on `PyPI` and can be installed using `pip`:
+`astartes` is available on `PyPI` and can be installed using `pip`:
 
  - To include the featurization options for chemical data, use `pip install astartes[molecules]`.
- - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer depdencies and may be more readily compatible in environments with existing workflows).
+ - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
 By default, `astartes` will use a random splitting approach identical to that which is implemented in `sklearn`, and a variety of deterministic sampling approaches can be used by specifying one additional argument ot the function:
@@ -57,55 +44,57 @@
 |:---:|---|
 | Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_example.ipynb) |
 | Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2FRDB7_barrier_prediction_example.ipynb) |
 
 ### Rational Splitting Algorithms
 While much machine learning is done with a random choice between training/test/validation data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been introduced, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
 
-There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-smaple data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`.
+There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
 
 #### Implemented Sampling Algorithms
 
 | Sampler Name | Usage String | Type | Hyperparameters | Reference | Notes |
 |:---:|---|---|---|---|---|
-| Random | 'random' | Interpolative | `random_state`, `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
+| Random | 'random' | Interpolative | `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
 | Kennard-Stone | 'kennard_stone' | Interpolative | _none_ | [yu9824's `kennard_stone`](https://github.com/yu9824/kennard_stone) | Fully deterministic, no hyperparameters accepted. |
 | Sample set Partitioning based on join X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
 | Scaffold | 'scaffold' | Extrapolative | `explicit_hydrogens`, `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
-| Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `random_state`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
-| Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `random_state`, `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
-| K-Means | 'kmeans' | Extrapolative | `random_state`, `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
+| Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
+| Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
+| K-Means | 'kmeans' | Extrapolative | `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
 | Density-Based Spatial Clustering of Applications with Noise (DBSCAN) | 'dbscan' | Extrapolative | `eps`, `min_samples`, `algorithm`, `metric`, `leaf_size` | [`sklearn DBSCAN`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) | Passthrough to `sklearn`'s `DBSCAN`. |
-| Mimimm Test Set Dissimilarity | ~ | ~ | _will be released with_ `astartes` _v1.0.0_ | ~ | ~ |
-| RBM Sampler | ~ | ~ | _will be released with_ `astartes` _v1.0.0_ | ~ | ~ |
+| Minimum Test Set Dissimilarity (MTSD) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| Restricted Boltzmann Machine (RBM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| Kohonen Self-Organizing Map (SOM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| SPlit Method | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 
 ### Using the `astartes.molecules` Subpackage
 After installing with `pip install astartes[molecules]` one can import the new train/test splitting function like this: `from astartes.molecules import train_test_split_molecules`
 
 The usage of this function is identical to `train_test_split` but with the addition of new arguments to control how the molecules are featurized:
 
 ```python
 train_test_split_molecules(
-    smiles=smiles,
+    molecules=smiles,
     y=y,
     test_size=0.2,
     train_size=0.8,
     fingerprint="daylight_fingerprint",
     fprints_hopts={
         "minPath": 2,
         "maxPath": 5,
         "fpSize": 200,
         "bitsPerHash": 4,
         "useHs": 1,
         "tgtDensity": 0.4,
         "minSize": 64,
     },
-    splitter="random",
+    sampler="random",
+    random_state=42,
     hopts={
-        "random_state": 42,
         "shuffle": True,
     },
 )
 ```
 
 To see a complete example of using `train_test_split_molecules` with actual chemical data, take a look in the `examples` directory.
 
@@ -113,40 +102,42 @@
 
 ## Online Documentation
 [The online documentation](https://JacksonBurns.github.io/astartes/) contains everything you see in this README with an additional tutorial for [moving from `train_test_split` in `sklearn` to `astartes`](https://jacksonburns.github.io/astartes/sklearn_to_astartes.html).
 
 ## Contributing & Developer Notes
 Pull Requests, Bug Reports, and all Contributions are welcome! Please use the appropriate issue or pull request template when making a contribution.
 
+We make use of [the GitHub Discussions page](https://github.com/JacksonBurns/astartes/discussions) to go over potential features to add. Please feel free to stop by if you are looking for something to develop or have an idea for a useful feature!
+
 When submitting a PR, please mark your PR with the "PR Ready for Review" label when you are finished making changes so that the GitHub actions bots can work their magic!
 
 ### Developer Install
 
 To contribute to the `astartes` source code, start by cloning the repository (i.e. `git clone git@github.com:JacksonBurns/astartes.git`) and then inside the repository run `pip install -e .[molecules,dev]`. This will set you up with all the required dependencies to run `astartes` and conform to our formatting standards (`black` and `isort`), which you can configure to run automatically in vscode [like this](https://marcobelo.medium.com/setting-up-python-black-on-visual-studio-code-5318eba4cd00#:~:text=Go%20to%20settings%20in%20your,%E2%80%9D%20and%20select%20%E2%80%9Cblack%E2%80%9D.).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install -e ".[molecules,dev]"`)
 
 ### Unit Testing
-All of the tests in `astartes` are written using the built-in python `unittest` module (to allow running without `pytest`) but we _highly_ reccomend using `pytest`. To execute the tests from the `astartes` repository, simply type `pytest` after running the developer install (or alternately, `pytest -v` for a more helpful output).
+All of the tests in `astartes` are written using the built-in python `unittest` module (to allow running without `pytest`) but we _highly_ recommend using `pytest`. To execute the tests from the `astartes` repository, simply type `pytest` after running the developer install (or alternately, `pytest -v` for a more helpful output).
 
 ### Adding New Samplers
 Adding a new sampler should extend the `abstract_sampler.py` abstract base class.
 
 It can be as simple as a passthrough to a another `train_test_split`, or it can be an original implementation that results in X and y being split into two lists. Take a look at `astartes/samplers/random_split.py` for a basic example!
 
-After the sampler has been implemented, add it to `__init__.py` in in `astartes/samplers` and it will automatically be unit tested. Additional unit tests to verify that hyperparameters can be properly passed, etc. are also reccomended.
+After the sampler has been implemented, add it to `__init__.py` in in `astartes/samplers` and it will automatically be unit tested. Additional unit tests to verify that hyperparameters can be properly passed, etc. are also recommended.
 
 For historical reasons, and as a guide for any developers who would like add new samplers, below is a running list of samplers which have been _considered_ for addition to `asartes` but ultimately not added for various reasons.
 
 #### Not Implemented Sampling Algorithms
 
-| Sampler Name | Reasoning |
-|:---:|---|
-| D-Optimal | Requires _a-priori_ knowledge of the test and train size which does not fit in the `astartes` framework (samplers are all agnostic to the size of the sets) and it is questionable if the use of the Fischer information matrix is actually meaningful in the context of sampling existing data rather than tuning for ideal data. |
-| Duplex | Requires knowing test and train size before execution, and can only partition data into two sets which owuld make it incompatible with `train_val_test_split`. |
+| Sampler Name | Reasoning | Relevant Link(s) |
+|:---:|---|---|
+| D-Optimal | Requires _a-priori_ knowledge of the test and train size which does not fit in the `astartes` framework (samplers are all agnostic to the size of the sets) and it is questionable if the use of the Fischer information matrix is actually meaningful in the context of sampling existing data rather than tuning for ideal data. | The [Wikipedia article for optimal design](https://en.wikipedia.org/wiki/Optimal_design#:~:text=Of%20course%2C%20fixing%20the%20number%20of%20experimental%20runs%20a%20priori%20would%20be%20impractical.) does a good job explaining why this is difficult, and points at some potential alternatives. |
+| Duplex | Requires knowing test and train size before execution, and can only partition data into two sets which would make it incompatible with `train_val_test_split`. | This [implementation in R](https://search.r-project.org/CRAN/refmans/prospectr/html/duplex.html#:~:text=The%20DUPLEX%20algorithm%20is%20similar,that%20are%20the%20farthest%20apart.) includes helpful references and a reference implementation. |
 
 ### Adding New Featurization Schemes
 All of the sampling methods implemented in `astartes` accept arbitrary arrays of numbers and return the sampled groups (with the exception of `Scaffold.py`). If you have an existing featurization scheme (i.e. take an arbitrary input and turn it into an array of numbers), we would be thrilled to include it in `astartes`.
 
 Adding a new interface should take on this format:
 
 ```python
@@ -178,15 +169,15 @@
         splitter=splitter,
         hopts=hopts,
     )
 ```
 
 If possible, we would like to also add an example Jupyter Notebook with any new interface to demonstrate to new users how it functions. See our other examples in the `examples` directory.
 
-Contact @JacksonBurns if you need assistance adding an existing workflow to `astartes`. If this featurization scheme requires additional dependencies to function, we may add it as an additional _extra_ package in the same way that `molecules` in installed.
+Contact [@JacksonBurns](https://github.com/JacksonBurns) if you need assistance adding an existing workflow to `astartes`. If this featurization scheme requires additional dependencies to function, we may add it as an additional _extra_ package in the same way that `molecules` in installed.
 
-## JORS Branch
+## JOSS Branch
 
-`astartes` corresponding JORS paper is stored in this repository on a separate branch. You can find `paper.tex` on the aptly named `jors-paper` paper. 
+`astartes` corresponding JOSS paper is stored in this repository on a separate branch. You can find `paper.md` on the aptly named `joss-paper` branch. 
 
-_Note for Maintainers_: To push changes from the `main` branch into the `jors-paper` branch, run the `Update JORS Branch` workflow.
+_Note for Maintainers_: To push changes from the `main` branch into the `joss-paper` branch, run the `Update JOSS Branch` workflow.
```

### Comparing `astartes-1.0.0b2/README.md` & `astartes-1.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,47 @@
+Metadata-Version: 2.1
+Name: astartes
+Version: 1.0.0rc1
+Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
+Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
+License: MIT
+Project-URL: Homepage, https://github.com/JacksonBurns/astartes
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: molecules
+Provides-Extra: dev
+License-File: LICENSE
+
 <h1 align="center">astartes</h1> 
-<h3 align="center">Train:Test Algorithmic Sampling for Molecules, Images, and Arbitrary Arrays</h3>
+<h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
   <img alt="astarteslogo" src="https://github.com/JacksonBurns/astartes/blob/main/astartes_logo.png">
 </p> 
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/astartes?style=social">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/astartes">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/astartes">
+  <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/astartes?style=plastic">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/astartes">
   <img alt="Test Status" src="https://github.com/JacksonBurns/astartes/actions/workflows/run_tests.yml/badge.svg?branch=main&event=schedule">
 </p>
 
 ## Installing `astartes`
-We reccomend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management.
+We recommend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management. Python versions 3.7, 3.8, 3.9, 3.10, and 3.11 are supported on all platforms.
 
-`astartes` is availble on `PyPI` and can be installed using `pip`:
+`astartes` is available on `PyPI` and can be installed using `pip`:
 
  - To include the featurization options for chemical data, use `pip install astartes[molecules]`.
- - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer depdencies and may be more readily compatible in environments with existing workflows).
+ - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
 By default, `astartes` will use a random splitting approach identical to that which is implemented in `sklearn`, and a variety of deterministic sampling approaches can be used by specifying one additional argument ot the function:
@@ -43,55 +62,57 @@
 |:---:|---|
 | Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_example.ipynb) |
 | Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2FRDB7_barrier_prediction_example.ipynb) |
 
 ### Rational Splitting Algorithms
 While much machine learning is done with a random choice between training/test/validation data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been introduced, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
 
-There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-smaple data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`.
+There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
 
 #### Implemented Sampling Algorithms
 
 | Sampler Name | Usage String | Type | Hyperparameters | Reference | Notes |
 |:---:|---|---|---|---|---|
-| Random | 'random' | Interpolative | `random_state`, `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
+| Random | 'random' | Interpolative | `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
 | Kennard-Stone | 'kennard_stone' | Interpolative | _none_ | [yu9824's `kennard_stone`](https://github.com/yu9824/kennard_stone) | Fully deterministic, no hyperparameters accepted. |
 | Sample set Partitioning based on join X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
 | Scaffold | 'scaffold' | Extrapolative | `explicit_hydrogens`, `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
-| Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `random_state`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
-| Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `random_state`, `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
-| K-Means | 'kmeans' | Extrapolative | `random_state`, `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
+| Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
+| Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
+| K-Means | 'kmeans' | Extrapolative | `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
 | Density-Based Spatial Clustering of Applications with Noise (DBSCAN) | 'dbscan' | Extrapolative | `eps`, `min_samples`, `algorithm`, `metric`, `leaf_size` | [`sklearn DBSCAN`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) | Passthrough to `sklearn`'s `DBSCAN`. |
-| Mimimm Test Set Dissimilarity | ~ | ~ | _will be released with_ `astartes` _v1.0.0_ | ~ | ~ |
-| RBM Sampler | ~ | ~ | _will be released with_ `astartes` _v1.0.0_ | ~ | ~ |
+| Minimum Test Set Dissimilarity (MTSD) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| Restricted Boltzmann Machine (RBM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| Kohonen Self-Organizing Map (SOM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| SPlit Method | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 
 ### Using the `astartes.molecules` Subpackage
 After installing with `pip install astartes[molecules]` one can import the new train/test splitting function like this: `from astartes.molecules import train_test_split_molecules`
 
 The usage of this function is identical to `train_test_split` but with the addition of new arguments to control how the molecules are featurized:
 
 ```python
 train_test_split_molecules(
-    smiles=smiles,
+    molecules=smiles,
     y=y,
     test_size=0.2,
     train_size=0.8,
     fingerprint="daylight_fingerprint",
     fprints_hopts={
         "minPath": 2,
         "maxPath": 5,
         "fpSize": 200,
         "bitsPerHash": 4,
         "useHs": 1,
         "tgtDensity": 0.4,
         "minSize": 64,
     },
-    splitter="random",
+    sampler="random",
+    random_state=42,
     hopts={
-        "random_state": 42,
         "shuffle": True,
     },
 )
 ```
 
 To see a complete example of using `train_test_split_molecules` with actual chemical data, take a look in the `examples` directory.
 
@@ -99,40 +120,42 @@
 
 ## Online Documentation
 [The online documentation](https://JacksonBurns.github.io/astartes/) contains everything you see in this README with an additional tutorial for [moving from `train_test_split` in `sklearn` to `astartes`](https://jacksonburns.github.io/astartes/sklearn_to_astartes.html).
 
 ## Contributing & Developer Notes
 Pull Requests, Bug Reports, and all Contributions are welcome! Please use the appropriate issue or pull request template when making a contribution.
 
+We make use of [the GitHub Discussions page](https://github.com/JacksonBurns/astartes/discussions) to go over potential features to add. Please feel free to stop by if you are looking for something to develop or have an idea for a useful feature!
+
 When submitting a PR, please mark your PR with the "PR Ready for Review" label when you are finished making changes so that the GitHub actions bots can work their magic!
 
 ### Developer Install
 
 To contribute to the `astartes` source code, start by cloning the repository (i.e. `git clone git@github.com:JacksonBurns/astartes.git`) and then inside the repository run `pip install -e .[molecules,dev]`. This will set you up with all the required dependencies to run `astartes` and conform to our formatting standards (`black` and `isort`), which you can configure to run automatically in vscode [like this](https://marcobelo.medium.com/setting-up-python-black-on-visual-studio-code-5318eba4cd00#:~:text=Go%20to%20settings%20in%20your,%E2%80%9D%20and%20select%20%E2%80%9Cblack%E2%80%9D.).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install -e ".[molecules,dev]"`)
 
 ### Unit Testing
-All of the tests in `astartes` are written using the built-in python `unittest` module (to allow running without `pytest`) but we _highly_ reccomend using `pytest`. To execute the tests from the `astartes` repository, simply type `pytest` after running the developer install (or alternately, `pytest -v` for a more helpful output).
+All of the tests in `astartes` are written using the built-in python `unittest` module (to allow running without `pytest`) but we _highly_ recommend using `pytest`. To execute the tests from the `astartes` repository, simply type `pytest` after running the developer install (or alternately, `pytest -v` for a more helpful output).
 
 ### Adding New Samplers
 Adding a new sampler should extend the `abstract_sampler.py` abstract base class.
 
 It can be as simple as a passthrough to a another `train_test_split`, or it can be an original implementation that results in X and y being split into two lists. Take a look at `astartes/samplers/random_split.py` for a basic example!
 
-After the sampler has been implemented, add it to `__init__.py` in in `astartes/samplers` and it will automatically be unit tested. Additional unit tests to verify that hyperparameters can be properly passed, etc. are also reccomended.
+After the sampler has been implemented, add it to `__init__.py` in in `astartes/samplers` and it will automatically be unit tested. Additional unit tests to verify that hyperparameters can be properly passed, etc. are also recommended.
 
 For historical reasons, and as a guide for any developers who would like add new samplers, below is a running list of samplers which have been _considered_ for addition to `asartes` but ultimately not added for various reasons.
 
 #### Not Implemented Sampling Algorithms
 
-| Sampler Name | Reasoning |
-|:---:|---|
-| D-Optimal | Requires _a-priori_ knowledge of the test and train size which does not fit in the `astartes` framework (samplers are all agnostic to the size of the sets) and it is questionable if the use of the Fischer information matrix is actually meaningful in the context of sampling existing data rather than tuning for ideal data. |
-| Duplex | Requires knowing test and train size before execution, and can only partition data into two sets which owuld make it incompatible with `train_val_test_split`. |
+| Sampler Name | Reasoning | Relevant Link(s) |
+|:---:|---|---|
+| D-Optimal | Requires _a-priori_ knowledge of the test and train size which does not fit in the `astartes` framework (samplers are all agnostic to the size of the sets) and it is questionable if the use of the Fischer information matrix is actually meaningful in the context of sampling existing data rather than tuning for ideal data. | The [Wikipedia article for optimal design](https://en.wikipedia.org/wiki/Optimal_design#:~:text=Of%20course%2C%20fixing%20the%20number%20of%20experimental%20runs%20a%20priori%20would%20be%20impractical.) does a good job explaining why this is difficult, and points at some potential alternatives. |
+| Duplex | Requires knowing test and train size before execution, and can only partition data into two sets which would make it incompatible with `train_val_test_split`. | This [implementation in R](https://search.r-project.org/CRAN/refmans/prospectr/html/duplex.html#:~:text=The%20DUPLEX%20algorithm%20is%20similar,that%20are%20the%20farthest%20apart.) includes helpful references and a reference implementation. |
 
 ### Adding New Featurization Schemes
 All of the sampling methods implemented in `astartes` accept arbitrary arrays of numbers and return the sampled groups (with the exception of `Scaffold.py`). If you have an existing featurization scheme (i.e. take an arbitrary input and turn it into an array of numbers), we would be thrilled to include it in `astartes`.
 
 Adding a new interface should take on this format:
 
 ```python
@@ -164,15 +187,15 @@
         splitter=splitter,
         hopts=hopts,
     )
 ```
 
 If possible, we would like to also add an example Jupyter Notebook with any new interface to demonstrate to new users how it functions. See our other examples in the `examples` directory.
 
-Contact @JacksonBurns if you need assistance adding an existing workflow to `astartes`. If this featurization scheme requires additional dependencies to function, we may add it as an additional _extra_ package in the same way that `molecules` in installed.
+Contact [@JacksonBurns](https://github.com/JacksonBurns) if you need assistance adding an existing workflow to `astartes`. If this featurization scheme requires additional dependencies to function, we may add it as an additional _extra_ package in the same way that `molecules` in installed.
 
-## JORS Branch
+## JOSS Branch
 
-`astartes` corresponding JORS paper is stored in this repository on a separate branch. You can find `paper.tex` on the aptly named `jors-paper` paper. 
+`astartes` corresponding JOSS paper is stored in this repository on a separate branch. You can find `paper.md` on the aptly named `joss-paper` branch. 
 
-_Note for Maintainers_: To push changes from the `main` branch into the `jors-paper` branch, run the `Update JORS Branch` workflow.
+_Note for Maintainers_: To push changes from the `main` branch into the `joss-paper` branch, run the `Update JOSS Branch` workflow.
```

### Comparing `astartes-1.0.0b2/astartes/main.py` & `astartes-1.0.0rc1/astartes/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,43 @@
     IMPLEMENTED_EXTRAPOLATION_SAMPLERS,
     IMPLEMENTED_INTERPOLATION_SAMPLERS,
 )
 from astartes.utils.exceptions import InvalidConfigurationError
 from astartes.utils.sampler_factory import SamplerFactory
 from astartes.utils.warnings import ImperfectSplittingWarning, NormalizationWarning
 
+# define random seed
+DEFAULT_RANDOM_STATE = 42
+
 
 def train_val_test_split(
     X: np.array,
     y: np.array = None,
     labels: np.array = None,
     train_size: float = 0.8,
     val_size: float = 0.1,
     test_size: float = 0.1,
     sampler: str = "random",
+    random_state: int = None,
     hopts: dict = {},
     return_indices: bool = False,
 ):
     """Deterministic train_test_splitting of arbitrary arrays.
 
     Args:
         X (np.array): Numpy array of feature vectors.
         y (np.array, optional): Targets corresponding to X, must be of same size. Defaults to None.
         labels (np.array, optional): Labels corresponding to X, must be of same size. Defaults to None.
         train_size (float, optional): Fraction of dataset to use in training set. Defaults to 0.8.
         val_size (float, optional): Fraction of dataset to use in validation set. Defaults to 0.1.
         test_size (float, optional): Fraction of dataset to use in test set. Defaults to 0.1.
         sampler (str, optional): Sampler to use, see IMPLEMENTED_INTER/EXTRAPOLATION_SAMPLERS. Defaults to "random".
+        random_state (int, optional): The random seed used throughout astartes.
         hopts (dict, optional): Hyperparameters for the sampler used above. Defaults to {}.
-        return_indices (bool, optional): True to return indices of train/test instead of values. Defaults to False.
+        return_indices (bool, optional): True to return indices of train/test after values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/val/test data, or indices.
     """
     msg = ""
     if y is not None and len(y) != len(X):
         msg += "len(y)={:d} ".format(len(y))
@@ -48,24 +53,28 @@
         raise InvalidConfigurationError(
             "Lengths of input arrays do not match: len(X)={:d} ".format(len(X)) + msg
         )
 
     train_size, val_size, test_size = _normalize_split_sizes(
         train_size, val_size, test_size
     )
+    hopts["random_state"] = (
+        random_state if random_state is not None else DEFAULT_RANDOM_STATE
+    )
     sampler_factory = SamplerFactory(sampler)
     sampler_instance = sampler_factory.get_sampler(X, y, labels, hopts)
 
     if sampler in IMPLEMENTED_EXTRAPOLATION_SAMPLERS:
         return _extrapolative_sampling(
             sampler_instance,
             test_size,
             val_size,
             train_size,
             return_indices,
+            random_state,
         )
     else:
         return _interpolative_sampling(
             sampler_instance,
             test_size,
             val_size,
             train_size,
@@ -76,76 +85,97 @@
 def train_test_split(
     X: np.array,
     y: np.array = None,
     labels: np.array = None,
     train_size: float = 0.75,
     test_size: float = None,
     sampler: str = "random",
+    random_state: int = None,
     hopts: dict = {},
     return_indices: bool = False,
 ):
     """Deterministic train_test_splitting of arbitrary arrays.
 
     Args:
         X (np.array): Numpy array of feature vectors.
         y (np.array, optional): Targets corresponding to X, must be of same size. Defaults to None.
         labels (np.array, optional): Labels corresponding to X, must be of same size. Defaults to None.
         train_size (float, optional): Fraction of dataset to use in training set. Defaults to 0.75.
         test_size (float, optional): Fraction of dataset to use in test set. Defaults to None.
         sampler (str, optional): Sampler to use, see IMPLEMENTED_INTER/EXTRAPOLATION_SAMPLERS. Defaults to "random".
+        random_state (int, optional): The random seed used throughout astartes.
         hopts (dict, optional): Hyperparameters for the sampler used above. Defaults to {}.
         return_indices (bool, optional): True to return indices of train/test instead of values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/val/test data, or indices.
     """
     return train_val_test_split(
-        X, y, labels, train_size, 0, test_size, sampler, hopts, return_indices
+        X,
+        y,
+        labels,
+        train_size,
+        0,
+        test_size,
+        sampler,
+        random_state,
+        hopts,
+        return_indices,
     )
 
 
 def _extrapolative_sampling(
     sampler_instance,
     test_size,
     val_size,
     train_size,
     return_indices,
+    random_state,
 ):
     """Helper function to perform extrapolative sampling.
 
     Attempts to fill train, val, and test without breaking up clusters. Prioiritizes underfilling
     test and then val and then the balance goes into train (which is why the floats are given
     in that order).
 
     Args:
         sampler_instance (sampler): The fit sampler instance.
         test_size (float): Fraction of data to use in test.
         val_size (float): Fraction of data to use in val.
         train_size (float): Fraction of data to use in train.
         return_indices (bool): Return indices or the arrays themselves.
+        random_state (int, optional): The random state used to shuffle small clusters. Default to no shuffle.
 
     Returns:
         calls: _return_helper
     """
     # calculate "goal" splitting sizes
     n_test_samples = floor(len(sampler_instance.X) * test_size)
     n_val_samples = floor(len(sampler_instance.X) * val_size)
     # unlike interpolative, cannot calculate n_train_samples here
     # since it will vary based on cluster_lengths
 
-    # can't break up clusters
-    cluster_counter = sampler_instance.get_sorted_cluster_counter()
+    # largest clusters must go into largest set, but smaller ones can optionally
+    # be shuffled
+    cluster_counter = None
+    if random_state is None:
+        cluster_counter = sampler_instance.get_sorted_cluster_counter()
+    else:
+        cluster_counter = sampler_instance.get_semi_sorted_cluster_counter(
+            max_shufflable_size=min(n_test_samples, n_val_samples)
+        )
+
     test_idxs, val_idxs, train_idxs = (
         np.array([], dtype=int),
         np.array([], dtype=int),
         np.array([], dtype=int),
     )
     for cluster_idx, cluster_length in cluster_counter.items():
-        # assemble test first
-        if (len(test_idxs) + cluster_length) <= n_test_samples:  # will not overfill
+        # assemble test first, avoid overfilling
+        if (len(test_idxs) + cluster_length) <= n_test_samples:
             test_idxs = np.append(
                 test_idxs, sampler_instance.get_sample_idxs(cluster_length)
             )
         if (len(val_idxs) + cluster_length) <= n_val_samples:
             val_idxs = np.append(
                 val_idxs, sampler_instance.get_sample_idxs(cluster_length)
             )
@@ -210,58 +240,57 @@
     """Convenience function to return the requested arrays appropriately.
 
     Args:
         sampler_instance (sampler): The fit sampler instance.
         test_size (float): Fraction of data to use in test.
         val_size (float): Fraction of data to use in val.
         train_size (float): Fraction of data to use in train.
-        return_indices (bool): Return indices or the arrays themselves.
+        return_indices (bool): Return indices after the value arrays.
 
     Returns:
         np.array: Either many arrays or indices in arrays.
     """
-    if return_indices:
-        if val_idxs.any():
-            return train_idxs, val_idxs, test_idxs
-        else:
-            return train_idxs, test_idxs
     out = []
     X_train = sampler_instance.X[train_idxs]
     out.append(X_train)
-    if val_idxs.any():
+    if len(val_idxs):
         X_val = sampler_instance.X[val_idxs]
         out.append(X_val)
     X_test = sampler_instance.X[test_idxs]
     out.append(X_test)
 
     if sampler_instance.y is not None:
         y_train = sampler_instance.y[train_idxs]
         out.append(y_train)
-        if val_idxs.any():
+        if len(val_idxs):
             y_val = sampler_instance.y[val_idxs]
             out.append(y_val)
         y_test = sampler_instance.y[test_idxs]
         out.append(y_test)
     if sampler_instance.labels is not None:
         labels_train = sampler_instance.labels[train_idxs]
         out.append(labels_train)
-        if val_idxs.any():
+        if len(val_idxs):
             labels_val = sampler_instance.labels[val_idxs]
             out.append(labels_val)
         labels_test = sampler_instance.labels[test_idxs]
         out.append(labels_test)
     if len(sampler_instance.get_clusters()):  # true when the list has been filled
         clusters_train = sampler_instance.get_clusters()[train_idxs]
         out.append(clusters_train)
-        if val_idxs.any():
+        if len(val_idxs):
             clusters_val = sampler_instance.get_clusters()[val_idxs]
             out.append(clusters_val)
         clusters_test = sampler_instance.get_clusters()[test_idxs]
         out.append(clusters_test)
-
+    if return_indices:
+        out.append(train_idxs)
+        if val_idxs.any():
+            out.append(val_idxs)
+        out.append(test_idxs)
     return (*out,)
 
 
 def _check_actual_split(
     train_idxs,
     val_idxs,
     test_idxs,
```

### Comparing `astartes-1.0.0b2/astartes/molecules.py` & `astartes-1.0.0rc1/astartes/molecules.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import warnings
-from typing import List
 
 import numpy as np
 
 from astartes.utils.exceptions import MoleculesNotInstalledError
 
 try:
     """
@@ -11,127 +10,145 @@
     be deprecated in a version of Python after 3.11, so it is throwing a deprecation warning
     We ignore this warning since we can't do anything about it (sklearn_extra seems to be
     abandonware) and in the future it will become an error that we can deal with.
     """
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=DeprecationWarning)
         from aimsim.chemical_datastructures import Molecule
+        from aimsim.exceptions import LoadingError
 except ImportError:  # pragma: no cover
     raise MoleculesNotInstalledError(
         """To use molecule featurizer, install astartes with pip install astartes[molecules]."""
     )
 
 
 from astartes import train_test_split, train_val_test_split
 
 
 def train_val_test_split_molecules(
-    smiles: List[str],
+    molecules: np.array,
     y: np.array = None,
     labels: np.array = None,
     train_size: float = 0.8,
     val_size: float = 0.1,
     test_size: float = 0.1,
     sampler: str = "random",
+    random_state: int = None,
     hopts: dict = {},
     fingerprint: str = "morgan_fingerprint",
     fprints_hopts: dict = {},
     return_indices: bool = False,
 ):
-    """Deterministic train_test_splitting of SMILES strings.
+    """Deterministic train_test_splitting of molecules (SMILES strings or RDKit objects).
 
     Args:
-        smiles (List[str]): List of SMILES strings representing molecules or reactions.
+        molecules (np.array): List of SMILES strings or RDKit molecule objects representing molecules or reactions.
         y (np.array, optional): Targets corresponding to SMILES, must be of same size. Defaults to None.
         labels (np.array, optional): Labels corresponding to SMILES, must be of same size. Defaults to None.
         train_size (float, optional): Fraction of dataset to use in training set. Defaults to 0.8.
         val_size (float, optional): Fraction of dataset to use in validation set. Defaults to 0.1.
         test_size (float, optional): Fraction of dataset to use in test set. Defaults to 0.1.
         sampler (str, optional): Sampler to use, see IMPLEMENTED_INTER/EXTRAPOLATION_SAMPLERS. Defaults to "random".
+        random_state (int, optional): The random seed used throughout astartes. Defaults to 42.
         hopts (dict, optional): Hyperparameters for the sampler used above. Defaults to {}.
         fingerprint (str, optional): Molecular fingerprint to be used from AIMSim. Defaults to "morgan_fingerprint".
         fprints_hopts (dict, optional): Hyperparameters for AIMSim featurization. Defaults to {}.
-        return_indices (bool, optional): True to return indices of train/test instead of values. Defaults to False.
+        return_indices (bool, optional): True to return indices of train/test after the values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/val/test data, or indices.
     """
-    X = _featurize(smiles, fingerprint, fprints_hopts)
+    X = _featurize(molecules, fingerprint, fprints_hopts)
     return train_val_test_split(
         X,
         y=y,
         labels=labels,
         test_size=test_size,
         val_size=val_size,
         train_size=train_size,
         sampler=sampler,
+        random_state=random_state,
         hopts=hopts,
         return_indices=return_indices,
     )
 
 
 def train_test_split_molecules(
-    smiles: List[str],
+    molecules: np.array,
     y: np.array = None,
     labels: np.array = None,
     train_size: float = 0.75,
     test_size: float = None,
     sampler: str = "random",
+    random_state: int = None,
     hopts: dict = {},
     fingerprint: str = "morgan_fingerprint",
     fprints_hopts: dict = {},
     return_indices: bool = False,
 ):
-    """Deterministic train/test splitting of SMILES strings.
+    """Deterministic train/test splitting of molecules (SMILES strings or RDKit objects).
 
     Args:
-        smiles (List[str]): List of SMILES strings representing molecules or reactions.
+        molecules (np.array): List of SMILES strings or RDKit molecule objects representing molecules or reactions.
         y (np.array, optional): Targets corresponding to SMILES, must be of same size. Defaults to None.
         labels (np.array, optional): Labels corresponding to SMILES, must be of same size. Defaults to None.
         train_size (float, optional): Fraction of dataset to use in training (test+train~1). Defaults to 0.75.
         test_size (float, optional): Fraction of dataset to use in test set. Defaults to None.
         sampler (str, optional): Sampler to use, see IMPLEMENTED_INTER/EXTRAPOLATION_SAMPLERS. Defaults to "random".
+        random_state (int, optional): The random seed used throughout astartes. Defaults to None.
         hopts (dict, optional): Hyperparameters for the sampler used above. Defaults to {}.
         fingerprint (str, optional): Molecular fingerprint to be used from AIMSim. Defaults to "morgan_fingerprint".
         fprints_hopts (dict, optional): Hyperparameters for AIMSim featurization. Defaults to {}.
-        return_indices (bool, optional): True to return indices of train/test instead of values. Defaults to False.
+        return_indices (bool, optional): True to return indices of train/test after the values. Defaults to False.
 
     Returns:
         np.array: X, y, and labels train/test data, or indices.
     """
     # turn the smiles into an input X
-    X = _featurize(smiles, fingerprint, fprints_hopts)
+    X = _featurize(molecules, fingerprint, fprints_hopts)
 
     # call train test split with this input
     return train_test_split(
         X,
         y=y,
         labels=labels,
         test_size=test_size,
         train_size=train_size,
         sampler=sampler,
+        random_state=random_state,
         hopts=hopts,
         return_indices=return_indices,
     )
 
 
-def _featurize(smiles, fingerprint, fprints_hopts):
-    """Call AIMSim's Molecule to featurize the SMILES string according to the arguments.
+def _featurize(molecules, fingerprint, fprints_hopts):
+    """Call AIMSim's Molecule to featurize the molecules according to the arguments.
 
     Args:
-        smiles (str): SMILES string.
+        molecules (np.array): SMILES strings or RDKit molecule objects.
         fingerprint (str): The molecular fingerprint to be used.
         fprints_hopts (dict): Hyperparameters for AIMSim.
 
     Returns:
-        np.array: X array (featurized SMILES)
+        np.array: X array (featurized molecules)
     """
     X = []
-    for smile in smiles:
-        mol = Molecule(mol_smiles=smile)
+    for molecule in molecules:
+        try:
+            if type(molecule) in (np.str_, str):
+                mol = Molecule(mol_smiles=molecule)
+            else:
+                mol = Molecule(mol_graph=molecule)
+        except LoadingError as le:
+            raise RuntimeError(
+                "Unable to featurize molecules using '{:s}' with this configuration: fprint_hopts={:s}"
+                "\nCheck terminal output for messages from the RDkit logger. ".format(
+                    fingerprint, repr(fprints_hopts)
+                )
+            ) from le
         mol.descriptor.make_fingerprint(
             mol.mol_graph,
             fingerprint,
             fingerprint_params=fprints_hopts,
         )
         X.append(mol.descriptor.to_numpy())
     return np.array(X)
```

### Comparing `astartes-1.0.0b2/astartes/samplers/__init__.py` & `astartes-1.0.0rc1/astartes/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/extrapolation/dbscan.py` & `astartes-1.0.0rc1/astartes/samplers/extrapolation/dbscan.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/extrapolation/kmeans.py` & `astartes-1.0.0rc1/astartes/samplers/extrapolation/kmeans.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/extrapolation/optisim.py` & `astartes-1.0.0rc1/astartes/samplers/extrapolation/optisim.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/extrapolation/scaffold.py` & `astartes-1.0.0rc1/astartes/samplers/extrapolation/scaffold.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/extrapolation/sphere_exclusion.py` & `astartes-1.0.0rc1/astartes/samplers/extrapolation/sphere_exclusion.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/interpolation/kennardstone.py` & `astartes-1.0.0rc1/astartes/samplers/interpolation/kennardstone.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/interpolation/random_split.py` & `astartes-1.0.0rc1/astartes/samplers/interpolation/random_split.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/samplers/interpolation/spxy.py` & `astartes-1.0.0rc1/astartes/samplers/interpolation/spxy.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/utils/exceptions.py` & `astartes-1.0.0rc1/astartes/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/utils/sampler_factory.py` & `astartes-1.0.0rc1/astartes/utils/sampler_factory.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes/utils/warnings.py` & `astartes-1.0.0rc1/astartes/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/astartes.egg-info/PKG-INFO` & `astartes-1.0.0rc1/astartes.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 Metadata-Version: 2.1
 Name: astartes
-Version: 1.0.0b2
-Summary: Train:Test Algorithmic Sampling for Molecules, Images, and Arbitrary Arrays
+Version: 1.0.0rc1
+Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
 Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/astartes
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: molecules
 Provides-Extra: dev
 License-File: LICENSE
 
 <h1 align="center">astartes</h1> 
-<h3 align="center">Train:Test Algorithmic Sampling for Molecules, Images, and Arbitrary Arrays</h3>
+<h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
   <img alt="astarteslogo" src="https://github.com/JacksonBurns/astartes/blob/main/astartes_logo.png">
 </p> 
 <p align="center">
   <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/JacksonBurns/astartes?style=social">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/astartes">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/astartes">
+  <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/astartes?style=plastic">
   <img alt="PyPI - License" src="https://img.shields.io/github/license/JacksonBurns/astartes">
   <img alt="Test Status" src="https://github.com/JacksonBurns/astartes/actions/workflows/run_tests.yml/badge.svg?branch=main&event=schedule">
 </p>
 
 ## Installing `astartes`
-We reccomend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management.
+We recommend installing `astartes` within a virtual environment, using either `venv` or `conda` (or other tools) to simplify dependency management. Python versions 3.7, 3.8, 3.9, 3.10, and 3.11 are supported on all platforms.
 
-`astartes` is availble on `PyPI` and can be installed using `pip`:
+`astartes` is available on `PyPI` and can be installed using `pip`:
 
  - To include the featurization options for chemical data, use `pip install astartes[molecules]`.
- - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer depdencies and may be more readily compatible in environments with existing workflows).
+ - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
 By default, `astartes` will use a random splitting approach identical to that which is implemented in `sklearn`, and a variety of deterministic sampling approaches can be used by specifying one additional argument ot the function:
@@ -57,55 +62,57 @@
 |:---:|---|
 | Using `train_val_test_split` with the `sklearn` example datasets | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2Ftrain_val_test_split_example.ipynb) |
 | Cheminformatics sample set partitioning with `astartes` | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JacksonBurns/astartes/main?labpath=examples%2FRDB7_barrier_prediction_example.ipynb) |
 
 ### Rational Splitting Algorithms
 While much machine learning is done with a random choice between training/test/validation data, an alternative is the use of so-called "rational" splitting algorithms. These approaches use some similarity-based algorithm to divide data into sets. Some of these algorithms include Kennard-Stone, minimal test set dissimilarity, and sphere exclusion algorithms [as discussed by Tropsha et. al](https://pubs.acs.org/doi/pdf/10.1021/ci300338w) as well as the OptiSim as discussed in [Applied Chemoinformatics: Achievements and Future Opportunities](https://www.wiley.com/en-us/Applied+Chemoinformatics%3A+Achievements+and+Future+Opportunities-p-9783527806546). Some clustering-based splitting techniques have also been introduced, such as [DBSCAN](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1016.890&rep=rep1&type=pdf).
 
-There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-smaple data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`.
+There are two broad categories of sampling algorithms implemented in `astartes`: extrapolative and interpolative. The former will force your model to predict on out-of-sample data, effectively asking a 'harder question' than interpolative sampling. See the table below for all of the sampling approaches currently implemented in `astartes`, as well as the hyperparameters that each algorithm accepts (which are passed in with `hopts`) and a helpful reference for understanding how the hyperparameters work. Note that `random_state` is defined as a keyword argument in `train_test_split` itself, even though these algorithms will use the `random_state` in their own work. Do not provide a `random_state` in the `hopts` dictionary - it will be overwritten by the `random_state` you provide for `train_test_split` (or the default if none is provided).
 
 #### Implemented Sampling Algorithms
 
 | Sampler Name | Usage String | Type | Hyperparameters | Reference | Notes |
 |:---:|---|---|---|---|---|
-| Random | 'random' | Interpolative | `random_state`, `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
+| Random | 'random' | Interpolative | `shuffle` | [`sklearn train_test_split`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) | This sampler is a direct passthrough to `sklearn`'s `train_test_split`, though it does not currently reproduce splits identically. |
 | Kennard-Stone | 'kennard_stone' | Interpolative | _none_ | [yu9824's `kennard_stone`](https://github.com/yu9824/kennard_stone) | Fully deterministic, no hyperparameters accepted. |
 | Sample set Partitioning based on join X-Y distances (SPXY) | 'spxy' | Interpolative | `distance_metric` | Saldhana et. al [original paper](https://www.sciencedirect.com/science/article/abs/pii/S003991400500192X) | Extension of Kennard Stone that also includes the response when sampling distances. |
 | Scaffold | 'scaffold' | Extrapolative | `explicit_hydrogens`, `include_chirality` | [Bemis-Murcko Scaffold](https://pubs.acs.org/doi/full/10.1021/jm9602928) as implemented in RDKit | This sampler requires SMILES strings as input (use the `molecules` subpackage) |
-| Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `random_state`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
-| Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `random_state`, `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
-| K-Means | 'kmeans' | Extrapolative | `random_state`, `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
+| Sphere Exclusion | 'sphere_exclusion' | Extrapolative | `metric`, `distance_cutoff` | _custom implementation_ | Variation on Sphere Exclusion for arbitrary-valued vectors. |
+| Optimizable K-Dissimilarity Selection (OptiSim) | 'optisim' | Extrapolative | `n_clusters`, `max_subsample_size`, `distance_cutoff` | _custom implementation_ | Variation on [OptiSim](https://pubs.acs.org/doi/10.1021/ci025662h) for arbitrary-valued vectors. |
+| K-Means | 'kmeans' | Extrapolative | `n_clusters`, `n_init` | [`sklearn KMeans`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) | Passthrough to `sklearn`'s `KMeans`. |
 | Density-Based Spatial Clustering of Applications with Noise (DBSCAN) | 'dbscan' | Extrapolative | `eps`, `min_samples`, `algorithm`, `metric`, `leaf_size` | [`sklearn DBSCAN`](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) | Passthrough to `sklearn`'s `DBSCAN`. |
-| Mimimm Test Set Dissimilarity | ~ | ~ | _will be released with_ `astartes` _v1.0.0_ | ~ | ~ |
-| RBM Sampler | ~ | ~ | _will be released with_ `astartes` _v1.0.0_ | ~ | ~ |
+| Minimum Test Set Dissimilarity (MTSD) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| Restricted Boltzmann Machine (RBM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| Kohonen Self-Organizing Map (SOM) | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
+| SPlit Method | ~ | ~ | _upcoming in_ `astartes` _v1.x_ | ~ | ~ |
 
 ### Using the `astartes.molecules` Subpackage
 After installing with `pip install astartes[molecules]` one can import the new train/test splitting function like this: `from astartes.molecules import train_test_split_molecules`
 
 The usage of this function is identical to `train_test_split` but with the addition of new arguments to control how the molecules are featurized:
 
 ```python
 train_test_split_molecules(
-    smiles=smiles,
+    molecules=smiles,
     y=y,
     test_size=0.2,
     train_size=0.8,
     fingerprint="daylight_fingerprint",
     fprints_hopts={
         "minPath": 2,
         "maxPath": 5,
         "fpSize": 200,
         "bitsPerHash": 4,
         "useHs": 1,
         "tgtDensity": 0.4,
         "minSize": 64,
     },
-    splitter="random",
+    sampler="random",
+    random_state=42,
     hopts={
-        "random_state": 42,
         "shuffle": True,
     },
 )
 ```
 
 To see a complete example of using `train_test_split_molecules` with actual chemical data, take a look in the `examples` directory.
 
@@ -113,40 +120,42 @@
 
 ## Online Documentation
 [The online documentation](https://JacksonBurns.github.io/astartes/) contains everything you see in this README with an additional tutorial for [moving from `train_test_split` in `sklearn` to `astartes`](https://jacksonburns.github.io/astartes/sklearn_to_astartes.html).
 
 ## Contributing & Developer Notes
 Pull Requests, Bug Reports, and all Contributions are welcome! Please use the appropriate issue or pull request template when making a contribution.
 
+We make use of [the GitHub Discussions page](https://github.com/JacksonBurns/astartes/discussions) to go over potential features to add. Please feel free to stop by if you are looking for something to develop or have an idea for a useful feature!
+
 When submitting a PR, please mark your PR with the "PR Ready for Review" label when you are finished making changes so that the GitHub actions bots can work their magic!
 
 ### Developer Install
 
 To contribute to the `astartes` source code, start by cloning the repository (i.e. `git clone git@github.com:JacksonBurns/astartes.git`) and then inside the repository run `pip install -e .[molecules,dev]`. This will set you up with all the required dependencies to run `astartes` and conform to our formatting standards (`black` and `isort`), which you can configure to run automatically in vscode [like this](https://marcobelo.medium.com/setting-up-python-black-on-visual-studio-code-5318eba4cd00#:~:text=Go%20to%20settings%20in%20your,%E2%80%9D%20and%20select%20%E2%80%9Cblack%E2%80%9D.).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install -e ".[molecules,dev]"`)
 
 ### Unit Testing
-All of the tests in `astartes` are written using the built-in python `unittest` module (to allow running without `pytest`) but we _highly_ reccomend using `pytest`. To execute the tests from the `astartes` repository, simply type `pytest` after running the developer install (or alternately, `pytest -v` for a more helpful output).
+All of the tests in `astartes` are written using the built-in python `unittest` module (to allow running without `pytest`) but we _highly_ recommend using `pytest`. To execute the tests from the `astartes` repository, simply type `pytest` after running the developer install (or alternately, `pytest -v` for a more helpful output).
 
 ### Adding New Samplers
 Adding a new sampler should extend the `abstract_sampler.py` abstract base class.
 
 It can be as simple as a passthrough to a another `train_test_split`, or it can be an original implementation that results in X and y being split into two lists. Take a look at `astartes/samplers/random_split.py` for a basic example!
 
-After the sampler has been implemented, add it to `__init__.py` in in `astartes/samplers` and it will automatically be unit tested. Additional unit tests to verify that hyperparameters can be properly passed, etc. are also reccomended.
+After the sampler has been implemented, add it to `__init__.py` in in `astartes/samplers` and it will automatically be unit tested. Additional unit tests to verify that hyperparameters can be properly passed, etc. are also recommended.
 
 For historical reasons, and as a guide for any developers who would like add new samplers, below is a running list of samplers which have been _considered_ for addition to `asartes` but ultimately not added for various reasons.
 
 #### Not Implemented Sampling Algorithms
 
-| Sampler Name | Reasoning |
-|:---:|---|
-| D-Optimal | Requires _a-priori_ knowledge of the test and train size which does not fit in the `astartes` framework (samplers are all agnostic to the size of the sets) and it is questionable if the use of the Fischer information matrix is actually meaningful in the context of sampling existing data rather than tuning for ideal data. |
-| Duplex | Requires knowing test and train size before execution, and can only partition data into two sets which owuld make it incompatible with `train_val_test_split`. |
+| Sampler Name | Reasoning | Relevant Link(s) |
+|:---:|---|---|
+| D-Optimal | Requires _a-priori_ knowledge of the test and train size which does not fit in the `astartes` framework (samplers are all agnostic to the size of the sets) and it is questionable if the use of the Fischer information matrix is actually meaningful in the context of sampling existing data rather than tuning for ideal data. | The [Wikipedia article for optimal design](https://en.wikipedia.org/wiki/Optimal_design#:~:text=Of%20course%2C%20fixing%20the%20number%20of%20experimental%20runs%20a%20priori%20would%20be%20impractical.) does a good job explaining why this is difficult, and points at some potential alternatives. |
+| Duplex | Requires knowing test and train size before execution, and can only partition data into two sets which would make it incompatible with `train_val_test_split`. | This [implementation in R](https://search.r-project.org/CRAN/refmans/prospectr/html/duplex.html#:~:text=The%20DUPLEX%20algorithm%20is%20similar,that%20are%20the%20farthest%20apart.) includes helpful references and a reference implementation. |
 
 ### Adding New Featurization Schemes
 All of the sampling methods implemented in `astartes` accept arbitrary arrays of numbers and return the sampled groups (with the exception of `Scaffold.py`). If you have an existing featurization scheme (i.e. take an arbitrary input and turn it into an array of numbers), we would be thrilled to include it in `astartes`.
 
 Adding a new interface should take on this format:
 
 ```python
@@ -178,15 +187,15 @@
         splitter=splitter,
         hopts=hopts,
     )
 ```
 
 If possible, we would like to also add an example Jupyter Notebook with any new interface to demonstrate to new users how it functions. See our other examples in the `examples` directory.
 
-Contact @JacksonBurns if you need assistance adding an existing workflow to `astartes`. If this featurization scheme requires additional dependencies to function, we may add it as an additional _extra_ package in the same way that `molecules` in installed.
+Contact [@JacksonBurns](https://github.com/JacksonBurns) if you need assistance adding an existing workflow to `astartes`. If this featurization scheme requires additional dependencies to function, we may add it as an additional _extra_ package in the same way that `molecules` in installed.
 
-## JORS Branch
+## JOSS Branch
 
-`astartes` corresponding JORS paper is stored in this repository on a separate branch. You can find `paper.tex` on the aptly named `jors-paper` paper. 
+`astartes` corresponding JOSS paper is stored in this repository on a separate branch. You can find `paper.md` on the aptly named `joss-paper` branch. 
 
-_Note for Maintainers_: To push changes from the `main` branch into the `jors-paper` branch, run the `Update JORS Branch` workflow.
+_Note for Maintainers_: To push changes from the `main` branch into the `joss-paper` branch, run the `Update JOSS Branch` workflow.
```

### Comparing `astartes-1.0.0b2/astartes.egg-info/SOURCES.txt` & `astartes-1.0.0rc1/astartes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astartes-1.0.0b2/test/test_astartes.py` & `astartes-1.0.0rc1/test/test_astartes.py`

 * *Files 13% similar despite different names*

```diff
@@ -82,17 +82,15 @@
                 self.X,
                 self.y,
                 labels=self.labels,
                 test_size=0.2,
                 val_size=0.2,
                 train_size=0.6,
                 sampler="random",
-                hopts={
-                    "random_state": 42,
-                },
+                random_state=42,
             )
             self.assertFalse(
                 len(w),
                 "\nNo warnings should have been raised when requesting a mathematically possible split."
                 "\nReceived {:d} warnings instead: \n -> {:s}".format(
                     len(w),
                     "\n -> ".join(
@@ -169,14 +167,149 @@
             np.testing.assert_array_equal(
                 labels_test,
                 np.array(["seven", "nine"]),
                 "Test labels incorrect.",
             )
         )
 
+    def test_train_val_test_split_extrpolation_shuffling(self):
+        """Split data into training, validation, and test sets with shuffling."""
+        with warnings.catch_warnings(record=True) as w:
+            warnings.filterwarnings("always")
+            (
+                X_train,
+                X_val,
+                X_test,
+                y_train,
+                y_val,
+                y_test,
+                labels_train,
+                labels_val,
+                labels_test,
+                clusters_train,
+                clusters_val,
+                clusters_test,
+            ) = train_val_test_split(
+                self.X,
+                self.y,
+                labels=self.labels,
+                test_size=0.1,
+                val_size=0.1,
+                train_size=0.8,
+                sampler="sphere_exclusion",
+                random_state=867_5309,
+            )
+            self.assertFalse(
+                len(w),
+                "\nNo warnings should have been raised when requesting a mathematically possible split."
+                "\nReceived {:d} warnings instead: \n -> {:s}".format(
+                    len(w),
+                    "\n -> ".join(
+                        [str(i.category.__name__) + ": " + str(i.message) for i in w]
+                    ),
+                ),
+            )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                X_train,
+                np.array(
+                    [
+                        [1, 0, 0, 0, 0],
+                        [1, 0, 0, 0, 0],
+                        [1, 1, 0, 0, 0],
+                        [1, 1, 0, 0, 0],
+                        [1, 1, 1, 0, 0],
+                        [1, 1, 1, 0, 0],
+                        [1, 1, 1, 1, 0],
+                        [1, 1, 1, 1, 0],
+                    ]
+                ),
+                "Train X incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                X_val,
+                np.array([[0, 0, 0, 0, 0]]),
+                "Validation X incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                X_test,
+                np.array([[1, 1, 1, 1, 1]]),
+                "Test X incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                y_train,
+                np.array([2, 6, 3, 7, 4, 8, 5, 9]),
+                "Train y incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                y_val,
+                np.array([1]),
+                "Validation y incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                y_test,
+                np.array([10]),
+                "Test y incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                labels_train,
+                np.array(
+                    ["two", "six", "three", "seven", "four", "eight", "five", "nine"]
+                ),
+                "Train labels incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                labels_val,
+                np.array(["one"]),
+                "Validation labels incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                labels_test,
+                np.array(["ten"]),
+                "Test labels incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                clusters_train,
+                np.array([4, 4, 0, 0, 1, 1, 5, 5]),
+                "Train cluster assignments incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                clusters_val,
+                np.array([2]),
+                "Validation cluster assignments incorrect.",
+            )
+        )
+        self.assertIsNone(
+            np.testing.assert_array_equal(
+                clusters_test,
+                np.array([3]),
+                "Test cluster assignments incorrect.",
+            )
+        )
+
     def test_insufficient_dataset_train(self):
         """If the user requests a split that would result in rounding down the size of the
         test set to zero, a helpful exception should be raised."""
         with self.assertRaises(InvalidConfigurationError):
             train_val_test_split(
                 self.X,
                 train_size=None,  # this will result in an empty train set due to rounding
@@ -364,17 +497,15 @@
             ) = train_test_split(
                 np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]),
                 np.array([10, 11, 12]),
                 labels=np.array(["apple", "banana", "apple"]),
                 test_size=0.5,
                 train_size=0.5,
                 sampler="random",
-                hopts={
-                    "random_state": 42,
-                },
+                random_state=42,
             )
             self.assertIsNone(
                 np.testing.assert_array_equal(
                     X_train,
                     np.array([[4, 5, 6]]),
                     "X_train incorrect.",
                 ),
@@ -412,55 +543,73 @@
                     labels_test,
                     np.array(["apple", "apple"]),
                     "labels_test incorrect.",
                 ),
             )
 
     def test_return_indices(self):
-        """Test the ability to return the indices and not the values."""
+        """Test the ability to return the indices and the values."""
         with self.assertWarns(ImperfectSplittingWarning):
-            (indices_train, indices_test,) = train_test_split(
+            (
+                train_X,
+                test_X,
+                train_y,
+                test_y,
+                train_labels,
+                test_labels,
+                train_indices,
+                test_indices,
+            ) = train_test_split(
                 np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]),
                 np.array([10, 11, 12]),
                 labels=np.array(["apple", "banana", "apple"]),
                 test_size=0.5,
                 train_size=0.5,
                 sampler="random",
-                hopts={
-                    "random_state": 42,
-                },
+                random_state=42,
                 return_indices=True,
             )
             self.assertIsNone(
                 np.testing.assert_array_equal(
-                    indices_test,
+                    test_indices,
                     np.array([2, 0]),
                     "Test indices incorrect.",
                 ),
             )
 
     def test_return_indices_with_validation(self):
         """Test the ability to return indices in train_val_test_split"""
         with self.assertWarns(ImperfectSplittingWarning):
-            (indices_train, indices_val, indices_test,) = train_val_test_split(
+            (
+                train_X,
+                val_X,
+                test_X,
+                train_y,
+                val_y,
+                test_y,
+                train_labels,
+                val_labels,
+                test_labels,
+                train_indices,
+                val_indices,
+                test_indices,
+            ) = train_val_test_split(
                 np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]),
                 np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]),
                 labels=np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]),
                 test_size=0.33,
                 val_size=0.33,
                 train_size=0.34,
                 sampler="random",
-                hopts={
-                    "random_state": 42,
-                },
+                random_state=42,
                 return_indices=True,
             )
             self.assertIsNone(
                 np.testing.assert_array_equal(
-                    indices_val,
+                    val_indices,
                     np.array([8, 2]),
                     "Validation indices incorrect.",
                 ),
             )
 
 
 if __name__ == "__main__":
```

### Comparing `astartes-1.0.0b2/test/test_molecules.py` & `astartes-1.0.0rc1/test/test_molecules.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 import unittest
 import warnings
 
 import numpy as np
+from rdkit import Chem
 
 from astartes.molecules import (
     train_test_split_molecules,
     train_val_test_split_molecules,
 )
 from astartes.samplers import (
     IMPLEMENTED_EXTRAPOLATION_SAMPLERS,
@@ -32,28 +33,54 @@
 
         qm9_smiles_short = [i.replace("\n", "") for i in lines[:100]]
         qm9_smiles_full = [i.replace("\n", "") for i in lines]
 
         self.X = np.array(qm9_smiles_short)
         self.y = np.array(list(range(len(qm9_smiles_short))))
 
+        molecule_array = []
+        for smile in qm9_smiles_short:
+            molecule_array.append(Chem.MolFromSmiles(smile))
+        self.molecules = np.array(molecule_array)
+
         self.X_long = np.array(qm9_smiles_full)
         self.y_long = np.array(list(range(len(qm9_smiles_full))))
 
     def test_molecules(self):
         """Try train_test_split molecules with every interpolative sampler."""
         for sampler in IMPLEMENTED_INTERPOLATION_SAMPLERS:
             tts = train_test_split_molecules(
                 self.X,
                 self.y,
                 train_size=0.2,
                 sampler=sampler,
                 fprints_hopts={"n_bits": 100},
             )
 
+    def test_molecules_with_rdkit(self):
+        """Try train_test_split molecules, every sampler, passing rdkit objects."""
+        for sampler in IMPLEMENTED_INTERPOLATION_SAMPLERS:
+            tts = train_test_split_molecules(
+                self.molecules,
+                self.y,
+                train_size=0.2,
+                sampler=sampler,
+                fprints_hopts={"n_bits": 100},
+            )
+
+    def test_molecules_with_troublesome_smiles(self):
+        """Helpful errors when rdkit graphs can't be featurized."""
+        with self.assertRaises(RuntimeError):
+            tts = train_test_split_molecules(
+                np.array(["Nc1ncnc2n(cnc12)[C@@H]3O[C@H](CN=[N]=N)[C@@H](O)[C@H]3O"]),
+                train_size=0.2,
+                sampler="random",
+                fprints_hopts={"n_bits": 100},
+            )
+
     def test_validation_split_molecules(self):
         """Try train_val_test_split_molecule with every extrapolative sampler."""
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             for sampler in IMPLEMENTED_EXTRAPOLATION_SAMPLERS:
                 if sampler == "scaffold":
                     continue
@@ -104,17 +131,15 @@
         """Test ability to pass through sampler hopts with molecules interface, expecting no warnings."""
         with warnings.catch_warnings(record=True) as w:
             warnings.filterwarnings("always")
             tts = train_test_split_molecules(
                 self.X,
                 self.y,
                 sampler="random",
-                hopts={
-                    "random_state": 42,
-                },
+                random_state=42,
             )
             self.assertFalse(
                 len(w),
                 "\nNo warnings should have been raised when requesting a mathematically possible split."
                 "\nReceived {:d} warnings instead: \n -> {:s}".format(
                     len(w),
                     "\n -> ".join(
@@ -136,15 +161,13 @@
                 "fpSize": 200,
                 "bitsPerHash": 4,
                 "useHs": 1,
                 "tgtDensity": 0.4,
                 "minSize": 64,
             },
             sampler="random",
-            hopts={
-                "random_state": 42,
-            },
+            random_state=42,
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

