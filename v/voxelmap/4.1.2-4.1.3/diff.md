# Comparing `tmp/voxelmap-4.1.2.tar.gz` & `tmp/voxelmap-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-4.1.2.tar", max compression
+gzip compressed data, was "voxelmap-4.1.3.tar", max compression
```

## Comparing `voxelmap-4.1.2.tar` & `voxelmap-4.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.1.2/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.1.2/README.md
--rw-r--r--   0        0        0      567 2023-05-01 00:58:57.089377 voxelmap-4.1.2/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.1.2/voxelmap/__init__.py
--rw-r--r--   0        0        0    21985 2023-04-30 23:03:40.856964 voxelmap-4.1.2/voxelmap/annex.py
--rwxr-xr-x   0        0        0    28849 2023-05-01 00:22:13.552180 voxelmap-4.1.2/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 voxelmap-4.1.2/setup.py
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 voxelmap-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.1.3/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.1.3/README.md
+-rw-r--r--   0        0        0      526 2023-05-01 01:49:27.131152 voxelmap-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.1.3/voxelmap/__init__.py
+-rw-r--r--   0        0        0    21518 2023-05-01 01:42:22.585166 voxelmap-4.1.3/voxelmap/annex.py
+-rwxr-xr-x   0        0        0    28849 2023-05-01 01:44:24.008146 voxelmap-4.1.3/voxelmap/jotunn.py
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 voxelmap-4.1.3/setup.py
+-rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 voxelmap-4.1.3/PKG-INFO
```

### Comparing `voxelmap-4.1.2/LICENSE` & `voxelmap-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.2/README.md` & `voxelmap-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.2/pyproject.toml` & `voxelmap-4.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [tool.poetry]
 name = "voxelmap"
-version = "4.1.2"
+version = "4.1.3"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1.24.1"
-pytest = "^7.2.0"
 matplotlib = "^3.6.2"
 pandas = "^1.5.2"
 opencv-python = "^4.7.0.68"
 scipy = "^1.10.0"
 scikit-image = "^0.19.3"
 pyvista = "^0.38.2"
 colorcet = "^3.0.1"
-setuptools = "^67.7.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `voxelmap-4.1.2/voxelmap/annex.py` & `voxelmap-4.1.3/voxelmap/annex.py`

 * *Files 7% similar despite different names*

