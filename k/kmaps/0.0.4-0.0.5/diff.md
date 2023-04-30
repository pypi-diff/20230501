# Comparing `tmp/kmaps-0.0.4.tar.gz` & `tmp/kmaps-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmaps-0.0.4.tar", last modified: Thu Apr 20 14:45:12 2023, max compression
+gzip compressed data, was "kmaps-0.0.5.tar", last modified: Sun Apr 30 23:14:24 2023, max compression
```

## Comparing `kmaps-0.0.4.tar` & `kmaps-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:45:12.180660 kmaps-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 14:44:59.000000 kmaps-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 14:44:59.000000 kmaps-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 14:45:12.180660 kmaps-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-20 14:44:59.000000 kmaps-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:45:12.176660 kmaps-0.0.4/kmaps/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 14:45:00.000000 kmaps-0.0.4/kmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-20 14:45:00.000000 kmaps-0.0.4/kmaps/folium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-20 14:45:00.000000 kmaps-0.0.4/kmaps/kmaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:45:12.176660 kmaps-0.0.4/kmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 14:45:12.000000 kmaps-0.0.4/kmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 14:45:00.000000 kmaps-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 14:45:12.180660 kmaps-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-20 14:45:00.000000 kmaps-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:14:24.668315 kmaps-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-30 23:14:15.000000 kmaps-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-30 23:14:15.000000 kmaps-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-30 23:14:24.668315 kmaps-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 23:14:15.000000 kmaps-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:14:24.668315 kmaps-0.0.5/kmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 23:14:15.000000 kmaps-0.0.5/kmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-30 23:14:15.000000 kmaps-0.0.5/kmaps/folmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-04-30 23:14:15.000000 kmaps-0.0.5/kmaps/kmaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:14:24.668315 kmaps-0.0.5/kmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-30 23:14:24.000000 kmaps-0.0.5/kmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-30 23:14:24.000000 kmaps-0.0.5/kmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 23:14:24.000000 kmaps-0.0.5/kmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 23:14:24.000000 kmaps-0.0.5/kmaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 23:14:24.000000 kmaps-0.0.5/kmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 23:14:24.000000 kmaps-0.0.5/kmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 23:14:15.000000 kmaps-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-30 23:14:24.668315 kmaps-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-30 23:14:15.000000 kmaps-0.0.5/setup.py
```

### Comparing `kmaps-0.0.4/LICENSE` & `kmaps-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.4/PKG-INFO` & `kmaps-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmaps
-Version: 0.0.4
+Version: 0.0.5
 Summary: TBA
 Home-page: https://github.com/ChangwhaOh/kmaps
 Author: Changwha Oh
 Author-email: coh4@vols.utk.edu
 License: MIT license
 Keywords: kmaps
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kmaps-0.0.4/README.md` & `kmaps-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.4/kmaps/folium.py` & `kmaps-0.0.5/kmaps/folmaps.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     Args:
         folium (_type_): Map object from folium.
     """
     def __init__(self, location = [37.5, 127], zoom_start = 8, **kwargs): 
         """Create a Map.
 
         Args:
-            center (list, optional): A coordinate representing the center of the map. Defaults to `[37.5, 127]`
-            zoom (int, optional): Zoom level. Defaults to 8
+            location (list, optional): A coordinate representing the center of the map. Defaults to `[37.5, 127]`
+            zoom_start (int, optional): Zoom level. Defaults to 8
         """            
         if 'scroll_wheel_zoom' not in kwargs:
             kwargs['scroll_wheel_zoom'] = True
         super().__init__(location = location, zoom_start = zoom_start, **kwargs) # inherited from the parent, in this case, ipyleaflet
 
 
     def add_layers_control(self, **kwargs):
@@ -44,8 +44,26 @@
         Args:
             data (str): A name of the shape file.
             name (str, optional): A layer name of the shape file to be displayed on the map. Defaults to 'Shapefile'.
         """
         import geopandas as gpd
         gdf = gpd.read_file(data)
         geojson = gdf.__geo_interface__
-        self.add_geojson(geojson, name = name, **kwargs)
+        self.add_geojson(geojson, name = name, **kwargs)
+    
+
+    def add_tile_layer(self, url, name, attr = 'Tile', **kwargs):
+        """Add a tile layer to the map.
+
+        Args:
+            url (str): xyz url of the tile layer.
+            name (str): A name of the layer that would be displayed on the map.
+            attr (str, optional): A name of the attribution. Defaults to 'Tile'.
+        """        
+        tile_layer = folium.TileLayer(
+            tiles = url,
+            name = name,
+            attr = attr,
+            **kwargs
+        )
+
+        self.add_child(tile_layer)
```

### Comparing `kmaps-0.0.4/kmaps.egg-info/PKG-INFO` & `kmaps-0.0.5/kmaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmaps
-Version: 0.0.4
+Version: 0.0.5
 Summary: TBA
 Home-page: https://github.com/ChangwhaOh/kmaps
 Author: Changwha Oh
 Author-email: coh4@vols.utk.edu
 License: MIT license
 Keywords: kmaps
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kmaps-0.0.4/setup.py` & `kmaps-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='kmaps',
     name='kmaps',
     packages=find_packages(include=['kmaps', 'kmaps.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChangwhaOh/kmaps',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

