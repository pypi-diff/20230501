# Comparing `tmp/voxelmap-3.7.1.tar.gz` & `tmp/voxelmap-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-3.7.1.tar", max compression
+gzip compressed data, was "voxelmap-4.0.0.tar", max compression
```

## Comparing `voxelmap-3.7.1.tar` & `voxelmap-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-3.7.1/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-3.7.1/README.md
--rw-r--r--   0        0        0      545 2023-04-27 03:49:34.502547 voxelmap-3.7.1/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-3.7.1/voxelmap/__init__.py
--rw-r--r--   0        0        0    17220 2023-03-31 17:25:56.067763 voxelmap-3.7.1/voxelmap/annex.py
--rwxr-xr-x   0        0        0    29140 2023-04-26 18:13:03.766171 voxelmap-3.7.1/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 voxelmap-3.7.1/setup.py
--rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 voxelmap-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.0.0/README.md
+-rw-r--r--   0        0        0      565 2023-04-30 22:23:22.071732 voxelmap-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.0.0/voxelmap/__init__.py
+-rw-r--r--   0        0        0    21552 2023-04-30 22:12:36.911725 voxelmap-4.0.0/voxelmap/annex.py
+-rwxr-xr-x   0        0        0    28050 2023-04-30 22:22:33.171997 voxelmap-4.0.0/voxelmap/jotunn.py
+-rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 voxelmap-4.0.0/setup.py
+-rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 voxelmap-4.0.0/PKG-INFO
```

### Comparing `voxelmap-3.7.1/LICENSE` & `voxelmap-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-3.7.1/README.md` & `voxelmap-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-3.7.1/pyproject.toml` & `voxelmap-4.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "3.7.1"
+version = "4.0.0"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -13,12 +13,13 @@
 matplotlib = "^3.6.2"
 pandas = "^1.5.2"
 opencv-python = "^4.7.0.68"
 scipy = "^1.10.0"
 scikit-image = "^0.19.3"
 pyvista = "^0.38.2"
 colorcet = "^3.0.1"