```diff
@@ -300,24 +300,24 @@
                     j3,(rand_t0+2)%4+1,j3 
                     ]
 
             f.write("f {}/{}/{} {}/{}/{} {}/{}/{}\n".format(*facestr))
 
 
 def voxelwrite(array, filename = 'voxelmodel.obj'):
-    """
+    '''
     Writes a 3-D voxel model from the provided, third-order (3-D) `array` as an .obj file
     
     Parameters
     ----------
     array : np.array(int)
             array of the third-order populated with discrete, non-zero integers which may represent a voxel block type
     filename : str
             name of .obj file to save model as. 
-    """
+    '''
 
 
     # vertices diff (diffvs) for cube writing
     diffvs = np.array([
         [-0.50, -0.50, 0.00],
         [-0.50, 0.50, 0.00],
         [0.50, 0.50, 0.00],
@@ -387,15 +387,15 @@
             # 2 -> 17
 
 
 
 
 
 def MarchingMesh(array, out_file='model.obj', level=0, spacing=(1., 1., 1.), gradient_direction='descent', step_size=1, allow_degenerate=True, method='lewiner', mask=None, plot=False, figsize=(4.8,4.8) ):
-    """
+    '''
     Marching cubes on sparse 3-D integer `voxelmap` arrays (GLOBAL)
 
     Parameters
     -------------
     array: np.array((int/float,int/float,int/float))
         3-D array for which to run the marching cubes algorithm   
     out_file : str
@@ -413,15 +413,15 @@
         Whether to allow degenerate (i.e. zero-area) triangles in the end-result. Default True. If False, degenerate triangles are removed, at the cost of making the algorithm slower.
     method: str, optional
         One of 'lewiner', 'lorensen' or '_lorensen'. Specify which of Lewiner et al. or Lorensen et al. method will be used. The '_lorensen' flag correspond to an old implementation that will be deprecated in version 0.19.
     mask : (M, N, P) array, optional
         Boolean array. The marching cube algorithm will be computed only on True elements. This will save computational time when interfaces are located within certain region of the volume M, N, P-e.g. the top half of the cube-and also allow to compute finite surfaces-i.e. open surfaces that do not end at the border of the cube.
     plot: bool
         plots a preliminary 3-D triangulated image if True
-    """
+    '''
 
     '''Adapted from: https://scikit-image.org/docs/stable/auto_examples/edges/plot_marching_cubes.html'''
     # Use marching cubes to obtain the surface mesh of these ellipsoids
     verts, faces, normals, values = measure.marching_cubes(
                                     array, level=level, spacing=spacing, 
                                     gradient_direction=gradient_direction, step_size=step_size,
                                     allow_degenerate=allow_degenerate, method=method, mask=mask
@@ -451,53 +451,53 @@
         # plt.tight_layout()
         # plt.show()
 
         MeshView(out_file)
 
 
 def MeshView(objfile='model.obj',color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
-    """
+    '''
     Triangulated mesh view with PyVista (GLOBAL)
     
     Parameters
-    ----------
+    --------------
     objfile: string
         .obj file to process with MeshView [in GLOBAL function only]
     color : string / hexadecimal
         mesh color. default: 'pink'
     alpha : float
         opacity transparency range: 0 - 1.0. Default: 0.5
     wireframe: bool
         Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
     wireframe_color: string / hex 
         edges or wireframe colors
     background_color : string / hexadecimal
         color of background. default: 'pink'
     viewport : (int,int)
         viewport / screen (width, height) for display window (default: 80% your screen's width & height)
-    """
+    '''
     # Define a custom theme for the 3D plot
     my_theme = pyvista.themes.DefaultTheme()
     my_theme.color = color
     my_theme.lighting = True
     my_theme.show_edges = True if wireframe else False
     my_theme.edge_color = wireframe_color
     my_theme.background = background_color
 
 
     mesh = pyvista.read(objfile)
     mesh.plot(theme=my_theme,opacity=alpha,window_size = viewport)
     
 
 def objdraw(array,filename='voxelmodel.obj',color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
-    """
+    '''
     Creates a 3-D voxel model (.obj file) from the provided, third-order (3-D) `array`. It then uses the global method MeshView to draw the .obj file and display it on screen 
     
     Parameters
-    ----------
+    ------------------
     array : np.array(int)
             array of the third-order populated with discrete, non-zero integers which may represent a voxel block type
     filename : str
             name of .obj file to save model as. 
     objfile: string
         .obj file to process with MeshView [in GLOBAL function only]
     wireframe: bool
@@ -506,46 +506,32 @@
         mesh color. default: 'pink'
     alpha : float
         opacity transparency range: 0 - 1.0. Default: 0.5
     background_color : string / hexadecimal
         color of background. default: 'pink'
     viewport : (int,int)
         viewport / screen (width, height) for display window (default: 80% your screen's width & height)
-    """
+    '''
     voxelwrite(array, filename = filename)
     # MeshView(objfile=filename,wireframe=wireframe,color=color,alpha=alpha,background_color=background_color, viewport = viewport)
     MeshView(filename,color,alpha,wireframe,wireframe_color,background_color, viewport )
 
 def xyz_to_sparse_array(df,hashblocks,spacing=1):
-    """
-    Converts a pandas DataFrame df with columns 'x', 'y', 'z', and 'rgb' to a sparse 3D array.
-
-    The function returns the array and a dictionary `hashblocks` that maps voxel colors to their corresponding index values in the array.
+    '''
+    Converts a pandas DataFrame df with columns 'x', 'y', 'z', and 'rgb' to a sparse 3D array. The function returns the array and a dictionary `hashblocks` that maps voxel colors to their corresponding index values in the array.
 
-    Parameters:
-    -----------
+    Parameters
+    -------------
     df : pandas DataFrame
         The input DataFrame containing 'x', 'y', 'z', and 'rgb' columns.
-
     hashblocks : dict
         A dictionary that maps voxel colors to their corresponding index values in the array.
-    
     spacing: float
-        Determines the distance between points in a point cloud. It can be adjusted to create a denser or sparser point cloud.
-        If points are all less than 1, the sparse array will be unable to draw a model because sparse arrays have discrete dimensions, 
-        so changing them to a larger value may be necessary. Likewise, if separation is too large, this value can be set to a fractional number e.g. 0.5
-
-    Returns:
-    --------
-    array : numpy array
-        A 3D numpy array with dimensions Z x Y x X, where Z, Y, and X represent the maximum voxel values of the input DataFrame.
-
-    hashblocks : dict
-        A dictionary that maps voxel colors to their corresponding index values in the array.
-    """
+        Determines the distance between points in a point cloud. It can be adjusted to create a denser or sparser point cloud. If points are all less than 1, the sparse array will be unable to draw a model because sparse arrays have discrete dimensions, so changing them to a larger value may be necessary. Likewise, if separation is too large, this value can be set to a fractional number e.g. 0.5
+    '''
     df[['x','y','z']] = spacing*df[['x','y','z']]
 
     minx, miny, minz = df.min()[0:3]
     maxx, maxy, maxz = df.max()[0:3]
 
     df['z'] += (-minz)
     df['y'] += (-miny)
@@ -577,24 +563,22 @@
         else:
             array[z, y, x] = elems[i][3]
 
     return array, hashblocks
 
 
 def wavefront_to_xyz(filename='model.obj'):
-    """
-    Converts a Wavefront .obj file into a df pandas dataframe of vertex coordinates to be represented as a point cloud, 
-    where df has columns 'z', 'y', 'x', and 'rgb'. 
+    '''
+    Converts a Wavefront .obj file into a df pandas dataframe of vertex coordinates to be represented as a point cloud, where df has columns 'z', 'y', 'x', and 'rgb'. 
 
     Parameters
-    ----------
+    ---------------
     filename : str, optional
         The path and name of the .obj file to be read. Default is 'model.obj'.
-
-    """
+    '''
 
     # Read the .obj file into a list of strings
     with open(filename) as f:
         lines = f.readlines()
 
     # Initialize an empty list to hold the vertex coordinates
     vertices = []
@@ -612,16 +596,22 @@
     df = pandas.DataFrame(vertices, columns=['z', 'y', 'x', 'rgb'])
 
     return df
 
 
 def objarray(filename='model.obj',spacing=1):
     '''
-    Converts a Wavefront .obj file into a sparse, third-order (3-D) `array` to represent a point-cloud model. Spacing variable determines the distance between points in a point cloud. It can be adjusted to create a denser or sparser point cloud.
-    If points are all less than 1, the sparse array will be unable to draw a model because sparse arrays have discrete dimensions, 
-    so changing them to a larger value may be necessary. Likewise, if separation is too large, this value can be set to a fractional number e.g. 0.5
+    Converts a Wavefront .obj file into a sparse, third-order (3-D) NumPy array to represent a point cloud model.
+
+    Parameters
+    ---------------
+    filename : str 
+        Path to the .obj file. Defaults to 'model.obj'.
+    spacing : float
+        Distance between points in the point cloud. Can be adjusted to create a denser or sparser point cloud. Defaults to 1.
     '''
+
     df = wavefront_to_xyz(filename)
     hashblocks={}
     array, _ = xyz_to_sparse_array(df,hashblocks,spacing)
 
     return array
```

