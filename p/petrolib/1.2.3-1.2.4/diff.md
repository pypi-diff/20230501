# Comparing `tmp/petrolib-1.2.3.tar.gz` & `tmp/petrolib-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrolib-1.2.3.tar", last modified: Fri Mar 31 14:07:10 2023, max compression
+gzip compressed data, was "petrolib-1.2.4.tar", last modified: Mon May  1 16:29:46 2023, max compression
```

## Comparing `petrolib-1.2.3.tar` & `petrolib-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-03-31 14:07:10.609552 petrolib-1.2.3/
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     1093 2023-03-26 20:57:50.000000 petrolib-1.2.3/LICENSE
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3680 2023-03-31 14:07:10.609552 petrolib-1.2.3/PKG-INFO
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3137 2023-03-31 13:29:52.000000 petrolib-1.2.3/README.md
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      739 2023-03-31 13:28:31.000000 petrolib-1.2.3/pyproject.toml
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       38 2023-03-31 14:07:10.609552 petrolib-1.2.3/setup.cfg
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-03-31 14:07:10.601552 petrolib-1.2.3/src/
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-03-31 14:07:10.605552 petrolib-1.2.3/src/petrolib/
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)       21 2023-03-26 22:39:40.000000 petrolib-1.2.3/src/petrolib/__init__.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     4829 2023-03-26 16:36:19.000000 petrolib-1.2.3/src/petrolib/file_reader.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     7999 2023-03-26 16:32:26.000000 petrolib-1.2.3/src/petrolib/interp.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    58784 2023-03-31 14:02:38.000000 petrolib-1.2.3/src/petrolib/plots.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     6700 2023-03-26 17:09:02.000000 petrolib-1.2.3/src/petrolib/procs.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     5394 2023-03-26 17:12:05.000000 petrolib-1.2.3/src/petrolib/stats.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    57715 2023-03-26 20:12:21.000000 petrolib-1.2.3/src/petrolib/workflow.py
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-03-31 14:07:10.609552 petrolib-1.2.3/src/petrolib.egg-info/
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3680 2023-03-31 14:07:10.000000 petrolib-1.2.3/src/petrolib.egg-info/PKG-INFO
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      343 2023-03-31 14:07:10.000000 petrolib-1.2.3/src/petrolib.egg-info/SOURCES.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        1 2023-03-31 14:07:10.000000 petrolib-1.2.3/src/petrolib.egg-info/dependency_links.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        9 2023-03-31 14:07:10.000000 petrolib-1.2.3/src/petrolib.egg-info/top_level.txt
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.796733 petrolib-1.2.4/
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     1093 2023-03-26 20:57:50.000000 petrolib-1.2.4/LICENSE
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       40 2023-05-01 16:09:25.000000 petrolib-1.2.4/MANIFEST.in
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3759 2023-05-01 16:29:46.792734 petrolib-1.2.4/PKG-INFO
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3137 2023-03-31 13:29:52.000000 petrolib-1.2.4/README.md
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      833 2023-05-01 16:22:17.000000 petrolib-1.2.4/pyproject.toml
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       38 2023-05-01 16:29:46.796733 petrolib-1.2.4/setup.cfg
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      984 2023-05-01 15:58:22.000000 petrolib-1.2.4/setup.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.760735 petrolib-1.2.4/src/
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.764735 petrolib-1.2.4/src/petrolib/
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)       21 2023-05-01 15:30:58.000000 petrolib-1.2.4/src/petrolib/__init__.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.768735 petrolib-1.2.4/src/petrolib/data/
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      286 2023-02-13 04:26:20.000000 petrolib-1.2.4/src/petrolib/data/litho_info.csv
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     4893 2023-05-01 15:44:07.000000 petrolib-1.2.4/src/petrolib/file_reader.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     8001 2023-04-12 22:16:51.000000 petrolib-1.2.4/src/petrolib/interp.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    58756 2023-05-01 16:14:23.000000 petrolib-1.2.4/src/petrolib/plots.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     6786 2023-04-12 22:19:13.000000 petrolib-1.2.4/src/petrolib/procs.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     5394 2023-03-26 17:12:05.000000 petrolib-1.2.4/src/petrolib/stats.py
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      236 2023-05-01 15:40:48.000000 petrolib-1.2.4/src/petrolib/utils.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    57715 2023-03-26 20:12:21.000000 petrolib-1.2.4/src/petrolib/workflow.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 16:29:46.768735 petrolib-1.2.4/src/petrolib.egg-info/
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3759 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/PKG-INFO
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      454 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        1 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       59 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/requires.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        9 2023-05-01 16:29:46.000000 petrolib-1.2.4/src/petrolib.egg-info/top_level.txt
```

### Comparing `petrolib-1.2.3/LICENSE` & `petrolib-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.3/PKG-INFO` & `petrolib-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: petrolib
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python Package for Petrophysical Evaluation
+Home-page: https://github.com/joshua-atolagbe/petrolib
+Author: Joshua Atolagbe
 Author-email: Joshua Atolagbe <atolagbejoshua2@gmail.com>
 Project-URL: Homepage, https://github.com/mayor-of-geology/petrolib
 Project-URL: Bug Tracker, https://github.com/mayor-of-geology/petrolib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Petrophysical Evaluation Package
 
 This is a python package designed to help users perform petrophysical analysis by estimating petrophysical parameters such as:
 ```
```