+trimesh = "^3.21.5"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `voxelmap-3.7.1/voxelmap/annex.py` & `voxelmap-4.0.0/voxelmap/annex.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 from skimage import measure
 from skimage.draw import ellipsoid
 from scipy import ndimage 
 import pyvista as pv
 
+import pandas
+
 def findcrossover(array,low,high,value):
     'finds crossover index of array for `value` value'
     if array[high] <= value:
         return high
     if array[low] > value:
         return low 
 
@@ -495,8 +497,120 @@
     background_color : string / hexadecimal
         color of background. default: 'pink'
     viewport : (int,int)
         viewport / screen (width, height) for display window (default: 80% your screen's width & height)
     """
 
     voxelwrite(array, filename = filename)
-    MeshView(objfile=filename,wireframe=wireframe,color=color,alpha=alpha,background_color=background_color, viewport = viewport)
+    MeshView(objfile=filename,wireframe=wireframe,color=color,alpha=alpha,background_color=background_color, viewport = viewport)
+
+
+def xyz_to_sparse_array(df,hashblocks,spacing=1):
+    """
+    Converts a pandas DataFrame df with columns 'x', 'y', 'z', and 'rgb' to a sparse 3D array.
+
+    The function returns the array and a dictionary `hashblocks` that maps voxel colors to their corresponding index values in the array.
+
+    Parameters:
+    -----------
+    df : pandas DataFrame
+        The input DataFrame containing 'x', 'y', 'z', and 'rgb' columns.
+
+    hashblocks : dict
+        A dictionary that maps voxel colors to their corresponding index values in the array.
+    
+    spacing: float
+        Determines the distance between points in a point cloud. It can be adjusted to create a denser or sparser point cloud.
+        If points are all less than 1, the sparse array will be unable to draw a model because sparse arrays have discrete dimensions, 
+        so changing them to a larger value may be necessary. Likewise, if separation is too large, this value can be set to a fractional number e.g. 0.5
+
+    Returns:
+    --------
+    array : numpy array
+        A 3D numpy array with dimensions Z x Y x X, where Z, Y, and X represent the maximum voxel values of the input DataFrame.
+
+    hashblocks : dict
+        A dictionary that maps voxel colors to their corresponding index values in the array.
+    """
+    df[['x','y','z']] = spacing*df[['x','y','z']]
+
+    minx, miny, minz = df.min()[0:3]
+    maxx, maxy, maxz = df.max()[0:3]
+
+    df['z'] += (-minz)
+    df['y'] += (-miny)
+    df['x'] += (-minx)
+
+    Z, Y, X = int(maxz-minz+1), int(maxy-miny+1), int(maxx-minx+1)
+
+    array =  np.zeros((Z, Y, X))
+
+    elems = df.T
+
+    'define voxel hashblocks dict from colors present in voxel file'
+    model_colors = sorted(list(set(df['rgb'])))
+
+    if isinstance(model_colors[0], str):
+        for i in range(len(model_colors)):
+            # hashblocks.update({i+1: model_colors[i] })
+            hashblocks[i+1] = ['#'+model_colors[i], 1]
+        print('Color list built from file!\nhashblocks =\n',hashblocks)
+
+    'write array from .txt file voxel color values and locs'
+    for i in range(len(elems.T)):
+        x, y, z = elems[i][0:3].astype('int')
+
+        if isinstance(model_colors[0], str):
+            rgb = '#'+elems[i][3]
+            array[z, y, x] = [
+                i for i in hashblocks if hashblocks[i][0] == rgb][0]
+        else:
+            array[z, y, x] = elems[i][3]
+
+    return array, hashblocks
+
+
+def wavefront_to_xyz(filename='model.obj'):
+    """
+    Converts a Wavefront .obj file into a df pandas dataframe of vertex coordinates to be represented as a point cloud, 
+    where df has columns 'z', 'y', 'x', and 'rgb'. 
+
+    Parameters
+    ----------
+    filename : str, optional
+        The path and name of the .obj file to be read. Default is 'model.obj'.
+
+    """
+
+    # Read the .obj file into a list of strings
+    with open(filename) as f:
+        lines = f.readlines()
+
+    # Initialize an empty list to hold the vertex coordinates
+    vertices = []
+
+    # Iterate over each line in the .obj file
+    for line in lines:
+        # Check if the line starts with 'v' and contains 3 coordinates
+        if line.startswith('v ') and len(line.split()) == 4:
+            # Extract the x, y, and z coordinates as floats
+            x, y, z = [float(coord) for coord in line.split()[1:]]
+            # Append the coordinates to the vertices list
+            vertices.append([z, y, x, "#ffffff"])  # placeholder for the rgb value
+
+    # Convert the vertices list to a pandas dataframe with headers z, y, x, rgb
+    df = pandas.DataFrame(vertices, columns=['z', 'y', 'x', 'rgb'])
+
+    return df
+
+
+def objarray(filename='model.obj',spacing=1):
+    '''
+    Converts a Wavefront .obj file into a sparse, third-order (3-D) `array` to represent a point-cloud model. Spacing variable determines the distance between points in a point cloud. It can be adjusted to create a denser or sparser point cloud.
+    If points are all less than 1, the sparse array will be unable to draw a model because sparse arrays have discrete dimensions, 
+    so changing them to a larger value may be necessary. Likewise, if separation is too large, this value can be set to a fractional number e.g. 0.5
+    '''
+    df = wavefront_to_xyz(filename)
+    hashblocks={}
+    array, _ = xyz_to_sparse_array(df,hashblocks,spacing)
+
+    return array
```

### Comparing `voxelmap-3.7.1/voxelmap/jotunn.py` & `voxelmap-4.0.0/voxelmap/jotunn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-'''
+"""
 VOXELMAP 
 A Python library for making voxel models from NumPy arrays.
 Andrew Garcia, 2022 - beyond
 
-'''
+"""
 import numpy as np
 import random as ran
 import matplotlib.pyplot as plt
 # This import registers the 3D projection, but is otherwise unused.
 from mpl_toolkits.mplot3d import Axes3D  # noqa: F401 unused import
 from matplotlib import cm
 from matplotlib import colors
@@ -25,17 +25,17 @@
 
 # from scipy.spatial import Delaunay
 
 
 
 def SectorHull(array, sector_dims, Z_here, Z_there, Y_here, Y_there, X_here, X_there,  
                 num_simplices, rel_depth, color='orange', trace_min=1, plot=True, ax=[]):