### Comparing `voxelmap-4.1.2/voxelmap/jotunn.py` & `voxelmap-4.1.3/voxelmap/jotunn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""
+'''
 VOXELMAP 
 A Python library for making voxel models from NumPy arrays.
 Andrew Garcia, 2022 - beyond
 
-"""
+'''
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
-    """SectorHull does ConvexHull on a specific 2-D sector of the selected image
+    '''SectorHull does ConvexHull on a specific 2-D sector of the selected image
     adapted [ significantly ] from 
-    https://stackoverflow.com/questions/27270477/3d-convex-hull-from-point-cloud"""
+    https://stackoverflow.com/questions/27270477/3d-convex-hull-from-point-cloud'''
 
     sector = array[Y_here:Y_there, X_here:X_there] if sector_dims == 2 else \
              array[Z_here:Z_there, Y_here:Y_there, X_here:X_there]
 
 
     if len(np.unique(sector)) > trace_min:
         
@@ -59,26 +59,26 @@
 
     else:
         return np.empty(0), np.empty(0)
 
 
 
 def binarize(array, colorindex=1):
-    """converts an array with integer entries to either 0 if 0 or 1 if !=0"""
+    '''converts an array with integer entries to either 0 if 0 or 1 if !=0'''
     arrayv = np.zeros((array.shape))
     for i in np.argwhere(array != 0):
         arrayv[tuple(i)] = colorindex
 
     return arrayv
 
 
 class Model:
 
     def __init__(self, array=[],file=''):
