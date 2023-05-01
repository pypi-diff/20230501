# Comparing `tmp/CVAugmentor-1.0.5.tar.gz` & `tmp/CVAugmentor-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-1.0.5.tar", last modified: Mon May  1 06:48:35 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.6.tar", last modified: Mon May  1 07:08:30 2023, max compression
```

## Comparing `CVAugmentor-1.0.5.tar` & `CVAugmentor-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.815702 CVAugmentor-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.773697 CVAugmentor-1.0.5/CVAugmentor/
--rw-rw-rw-   0        0        0      498 2023-05-01 06:48:25.000000 CVAugmentor-1.0.5/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.799695 CVAugmentor-1.0.5/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.5/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.806702 CVAugmentor-1.0.5/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26921 2023-05-01 06:45:51.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.5/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.812691 CVAugmentor-1.0.5/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.5/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.5/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.5/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     6857 2023-05-01 06:45:51.000000 CVAugmentor-1.0.5/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:48:35.797691 CVAugmentor-1.0.5/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 06:48:35.000000 CVAugmentor-1.0.5/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.5/LICENCE
--rw-rw-rw-   0        0        0     3318 2023-05-01 06:48:35.814697 CVAugmentor-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2763 2023-05-01 06:48:15.000000 CVAugmentor-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 06:48:35.816698 CVAugmentor-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-05-01 06:48:29.000000 CVAugmentor-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:08:30.980811 CVAugmentor-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:08:30.932807 CVAugmentor-1.0.6/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-05-01 07:07:29.000000 CVAugmentor-1.0.6/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:08:30.961811 CVAugmentor-1.0.6/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.6/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:08:30.970826 CVAugmentor-1.0.6/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.6/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26921 2023-05-01 06:45:51.000000 CVAugmentor-1.0.6/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.6/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.6/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:08:30.976817 CVAugmentor-1.0.6/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.6/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.6/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.6/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     7026 2023-05-01 07:07:25.000000 CVAugmentor-1.0.6/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:08:30.959810 CVAugmentor-1.0.6/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-01 07:08:30.000000 CVAugmentor-1.0.6/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-05-01 07:08:30.000000 CVAugmentor-1.0.6/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:08:30.000000 CVAugmentor-1.0.6/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-01 07:08:30.000000 CVAugmentor-1.0.6/CVAugmentor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 07:08:30.000000 CVAugmentor-1.0.6/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.6/LICENCE
+-rw-rw-rw-   0        0        0     3318 2023-05-01 07:08:30.979806 CVAugmentor-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2763 2023-05-01 07:07:19.000000 CVAugmentor-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:08:30.980811 CVAugmentor-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-05-01 07:07:33.000000 CVAugmentor-1.0.6/setup.py
```

### Comparing `CVAugmentor-1.0.5/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.6/CVAugmentor/assets/main/augmentations_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.6/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.6/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.6/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.6/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.6/CVAugmentor/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Importing the libraries
 from .assets.utils.alphanumeric_sorter_class import AlphanumericSorter
 from .assets.utils.file_type_checker_class import FileTypeChecker
 from .assets.main.video_augmentor_class import VideoAugmentor
 from .assets.main.image_augmentor_class import ImageAugmentor
 from typing import Dict, Callable, Optional
 import os
+from tqdm import tqdm
 
 
 # Defining the Pipeline class
 class Pipeline(AlphanumericSorter, FileTypeChecker):
 
     # Defining the constructor
     def __init__(self) -> None:
@@ -31,15 +32,15 @@
         """
 
         pass
 
 
     # Defining the augment method
     def augment(self, input_path: str, output_path: str, target: str, process_type: str, mode: str,
-                augmentations: Dict[str, Callable], verbose: Optional[bool] = False, warn_verbose: Optional[bool] = False) -> None:
+                augmentations: Dict[str, Callable], verbose: Optional[bool] = False, aug_verbose: Optional[False] = False, warn_verbose: Optional[bool] = False) -> None:
         
         """
         
         Augments the input data.
 
 
         Parameters
@@ -129,15 +130,15 @@
         else:
             raise ValueError(f"Invalid target type: {target}")
         
         # Augmentation
         if process_type == "batch":
             
             # Looping through the input files
-            for input_file in self.sorted_alphanumeric(os.listdir(input_path)):
+            for input_file in tqdm(self.sorted_alphanumeric(os.listdir(input_path)), desc='Overall Progress', unit=' Videos', leave=False, dynamic_ncols=True, diable=not verbose):
                 
                 # Checking if the input file is valid
                 if not self.is_target_type(input_file, target):
 
                     if warn_verbose:
                         print(f"Skipping invalid input file: {input_file}")
 
@@ -147,17 +148,17 @@
                 input_file_path = os.path.join(input_path, input_file)
 
                 # Defining the output file path
                 output_file_path = os.path.join(output_path, input_file)
 
                 # Augmenting the input file
                 if mode == "sequential":
-                    augmentor.augment_one_by_one(input_file_path, output_file_path, augmentations, verbose)
+                    augmentor.augment_one_by_one(input_file_path, output_file_path, augmentations, aug_verbose)
                 elif mode == "singular":
-                    augmentor.augment_all_at_once(input_file_path, output_file_path, augmentations, verbose)
+                    augmentor.augment_all_at_once(input_file_path, output_file_path, augmentations, aug_verbose)
 
         elif process_type == "single":
                 
                 # Checking if the input file is valid
                 if not self.is_target_type(input_path, target):
                     raise ValueError(f"Invalid input file. Expected {target} file, got {os.path.splitext(input_path)[1]} instead.")
```

### Comparing `CVAugmentor-1.0.5/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.6/CVAugmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CVAugmentor-1.0.5/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.6/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/LICENCE` & `CVAugmentor-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/PKG-INFO` & `CVAugmentor-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CVAugmentor-1.0.5/README.md` & `CVAugmentor-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.5/setup.py` & `CVAugmentor-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='1.0.5',
+        version='1.0.6',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

