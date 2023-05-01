# Comparing `tmp/testprepup-0.3.tar.gz` & `tmp/testprepup-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testprepup-0.3.tar", last modified: Mon May  1 01:22:31 2023, max compression
+gzip compressed data, was "testprepup-0.4.tar", last modified: Mon May  1 02:24:54 2023, max compression
```

## Comparing `testprepup-0.3.tar` & `testprepup-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 01:22:31.031663 testprepup-0.3/
--rw-rw-rw-   0        0        0       55 2023-05-01 01:22:31.027740 testprepup-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-01 01:22:31.032626 testprepup-0.3/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-05-01 01:22:19.000000 testprepup-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:22:31.025791 testprepup-0.3/testprepup.egg-info/
--rw-rw-rw-   0        0        0       55 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 02:24:54.062658 testprepup-0.4/
+-rw-rw-rw-   0        0        0       55 2023-05-01 02:24:54.062658 testprepup-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-01 02:24:54.063633 testprepup-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      873 2023-05-01 02:24:46.000000 testprepup-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 02:24:54.061680 testprepup-0.4/testprepup.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-05-01 02:24:53.000000 testprepup-0.4/testprepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-01 02:24:53.000000 testprepup-0.4/testprepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:24:53.000000 testprepup-0.4/testprepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-05-01 02:24:53.000000 testprepup-0.4/testprepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2023-05-01 02:24:53.000000 testprepup-0.4/testprepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 02:24:53.000000 testprepup-0.4/testprepup.egg-info/top_level.txt
```

### Comparing `testprepup-0.3/setup.py` & `testprepup-0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testprepup',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'inspect=testprepup.test.inspect:main',
-            'explore=testprepup.test.explore:main',
-            'impute=testprepup.test.impute:main',
-            "normalize=testprepup.test.normalize:main",
+            'inspect=inspect:main',
+            'explore=explore:main',
+            'impute=impute:main',
+            "normalize=normalize:main",
         ],
     },
     install_requires=[
         "argparse",
         "polars",
         "termcolor",
         "pyfiglet",
```