-        """Model structure. Calls `3-D` array to process into 3-D model.
+        '''Model structure. Calls `3-D` array to process into 3-D model.
 
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
-        """
+        '''
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
-        """Resize the intensity matrix of the provided image.
+        '''Resize the intensity matrix of the provided image.
 
         Parameters
         ----------
         res : float, optional
             relative resizing percentage as `x` times the original (default 1.0 [1.0x original dimensions])
         res_interp: object, optional 
             cv2 interpolation function for resizing (default cv2.INTER_AREA)
-        """
+        '''
         
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
-        """Turn image into intensity matrix i.e. matrix with pixel intensities. Outputs self.array as mutable matrix to contain relative pixel intensities in int levels [for file if specified]
-        """
+        '''Turn image into intensity matrix i.e. matrix with pixel intensities. Outputs self.array as mutable matrix to contain relative pixel intensities in int levels [for file if specified]
+        '''
         # if self.array == []:
         #     self.array = mpimg.imread(self.file)       #load image
         
         'Use CCIR 601 luma to convert RGB image to rel. grayscale 2-D matrix (https://en.wikipedia.org/wiki/Luma_(video)) '
         color_weights = [0.299,0.587,0.114]
         intensity = np.sum([self.array[:,:,i]*color_weights[i] for i in range(3)],0)*100
 
@@ -161,53 +161,53 @@
 
         self.array = intensity.astype('float')  # floor-divide
 
 
     def importdata(self, filename=''):
 
         def dfgox(file):
-            """Import Goxel file and convert to numpy array
-            """
+            '''Import Goxel file and convert to numpy array
+            '''
             df = pandas.read_csv(file,
                                  sep=' ', skiprows=(0, 1, 2), names=['x', 'y', 'z', 'rgb', 'none'])
 
             return df
 
         def dfXYZ():
-            """Import Goxel file and convert to numpy array
-            """
+            '''Import Goxel file and convert to numpy array
+            '''
             df = pandas.DataFrame(self.sparsity*self.XYZ,
                                   columns=['x', 'y', 'z'])
 
             df['rgb'] = self.RGB if len(self.RGB) else len(df)*['a3ebb1']
 
             return df
 
         df = dfgox(filename) if len(filename) != 0 else dfXYZ()
 
         self.array, self.hashblocks = xyz_to_sparse_array(df,self.hashblocks)
 
         return self.array
 
     def hashblocks_add(self, key, color, alpha=1):
-        """Make your own 3-D colormap option. Adds to hashblocks dictionary.
+        '''Make your own 3-D colormap option. Adds to hashblocks dictionary.
 
         Parameters
         ----------
         key : int   
             array value to color as voxel
         color : str
             color of voxel with corresponding `key` index (either in hexanumerical # format  or default python color string)
         alpha : float, optional
             transparency index (0 -> transparent; 1 -> opaque; default = 1.0)
-        """
+        '''
         self.hashblocks[key] = [color, alpha]
 
     def build(self):
-        """Builds voxel model structure from python numpy array"""
+        '''Builds voxel model structure from python numpy array'''
         binarray = binarize(self.array)   # `binarize` array
         Z, X, Y = np.shape(self.array)
 
         z, x, y = np.indices((Z, X, Y))
 
         'cubes below max cubes(max values in array)'
         voxels = (x == 0) & (y == 0) & (z < binarray[0][0])
@@ -219,15 +219,15 @@
                         cube0 = (x == i) & (y == j) & (z == k)
 
                         voxels = voxels | cube0
 
         return voxels
 
     def draw_mpl(self, coloring='custom', edgecolors=None, figsize=(6.4, 4.8), axis3don=False):