### Comparing `petrolib-1.2.3/README.md` & `petrolib-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.3/pyproject.toml` & `petrolib-1.2.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 requires = ['matplotlib', 'pandas', 'numpy', 'lasio',
 			'scipy', 'seaborn', 'geopandas', 'contextily'
 		]
 build-backend = "setuptools.build_meta"
 
 [project]			
 name = "petrolib"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
 	{name="Joshua Atolagbe", email="atolagbejoshua2@gmail.com"},	
 ]
 description = "A Python Package for Petrophysical Evaluation"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.5"
 license = {file = "LICENSE.txt"}
 classifiers = [
 		"Programming Language :: Python :: 3",
         	"License :: OSI Approved :: MIT License",
         	"Operating System :: OS Independent",
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/mayor-of-geology/petrolib"
 "Bug Tracker" = "https://github.com/mayor-of-geology/petrolib/issues"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools]
+include-package-data = true
```

### Comparing `petrolib-1.2.3/src/petrolib/file_reader.py` & `petrolib-1.2.4/src/petrolib/file_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 '''
 
 from pathlib import Path
 from warnings import filterwarnings
 filterwarnings('ignore')
 import lasio
 import pandas as pd
+from .utils import MnemonicError
 
 def load_las(file:Path|str, return_csv:bool=False, curves:list|tuple=None) -> lasio.las.LASFile|pd.DataFrame:
 
     '''
     Function to read LAS file
 
     Arguments
@@ -48,15 +49,15 @@
 
     '''
 
     try:
 
         if type(file) == Path:
 
-            exist = file.exists()      
+            assert file.exists(), 'File does not exists'      
 
     except:
 
         raise FileNotFoundError(f'{file} path does not exists.')
 
         # raise TypeError(f'{file} is not a LAS file')
 
@@ -70,34 +71,34 @@
 
         if curves != None:
 
             try:
             
                 for i in curves:
                     
-                    assert i in df.columns, f"'{i}' not found in data."
+                    assert i in df.columns, f"'{i}' not found in log data."
                     
             except:
                 
-                raise AttributeError('Check data. Log curve mnemonic not passed correctly.')
+                raise MnemonicError('Check data. Log curve mnemonic not passed correctly.')
         
             df = df.filter(curves, axis=1)
             
             return df, las
     
         elif curves == None:
             
             return df, las
 
     else:
         
         return las
 
 
-def load_table(file:Path|str, curves:list[str]=None, delimiter:str=None, header:int|list[int]='infer', 
+def load_table(file:Path|str, curves:list[str]=None, delimiter:str=None, header:int|list[int]|str='infer', 
                     skiprows:list|int=None, sheet_name:int|str|list=None) -> pd.DataFrame:
 
     r"""
     Function to load a table data, either csv, tsv, or excel file
 
     Arguments
     ---------
```

### Comparing `petrolib-1.2.3/src/petrolib/interp.py` & `petrolib-1.2.4/src/petrolib/interp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pandas as pd
 from itertools import cycle
 from random import choice
 from matplotlib import pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 
 def crossPlot(df:pd.DataFrame, column_x:str, column_y:str, hue:str=None,
-               color_code:str=None, figsize:slice=(20,7), rhob_fluid:float=1., res_name:str=None, cmap='viridis'):  
+               color_code:str=None, figsize:tuple=(20,7), rhob_fluid:float=1., res_name:str=None, cmap='viridis'):  
 
     r'''
     Plots the cross plot relationship of density against porosity on compatible scales
     to facilitate in identification of reservoir type and its fluid type.
 
     Reference
     ---------
