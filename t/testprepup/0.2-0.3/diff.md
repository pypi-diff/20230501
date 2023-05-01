# Comparing `tmp/testprepup-0.2.tar.gz` & `tmp/testprepup-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testprepup-0.2.tar", last modified: Mon May  1 01:13:26 2023, max compression
+gzip compressed data, was "testprepup-0.3.tar", last modified: Mon May  1 01:22:31 2023, max compression
```

## Comparing `testprepup-0.2.tar` & `testprepup-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 01:13:26.370081 testprepup-0.2/
--rw-rw-rw-   0        0        0       55 2023-05-01 01:13:26.369104 testprepup-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-01 01:13:26.371055 testprepup-0.2/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-05-01 01:13:22.000000 testprepup-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:13:26.367162 testprepup-0.2/testprepup.egg-info/
--rw-rw-rw-   0        0        0       55 2023-05-01 01:13:26.000000 testprepup-0.2/testprepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-01 01:13:26.000000 testprepup-0.2/testprepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:13:26.000000 testprepup-0.2/testprepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-05-01 01:13:26.000000 testprepup-0.2/testprepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2023-05-01 01:13:26.000000 testprepup-0.2/testprepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:13:26.000000 testprepup-0.2/testprepup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 01:22:31.031663 testprepup-0.3/
+-rw-rw-rw-   0        0        0       55 2023-05-01 01:22:31.027740 testprepup-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-01 01:22:31.032626 testprepup-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-05-01 01:22:19.000000 testprepup-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 01:22:31.025791 testprepup-0.3/testprepup.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 01:22:30.000000 testprepup-0.3/testprepup.egg-info/top_level.txt
```

### Comparing `testprepup-0.2/setup.py` & `testprepup-0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testprepup',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'inspect=test.inspect:main',
-            'explore=test.explore:main',
-            'impute=test.impute:main',
-            "normalize=test.normalize:main",
+            'inspect=testprepup.test.inspect:main',
+            'explore=testprepup.test.explore:main',
+            'impute=testprepup.test.impute:main',
+            "normalize=testprepup.test.normalize:main",
         ],
     },
     install_requires=[
         "argparse",
         "polars",
         "termcolor",
         "pyfiglet",
```

