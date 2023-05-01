# Comparing `tmp/geode-ml-2.6.3.tar.gz` & `tmp/geode-ml-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geode-ml-2.6.3.tar", last modified: Tue Apr  4 17:43:29 2023, max compression
+gzip compressed data, was "geode-ml-2.6.4.tar", last modified: Mon May  1 17:48:11 2023, max compression
```

## Comparing `geode-ml-2.6.3.tar` & `geode-ml-2.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 17:43:29.421275 geode-ml-2.6.3/
--rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.3/LICENSE
--rw-rw-rw-   0        0        0     3804 2023-04-04 17:43:29.419274 geode-ml-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 17:43:29.394276 geode-ml-2.6.3/geode/
--rw-rw-rw-   0        0        0       74 2023-04-04 17:43:04.000000 geode-ml-2.6.3/geode/__init__.py
--rw-rw-rw-   0        0        0    21562 2023-04-04 17:38:31.000000 geode-ml-2.6.3/geode/datasets.py
--rw-rw-rw-   0        0        0     2679 2023-03-29 15:32:57.000000 geode-ml-2.6.3/geode/losses.py
--rw-rw-rw-   0        0        0     5491 2023-03-29 15:50:12.000000 geode-ml-2.6.3/geode/metrics.py
--rw-rw-rw-   0        0        0    18087 2023-03-29 15:28:46.000000 geode-ml-2.6.3/geode/models.py
--rw-rw-rw-   0        0        0    17932 2023-04-03 18:02:01.000000 geode-ml-2.6.3/geode/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-04 17:43:29.416275 geode-ml-2.6.3/geode_ml.egg-info/
--rw-rw-rw-   0        0        0     3804 2023-04-04 17:43:29.000000 geode-ml-2.6.3/geode_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-04-04 17:43:29.000000 geode-ml-2.6.3/geode_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 17:43:29.000000 geode-ml-2.6.3/geode_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-04 17:43:29.000000 geode-ml-2.6.3/geode_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-04 17:43:29.000000 geode-ml-2.6.3/geode_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      961 2023-04-04 17:43:04.000000 geode-ml-2.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 17:43:29.421275 geode-ml-2.6.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 17:48:11.483026 geode-ml-2.6.4/
+-rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.4/LICENSE
+-rw-rw-rw-   0        0        0     3804 2023-05-01 17:48:11.479018 geode-ml-2.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 17:48:11.422986 geode-ml-2.6.4/geode/
+-rw-rw-rw-   0        0        0       74 2023-05-01 17:46:58.000000 geode-ml-2.6.4/geode/__init__.py
+-rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.4/geode/datasets.py
+-rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.4/geode/losses.py
+-rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.4/geode/metrics.py
+-rw-rw-rw-   0        0        0    21871 2023-04-11 13:49:32.000000 geode-ml-2.6.4/geode/models.py
+-rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.4/geode/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-01 17:48:11.472019 geode-ml-2.6.4/geode_ml.egg-info/
+-rw-rw-rw-   0        0        0     3804 2023-05-01 17:48:11.000000 geode-ml-2.6.4/geode_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-01 17:48:11.000000 geode-ml-2.6.4/geode_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 17:48:11.000000 geode-ml-2.6.4/geode_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-01 17:48:11.000000 geode-ml-2.6.4/geode_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 17:48:11.000000 geode-ml-2.6.4/geode_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      961 2023-05-01 17:46:52.000000 geode-ml-2.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 17:48:11.483987 geode-ml-2.6.4/setup.cfg
```

### Comparing `geode-ml-2.6.3/LICENSE` & `geode-ml-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.3/PKG-INFO` & `geode-ml-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.3
+Version: 2.6.4
 Summary: Classes and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.3/README.md` & `geode-ml-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.3/geode/datasets.py` & `geode-ml-2.6.4/geode/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,30 @@
 from os import listdir, mkdir
 from os.path import isdir, join, splitext
 from osgeo import gdal, ogr
 import tensorflow as tf
 
 
 class SegmentationDataset:
