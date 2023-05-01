# Comparing `tmp/hilltop-py-2.2.0.tar.gz` & `tmp/hilltop-py-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilltop-py-2.2.0.tar", last modified: Fri Aug 12 16:59:31 2022, max compression
+gzip compressed data, was "hilltop-py-2.2.1.tar", last modified: Mon May  1 05:23:47 2023, max compression
```

## Comparing `hilltop-py-2.2.0.tar` & `hilltop-py-2.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-08-12 16:59:31.449823 hilltop-py-2.2.0/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/LICENSE.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       98 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/MANIFEST.in
--rw-rw-r--   0 mike      (1000) mike      (1000)      723 2022-08-12 16:59:31.449823 hilltop-py-2.2.0/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      313 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-08-12 16:59:31.449823 hilltop-py-2.2.0/hilltop_py.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      723 2022-08-12 16:59:31.000000 hilltop-py-2.2.0/hilltop_py.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      443 2022-08-12 16:59:31.000000 hilltop-py-2.2.0/hilltop_py.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2022-08-12 16:59:31.000000 hilltop-py-2.2.0/hilltop_py.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       32 2022-08-12 16:59:31.000000 hilltop-py-2.2.0/hilltop_py.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       10 2022-08-12 16:59:31.000000 hilltop-py-2.2.0/hilltop_py.egg-info/top_level.txt
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-08-12 16:59:31.449823 hilltop-py-2.2.0/hilltoppy/
--rw-rw-r--   0 mike      (1000) mike      (1000)       89 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/hilltoppy/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    16356 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/hilltoppy/com.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6068 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/hilltoppy/hilltop.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    22966 2022-08-12 16:52:58.000000 hilltop-py-2.2.0/hilltoppy/mountain_top.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2022-08-12 16:59:31.449823 hilltop-py-2.2.0/hilltoppy/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/hilltoppy/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3772 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/hilltoppy/tests/test_mountain_top.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2536 2022-08-12 16:16:41.000000 hilltop-py-2.2.0/hilltoppy/tests/test_web_service.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12887 2022-08-12 16:17:02.000000 hilltop-py-2.2.0/hilltoppy/utils.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    19092 2022-08-12 16:55:16.000000 hilltop-py-2.2.0/hilltoppy/web_service.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2022-08-12 16:59:31.449823 hilltop-py-2.2.0/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     6692 2022-08-12 16:57:36.000000 hilltop-py-2.2.0/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-01 05:23:47.264131 hilltop-py-2.2.1/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2022-06-21 04:38:45.000000 hilltop-py-2.2.1/LICENSE.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       98 2022-06-21 04:38:45.000000 hilltop-py-2.2.1/MANIFEST.in
+-rw-rw-r--   0 mike      (1000) mike      (1000)      723 2023-05-01 05:23:47.264131 hilltop-py-2.2.1/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      313 2022-07-21 04:10:55.000000 hilltop-py-2.2.1/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-01 05:23:47.264131 hilltop-py-2.2.1/hilltop_py.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      723 2023-05-01 05:23:47.000000 hilltop-py-2.2.1/hilltop_py.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      443 2023-05-01 05:23:47.000000 hilltop-py-2.2.1/hilltop_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-01 05:23:47.000000 hilltop-py-2.2.1/hilltop_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       32 2023-05-01 05:23:47.000000 hilltop-py-2.2.1/hilltop_py.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       10 2023-05-01 05:23:47.000000 hilltop-py-2.2.1/hilltop_py.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-01 05:23:47.264131 hilltop-py-2.2.1/hilltoppy/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       89 2022-07-27 08:09:38.000000 hilltop-py-2.2.1/hilltoppy/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16356 2022-06-24 04:13:17.000000 hilltop-py-2.2.1/hilltoppy/com.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6068 2022-06-24 04:13:25.000000 hilltop-py-2.2.1/hilltoppy/hilltop.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    23102 2023-05-01 05:21:08.000000 hilltop-py-2.2.1/hilltoppy/mountain_top.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-01 05:23:47.264131 hilltop-py-2.2.1/hilltoppy/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2022-06-21 04:38:45.000000 hilltop-py-2.2.1/hilltoppy/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3772 2022-07-27 09:04:19.000000 hilltop-py-2.2.1/hilltoppy/tests/test_mountain_top.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2536 2022-07-27 09:00:18.000000 hilltop-py-2.2.1/hilltoppy/tests/test_web_service.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12887 2022-07-27 22:44:28.000000 hilltop-py-2.2.1/hilltoppy/utils.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    19092 2022-11-06 03:15:36.000000 hilltop-py-2.2.1/hilltoppy/web_service.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2023-05-01 05:23:47.264131 hilltop-py-2.2.1/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6692 2023-05-01 05:22:53.000000 hilltop-py-2.2.1/setup.py
```

### Comparing `hilltop-py-2.2.0/LICENSE.txt` & `hilltop-py-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/PKG-INFO` & `hilltop-py-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilltop-py
-Version: 2.2.0
+Version: 2.2.1
 Summary: Functions to access Hilltop data
 Home-page: https://github.com/mullenkamp/hilltop-py
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: hilltop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hilltop-py-2.2.0/hilltop_py.egg-info/PKG-INFO` & `hilltop-py-2.2.1/hilltop_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilltop-py
-Version: 2.2.0
+Version: 2.2.1
 Summary: Functions to access Hilltop data
 Home-page: https://github.com/mullenkamp/hilltop-py
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: hilltop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hilltop-py-2.2.0/hilltoppy/com.py` & `hilltop-py-2.2.1/hilltoppy/com.py`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/hilltoppy/hilltop.py` & `hilltop-py-2.2.1/hilltoppy/hilltop.py`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/hilltoppy/mountain_top.py` & `hilltop-py-2.2.1/hilltoppy/mountain_top.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,15 +450,20 @@
                 for val in data1:
                     val_text = val.text.encode('ascii', 'ignore').decode()
                     mowsecs = int(val_text.split(' ')[0])
                     time = convert_mowsecs(mowsecs)
 
                     val_dict = {'Time': time}
 
-                    v1 = int(val_text.split(' ')[item_num])
+                    v1 = val_text.split(' ')[item_num]
+
+                    try:
+                        v1 = int(v1)
+                    except ValueError:
+                        v1 = float(v1)
 
                     if v1 >= 0:
                         if 'Divisor' in m_dict1:
                             v1 = v1 / m_dict1['Divisor']
 
                         val_dict['Value'] = v1
```

### Comparing `hilltop-py-2.2.0/hilltoppy/tests/test_mountain_top.py` & `hilltop-py-2.2.1/hilltoppy/tests/test_mountain_top.py`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/hilltoppy/tests/test_web_service.py` & `hilltop-py-2.2.1/hilltoppy/tests/test_web_service.py`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/hilltoppy/utils.py` & `hilltop-py-2.2.1/hilltoppy/utils.py`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/hilltoppy/web_service.py` & `hilltop-py-2.2.1/hilltoppy/web_service.py`

 * *Files identical despite different names*

### Comparing `hilltop-py-2.2.0/setup.py` & `hilltop-py-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'hilltop-py'
 main_package = 'hilltoppy'
 # datasets = 'datasets'
-version = '2.2.0'
+version = '2.2.1'
 descrip = 'Functions to access Hilltop data'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