@@ -41,15 +41,15 @@
     hue : str 
         Column to color code the scatter plot by
         
     color_code : str default None
         Color code typing. If 'num', arg `hue` must be a continuous column.
         If 'cat', argument `hue` must be a categorical column
 
-    figsize : slice
+    figsize : tuple
         Size of plot
 
     rhob_fluid : float, default 1.0
         Fluid density
     
     res_name : str
         Reservoir name
@@ -130,15 +130,15 @@
     plt.ylim(3, 1.3)
     plt.xlabel('$\phi (m3/m3) $',fontsize=18); plt.ylabel(r'$\rho (g/cm3)$', fontsize=18)
     plt.show()
 
 
 
 def picketPlot(df:pd.DataFrame, rt:str='RT', por:str='NPHI', rwa:float=0.018,
-                a:float=1., m:float=1.8, n:float=2., res_name:str=None, figsize:slice=(20, 8),
+                a:float=1., m:float=1.8, n:float=2., res_name:str=None, figsize:tuple=(20, 8),
                hue:str=None, color_code:str=None, cmap=None):
     
     r'''
 
     Plot Pickett plot based on a pattern recognition approach to solving Archie’s equation. The resistivity
     and porosity logs are plotted on a logarithmic scales to evaluate formation characteristics of conventional, granular reservoirs.
     Read more here: https://wiki.seg.org/wiki/Pickett_plot
@@ -162,15 +162,15 @@
 
     n : float default 2.
         Saturation exponent
 
     res_name : str 
         Reservoir/Zone name
 
-    figsize : slice
+    figsize : tuple
         Size of plot
 
     hue : str 
         Column to color code the scatter plot by.
         
     color_code : str default None
         Color code typing. If 'num', arg `hue` must be a continuous column
@@ -239,8 +239,8 @@
             rt_result = ((a*rwa)/(sw[i]**n)/(phi[j]**m))
             rt[i,j] = rt_result     
 
     for i in range(0,len(sw)):
         plt.plot(rt[i], phi, label=str(int(sw[i]*100))+'%')
         plt.legend(loc='best')
     
-    plt.show()
+    plt.show()
```

### Comparing `petrolib-1.2.3/src/petrolib/plots.py` & `petrolib-1.2.4/src/petrolib/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,35 +8,34 @@
 Function
 --------
 plotLoc
 tripleCombo
 plotLog
 plotZoneCombo
 plotLogFacies
-plotLogs_
+plotLogs
 '''
 
 
 import numpy as np
 import lasio
 import csv
 import pandas as pd
 import contextily as ctx
 import geopandas as gpd 
 import os
-from pkg_resources import resource_filename
 from itertools import cycle
 from pathlib import Path
 from random import choice
 from matplotlib import pyplot as plt
 from typing import *
 from random import choice
 from matplotlib.patches import Patch 
 