-        """
+        '''
         Draws voxel model after building it with the provided `array` (Matplotlib version. For faster graphics, try the ``draw()`` method (uses PyVista)). 
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
                 * 'custom' --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
@@ -237,15 +237,15 @@
                 * 'linear'   colors voxel model vertically, top to bottom. 
         edgecolors: string/hex
             edge color of voxels (default: None)
         figsize : (float,float)
             defines plot window dimensions. From matplotlib.pyplot.figure(figsize) kwarg. 
         axis3don: bool
             defines presence of 3D axis in voxel model plot (Default: False)
-        """
+        '''
 
         Z, X, Y = np.shape(self.array)
 
         voxcolors = np.ones((Z, X, Y), dtype=object)
 
         def gradient_nuclear_coloring():
 
@@ -315,15 +315,15 @@
         voxels = Model(self.array).build()
 
         ax.voxels(voxels, facecolors=voxcolors, edgecolors=edgecolors)
         set_axes_equal(ax)
         plt.show()
 
     def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, wireframe_color='k', window_size=[1024, 768],voxel_spacing=(1,1,1)):
-        """Draws voxel model after building it with the provided `array` with PyVista library
+        '''Draws voxel model after building it with the provided `array` with PyVista library
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
                 * 'custom'                      --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
                 * 'custom: #8599A6'             -->  color all voxel types with the #8599A6 hex color (bluish dark gray) and an alpha transparency of 1.0 (default)
@@ -345,15 +345,15 @@
             Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
         wireframe_color: string / hex 
             edges or wireframe colors
         window_size : (float,float)
             defines plot window dimensions. Defaults to [1024, 768], unless set differently in the relevant theme’s window_size property [pyvista.Plotter]
         voxel_spacing : (float,float,float)
             changes voxel spacing by defining length scales of x y and z directions (default:(1,1,1)).
-        """
+        '''
 
         xx, yy, zz, voxid = arr2crds(self.array, -1).T
 
         centers = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
 
         pl = pyvista.Plotter(window_size=window_size)
 
@@ -446,42 +446,42 @@
                 pl.add_mesh(voxel, scalars=[i for i in range(
                     8)] if scalars == '' else scalars,smooth_shading=smooth, show_edges=True if wireframe else False, edge_color=wireframe_color, cmap=coloring)
 
         pl.isometric_view_interactive()
         pl.show(interactive=True)
 
     def save(self, filename='voxeldata.json'):
-        """Save sparse array + color assignments Model data as a dictionary of keys (DOK) JSON file
+        '''Save sparse array + color assignments Model data as a dictionary of keys (DOK) JSON file
 
         Parameters
         ----------
         filename: string  
             name of file (e.g. 'voxeldata.json')
             Data types:
             .json -> voxel data represented as (DOK) JSON file 
             .txt -> voxel data represented x,y,z,rgb matrix in .txt file (see Goxel .txt imports)
-        """
+        '''
         if filename[-4:] == 'json':
             tojson(filename, self.array, self.hashblocks)
         else:
             toTXT(filename,self.array, self.hashblocks)
 
         return None
     
     def load(self, filename='voxeldata.json', coords=False):
-        """
+        '''
         Load to Model object.
 
         Parameters
         ----------
         filename: string (.json or .txt extensions (see above))
             name of file to be loaded (e.g 'voxeldata.json')
         coords: bool
             loads and processes self.XYZ, self.RGB, and self.sparsity = 10.0 (see Model class desc above) to Model if True. This boolean overrides filename loader option. 
-        """
+        '''
         if coords:
             self.importdata(filename='')
         else:
             if filename[-4:] == 'json':
 
                 data = load_from_json(filename)
                 self.hashblocks = data['hashblocks']
@@ -497,25 +497,25 @@
 
             else:
                 self.importdata(filename)
 
 
 
     def ImageMap(self,depth=5,out_file='model.obj',plot = False):
-        """Map image or 2-D array (matrix) to 3-D array
+        '''Map image or 2-D array (matrix) to 3-D array
         
         Parameters
         -----------
         depth : int
             depth in number of voxels (default = 5 voxels)
         out_file : str
             name and/or path for Wavefront .obj file output. This is the common format for OpenGL 3-D model files (default: model.obj) 
         plot: bool / str
             plots a preliminary 3-D triangulated image if True with PyVista. For more plotting options, plot by calling MeshView separately.
-        """
+        '''
         matrix = self.array
 
         length, width = np.shape(matrix)
 
         low, high = np.min(matrix),np.max(matrix)
         intensities = np.linspace(low,high,depth).astype('int')
         
@@ -535,30 +535,30 @@
 
         if plot:
             self.MeshView()
 
         return model
     
     def ImageMesh(self, out_file='model.obj', L_sectors = 4, rel_depth = 0.50, trace_min = 1, plot = True, figsize=(4.8,4.8), verbose=False ):
-        """
+        '''
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
-        """
+        '''
 
         matrix = self.array
 
         print(matrix)
         L = matrix.shape[0]
         W = matrix.shape[1]
         print(L,W)