-    """A class for defining and manipulating semantic segmentation datasets.
-
-    Attributes:
-        source_path: the directory containing source imagery;
-        polygons_path: the directory containing subdirectories of polygon shapefiles;
-        labels_path: the directory to contain label rasters;
-        tiles_path: the directory to contain the imagery/labels subdirectory pairs for tiles;
-        n_channels: the number of channels in the source_imagery;
-        tile_dimension: the length/width of tiles;
-        source_image_names: the filenames of source imagery;
-        data_names: the source imagery names without filename extensions;
-    """
 
     def __init__(self, source_path: str = '',
                  polygons_path: str = '',
                  labels_path: str = '',
                  tiles_path: str = '',
                  n_channels: int = 3,
                  tile_dimension: int = 0):
-        """
-        Args:
-            source_path: the directory containing the source imagery;
-            polygons_path: the directory containing polygons;
-            labels_path: the directory containing the label rasters;
-            n_channels: the number of channels in the source imagery;
+
+        """A class for defining and manipulating semantic segmentation datasets.
+
+        Attributes:
+            source_path: the directory containing source imagery;
+            polygons_path: the directory containing subdirectories of polygon shapefiles;
+            labels_path: the directory to contain label rasters;
+            tiles_path: the directory to contain the imagery/labels subdirectory pairs for tiles;
+            n_channels: the number of channels in the source_imagery;
             tile_dimension: the length/width of tiles;
 
         Raises:
             ValueError: if source_path is the empty string;
             Exception: if the source_path is empty;
             ValueError: if n_channels is negative;
             ValueError: if tile_dimension is negative.
@@ -63,14 +54,15 @@
         if self.n_channels <= 0:
             raise ValueError("The argument n_channels must be a positive integer.")
 
         if self.tile_dimension <= 0:
             raise ValueError("The argument tile_dimension must be a postiive integer.")
 
     def check_polygons(self) -> None:
+
         """Checks whether the polygon data has been set, and matches the names of the source imagery.
 
         Returns:
             None
 
         Raises:
             ValueError: if polygons_path has not been set;
@@ -89,14 +81,15 @@
             for directory in listdir(self.polygons_path):
                 filenames = listdir(join(self.polygons_path, directory))
                 shapefiles = [x for x in filenames if splitext(x)[1] == '.shp']
                 if len(shapefiles) != 1:
                     raise Exception("The polygons data directories must have exactly one shapefile.")
 
     def check_labels(self) -> None:
+
         """Checks whether the label rasters have been generated, and match the names of the source imagery.
 
         Returns:
             None
 
         Raises:
             ValueError: if labels_path has not been set;
@@ -124,14 +117,15 @@
                 # check other metadata to see if it matches
                 if source_dataset.RasterXSize != label_dataset.RasterXSize:
                     raise Exception("Raster x-dimensions do not match for " + filename + " pair.")
                 elif source_dataset.RasterYSize != label_dataset.RasterYSize:
                     raise Exception("Raster y-dimensions do not match for " + filename + " pair.")
 
     def check_tiles(self) -> None:
+
         """Checks whether the tiles have been correctly generated.
 
         Returns:
             None
 
         Raises:
             ValueError: if tiles_path has not been specified;
@@ -173,14 +167,15 @@
             pass
         else:
             raise Exception("The imagery and label tiles do not have the same filenames.")
 
     def generate_tiles(self, stride_length: int = 0,
                        label_proportion: float = 0.2,
                        verbose: bool = True) -> None:
+
         """Generates image tiles from the source and label imagery for use in model training.
 
         Args:
             stride_length: the number of pixels of overlap between tiles;
             label_proportion: the minimum proportion which any single class must have per tile;
             verbose: whether to print progress to the console.
 
@@ -236,14 +231,15 @@
                              label_tiles_dir=label_tiles_dir,
                              filename=filename)
 
             if verbose:
                 print(filename + " tiles generated.")
 
     def get_tile_quantities(self) -> dict:
