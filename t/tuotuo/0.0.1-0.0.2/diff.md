# Comparing `tmp/tuotuo-0.0.1.tar.gz` & `tmp/tuotuo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuotuo-0.0.1.tar", last modified: Mon May  1 21:10:20 2023, max compression
+gzip compressed data, was "tuotuo-0.0.2.tar", last modified: Mon May  1 21:21:50 2023, max compression
```

## Comparing `tuotuo-0.0.1.tar` & `tuotuo-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.335137 tuotuo-0.0.1/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 tuotuo-0.0.1/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.313584 tuotuo-0.0.1/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.318576 tuotuo-0.0.1/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 tuotuo-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 tuotuo-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       22 2023-04-30 20:39:42.000000 tuotuo-0.0.1/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.318842 tuotuo-0.0.1/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 tuotuo-0.0.1/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 tuotuo-0.0.1/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)      782 2023-05-01 21:10:20.335317 tuotuo-0.0.1/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 tuotuo-0.0.1/README.md
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-03-04 12:30:22.000000 tuotuo-0.0.1/__init__.py
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 tuotuo-0.0.1/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.321413 tuotuo-0.0.1/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 tuotuo-0.0.1/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)     4572 2023-04-23 10:52:23.000000 tuotuo-0.0.1/notebook/computational_test.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    56721 2023-05-01 20:21:00.000000 tuotuo-0.0.1/notebook/main copy.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    83540 2023-04-23 10:52:50.000000 tuotuo-0.0.1/notebook/main.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    91088 2023-04-19 06:55:27.000000 tuotuo-0.0.1/notebook/reference.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    19221 2023-03-04 12:35:47.000000 tuotuo-0.0.1/notebook/test.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 tuotuo-0.0.1/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-01 21:10:20.335682 tuotuo-0.0.1/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1358 2023-05-01 21:10:11.000000 tuotuo-0.0.1/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.326457 tuotuo-0.0.1/src/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 tuotuo-0.0.1/src/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.314159 tuotuo-0.0.1/src/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.326739 tuotuo-0.0.1/src/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.1/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.327987 tuotuo-0.0.1/src/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 tuotuo-0.0.1/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-04-19 20:14:47.000000 tuotuo-0.0.1/src/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.1/src/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)   163779 2023-04-19 20:14:47.000000 tuotuo-0.0.1/src/cutils.html
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 tuotuo-0.0.1/src/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 tuotuo-0.0.1/src/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16219 2023-04-29 19:54:15.000000 tuotuo-0.0.1/src/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 tuotuo-0.0.1/src/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9789 2023-05-01 20:58:36.000000 tuotuo-0.0.1/src/utils.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:10:20.335021 tuotuo-0.0.1/tuotuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)      782 2023-05-01 21:10:20.000000 tuotuo-0.0.1/tuotuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      803 2023-05-01 21:10:20.000000 tuotuo-0.0.1/tuotuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-01 21:10:20.000000 tuotuo-0.0.1/tuotuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       35 2023-05-01 21:10:20.000000 tuotuo-0.0.1/tuotuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       15 2023-05-01 21:10:20.000000 tuotuo-0.0.1/tuotuo.egg-info/top_level.txt
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.434500 tuotuo-0.0.2/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 tuotuo-0.0.2/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.416888 tuotuo-0.0.2/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.421039 tuotuo-0.0.2/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 tuotuo-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 tuotuo-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       60 2023-05-01 21:19:43.000000 tuotuo-0.0.2/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.421280 tuotuo-0.0.2/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 tuotuo-0.0.2/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 tuotuo-0.0.2/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1515 2023-05-01 21:21:50.434655 tuotuo-0.0.2/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 tuotuo-0.0.2/README.md
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-03-04 12:30:22.000000 tuotuo-0.0.2/__init__.py
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 tuotuo-0.0.2/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.424353 tuotuo-0.0.2/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 tuotuo-0.0.2/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     4572 2023-04-23 10:52:23.000000 tuotuo-0.0.2/notebook/computational_test.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)    56721 2023-05-01 20:21:00.000000 tuotuo-0.0.2/notebook/main copy.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)    83540 2023-04-23 10:52:50.000000 tuotuo-0.0.2/notebook/main.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)    91088 2023-04-19 06:55:27.000000 tuotuo-0.0.2/notebook/reference.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)    19221 2023-03-04 12:35:47.000000 tuotuo-0.0.2/notebook/test.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 tuotuo-0.0.2/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-01 21:21:50.435072 tuotuo-0.0.2/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1555 2023-05-01 21:21:40.000000 tuotuo-0.0.2/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.429659 tuotuo-0.0.2/src/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 tuotuo-0.0.2/src/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.417298 tuotuo-0.0.2/src/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.429929 tuotuo-0.0.2/src/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.2/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.431256 tuotuo-0.0.2/src/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 tuotuo-0.0.2/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-04-19 20:14:47.000000 tuotuo-0.0.2/src/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.2/src/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)   163779 2023-04-19 20:14:47.000000 tuotuo-0.0.2/src/cutils.html
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 tuotuo-0.0.2/src/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 tuotuo-0.0.2/src/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16219 2023-04-29 19:54:15.000000 tuotuo-0.0.2/src/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 tuotuo-0.0.2/src/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9789 2023-05-01 20:58:36.000000 tuotuo-0.0.2/src/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.434382 tuotuo-0.0.2/tuotuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1515 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      803 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       28 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       15 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/top_level.txt
```

### Comparing `tuotuo-0.0.1/.DS_Store` & `tuotuo-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/.github/workflows/python-package.yml` & `tuotuo-0.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/.github/workflows/python-publish.yml` & `tuotuo-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/.vscode/c_cpp_properties.json` & `tuotuo-0.0.2/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/LICENSE` & `tuotuo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/README.md` & `tuotuo-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/cutils.cpython-38-darwin.so` & `tuotuo-0.0.2/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/notebook/computational_test.ipynb` & `tuotuo-0.0.2/notebook/computational_test.ipynb`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/notebook/main copy.ipynb` & `tuotuo-0.0.2/notebook/main copy.ipynb`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/notebook/main.ipynb` & `tuotuo-0.0.2/notebook/main.ipynb`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/notebook/reference.ipynb` & `tuotuo-0.0.2/notebook/reference.ipynb`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/notebook/test.ipynb` & `tuotuo-0.0.2/notebook/test.ipynb`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/requirements.txt` & `tuotuo-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/setup.py` & `tuotuo-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import Extension, setup
 from Cython.Build import cythonize
 import numpy 
 from distutils.core import setup
+from pathlib import Path
+this_directory = Path(__file__).parent
 
 extensions = [
     Extension(
         "src/cutils", 
         ["src/cutils.pyx"],
         include_dirs=[numpy.get_include()], 
     ),
 ]
 
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name = 'tuotuo',
     packages = ['src'],
-    version = '0.0.1',  
+    version = '0.0.2',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
-    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/ReleaseV0.0.2.tar.gz',
+    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-V0.0.2.tar.gz',
     keywords = ['Generative Topic Modelling','Latent Dirichlet Allocation'],
     install_requires=[            
         'numpy',
         'torch',
         'scipy',
-        'cython',
         'pyro',
         'nltk',
     ],
     ext_modules=cythonize(extensions, annotate=True),
     classifiers=[
         'Development Status :: 3 - Alpha', 
         'Intended Audience :: Science/Research',
```

### Comparing `tuotuo-0.0.1/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `tuotuo-0.0.2/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `tuotuo-0.0.2/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/cutils.c` & `tuotuo-0.0.2/src/cutils.c`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/cutils.cpython-38-darwin.so` & `tuotuo-0.0.2/src/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/cutils.html` & `tuotuo-0.0.2/src/cutils.html`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/cutils.pyx` & `tuotuo-0.0.2/src/cutils.pyx`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/generator.py` & `tuotuo-0.0.2/src/generator.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/lda_model.py` & `tuotuo-0.0.2/src/lda_model.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/text_pre_processor.py` & `tuotuo-0.0.2/src/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/src/utils.py` & `tuotuo-0.0.2/src/utils.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.1/tuotuo.egg-info/SOURCES.txt` & `tuotuo-0.0.2/tuotuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