-def plotLoc(data:list[lasio.las.LASFile], shape_file:Path=None, area:str=None, figsize:slice=(7, 7),
+def plotLoc(data:list[lasio.las.LASFile], shape_file:Path=None, area:str=None, figsize:tuple=(7, 7),
              label:list=None, withmap:bool=False, return_table:bool=False) -> pd.DataFrame|None:
     
     '''
     Plots location of wells
     The longitude and latitude must be available in th LAS fils
     
     Arguments
@@ -48,15 +47,15 @@
     shape_file : str, default None
         A .shp, .shx or .dbf file containing the shape file of the area where the well is located
         If not supplied, `area` must be passed
 
     area : str default, None
         Well location. Must inlcude area from `gpd.datasets.get_path('naturalearth_lowres')`
 
-    figsize : slice
+    figsize : tuple
         Size of plot
 
     label : list of str
         Well name(s). Must be a list of equal length with `data`
 
     withmap : bool default False  
         Plots location of wells on a map if True
@@ -167,15 +166,15 @@
 
         pass
 
 
 
 def tripleCombo(data:pd.DataFrame, depth:str, gr:str, res:str, nphi:str, rhob:str, ztop:float, zbot:float, 
                 res_thres:float=10.0, fill:str=None, palette_op:str=None,
-                limit:str=None, figsize:slice=(9, 10), title:str='Three Combo Log Plot') -> None:
+                limit:str=None, figsize:tuple=(9, 10), title:str='Three Combo Log Plot') -> None:
     
     r'''
     Plots a three combo log of well data
 
     Arguments
     --------
 
@@ -218,15 +217,15 @@
     palette_op : str optional 
         Palette option to fill gamma ray log
 
     limit : str default None
         Tells which side to fill the gamma ray track, ['left', 'right']
         lf None, it's filled in both sides delineating shale-sand region
 
-    figsize : slice
+    figsize : tuple
         Size of plot
     
     title : str
         Title of plot
 
     Example
     -------
@@ -457,15 +456,15 @@
         Example
         -------
         >>> ztop, zbot, zn, fm = zones()
         
         '''
         return self._ztop, self._zbot, self._zonename, self._fm_mid
 
-    def plotZone(self, depth:str, logs:List[str], top:float, bottom:float, title:str='Log Plot', figsize:slice=(8, 12)):
+    def plotZone(self, depth:str, logs:List[str], top:float, bottom:float, title:str='Log Plot', figsize:tuple=(8, 12)):
 
         r'''
         Plots log curves with zonation track.
 
         Attributes
         ----------
 
@@ -480,15 +479,15 @@
 
         bottom : float
             Maximum depth to zoom on
 
         title : str
             Plot title
 
-        figsize : slice
+        figsize : tuple
             Size of plot
 
         Example
         -------
         >>> Zonation.plotZone('DEPTH', ['GR', 'RT', 'RHOB', 'NPHI', 'CALI'], 3300, 3600, 'Volve')
         
         '''
@@ -551,15 +550,15 @@
                     fontsize='large')
     #    
         plt.tight_layout(h_pad=1)
         fig.subplots_adjust(wspace = 0.04)
         plt.show()
 
 
-def plotLog(df:pd.DataFrame, depth:str, logs:List[str], top:float, bottom:float, title:str='Log Plot', figsize:slice=(8, 12)):
+def plotLog(df:pd.DataFrame, depth:str, logs:List[str], top:float, bottom:float, title:str='Log Plot', figsize:tuple=(8, 12)):
 
         r'''
         Plots log curves singly. To plot overlay plots use `plots.plotLogs_` or `plots.plotLogFacies`
 
         Argument
         --------
         df : pd.DataFrame
@@ -576,15 +575,15 @@
 
         bottom : float
             Maximum depth to zoom on
 
         title : str
             Plot title
 
-        figsize : slice
+        figsize : tuple
             Size of plot
 
         Example
         -------
         >>> import petrolib.plots.plotLog
         >>> plotLog('DEPTH', ['GR', 'RT', 'RHOB', 'NPHI', 'CALI'], 3300, 3600, 'Volve')
         >>> plotLog(df,'DEPTH', ['NPHI'], 2751, 2834.58, 'Fre-1')
@@ -597,15 +596,15 @@
 
         cycol = cycle('bgrcmyk')
         color = [choice(next(cycol)) for i in range(len(logs))]
         np.random.shuffle(color)
 
         if len(logs) > 1:
             for i in range(len(logs)):
-
+                np.random.shuffle(color)
                 if logs[i] == 'RT' or logs[i] == 'ILD':
                     # for resistivity, semilog plot
                     ax[i].semilogx(df[logs[i]], df[depth], color=color[i])
                 else:
                     # for non-resistivity, normal plot
                     ax[i].plot(df[logs[i]], df[depth], color=color[i])
 
@@ -622,14 +621,15 @@
                 ax[i].spines['top'].set_edgecolor(color[i])
                 ax[i].spines["top"].set_position(("axes", 1.02)); ax[i].xaxis.set_ticks_position("top")
                 ax[i].xaxis.set_label_position("top")
         
         elif len(logs) == 1:
             
             for i in logs:
+                np.random.shuffle(color)
                 if i == 'RT' or i == 'ILD':
                     # for resistivity, semilog plot
                     plt.semilogx(df[i], df[depth], color=next(cycol))
                 else:
                         # for non-resistivity, normal plot
                     plt.plot(df[i], df[depth], color=next(cycol))
 
@@ -646,15 +646,15 @@
         fig.subplots_adjust(wspace = 0.02)
         plt.show()
 
 
     
 def plotZoneCombo(data:pd.DataFrame, depth:str, gr:str, res:str, nphi:str, rhob:str, ztop:float, zbot:float,
                    ztops:List[float], zbots:List[float], zonename:List[str], limit:str, res_thres:float=10., 
-                   palette_op:str=None, fill:str=None, title:str='Log plot', figsize:slice=(10, 20)) -> None:
+                   palette_op:str=None, fill:str=None, title:str='Log plot', figsize:tuple=(10, 20)) -> None:
     
     r'''
     Function for plotting three combo logs alongside the zonation/reservoir track
 
     Arguments
     --------
 
@@ -706,15 +706,15 @@
         Can either be ['left', 'right', 'both']
 
         * default None - show neither of the porous nor non-porous zones
         * 'left' - shows only porous zones
         * 'right' - shows only non-porous zones
         * 'both' - shows both porous and non-porous zones
 
-    figsize : slice
+    figsize : tuple
         Size of plot
         
     Example
     -------
     >>> from petrolib.plots import plotZoneCombo
     >>> plotZoneCombo(well11, 'DEPTH', 'GR', 'RT', 'NPHI', 'RHOB', min(ztop), max(zbot),
                ztop, zbot, zn, fill='both', limit=None, figsize=(13, 30), title='ATAGA-11')
@@ -888,15 +888,15 @@
                 fontsize='large')
             
     plt.tight_layout(h_pad=1.2)
     fig.subplots_adjust(wspace = 0.0)
 
 
 def plotLogFacies(df:pd.DataFrame, depth:str, logs:List[list], top:float, bottom:float, facies:str=None,  
-                  title:str='Log Plot', figsize:slice=(8, 12)):
+                  title:str='Log Plot', figsize:tuple=(8, 12)):
 
     r'''
     
     Plots overlayed/super-imposed log curves along with the facies. 
 
     Argument
     --------