+
         """Computes the number of tiles generated from each source image.
 
         Returns:
             A dictionary containing the number of tiles for each source image."""
 
         # check that the tiles have been generated properly
         self.check_tiles()
@@ -260,14 +256,15 @@
             quantity_dict[fname] = len(tile_subset)
 
         return quantity_dict
 
     def rasterize_polygon_layers(self, burn_feature: str = 'bool',
                                  no_data_value: int = 0,
                                  verbose: bool = True) -> None:
+
         """Generates label rasters from the polygon data, with dimensions matching the source imagery.
 
         Args:
             burn_feature: the feature from the attribute table to write;
             no_data_value: the value to burn into NoData pixels;
             verbose: whether to print progress to the console.
 
@@ -311,14 +308,15 @@
                 print(filename + " rasterized.")
 
     def resample_source_imagery(self, output_path: str,
                                 target_resolutions: tuple,
                                 resample_algorithm: str = 'cubic',
                                 replace_source_dataset: bool = True,
                                 verbose: bool = True) -> None:
+
         """Resamples the source imagery to the target resolution.
 
         Args:
             output_path: the directory to hold the resampled imagery;
             target_resolutions: a tuple of the form (xRes, yRes) for target resolutions, in units of meters;
             resample_algorithm: the method used for resampling (see gdalwarp documentation for more options);
             replace_source_dataset: whether to use the resampled imagery as the new source imagery;
@@ -359,14 +357,15 @@
                 print(filename + " resampled to " + str(target_resolutions) + ".")
 
         # change dataset's source imagery if requested
         if replace_source_dataset:
             self.source_path = output_path
 
     def set_label_imagery(self, labels_path: str) -> None:
+
         """Defines the label imagery to use for other methods, if not already created by rasterize_polygons.
 
         Args:
             labels_path: the directory containing the label rasters.
 
         Returns:
             None
@@ -375,14 +374,15 @@
         # attempt to coerce argument to the correct type
         labels_path = str(labels_path)
 
         self.labels_path = labels_path
         self.check_labels()
 
     def set_label_polygons(self, polygons_path: str) -> None:
+
         """Defines the polygon data, and provides a manual alternative to the get_label_polygons method; e.g., this
         method is useful when one wants to use polygon data from a source other than OpenStreetMaps.
 
         Args:
             polygons_path: the directory containing the polygon data (one sub-directory for each source image).
 
         Returns:
```

### Comparing `geode-ml-2.6.3/geode/losses.py` & `geode-ml-2.6.4/geode/losses.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # losses.py
 
