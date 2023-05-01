# Comparing `tmp/SeedsLabeler-0.0.8.tar.gz` & `tmp/SeedsLabeler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SeedsLabeler-0.0.8.tar", last modified: Mon Aug  5 14:16:20 2019, max compression
+gzip compressed data, was "dist/SeedsLabeler-0.0.9.tar", last modified: Mon Aug  5 15:29:35 2019, max compression
```

## Comparing `SeedsLabeler-0.0.8.tar` & `SeedsLabeler-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     3714 2019-08-05 14:15:23.000000 SeedsLabeler-0.0.8/setup.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)       38 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/setup.cfg
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1028 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/PKG-INFO
-drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/src/
--rw-rw-r--   0 giancos   (1001) giancos   (1001)   248667 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/resources.py
-drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/src/libs/
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     6547 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/shape.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)    10513 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/project.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1790 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/projectDialog.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     3752 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/labelFile.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)       76 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/version.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     2264 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/stringBundle.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)    27681 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/canvas.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     2882 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/labelDialog.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)      790 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/hashableQListWidgetItem.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1453 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/category.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1767 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/project_data.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/__init__.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1293 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/colorDialog.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     6634 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/image.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     6036 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/zoom.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     2760 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/lib.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     4335 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/file_loader.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     6222 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/pascal_voc_io.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1400 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/constants.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)      528 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/ustr.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1192 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/toolBar.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1426 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/settings.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)      780 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/zoomWidget.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     4722 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/libs/yolo_io.py
-drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/src/api/
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1690 2019-08-05 13:24:45.000000 SeedsLabeler-0.0.8/src/api/inference_api.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/api/__init__.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     2631 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/api/detection_client.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/__init__.py
-drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/src/gui/
--rw-rw-r--   0 giancos   (1001) giancos   (1001)    33717 2019-08-05 13:25:21.000000 SeedsLabeler-0.0.8/src/gui/ui_mainwindow.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)    38017 2019-08-05 13:17:06.000000 SeedsLabeler-0.0.8/src/gui/LabelerWindow.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.8/src/gui/__init__.py
-drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1004 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/SOURCES.txt
--rw-rw-r--   0 giancos   (1001) giancos   (1001)        1 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/not-zip-safe
--rw-rw-r--   0 giancos   (1001) giancos   (1001)     1028 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/PKG-INFO
--rw-rw-r--   0 giancos   (1001) giancos   (1001)       33 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/requires.txt
--rw-rw-r--   0 giancos   (1001) giancos   (1001)        1 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/dependency_links.txt
--rw-rw-r--   0 giancos   (1001) giancos   (1001)       65 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/entry_points.txt
--rw-rw-r--   0 giancos   (1001) giancos   (1001)       17 2019-08-05 14:16:20.000000 SeedsLabeler-0.0.8/SeedsLabeler.egg-info/top_level.txt
--rw-rw-r--   0 giancos   (1001) giancos   (1001)       21 2019-08-05 14:16:16.000000 SeedsLabeler-0.0.8/__init__.py
--rwxrwxr-x   0 giancos   (1001) giancos   (1001)     3395 2019-08-05 13:39:27.000000 SeedsLabeler-0.0.8/SeedsLabeler.py
--rw-rw-r--   0 giancos   (1001) giancos   (1001)      132 2019-08-05 14:14:02.000000 SeedsLabeler-0.0.8/README.md
+drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)      986 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/PKG-INFO
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       98 2019-08-05 14:17:14.000000 SeedsLabeler-0.0.9/README.md
+drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)      986 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/PKG-INFO
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1004 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/SOURCES.txt
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)        1 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/dependency_links.txt
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       65 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/entry_points.txt
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)        1 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/not-zip-safe
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       33 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/requires.txt
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       17 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/SeedsLabeler.egg-info/top_level.txt
+-rwxrwxr-x   0 giancos   (1001) giancos   (1001)     3395 2019-08-05 13:39:27.000000 SeedsLabeler-0.0.9/SeedsLabeler.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       21 2019-08-05 15:28:49.000000 SeedsLabeler-0.0.9/__init__.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       38 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/setup.cfg
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     3714 2019-08-05 14:15:23.000000 SeedsLabeler-0.0.9/setup.py
+drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/src/
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/__init__.py
+drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/src/api/
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/api/__init__.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     2631 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/api/detection_client.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1690 2019-08-05 13:24:45.000000 SeedsLabeler-0.0.9/src/api/inference_api.py
+drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/src/gui/
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)    38017 2019-08-05 13:17:06.000000 SeedsLabeler-0.0.9/src/gui/LabelerWindow.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/gui/__init__.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)    33717 2019-08-05 13:25:21.000000 SeedsLabeler-0.0.9/src/gui/ui_mainwindow.py
+drwxrwxr-x   0 giancos   (1001) giancos   (1001)        0 2019-08-05 15:29:35.000000 SeedsLabeler-0.0.9/src/libs/
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)        0 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/__init__.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)    27681 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/canvas.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1453 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/category.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1293 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/colorDialog.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1400 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/constants.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     4335 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/file_loader.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)      790 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/hashableQListWidgetItem.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     6634 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/image.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     2882 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/labelDialog.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     3752 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/labelFile.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     2760 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/lib.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     6222 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/pascal_voc_io.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)    10513 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/project.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1790 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/projectDialog.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1767 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/project_data.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1426 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/settings.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     6547 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/shape.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     2264 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/stringBundle.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     1192 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/toolBar.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)      528 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/ustr.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)       76 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/version.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     4722 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/yolo_io.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)     6043 2019-08-05 15:27:50.000000 SeedsLabeler-0.0.9/src/libs/zoom.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)      780 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/libs/zoomWidget.py
+-rw-rw-r--   0 giancos   (1001) giancos   (1001)   248667 2019-08-05 13:10:59.000000 SeedsLabeler-0.0.9/src/resources.py
```

### Comparing `SeedsLabeler-0.0.8/setup.py` & `SeedsLabeler-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/PKG-INFO` & `SeedsLabeler-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 1.2
 Name: SeedsLabeler
