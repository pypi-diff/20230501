# Comparing `tmp/pdpyras-5.0.0.tar.gz` & `tmp/pdpyras-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpyras-5.0.0.tar", last modified: Mon May  1 18:31:36 2023, max compression
+gzip compressed data, was "pdpyras-5.0.1.tar", last modified: Mon May  1 19:52:54 2023, max compression
```

## Comparing `pdpyras-5.0.0.tar` & `pdpyras-5.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 18:31:36.206900 pdpyras-5.0.0/
--rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.0/LICENSE
--rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 18:31:36.206785 pdpyras-5.0.0/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-01 18:31:04.000000 pdpyras-5.0.0/README.rst
-drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 18:31:36.206607 pdpyras-5.0.0/pdpyras.egg-info/
--rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 18:31:35.000000 pdpyras-5.0.0/pdpyras.egg-info/PKG-INFO
--rw-r--r--   0 demitri    (503) staff       (20)      192 2023-05-01 18:31:36.000000 pdpyras-5.0.0/pdpyras.egg-info/SOURCES.txt
--rw-r--r--   0 demitri    (503) staff       (20)        1 2023-05-01 18:31:35.000000 pdpyras-5.0.0/pdpyras.egg-info/dependency_links.txt
--rw-r--r--   0 demitri    (503) staff       (20)       17 2023-05-01 18:31:36.000000 pdpyras-5.0.0/pdpyras.egg-info/requires.txt
--rw-r--r--   0 demitri    (503) staff       (20)        8 2023-05-01 18:31:36.000000 pdpyras-5.0.0/pdpyras.egg-info/top_level.txt
--rw-r--r--   0 demitri    (503) staff       (20)    86705 2023-05-01 18:31:04.000000 pdpyras-5.0.0/pdpyras.py
--rw-r--r--   0 demitri    (503) staff       (20)       38 2023-05-01 18:31:36.206947 pdpyras-5.0.0/setup.cfg
--rw-r--r--   0 demitri    (503) staff       (20)      642 2023-05-01 18:31:04.000000 pdpyras-5.0.0/setup.py
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 19:52:54.548575 pdpyras-5.0.1/
+-rw-r--r--   0 demitri    (503) staff       (20)     1053 2023-05-01 18:31:04.000000 pdpyras-5.0.1/LICENSE
+-rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 19:52:54.548441 pdpyras-5.0.1/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)     4792 2023-05-01 18:31:04.000000 pdpyras-5.0.1/README.rst
+drwxr-xr-x   0 demitri    (503) staff       (20)        0 2023-05-01 19:52:54.548263 pdpyras-5.0.1/pdpyras.egg-info/
+-rw-r--r--   0 demitri    (503) staff       (20)      393 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/PKG-INFO
+-rw-r--r--   0 demitri    (503) staff       (20)      192 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/SOURCES.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        1 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/dependency_links.txt
+-rw-r--r--   0 demitri    (503) staff       (20)       29 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/requires.txt
+-rw-r--r--   0 demitri    (503) staff       (20)        8 2023-05-01 19:52:54.000000 pdpyras-5.0.1/pdpyras.egg-info/top_level.txt
+-rw-r--r--   0 demitri    (503) staff       (20)    86705 2023-05-01 19:52:37.000000 pdpyras-5.0.1/pdpyras.py
+-rw-r--r--   0 demitri    (503) staff       (20)       38 2023-05-01 19:52:54.548626 pdpyras-5.0.1/setup.cfg
+-rw-r--r--   0 demitri    (503) staff       (20)      657 2023-05-01 19:52:37.000000 pdpyras-5.0.1/setup.py
```

### Comparing `pdpyras-5.0.0/LICENSE` & `pdpyras-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.0/README.rst` & `pdpyras-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pdpyras-5.0.0/pdpyras.py` & `pdpyras-5.0.1/pdpyras.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Libraries from PyPI
 import requests
 from deprecation import deprecated, DeprecatedWarning
 from urllib3.exceptions import HTTPError, PoolError
 from requests.exceptions import RequestException
 
-__version__ = '5.0.0'
+__version__ = '5.0.1'
 
 #######################
 ### CLIENT DEFAULTS ###
 #######################
 ITERATION_LIMIT = 1e4
 """
 The maximum position of a result in classic pagination.
```

### Comparing `pdpyras-5.0.0/setup.py` & `pdpyras-5.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-__version__ = '5.0.0'
+__version__ = '5.0.1'
 
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
-        install_requires=['requests', 'urllib3'],
+        install_requires=['requests', 'urllib3', 'deprecation'],
         author='PagerDuty',
         author_email='support@pagerduty.com',
         python_requires='>=3.6'
     )
```