-from numpy import ndarray
+from numpy import asarray, ndarray
 import tensorflow as tf
 from tensorflow.keras import backend as K
 
 
 def dice_loss(y_true: ndarray,
               y_pred: ndarray,
               smooth: float = 100.) -> float:
     """Computes the dice-loss between one-hot encoded arrays, then returns a score between [0, 1].
 
     Args:
-        y_true: tensor of ground-truth values of size (batch, height, width, n_classes;
+        y_true: tensor of ground-truth values of size (batch, height, width, n_classes);
         y_pred: tensor of model predictions of size (batch, height, width, n_classes);
         smooth: a value to avoid division by zero (among other things).
 
     Returns:
         The dice-loss score.
+
+    Raises:
+        ValueError: if smooth is less than zero.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    smooth = float(smooth)
+
+    # check for the correct float range
+    if smooth < 0:
+        raise ValueError("Argument smooth must be greater than or equal to zero.")
+
     y_true = K.cast(y_true, dtype=tf.float32)
     y_pred = K.cast(y_pred, dtype=tf.float32)
 
     y_true_f = K.flatten(y_true)
     y_pred_f = K.flatten(y_pred)
     intersection = K.sum(y_true_f * y_pred_f)
 
@@ -39,16 +51,28 @@
     Args:
         y_true: tensor of ground-truth values of size (batch, height, width);
         y_pred: tensor of model predictions of size (batch, height, width);
         smooth: a value to avoid division by zero (among other things).
 
     Returns:
         The iou-loss score.
+
+    Raises:
+        ValueError: if smooth is less than zero.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    smooth = float(smooth)
+
+    # check for the correct float range
+    if smooth < 0:
+        raise ValueError("Argument smooth must be greater than or equal to zero.")
+
     y_true = K.cast(y_true, dtype=tf.float32)
     y_pred = K.cast(y_pred, dtype=tf.float32)
 
     intersection = K.sum(K.flatten(y_true * y_pred))
     union = K.sum(K.flatten(y_true + y_pred - y_true * y_pred)) + smooth
 
     iou = intersection / union
@@ -65,16 +89,28 @@
     Args:
         y_true: tensor of ground-truth values of size (batch, height, width);
         y_pred: tensor of model predictions of size (batch, height, width);
         smooth: a value to avoid division by zero (among other things).
 
     Returns:
         The log-iou-loss score.
+
+    Raises:
+        ValueError: if smooth is less than zero.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    smooth = float(smooth)
+
+    # check for the correct float range
+    if smooth < 0:
+        raise ValueError("Argument smooth must be greater than or equal to zero.")
+
     y_true = K.cast(y_true, dtype=tf.float32)
     y_pred = K.cast(y_pred, dtype=tf.float32)
 
     intersection = K.sum(K.flatten(y_true * y_pred)) + smooth
     union = K.sum(K.flatten(y_true + y_pred - y_true * y_pred)) + smooth
 
     final = - K.log(intersection / union)
```

### Comparing `geode-ml-2.6.3/geode/metrics.py` & `geode-ml-2.6.4/geode/metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,214 @@
 # metrics.py
 
 import numpy as np
-from numpy import ndarray
+from numpy import asarray, ndarray
 
 
 def convert_and_flatten(y_true: ndarray,
                         y_pred: ndarray,
                         pos_label: int) -> tuple:
+
     """Converts input arrays to binary labels, and flattens them.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         A tuple containing the converted and flattened arrays.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     y_true = np.where(y_true.flatten() == pos_label, 1, 0)
     y_pred = np.where(y_pred.flatten() == pos_label, 1, 0)
 
     return y_true, y_pred
 
 
 def true_positives(y_true: ndarray,
                    y_pred: ndarray,
                    pos_label: int) -> int:
+
     """Computes the true positives between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The number of true positives between the arrays.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     y_true, y_pred = convert_and_flatten(y_true, y_pred, pos_label)
 
     return int(np.sum(y_true * y_pred))
 
 
 def false_positives(y_true: ndarray,
                     y_pred: ndarray,
                     pos_label: int) -> int:
+
     """Computes the false positives between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The number of false positives between the arrays.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     y_true, y_pred = convert_and_flatten(y_true, y_pred, pos_label)
 
     return int(np.sum(np.where(y_pred - y_true == 1, 1, 0)))
 
 
 def false_negatives(y_true: ndarray,
                     y_pred: ndarray,
                     pos_label: int) -> int:
+
     """Computes the false negatives between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The number of false negatives between the arrays.
     """
+
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     y_true, y_pred = convert_and_flatten(y_true, y_pred, pos_label)
 
     return int(np.sum(np.where(y_true - y_pred == 1, 1, 0)))
 
 
 def f1(y_true: ndarray,
        y_pred: ndarray,
        pos_label: int) -> float:
+
     """Computes the F1 (aka, dice) score between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The F1 score.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     tp = true_positives(y_true, y_pred, pos_label)
     fp = false_positives(y_true, y_pred, pos_label)
     fn = false_negatives(y_true, y_pred, pos_label)
 
     return tp / (tp + 0.5 * (fp + fn))
 
 
 def jaccard(y_true: ndarray,
             y_pred: ndarray,
             pos_label: int) -> float:
+
     """Computes the Jaccard (aka, intersection-over-union) score between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The Jaccard score.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     tp = true_positives(y_true, y_pred, pos_label)
     fp = false_positives(y_true, y_pred, pos_label)
     fn = false_negatives(y_true, y_pred, pos_label)
 
     return tp / (tp + fp + fn)
 
 
 def precision(y_true: ndarray,
               y_pred: ndarray,
               pos_label: int) -> float:
