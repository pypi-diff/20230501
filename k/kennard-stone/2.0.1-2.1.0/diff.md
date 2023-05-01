# Comparing `tmp/kennard_stone-2.0.1.tar.gz` & `tmp/kennard_stone-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kennard_stone-2.0.1.tar", last modified: Tue Apr 25 14:21:56 2023, max compression
+gzip compressed data, was "kennard_stone-2.1.0.tar", last modified: Mon May  1 14:30:08 2023, max compression
```

## Comparing `kennard_stone-2.0.1.tar` & `kennard_stone-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-25 14:21:56.864410 kennard_stone-2.0.1/
--rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.0.1/LICENSE
--rw-r--r--   0 yu9824     (501) staff       (20)       71 2023-04-22 06:08:03.000000 kennard_stone-2.0.1/MANIFEST.in
--rw-r--r--   0 yu9824     (501) staff       (20)     5431 2023-04-25 14:21:56.864278 kennard_stone-2.0.1/PKG-INFO
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-25 14:21:56.863433 kennard_stone-2.0.1/kennard_stone/
--rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-04-25 14:15:51.000000 kennard_stone-2.0.1/kennard_stone/__init__.py
--rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-22 05:20:01.000000 kennard_stone-2.0.1/kennard_stone/_deprecated.py
--rw-r--r--   0 yu9824     (501) staff       (20)     9616 2023-04-25 13:35:46.000000 kennard_stone-2.0.1/kennard_stone/kennard_stone.py
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-25 14:21:56.864099 kennard_stone-2.0.1/kennard_stone.egg-info/
--rw-r--r--   0 yu9824     (501) staff       (20)     5431 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/PKG-INFO
--rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/SOURCES.txt
--rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/dependency_links.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/requires.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/top_level.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:20:01.000000 kennard_stone-2.0.1/requirements.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-04-25 14:21:56.864450 kennard_stone-2.0.1/setup.cfg
--rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 06:08:03.000000 kennard_stone-2.0.1/setup.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-01 14:30:08.072441 kennard_stone-2.1.0/
+-rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.1.0/LICENSE
+-rw-r--r--   0 yu9824     (501) staff       (20)       71 2023-04-22 06:08:03.000000 kennard_stone-2.1.0/MANIFEST.in
+-rw-r--r--   0 yu9824     (501) staff       (20)     6217 2023-05-01 14:30:08.072330 kennard_stone-2.1.0/PKG-INFO
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-01 14:30:08.071564 kennard_stone-2.1.0/kennard_stone/
+-rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-05-01 14:28:01.000000 kennard_stone-2.1.0/kennard_stone/__init__.py
+-rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-22 05:20:01.000000 kennard_stone-2.1.0/kennard_stone/_deprecated.py
+-rw-r--r--   0 yu9824     (501) staff       (20)    16105 2023-05-01 14:28:01.000000 kennard_stone-2.1.0/kennard_stone/kennard_stone.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-01 14:30:08.072176 kennard_stone-2.1.0/kennard_stone.egg-info/
+-rw-r--r--   0 yu9824     (501) staff       (20)     6217 2023-05-01 14:30:07.000000 kennard_stone-2.1.0/kennard_stone.egg-info/PKG-INFO
+-rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-05-01 14:30:08.000000 kennard_stone-2.1.0/kennard_stone.egg-info/SOURCES.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-05-01 14:30:07.000000 kennard_stone-2.1.0/kennard_stone.egg-info/dependency_links.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-05-01 14:30:07.000000 kennard_stone-2.1.0/kennard_stone.egg-info/requires.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-05-01 14:30:08.000000 kennard_stone-2.1.0/kennard_stone.egg-info/top_level.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:20:01.000000 kennard_stone-2.1.0/requirements.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-05-01 14:30:08.072477 kennard_stone-2.1.0/setup.cfg
+-rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 06:08:03.000000 kennard_stone-2.1.0/setup.py
```

### Comparing `kennard_stone-2.0.1/LICENSE` & `kennard_stone-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kennard_stone-2.0.1/PKG-INFO` & `kennard_stone-2.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kennard_stone
-Version: 2.0.1
+Version: 2.1.0
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
@@ -17,19 +17,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kennard Stone
+
 [![python_badge](https://img.shields.io/pypi/pyversions/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![license_badge](https://img.shields.io/pypi/l/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![PyPI version](https://badge.fury.io/py/kennard-stone.svg)](https://pypi.org/project/kennard-stone/)
 [![Downloads](https://pepy.tech/badge/kennard-stone)](https://pepy.tech/project/kennard-stone)
 
+[![Test on each version](https://github.com/yu9824/kennard_stone/actions/workflows/pytest-on-each-version.yaml/badge.svg)](https://github.com/yu9824/kennard_stone/actions/workflows/pytest-on-each-version.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/version.svg)](https://anaconda.org/conda-forge/kennard-stone)
 [![Anaconda-platform badge](https://anaconda.org/conda-forge/kennard-stone/badges/platforms.svg)](https://anaconda.org/conda-forge/kennard-stone)
 
 ## What is this?
 
 This is an algorithm for evenly partitioning data in a `scikit-learn`-like interface. (See [References](#References) for details of the algorithm.)
@@ -122,61 +124,81 @@
 
 #### kennard_stone
 
 ```python
 from kennard_stone import KFold
 from sklearn.model_selection import cross_validate
 
-kf = KFold(n_splits = 5)
-print(cross_validate(estimator, X, y, cv = kf))
+kf = KFold(n_splits=5)
+print(cross_validate(estimator, X, y, cv=kf))
 ```
 
 #### scikit-learn
 
 ```python
 from sklearn.model_selection import KFold
 from sklearn.model_selection import cross_validate
 
-kf = KFold(n_splits = 5, shuffle = True, random_state = 334)
-print(cross_validate(estimator, X, y, cv = kf))
+kf = KFold(n_splits=5, shuffle=True, random_state=334)
+print(cross_validate(estimator, X, y, cv=kf))
 ```
 OR
 ```python
 from sklearn.model_selection import cross_validate
 
-print(cross_validate(estimator, X, y, cv = 5))
+print(cross_validate(estimator, X, y, cv=5))
 ```
 
 
 ## Notes
 
 There is no notion of `random_state` or `shuffle` because the partitioning is determined uniquely for the dataset.
 If these arguments are included, they do not cause an error. They simply have no effect on the result. Please be careful.
 
 If you want to run the notebook in example directory, you will need to additionally download `pandas`, `matplotlib`, `seaborn`, `tqdm`, and `jupyter` other than the packages in requirements.txt.
 
+## Parallelization (since v2.1.0)
+
+This algorithm is very computationally intensive and takes a lot of computation time.
+To solve this problem, we have implemented parallelization and optimized the algorithm since v2.1.0.
+`n_jobs` can be specified for parallelization as in the scikit-learn-like api.
+
+
 ## LICENSE
 
 MIT Licence
 
 Copyright (c) 2021 yu9824
 
 
 ## References
+
 ### Papers
 
-* R. W. Kennard & L. A. Stone (1969) Computer Aided Design of Experiments, Technometrics, 11:1, 137-148, DOI: [10.1080/00401706.1969.10490666](https://doi.org/10.1080/00401706.1969.10490666)
+- R. W. Kennard & L. A. Stone (1969) Computer Aided Design of Experiments, Technometrics, 11:1, 137-148, DOI: [10.1080/00401706.1969.10490666](https://doi.org/10.1080/00401706.1969.10490666)
 
 ### Sites
 
-* [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/) (Japanese site)
+- [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/) (Japanese site)
 
 
 ## Histories
 
 ### v2.0.0
 
 - Define Extended Kennard-Stone algorithm (multi-class) i.e. Improve KFold algorithm.
 - Delete `alternate` argument in `KFold`.
 - Delete requirements of `pandas`.
 
+### v2.0.1
+
+- Fix bug with Python3.7.
+
+### v2.1.0
+
+- Optimize algorithm
+- Deal with Large number of data.
+  - parallel calculation when calculating distance (Add `n_jobs` argument)
+  - recursion number settings
+- Add other than "euclidean" calculation methods (Add `metric` argument)
+
```

### Comparing `kennard_stone-2.0.1/kennard_stone/_deprecated.py` & `kennard_stone-2.1.0/kennard_stone/_deprecated.py`

 * *Files identical despite different names*

### Comparing `kennard_stone-2.0.1/kennard_stone.egg-info/PKG-INFO` & `kennard_stone-2.1.0/kennard_stone.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kennard-stone
-Version: 2.0.1
+Version: 2.1.0
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
@@ -17,19 +17,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kennard Stone
+
 [![python_badge](https://img.shields.io/pypi/pyversions/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![license_badge](https://img.shields.io/pypi/l/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![PyPI version](https://badge.fury.io/py/kennard-stone.svg)](https://pypi.org/project/kennard-stone/)
 [![Downloads](https://pepy.tech/badge/kennard-stone)](https://pepy.tech/project/kennard-stone)
 
+[![Test on each version](https://github.com/yu9824/kennard_stone/actions/workflows/pytest-on-each-version.yaml/badge.svg)](https://github.com/yu9824/kennard_stone/actions/workflows/pytest-on-each-version.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/version.svg)](https://anaconda.org/conda-forge/kennard-stone)
 [![Anaconda-platform badge](https://anaconda.org/conda-forge/kennard-stone/badges/platforms.svg)](https://anaconda.org/conda-forge/kennard-stone)
 
 ## What is this?
 
 This is an algorithm for evenly partitioning data in a `scikit-learn`-like interface. (See [References](#References) for details of the algorithm.)
@@ -122,61 +124,81 @@
 
 #### kennard_stone
 
 ```python
 from kennard_stone import KFold
 from sklearn.model_selection import cross_validate
 
-kf = KFold(n_splits = 5)
-print(cross_validate(estimator, X, y, cv = kf))
+kf = KFold(n_splits=5)
+print(cross_validate(estimator, X, y, cv=kf))
 ```
 
 #### scikit-learn
 
 ```python
 from sklearn.model_selection import KFold
 from sklearn.model_selection import cross_validate
 
-kf = KFold(n_splits = 5, shuffle = True, random_state = 334)
-print(cross_validate(estimator, X, y, cv = kf))
+kf = KFold(n_splits=5, shuffle=True, random_state=334)
+print(cross_validate(estimator, X, y, cv=kf))
 ```
 OR
 ```python
 from sklearn.model_selection import cross_validate
 
-print(cross_validate(estimator, X, y, cv = 5))
+print(cross_validate(estimator, X, y, cv=5))
 ```
 
 
 ## Notes
 
 There is no notion of `random_state` or `shuffle` because the partitioning is determined uniquely for the dataset.
 If these arguments are included, they do not cause an error. They simply have no effect on the result. Please be careful.
 
 If you want to run the notebook in example directory, you will need to additionally download `pandas`, `matplotlib`, `seaborn`, `tqdm`, and `jupyter` other than the packages in requirements.txt.
 
+## Parallelization (since v2.1.0)
+
+This algorithm is very computationally intensive and takes a lot of computation time.
+To solve this problem, we have implemented parallelization and optimized the algorithm since v2.1.0.
+`n_jobs` can be specified for parallelization as in the scikit-learn-like api.
+
+
 ## LICENSE
 
 MIT Licence
 
 Copyright (c) 2021 yu9824
 
 
 ## References
+
 ### Papers
 
-* R. W. Kennard & L. A. Stone (1969) Computer Aided Design of Experiments, Technometrics, 11:1, 137-148, DOI: [10.1080/00401706.1969.10490666](https://doi.org/10.1080/00401706.1969.10490666)
+- R. W. Kennard & L. A. Stone (1969) Computer Aided Design of Experiments, Technometrics, 11:1, 137-148, DOI: [10.1080/00401706.1969.10490666](https://doi.org/10.1080/00401706.1969.10490666)
 
 ### Sites
 
-* [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/) (Japanese site)
+- [https://datachemeng.com/trainingtestdivision/](https://datachemeng.com/trainingtestdivision/) (Japanese site)
 
 
 ## Histories
 
 ### v2.0.0
 
 - Define Extended Kennard-Stone algorithm (multi-class) i.e. Improve KFold algorithm.
 - Delete `alternate` argument in `KFold`.
 - Delete requirements of `pandas`.
 
+### v2.0.1
+
+- Fix bug with Python3.7.
+
+### v2.1.0
+
+- Optimize algorithm
+- Deal with Large number of data.
+  - parallel calculation when calculating distance (Add `n_jobs` argument)
+  - recursion number settings
+- Add other than "euclidean" calculation methods (Add `metric` argument)
+
```

### Comparing `kennard_stone-2.0.1/setup.py` & `kennard_stone-2.1.0/setup.py`

 * *Files identical despite different names*