-    '''SectorHull does ConvexHull on a specific 2-D sector of the selected image
+    """SectorHull does ConvexHull on a specific 2-D sector of the selected image
     adapted [ significantly ] from 
-    https://stackoverflow.com/questions/27270477/3d-convex-hull-from-point-cloud'''
+    https://stackoverflow.com/questions/27270477/3d-convex-hull-from-point-cloud"""
 
     sector = array[Y_here:Y_there, X_here:X_there] if sector_dims == 2 else \
              array[Z_here:Z_there, Y_here:Y_there, X_here:X_there]
 
 
     if len(np.unique(sector)) > trace_min:
         
@@ -59,26 +59,26 @@
 
     else:
         return np.empty(0), np.empty(0)
 
 
 
 def binarize(array, colorindex=1):
-    '''converts an array with integer entries to either 0 if 0 or 1 if !=0'''
+    """converts an array with integer entries to either 0 if 0 or 1 if !=0"""
     arrayv = np.zeros((array.shape))
     for i in np.argwhere(array != 0):
         arrayv[tuple(i)] = colorindex
 
     return arrayv
 
 
 class Model:
 
     def __init__(self, array=[],file=''):
-        '''Model structure. Calls `3-D` array to process into 3-D model.
+        """Model structure. Calls `3-D` array to process into 3-D model.
 
         Parameters
         ----------
         array : np.array(int)
             array of the third-order populated with discrete, non-zero integers which may represent a voxel block type
         file : str
             file name and/or path for image file
@@ -98,15 +98,15 @@
 
         XYZ : np.array(float )
             an array containing the x,y,z coordinates of shape `number_voxel-locations` x 3 [for each x y z]
         RGB : list[str] 
             a list for the colors of every voxels in xyz array (length: `number_voxel-locations`)
         sparsity : float
             a factor to separate the relative distance between each voxel (default:10.0 [> 50.0 may have memory limitations])
-        '''
+        """
         self.file = file
         self.array = mpimg.imread(self.file) if file != '' else array   # array of third-order (3-D)
         self.make_intensity() if file != '' else None
 
         self.hashblocks = {}        # start with empty voxel-color dictionary
         self.colormap = cm.cool     # default: cool colormap
         self.alphacm = 1            # default: opaque colormap (alpha=1)
@@ -115,23 +115,23 @@
         self.objfile = 'model.obj'
         self.XYZ = []
         self.RGB = []
         self.sparsity = 10.0
         
 
     def resize_intensity(self, res = 1.0, res_interp = cv2.INTER_AREA):
-        '''Resize the intensity matrix of the provided image.
+        """Resize the intensity matrix of the provided image.
 
         Parameters
         ----------
         res : float, optional
             relative resizing percentage as `x` times the original (default 1.0 [1.0x original dimensions])
         res_interp: object, optional 
             cv2 interpolation function for resizing (default cv2.INTER_AREA)
