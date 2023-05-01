# Comparing `tmp/get_all_files-0.0.1.tar.gz` & `tmp/get_all_files-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_all_files-0.0.1.tar", max compression
+gzip compressed data, was "get_all_files-0.1.0.tar", max compression
```

## Comparing `get_all_files-0.0.1.tar` & `get_all_files-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-05-01 01:04:07.012745 get_all_files-0.0.1/LICENSE
--rw-r--r--   0        0        0     1525 2023-05-01 01:53:17.858619 get_all_files-0.0.1/README.md
--rw-r--r--   0        0        0      112 2023-05-01 01:42:46.767630 get_all_files-0.0.1/get_all_files/__init__.py
--rw-r--r--   0        0        0     2925 2023-05-01 01:49:16.153729 get_all_files-0.0.1/get_all_files/_get_all_files.py
--rw-r--r--   0        0        0      644 2023-05-01 02:12:27.564223 get_all_files-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 get_all_files-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-01 03:49:13.250535 get_all_files-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1877 2023-05-01 03:49:13.250535 get_all_files-0.1.0/README.md
+-rw-r--r--   0        0        0      198 2023-05-01 03:49:13.250535 get_all_files-0.1.0/get_all_files/__init__.py
+-rw-r--r--   0        0        0     2925 2023-05-01 03:49:13.250535 get_all_files-0.1.0/get_all_files/_get_all_files.py
+-rw-r--r--   0        0        0      644 2023-05-01 03:49:13.250535 get_all_files-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 get_all_files-0.1.0/PKG-INFO
```

### Comparing `get_all_files-0.0.1/LICENSE` & `get_all_files-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `get_all_files-0.0.1/README.md` & `get_all_files-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # READ ME
 
+![tests](https://github.com/bwheelz36/get_all_files/actions/workflows/run_tests.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/get_all_files.svg)](https://badge.fury.io/py/get_all_files)
+[![codecov](https://codecov.io/gh/bwheelz36/get_all_files/branch/main/graph/badge.svg?token=CCVB5BAR8W)](https://codecov.io/gh/bwheelz36/get_all_files)
+
+
 This is a very simple package which simply gets all the files with extension matching a list of extensions in a given
 directory. I found that I was including functionality like this in so many other projects I might as well just make
 it a package. Plus I wanted to play with poetry.
 
 ## install 
 
 ```bash
@@ -51,8 +56,8 @@
 home_dir = Path('~').expanduser()
 subfolders = [f.path for f in os.scandir(home_dir) if f.is_dir()]
 extension = 'txt'  # why not
 all_files = []
 for folder in subfolders:
     files = get_all_files(folder, extension, return_absolute_filepath=True)
     all_files.extend(files)
-```
+```
```

### Comparing `get_all_files-0.0.1/get_all_files/_get_all_files.py` & `get_all_files-0.1.0/get_all_files/_get_all_files.py`

 * *Files identical despite different names*

### Comparing `get_all_files-0.0.1/pyproject.toml` & `get_all_files-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get-all-files"
-version = "0.0.1"
+version = "0.1.0"
 description = "a simple package to get all files with given file extension in a directory"
 authors = ["brendan whelan <bwheelz360@gmail.com>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "get_all_files"}]
 
 [tool.poetry.dependencies]
```

### Comparing `get_all_files-0.0.1/PKG-INFO` & `get_all_files-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-all-files
-Version: 0.0.1
+Version: 0.1.0
 Summary: a simple package to get all files with given file extension in a directory
 License: LICENSE
 Author: brendan whelan
 Author-email: bwheelz360@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # READ ME
 
+![tests](https://github.com/bwheelz36/get_all_files/actions/workflows/run_tests.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/get_all_files.svg)](https://badge.fury.io/py/get_all_files)
+[![codecov](https://codecov.io/gh/bwheelz36/get_all_files/branch/main/graph/badge.svg?token=CCVB5BAR8W)](https://codecov.io/gh/bwheelz36/get_all_files)
+
+
 This is a very simple package which simply gets all the files with extension matching a list of extensions in a given
 directory. I found that I was including functionality like this in so many other projects I might as well just make
 it a package. Plus I wanted to play with poetry.
 
 ## install 
 
 ```bash
@@ -68,7 +73,8 @@
 subfolders = [f.path for f in os.scandir(home_dir) if f.is_dir()]
 extension = 'txt'  # why not
 all_files = []
 for folder in subfolders:
     files = get_all_files(folder, extension, return_absolute_filepath=True)
     all_files.extend(files)
 ```
+
```

