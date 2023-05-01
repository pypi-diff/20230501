# Comparing `tmp/material_zui-0.0.2.tar.gz` & `tmp/material_zui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.0.2.tar", last modified: Mon May  1 13:54:01 2023, max compression
+gzip compressed data, was "material_zui-0.0.3.tar", last modified: Mon May  1 14:12:41 2023, max compression
```

## Comparing `material_zui-0.0.2.tar` & `material_zui-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.328469 material_zui-0.0.2/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      622 2023-05-01 13:54:01.328469 material_zui-0.0.2/PKG-INFO
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.324469 material_zui-0.0.2/image/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      121 2023-04-30 11:48:20.000000 material_zui-0.0.2/image/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1604 2023-04-30 11:48:06.000000 material_zui-0.0.2/image/convert.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-04-28 09:55:18.000000 material_zui-0.0.2/image/data.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1392 2023-04-30 12:03:19.000000 material_zui-0.0.2/image/index.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      801 2023-04-29 15:11:22.000000 material_zui-0.0.2/image/remove_background.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      278 2023-04-29 15:11:37.000000 material_zui-0.0.2/image/transparent_background.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      249 2023-04-28 09:24:02.000000 material_zui-0.0.2/image/type.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     3842 2023-04-30 11:48:06.000000 material_zui-0.0.2/image/upscale.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.324469 material_zui-0.0.2/log/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       37 2023-04-30 11:48:06.000000 material_zui-0.0.2/log/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      858 2023-04-28 04:39:06.000000 material_zui-0.0.2/log/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.324469 material_zui-0.0.2/material_zui.egg-info/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      622 2023-05-01 13:54:01.000000 material_zui-0.0.2/material_zui.egg-info/PKG-INFO
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      487 2023-05-01 13:54:01.000000 material_zui-0.0.2/material_zui.egg-info/SOURCES.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-01 13:54:01.000000 material_zui-0.0.2/material_zui.egg-info/dependency_links.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        8 2023-05-01 13:54:01.000000 material_zui-0.0.2/material_zui.egg-info/requires.txt
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       37 2023-05-01 13:54:01.000000 material_zui-0.0.2/material_zui.egg-info/top_level.txt
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.324469 material_zui-0.0.2/replicate/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       43 2023-04-30 11:47:27.000000 material_zui-0.0.2/replicate/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1884 2023-04-30 14:10:18.000000 material_zui-0.0.2/replicate/index.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-01 13:54:01.328469 material_zui-0.0.2/setup.cfg
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      864 2023-05-01 13:52:08.000000 material_zui-0.0.2/setup.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.324469 material_zui-0.0.2/telegram_bot/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 15:00:34.000000 material_zui-0.0.2/telegram_bot/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-30 15:00:34.000000 material_zui-0.0.2/telegram_bot/index.py
-drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 13:54:01.328469 material_zui-0.0.2/tmp/
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 11:48:06.000000 material_zui-0.0.2/tmp/__init__.py
--rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-28 03:39:00.000000 material_zui-0.0.2/tmp/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.934539 material_zui-0.0.3/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      622 2023-05-01 14:12:41.934539 material_zui-0.0.3/PKG-INFO
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/image/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      121 2023-04-30 11:48:20.000000 material_zui-0.0.3/image/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1604 2023-04-30 11:48:06.000000 material_zui-0.0.3/image/convert.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       78 2023-04-28 09:55:18.000000 material_zui-0.0.3/image/data.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1392 2023-04-30 12:03:19.000000 material_zui-0.0.3/image/index.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      801 2023-04-29 15:11:22.000000 material_zui-0.0.3/image/remove_background.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      278 2023-04-29 15:11:37.000000 material_zui-0.0.3/image/transparent_background.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      249 2023-04-28 09:24:02.000000 material_zui-0.0.3/image/type.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     3842 2023-04-30 11:48:06.000000 material_zui-0.0.3/image/upscale.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/log/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       37 2023-04-30 11:48:06.000000 material_zui-0.0.3/log/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      858 2023-04-28 04:39:06.000000 material_zui-0.0.3/log/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/material_zui.egg-info/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      622 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/PKG-INFO
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      557 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/SOURCES.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        1 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/dependency_links.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        8 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/requires.txt
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       51 2023-05-01 14:12:41.000000 material_zui-0.0.3/material_zui.egg-info/top_level.txt
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/replicate/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       43 2023-04-30 11:47:27.000000 material_zui-0.0.3/replicate/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)     1884 2023-04-30 14:10:18.000000 material_zui-0.0.3/replicate/index.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       38 2023-05-01 14:12:41.934539 material_zui-0.0.3/setup.cfg
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)      864 2023-05-01 14:11:46.000000 material_zui-0.0.3/setup.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/telegram_bot/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 15:00:34.000000 material_zui-0.0.3/telegram_bot/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-30 15:00:34.000000 material_zui-0.0.3/telegram_bot/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/text/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-01 14:11:27.000000 material_zui-0.0.3/text/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:11:27.000000 material_zui-0.0.3/text/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.930539 material_zui-0.0.3/tmp/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-04-30 11:48:06.000000 material_zui-0.0.3/tmp/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-04-28 03:39:00.000000 material_zui-0.0.3/tmp/index.py
+drwxrwxr-x   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:12:41.934539 material_zui-0.0.3/validate/
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)       36 2023-05-01 14:11:23.000000 material_zui-0.0.3/validate/__init__.py
+-rw-rw-r--   0 chaunguyen  (1001) chaunguyen  (1001)        0 2023-05-01 14:11:23.000000 material_zui-0.0.3/validate/index.py
```

### Comparing `material_zui-0.0.2/PKG-INFO` & `material_zui-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: material_zui
-Version: 0.0.2
+Version: 0.0.3
 Summary: Zui Material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `material_zui-0.0.2/image/convert.py` & `material_zui-0.0.3/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.2/image/index.py` & `material_zui-0.0.3/image/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.2/image/remove_background.py` & `material_zui-0.0.3/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.2/image/upscale.py` & `material_zui-0.0.3/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.2/log/index.py` & `material_zui-0.0.3/log/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.2/material_zui.egg-info/PKG-INFO` & `material_zui-0.0.3/material_zui.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.0.2
+Version: 0.0.3
 Summary: Zui Material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `material_zui-0.0.2/replicate/index.py` & `material_zui-0.0.3/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.2/setup.py` & `material_zui-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("readme.md", "r") as fh:
     # with open("src/material_zui/readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='material_zui',
-    version='0.0.2',
+    version='0.0.3',
     # url='https://github.com/username/my_module',
     author='chauhmnguyen',
     author_email='chauhoangminhnguyen@gmail.com',
     description='Zui Material',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
```