+
     """Computes the precision score between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The precision score.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     tp = true_positives(y_true, y_pred, pos_label)
     fp = false_positives(y_true, y_pred, pos_label)
 
     return tp / (tp + fp)
 
 
 def recall(y_true: ndarray,
            y_pred: ndarray,
            pos_label: int) -> float:
+
     """Computes the recall score between the ground-truth and predicted array.
 
     Args:
         y_true: an array of true labels;
         y_pred: an array of predicted labels;
         pos_label: the label in y_true and y_pred to change to 1.
 
     Returns:
         The recall score.
     """
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+    pos_label = int(pos_label)
+
     tp = true_positives(y_true, y_pred, pos_label)
     fn = false_negatives(y_true, y_pred, pos_label)
 
     return tp / (tp + fn)
 
 
 def total_accuracy(y_true: ndarray,
@@ -173,17 +222,19 @@
 
     Returns:
         The proportion of correctly predicted labels.
 
     Raises:
         Exception: if the two provided arrays do not have the same shape."""
 
+    # coerce arguments to the correct type
+    y_true = asarray(y_true)
+    y_pred = asarray(y_pred)
+
     # check whether the two arrays have the same shape
-    if y_true.shape == y_pred.shape:
-        pass
-    else:
+    if y_true.shape != y_pred.shape:
         raise Exception("The provided arrays do not have the same shape.")
 
     # compute accuracy
     acc = np.sum(np.where(y_true == y_pred, 1, 0)) / np.prod(y_true.shape)
 
     return acc
```

### Comparing `geode-ml-2.6.3/geode/models.py` & `geode-ml-2.6.4/geode/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,145 +1,173 @@
 # models.py
 
 from geode.metrics import f1, jaccard, total_accuracy
 from geode.utilities import predict_raster
-from numpy import unique
+from numpy import mean, unique
 from os import listdir, makedirs
 from os.path import isdir, join
 from osgeo.gdal import Open
 import tensorflow as tf
 from tensorflow.keras.layers import Add, BatchNormalization, Concatenate, Conv2D, Dropout, Input, MaxPooling2D, \
     UpSampling2D
 from tensorflow.keras.layers.experimental.preprocessing import Rescaling
 
 
 class SegmentationModel:
+    """A class for defining and testing semantic segmentation models.
 
-    def __init__(self):
-
+    Attributes:
+        test_imagery_path: the directory containing the test imagery;
+        test_labels_path: the directory containing the true labels;
+        test_predictions_path: the directory containing the predicted labels;
+        data_names: a list of imagery names (usually regions before tiling was applied);
+        test_metrics: the dictionary which stores computed metrics;
+        test_imagery_names: the files which make up the test imagery set;
+        model: the model object."""
+
+    def __init__(self, test_imagery_path: str = None,
+                 test_labels_path: str = None,
+                 test_predictions_path: str = None,
+                 data_names: list = None):
+
+        self.test_imagery_path = str(test_imagery_path)
+        self.test_labels_path = str(test_labels_path)
+        self.test_predictions_path = str(test_predictions_path)
+        self.data_names = str(data_names)
         self.test_metrics = {}
-        self.test_filenames = []
         self.model = None
 
-    def compute_metrics(self, test_labels_path: str = None,
-                        test_predictions_path: str = None,
-                        output_path: str = None) -> dict:
+        if test_imagery_path is not None:
+            self.test_imagery_names = listdir(test_imagery_path)
+
+        if len(self.test_imagery_names) == 0:
+            raise Exception("No test imagery has been supplied.")
+
+        if test_labels_path is not None:
+            self.test_labels_name = listdir(test_labels_path)
+
+        if len(self.test_imagery_names) != len(self.test_imagery_names):
+            raise Exception("There are a different number of test imagery and label files.")
+
+        if set(self.test_imagery_names) != set(self.test_labels_name):
+            raise Exception("Test imagery and label file names do not match.")
+
+    def compute_metrics(self, output_path: str = None) -> dict:
 
         """Computes various metrics on a test dataset; paired images and labels should have identical filenames.
 
         Args:
-            test_labels_path: the location of test labels;
-            test_predictions_path: the location at which to save model predictions;
             output_path: the path to write a text-file of metrics.
 
         Returns:
              A dictionary containing various calculated metrics for each test raster.
 
         Raises:
-            Exception: if there are no predicted rasters at test_predictions_path.
+            Exception: if there are no predicted rasters at test_predictions_path;
         """
 
