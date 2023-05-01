# Comparing `tmp/CVAugmentor-1.0.3.tar.gz` & `tmp/CVAugmentor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CVAugmentor-1.0.3.tar", last modified: Mon May  1 05:36:05 2023, max compression
+gzip compressed data, was "CVAugmentor-1.0.4.tar", last modified: Mon May  1 06:30:57 2023, max compression
```

## Comparing `CVAugmentor-1.0.3.tar` & `CVAugmentor-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.858437 CVAugmentor-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.807434 CVAugmentor-1.0.3/CVAugmentor/
--rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.3/CVAugmentor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.831434 CVAugmentor-1.0.3/CVAugmentor/assets/
--rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.3/CVAugmentor/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.849435 CVAugmentor-1.0.3/CVAugmentor/assets/main/
--rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/__init__.py
--rw-rw-rw-   0        0        0    26982 2023-04-29 09:27:03.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/augmentations_class.py
--rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/image_augmentor_class.py
--rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.3/CVAugmentor/assets/main/video_augmentor_class.py
-drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.855435 CVAugmentor-1.0.3/CVAugmentor/assets/utils/
--rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.3/CVAugmentor/assets/utils/__init__.py
--rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.3/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
--rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.3/CVAugmentor/assets/utils/file_type_checker_class.py
--rw-rw-rw-   0        0        0     6857 2023-05-01 05:32:36.000000 CVAugmentor-1.0.3/CVAugmentor/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-01 05:36:05.830434 CVAugmentor-1.0.3/CVAugmentor.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 05:36:05.000000 CVAugmentor-1.0.3/CVAugmentor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.3/LICENCE
--rw-rw-rw-   0        0        0     3318 2023-05-01 05:36:05.856436 CVAugmentor-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2763 2023-05-01 05:35:35.000000 CVAugmentor-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 05:36:05.858437 CVAugmentor-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-05-01 05:33:30.000000 CVAugmentor-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.706217 CVAugmentor-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.607214 CVAugmentor-1.0.4/CVAugmentor/
+-rw-rw-rw-   0        0        0      498 2023-04-30 08:40:00.000000 CVAugmentor-1.0.4/CVAugmentor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.670215 CVAugmentor-1.0.4/CVAugmentor/assets/
+-rw-rw-rw-   0        0        0      317 2023-04-29 05:52:52.000000 CVAugmentor-1.0.4/CVAugmentor/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.695216 CVAugmentor-1.0.4/CVAugmentor/assets/main/
+-rw-rw-rw-   0        0        0      178 2023-04-29 05:52:49.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/__init__.py
+-rw-rw-rw-   0        0        0    26921 2023-05-01 06:27:34.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/augmentations_class.py
+-rw-rw-rw-   0        0        0     3519 2023-04-27 08:22:59.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/image_augmentor_class.py
+-rw-rw-rw-   0        0        0     6805 2023-04-27 08:38:31.000000 CVAugmentor-1.0.4/CVAugmentor/assets/main/video_augmentor_class.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.703217 CVAugmentor-1.0.4/CVAugmentor/assets/utils/
+-rw-rw-rw-   0        0        0      143 2023-04-29 05:59:11.000000 CVAugmentor-1.0.4/CVAugmentor/assets/utils/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-03-26 09:42:33.000000 CVAugmentor-1.0.4/CVAugmentor/assets/utils/alphanumeric_sorter_class.py
+-rw-rw-rw-   0        0        0     1210 2023-04-27 07:28:18.000000 CVAugmentor-1.0.4/CVAugmentor/assets/utils/file_type_checker_class.py
+-rw-rw-rw-   0        0        0     6857 2023-05-01 05:32:36.000000 CVAugmentor-1.0.4/CVAugmentor/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:30:57.667214 CVAugmentor-1.0.4/CVAugmentor.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 06:30:57.000000 CVAugmentor-1.0.4/CVAugmentor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-29 06:37:13.000000 CVAugmentor-1.0.4/LICENCE
+-rw-rw-rw-   0        0        0     3318 2023-05-01 06:30:57.705215 CVAugmentor-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2763 2023-05-01 06:10:14.000000 CVAugmentor-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 06:30:57.706217 CVAugmentor-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-05-01 06:28:07.000000 CVAugmentor-1.0.4/setup.py
```

### Comparing `CVAugmentor-1.0.3/CVAugmentor/assets/main/augmentations_class.py` & `CVAugmentor-1.0.4/CVAugmentor/assets/main/augmentations_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             hue,
             saturation,
             brightness,
             exposure,
             blur,
             noise,
             cutout,
