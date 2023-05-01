# Comparing `tmp/napari-clusters-plotter-0.7.0.tar.gz` & `tmp/napari-clusters-plotter-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-clusters-plotter-0.7.0.tar", last modified: Sat Apr 29 18:02:12 2023, max compression
+gzip compressed data, was "napari-clusters-plotter-0.7.1.tar", last modified: Mon May  1 07:37:46 2023, max compression
```

## Comparing `napari-clusters-plotter-0.7.0.tar` & `napari-clusters-plotter-0.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.717066 napari-clusters-plotter-0.7.0/
--rw-rw-rw-   0        0        0     1642 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/LICENSE
--rw-rw-rw-   0        0        0      127 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0    15617 2023-04-29 18:02:12.717066 napari-clusters-plotter-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    14228 2023-04-29 17:52:49.000000 napari-clusters-plotter-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.671663 napari-clusters-plotter-0.7.0/napari_clusters_plotter/
--rw-rw-rw-   0        0        0    24305 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_Qt_code.py
--rw-rw-rw-   0        0        0      184 2023-04-29 17:56:31.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/__init__.py
--rw-rw-rw-   0        0        0    21295 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_clustering.py
--rw-rw-rw-   0        0        0    37507 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_dimensionality_reduction.py
--rw-rw-rw-   0        0        0      406 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_dock_widget.py
--rw-rw-rw-   0        0        0    33249 2023-04-29 17:16:06.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter.py
--rw-rw-rw-   0        0        0    17769 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.705752 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/
--rw-rw-rw-   0        0        0        0 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/__init__.py
--rw-rw-rw-   0        0        0     7838 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_clustering.py
--rw-rw-rw-   0        0        0     7373 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dimension_reduction.py
--rw-rw-rw-   0        0        0     2457 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dock_widget.py
--rw-rw-rw-   0        0        0     6619 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_plotter.py
--rw-rw-rw-   0        0        0     5256 2023-03-16 15:33:04.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_utils.py
--rw-rw-rw-   0        0        0    15576 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.716063 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/
--rw-rw-rw-   0        0        0     6680 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Back.png
--rw-rw-rw-   0        0        0     6951 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Customize.png
--rw-rw-rw-   0        0        0     6535 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Forward.png
--rw-rw-rw-   0        0        0     7143 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Home.png
--rw-rw-rw-   0        0        0     7114 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan.png
--rw-rw-rw-   0        0        0    11810 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan_checked.png
--rw-rw-rw-   0        0        0     7381 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Save.png
--rw-rw-rw-   0        0        0     6739 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Subplots.png
--rw-rw-rw-   0        0        0     8064 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom.png
--rw-rw-rw-   0        0        0    12372 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom_checked.png
-drwxrwxrwx   0        0        0        0 2023-04-29 18:02:12.699737 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/
--rw-rw-rw-   0        0        0    15617 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1384 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-29 18:02:12.000000 napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.0/requirements.txt
--rw-rw-rw-   0        0        0     1928 2023-04-29 18:02:12.719071 napari-clusters-plotter-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      117 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.820173 napari-clusters-plotter-0.7.1/
+-rw-rw-rw-   0        0        0     1642 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    15617 2023-05-01 07:37:46.820173 napari-clusters-plotter-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14228 2023-04-29 17:52:49.000000 napari-clusters-plotter-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.776058 napari-clusters-plotter-0.7.1/napari_clusters_plotter/
+-rw-rw-rw-   0        0        0    24305 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_Qt_code.py
+-rw-rw-rw-   0        0        0      184 2023-05-01 07:35:45.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/__init__.py
+-rw-rw-rw-   0        0        0    21295 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_clustering.py
+-rw-rw-rw-   0        0        0    37507 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_dimensionality_reduction.py
+-rw-rw-rw-   0        0        0      406 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_dock_widget.py
+-rw-rw-rw-   0        0        0    33249 2023-04-29 17:16:06.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter.py
+-rw-rw-rw-   0        0        0    17769 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.804131 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/
+-rw-rw-rw-   0        0        0        0 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/__init__.py
+-rw-rw-rw-   0        0        0     7838 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_clustering.py
+-rw-rw-rw-   0        0        0     7373 2023-04-29 16:40:07.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dimension_reduction.py
+-rw-rw-rw-   0        0        0     2457 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dock_widget.py
+-rw-rw-rw-   0        0        0     6619 2023-04-29 17:14:10.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_plotter.py
+-rw-rw-rw-   0        0        0     5256 2023-03-16 15:33:04.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_utils.py
+-rw-rw-rw-   0        0        0    15576 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.819171 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/
+-rw-rw-rw-   0        0        0     6680 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Back.png
+-rw-rw-rw-   0        0        0     6951 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Customize.png
+-rw-rw-rw-   0        0        0     6535 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Forward.png
+-rw-rw-rw-   0        0        0     7143 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Home.png
+-rw-rw-rw-   0        0        0     7114 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan.png
+-rw-rw-rw-   0        0        0    11810 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan_checked.png
+-rw-rw-rw-   0        0        0     7381 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Save.png
+-rw-rw-rw-   0        0        0     6739 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Subplots.png
+-rw-rw-rw-   0        0        0     8064 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom.png
+-rw-rw-rw-   0        0        0    12372 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom_checked.png
+drwxrwxrwx   0        0        0        0 2023-05-01 07:37:46.797113 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/
+-rw-rw-rw-   0        0        0    15617 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1384 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-01 07:37:46.000000 napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2023-04-13 08:01:20.000000 napari-clusters-plotter-0.7.1/requirements.txt
+-rw-rw-rw-   0        0        0     1928 2023-05-01 07:37:46.822179 napari-clusters-plotter-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      117 2023-03-16 08:21:53.000000 napari-clusters-plotter-0.7.1/setup.py
```

### Comparing `napari-clusters-plotter-0.7.0/LICENSE` & `napari-clusters-plotter-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/PKG-INFO` & `napari-clusters-plotter-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-clusters-plotter
-Version: 0.7.0
+Version: 0.7.1
 Summary: A plugin to use with napari for clustering objects according to their properties
 Home-page: https://github.com/BiAPoL/napari-clusters-plotter
 Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
 Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