@@ -606,15 +606,15 @@
                 plt.axis('off')
                 plt.show()
             else:
                 self.MeshView()
 
 
     def MarchingMesh(self, voxel_depth=12, level=0, spacing=(1., 1., 1.), gradient_direction='descent', step_size=1, allow_degenerate=True, method='lewiner', mask=None,plot=False, figsize=(4.8,4.8) ):
-        """
+        '''
         Marching cubes on 3-D mapped image or 3-D array
 
         Parameters
         ---------------
         voxel_depth : int (optional)
             depth of 3-D mapped image on number of voxels (if file [image] is to be processed / i.e. specified)
         level : float, optional
@@ -630,25 +630,25 @@
             Whether to allow degenerate (i.e. zero-area) triangles in the end-result. Default True. If False, degenerate triangles are removed, at the cost of making the algorithm slower.
         method: str, optional
             One of 'lewiner', 'lorensen' or '_lorensen'. Specify which of Lewiner et al. or Lorensen et al. method will be used. The '_lorensen' flag correspond to an old implementation that will be deprecated in version 0.19.
         mask : (M, N, P) array, optional
             Boolean array. The marching cube algorithm will be computed only on True elements. This will save computational time when interfaces are located within certain region of the volume M, N, P-e.g. the top half of the cube-and also allow to compute finite surfaces-i.e. open surfaces that do not end at the border of the cube.
         plot: bool
             plots a preliminary 3-D triangulated image if True
-        """
+        '''
 
         # image in self.file mapped to 3d if self.file image specified else it takes the 3-D array defined in self.array
         array = self.ImageMap(voxel_depth) if self.file != '' else self.array              
 
         MarchingMesh(array, out_file=self.objfile, level=level,spacing=spacing, gradient_direction=gradient_direction, step_size=step_size, allow_degenerate=allow_degenerate, method=method, mask=mask, plot=plot, figsize=figsize)
         
         print('mesh created! saved as {}.'.format(self.objfile))
 
     def MeshView(self,color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
-        """
+        '''
         Triangulated mesh view with PyVista
 
         Parameters
         --------------
         objfile: string
             .obj file to process with MeshView [in GLOBAL function only]
         color : string / hexadecimal