-        '''
+        """
         
         'Turn image into intensity matrix'
         # self.array = mpimg.imread(self.file)       #load image
         'Use CCIR 601 luma to convert RGB image to rel. grayscale 2-D matrix (https://en.wikipedia.org/wiki/Luma_(video)) '
         color_weights = [0.299,0.587,0.114]
         intensity = np.sum([self.array[:,:,i]*color_weights[i] for i in range(3)],0)*100
 
@@ -140,16 +140,16 @@
         x,y = int(x*res),int(y*res)
         intensity = cv2.resize(intensity, (x,y), interpolation = res_interp )
 
         self.array = intensity.astype('float')  # floor-divide
 
 
     def make_intensity(self):
-        '''Turn image into intensity matrix i.e. matrix with pixel intensities. Outputs self.array as mutable matrix to contain relative pixel intensities in int levels [for file if specified]
-        '''
+        """Turn image into intensity matrix i.e. matrix with pixel intensities. Outputs self.array as mutable matrix to contain relative pixel intensities in int levels [for file if specified]
+        """
         # if self.array == []:
         #     self.array = mpimg.imread(self.file)       #load image
         
         'Use CCIR 601 luma to convert RGB image to rel. grayscale 2-D matrix (https://en.wikipedia.org/wiki/Luma_(video)) '
         color_weights = [0.299,0.587,0.114]
         intensity = np.sum([self.array[:,:,i]*color_weights[i] for i in range(3)],0)*100
 
@@ -161,84 +161,53 @@
 
         self.array = intensity.astype('float')  # floor-divide
 
 
     def importdata(self, filename=''):
 
         def dfgox(file):
-            '''Import Goxel file and convert to numpy array
-            '''
+            """Import Goxel file and convert to numpy array
+            """
             df = pandas.read_csv(file,
                                  sep=' ', skiprows=(0, 1, 2), names=['x', 'y', 'z', 'rgb', 'none'])
 
             return df
 
         def dfXYZ():
-            '''Import Goxel file and convert to numpy array
-            '''
+            """Import Goxel file and convert to numpy array
+            """
             df = pandas.DataFrame(self.sparsity*self.XYZ,
                                   columns=['x', 'y', 'z'])
 
             df['rgb'] = self.RGB if len(self.RGB) else len(df)*['a3ebb1']
 
             return df
 
         df = dfgox(filename) if len(filename) != 0 else dfXYZ()
 
-        minx, miny, minz = df.min()[0:3]
-        maxx, maxy, maxz = df.max()[0:3]
-
-        df['z'] += (-minz)
-        df['y'] += (-miny)
-        df['x'] += (-minx)
-
-        Z, Y, X = int(maxz-minz+1), int(maxy-miny+1), int(maxx-minx+1)
-
-        self.array = np.zeros((Z, Y, X))
-
-        elems = df.T
-
-        'define voxel hashblocks dict from colors present in voxel file'
-        model_colors = sorted(list(set(df['rgb'])))
-
-        if isinstance(model_colors[0], str):
-            for i in range(len(model_colors)):
-                # self.hashblocks.update({i+1: model_colors[i] })
-                self.hashblocks[i+1] = ['#'+model_colors[i], 1]
-            print('Color list built from file!\nself.hashblocks =\n',self.hashblocks)
-
-        'write array from .txt file voxel color values and locs'
-        for i in range(len(elems.T)):
-            x, y, z = elems[i][0:3].astype('int')
-
-            if isinstance(model_colors[0], str):
-                rgb = '#'+elems[i][3]
-                self.array[z, y, x] = [
-                    i for i in self.hashblocks if self.hashblocks[i][0] == rgb][0]
-            else:
-                self.array[z, y, x] = elems[i][3]
+        self.array, self.hashblocks = xyz_to_sparse_array(df,self.hashblocks)
 
         return self.array
 
     def hashblocks_add(self, key, color, alpha=1):
-        '''Make your own 3-D colormap option. Adds to hashblocks dictionary.
+        """Make your own 3-D colormap option. Adds to hashblocks dictionary.
 
         Parameters
         ----------
         key : int   
             array value to color as voxel
         color : str
             color of voxel with corresponding `key` index (either in hexanumerical # format  or default python color string)
         alpha : float, optional
             transparency index (0 -> transparent; 1 -> opaque; default = 1.0)
-        '''
+        """
         self.hashblocks[key] = [color, alpha]
 
     def build(self):
-        '''Builds voxel model structure from python numpy array'''
+        """Builds voxel model structure from python numpy array"""
         binarray = binarize(self.array)   # `binarize` array
         Z, X, Y = np.shape(self.array)
 
         z, x, y = np.indices((Z, X, Y))
 
         'cubes below max cubes(max values in array)'
         voxels = (x == 0) & (y == 0) & (z < binarray[0][0])
@@ -346,15 +315,15 @@
         voxels = Model(self.array).build()
 
         ax.voxels(voxels, facecolors=voxcolors, edgecolors=edgecolors)
         set_axes_equal(ax)
         plt.show()
 
     def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, window_size=[1024, 768],voxel_spacing=(1,1,1)):