@@ -919,31 +919,29 @@
         Facies columns. Supported facies include :
             ['Sandstone', 'Sandstone/Shale', 'Shale', 'Marl', 'Dolomite', 'Limestone',
             'Chalk', 'Halite', 'Anhydrite', 'Tuff', 'Coal', 'Basement']
 
     title : str
         Plot title
 
-    figsize : slice
+    figsize : tuple
         Size of plot
 
     Example
     -------
     >>> from petrolib.plots import *
     >>> plotLogFacies(well11, 'DEPTH', ['GR', 'RT', ['RHOB', 'NPHI']], facies='litho', top=well11.DEPTH.min(),
                             bottom=well11.DEPTH.max(), figsize=(9, 12), title='15-9-F1A')
 
     '''    
 
     df = df.copy()
     # file_dir, file_name = os.path.split(__file__)
     
-    # df_litho = pd.read_csv(os.path.join(file_dir, 'data', 'Litho info.csv'))
-
-    df_litho = pd.read_csv(resource_filename(__name__, 'data/Litho info.csv'))
+    df_litho = pd.read_csv(os.path.join(os.path.dirname(__file__), 'data', 'litho_info.csv'))
     
     # create the subplots; ncols equals the number of logs
     if facies is None:
         fig, ax = plt.subplots(nrows=1, ncols=len(logs), figsize=figsize, sharey=True)
     else:
         fig, ax = plt.subplots(nrows=1, ncols=len(logs)+1, figsize=figsize, sharey=True)
 
@@ -1247,15 +1245,15 @@
     plt.tight_layout(h_pad=1)
     fig.subplots_adjust(wspace = 0.04)
 
     plt.show()
 
 
 def plotLogs(df:pd.DataFrame, depth:str, logs:List[List[str]], top:float, bottom:float,  
-                  title:str='Log Plot', figsize:slice=(8, 12)):
+                  title:str='Log Plot', figsize:tuple=(8, 12)):
 
     r'''
     
     Plots overlayed/super-imposed log curves. 
 
     Argument
     --------