-Version: 0.0.8
+Version: 0.0.9
 Summary: Seeds annotation tool
 Home-page: https://github.com/meryusha/seeds_labeler/
 Author: Merey Ramazanova, Silvio Giancola
 Author-email: merey.ramazanova@kaust.edu.sa
 License: MIT license
 Description: # Seeds Labeler
-        # TCP communication using QTCPSocket
         
-        install with `pip install TCPClient`
+        install with `pip install SeedsLabeler`
         
         # Update pip:
         
         `python setup.py upload`
```

### Comparing `SeedsLabeler-0.0.8/src/resources.py` & `SeedsLabeler-0.0.9/src/resources.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/shape.py` & `SeedsLabeler-0.0.9/src/libs/shape.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/project.py` & `SeedsLabeler-0.0.9/src/libs/project.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/projectDialog.py` & `SeedsLabeler-0.0.9/src/libs/projectDialog.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/labelFile.py` & `SeedsLabeler-0.0.9/src/libs/labelFile.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/stringBundle.py` & `SeedsLabeler-0.0.9/src/libs/stringBundle.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/canvas.py` & `SeedsLabeler-0.0.9/src/libs/canvas.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/labelDialog.py` & `SeedsLabeler-0.0.9/src/libs/labelDialog.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/hashableQListWidgetItem.py` & `SeedsLabeler-0.0.9/src/libs/hashableQListWidgetItem.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/category.py` & `SeedsLabeler-0.0.9/src/libs/category.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/project_data.py` & `SeedsLabeler-0.0.9/src/libs/project_data.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/colorDialog.py` & `SeedsLabeler-0.0.9/src/libs/colorDialog.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/image.py` & `SeedsLabeler-0.0.9/src/libs/image.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/zoom.py` & `SeedsLabeler-0.0.9/src/libs/zoom.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         # get the cursor position and canvas size
         # calculate the desired movement from 0 to 1
         # where 0 = move left
         #       1 = move right
         # up and down analogous
         cursor = QCursor()
         pos = cursor.pos()
-        relative_pos = QWidget.mapFromGlobal(self, pos)
+        relative_pos = QWidget.mapFromGlobal(self.parent, pos)
 
         cursor_x = relative_pos.x()
         cursor_y = relative_pos.y()
 
         w = self.parent.scroll.width()
         h = self.parent.scroll.height()
```

### Comparing `SeedsLabeler-0.0.8/src/libs/lib.py` & `SeedsLabeler-0.0.9/src/libs/lib.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/file_loader.py` & `SeedsLabeler-0.0.9/src/libs/file_loader.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/pascal_voc_io.py` & `SeedsLabeler-0.0.9/src/libs/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/constants.py` & `SeedsLabeler-0.0.9/src/libs/constants.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/ustr.py` & `SeedsLabeler-0.0.9/src/libs/ustr.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/toolBar.py` & `SeedsLabeler-0.0.9/src/libs/toolBar.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/settings.py` & `SeedsLabeler-0.0.9/src/libs/settings.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/zoomWidget.py` & `SeedsLabeler-0.0.9/src/libs/zoomWidget.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/libs/yolo_io.py` & `SeedsLabeler-0.0.9/src/libs/yolo_io.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/api/inference_api.py` & `SeedsLabeler-0.0.9/src/api/inference_api.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/api/detection_client.py` & `SeedsLabeler-0.0.9/src/api/detection_client.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/gui/ui_mainwindow.py` & `SeedsLabeler-0.0.9/src/gui/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/src/gui/LabelerWindow.py` & `SeedsLabeler-0.0.9/src/gui/LabelerWindow.py`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/SeedsLabeler.egg-info/SOURCES.txt` & `SeedsLabeler-0.0.9/SeedsLabeler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SeedsLabeler-0.0.8/SeedsLabeler.egg-info/PKG-INFO` & `SeedsLabeler-0.0.9/SeedsLabeler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 1.2
 Name: SeedsLabeler
-Version: 0.0.8
+Version: 0.0.9
 Summary: Seeds annotation tool
 Home-page: https://github.com/meryusha/seeds_labeler/
 Author: Merey Ramazanova, Silvio Giancola
 Author-email: merey.ramazanova@kaust.edu.sa
 License: MIT license
 Description: # Seeds Labeler
-        # TCP communication using QTCPSocket
         
-        install with `pip install TCPClient`
+        install with `pip install SeedsLabeler`
         
         # Update pip:
         
         `python setup.py upload`
```

### Comparing `SeedsLabeler-0.0.8/SeedsLabeler.py` & `SeedsLabeler-0.0.9/SeedsLabeler.py`

 * *Files identical despite different names*