```

### Comparing `napari-clusters-plotter-0.7.0/README.md` & `napari-clusters-plotter-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_Qt_code.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_Qt_code.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_clustering.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_clustering.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_dimensionality_reduction.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_plotter_utilities.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_plotter_utilities.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_clustering.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dimension_reduction.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_dock_widget.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_plotter.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_tests/test_utils.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/_utilities.py` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/_utilities.py`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Back.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Back.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Customize.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Customize.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Forward.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Forward.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Home.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Home.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Pan_checked.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Save.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Save.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Subplots.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter/icons/Zoom_checked.png` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter/icons/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/PKG-INFO` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-clusters-plotter
-Version: 0.7.0
+Version: 0.7.1
 Summary: A plugin to use with napari for clustering objects according to their properties
 Home-page: https://github.com/BiAPoL/napari-clusters-plotter
 Author: Laura Zigutyte, Ryan Savill, Johannes Müller, Marcelo Zoccoler, Robert Haase
 Author-email: zigutyte@gmail.com, robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/BiAPoL/napari-clusters-plotter/issues
 Project-URL: Documentation, https://github.com/BiAPoL/napari-clusters-plotter
```

### Comparing `napari-clusters-plotter-0.7.0/napari_clusters_plotter.egg-info/SOURCES.txt` & `napari-clusters-plotter-0.7.1/napari_clusters_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/requirements.txt` & `napari-clusters-plotter-0.7.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `napari-clusters-plotter-0.7.0/setup.cfg` & `napari-clusters-plotter-0.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 636c 7573 7465   = napari-cluste
 00000020: 7273 2d70 6c6f 7474 6572 0d0a 7665 7273  rs-plotter..vers
-00000030: 696f 6e20 3d20 302e 372e 300d 0a61 7574  ion = 0.7.0..aut
+00000030: 696f 6e20 3d20 302e 372e 310d 0a61 7574  ion = 0.7.1..aut
 00000040: 686f 7220 3d20 4c61 7572 6120 5a69 6775  hor = Laura Zigu
 00000050: 7479 7465 2c20 5279 616e 2053 6176 696c  tyte, Ryan Savil
 00000060: 6c2c 204a 6f68 616e 6e65 7320 4dc3 bc6c  l, Johannes M..l
 00000070: 6c65 722c 204d 6172 6365 6c6f 205a 6f63  ler, Marcelo Zoc
 00000080: 636f 6c65 722c 2052 6f62 6572 7420 4861  coler, Robert Ha
 00000090: 6173 650d 0a61 7574 686f 725f 656d 6169  ase..author_emai
 000000a0: 6c20 3d20 7a69 6775 7479 7465 4067 6d61  l = zigutyte@gma
```