+        # coerce arguments to correct type
+        output_path = str(output_path)
+
         # check that there are predictions
-        if len(listdir(test_predictions_path)) == 0:
+        if len(listdir(self.test_predictions_path)) == 0:
             raise Exception("No predicted imagery has been generated.")
 
         # create dictionary to hold metric dictionaries
-        fname_metrics = {}
+        dname_metrics = {}
+
+        # get the test_filenames:
+        filenames = listdir(self.test_labels_path)
 
         # loop through the test imagery
-        for fname in self.test_filenames:
+        for dname in self.data_names:
+            # get the relevant subset
+            sub_filenames = [x for x in filenames if dname in x]
+
             # create metrics dictionary
             metrics_dict = {}
 
-            # open the relevant datasets
-            y_true = Open(join(test_labels_path, fname)).ReadAsArray()
-            y_pred = Open(join(test_predictions_path, fname)).ReadAsArray()
-
-            # get the label values
-            labels = unique(y_true)
-
-            # compute total accuracy
-            metrics_dict['total_accuracy'] = total_accuracy(y_true, y_pred)
-
-            # compute F1 and Jaccard scores for each label
+            # create lists for each metric
+            acc_scores = []
             f1_scores = []
             jaccard_scores = []
-            for label in labels:
-                f1_scores.append(f1(y_true=y_true,
-                                    y_pred=y_pred,
-                                    pos_label=label))
-
-                jaccard_scores.append(jaccard(y_true=y_true,
-                                              y_pred=y_pred,
-                                              pos_label=label))
+
+            # loop through the test subset
+            for fname in sub_filenames:
+                # open the relevant datasets
+                y_true = Open(join(self.test_labels_path, fname)).ReadAsArray()
+                y_pred = Open(join(self.test_predictions_path, fname)).ReadAsArray()
+
+                # get the label values
+                labels = unique(y_true)
+
+                # compute total accuracy
+                acc_scores.append(total_accuracy(y_true, y_pred))
+
+                # compute F1 and Jaccard scores for each label
+                for label in labels:
+                    f1_scores.append(f1(y_true=y_true,
+                                        y_pred=y_pred,
+                                        pos_label=label))
+
+                    jaccard_scores.append(jaccard(y_true=y_true,
+                                                  y_pred=y_pred,
+                                                  pos_label=label))
 
             # add F1 and Jaccard scores to the metrics dictionary
-            metrics_dict['F1'] = f1_scores
-            metrics_dict['Jaccard'] = jaccard_scores
+            metrics_dict['Acc'] = mean(acc_scores)
+            metrics_dict['F1'] = mean(f1_scores)
+            metrics_dict['Jaccard'] = mean(jaccard_scores)
 
-            fname_metrics[fname] = metrics_dict
+            dname_metrics[dname] = metrics_dict
 
         # write the dictionary to a file
         if output_path is not None:
             with open(output_path, 'w') as f:
-                for key, value in fname_metrics.items():
+                for key, value in dname_metrics.items():
                     f.write('%s: %s' % (key, value))
 
-        self.test_metrics = fname_metrics
+        self.test_metrics = dname_metrics
+
+        return dname_metrics
 
-        return fname_metrics
+    def predict_test_imagery(self, verbose: bool = True) -> None:
 
