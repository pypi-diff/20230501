# Comparing `tmp/voxelmap-4.0.0.tar.gz` & `tmp/voxelmap-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-4.0.0.tar", max compression
+gzip compressed data, was "voxelmap-4.1.0.tar", max compression
```

## Comparing `voxelmap-4.0.0.tar` & `voxelmap-4.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.0.0/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.0.0/README.md
--rw-r--r--   0        0        0      565 2023-04-30 22:23:22.071732 voxelmap-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.0.0/voxelmap/__init__.py
--rw-r--r--   0        0        0    21552 2023-04-30 22:12:36.911725 voxelmap-4.0.0/voxelmap/annex.py
--rwxr-xr-x   0        0        0    28050 2023-04-30 22:22:33.171997 voxelmap-4.0.0/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 voxelmap-4.0.0/setup.py
--rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 voxelmap-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.1.0/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.1.0/README.md
+-rw-r--r--   0        0        0      565 2023-05-01 00:23:26.839090 voxelmap-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.1.0/voxelmap/__init__.py
+-rw-r--r--   0        0        0    21985 2023-04-30 23:03:40.856964 voxelmap-4.1.0/voxelmap/annex.py
+-rwxr-xr-x   0        0        0    28849 2023-05-01 00:22:13.552180 voxelmap-4.1.0/voxelmap/jotunn.py
+-rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 voxelmap-4.1.0/setup.py
+-rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 voxelmap-4.1.0/PKG-INFO
```

### Comparing `voxelmap-4.0.0/LICENSE` & `voxelmap-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-4.0.0/README.md` & `voxelmap-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-4.0.0/pyproject.toml` & `voxelmap-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "4.0.0"
+version = "4.1.0"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `voxelmap-4.0.0/voxelmap/annex.py` & `voxelmap-4.1.0/voxelmap/annex.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 from skimage import measure
 from skimage.draw import ellipsoid
 from scipy import ndimage 
-import pyvista as pv
+import pyvista
 
 import pandas
 
 def findcrossover(array,low,high,value):
     'finds crossover index of array for `value` value'
     if array[high] <= value:
         return high
@@ -450,37 +450,49 @@
 
         # plt.tight_layout()
         # plt.show()
 
         MeshView(out_file)
 
 
-def MeshView(objfile='model.obj',wireframe=False,color='pink',alpha=0.5,background_color='#333333', viewport = [1024, 768]):
+def MeshView(objfile='model.obj',color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
     """
     Triangulated mesh view with PyVista (GLOBAL)
     
     Parameters
     ----------
     objfile: string
         .obj file to process with MeshView [in GLOBAL function only]
-    wireframe: bool
-        Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
     color : string / hexadecimal
         mesh color. default: 'pink'
     alpha : float
         opacity transparency range: 0 - 1.0. Default: 0.5
+    wireframe: bool
+        Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
+    wireframe_color: string / hex 
+        edges or wireframe colors
     background_color : string / hexadecimal
         color of background. default: 'pink'
     viewport : (int,int)
         viewport / screen (width, height) for display window (default: 80% your screen's width & height)
     """
-    mesh = pv.read(objfile)
-    mesh.plot(show_edges=True if wireframe else False, color=color,opacity=alpha,background=background_color,window_size = viewport)
+    # Define a custom theme for the 3D plot
+    my_theme = pyvista.themes.DefaultTheme()
+    my_theme.color = color
+    my_theme.lighting = True
+    my_theme.show_edges = True if wireframe else False
+    my_theme.edge_color = wireframe_color
+    my_theme.background = background_color
+
 
-def objdraw(array,filename='voxelmodel.obj',wireframe=False,color='pink',alpha=0.5,background_color='#333333', viewport = [1024, 768]):
+    mesh = pyvista.read(objfile)
+    mesh.plot(theme=my_theme,opacity=alpha,window_size = viewport)
+    
+
+def objdraw(array,filename='voxelmodel.obj',color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
     """
     Creates a 3-D voxel model (.obj file) from the provided, third-order (3-D) `array`. It then uses the global method MeshView to draw the .obj file and display it on screen 
     
     Parameters
     ----------
     array : np.array(int)
             array of the third-order populated with discrete, non-zero integers which may represent a voxel block type
@@ -495,18 +507,17 @@
     alpha : float
         opacity transparency range: 0 - 1.0. Default: 0.5
     background_color : string / hexadecimal
         color of background. default: 'pink'
     viewport : (int,int)
         viewport / screen (width, height) for display window (default: 80% your screen's width & height)
     """
-
     voxelwrite(array, filename = filename)
-    MeshView(objfile=filename,wireframe=wireframe,color=color,alpha=alpha,background_color=background_color, viewport = viewport)
-
+    # MeshView(objfile=filename,wireframe=wireframe,color=color,alpha=alpha,background_color=background_color, viewport = viewport)
+    MeshView(filename,color,alpha,wireframe,wireframe_color,background_color, viewport )
 
 def xyz_to_sparse_array(df,hashblocks,spacing=1):
     """
     Converts a pandas DataFrame df with columns 'x', 'y', 'z', and 'rgb' to a sparse 3D array.
 
     The function returns the array and a dictionary `hashblocks` that maps voxel colors to their corresponding index values in the array.
```

