# Comparing `tmp/nurtelecom_gras_library-1.1.3.tar.gz` & `tmp/nurtelecom_gras_library-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nurtelecom_gras_library-1.1.3.tar", last modified: Mon May  1 09:25:08 2023, max compression
+gzip compressed data, was "nurtelecom_gras_library-1.1.4.tar", last modified: Mon May  1 09:29:05 2023, max compression
```

## Comparing `nurtelecom_gras_library-1.1.3.tar` & `nurtelecom_gras_library-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.161090 nurtelecom_gras_library-1.1.3/
--rw-r--r--   0 kazamabeks   (501) staff       (20)      693 2023-05-01 09:25:08.161539 nurtelecom_gras_library-1.1.3/PKG-INFO
--rw-r--r--   0 kazamabeks   (501) staff       (20)      315 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/README.md
--rw-r--r--   0 kazamabeks   (501) staff       (20)      107 2023-05-01 09:25:08.163325 nurtelecom_gras_library-1.1.3/setup.cfg
--rw-r--r--   0 kazamabeks   (501) staff       (20)     1324 2023-05-01 09:24:31.000000 nurtelecom_gras_library-1.1.3/setup.py
-drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.136416 nurtelecom_gras_library-1.1.3/src/
-drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.149080 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/
--rw-r--r--   0 kazamabeks   (501) staff       (20)     6927 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_data_importer.py
--rw-r--r--   0 kazamabeks   (501) staff       (20)     2797 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_geodata_importer.py
--rw-r--r--   0 kazamabeks   (501) staff       (20)      307 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/__init__.py
--rw-r--r--   0 kazamabeks   (501) staff       (20)     7399 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/additional_functions.py
-drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:25:08.160426 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/
--rw-r--r--   0 kazamabeks   (501) staff       (20)      693 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/PKG-INFO
--rw-r--r--   0 kazamabeks   (501) staff       (20)      479 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/SOURCES.txt
--rw-r--r--   0 kazamabeks   (501) staff       (20)        1 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/dependency_links.txt
--rw-r--r--   0 kazamabeks   (501) staff       (20)       60 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/requires.txt
--rw-r--r--   0 kazamabeks   (501) staff       (20)       24 2023-05-01 09:25:08.000000 nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library.egg-info/top_level.txt
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:29:05.023748 nurtelecom_gras_library-1.1.4/
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     1040 2023-05-01 09:29:05.024710 nurtelecom_gras_library-1.1.4/PKG-INFO
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      315 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.4/README.md
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      107 2023-05-01 09:29:05.025668 nurtelecom_gras_library-1.1.4/setup.cfg
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     1539 2023-05-01 09:28:30.000000 nurtelecom_gras_library-1.1.4/setup.py
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:29:05.009056 nurtelecom_gras_library-1.1.4/src/
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:29:05.017389 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     6927 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/PLSQL_data_importer.py
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     2797 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/PLSQL_geodata_importer.py
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      307 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/__init__.py
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     7399 2023-05-01 09:17:23.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/additional_functions.py
+drwxr-xr-x   0 kazamabeks   (501) staff       (20)        0 2023-05-01 09:29:05.022781 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library.egg-info/
+-rw-r--r--   0 kazamabeks   (501) staff       (20)     1040 2023-05-01 09:29:04.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library.egg-info/PKG-INFO
+-rw-r--r--   0 kazamabeks   (501) staff       (20)      479 2023-05-01 09:29:04.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library.egg-info/SOURCES.txt
+-rw-r--r--   0 kazamabeks   (501) staff       (20)        1 2023-05-01 09:29:04.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library.egg-info/dependency_links.txt
+-rw-r--r--   0 kazamabeks   (501) staff       (20)       60 2023-05-01 09:29:04.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library.egg-info/requires.txt
+-rw-r--r--   0 kazamabeks   (501) staff       (20)       24 2023-05-01 09:29:04.000000 nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library.egg-info/top_level.txt
```

### Comparing `nurtelecom_gras_library-1.1.3/setup.py` & `nurtelecom_gras_library-1.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
-
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='nurtelecom_gras_library',
-    version='1.1.3',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    version='1.1.4',
     license='MIT',
     author="Beksultan Tuleev",
     author_email='kazamabeks@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/beksultantuleev/nurtelecom_gras_library.git',
     keywords='NurTelecom',
```

### Comparing `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_data_importer.py` & `nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/PLSQL_data_importer.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/PLSQL_geodata_importer.py` & `nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/PLSQL_geodata_importer.py`

 * *Files identical despite different names*

### Comparing `nurtelecom_gras_library-1.1.3/src/nurtelecom_gras_library/additional_functions.py` & `nurtelecom_gras_library-1.1.4/src/nurtelecom_gras_library/additional_functions.py`

 * *Files identical despite different names*

