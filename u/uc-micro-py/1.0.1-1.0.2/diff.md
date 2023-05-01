# Comparing `tmp/uc-micro-py-1.0.1.tar.gz` & `tmp/uc-micro-py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uc-micro-py-1.0.1.tar", last modified: Tue Dec 15 11:56:01 2020, max compression
+gzip compressed data, was "/home/runner/work/uc.micro-py/uc.micro-py/dist/.tmp-_wbd9hyz/uc-micro-py-1.0.2.tar", last modified: Mon May  1 16:10:27 2023, max compression
```

## Comparing `uc-micro-py-1.0.1.tar` & `uc-micro-py-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)      300 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     2253 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      159 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      731 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1430 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/
--rw-r--r--   0 runner    (1001) docker     (116)       88 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/categories/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/categories/Cc/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/Cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/Cc/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/categories/Cf/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/Cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      239 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/Cf/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/categories/P/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/P/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1916 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/P/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/categories/Z/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/Z/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       68 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/Z/regex.py
--rw-r--r--   0 runner    (1001) docker     (116)       70 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/categories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/properties/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro/properties/Any/
--rw-r--r--   0 runner    (1001) docker     (116)       25 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/properties/Any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      154 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/properties/Any/regex.py
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-12-15 11:55:59.000000 uc-micro-py-1.0.1/uc_micro/properties/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      643 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       35 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-15 11:56:01.000000 uc-micro-py-1.0.1/uc_micro_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/test/test_uc_micro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/categories/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/categories/Cc/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/Cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/Cc/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/categories/Cf/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/Cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/Cf/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/categories/P/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/P/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/P/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/categories/Z/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/Z/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/Z/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/categories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/properties/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro/properties/Any/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/properties/Any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/properties/Any/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 16:10:02.000000 uc-micro-py-1.0.2/uc_micro/properties/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 16:10:27.000000 uc-micro-py-1.0.2/uc_micro_py.egg-info/top_level.txt
```

### Comparing `uc-micro-py-1.0.1/LICENSE` & `uc-micro-py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uc-micro-py-1.0.1/PKG-INFO` & `uc-micro-py-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 Metadata-Version: 2.1
 Name: uc-micro-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: Micro subset of unicode data files for linkify-it-py projects.
-Home-page: https://github.com/tsutsu3/uc.micro-py
 Author: tsutsu3
 License: MIT