@@ -1273,15 +1271,15 @@
 
     bottom : float
         Maximum depth to zoom on
 
     title : str
         Plot title
 
-    figsize : slice
+    figsize : tuple
         Size of plot
 
     Example
     -------
     >>> plotLogs_(well11, 'DEPTH', ['GR', 'RT', ['RHOB', 'NPHI']], top=well11.DEPTH.min(),
                             bottom=well11.DEPTH.max(), figsize=(9, 12), title='15-9-F1A')
 
@@ -1469,8 +1467,8 @@
                     axes.patch.set_visible(False)
                     axes.invert_yaxis()
                     additive += 0.06
 
     plt.tight_layout(h_pad=1)
     fig.subplots_adjust(wspace = 0.04)
 
-    plt.show()
+    plt.show()
```

### Comparing `petrolib-1.2.3/src/petrolib/procs.py` & `petrolib-1.2.4/src/petrolib/procs.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 '''
 
 from warnings import filterwarnings
 filterwarnings('ignore')
 import pandas as pd
 import numpy as np
+from typing import Optional
 
 
-def set_alias(df, DEPTH, GR, RT, NPHI, RHOB, DT=None) -> pd.DataFrame:
+def set_alias(df:pd.DataFrame, DEPTH:str, GR:str, RT:str, NPHI:str, RHOB:str, DT:Optional[str]=None) -> pd.DataFrame:
 
     r'''
     Function to rename the log curves in order to maintain petrophysics conventions
 
     Arguments
     ---------
 
@@ -64,15 +65,15 @@
     else:
         dataframe = df.rename({DEPTH:'DEPTH', GR:'GR', RT:'RT', 
                         NPHI:'NPHI', RHOB:'RHOB'}, axis=1)
 
     return dataframe
 
 
-def process_data(df:pd.DataFrame, gr:str, rt:str, nphi:str, rhob:str, dt:str=None, trim:str='both') -> pd.DataFrame:
+def process_data(df:pd.DataFrame, gr:str, rt:str, nphi:str, rhob:str, dt:Optional[str]=None, trim:str='both') -> pd.DataFrame:
 
     r'''
     Function to preprocess data before beginning petrophysics workflow.
     This processing workflow uses conventional values for the log curves. 
     To use user-defined preprocessing method , refer to the `petrolib.data.procs.trim()`
 
     Arguments
```

### Comparing `petrolib-1.2.3/src/petrolib/stats.py` & `petrolib-1.2.4/src/petrolib/stats.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.3/src/petrolib/workflow.py` & `petrolib-1.2.4/src/petrolib/workflow.py`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.3/src/petrolib.egg-info/PKG-INFO` & `petrolib-1.2.4/src/petrolib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: petrolib
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python Package for Petrophysical Evaluation
+Home-page: https://github.com/joshua-atolagbe/petrolib
+Author: Joshua Atolagbe
 Author-email: Joshua Atolagbe <atolagbejoshua2@gmail.com>
 Project-URL: Homepage, https://github.com/mayor-of-geology/petrolib
 Project-URL: Bug Tracker, https://github.com/mayor-of-geology/petrolib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Petrophysical Evaluation Package
 
 This is a python package designed to help users perform petrophysical analysis by estimating petrophysical parameters such as:
 ```
```