### Comparing `voxelmap-4.0.0/voxelmap/jotunn.py` & `voxelmap-4.1.0/voxelmap/jotunn.py`

 * *Files 6% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
         voxels = Model(self.array).build()
 
         ax.voxels(voxels, facecolors=voxcolors, edgecolors=edgecolors)
         set_axes_equal(ax)
         plt.show()
 
-    def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, window_size=[1024, 768],voxel_spacing=(1,1,1)):
+    def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, wireframe_color='k', window_size=[1024, 768],voxel_spacing=(1,1,1)):
         """Draws voxel model after building it with the provided `array` with PyVista library
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
                 * 'custom'                      --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
@@ -337,19 +337,24 @@
                 * and so on...
         geometry: string  
             voxel geometry. Choose voxels to have a box geometry with geometry='voxels' or spherical one with geometry='particles'
         scalars : list
             list of scalars for cmap coloring scheme
         background_color : string / hex
             background color of pyvista plot
+        wireframe: bool
+            Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
+        wireframe_color: string / hex 
+            edges or wireframe colors
         window_size : (float,float)
             defines plot window dimensions. Defaults to [1024, 768], unless set differently in the relevant theme’s window_size property [pyvista.Plotter]
         voxel_spacing : (float,float,float)
             changes voxel spacing by defining length scales of x y and z directions (default:(1,1,1)).
         """
+
         xx, yy, zz, voxid = arr2crds(self.array, -1).T
 
         centers = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
 
         pl = pyvista.Plotter(window_size=window_size)
 
         if background_color != "":
@@ -430,20 +435,20 @@
             else:
                 voxel = pyvista.Cube(center=centers[i],x_length=x_len, y_length=y_len, z_length=z_len)
                 smooth= None
 
             # Mesh creation and coloring
             if coloring[:6] == 'custom' or coloring[:4] == 'cmap' :
                 voxel_color, voxel_alpha = self.hashblocks[voxid[i]]
-                pl.add_mesh(voxel, color=voxel_color, smooth_shading=smooth, opacity=voxel_alpha,show_edges=True if wireframe else False)
+                pl.add_mesh(voxel, color=voxel_color, smooth_shading=smooth, opacity=voxel_alpha,show_edges=True if wireframe else False, edge_color=wireframe_color)
             elif coloring == 'none':