-        '''Draws voxel model after building it with the provided `array` with PyVista library
+        """Draws voxel model after building it with the provided `array` with PyVista library
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
                 * 'custom'                      --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
                 * 'custom: #8599A6'             -->  color all voxel types with the #8599A6 hex color (bluish dark gray) and an alpha transparency of 1.0 (default)
@@ -372,15 +341,15 @@
             list of scalars for cmap coloring scheme
         background_color : string / hex
             background color of pyvista plot
         window_size : (float,float)
             defines plot window dimensions. Defaults to [1024, 768], unless set differently in the relevant theme’s window_size property [pyvista.Plotter]
         voxel_spacing : (float,float,float)
             changes voxel spacing by defining length scales of x y and z directions (default:(1,1,1)).
-        '''
+        """
         xx, yy, zz, voxid = arr2crds(self.array, -1).T
 
         centers = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
 
         pl = pyvista.Plotter(window_size=window_size)
 
         if background_color != "":
@@ -472,24 +441,24 @@
                 pl.add_mesh(voxel, scalars=[i for i in range(
                     8)] if scalars == '' else scalars,smooth_shading=smooth, show_edges=True if wireframe else False, cmap=coloring)
 
         pl.isometric_view_interactive()
         pl.show(interactive=True)
 
     def save(self, filename='voxeldata.json'):
-        '''Save sparse array + color assignments Model data as a dictionary of keys (DOK) JSON file
+        """Save sparse array + color assignments Model data as a dictionary of keys (DOK) JSON file
 
         Parameters
         ----------
         filename: string  
             name of file (e.g. 'voxeldata.json')
             Data types:
             .json -> voxel data represented as (DOK) JSON file 
             .txt -> voxel data represented x,y,z,rgb matrix in .txt file (see Goxel .txt imports)
-        '''
+        """
         if filename[-4:] == 'json':
             tojson(filename, self.array, self.hashblocks)
         else:
             toTXT(filename,self.array, self.hashblocks)
 
         return None
     
@@ -523,25 +492,25 @@
 
             else:
                 self.importdata(filename)
 
 
 
     def ImageMap(self,depth=5,out_file='model.obj',plot = False):
-        '''Map image or 2-D array (matrix) to 3-D array
+        """Map image or 2-D array (matrix) to 3-D array
         
         Parameters
         -----------
         depth : int
             depth in number of voxels (default = 5 voxels)
         out_file : str
             name and/or path for Wavefront .obj file output. This is the common format for OpenGL 3-D model files (default: model.obj) 
         plot: bool / str
             plots a preliminary 3-D triangulated image if True with PyVista. For more plotting options, plot by calling MeshView separately.
-        '''
+        """
         matrix = self.array
 
         length, width = np.shape(matrix)
 
         low, high = np.min(matrix),np.max(matrix)
         intensities = np.linspace(low,high,depth).astype('int')
         
@@ -561,30 +530,30 @@
 
         if plot:
             self.MeshView()
 
         return model
     
     def ImageMesh(self, out_file='model.obj', L_sectors = 4, rel_depth = 0.50, trace_min = 1, plot = True, figsize=(4.8,4.8), verbose=False ):