-    def predict_test_imagery(self, test_imagery_path: str = None,
-                             test_labels_path: str = None,
-                             test_predictions_path: str = None,
-                             verbose=True) -> None:
         """Predicts the test imagery in the supplied path.
 
         Args:
-            test_imagery_path: the location of input test imagery;
-            test_labels_path: the location of test labels;
-            test_predictions_path: the location at which to save model predictions;
             verbose: whether to print an update for each file when inference is completed.
 
         Returns:
             None
 
         Raises:
-            Exception: if any of the input paths are None;
-            Exception: if no test files exist at the supplied paths.
+            TypeError: if verbose is not boolean;
         """
 
-        # check that input paths are supplied
-        if test_imagery_path is None or test_labels_path is None or test_predictions_path is None:
-            raise Exception("One of the required path arguments has not been supplied.")
-
-        # check that test imagery exists and has correctly named labels
-        if set(listdir(test_imagery_path)) == set(listdir(test_labels_path)):
-            self.test_filenames = listdir(test_imagery_path)
-            if len(self.test_filenames) == 0:
-                raise Exception("There is no test imagery.")
-        else:
-            raise Exception("The test imagery and labels must have identical filenames.")
+        # check for the correct type
+        if not isinstance(verbose, bool):
+            raise TypeError("Argument verbose must be boolean.")
 
         # get filenames
-        filenames = listdir(test_imagery_path)
+        filenames = listdir(self.test_imagery_path)
 
         # create directory for predicted rasters
-        if isdir(test_predictions_path):
+        if isdir(self.test_predictions_path):
             pass
         else:
-            makedirs(test_predictions_path)
+            makedirs(self.test_predictions_path)
 
         # loop through the files in test_imagery_path
         for fname in filenames:
-            rgb = Open(join(test_imagery_path, fname))
+            rgb = Open(join(self.test_imagery_path, fname))
 
             predict_raster(input_dataset=rgb,
                            model=self.model,
-                           output_path=join(test_predictions_path, fname))
+                           output_path=join(self.test_predictions_path, fname))
 
             # close the input dataset
             rgb = None
 
             # print status if required
             if verbose:
                 print("Prediction finished for", fname + ".")
@@ -150,26 +178,50 @@
     def __init__(self, n_channels: int = 3,
                  n_classes: int = 2,
                  n_filters: int = 16,
                  dropout_rate: float = 0.3,
                  rescale_factor: float = 1 / 255,
                  include_residual: bool = False):
 
+        """Instantiates the Unet architecture, with mirrored VGG19 architectures for the up- and down-sampling paths.
+
+        Attributes:
+            n_channels: the number of channels in the input imagery;
+            n_classes: the number of classes to predict;
+            n_filters: the number of convolutional filters in the first layer;
+            dropout_rate: the proportion of nodes to turn off for each inference step during training.
+
+        Raises:
+            ValueError: if n_channels is less than 1;
+            ValueError: if n_classes is less than 2;
+            ValueError: if n_filters is less than 1;
+            ValueError: if dropout_rate is not between 0.0 and 1.0;
+            TypeError:  if include_residual is not boolean.
+        """
+
         # initialize the superclass
         super().__init__()
 
-        # define attributes
-        self.n_channels = n_channels
-        self.n_classes = n_classes
-        self.n_filters = n_filters
-        self.dropout_rate = dropout_rate
-
-        # ensure that n_classes >= 2
+        # coerce arguments to correct types and define attributes
+        self.n_channels = int(n_channels)
+        self.n_classes = int(n_classes)
+        self.n_filters = int(n_filters)
+        self.dropout_rate = float(dropout_rate)
+
+        # perform type-checking
+        if self.n_channels < 1:
+            raise ValueError("The argument n_channels must be greater than or equal to one.")
         if self.n_classes < 2:
-            raise Exception("Number of classes must at least 2.")
+            raise ValueError("The argument n_classes must be greater than or equal to 2.")
+        if self.n_filters < 1:
+            raise ValueError("The argument n_filters must be at least 1.")
+        if self.dropout_rate < 0.0 or self.dropout_rate > 1.0:
+            raise ValueError("The argument dropout_rate must be between 0.0 and 1.0, inclusive.")
+        if not isinstance(include_residual, bool):
+            raise TypeError("The argument include_residual must be boolean.")
 
         # define the layers and model
         include_dropout = (self.dropout_rate > 0.0)
 
         def conv_block(input_tensor,
                        filters):
 