-                pl.add_mesh(voxel,smooth_shading=smooth, show_edges=True if wireframe else False)
+                pl.add_mesh(voxel,smooth_shading=smooth, show_edges=True if wireframe else False, edge_color=wireframe_color)
             else:
                 pl.add_mesh(voxel, scalars=[i for i in range(
-                    8)] if scalars == '' else scalars,smooth_shading=smooth, show_edges=True if wireframe else False, cmap=coloring)
+                    8)] if scalars == '' else scalars,smooth_shading=smooth, show_edges=True if wireframe else False, edge_color=wireframe_color, cmap=coloring)
 
         pl.isometric_view_interactive()
         pl.show(interactive=True)
 
     def save(self, filename='voxeldata.json'):
         """Save sparse array + color assignments Model data as a dictionary of keys (DOK) JSON file
 
@@ -634,28 +639,41 @@
         # image in self.file mapped to 3d if self.file image specified else it takes the 3-D array defined in self.array
         array = self.ImageMap(voxel_depth) if self.file != '' else self.array              
 
         MarchingMesh(array, out_file=self.objfile, level=level,spacing=spacing, gradient_direction=gradient_direction, step_size=step_size, allow_degenerate=allow_degenerate, method=method, mask=mask, plot=plot, figsize=figsize)
         
         print('mesh created! saved as {}.'.format(self.objfile))
 
-    def MeshView(self,wireframe=False,color='pink',alpha=0.5,background_color='#333333', viewport = [1024, 768]):
+    def MeshView(self,color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
         """
         Triangulated mesh view with PyVista
 
         Parameters
         --------------
         objfile: string
             .obj file to process with MeshView [in GLOBAL function only]
-        wireframe: bool
-            Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
         color : string / hexadecimal
             mesh color. default: 'pink'
         alpha : float
             opacity transparency range: 0 - 1.0. Default: 0.5
+        wireframe: bool
+            Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
+        wireframe_color: string / hex 
+            edges or wireframe colors
         background_color : string / hexadecimal
             color of background. default: 'pink'
         viewport : (int,int)
             viewport / screen (width, height) for display window (default: 80% your screen's width & height)
         """
-        mesh = pv.read(self.objfile)
-        mesh.plot(show_edges=True if wireframe else False, color=color,opacity=alpha,background=background_color,window_size = viewport)
+        # Define a custom theme for the 3D plot
+        my_theme = pyvista.themes.DefaultTheme()
+        my_theme.color = color
+        my_theme.lighting = True
+        my_theme.show_edges = True if wireframe else False
+        my_theme.edge_color = wireframe_color
+        my_theme.background = background_color
+
+
+        mesh = pyvista.read(self.objfile)
+        # mesh.plot(show_edges=True if wireframe else False, color=color,opacity=alpha,background=background_color,window_size = viewport)
+        mesh.plot(theme=my_theme,opacity=alpha,window_size = viewport)
+
```

### Comparing `voxelmap-4.0.0/setup.py` & `voxelmap-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pyvista>=0.38.2,<0.39.0',
  'scikit-image>=0.19.3,<0.20.0',
  'scipy>=1.10.0,<2.0.0',
  'trimesh>=3.21.5,<4.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '4.0.0',
+    'version': '4.1.0',
     'description': 'A Python library for making voxel and 3D models from NumPy arrays.',
     'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making voxel and three-dimensional models from NumPy arrays. \n\n<a href="https://voxelmap.readthedocs.io/en/latest/">\n<img src="https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true" width="250"></a>\n\n## Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n\n## Just starting? Remote Usage with a Colab notebook (click below)\n\n<a href="https://colab.research.google.com/drive/1RMEMgZHlk_tKAzfS4QfXLJV9joDgdh8N?usp=sharing">\n<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/colaboratory.png" width="500" ></a>\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is free software. It comes without any warranty, to the extent permitted by applicable law. You can redistribute it and/or modify it under the terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.\n\n**[MIT license](./LICENSE)** Copyright 2022 © <a href="https://github.com/andrewrgarcia" target="_blank">Andrew Garcia</a>.\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
 python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.2.0,<8.0.0',
 'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
 'scipy>=1.10.0,<2.0.0', 'trimesh>=3.21.5,<4.0.0'] setup_kwargs = { 'name':
-'voxelmap', 'version': '4.0.0', 'description': 'A Python library for making
+'voxelmap', 'version': '4.1.0', 'description': 'A Python library for making
 voxel and 3D models from NumPy arrays.', 'long_description': '# voxelmap\n\n[!
 [License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
 (https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
 [Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
 Python library for making voxel and three-dimensional models from NumPy arrays.
 \n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
```

### Comparing `voxelmap-4.0.0/PKG-INFO` & `voxelmap-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 4.0.0
+Version: 4.1.0
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 4.0.0 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 4.1.0 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
```