-            negative,
+            negative.
     
     """
     
     # Defining the constructor
     def __init__(self) -> None:
         
         """
@@ -51,71 +51,71 @@
         pass
 
 
     # Defining the no_augmentation method
     @staticmethod
     def no_augmentation() -> Callable[[Image.Image], Image.Image]:
             
-            """
-    
-            No augmentation. 
-            This can be used when you want to copy the image to the output folder without augmenting it.
-    
-    
-            Parameters
-            ----------
-            image : Image.Image
-                Image to be augmented.
-    
-    
-            Returns
-            -------
-            image : Image.Image
-                Augmented image.
-    
-            """
-    
-            # Defining the wrapper function
-            def no_augmentation_wrapper(image: Image.Image) -> Image.Image:
-    
-                # Return the image
-                return image
-    
-    
-            # Return the wrapper function
-            return no_augmentation_wrapper
+        """
+
+        No augmentation. 
+        This can be used when you want to copy the image to the output folder without augmenting it.
+
+
+        Parameters
+        ----------
+        None.
+
+
+        Returns
+        -------
+        no_augmentation_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
+
+        """
+
+        # Defining the wrapper function
+        def no_augmentation_wrapper(image: Image.Image) -> Image.Image:
+
+            # Return the image
+            return image
+
+
+        # Return the wrapper function
+        return no_augmentation_wrapper
     
 
     # Defining the flip method
     @staticmethod
     def flip(flip_type: Optional[str] = "vertical") -> Callable[[Image.Image], Image.Image]:
 
         """
 
         Flip the image horizontally or vertically.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be flipped.
-
         flip_type : str, optional
             Type of flip. The default is "vertical".
                 The options are:
                     "horizontal"
                         Flip the image horizontally
                     "vertical"
                         Flip the image vertically
 
 
         Returns
         -------
-        img_flipped : Image.Image
-            Flipped image.
+        flip_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def flip_wrapper(image: Image.Image) -> Image.Image:
 
             # Check if the flip_type is valid
@@ -151,25 +151,24 @@
         """
 
         Zoom the image.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be zoomed.
-
         zoom_size : tuple, optional
             Size of the zoom. The default is None. If None, a random zoom size is generated.
 
 
         Returns
         -------
-        img_zoomed : Image.Image
-            Zoomed image.
+        zoom_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the position variables in order to prevent inconsistent zooming
         x, y = None, None
 
 
@@ -228,33 +227,32 @@
         """
 
         Rotate the image by a definite angle or a random angle.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be rotated.
-
         rotate_type : str, optional
             Type of rotation. The default is "definite".
                 The options are:
                     "definite"
                         Rotate the image by a definite angle
                     "random"
                         Rotate the image by a random angle
                         
         angle : int or float, optional if rotate_type is "random"
             Angle of rotation. The default is 90.
         
             
         Returns
         -------
-        img_rotated : Image.Image
-            Rotated image.
+        rotate_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def rotate_wrapper(image: Image.Image) -> Image.Image:
 
             # Check if the rotate_type is valid
@@ -293,25 +291,24 @@
         """
 
         Shear the image. The shearing means that the image is slanted along the x-axis and/or y-axis.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be sheared.
-
         shear : tuple, optional
             Shear values. The default is None. If None, a random shear value is generated.
         
             
         Returns
         -------