@@ -293,40 +345,67 @@
             loss: the loss function to use during training;
             learning_rate: the starting learning rate for the Adam optimizer.
 
         Returns:
             None
         """
 
+        # coerce arguments to correct type
+        learning_rate = float(learning_rate)
+
         # compile the model
         self.model.compile(loss=loss,
                            optimizer=tf.keras.optimizers.Adam(learning_rate=learning_rate))
 
 
 class Unet(SegmentationModel):
 
     def __init__(self, n_channels: int = 3,
                  n_classes: int = 2,
                  n_filters: int = 16,
                  dropout_rate: float = 0.3,
                  rescale_factor: float = 1 / 255,
                  include_residual: bool = False):
 
+        """Instantiates the Unet architecture, with filters doubling in each level.
+
+        Attributes:
+            n_channels: the number of channels in the input imagery;
+            n_classes: the number of classes to predict;
+            n_filters: the number of convolutional filters in the first layer;
+            dropout_rate: the proportion of nodes to turn off for each inference step during training.
+
+        Raises:
+            ValueError: if n_channels is less than 1;
+            ValueError: if n_classes is less than 2;
+            ValueError: if n_filters is less than 1;
+            ValueError: if dropout_rate is not between 0.0 and 1.0;
+            TypeError:  if include_residual is not boolean.
+        """
+
         # initialize the superclass
         super().__init__()
 
-        # define attributes
-        self.n_channels = n_channels
-        self.n_classes = n_classes
-        self.n_filters = n_filters
-        self.dropout_rate = dropout_rate
-
-        # ensure that n_classes >= 2
+        # coerce arguments to correct types and define attributes
+        self.n_channels = int(n_channels)
+        self.n_classes = int(n_classes)
+        self.n_filters = int(n_filters)
+        self.dropout_rate = float(dropout_rate)
+
+        # perform type-checking
+        if self.n_channels < 1:
+            raise ValueError("The argument n_channels must be greater than or equal to one.")
         if self.n_classes < 2:
-            raise Exception("Number of classes must at least 2.")
+            raise ValueError("The argument n_classes must be greater than or equal to 2.")
+        if self.n_filters < 1:
+            raise ValueError("The argument n_filters must be at least 1.")
+        if self.dropout_rate < 0.0 or self.dropout_rate > 1.0:
+            raise ValueError("The argument dropout_rate must be between 0.0 and 1.0, inclusive.")
+        if not isinstance(include_residual, bool):
+            raise TypeError("The argument include_residual must be boolean.")
 
         include_dropout = (self.dropout_rate > 0.0)
 
         def conv_block(input_tensor,
                        filters):
 
             conv = Conv2D(filters=filters,
```

### Comparing `geode-ml-2.6.3/geode/utilities.py` & `geode-ml-2.6.4/geode/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,15 @@
     output_band.SetNoDataValue(0)
     output_band.FlushCache()
 
     # without the following lines, the arrays won't actually be written into the tif file
     output_band = None
     output_dataset = None
 
+
 def rasterize_polygon_layer(rgb: Dataset,
                             polygons: DataSource,
                             output_path: str,
                             burn_attribute: str,
                             no_data_value: int = 0) -> None:
     """Converts polygon vector layers into rasters of the same size as the source RGB dataset.
```

### Comparing `geode-ml-2.6.3/geode_ml.egg-info/PKG-INFO` & `geode-ml-2.6.4/geode_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.3
+Version: 2.6.4
 Summary: Classes and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geode-ml-2.6.3/pyproject.toml` & `geode-ml-2.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'geode-ml'
-version = '2.6.3'
+version = '2.6.4'
 description = "Classes and methods to help with the creation of geospatial training datasets and deep-learning models."
 readme = 'README.md'
 license = {file='LICENSE'}
 authors = [
     {name = 'Matt Reichenbach', email='matthew.reichenbach@gmail.com'},
 ]
 requires-python = '>=3.7'
```

