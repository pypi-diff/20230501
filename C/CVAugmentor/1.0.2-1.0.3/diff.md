# Comparing `tmp/CVAugmentor-1.0.2.tar.gz` & `tmp/CVAugmentor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-1.0.2.tar", last modified: Sun Apr 30 16:57:05 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.3.tar", last modified: Mon May  1 05:36:05 2023, max compression
```

## Comparing `CVAugmentor-1.0.2.tar` & `CVAugmentor-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:57:05.137246 CVAugmentor-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-30 16:57:05.095243 CVAugmentor-1.0.2/CVAugmentor/
--rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.2/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:57:05.119245 CVAugmentor-1.0.2/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.2/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:57:05.129284 CVAugmentor-1.0.2/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.2/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26982 2023-04-29 09:27:03.000000 CVAugmentor-1.0.2/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.2/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.2/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:57:05.134261 CVAugmentor-1.0.2/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.2/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.2/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.2/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     6776 2023-04-29 08:09:44.000000 CVAugmentor-1.0.2/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:57:05.117254 CVAugmentor-1.0.2/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3286 2023-04-30 16:57:04.000000 CVAugmentor-1.0.2/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-04-30 16:57:04.000000 CVAugmentor-1.0.2/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:57:04.000000 CVAugmentor-1.0.2/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-04-30 16:57:04.000000 CVAugmentor-1.0.2/CVAugmentor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 16:57:04.000000 CVAugmentor-1.0.2/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.2/LICENCE
--rw-rw-rw-   0        0        0     3286 2023-04-30 16:57:05.136245 CVAugmentor-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2023-04-30 08:54:03.000000 CVAugmentor-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 16:57:05.138246 CVAugmentor-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-30 16:55:56.000000 CVAugmentor-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.858437 CVAugmentor-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.807434 CVAugmentor-1.0.3/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.3/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.831434 CVAugmentor-1.0.3/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.3/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.849435 CVAugmentor-1.0.3/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26982 2023-04-29 09:27:03.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.855435 CVAugmentor-1.0.3/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.3/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.3/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.3/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     6857 2023-05-01 05:32:36.000000 CVAugmentor-1.0.3/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.830434 CVAugmentor-1.0.3/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.3/LICENCE
+-rw-rw-rw-   0        0        0     3318 2023-05-01 05:36:05.856436 CVAugmentor-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2763 2023-05-01 05:35:35.000000 CVAugmentor-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 05:36:05.858437 CVAugmentor-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-05-01 05:33:30.000000 CVAugmentor-1.0.3/setup.py
```

### Comparing `CVAugmentor-1.0.2/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.3/CVAugmentor/assets/main/augmentations_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.3/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.3/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.3/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.3/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.3/CVAugmentor/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         
         """
 
         pass
 
 
     # Defining the augment method
-    def augment(self, input_path: str, output_path: str, target: str, type: str, mode: str,
+    def augment(self, input_path: str, output_path: str, target: str, process_type: str, mode: str,
                 augmentations: Dict[str, Callable], verbose: Optional[bool] = False, warn_verbose: Optional[bool] = False) -> None:
         
         """
         
         Augments the input data.
 
 
@@ -54,15 +54,15 @@
             Target of the augmentation.
                 The options are:
                     "image"
                         Specifies that the target of the augmentation is an image.
                     "video"
                         Specifies that the target of the augmentation is a video.
 
-        type : str
+        process_type : str
             Type of the augmentation.
                 The options are:
                     "batch"
                         Batch type means that the input and output paths are directories.
                     "single"
                         Single type means that the input and output paths are files.
 