-        '''
+        """
         3-D triangulation of 2-D images / 2-D arrays (matrices) with a Convex Hull algorithm (Andrew Garcia, 2022)
 
         Parameters
         ------------
         out_file : str
             name and/or path for Wavefront .obj file output. This is the common format for OpenGL 3-D model files (default: model.obj) 
         L_sectors: int
             length scale of Convex Hull segments in sector grid, e.g. L_sectors = 4 makes a triangulation of 4 x 4 Convex Hull segments
         rel_depth: float
             relative depth of 3-D model with respect to the image's intensity magnitudes (default: 0.50)
         trace_min: int
             minimum number of points in different z-levels to triangulate per sector (default: 1)
         plot: bool / str
             plots a preliminary 3-D triangulated image if True [with PyVista (& with matplotlib if plot = 'img'). For more plotting options, plot with Meshview instead. 
-        '''
+        """
 
         matrix = self.array
 
         print(matrix)
         L = matrix.shape[0]
         W = matrix.shape[1]
         print(L,W)
```

### Comparing `voxelmap-3.7.1/setup.py` & `voxelmap-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,20 @@
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
  'opencv-python>=4.7.0.68,<5.0.0.0',
  'pandas>=1.5.2,<2.0.0',
  'pytest>=7.2.0,<8.0.0',
  'pyvista>=0.38.2,<0.39.0',
  'scikit-image>=0.19.3,<0.20.0',
- 'scipy>=1.10.0,<2.0.0']
+ 'scipy>=1.10.0,<2.0.0',
+ 'trimesh>=3.21.5,<4.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '3.7.1',
+    'version': '4.0.0',
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
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
 python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.2.0,<8.0.0',
 'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
-'scipy>=1.10.0,<2.0.0'] setup_kwargs = { 'name': 'voxelmap', 'version':
-'3.7.1', 'description': 'A Python library for making voxel and 3D models from
-NumPy arrays.', 'long_description': '# voxelmap\n\n[![License](http://
-img.shields.io/:license-mit-blue.svg?style=flat-square)](https://
-raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
+'scipy>=1.10.0,<2.0.0', 'trimesh>=3.21.5,<4.0.0'] setup_kwargs = { 'name':
+'voxelmap', 'version': '4.0.0', 'description': 'A Python library for making
+voxel and 3D models from NumPy arrays.', 'long_description': '# voxelmap\n\n[!
+[License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
+(https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
 [Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
 Python library for making voxel and three-dimensional models from NumPy arrays.
 \n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
 voxelmap.svg?raw=true]\n\n## Installation and Local Usage \n\n```ruby\npip
 install voxelmap\n```\n\nIt is recommended you run voxelmap using a
 `virtualenv` virtual environment. To do so, follow the below simple protocol to
```

### Comparing `voxelmap-3.7.1/PKG-INFO` & `voxelmap-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 3.7.1
+Version: 4.0.0
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,15 @@
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: pyvista (>=0.38.2,<0.39.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: trimesh (>=3.21.5,<4.0.0)
 Description-Content-Type: text/markdown
 
 # voxelmap
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 3.7.1 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 4.0.0 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
 (>=3.6.2,<4.0.0) Requires-Dist: numpy (>=1.24.1,<2.0.0) Requires-Dist: opencv-
 python (>=4.7.0.68,<5.0.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-
 Dist: pytest (>=7.2.0,<8.0.0) Requires-Dist: pyvista (>=0.38.2,<0.39.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0) Requires-Dist: scipy
-(>=1.10.0,<2.0.0) Description-Content-Type: text/markdown # voxelmap [!
-[License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
-(https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE) [!
-[Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
-?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest) A
-Python library for making voxel and three-dimensional models from NumPy arrays.
-[https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true] ##
-Installation and Local Usage ```ruby pip install voxelmap ``` It is recommended
-you run voxelmap using a `virtualenv` virtual environment. To do so, follow the
-below simple protocol to create the virtual environment, run it, and install
-the package there: ```ruby virtualenv venv source venv/bin/activate pip install
-voxelmap python [your-voxelmap-script.py] ``` To exit the virtual environment,
-simply type `deactivate`. To access it at any other time again, enter with the
-above `source venv...` command. ## Just starting? Remote Usage with a Colab
-notebook (click below) [https://raw.githubusercontent.com/andrewrgarcia/
-voxelmap/main/docs/img/colaboratory.png] ## Disclaimer: Use At Your Own Risk
-This program is free software. It comes without any warranty, to the extent
-permitted by applicable law. You can redistribute it and/or modify it under the
-terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for
-more details. **[MIT license](./LICENSE)** Copyright 2022 Â© Andrew_Garcia.
+(>=1.10.0,<2.0.0) Requires-Dist: trimesh (>=3.21.5,<4.0.0) Description-Content-
+Type: text/markdown # voxelmap [![License](http://img.shields.io/:license-mit-
+blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/
+voxelmap/main/LICENSE) [![Documentation Status](https://readthedocs.org/
+projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/
+latest/?badge=latest) A Python library for making voxel and three-dimensional
+models from NumPy arrays. [https://github.com/andrewrgarcia/voxelmap/blob/main/
+voxelmap.svg?raw=true] ## Installation and Local Usage ```ruby pip install
+voxelmap ``` It is recommended you run voxelmap using a `virtualenv` virtual
+environment. To do so, follow the below simple protocol to create the virtual
+environment, run it, and install the package there: ```ruby virtualenv venv
+source venv/bin/activate pip install voxelmap python [your-voxelmap-script.py]
+``` To exit the virtual environment, simply type `deactivate`. To access it at
+any other time again, enter with the above `source venv...` command. ## Just
+starting? Remote Usage with a Colab notebook (click below) [https://
+raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/
+colaboratory.png] ## Disclaimer: Use At Your Own Risk This program is free
+software. It comes without any warranty, to the extent permitted by applicable
+law. You can redistribute it and/or modify it under the terms of the MIT
+LICENSE, as published by Andrew Garcia. See LICENSE below for more details. **
+[MIT license](./LICENSE)** Copyright 2022 Â© Andrew_Garcia.
```