@@ -659,15 +659,15 @@
             Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
         wireframe_color: string / hex 
             edges or wireframe colors
         background_color : string / hexadecimal
             color of background. default: 'pink'
         viewport : (int,int)
             viewport / screen (width, height) for display window (default: 80% your screen's width & height)
-        """
+        '''
         # Define a custom theme for the 3D plot
         my_theme = pyvista.themes.DefaultTheme()
         my_theme.color = color
         my_theme.lighting = True
         my_theme.show_edges = True if wireframe else False
         my_theme.edge_color = wireframe_color
         my_theme.background = background_color
```

### Comparing `voxelmap-4.1.2/setup.py` & `voxelmap-4.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 
 install_requires = \
 ['colorcet>=3.0.1,<4.0.0',
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
  'opencv-python>=4.7.0.68,<5.0.0.0',
  'pandas>=1.5.2,<2.0.0',
- 'pytest>=7.2.0,<8.0.0',
  'pyvista>=0.38.2,<0.39.0',
  'scikit-image>=0.19.3,<0.20.0',
- 'scipy>=1.10.0,<2.0.0',
- 'setuptools>=67.7.2,<68.0.0']
+ 'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '4.1.2',
+    'version': '4.1.3',
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
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
-python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.2.0,<8.0.0',
-'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
-'scipy>=1.10.0,<2.0.0', 'setuptools>=67.7.2,<68.0.0'] setup_kwargs = { 'name':
-'voxelmap', 'version': '4.1.2', 'description': 'A Python library for making
-voxel and 3D models from NumPy arrays.', 'long_description': '# voxelmap\n\n[!
-[License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
-(https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
-[Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
-?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
-Python library for making voxel and three-dimensional models from NumPy arrays.
-\n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
-voxelmap.svg?raw=true]\n\n## Installation and Local Usage \n\n```ruby\npip
-install voxelmap\n```\n\nIt is recommended you run voxelmap using a
-`virtualenv` virtual environment. To do so, follow the below simple protocol to
-create the virtual environment, run it, and install the package there:
-\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install
+python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pyvista>=0.38.2,<0.39.0',
+'scikit-image>=0.19.3,<0.20.0', 'scipy>=1.10.0,<2.0.0'] setup_kwargs =
+{ 'name': 'voxelmap', 'version': '4.1.3', 'description': 'A Python library for
+making voxel and 3D models from NumPy arrays.', 'long_description': '#
+voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-
+square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/
+LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/
+badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/
+?badge=latest)\n\nA Python library for making voxel and three-dimensional
+models from NumPy arrays. \n\n\n[https://github.com/andrewrgarcia/voxelmap/
+blob/main/voxelmap.svg?raw=true]\n\n## Installation and Local Usage
+\n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap
+using a `virtualenv` virtual environment. To do so, follow the below simple
+protocol to create the virtual environment, run it, and install the package
+there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install
 voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual
 environment, simply type `deactivate`. To access it at any other time again,
 enter with the above `source venv...` command. \n\n## Just starting? Remote
 Usage with a Colab notebook (click below)\n\n\n[https://
 raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/
 colaboratory.png]\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is
 free software. It comes without any warranty, to the extent permitted by
```

### Comparing `voxelmap-4.1.2/PKG-INFO` & `voxelmap-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 4.1.2
+Version: 4.1.3
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,19 +13,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: pyvista (>=0.38.2,<0.39.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Description-Content-Type: text/markdown
 
 # voxelmap
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 4.1.2 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 4.1.3 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
 (>=3.6.2,<4.0.0) Requires-Dist: numpy (>=1.24.1,<2.0.0) Requires-Dist: opencv-
 python (>=4.7.0.68,<5.0.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-
-Dist: pytest (>=7.2.0,<8.0.0) Requires-Dist: pyvista (>=0.38.2,<0.39.0)
-Requires-Dist: scikit-image (>=0.19.3,<0.20.0) Requires-Dist: scipy
-(>=1.10.0,<2.0.0) Requires-Dist: setuptools (>=67.7.2,<68.0.0) Description-
-Content-Type: text/markdown # voxelmap [![License](http://img.shields.io/:
-license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/
-andrewrgarcia/voxelmap/main/LICENSE) [![Documentation Status](https://
-readthedocs.org/projects/voxelmap/badge/?version=latest)](https://
-voxelmap.readthedocs.io/en/latest/?badge=latest) A Python library for making
-voxel and three-dimensional models from NumPy arrays. [https://github.com/
-andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true] ## Installation and
-Local Usage ```ruby pip install voxelmap ``` It is recommended you run voxelmap
-using a `virtualenv` virtual environment. To do so, follow the below simple
-protocol to create the virtual environment, run it, and install the package
-there: ```ruby virtualenv venv source venv/bin/activate pip install voxelmap
-python [your-voxelmap-script.py] ``` To exit the virtual environment, simply
-type `deactivate`. To access it at any other time again, enter with the above
-`source venv...` command. ## Just starting? Remote Usage with a Colab notebook
-(click below) [https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/
-docs/img/colaboratory.png] ## Disclaimer: Use At Your Own Risk This program is
-free software. It comes without any warranty, to the extent permitted by
-applicable law. You can redistribute it and/or modify it under the terms of the
-MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.
-**[MIT license](./LICENSE)** Copyright 2022 Â© Andrew_Garcia.
+Dist: pyvista (>=0.38.2,<0.39.0) Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
+# voxelmap [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-
+square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
+?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest) A
+Python library for making voxel and three-dimensional models from NumPy arrays.
+[https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true] ##
+Installation and Local Usage ```ruby pip install voxelmap ``` It is recommended
+you run voxelmap using a `virtualenv` virtual environment. To do so, follow the
+below simple protocol to create the virtual environment, run it, and install
+the package there: ```ruby virtualenv venv source venv/bin/activate pip install
+voxelmap python [your-voxelmap-script.py] ``` To exit the virtual environment,
+simply type `deactivate`. To access it at any other time again, enter with the
+above `source venv...` command. ## Just starting? Remote Usage with a Colab
+notebook (click below) [https://raw.githubusercontent.com/andrewrgarcia/
+voxelmap/main/docs/img/colaboratory.png] ## Disclaimer: Use At Your Own Risk
+This program is free software. It comes without any warranty, to the extent
+permitted by applicable law. You can redistribute it and/or modify it under the
+terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for
+more details. **[MIT license](./LICENSE)** Copyright 2022 Â© Andrew_Garcia.
```

