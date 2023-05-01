# Comparing `tmp/pdpyras-4.5.2.tar.gz` & `tmp/pdpyras-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpyras-4.5.2.tar", last modified: Thu Oct 13 20:14:37 2022, max compression
+gzip compressed data, was "pdpyras-5.0.0.tar", last modified: Mon May  1 18:31:36 2023, max compression
```

## Comparing `pdpyras-4.5.2.tar` & `pdpyras-5.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2022-10-13 20:14:37.876869 pdpyras-4.5.2/
--rw-r--r--   0 demitri    (503) staff       (20)     1053 2022-04-29 15:41:53.000000 pdpyras-4.5.2/LICENSE
--rw-r--r--   0 demitri    (503) staff       (20)      393 2022-10-13 20:14:37.876692 pdpyras-4.5.2/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)    36530 2022-10-13 20:03:05.000000 pdpyras-4.5.2/README.rst
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2022-10-13 20:14:37.876530 pdpyras-4.5.2/pdpyras.egg-info/
--rw-r--r--   0 demitri    (503) staff       (20)      393 2022-10-13 20:14:37.000000 pdpyras-4.5.2/pdpyras.egg-info/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)      192 2022-10-13 20:14:37.000000 pdpyras-4.5.2/pdpyras.egg-info/SOURCES.txt
--rw-r--r--   0 demitri    (503) staff       (20)        1 2022-10-13 20:14:37.000000 pdpyras-4.5.2/pdpyras.egg-info/dependency_links.txt
--rw-r--r--   0 demitri    (503) staff       (20)       17 2022-10-13 20:14:37.000000 pdpyras-4.5.2/pdpyras.egg-info/requires.txt
--rw-r--r--   0 demitri    (503) staff       (20)        8 2022-10-13 20:14:37.000000 pdpyras-4.5.2/pdpyras.egg-info/top_level.txt
--rw-r--r--   0 demitri    (503) staff       (20)    60072 2022-10-13 20:13:28.000000 pdpyras-4.5.2/pdpyras.py
--rw-r--r--   0 demitri    (503) staff       (20)       38 2022-10-13 20:14:37.876915 pdpyras-4.5.2/setup.cfg
--rw-r--r--   0 demitri    (503) staff       (20)      642 2022-10-13 20:13:28.000000 pdpyras-4.5.2/setup.py
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 18:31:36.206900 pdpyras-5.0.0/
+-rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.0/LICENSE
+-rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 18:31:36.206785 pdpyras-5.0.0/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-01 18:31:04.000000 pdpyras-5.0.0/README.rst
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 18:31:36.206607 pdpyras-5.0.0/pdpyras.egg-info/
+-rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 18:31:35.000000 pdpyras-5.0.0/pdpyras.egg-info/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)      192 2023-05-01 18:31:36.000000 pdpyras-5.0.0/pdpyras.egg-info/SOURCES.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        1 2023-05-01 18:31:35.000000 pdpyras-5.0.0/pdpyras.egg-info/dependency_links.txt
+-rw-r--r--   0 demitri    (503) staff       (20)       17 2023-05-01 18:31:36.000000 pdpyras-5.0.0/pdpyras.egg-info/requires.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        8 2023-05-01 18:31:36.000000 pdpyras-5.0.0/pdpyras.egg-info/top_level.txt
+-rw-r--r--   0 demitri    (503) staff       (20)    86705 2023-05-01 18:31:04.000000 pdpyras-5.0.0/pdpyras.py
+-rw-r--r--   0 demitri    (503) staff       (20)       38 2023-05-01 18:31:36.206947 pdpyras-5.0.0/setup.cfg
+-rw-r--r--   0 demitri    (503) staff       (20)      642 2023-05-01 18:31:04.000000 pdpyras-5.0.0/setup.py
```

### Comparing `pdpyras-4.5.2/LICENSE` & `pdpyras-5.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 PagerDuty
+Copyright (c) 2023 PagerDuty
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pdpyras-4.5.2/setup.py` & `pdpyras-5.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-__version__ = '4.5.2'
+__version__ = '5.0.0'
 
 if __name__ == '__main__':
     setup(
         name='pdpyras',
         description="PagerDuty Python REST API Sessions",
         long_description="A basic REST API client for PagerDuty based on Requests' Session class",
         py_modules=['pdpyras'],
         version=__version__,
         license='MIT',
         url='https://pagerduty.github.io/pdpyras',
         download_url='https://pypi.org/project/pdpyras/',
         install_requires=['requests', 'urllib3'],
         author='PagerDuty',
         author_email='support@pagerduty.com',
-        python_requires='>=3.5'
+        python_requires='>=3.6'
     )
```

