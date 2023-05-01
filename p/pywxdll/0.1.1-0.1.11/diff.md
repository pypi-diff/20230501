# Comparing `tmp/pywxdll-0.1.1.tar.gz` & `tmp/pywxdll-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywxdll-0.1.1.tar", last modified: Mon May  1 18:03:21 2023, max compression
+gzip compressed data, was "dist/pywxdll-0.1.11.tar", last modified: Mon May  1 18:35:41 2023, max compression
```

## Comparing `pywxdll-0.1.1.tar` & `pywxdll-0.1.11.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-01 18:03:21.000000 pywxdll-0.1.1/
--rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.1/LICENSE
--rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 17:30:43.000000 pywxdll-0.1.1/MANIFEST.in
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-01 18:03:21.000000 pywxdll-0.1.1/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      471 2023-05-01 16:22:12.000000 pywxdll-0.1.1/README.md
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      226 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/SOURCES.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/dependency_links.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       45 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/entry_points.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       17 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/requires.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-01 18:03:21.000000 pywxdll-0.1.1/pywxdll.egg-info/top_level.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-01 18:03:21.000000 pywxdll-0.1.1/setup.cfg
--rw-r--r--   0 henryyang   (501) staff       (20)     3776 2023-05-01 18:02:00.000000 pywxdll-0.1.1/setup.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-01 18:35:41.000000 pywxdll-0.1.11/
+-rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.11/LICENSE
+-rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.11/MANIFEST.in
+-rw-r--r--   0 henryyang   (501) staff       (20)      700 2023-05-01 18:35:41.000000 pywxdll-0.1.11/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      495 2023-05-01 18:07:43.000000 pywxdll-0.1.11/README.md
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll/
+-rw-r--r--   0 henryyang   (501) staff       (20)     7471 2023-05-01 16:30:07.000000 pywxdll-0.1.11/pywxdll/pywxdll.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     3935 2023-05-01 16:00:13.000000 pywxdll-0.1.11/pywxdll/pywxdll_json.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll.egg-info/
+-rw-r--r--   0 henryyang   (501) staff       (20)      700 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll.egg-info/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      235 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll.egg-info/SOURCES.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll.egg-info/dependency_links.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       17 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll.egg-info/requires.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-01 18:35:41.000000 pywxdll-0.1.11/pywxdll.egg-info/top_level.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-01 18:35:41.000000 pywxdll-0.1.11/setup.cfg
+-rw-r--r--   0 henryyang   (501) staff       (20)     3767 2023-05-01 18:35:33.000000 pywxdll-0.1.11/setup.py
```

### Comparing `pywxdll-0.1.1/LICENSE` & `pywxdll-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.1/PKG-INFO` & `pywxdll-0.1.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.1
+Version: 0.1.11
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.1/pywxdll.egg-info/PKG-INFO` & `pywxdll-0.1.11/pywxdll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.1
+Version: 0.1.11
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.1/setup.py` & `pywxdll-0.1.11/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywxdll'
 DESCRIPTION = 'A Python package for wechat dll hook'
 URL = 'https://github.com/HenryXiaoYang/pywxdll'
 EMAIL = 'henryyang666@hotmal.com'
 AUTHOR = 'HenryXiaoYang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.1.11'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['websocket-client']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
@@ -97,21 +97,23 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    #packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    py_modules=['pywxdll'],
-
-    entry_points={
-        'console_scripts': ['pywxdll=pywxdll:pywxdll'],
-    },
+    package_data={'pywxdll':['*.py']},
+    packages=find_packages(),
+
+    #If your package is a single module, use this instead of 'packages':
+    #py_modules=['pywxdll'],
+    #entry_points={
+    #    'console_scripts': ['pywxdll=pywxdll:Pywxdll'],
+    #},
+
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