-        img_sheared : Image.Image
-            Sheared image.
+        shear_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def shear_wrapper(image: Image.Image) -> Image.Image:
 
             # If shear is None, generate a random shear value
@@ -358,22 +355,23 @@
         Convert the image to grayscale. The grayscale conversion is done using the formula:
             gray_value = 0.2989 * r + 0.5870 * g + 0.1140 * b
         Note that the grayscale conversion is keeping the image in RGB format in order to be consistent with the other methods.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
+        None.
             
+        
         Returns
         -------
-        img_grayed : Image.Image
-            Grayscaled image.
+        grayscale_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def grayscale_wrapper(image: Image.Image) -> Image.Image:
 
             # Get the width and height of the image
@@ -413,25 +411,24 @@
         """
 
         Shift the hue of the image. Hue is the color of the image.
         
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
         hue_shift : int or float, optional
             Hue shift value. The default is None. If None, a random hue shift value is generated.
 
             
         Returns
         -------
-        img_hued : Image.Image
-            Hue shifted image.
+        hue_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def hue_wrapper(image: Image.Image) -> Image.Image:
 
             # If hue_shift is None, generate a random hue shift value
@@ -481,25 +478,24 @@
         """
 
         Adjust the saturation of the image. The stauration means the intensity of the colors.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
         saturation_factor : int or float, optional
             Saturation factor. The default is None. If None, a random saturation factor is generated.
 
 
         Returns
         -------
-        img_saturated : Image.Image
-            Saturation adjusted image.
+        saturation_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def saturation_wrapper(image: Image.Image) -> Image.Image:
 
             # If saturation_factor is None, generate a random saturation factor
@@ -533,25 +529,24 @@
         """
 
         Adjust the brightness of the image.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
         brightness_factor : int or float, optional
             Brightness factor. The default is None. If None, a random brightness factor is generated.
 
 
         Returns
         -------
-        img_brightened : Image.Image
-            Brightness adjusted image.
+        brightness_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def brightness_wrapper(image: Image.Image) -> Image.Image:
 
             # If brightness_factor is None, generate a random brightness factor
@@ -585,25 +580,24 @@
         """
 
         Adjust the exposure of the image. The exposure means the amount of light that reaches the image sensor.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
         exposure_factor : int or float, optional
             Exposure factor. The default is None. If None, a random exposure factor is generated.
 
 
         Returns
         -------
-        img_exposed : Image.Image
-            Exposure adjusted image.
+        exposure_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
         
         # Defining the wrapper function
         def exposure_wrapper(image: Image.Image) -> Image.Image:
 
             # If exposure_factor is None, generate a random exposure factor
@@ -650,25 +644,24 @@
         """
 
         Blur the image. The blur radius is the standard deviation of the Gaussian blur.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
         radius : int or float, optional
             Blur radius. The default is None. If None, a random blur radius is generated.
 
 
         Returns
         -------
-        img_blurred : Image.Image
-            Blurred image.
+        blur_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def blur_wrapper(image: Image.Image) -> Image.Image:
 
             # If radius is None, generate a random radius
@@ -711,25 +704,24 @@
 
         Add noise to the image. This method adds noise to the image by multiplying the pixel values by a random number between -1 and 1.
         It creates a noisy image that looks like the output from an analog TV with bad reception.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-        
         intensity : int or float, optional
             Noise intensity. The default is None. If None, a random noise intensity is generated.
 
 
         Returns
         -------
-        noisy_img : Image.Image
-            Noisy image.
+        noise_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the noise array in order to prevent inconsistent noise patterns
         noise = None
 
 
@@ -783,28 +775,27 @@
         """
 
         Cutout a random part of the image. This method cuts out a random part of the image and replaces it with a black rectangle.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to grayscale.
