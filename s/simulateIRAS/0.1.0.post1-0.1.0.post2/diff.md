# Comparing `tmp/simulateIRAS-0.1.0.post1.tar.gz` & `tmp/simulateIRAS-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulateIRAS-0.1.0.post1.tar", last modified: Mon May  1 20:53:32 2023, max compression
+gzip compressed data, was "simulateIRAS-0.1.0.post2.tar", last modified: Mon May  1 21:06:23 2023, max compression
```

## Comparing `simulateIRAS-0.1.0.post1.tar` & `simulateIRAS-0.1.0.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.091927 simulateIRAS-0.1.0.post1/
--rw-rw-rw-   0        0        0    35184 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     1288 2023-05-01 20:53:32.091927 simulateIRAS-0.1.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/README.md
--rw-rw-rw-   0        0        0       99 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 20:53:32.091927 simulateIRAS-0.1.0.post1/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-05-01 20:53:22.000000 simulateIRAS-0.1.0.post1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.083927 simulateIRAS-0.1.0.post1/src/
--rw-rw-rw-   0        0        0        2 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.090927 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/
--rw-rw-rw-   0        0        0     1288 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-01 20:53:32.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 20:53:31.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9905 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/src/simulateIRAS.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:53:32.090927 simulateIRAS-0.1.0.post1/tests/
--rw-rw-rw-   0        0        0      146 2023-05-01 20:47:08.000000 simulateIRAS-0.1.0.post1/tests/test_code.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.768756 simulateIRAS-0.1.0.post2/
+-rw-rw-rw-   0        0        0    35184 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/MANIFEST.in
+-rw-rw-rw-   0        0        0      893 2023-05-01 21:06:23.768756 simulateIRAS-0.1.0.post2/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/README.md
+-rw-rw-rw-   0        0        0       99 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 21:06:23.768756 simulateIRAS-0.1.0.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-01 21:06:12.000000 simulateIRAS-0.1.0.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.757759 simulateIRAS-0.1.0.post2/src/
+-rw-rw-rw-   0        0        0        2 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.763755 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/
+-rw-rw-rw-   0        0        0      893 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 21:06:23.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9905 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/src/simulateIRAS.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:23.767758 simulateIRAS-0.1.0.post2/tests/
+-rw-rw-rw-   0        0        0      146 2023-05-01 21:04:58.000000 simulateIRAS-0.1.0.post2/tests/test_code.py
```

### Comparing `simulateIRAS-0.1.0.post1/LICENSE` & `simulateIRAS-0.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post1/setup.py` & `simulateIRAS-0.1.0.post2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="simulateIRAS",
-    version = '0.1.0-1',
+    version = '0.1.0-2',
     description="A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements",
     py_modules = ["simulateIRAS"],
     package_dir = {'':'src'},
     
     author="coconnor24",
     author_email="coconnor@g.harvard.edu",
     
@@ -18,30 +18,22 @@
     
     license="GPLv3",
     
     classifiers  = [
         'Development Status :: 4 - Beta',
         
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         
         "License :: OSI Approved :: BSD License",
         
-        'Intended Audience :: Developers',
-        'Intended Audience :: Other Audience',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics',
         
         'Operating System :: Microsoft :: Windows',
-        'Operating System :: OS Independent',
         ],
         
-    install_requires=["numpy", "scipy"],
+    install_requires=['numpy', 'scipy'],
     keywords = ["IRAS", "Surface Science", "FTIR", "doi:"]
 )
```

### Comparing `simulateIRAS-0.1.0.post1/src/simulateIRAS.py` & `simulateIRAS-0.1.0.post2/src/simulateIRAS.py`

 * *Files identical despite different names*

