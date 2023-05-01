# Comparing `tmp/CVAugmentor-1.0.4.tar.gz` & `tmp/CVAugmentor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-1.0.4.tar", last modified: Mon May  1 06:30:57 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.5.tar", last modified: Mon May  1 06:48:35 2023, max compression
```

## Comparing `CVAugmentor-1.0.4.tar` & `CVAugmentor-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.706217 CVAugmentor-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.607214 CVAugmentor-1.0.4/CVAugmentor/
--rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.4/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.670215 CVAugmentor-1.0.4/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.4/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.695216 CVAugmentor-1.0.4/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26921 2023-05-01 06:27:34.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.703217 CVAugmentor-1.0.4/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.4/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.4/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.4/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     6857 2023-05-01 05:32:36.000000 CVAugmentor-1.0.4/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.667214 CVAugmentor-1.0.4/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.4/LICENCE
--rw-rw-rw-   0        0        0     3318 2023-05-01 06:30:57.705215 CVAugmentor-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2763 2023-05-01 06:10:14.000000 CVAugmentor-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 06:30:57.706217 CVAugmentor-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-05-01 06:28:07.000000 CVAugmentor-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.815702 CVAugmentor-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.773697 CVAugmentor-1.0.5/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-05-01 06:48:25.000000 CVAugmentor-1.0.5/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.799695 CVAugmentor-1.0.5/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.5/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.806702 CVAugmentor-1.0.5/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26921 2023-05-01 06:45:51.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.812691 CVAugmentor-1.0.5/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.5/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.5/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.5/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     6857 2023-05-01 06:45:51.000000 CVAugmentor-1.0.5/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.797691 CVAugmentor-1.0.5/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.5/LICENCE
+-rw-rw-rw-   0        0        0     3318 2023-05-01 06:48:35.814697 CVAugmentor-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2763 2023-05-01 06:48:15.000000 CVAugmentor-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 06:48:35.816698 CVAugmentor-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-05-01 06:48:29.000000 CVAugmentor-1.0.5/setup.py
```

### Comparing `CVAugmentor-1.0.4/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.5/CVAugmentor/assets/main/augmentations_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.5/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.5/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.5/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.5/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.5/CVAugmentor/pipeline.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.5/CVAugmentor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CVAugmentor-1.0.4/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.5/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/LICENCE` & `CVAugmentor-1.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/PKG-INFO` & `CVAugmentor-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CVAugmentor-1.0.4/README.md` & `CVAugmentor-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.4/setup.py` & `CVAugmentor-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='1.0.4',
+        version='1.0.5',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

