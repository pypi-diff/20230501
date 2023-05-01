# Comparing `tmp/afloat-0.0.3.tar.gz` & `tmp/afloat-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afloat-0.0.3.tar", last modified: Mon May  1 13:19:56 2023, max compression
+gzip compressed data, was "afloat-0.0.3.dev0.tar", last modified: Wed Feb  8 07:48:50 2023, max compression
```

## Comparing `afloat-0.0.3.tar` & `afloat-0.0.3.dev0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:19:56.545796 afloat-0.0.3/
--rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      239 2023-05-01 13:19:56.543800 afloat-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 13:19:56.521793 afloat-0.0.3/afloat/
--rw-rw-rw-   0        0        0       98 2022-08-09 14:36:08.000000 afloat-0.0.3/afloat/__init__.py
--rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.3/afloat/bottom_lander.py
--rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.3/afloat/clean.py
--rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.3/afloat/currents.py
--rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.3/afloat/netcdf.py
--rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.0.3/afloat/operational.py
--rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.3/afloat/pca.py
--rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.0.3/afloat/sentinel.py
--rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.3/afloat/shape.py
--rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.3/afloat/time.py
--rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.3/afloat/timeseries.py
--rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.3/afloat/xr.py
--rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.3/afloat/xrwrap.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:19:56.537796 afloat-0.0.3/afloat.egg-info/
--rw-rw-rw-   0        0        0      239 2023-05-01 13:19:56.000000 afloat-0.0.3/afloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-05-01 13:19:56.000000 afloat-0.0.3/afloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:19:56.000000 afloat-0.0.3/afloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-01 13:19:56.000000 afloat-0.0.3/afloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 13:19:56.000000 afloat-0.0.3/afloat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 13:19:56.545796 afloat-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-05-01 13:19:20.000000 afloat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-08 07:48:50.466619 afloat-0.0.3.dev0/
+-rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.3.dev0/LICENSE
+-rw-rw-rw-   0        0        0      244 2023-02-08 07:48:50.465619 afloat-0.0.3.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.3.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-02-08 07:48:50.361637 afloat-0.0.3.dev0/afloat/
+-rw-rw-rw-   0        0        0       98 2022-08-09 14:36:08.000000 afloat-0.0.3.dev0/afloat/__init__.py
+-rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.3.dev0/afloat/bottom_lander.py
+-rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.3.dev0/afloat/clean.py
+-rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.3.dev0/afloat/currents.py
+-rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.3.dev0/afloat/netcdf.py
+-rw-rw-rw-   0        0        0     5125 2023-01-19 00:06:21.000000 afloat-0.0.3.dev0/afloat/operational.py
+-rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.3.dev0/afloat/pca.py
+-rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.3.dev0/afloat/shape.py
+-rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.3.dev0/afloat/time.py
+-rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.3.dev0/afloat/timeseries.py
+-rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.3.dev0/afloat/xr.py
+-rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.3.dev0/afloat/xrwrap.py
+drwxrwxrwx   0        0        0        0 2023-02-08 07:48:50.464625 afloat-0.0.3.dev0/afloat.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-02-08 07:48:48.000000 afloat-0.0.3.dev0/afloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-02-08 07:48:49.000000 afloat-0.0.3.dev0/afloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-08 07:48:48.000000 afloat-0.0.3.dev0/afloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-02-08 07:48:48.000000 afloat-0.0.3.dev0/afloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-02-08 07:48:48.000000 afloat-0.0.3.dev0/afloat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-08 07:48:50.467633 afloat-0.0.3.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-02-08 07:46:02.000000 afloat-0.0.3.dev0/setup.py
```

### Comparing `afloat-0.0.3/LICENSE` & `afloat-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/README.md` & `afloat-0.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/bottom_lander.py` & `afloat-0.0.3.dev0/afloat/bottom_lander.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/clean.py` & `afloat-0.0.3.dev0/afloat/clean.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/currents.py` & `afloat-0.0.3.dev0/afloat/currents.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/netcdf.py` & `afloat-0.0.3.dev0/afloat/netcdf.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/operational.py` & `afloat-0.0.3.dev0/afloat/operational.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 """
 
 import numpy as np 
 import matplotlib.pyplot as plt
 import scipy.optimize
 import utm
 
-import gpxpy
-import gpxpy.gpx
-
 def triangulate(x, 
                 y, 
                 ranges, 
                 total_depth,
                 responder_height,
                 x_drop=None,
                 y_drop=None, 
@@ -67,22 +64,18 @@
     got_drop=False
     if not y_drop is None:
         if not x_drop is None:
             got_drop=True
             
     if coord_sys == 'latlon':
         if got_drop:
-            x_drop, y_drop, zone1, zone2 = utm.from_latlon(y_drop, x_drop)
+            x_drop, y_drop, blank, blank = utm.from_latlon(y_drop, x_drop)
 
         for ii, (xi, yi) in enumerate(zip(x, y)):#np.arange(0, len(x_extra)):
-            x[ii], y[ii], zone1, zone2 = utm.from_latlon(y[ii], x[ii])
-
-    print('UTM Zone: {0:.0f}, {1:s}'.format(zone1, zone2)) 
-    # print(zone1)
-    # print(zone2)
+            x[ii], y[ii], blank, blank = utm.from_latlon(y[ii], x[ii])
 
     # Only triangulates ont the first 3...
     r1 = np.sqrt(np.power(ranges[0], 2) - np.power(vert_disp, 2))
     r2 = np.sqrt(np.power(ranges[1], 2) - np.power(vert_disp, 2))
     r3 = np.sqrt(np.power(ranges[2], 2) - np.power(vert_disp, 2))
 
     # ... others are 'extra' and are plotted but not used
@@ -124,16 +117,15 @@
         x0 = [x_drop, y_drop]
     else:
         print('Initial guess taken as average of all marks, regardless of range.')
         x0 = [np.mean(x), np.mean(y)]
         print(x0)
         
     locale = scipy.optimize.fmin(func=fh, x0=x0)
-    # lat, long = utm.to_latlon(locale[0], locale[1], 50, 'K')
-    lat, long = utm.to_latlon(locale[0], locale[1], zone1, zone2)
+    lat, long = utm.to_latlon(locale[0], locale[1], 50, 'K')
 
     foundh, = plt.plot(locale[0], locale[1], 'gx', label='Solution')
 
 #     if got_drop:
 #         d = calculate_distance(locale, verbose = True)
 #         textt = name + ': {0:.0f}, {1:.0f} [error: {2:.0f} m]'.format(locale[0], locale[1], d)
 #         textt = name + ': {0:.5f}, {1:.5f} [error: {2:.0f} m]'.format(lat, long, d)
@@ -154,80 +146,8 @@
 #     axes.legend()
     handles, labels = axes.get_legend_handles_labels()
     by_label = dict(zip(labels, handles))
     axes.legend(by_label.values(), by_label.keys(), loc='center left', bbox_to_anchor=(1, 0.5))
 
     fullpathsave = '{name} Triangulation.png'.format(name=name)
     fig.savefig(fullpathsave)  
-    
-    return [lat, long], locale
-
-
-class mygpx():
-    """
-    Parser/handler for GPX ship tracks which has seen very little testing. 
-    """
-
-    # Shouldn't import like this, but going for it!
-    
-
-    def __init__(self, gpxfgile):
-
-        self.gpxfgile = gpxfgile
-        self.read()
-        self.process()
-        
-    def read(self):
-        
-        f = open(self.gpxfgile, 'r')
-        print('File open')
-
-        gpx = gpxpy.parse(f)
-        print('File parsed')
-        
-        self.gpx = gpx
-        
-    def process(self):
-
-        gpx_x = []
-        gpx_y = []
-        gpx_z = []
-        gpx_t = []
-
-        for track in self.gpx.tracks:
-            for segment in track.segments:
-                
-                x = np.array([point.longitude for point in segment.points])
-                y = np.array([point.latitude for point in segment.points])
-                z = np.array([point.elevation for point in segment.points])
-                t = np.array([point.time for point in segment.points])
-
-                gpx_x += [x]
-                gpx_y += [y]
-                gpx_z += [z]
-                gpx_t += [t]
-                
-        
-        self.gpx_x = gpx_x
-        self.gpx_y = gpx_y
-        self.gpx_z = gpx_z
-        self.gpx_t = gpx_t
-        
-        #         for point in segment.points:
-        #             print('Point at ({0},{1}) -> {2}'.format(point.latitude, point.longitude, point.elevation))
-
-        # for waypoint in gpx.waypoints:
-        #     print('waypoint {0} -> ({1},{2})'.format(waypoint.name, waypoint.latitude, waypoint.longitude))
-
-        # for route in gpx.routes:
-        #     print('Route:')
-        #     for point in route.points:
-        #         print('Point at ({0},{1}) -> {2}'.format(point.latitude, point.longitude, point.elevation))
-
-# parse_solander_gpx(gpxfgile)
-    def plot_gpx(self, plot_dict={}):
-
-        for x, y in zip(self.gpx_x, self.gpx_y):
-            plt.plot(x, y, linewidth=0.5, alpha=0.5)
-
-        plt.gca().set_aspect('equal')
```

### Comparing `afloat-0.0.3/afloat/pca.py` & `afloat-0.0.3.dev0/afloat/pca.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/shape.py` & `afloat-0.0.3.dev0/afloat/shape.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/time.py` & `afloat-0.0.3.dev0/afloat/time.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/timeseries.py` & `afloat-0.0.3.dev0/afloat/timeseries.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/xr.py` & `afloat-0.0.3.dev0/afloat/xr.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/afloat/xrwrap.py` & `afloat-0.0.3.dev0/afloat/xrwrap.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.3/setup.py` & `afloat-0.0.3.dev0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class BinaryDistribution(Distribution):
     def is_pure(self):
         return False
 
 		
 setup(name='afloat',
-      version='0.0.3',
+      version='0.0.3.dev0',
       description='A Fairly useful Library of Ocean Analysis Tools',
       author='Andrew Zulberti',
       author_email='andrew.zulberti@gmail.com',
       packages=find_packages(),
       install_requires=['numpy',
                         'matplotlib', 
                         'netcdf4',
```

