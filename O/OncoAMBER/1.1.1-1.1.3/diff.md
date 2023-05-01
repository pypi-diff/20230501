# Comparing `tmp/OncoAMBER-1.1.1.tar.gz` & `tmp/OncoAMBER-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.1.1.tar", last modified: Thu Apr 27 16:58:20 2023, max compression
+gzip compressed data, was "OncoAMBER-1.1.3.tar", last modified: Mon May  1 16:41:24 2023, max compression
```

## Comparing `OncoAMBER-1.1.1.tar` & `OncoAMBER-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-27 16:58:20.909339 OncoAMBER-1.1.1/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-27 16:58:20.889481 OncoAMBER-1.1.1/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      554 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-04-27 16:58:20.909034 OncoAMBER-1.1.1/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-27 16:58:20.907870 OncoAMBER-1.1.1/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5291 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/CONFIG_default.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    21348 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.1.1/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      719 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/RunTopas.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14247 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5487 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    21482 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      332 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-27 16:58:20.909422 OncoAMBER-1.1.1/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3009 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-01 16:41:24.273994 OncoAMBER-1.1.3/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-01 16:41:24.218954 OncoAMBER-1.1.3/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      613 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-01 16:41:24.273658 OncoAMBER-1.1.3/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.1.3/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-01 16:41:24.272187 OncoAMBER-1.1.3/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.1.3/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5291 2023-04-27 16:58:04.000000 OncoAMBER-1.1.3/amber/CONFIG_default.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    21348 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.1.3/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14247 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5487 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    21621 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-01 16:41:24.274087 OncoAMBER-1.1.3/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3009 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/setup.py
```

### Comparing `OncoAMBER-1.1.1/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.1.3/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.1.1
+Version: 1.1.3
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.1.1/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.1.3/OncoAMBER.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 OncoAMBER.egg-info/top_level.txt
 amber/BasicGeometries.py
 amber/BetaDistributionCalibration.py
 amber/CONFIG_default.txt
 amber/Cell.py
 amber/Process.py
 amber/ReadAndWrite.py
-amber/RunTopas.py
 amber/ScalarField.py
 amber/Terminal.py
 amber/Vessel.py
 amber/Voxel.py
 amber/World.py
 amber/__init__.py
+amber/cell.py
 amber/config.py
+amber/process.py
 amber/save_alpha_dataframe6.csv
-amber/save_beta_dataframe6.csv
+amber/save_beta_dataframe6.csv
+amber/vessel.py
+amber/voxel.py
+amber/world.py
```

### Comparing `OncoAMBER-1.1.1/PKG-INFO` & `OncoAMBER-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.1.1
+Version: 1.1.3
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.1.1/README.md` & `OncoAMBER-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/BasicGeometries.py` & `OncoAMBER-1.1.3/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.1.3/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/CONFIG_default.txt` & `OncoAMBER-1.1.3/amber/CONFIG_default.txt`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/Cell.py` & `OncoAMBER-1.1.3/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/Process.py` & `OncoAMBER-1.1.3/amber/Process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from amber.World import *
-from amber.Voxel import *
+from amber.world import *
+from amber.voxel import *
 from amber.ScalarField import *
 import amber.Terminal as term
 import amber.ReadAndWrite as rw
 import pandas as pd
 from matplotlib.colors import TwoSlopeNorm
 import matplotlib.pyplot as plt
 import os
```

### Comparing `OncoAMBER-1.1.1/amber/ReadAndWrite.py` & `OncoAMBER-1.1.3/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/ScalarField.py` & `OncoAMBER-1.1.3/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/Terminal.py` & `OncoAMBER-1.1.3/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/Vessel.py` & `OncoAMBER-1.1.3/amber/Vessel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/Voxel.py` & `OncoAMBER-1.1.3/amber/Voxel.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/World.py` & `OncoAMBER-1.1.3/amber/World.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from amber.Voxel import *
-from amber.Vessel import *
+from amber.voxel import *
+from amber.vessel import *
 from amber.ScalarField import *
 from amber.BasicGeometries import *
 #np.set_printoptions(threshold=sys.maxsize)
 # from scipy.stats import qmc
 import matplotlib.tri as mtri
 import scipy.sparse as sparse
 
 class World:
-    def __init__(self, config , half_length, number_of_voxels : int = 20):
-        self.half_length = half_length
+    def __init__(self, config):
+        print('Initializing world')
+        print(config.voxel_per_side, config.half_length_world)
+        self.half_length = config.half_length_world
         self.voxel_list = []
-        self.total_number_of_voxels = number_of_voxels ** 3
+        self.number_of_voxels = config.voxel_per_side
+        self.total_number_of_voxels = self.number_of_voxels ** 3
         self.config = config
-        voxel_length = 2 * half_length / number_of_voxels
+        voxel_length = 2 * self.half_length / self.number_of_voxels
 
-        for i in range(number_of_voxels):
-            for j in range(number_of_voxels):
-                for k in range(number_of_voxels):
+        for i in range(self.number_of_voxels):
+            for j in range(self.number_of_voxels):
+                for k in range(self.number_of_voxels):
                     position = np.array([
-                        i * voxel_length - half_length + voxel_length / 2,
-                        j * voxel_length - half_length + voxel_length / 2,
-                        k * voxel_length - half_length + voxel_length / 2
+                        i * voxel_length - self.half_length + voxel_length / 2,
+                        j * voxel_length - self.half_length + voxel_length / 2,
+                        k * voxel_length - self.half_length + voxel_length / 2
                     ])
-                    self.voxel_list.append(Voxel(position, half_length / number_of_voxels, voxel_number=i * number_of_voxels ** 2 + j * number_of_voxels + k))
-        self.number_of_voxels = number_of_voxels
+                    self.voxel_list.append(Voxel(position, self.half_length / self.number_of_voxels, voxel_number=i * self.number_of_voxels ** 2 + j * self.number_of_voxels + k))
         self.vasculature = VasculatureNetwork(self.config)
 
     def initiate_vasculature(self, list_of_mother_vessels):
         self.vasculature = VasculatureNetwork(self.config, list_of_mother_vessels)
         return
 
     def vasculature_growth(self, dt, splitting_rate, macro_steps=1, micro_steps=10, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5, radius_pressure_sensitive = False):
```

### Comparing `OncoAMBER-1.1.1/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.1.3/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.1.3/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.1/setup.py` & `OncoAMBER-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.1.1'
+VERSION = '1.1.3'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
```