@@ -90,33 +90,33 @@
         
         """
 
         # Checking if the input path is valid
         if not os.path.exists(input_path):
             raise ValueError(f"Invalid input path: {input_path}")
         
-        # Checking if the type is valid
-        if type != "batch" and type != "single":
-            raise ValueError(f"Invalid type type: {type}")
+        # Checking if the process_type is valid
+        if process_type != "batch" and process_type != "single":
+            raise ValueError(f"Invalid process type: {process_type}")
         
         # Checking if the output path is valid
-        if type == "batch" and not os.path.exists(output_path):
+        if process_type == "batch" and not os.path.exists(output_path):
             raise ValueError(f"Invalid output path: {output_path}")
 
         # Checking if the target is valid
         if target != "image" and target != "video":
             raise ValueError(f"Invalid target type: {target}")
         
         # Checking if the mode is valid
         if mode != "sequential" and mode != "singular":
             raise ValueError(f"Invalid mode type: {mode}")
         
         # Checking if the augmentations is valid
         if not isinstance(augmentations, dict):
-            raise ValueError(f"Invalid augmentations type: {type}")
+            raise ValueError(f"Invalid augmentations type: {process_type}")
         elif len(augmentations) == 0:
             raise ValueError("augmentations dict is empty.")
         
         # Checking if the verbose is valid
         if not isinstance(verbose, bool):
             raise ValueError(f"Invalid verbose type: {verbose}")
 
@@ -126,15 +126,15 @@
             augmentor = ImageAugmentor()
         elif target == "video":
             augmentor = VideoAugmentor()
         else:
             raise ValueError(f"Invalid target type: {target}")
         
         # Augmentation
-        if type == "batch":
+        if process_type == "batch":
             
             # Looping through the input files
             for input_file in self.sorted_alphanumeric(os.listdir(input_path)):
                 
                 # Checking if the input file is valid
                 if not self.is_target_type(input_file, target):
 
@@ -151,15 +151,15 @@
 
                 # Augmenting the input file
                 if mode == "sequential":
                     augmentor.augment_one_by_one(input_file_path, output_file_path, augmentations, verbose)
                 elif mode == "singular":
                     augmentor.augment_all_at_once(input_file_path, output_file_path, augmentations, verbose)
 
-        elif type == "single":
+        elif process_type == "single":
                 
                 # Checking if the input file is valid
                 if not self.is_target_type(input_path, target):
                     raise ValueError(f"Invalid input file. Expected {target} file, got {os.path.splitext(input_path)[1]} instead.")
                 
                 # Checking if the format of the input file and the output file are the same
                 if os.path.splitext(input_path)[1] != os.path.splitext(output_path)[1]:
@@ -167,8 +167,8 @@
                 elif os.path.splitext(input_path)[1] == ".gif":
                     raise ValueError(f"The GIF format is not supported.")
                 
                 # Augmenting the input file
                 if mode == "sequential":
                     augmentor.augment_one_by_one(input_path, output_path, augmentations, verbose)
                 elif mode == "singular":
-                    augmentor.augment_all_at_once(input_path, output_path, augmentations, verbose)
+                    augmentor.augment_all_at_once(input_path, output_path, augmentations, verbose)
```

### Comparing `CVAugmentor-1.0.2/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.3/CVAugmentor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -52,15 +52,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the image
-p.augment(input_path="path/to/input_image", output_path="path/to/output_image", target="image", type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_image", output_path="path/to/output_image", target="image", process_type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Single Video Augmentation
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -71,15 +71,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the video
-p.augment(input_path="path/to/input_video", output_path="path/to/output_video", target="video", type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_video", output_path="path/to/output_video", target="video", process_type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Augmenting Multiple Images
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -90,15 +90,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the images
-p.augment(input_path="path/to/input_images", output_path="path/to/output_images", target="image", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_images", output_path="path/to/output_images", target="image", process_type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Augmenting Multiple Videos
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -109,11 +109,11 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the videos
-p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", process_type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ## License
 This work is licensed under an [MIT](https://choosealicense.com/licenses/mit/) License.
```

### Comparing `CVAugmentor-1.0.2/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.3/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/LICENCE` & `CVAugmentor-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.2/PKG-INFO` & `CVAugmentor-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -52,15 +52,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the image
-p.augment(input_path="path/to/input_image", output_path="path/to/output_image", target="image", type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_image", output_path="path/to/output_image", target="image", process_type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Single Video Augmentation
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -71,15 +71,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the video
-p.augment(input_path="path/to/input_video", output_path="path/to/output_video", target="video", type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_video", output_path="path/to/output_video", target="video", process_type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Augmenting Multiple Images
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -90,15 +90,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the images
-p.augment(input_path="path/to/input_images", output_path="path/to/output_images", target="image", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_images", output_path="path/to/output_images", target="image", process_type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Augmenting Multiple Videos
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -109,11 +109,11 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the videos
-p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", process_type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ## License
 This work is licensed under an [MIT](https://choosealicense.com/licenses/mit/) License.
```

### Comparing `CVAugmentor-1.0.2/README.md` & `CVAugmentor-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the image
-p.augment(input_path="path/to/input_image", output_path="path/to/output_image", target="image", type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_image", output_path="path/to/output_image", target="image", process_type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Single Video Augmentation
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -56,15 +56,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the video
-p.augment(input_path="path/to/input_video", output_path="path/to/output_video", target="video", type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_video", output_path="path/to/output_video", target="video", process_type="single", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Augmenting Multiple Images
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -75,15 +75,15 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the images
-p.augment(input_path="path/to/input_images", output_path="path/to/output_images", target="image", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_images", output_path="path/to/output_images", target="image", process_type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ### Augmenting Multiple Videos
 ```python
 # Importing the libraries
 from CVAugmentor import Augmentations as aug
 from CVAugmentor import Pipeline
 
@@ -94,11 +94,11 @@
     "flip": aug.flip(),
 }
 
 # Create a Pipeline object
 p = Pipeline()
 
 # Augment the videos
-p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
+p.augment(input_path="path/to/input_videos", output_path="path/to/output_videos", target="video", process_type="batch", mode="singular", augmentations=augmentations, verbose=True, warn_verbose=True)
 ```
 ## License
 This work is licensed under an [MIT](https://choosealicense.com/licenses/mit/) License.
```

### Comparing `CVAugmentor-1.0.2/setup.py` & `CVAugmentor-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='1.0.2',
+        version='1.0.3',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