-
         max_size : int or float, optional
             Maximum size of the cutout. The default is None. If None, a random maximum size is generated.
 
         max_count : int, optional
             Maximum number of cutouts. The default is None. If None, a random maximum count is generated.
 
 
         Returns
         -------
-        img_cutout : Image.Image
-            Cutout image.
+        cutout_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def cutout_wrapper(image: Image.Image) -> Image.Image:
 
             # Get the width and height of the image
@@ -865,22 +856,23 @@
         """
 
         Convert the image to negative. This method converts the image to negative by inverting each pixel's RGB value.
 
 
         Parameters
         ----------
-        image : Image.Image
-            Image to be converted to negative.
+        None.
 
         
         Returns
         -------
-        img_negative : Image.Image
-            Negative image.
+        negative_wrapper : function
+            Args:
+                image : Image.Image
+                    The image to be augmented.
 
         """
 
         # Defining the wrapper function
         def negative_wrapper(image: Image.Image) -> Image.Image:
 
             # Load the image
```

### Comparing `CVAugmentor-1.0.3/CVAugmentor/assets/main/image_augmentor_class.py` & `CVAugmentor-1.0.4/CVAugmentor/assets/main/image_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/CVAugmentor/assets/main/video_augmentor_class.py` & `CVAugmentor-1.0.4/CVAugmentor/assets/main/video_augmentor_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/CVAugmentor/assets/utils/alphanumeric_sorter_class.py` & `CVAugmentor-1.0.4/CVAugmentor/assets/utils/alphanumeric_sorter_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/CVAugmentor/assets/utils/file_type_checker_class.py` & `CVAugmentor-1.0.4/CVAugmentor/assets/utils/file_type_checker_class.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/CVAugmentor/pipeline.py` & `CVAugmentor-1.0.4/CVAugmentor/pipeline.py`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/CVAugmentor.egg-info/PKG-INFO` & `CVAugmentor-1.0.4/CVAugmentor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
     hue,
     saturation,
     brightness,
     exposure,
     blur,
     noise,
     cutout,
-    negative,
+    negative.
 ## Installation
 You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
 For a detailed usage guide, please refer to the [documentation](https://alikhalilit.github.io/CVAugmentor/).
```

### Comparing `CVAugmentor-1.0.3/CVAugmentor.egg-info/SOURCES.txt` & `CVAugmentor-1.0.4/CVAugmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/LICENCE` & `CVAugmentor-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `CVAugmentor-1.0.3/PKG-INFO` & `CVAugmentor-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CVAugmentor
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for augmenting images and videos for computer vision tasks
 Home-page: https://github.com/AliKHaliliT/CVAugmentor
 Author: Ali Khalili Tazehkandgheshlagh
 Author-email: ali.khalili.t98@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
     hue,
     saturation,
     brightness,
     exposure,
     blur,
     noise,
     cutout,
-    negative,
+    negative.
 ## Installation
 You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
 For a detailed usage guide, please refer to the [documentation](https://alikhalilit.github.io/CVAugmentor/).
```

### Comparing `CVAugmentor-1.0.3/README.md` & `CVAugmentor-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     hue,
     saturation,
     brightness,
     exposure,
     blur,
     noise,
     cutout,
-    negative,
+    negative.
 ## Installation
 You can install the package using pip:
 ```bash
 pip install CVAugmentor
 ```
 ## Usage
 For a detailed usage guide, please refer to the [documentation](https://alikhalilit.github.io/CVAugmentor/).
```

### Comparing `CVAugmentor-1.0.3/setup.py` & `CVAugmentor-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
     
 
 # Defining the setup function
 setup(name='CVAugmentor',
-        version='1.0.3',
+        version='1.0.4',
         description='A package for augmenting images and videos for computer vision tasks',
         long_description=readme(),
         long_description_content_type='text/markdown',
         url='https://github.com/AliKHaliliT/CVAugmentor',
         author='Ali Khalili Tazehkandgheshlagh',
         author_email='ali.khalili.t98@gmail.com',
         license='MIT',
```