-Description: # uc.micro-py
-        
-        [![pypi](https://img.shields.io/pypi/v/uc-micro-py)](https://pypi.org/project/uc-micro-py/)
-        [![CI](https://github.com/tsutsu3/uc.micro-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/uc.micro-py/actions)
-        [![codecov](https://codecov.io/gh/tsutsu3/uc.micro-py/branch/main/graph/badge.svg?token=5Y7559D69U)](https://codecov.io/gh/tsutsu3/uc.micro-py)
-        
-        This is a Python port of [uc.micro](https://github.com/markdown-it/uc.micro).
-        
-        > Micro subset of unicode data files for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) projects.
-        
-        **This package content is ONLY for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py)projects needs.**
-        
-        ## install
-        
-        ```bash
-        pip install uc-micro-py
-        ```
-        
+Project-URL: Homepage, https://github.com/tsutsu3/uc.micro-py
 Keywords: unicode
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# uc.micro-py
+
+[![pypi](https://img.shields.io/pypi/v/uc-micro-py)](https://pypi.org/project/uc-micro-py/)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/uc-micro-py/badges/version.svg)](https://anaconda.org/conda-forge/uc-micro-py)
+[![CI](https://github.com/tsutsu3/uc.micro-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/uc.micro-py/actions)
+[![codecov](https://codecov.io/gh/tsutsu3/uc.micro-py/branch/main/graph/badge.svg?token=5Y7559D69U)](https://codecov.io/gh/tsutsu3/uc.micro-py)
+
+This is a Python port of [uc.micro](https://github.com/markdown-it/uc.micro).
+
+> Micro subset of unicode data files for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) projects.
+
+**This package content is ONLY for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py)projects needs.**
+
+## install
+
+```bash
+pip install uc-micro-py
+```
+
+or
+
+```bash
+conda install -c conda-forge uc-micro-py
+```
```

### Comparing `uc-micro-py-1.0.1/README.md` & `uc-micro-py-1.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # uc.micro-py
 
 [![pypi](https://img.shields.io/pypi/v/uc-micro-py)](https://pypi.org/project/uc-micro-py/)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/uc-micro-py/badges/version.svg)](https://anaconda.org/conda-forge/uc-micro-py)
 [![CI](https://github.com/tsutsu3/uc.micro-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/uc.micro-py/actions)
 [![codecov](https://codecov.io/gh/tsutsu3/uc.micro-py/branch/main/graph/badge.svg?token=5Y7559D69U)](https://codecov.io/gh/tsutsu3/uc.micro-py)
 
 This is a Python port of [uc.micro](https://github.com/markdown-it/uc.micro).
 
 > Micro subset of unicode data files for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) projects.
 
 **This package content is ONLY for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py)projects needs.**
 
 ## install
 
 ```bash
 pip install uc-micro-py
 ```
+
+or
+
+```bash
+conda install -c conda-forge uc-micro-py
+```
```

### Comparing `uc-micro-py-1.0.1/uc_micro/categories/P/regex.py` & `uc-micro-py-1.0.2/uc_micro/categories/P/regex.py`

 * *Files identical despite different names*

### Comparing `uc-micro-py-1.0.1/uc_micro_py.egg-info/PKG-INFO` & `uc-micro-py-1.0.2/uc_micro_py.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 Metadata-Version: 2.1
 Name: uc-micro-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: Micro subset of unicode data files for linkify-it-py projects.
-Home-page: https://github.com/tsutsu3/uc.micro-py
 Author: tsutsu3
 License: MIT
-Description: # uc.micro-py
-        
-        [![pypi](https://img.shields.io/pypi/v/uc-micro-py)](https://pypi.org/project/uc-micro-py/)
-        [![CI](https://github.com/tsutsu3/uc.micro-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/uc.micro-py/actions)
-        [![codecov](https://codecov.io/gh/tsutsu3/uc.micro-py/branch/main/graph/badge.svg?token=5Y7559D69U)](https://codecov.io/gh/tsutsu3/uc.micro-py)
-        
-        This is a Python port of [uc.micro](https://github.com/markdown-it/uc.micro).
-        
-        > Micro subset of unicode data files for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) projects.
-        
-        **This package content is ONLY for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py)projects needs.**
-        
-        ## install
-        
-        ```bash
-        pip install uc-micro-py
-        ```
-        
+Project-URL: Homepage, https://github.com/tsutsu3/uc.micro-py
 Keywords: unicode
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# uc.micro-py
+
+[![pypi](https://img.shields.io/pypi/v/uc-micro-py)](https://pypi.org/project/uc-micro-py/)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/uc-micro-py/badges/version.svg)](https://anaconda.org/conda-forge/uc-micro-py)
+[![CI](https://github.com/tsutsu3/uc.micro-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/uc.micro-py/actions)
+[![codecov](https://codecov.io/gh/tsutsu3/uc.micro-py/branch/main/graph/badge.svg?token=5Y7559D69U)](https://codecov.io/gh/tsutsu3/uc.micro-py)
+
+This is a Python port of [uc.micro](https://github.com/markdown-it/uc.micro).
+
+> Micro subset of unicode data files for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) projects.
+
+**This package content is ONLY for [linkify-it-py](https://github.com/tsutsu3/linkify-it-py)projects needs.**
+
+## install
+
+```bash
+pip install uc-micro-py
+```
+
+or
+
+```bash
+conda install -c conda-forge uc-micro-py
+```
```

### Comparing `uc-micro-py-1.0.1/uc_micro_py.egg-info/SOURCES.txt` & `uc-micro-py-1.0.2/uc_micro_py.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+tox.ini
+test/test_uc_micro.py
 uc_micro/__init__.py
 uc_micro/categories/__init__.py
 uc_micro/categories/Cc/__init__.py
 uc_micro/categories/Cc/regex.py
 uc_micro/categories/Cf/__init__.py
 uc_micro/categories/Cf/regex.py
 uc_micro/categories/P/__init__.py
```

