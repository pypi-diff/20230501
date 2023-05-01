# Comparing `tmp/palmari-0.2.8.tar.gz` & `tmp/palmari-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palmari-0.2.8.tar", last modified: Mon Oct 24 11:26:17 2022, max compression
+gzip compressed data, was "palmari-0.3.0.tar", last modified: Mon May  1 18:42:50 2023, max compression
```

## Comparing `palmari-0.2.8.tar` & `palmari-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.600133 palmari-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-24 11:25:58.000000 palmari-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21780 2022-10-24 11:25:58.000000 palmari-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-24 11:25:58.000000 palmari-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-24 11:26:17.600133 palmari-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-10-24 11:25:58.000000 palmari-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-10-24 11:25:58.000000 palmari-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-24 11:26:17.600133 palmari-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/palmari/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8431 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/palmari/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.596133 palmari-0.2.8/src/palmari/data_structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/data_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21364 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/data_structure/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (121)    16307 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/data_structure/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.596133 palmari-0.2.8/src/palmari/processing/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8279 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/edit_pipeline_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.596133 palmari-0.2.8/src/palmari/processing/steps/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/drift_corrector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/quot_localizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6339 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/quot_tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/trackpy_tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/window_percentile.py
--rw-r--r--   0 runner    (1001) docker     (121)    14976 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/tif_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    22519 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/tif_pipeline_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.600133 palmari-0.2.8/src/palmari/quot/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15820 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/chunkFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8583 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    23222 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/findSpots.py
--rw-r--r--   0 runner    (1001) docker     (121)    47710 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13888 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/measureGain.py
--rw-r--r--   0 runner    (1001) docker     (121)    38259 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    11057 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/read.py
--rw-r--r--   0 runner    (1001) docker     (121)    14554 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/subpixel.py
--rw-r--r--   0 runner    (1001) docker     (121)    32243 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/track.py
--rw-r--r--   0 runner    (1001) docker     (121)    10373 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/trajUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.600133 palmari-0.2.8/src/palmari/tif_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/cell_mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3967 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/correct_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/density_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/intensity.py
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/localization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/palmari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.181620 palmari-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 18:42:34.000000 palmari-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-05-01 18:42:34.000000 palmari-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 18:42:34.000000 palmari-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-01 18:42:50.181620 palmari-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-01 18:42:34.000000 palmari-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-01 18:42:34.000000 palmari-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-01 18:42:50.185620 palmari-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.177620 palmari-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.177620 palmari-0.3.0/src/palmari/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.177620 palmari-0.3.0/src/palmari/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.181620 palmari-0.3.0/src/palmari/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/data_structure/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/data_structure/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.181620 palmari-0.3.0/src/palmari/image_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/image_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/image_tools/cell_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/image_tools/correct_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/image_tools/density_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/image_tools/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/image_tools/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.181620 palmari-0.3.0/src/palmari/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/edit_pipeline_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/image_pipeline_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.181620 palmari-0.3.0/src/palmari/processing/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/drift_corrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/quot_localizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/quot_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/trackpy_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/steps/window_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/processing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.181620 palmari-0.3.0/src/palmari/quot/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/chunkFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23222 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/findSpots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47712 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/measureGain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/subpixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32243 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-05-01 18:42:34.000000 palmari-0.3.0/src/palmari/quot/trajUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:42:50.177620 palmari-0.3.0/src/palmari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-01 18:42:50.000000 palmari-0.3.0/src/palmari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 18:42:50.000000 palmari-0.3.0/src/palmari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:42:50.000000 palmari-0.3.0/src/palmari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 18:42:50.000000 palmari-0.3.0/src/palmari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-01 18:42:50.000000 palmari-0.3.0/src/palmari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 18:42:50.000000 palmari-0.3.0/src/palmari.egg-info/top_level.txt
```

### Comparing `palmari-0.2.8/LICENSE` & `palmari-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/PKG-INFO` & `palmari-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: palmari
-Version: 0.2.8
-Summary: A pipeline for PALM movies analysis (pre-processing, localization, drifft correction, tracking)
+Version: 0.3.0
+Summary: Palmari provides a plugin to analyze PALM movies, as well as microscope recordings of other SMLM-based SPT modalities. Set up your pipeline on one file, run it on a folder !
 Home-page: https://github.com/hippover/palmari
 Author: Hippolyte Verdier
 Author-email: hverdier@pasteur.fr
 License: "CeCILL"
 Project-URL: Bug Tracker, https://github.com/hippover/palmari/issues
 Project-URL: Documentation, https://palmari.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/hippover/palmari
 Project-URL: User Support, https://github.com/hippover/palmari/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
+Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -35,15 +36,15 @@
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/palmari)](https://napari-hub.org/plugins/palmari)
 [![License](https://img.shields.io/pypi/l/palmari.svg?color=green)](https://github.com/hippover/palmari/raw/main/LICENSE)
 
 A processing pipeline for PALM movies analysis (pre-processing, localization, drift correction, tracking).
 
 Check out the [documentation] to get started.
 
-![napari_plugin](docs/images/plugin_steps.png "Fine-tune your pipelines on a movie, run it on a batch easily !")
+![napari_plugin](https://github.com/hippover/palmari/raw/main/docs/images/plugin_steps.png "Fine-tune your pipelines on a movie, run it on a batch easily !")
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `palmari-0.2.8/README.md` & `palmari-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/palmari)](https://napari-hub.org/plugins/palmari)
 [![License](https://img.shields.io/pypi/l/palmari.svg?color=green)](https://github.com/hippover/palmari/raw/main/LICENSE)
 
 A processing pipeline for PALM movies analysis (pre-processing, localization, drift correction, tracking).
 
 Check out the [documentation] to get started.
 
-![napari_plugin](docs/images/plugin_steps.png "Fine-tune your pipelines on a movie, run it on a batch easily !")
+![napari_plugin](https://github.com/hippover/palmari/raw/main/docs/images/plugin_steps.png "Fine-tune your pipelines on a movie, run it on a batch easily !")
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `palmari-0.2.8/setup.cfg` & `palmari-0.3.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [metadata]
 name = palmari
-version = 0.2.8
+version = 0.3.0
 author = Hippolyte Verdier
 author_email = hverdier@pasteur.fr
 url = https://github.com/hippover/palmari
 license = "CeCILL"
-description = A pipeline for PALM movies analysis (pre-processing, localization, drifft correction, tracking)
+description = Palmari provides a plugin to analyze PALM movies, as well as microscope recordings of other SMLM-based SPT modalities. Set up your pipeline on one file, run it on a folder !
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
-	Intended Audience :: Developers
+	Development Status :: 4 - Beta
+	Intended Audience :: Science/Research
 	Framework :: napari
-	Topic :: Software Development :: Testing
+	Environment :: Plugins
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Topic :: Scientific/Engineering :: Image Processing
 	Operating System :: OS Independent
 	License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 project_urls = 
 	Bug Tracker = https://github.com/hippover/palmari/issues
 	Documentation = https://palmari.readthedocs.io/en/latest/
 	Source Code = https://github.com/hippover/palmari
 	User Support = https://github.com/hippover/palmari/issues
@@ -37,21 +38,21 @@
 	dask>=2022.1.0
 	dask-image>=2021.12.0
 	imageio-ffmpeg
 	magicgui>=0.5.0
 	matplotlib>=3.5
 	munkres
 	napari
-	nd2reader
+	napari-aicsimageio
 	numpy
 	pandas
 	pyyaml
-	sklearn
+	qtpy
 	scikit-image>=0.18.3
-	tiffile
+	scikit-learn
 	toml
 	tqdm
 	trackpy>=0.5.0
 
 [options.extras_require]
 testing = 
 	tox
```

### Comparing `palmari-0.2.8/src/palmari/_runner.py` & `palmari-0.3.0/src/palmari/_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from napari import Viewer
+from napari.qt import thread_worker
 import os
 
-from .processing import TifPipeline
+from .processing import ImagePipeline
 from .processing.steps import *
 from qtpy.QtWidgets import (
     QDialog,
     QErrorMessage,
     QLineEdit,
     QPushButton,
     QWidget,
     QVBoxLayout,
     QHBoxLayout,
     QLabel,
 )
-from PyQt5.QtCore import pyqtSignal
+from qtpy.QtCore import Signal
 from magicgui.widgets import FileEdit, FloatSpinBox, LineEdit, ProgressBar
-from threading import Thread
+import dask
 
 
 class PipelineRunner(QWidget):
 
-    progressChanged = pyqtSignal(int)
-    progressRunning = pyqtSignal(bool)
-    nFilesChanged = pyqtSignal(int)
-    nameProcessingFile = pyqtSignal(str)
+    progressChanged = Signal(int)
+    progressRunning = Signal(bool)
+    nFilesChanged = Signal(int)
+    nameProcessingFile = Signal(str)
 
-    def __init__(self):
+    def __init__(self, napari_viewer: Viewer):
         super().__init__()
         self.setup_ui()
         self.running = False
         self.pixel_size = 0.097
         self.DT = 0.03
         self.file_pattern = ".tif"
 
@@ -48,14 +49,17 @@
         def updateFileName(s):
             self.file_label.setText(s)
 
         self.progressChanged.connect(updatePgBar)
         self.progressRunning.connect(showPgBar)
         self.nFilesChanged.connect(updateNFiles)
         self.nameProcessingFile.connect(updateFileName)
+        
+        self.viewer = napari_viewer
+        self.viewer.reset_view()
 
     def setup_ui(self):
         main_layout = QVBoxLayout()
         main_layout.addLayout(self.choose_pipeline_layout())
         main_layout.addLayout(self.choose_input_folder_layout())
         main_layout.addLayout(self.choose_export_folder_layout())
 
@@ -148,63 +152,81 @@
 
     ###
     # ACTION
     ###
 
     def load_pipeline(self, file_path):
         try:
-            tp = TifPipeline.from_yaml(file_path)
+            tp = ImagePipeline.from_yaml(file_path)
             self.tp = tp
         except BaseException as e:
             print(e)
             em = QErrorMessage()
             em.showMessage(
                 "Could not load pipeline from file %s, check the format"
                 % file_path
             )
 
     def run_pipeline(self):
         self.running = True
         self.enable_run_button()
-        # self._run_pipeline()
-        th = Thread(target=self._run_pipeline)
-        th.start()
-
-    def _run_pipeline(self):
+        worker = self._run_pipeline()
+        worker.finished.connect(self._run_finished)
+        worker.yielded.connect(self._run_progressed)
+        worker.started.connect(self._run_started)
+        worker.start()
+        
+    def _run_started(self):
         exp = self.exp
         assert exp is not None
         self.nFilesChanged.emit(len(exp.scan_folder()))
         self.progressChanged.emit(0)
         self.progressRunning.emit(True)
+    
+    def _run_finished(self):
+        self.progressRunning.emit(False)
+        self.enable_run_button()
+        
+    def _run_progressed(self, yielded):
+        image_number, image_file = yielded
+        if image_file != "DONE":
+            self.nameProcessingFile.emit("Processing %s ..." % image_file)
+        self.progressChanged.emit(image_number)
+
+    @thread_worker
+    def _run_pipeline(self):
+        
+        dask.config.set(scheduler='processes') 
+        
+        exp = self.exp
         for i, f in enumerate(exp):
-            self.nameProcessingFile.emit("Processing %s ..." % f)
-            acq = Acquisition(f, experiment=exp, tif_pipeline=self.tp)
+            yield (i, f)
+            acq = Acquisition(f, experiment=exp, image_pipeline=self.tp)
             if i == 0:
                 pipeline_export_path_for_exp = self.tp.exp_params_path(acq)
                 logging.info(
                     "Saving pipeline to %s" % pipeline_export_path_for_exp
                 )
             self.tp.process(to_process=acq, force_reprocess=True)
-            self.progressChanged.emit(i + 1)
-        self.progressRunning.emit(False)
-        self.enable_run_button()
+        yield (i+1, "DONE")
+        
 
     ###
     # PROPERTIES
     ###
 
     @property
     def tp(self):
         if hasattr(self, "_tp"):
             return self._tp
         else:
             return None
 
     @tp.setter
-    def tp(self, tp: TifPipeline):
+    def tp(self, tp: ImagePipeline):
         self._tp = tp
         self.enable_run_button()
         self.setWindowTitle("Palmari | %s" % tp.name)
 
     @property
     def exp(self):
         if hasattr(self, "_input_folder") and hasattr(self, "_export_folder"):
@@ -253,32 +275,38 @@
 
     ###
     # OTHERS
     ###
 
     def enable_run_button(self):
         exp = self.exp
+        exp_has_files = False
         if self.running:
             self.run_button.setText("Processing...")
         else:
             if exp is not None:
+                files = exp.scan_folder()
+                n_files = len(files)
+                exp_has_files = n_files > 0
                 self.run_button.setText(
-                    "Process %d files !" % len(exp.scan_folder())
+                    "Process %d files !" % n_files
                 )
             else:
                 self.run_button.setText("Process (?) files !")
 
         self.run_button.setEnabled(
             (self.tp is not None)
             and (self.export_folder is not None)
             and (self.input_folder is not None)
+            and exp_has_files
             and (not self.running)
         )
 
     def setExpPixel(self, s: float):
         self.pixel_size = s
 
     def setExpPattern(self, p: str):
         self.file_pattern = p
+        self.enable_run_button()
 
     def setExpDT(self, DT: float):
-        self.DT = DT
+        self.DT = DT
```

### Comparing `palmari-0.2.8/src/palmari/_tests/test_widget.py` & `palmari-0.3.0/src/palmari/_tests/test_widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 from .._widget import PalmariWidget
+from ..data_structure.acquisition import Acquisition
+from ..data_structure.experiment import Experiment
+from ..processing.image_pipeline import ImagePipeline
+from glob import glob
 import numpy as np
 
 # make_napari_viewer is a pytest fixture that returns a napari viewer object
 # capsys is a pytest fixture that captures stdout and stderr output streams
 def test_example_q_widget(make_napari_viewer, capsys):
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
@@ -10,8 +14,8 @@
 
     # create our widget, passing in the viewer
     my_widget = PalmariWidget(viewer)
 
     # read captured output and check that it's as we expected
     # captured = capsys.readouterr()
     # assert captured.out == "napari has 1 layers\n"
-    assert True
+    assert True
```

### Comparing `palmari-0.2.8/src/palmari/_widget.py` & `palmari-0.3.0/src/palmari/_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-from .processing import TifPipelineWidget
-from .processing import TifPipeline
+from __future__ import annotations
+
+from .processing.image_pipeline_widget import ImagePipelineWidget
+from .processing.image_pipeline import ImagePipeline
 from .processing.steps import *
-from napari import Viewer
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from napari import Viewer
 
 
-class PalmariWidget(TifPipelineWidget):
+class PalmariWidget(ImagePipelineWidget):
     def __init__(self, napari_viewer: Viewer):
-        tp = TifPipeline.from_dict(
+        tp = ImagePipeline.from_dict(
             {
                 "name": "palmari-default",
                 "detector": {"BaseDetector": {"k": 1.5, "w": 21, "t": 1.0}},
                 "localizer": {
                     "MaxLikelihoodLocalizer": {
                         "method": "ls_int_gaussian",
                         "window_size": 9,
@@ -24,8 +29,8 @@
                         "init_cost": 50.0,
                         "d_bound_naive": 0.1,
                     }
                 },
             }
         )
         print(tp)
-        super().__init__(tif_pipeline=tp, napari_viewer=napari_viewer)
+        super().__init__(image_pipeline=tp, napari_viewer=napari_viewer)
```

### Comparing `palmari-0.2.8/src/palmari/data_structure/acquisition.py` & `palmari-0.3.0/src/palmari/data_structure/acquisition.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,87 +3,83 @@
 from typing import TYPE_CHECKING, Any, Callable, List
 import os
 import warnings
 import pandas as pd
 import numpy as np
 import trackpy as tp
 import logging
-import napari
 from glob import glob
-import dask_image.imread
 import dask.array as da
 import dask_image.ndfilters
 from skimage.filters import sato, threshold_local
+from aicsimageio import AICSImage
 
 
-from ..tif_tools.intensity import mean_intensity_center
-from ..tif_tools.correct_drift import correct_drift
-from ..tif_tools.localization import localize_movie
+from ..image_tools.intensity import mean_intensity_center
+from ..image_tools.correct_drift import correct_drift
 
 if TYPE_CHECKING:
     from .experiment import Experiment
-    from ..processing.tif_pipeline import TifPipeline
+    from ..processing.image_pipeline import ImagePipeline
 
 
 class Acquisition:
     """
     An acquisition corresponds to a PALM movie.
-    It is part of an :py:class:`Experiment`, and bound to a :py:class:`TifPipeline` with which it is processed.
+    It is part of an :py:class:`Experiment`, and bound to a :py:class:`ImagePipeline` with which it is processed.
     """
 
     def __init__(
         self,
-        tif_file,
+        image_file,
         experiment: Experiment,
-        tif_pipeline: TifPipeline,
+        image_pipeline: ImagePipeline,
     ):
-        self.tif_file = tif_file
-        self.tif_pipeline = tif_pipeline
+        self.image_file = image_file
+        self.image_pipeline = image_pipeline
         self.experiment = experiment
         self.export_root = os.path.join(
             self.experiment.export_folder,
-            self.tif_pipeline.name,
-            ".".join(self.tif_file.split(".")[:-1]),
+            self.image_pipeline.name,
+            ".".join(self.image_file.split(".")[:-1]),
         )
         logging.debug(
-            "export_root : file %s -> %s" % (self.tif_file, self.export_root)
+            "export_root : file %s -> %s" % (self.image_file, self.export_root)
         )
         export_parent_folder = os.sep.join(self.export_root.split(os.sep)[:-1])
         os.makedirs(export_parent_folder, exist_ok=True)
 
     @property
     def image(self) -> da.Array:
         """
         The actual movie, loaded with Dask.
 
         Returns:
             da.Array: the movie.
         """
         if not hasattr(self, "_image"):
-            logging.info("Loading tif file %s" % self.tif_file)
-            # self._image = tifffile.imread(
+            logging.info("Loading tif file %s" % self.image_file)
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
-                self._image = dask_image.imread.imread(
-                    os.path.join(self.experiment.data_folder, self.tif_file),
-                    nframes=300,
-                )
+                image_path = os.path.join(self.experiment.data_folder, self.image_file)
+                self._image = da.rechunk(da.squeeze(AICSImage(image_path).dask_data),chunks={0:255,1:-1,2:-1})
+                assert len(self._image.shape) == 3, "Images should have 3 dimensions of size > 1"
         return self._image
 
     def get_property(self, col: str) -> Any:
         """Access an acquisition's property, read from its experiment's index table.
 
         Args:
             col (str): name of the index table column to look into
 
         Returns:
             Any: value of the corresponding row x column in the experiment's index table
         """
         df = self.experiment.index_df
-        return df.loc[df.file == self.tif_file, col].values[0]
+        return df.loc[df.file == self.image_file, col].values[0]
 
     @property
     def ID(self) -> str:
         return self.get_property("ID")
 
     def _clean_locs_table(self, df: pd.DataFrame) -> pd.DataFrame:
         for c in ["frame", "x", "y", "t"]:
@@ -258,30 +254,30 @@
         )
 
     def compute_intensity(self):
         if not self.intensity_is_computed:
             self._intensity = mean_intensity_center(self.image)
             self._save_intensity()
         else:
-            logging.info("%s : intensity is already computed" % self.tif_file)
+            logging.info("%s : intensity is already computed" % self.image_file)
 
     def _save_intensity(self):
         storage_path = self.intensity_path
         self._intensity.to_csv(storage_path, index=False)
         logging.info(
             "Stored Intensity of ROI %s at path %s"
-            % (self.tif_file, storage_path)
+            % (self.image_file, storage_path)
         )
 
     def compute_tubeness(self):
         if not self.tubeness_is_computed:
             self._compute_tubeness()
             self._save_tubeness()
         else:
-            logging.info("%s : tubeness was already processed" % self.tif_file)
+            logging.info("%s : tubeness was already processed" % self.image_file)
 
     def _compute_tubeness(self):
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             mean = self.image[::10].mean(axis=0)
             mean_intensity = mean.compute()
@@ -295,86 +291,65 @@
     def _save_tubeness(self):
         storage_path = self.tubeness_path
         np.save(storage_path, self._tubeness)
         logging.info("Saved tubeness at %s" % storage_path)
 
     def localize(self):
         if not self.is_localized:
-            logging.info("Running localization for file %s" % self.tif_file)
-            self._localize(**self.tif_pipeline.params.loc_params)
+            logging.info("Running localization for file %s" % self.image_file)
+            self._localize(**self.image_pipeline.params.loc_params)
             self._save_raw_locs()
         else:
             logging.info(
                 "Localization step has already been done for file %s"
-                % self.tif_file
+                % self.image_file
             )
 
-    def _localize(
-        self, threshold, sliding_window_filter, subpixel_mode, **args
-    ):
-
-        data = self.image
-        self._raw_locs = localize_movie(
-            data,
-            progress_bar=True,
-            verbose=False,
-            sliding_filter=sliding_window_filter,
-            factor=threshold,
-            subpixel_mode=subpixel_mode,
-        )
-        self._raw_locs["t"] = self._raw_locs["frame"] * self.experiment.DT
-        self._raw_locs[
-            ["x", "y"]
-        ] *= self.experiment.pixel_size  # x, y are in um
-        N = self._raw_locs.shape[0]
-        T = data.shape[0]
-        logging.info("==== %d locs\t %.2f / frame" % (N, N / T))
-
     def _save_raw_locs(self):
         storage_path = self.raw_locs_path
         self._raw_locs.to_csv(storage_path, index=False)
         logging.info(
             "Stored raw locs of ROI %s at path %s"
-            % (self.tif_file, storage_path)
+            % (self.image_file, storage_path)
         )
 
     def correct_drift(self):
         if not self.drift_is_corrected:
-            if self.tif_pipeline.params.loc_params["correct_drift"] == True:
+            if self.image_pipeline.params.loc_params["correct_drift"] == True:
                 self._correct_drift()
             else:
                 self._locs = self.raw_locs
             self._save_locs()
         else:
             logging.info(
                 "Drift correction step has already been done for file %s"
-                % self.tif_file
+                % self.image_file
             )
 
     def _correct_drift(self):
         logging.info("Correcting drift iteration #1/2")
         df, self._shift_1 = correct_drift(self.raw_locs, L=0.2, step_size=0.03)
         logging.info("Correcting drift iteration #2/2")
         self._locs, self._shift_2 = correct_drift(df, L=0.05, step_size=0.01)
 
     def _save_locs(self):
         storage_path = self.locs_path
         self._locs.to_csv(storage_path, index=False)
         logging.info(
-            "Stored locs of ROI %s at path %s" % (self.tif_file, storage_path)
+            "Stored locs of ROI %s at path %s" % (self.image_file, storage_path)
         )
 
     def track(self):
         if not self.is_tracked:
-            logging.info("Running tracking for file %s" % self.tif_file)
-            self._track(**self.tif_pipeline.params.track_params)
+            logging.info("Running tracking for file %s" % self.image_file)
+            self._track(**self.image_pipeline.params.track_params)
             self._save_locs()
         else:
             logging.info(
-                "Tracking was already done for file %s" % self.tif_file
+                "Tracking was already done for file %s" % self.image_file
             )
 
     def _track(self, mode, max_diffusivity):
 
         if mode == "trackpy":
             self._track_trackpy(max_diffusivity)
         else:
@@ -389,15 +364,15 @@
             self.locs, search_range=max_radius, link_strategy="drop"
         )
         self._locs["n"] = tracks["particle"]
         traj_length = self._locs.n.value_counts()
         n_long_trajs = (traj_length >= 7).sum()
         logging.info(
             "Found %d long trajectories for file %s"
-            % (n_long_trajs, self.tif_file)
+            % (n_long_trajs, self.image_file)
         )
 
     # EXPLOITATION OF TRACKS AND LOCS
 
     def trajectories_list(
         self,
         min_length: int = 7,
@@ -444,15 +419,15 @@
     def get_traj(self, n: int):
         return (
             self.locs.loc[self.locs.n == n].sort_values("t")[["x", "y"]].values
         )
 
     def basic_stats(self):
         stats = {}
-        stats["file"] = self.tif_file
+        stats["file"] = self.image_file
         stats["n_frames"] = self.locs.frame.max()
         stats["duration"] = stats["n_frames"] * self.experiment.DT
         # the above is not exactly true, but is much faster than what's below
         # self.image.shape[0]
         if not self.is_processed:
             return stats
         stats["n_locs"] = self.locs.shape[0]
@@ -466,18 +441,20 @@
     def view(
         self,
         min_traj_length=1,
         polygon_ID_col: str = None,
         short_for_tests: bool = False,
         contrast_limits: tuple = (100, 500),
     ):
-        viewer = napari.viewer.Viewer(title=os.path.dirname(self.tif_file))
+        import napari
+        
+        viewer = napari.viewer.Viewer(title=os.path.dirname(self.image_file))
         viewer.add_image(
             self.image[:1000] if short_for_tests else self.image,
-            name=self.tif_file.split("/")[-1],
+            name=self.image_file.split("/")[-1],
             multiscale=False,
             contrast_limits=contrast_limits,
             scale=(1, self.experiment.pixel_size, self.experiment.pixel_size),
         )
         if self.locs is not None:
             self.view_points(viewer, polygon_ID_col=polygon_ID_col)
             self.view_tracks(
@@ -487,14 +464,15 @@
             )
             self.view_polygons(viewer)
 
     def view_points(
         self, viewer=None, polygon_ID_col: str = None, subsample: int = None
     ):
         if viewer is None:
+            import napari
             viewer = napari.viewer.Viewer()
         locs = self.locs.copy()
         if subsample is not None and subsample < locs.shape[0]:
             locs = locs.sample(subsample)
 
         points = locs[["frame", "x", "y"]].copy()
         # points[["x","y"]] /= self.pixel_size
@@ -537,14 +515,15 @@
 
     # FOR THE VIEWER
 
     def view_tracks(
         self, viewer=None, min_length=1, polygon_ID_col: str = None
     ):
         if viewer is None:
+            import napari
             viewer = napari.viewer.Viewer()
 
         traj_length = self.locs.n.value_counts()
         good_trajs = traj_length.loc[traj_length >= min_length].index.tolist()
 
         tracks = self.locs.loc[
             self.locs.n.isin(good_trajs),
@@ -597,16 +576,17 @@
             tail_width=0.2,
             name="Tracks",
             tail_length=10,
             head_length=10,
             properties=track_properties,
         )
 
-    def view_polygons(self, viewer: napari.Viewer = None):
+    def view_polygons(self, viewer = None):
         if viewer is None:
+            import napari
             viewer = napari.viewer.Viewer()
         polygons = []
 
         for p in self.polygon_files:
             polygon_dict = json.load(open(p, "r"))
             if len(polygon_dict["x"]) < 3:
                 logging.debug("%s a moins de 3 points, on le supprime" % p)
```

### Comparing `palmari-0.2.8/src/palmari/data_structure/experiment.py` & `palmari-0.3.0/src/palmari/data_structure/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,119 +62,105 @@
         else:
             raise "Invalid item %s" % item
 
     def __len__(self):
         return self.index_df.shape[0]
 
     @classmethod
-    def from_single_tif(cls, tif_file: str, export_folder: str):
-        data_folder = os.path.split(tif_file)[0]
+    def from_single_tif(cls, image_file: str, export_folder: str):
+        data_folder = os.path.split(image_file)[0]
         return Experiment(data_folder=data_folder, export_folder=export_folder)
 
-    """
-    def to_tracksets(self, tif_pipeline: TifPipeline) -> TrackSets:
-        tracksets = []
-        included_files = []
-        for tif_file in self:
-            acq = Acquisition(
-                tif_file=tif_file, experiment=self, tif_pipeline=tif_pipeline
-            )
-            if not acq.is_processed:
-                logging.debug("Not including %s" % tif_file)
-                continue
-            included_files.append(tif_file)
-            tracksets.append(
-                TrackSet(locs_path=acq.locs_path, origin_file=tif_file)
-            )
-        return TrackSets(
-            tracksets=tracksets,
-            root_folder=self.export_folder,
-            index_df=self.index_df.loc[
-                self.index_df.file.isin(included_files)
-            ],
-        )
-    """
-
     def check_export_folder_and_load_info(self):
         json_path = os.path.join(self.export_folder, "exp_info.json")
         if not os.path.isdir(self.export_folder):
             # Create a json file with experiment-level information
             logging.info("Create %s" % self.export_folder)
             os.mkdir(self.export_folder)
-
-        if not os.path.exists(json_path):
-            logging.info("JSON does not exist, create %s" % json_path)
-            # Quite some redundancies here...
-            pixel_size = self.pixel_size
-            if pixel_size is None:
-                pixel_size = 0.097
-                try:
-                    pixel_size = float(
-                        input("Pixel size, in microns (default is 0.097) : ")
-                    )
-                except BaseException as e:
-                    print(e)
-                    print(
-                        "Incorrect value, keeping default : %.2f um"
-                        % pixel_size
-                    )
-                self.pixel_size = pixel_size
-
-            DT = self.DT
-            if DT is None:
-                DT = 0.03
-                try:
-                    DT = float(
-                        input(
-                            "Time interval between successive frames, in seconds (default is 0.03) : "
-                        )
-                    )
-                except BaseException as e:
-                    print(e)
-                    print("Incorrect value, keeping default : %.2f s" % DT)
-                self.DT = DT
-
-            file_pattern = self.file_pattern
-            if file_pattern is None:
-                file_pattern = ".tif"
-                try:
-                    input_file_pattern = str(
-                        input('File pattern (default is ".tif") : ')
-                    )
-                    if len(input_file_pattern) > 0:
-                        file_pattern = input_file_pattern
-
-                except BaseException as e:
-                    print(e)
-                    print("Incorrect value, keeping default : %.2f s" % DT)
-                self.file_pattern = file_pattern
-
-            exp_info = {
-                "data_path": self.data_folder,
-                "pixel_size": self.pixel_size,
-                "file_pattern": self.file_pattern,
-                "DT": self.DT,
-            }
-            json.dump(
-                exp_info,
-                open(json_path, "w"),
-            )
-        else:
+            
+        exp_info = {}
+        if os.path.exists(json_path):
             # Read the JSON file and check that path of origin data is the same
             logging.info("JSON already exists : %s" % json_path)
             exp_info = json.load(open(json_path, "r"))
 
-            if not os.path.samefile(self.data_folder, exp_info["data_path"]):
+            if os.path.exists(exp_info["data_path"]) and not os.path.samefile(self.data_folder, exp_info["data_path"]):
                 logging.debug("Data folder is %s" % self.data_folder)
                 logging.debug(
                     "Data path in JSON in %s" % exp_info["data_path"]
                 )
-        self.DT = exp_info["DT"]
-        self.pixel_size = exp_info["pixel_size"]
-        self.file_pattern = exp_info["file_pattern"]
+                
+        if self.pixel_size is None and "pixel_size" in exp_info:
+            self.pixel_size = exp_info["pixel_size"]
+        elif self.pixel_size is not None:
+            exp_info["pixel_size"] = self.pixel_size
+        else:
+            pixel_size = 0.097
+            try:
+                pixel_size = float(
+                    input("Pixel size, in microns (default is 0.097) : ")
+                )
+            except BaseException as e:
+                print(e)
+                print(
+                    "Incorrect value, keeping default : %.2f um"
+                    % pixel_size
+                )
+            self.pixel_size = pixel_size
+            exp_info["pixel_size"] = self.pixel_size
+            
+        if self.DT is None and "DT" in exp_info:
+            self.DT = exp_info["DT"]
+        elif self.DT is not None:
+            exp_info["DT"] = self.DT
+        else:
+            DT = 0.03
+            try:
+                DT = float(
+                    input(
+                        "Time interval between successive frames, in seconds (default is 0.03) : "
+                    )
+                )
+            except BaseException as e:
+                print(e)
+                print("Incorrect value, keeping default : %.2f s" % DT)
+            self.DT = DT
+            exp_info["DT"] = DT
+            
+        if self.file_pattern is None and "file_pattern" in exp_info:
+            self.file_pattern = exp_info["file_pattern"]
+        elif self.file_pattern is not None:
+            exp_info["file_pattern"] = self.file_pattern
+        else:
+            print("Using a new file pattern")
+            file_pattern = ".tif"
+            try:
+                input_file_pattern = str(
+                    input('File pattern (default is ".tif") : ')
+                )
+                if len(input_file_pattern) > 0:
+                    file_pattern = input_file_pattern
+
+            except BaseException as e:
+                print(e)
+                print("Incorrect value, keeping default : %s s" % file_pattern)
+            self.file_pattern = file_pattern
+            
+        
+
+        exp_info = {
+            "data_path": self.data_folder,
+            "pixel_size": self.pixel_size,
+            "file_pattern": self.file_pattern,
+            "DT": self.DT,
+        }
+        json.dump(
+            exp_info,
+            open(json_path, "w"),
+        )
 
     @property
     def index_df(self) -> pd.DataFrame:
         if not hasattr(self, "_index_df"):
             if not os.path.exists(self.index_path):
                 self._index_df = pd.DataFrame(columns=["file", "ID"])
             else:
@@ -209,27 +195,14 @@
         .. code-block:: python3
 
             {"condition":get_condition_from_name}
 
         """
         return {}
 
-    """
-    @property
-    def available_processing_runs(self) -> List[TifProcessingRun]:
-        if not hasattr(self, "_processing_runs"):
-            os.chdir(self.export_folder)
-            run_param_files = glob("*/run_params.json", recursive=True)
-            logging.info("%d available processing runs" % len(run_param_files))
-            self._processing_runs = [
-                TifProcessingRun.from_json(f, self) for f in run_param_files
-            ]
-        return self._processing_runs
-    """
-
     @property
     def all_files(self) -> List[str]:
         """Return all files indexed in self.index_df
 
         Returns:
             List[Acquisition]: all files indexed in self.index_df
         """
@@ -264,15 +237,15 @@
                 raise
         files = self.index_df.loc[cond].file.tolist()
         if only_processed_with_run is not None:
             files = [
                 f
                 for f in files
                 if Acquisition(
-                    f, experiment=self, tif_pipeline=only_processed_with_run
+                    f, experiment=self, image_pipeline=only_processed_with_run
                 ).is_processed
             ]
         return files
     """
 
     def add_new_roi_to_index(self, f: str):
         row = pd.DataFrame.from_dict(
@@ -286,20 +259,18 @@
 
     def remove_old_roi_from_index(self, f: str):
         assert f in self.index_df["file"].tolist()
         self.index_df = self.index_df.loc[self.index_df.file != f]
         logging.info("Removed in index the row %s" % f)
 
     def scan_folder(self) -> list:
-        os.chdir(self.data_folder)
-        roi_files = glob("**/*%s" % self.file_pattern, recursive=True)
+        roi_files = glob(os.path.join(self.data_folder,"**","*%s" % self.file_pattern), recursive=True)
         roi_files = [
             f for f in roi_files if os.path.getsize(f) > 1e6
         ]  # Don't consider files of less than 1Mb
-        # TODO: improve filtering here
         return roi_files
 
     def look_for_updates(self):
         """
         Look if the index dataframe matches
         the reality of present/absent files
         And computes custom columns if needed
@@ -319,17 +290,17 @@
             if f not in roi_files:
                 self.remove_old_roi_from_index(f)
 
         self.look_for_new_columns()
 
     def get_ID_of_acq(self, acquisition: Acquisition):
         ID = self.index_df.loc[
-            self.index_df.file == acquisition.tif_file, "ID"
+            self.index_df.file == acquisition.image_file, "ID"
         ].values[0]
-        logging.debug("ID of file %s is %s" % (acquisition.tif_file, ID))
+        logging.debug("ID of file %s is %s" % (acquisition.image_file, ID))
         return str(ID)
 
     def look_for_new_columns(self, overwrite=False):
         """
         Computes custom columns
 
         Args:
```

### Comparing `palmari-0.2.8/src/palmari/processing/edit_pipeline_window.py` & `palmari-0.3.0/src/palmari/processing/edit_pipeline_window.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     QHBoxLayout,
     QPushButton,
     QStyle,
     QTreeWidget,
     QTreeWidgetItem,
 )
 from qtpy import QtCore
-
+import logging
 from magicgui.widgets import LineEdit
 
-from .tif_pipeline import TifPipeline
+from .image_pipeline import ImagePipeline
 
 
 class PipelineEditor(QDialog):
-    def __init__(self, tif_pipeline: TifPipeline):
+    def __init__(self, image_pipeline: ImagePipeline):
         super().__init__()
 
-        self.initial_tp_dict = dict(tif_pipeline.to_dict())
-        self.tp = tif_pipeline
+        self.initial_tp_dict = dict(image_pipeline.to_dict())
+        self.tp = image_pipeline
         self.setup_ui()
         self.selected_class(None)
         self.setModal(True)
 
     def setup_ui(self):
         main_layout = QVBoxLayout()
 
@@ -88,23 +88,33 @@
         action_buttons_layout.addWidget(doneButton)
 
         main_layout.addLayout(action_buttons_layout)
 
     def populate_steps_view(self):
         try:
             self.steps_view.currentItemChanged.disconnect()
-        except TypeError as e:
+        except Exception as e:
+            logging.error("For some reason, could not disconnect the currentItemChanged slot")
+            logging.error(e)
             pass
 
         self.steps_view.clear()
         for step_type, steps in self.tp.available_steps.items():
             step_type_item = QTreeWidgetItem()
             # Indicate that it cannot be selected, using Flags
             step_type_item.setFlags(QtCore.Qt.ItemIsEnabled)
             step_type_item.setText(0, step_type)
+            
+            # First, we display all present stpes, in the correct order
+            included_steps = [s for s in steps if self.tp.contains_class(s[0])]
+            included_steps_indices = [self.tp.index_of(s[0]) for s in included_steps]
+            included_steps = [included_steps[i] for i in included_steps_indices]
+            # Then, all other possible steps
+            not_included_steps = [s for s in steps if not self.tp.contains_class(s[0])]
+            steps = included_steps + not_included_steps
             for (step_name, step_class) in steps:
                 step_item = QTreeWidgetItem()
                 step_item.setText(0, step_name)
                 step_item.setData(0, 0, step_name)
                 step_item.setData(0, 1, step_class)
                 step_item.setIcon(
                     0,
@@ -116,15 +126,15 @@
             self.steps_view.addTopLevelItem(step_type_item)
         self.steps_view.currentItemChanged.connect(self.selected_class)
         self.steps_view.itemSelectionChanged.connect(self.selected_index)
         self.steps_view.expandAll()
         self.selected_index()
 
     def cancel(self):
-        self.tp = TifPipeline.from_dict(self.initial_tp_dict)
+        self.tp = ImagePipeline.from_dict(self.initial_tp_dict)
         self.reject()
 
     def selected_index(self):
         if len(self.steps_view.selectedItems()) == 0:
             self.addButton.setDisabled(True)
             self.removeButton.setDisabled(True)
             self.upButton.setDisabled(True)
@@ -160,34 +170,42 @@
     def selected_step_name(self) -> str:
         try:
             step_item = self.steps_view.selectedItems()[0]
             step_name = step_item.text(0)
             return step_name
         except IndexError as e:
             return None
-
-    def move_step_up(self):
+        
+    def move_step(self, up):
         step_name = self.selected_step_name()
         if step_name is None:
             return
         step_type = self.tp.step_type_of(step_name)
         old_index = self.tp.index_of(step_name)
-        new_index = max(old_index - 1, 0)
-        self.tp[step_type].insert(new_index, self.tp[step_type].pop(old_index))
+        tp_dict = self.tp.to_dict()
+        if up:
+            new_index = max(old_index - 1, 0)
+        else:
+            new_index = min(old_index + 1, len(tp_dict[step_type]) - 1)
+        #print("Step : %s \t New index : %d, old index: %d" % (step_name, new_index,old_index))
+        item = self.tp[step_type][old_index]
+        #print(tp_dict[step_type])
+        tp_dict[step_type].pop(old_index)
+        #print(tp_dict[step_type])
+        tp_dict[step_type].insert(new_index, item)
+        #print(tp_dict[step_type])
+        self.tp = ImagePipeline.from_dict(tp_dict)
+        #print(self.tp.to_dict())
         self.populate_steps_view()
 
+    def move_step_up(self):
+        self.move_step(up=True)
+
     def move_step_down(self):
-        step_name = self.selected_step_name()
-        if step_name is None:
-            return
-        step_type = self.tp.step_type_of(step_name)
-        old_index = self.tp.index_of(step_name)
-        new_index = max(old_index + 1, len(self.tp[step_type]) - 1)
-        self.tp[step_type].insert(new_index, self.tp[step_type].pop(old_index))
-        self.populate_steps_view()
+        self.move_step(up=False)
 
     def add_step(self):
         step_name = self.selected_step_name()
         if step_name is None:
             return
         step_type = self.tp.step_type_of(step_name)
         # print("Trying to add %s" % step_name)
```

### Comparing `palmari-0.2.8/src/palmari/processing/steps/base.py` & `palmari-0.3.0/src/palmari/processing/steps/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         return pd.DataFrame.from_dict(
             {"x": [], "y": [], "frame": []}, orient="columns"
         )
 
     def movie_detection(self, mov: da.Array):
         slice_size = mov.chunksize[0]
         n_slices = mov.shape[0] // slice_size
+        logging.warn("Slice size is %d, image is cut in %d slices" % (slice_size, n_slices))
         positions_dfs = []
         for i in range(n_slices + 1):
             start = i * slice_size
             end = min((i + 1) * slice_size, mov.shape[0])
             if start >= end:
                 continue
             positions_dfs.append(
@@ -210,15 +211,15 @@
     }
 
     @abstractmethod
     def localize_frame(
         self, img: np.array, detections: np.array
     ) -> pd.DataFrame:
         """
-        Extract localizations from a slice of a .tif file. Override in subclasses
+        Extract localizations from a slice of an image file. Override in subclasses
 
         Args:
             img (np.array): 2D array [X, Y]
 
             detections (np.array):  2D array [X, Y] center of spots (pixel indices)
 
         Returns:
```

### Comparing `palmari-0.2.8/src/palmari/processing/steps/drift_corrector.py` & `palmari-0.3.0/src/palmari/processing/steps/drift_corrector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import *
-from ...tif_tools.correct_drift import correct_drift
+from ...image_tools.correct_drift import correct_drift
 from dask_image.ndfilters import gaussian_filter
 from .quot_localizer import BaseDetector, MaxLikelihoodLocalizer
 from scipy.ndimage import gaussian_filter1d
 from scipy.interpolate import interp1d
 
 
 class CorrelationDriftCorrector(LocProcessor):
```

### Comparing `palmari-0.2.8/src/palmari/processing/steps/quot_localizer.py` & `palmari-0.3.0/src/palmari/processing/steps/quot_localizer.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/processing/steps/quot_tracker.py` & `palmari-0.3.0/src/palmari/processing/steps/quot_tracker.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/processing/steps/trackpy_tracker.py` & `palmari-0.3.0/src/palmari/processing/steps/trackpy_tracker.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/processing/steps/window_percentile.py` & `palmari-0.3.0/src/palmari/processing/steps/window_percentile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import *
-from ...tif_tools.localization import sliding_window_filter
+from ...image_tools.localization import sliding_window_filter
 
 
 class WindowPercentileFilter(MoviePreProcessor):
 
     widget_types = {"percentile": "FloatSpinBox", "window_size": "SpinBox"}
     widget_options = {
         "percentile": {
```

### Comparing `palmari-0.2.8/src/palmari/processing/tif_pipeline.py` & `palmari-0.3.0/src/palmari/processing/image_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import yaml
 
 from ..data_structure.acquisition import Acquisition
 from ..data_structure.experiment import Experiment
 from .steps import *
 
 
-class TifPipeline:
+class ImagePipeline:
     def __init__(
         self,
         name: str,
         movie_preprocessors: List[MoviePreProcessor],
         detector: Detector,
         localizer: SubpixelLocalizer,
         loc_processors: List[LocProcessor],
@@ -26,14 +26,17 @@
         self.movie_preprocessors = movie_preprocessors
         self.detector = detector
         self.localizer = localizer
         self.loc_processors = loc_processors
         self.tracker = tracker
         self.last_storage_path = None
 
+    def __getitem__(self, item):
+        return self.to_dict()[item]
+
     @classmethod
     def from_dict(cls, p: Dict):
         """
         Instantiate from a dictionnary.
         Here's an example Dictionnary which could be passed as an argument :
 
         .. code-block:: python3
@@ -202,18 +205,18 @@
     def index_of(self, step):
         d = self.to_dict()
         for step_type, steps in d.items():
             if step_type == "name":
                 continue
             if isinstance(steps, list):
                 # Si possible d'avoir plusieurs items, on trouve le rang
-                for step_dict in steps:
-                    for i, option in enumerate(step_dict):
-                        if step == option:
-                            return step_type
+                for step_num, step_dict in enumerate(steps):
+                    step_name = list(step_dict.keys())[0]
+                    if step_name == step: 
+                        return step_num
             else:
                 assert isinstance(steps, dict), steps
                 # Sinon, on renvoie zéro parce qu'il n'y a forcément qu'un step
                 if step in steps:
                     return 0
         return None
 
@@ -339,15 +342,15 @@
             )
         elif isinstance(to_process, Experiment):
 
             # Actually process, acquisition after acquisition
 
             for i, acq_file in enumerate(to_process):
                 acq = Acquisition(
-                    acq_file, experiment=to_process, tif_pipeline=self
+                    acq_file, experiment=to_process, image_pipeline=self
                 )
                 if i == 0:
                     pipeline_export_path_for_exp = self.exp_params_path(acq)
                     logging.info(
                         "Saving pipeline to %s" % pipeline_export_path_for_exp
                     )
                     self.to_yaml(pipeline_export_path_for_exp)
```

### Comparing `palmari-0.2.8/src/palmari/processing/tif_pipeline_widget.py` & `palmari-0.3.0/src/palmari/processing/image_pipeline_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     QPushButton,
     QSplitter,
     QGroupBox,
     QFileDialog,
     QScrollArea,
     QTabWidget,
 )
+from qtpy.compat import getsavefilename
 
 from magicgui.widgets import FileEdit
 from functools import partial
 
 
 from napari.qt import thread_worker
 from magicgui.widgets import (
@@ -32,15 +33,15 @@
 import enum
 import dask.array as da
 import dask_image
 import pandas as pd
 import logging
 import os
 from ..data_structure.acquisition import Acquisition
-from .tif_pipeline import TifPipeline, ProcessingStep
+from .image_pipeline import ImagePipeline, ProcessingStep
 from .edit_pipeline_window import PipelineEditor
 
 
 class handled_types(enum.Enum):
     image = "Image"
     points = "Points"
     tracks = "Tracks"
@@ -73,25 +74,25 @@
             )
             self.widgets_dict[param] = widget
 
             widget.changed.connect(partial(step.update_param, param))
         super().__init__(widgets=[w for _, w in self.widgets_dict.items()])
 
 
-class TifPipelineWidget(QWidget):
+class ImagePipelineWidget(QWidget):
     def __init__(
-        self, tif_pipeline: TifPipeline, napari_viewer: napari.Viewer
+        self, image_pipeline: ImagePipeline, napari_viewer: napari.Viewer
     ):
         super().__init__()
 
-        self.pixel_size = 0.093
+        self.pixel_size = 1.00
         self.delta_t = 0.03
         self.to_export = None
         self.viewer = napari_viewer
-        self.tp = tif_pipeline
+        self.tp = image_pipeline
         self._init_layers_dict()
         self.setup_ui()
 
     def activate_buttons(self, last_clicked: int = 0):
         for button_index, button in self._buttons.items():
             enable = button_index <= last_clicked + 1
             button.setEnabled(enable)
@@ -267,15 +268,15 @@
         main_layout = QVBoxLayout()
         main_layout.addWidget(main_box)
 
         return main_layout
 
     def load_pipeline(self, file_path):
         try:
-            tp = TifPipeline.from_yaml(file_path)
+            tp = ImagePipeline.from_yaml(file_path)
         except BaseException as e:
             logging.error(e)
             logging.error(
                 "Could not load pipeline from file %s, check the format"
                 % file_path
             )
             return
@@ -327,28 +328,31 @@
         self.export_locs_button.clicked.connect(self.export_locs)
         export_pipeline_button.clicked.connect(self.export_pipeline)
 
         return main_layout
 
     def export_locs(self):
         assert self.to_export is not None
-        fileName, _ = QFileDialog.getSaveFileName(
-            self,
+        fileName, _ = getsavefilename(
+            parent=self,
             caption="Export localizations and tracks",
-        )
+            )
         logging.debug(fileName)
         if fileName is not None and len(fileName) > 2:
+            if "." not in fileName:
+                fileName = "%s.csv" % fileName
             self.to_export.to_csv(fileName, index=True)
 
     def export_pipeline(self):
-        fileName, _ = QFileDialog.getSaveFileName(
-            self,
-            directory=self.tp.last_storage_path,
+        fileName, _ = getsavefilename(
+            parent=self,
+            basedir=self.tp.last_storage_path,
             caption="Save pipeline parameters",
         )
+        
         logging.debug(fileName)
 
         if fileName is not None and len(fileName) > 2:
             if ".yaml" not in fileName:
                 fileName = "%s.yaml" % fileName
             self.tp.to_yaml(fileName)
 
@@ -488,47 +492,46 @@
                 self.activate_buttons(last_clicked=btn_index - 1)
             if is_final_step:
                 self.to_export = data
             else:
                 self.to_export = None
             self.export_locs_button.setEnabled(is_final_step)
 
+        def to_dask(array):
+            if isinstance(array, da.Array):
+                return array
+            else:
+                return da.from_array(array)
+
         @thread_worker(connect={"returned": add_layer})
         def run_step(checked: bool = True):
             logging.debug(self._layers)
             assert input_layer_idx in self._layers
             self.setEnabled(False)
             if input_type == handled_types.image:
-                input_data = (self._layers[input_layer_idx].data,)
+                input_data = (to_dask(self._layers[input_layer_idx].data),)
             elif input_type == handled_types.points:
                 input_data = (self._layers[input_layer_idx].result,)
             elif input_type == handled_types.tracks:
                 input_data = (self._layers[input_layer_idx].result,)
             elif input_type == handled_types.detections:
                 detections = pd.DataFrame(
                     data=self._layers[input_layer_idx].data.copy(),
                     columns=["frame", "x", "y"],
                 )
                 detections[["x", "y"]] /= self.pixel_size
                 # On inverse x et y volontairement
                 detections[["y", "x"]] = detections[["x", "y"]].astype(int)
                 input_data = (
-                    self._layers[input_layer_idx - 1].data,
+                    to_dask(self._layers[input_layer_idx - 1].data),
                     detections,
                 )
             elif input_type == handled_types.image_locs_and_pixel_size:
-                # detections = pd.DataFrame(
-                #    data=self._layers[input_layer_idx].data.copy(),
-                #    columns=["frame", "x", "y"],
-                # )
-                # detections[["x", "y"]] /= self.pixel_size
-                # On inverse x et y volontairement
-                # detections[["y", "x"]] = detections[["x", "y"]].astype(int)
                 input_data = (
-                    self._layers[0].data,
+                    to_dask(self._layers[0].data),
                     self._layers[input_layer_idx].result,
                     self.pixel_size,
                 )
             return step.process(*input_data)
 
         step_run_btn.clicked.connect(run_step)
 
@@ -573,30 +576,32 @@
             )
             self._layers[layer_idx] = new_layer
         else:
             self._layers[layer_idx].data = returned_image
 
     def add_points_layer(
         self,
-        points,
+        points: pd.DataFrame,
         layer_idx: int,
         step_name: str,
     ):
 
         if layer_idx not in self._layers:
-            new_layer = self.viewer.add_points(
-                points[["frame", "x", "y"]].values,
-                properties=points[
+            points_ = points.astype({"x":float,"y":float,"frame":float})
+            properties = points_[
                     [
                         c
-                        for c in points.columns
+                        for c in points_.columns
                         if (c not in ["x", "y"])
-                        and (points[c].dtype.kind in "uifb")
+                        and (points_[c].dtype.kind in "uifb")
                     ]
-                ].to_dict(),
+                ].to_dict(orient="list")
+            new_layer = self.viewer.add_points(
+                points_[["frame", "x", "y"]].values,
+                properties=properties,
                 symbol="disc",
                 size=0.25,
                 edge_width=0.1,
                 face_color="transparent" if (points.shape[0] > 0) else None,
                 edge_color="frame" if (points.shape[0] > 0) else None,
                 edge_colormap="rainbow",
                 blending="translucent_no_depth",
@@ -633,37 +638,32 @@
             self._layers[layer_idx].tracks = tracks
 
         self._layers[layer_idx].result = tracks
 
     @classmethod
     def view_pipeline(
         cls,
-        tif_pipeline: TifPipeline,
+        image_pipeline: ImagePipeline,
         acq: Acquisition = None,
-        tif_file: str = None,
+        image_file: str = None,
     ):
         napari.Viewer()
         viewer = napari.current_viewer()
-        widget = cls(tif_pipeline, viewer)
+        widget = cls(image_pipeline, viewer)
 
         if acq is not None:
             widget.pixel_size = acq.experiment.pixel_size
             widget.delta_t = acq.experiment.DT
             viewer.add_image(
                 data=acq.image,
-                name=acq.tif_file.split(os.path.sep)[-1],
+                name=acq.image_file.split(os.path.sep)[-1],
                 scale=(1.0, widget.pixel_size, widget.pixel_size),
             )
-        elif tif_file is not None:
-            viewer.add_image(
-                data=dask_image.imread.imread(
-                    tif_file,
-                    nframes=300,
-                )
-            )
+        elif image_file is not None:
+            viewer.open(image_file)
 
         viewer.window.add_dock_widget(
             widget=widget,
-            name="PALM pipeline : %s" % tif_pipeline.name,
+            name="PALM pipeline : %s" % image_pipeline.name,
             area="right",
         )
         widget.rescale_image_layers()
```

### Comparing `palmari-0.2.8/src/palmari/processing/utils.py` & `palmari-0.3.0/src/palmari/processing/utils.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/__init__.py` & `palmari-0.3.0/src/palmari/quot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 """
 # Enforce PySide2 backend to pyqtgraph
 # import PySide2
 # import pyqtgraph
 
 # Core functions to run localization and tracking on single files
 # or directories
-from .core import (
-    localize_file,
-    track_file,
-    track_directory,
-    retrack_file,
-    retrack_files,
-)
+# from .core import (
+#    localize_file,
+#    track_file,
+#    track_directory,
+#    retrack_file,
+#    retrack_files,
+# )
 
 # Read and filter image files
-from .read import ImageReader, read_config
-from .chunkFilter import ChunkFilter
+#from .read import ImageReader, read_config
+#from .chunkFilter import ChunkFilter
 
 # Find spots
 from .findSpots import detect
 
 # Localize spots to subpixel resolution
 from .subpixel import localize, localize_frame
```

### Comparing `palmari-0.2.8/src/palmari/quot/__main__.py` & `palmari-0.3.0/src/palmari/quot/__main__.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/chunkFilter.py` & `palmari-0.3.0/src/palmari/quot/chunkFilter.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/core.py` & `palmari-0.3.0/src/palmari/quot/core.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/findSpots.py` & `palmari-0.3.0/src/palmari/quot/findSpots.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/helper.py` & `palmari-0.3.0/src/palmari/quot/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # Warnings, to filter out warnings for a potentially dangerous
 # division in rs() that is subsequent corrected
 import warnings 
 
 # Profiling
 from time import time 
 
-from .plot import wireframe_overlay
+# from .plot import wireframe_overlay
 
 def time_f(f):
     """
     Decorator. When executing the decorated function,
     also print the time to execute.
 
     args
```

### Comparing `palmari-0.2.8/src/palmari/quot/mask.py` & `palmari-0.3.0/src/palmari/quot/mask.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/measureGain.py` & `palmari-0.3.0/src/palmari/quot/measureGain.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/plot.py` & `palmari-0.3.0/src/palmari/quot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 import sys
 import os 
 
 # Numeric
 import numpy as np 
 from scipy import ndimage as ndi 
 
-# Image file reader
-from nd2reader import ND2Reader 
-
 # Dataframes, for handling trajectories
 import pandas as pd 
 
 # Core matplotlib library
 import matplotlib.pyplot as plt 
 
 # Color schema
@@ -134,14 +131,16 @@
         scalebar    :   bool, make a scalebar
 
     returns
     -------
         None; plots directly to *axes*
 
     """
+    from nd2reader import ND2Reader 
+    
     reader = ND2Reader(nd2_path)
     mip = reader.get_frame(0).astype(np.float64)
     for frame_idx in range(1, reader.metadata["total_images_per_channel"]):
         try:
             mip = np.maximum(mip, reader.get_frame(frame_idx))
         except:
             continue
```

### Comparing `palmari-0.2.8/src/palmari/quot/read.py` & `palmari-0.3.0/src/palmari/quot/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # File paths
 import os
 
 # Read config files in TOML format
 import toml 
 
 # Underlying file readers for each file format
-import tifffile
-from nd2reader import ND2Reader 
 
 def read_config(path):
     """
     Read a config file.
 
     args
         path    :   str
@@ -70,17 +68,19 @@
 
         assert os.path.isfile(path), "ImageReader.__init__: " \
             "path %s does not exist" % path 
         self.path = path
 
         if '.nd2' in path:
             self.ext = '.nd2'
+            from nd2reader import ND2Reader 
             self._reader = ND2Reader(path)
         elif ('.tif' in path) or ('.tiff' in path):
             self.ext = '.tif'
+            import tifffile
             self._reader = tifffile.TiffFile(path)
         #elif ('.czi' in path):
         #    self.ext = '.czi'
         #    self._reader = CziFile(path)
         else:
             raise RuntimeError("Image format %s not recognized" % \
                 os.path.splitext(path)[1])
```

### Comparing `palmari-0.2.8/src/palmari/quot/subpixel.py` & `palmari-0.3.0/src/palmari/quot/subpixel.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/track.py` & `palmari-0.3.0/src/palmari/quot/track.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/quot/trajUtils.py` & `palmari-0.3.0/src/palmari/quot/trajUtils.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/tif_tools/cell_mask.py` & `palmari-0.3.0/src/palmari/image_tools/cell_mask.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/tif_tools/correct_drift.py` & `palmari-0.3.0/src/palmari/image_tools/correct_drift.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/tif_tools/density_filtering.py` & `palmari-0.3.0/src/palmari/image_tools/density_filtering.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/tif_tools/intensity.py` & `palmari-0.3.0/src/palmari/image_tools/intensity.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.8/src/palmari/tif_tools/localization.py` & `palmari-0.3.0/src/palmari/image_tools/localization.py`

 * *Files 15% similar despite different names*

```diff
@@ -275,68 +275,8 @@
         spot["sigma"] = sigma
         spot["total_intensity"] = np.sum(img)
         spots[i] = spot
     spots = pd.DataFrame.from_dict(spots, orient="index")
     if return_all:
         return spots, is_peak, F2
     else:
-        return spots
-
-
-def localize_movie(
-    movie: Any,  # Dask or numpy
-    factor: float = 1.0,
-    filter_size: int = 3,
-    sliding_filter: bool = False,
-    verbose: bool = False,
-    subpixel_mode: str = "radial",
-    progress_bar: bool = False,
-):
-
-    data = movie.astype(float)
-    if sliding_filter:
-        logging.debug("Sliding filter starts")
-        logging.info("Computing sliding filter...")
-        data = sliding_window_filter(data)
-        logging.info("... Done !")
-        logging.debug("Sliding filter done")
-
-    logging.debug("Converted to float")
-    # TODO: progress_bar does not work
-
-    slice_size = data.chunksize[0]
-    n_slices = data.shape[0] // slice_size
-    positions_dfs = []
-    for i in range(n_slices + 1):
-        start = i * slice_size
-        end = min((i + 1) * slice_size, data.shape[0])
-        if start >= end:
-            continue
-        positions_dfs.append(
-            delayed(SMLM_localization)(
-                data[start:end],
-                factor=factor,
-                return_all=False,
-                verbose=verbose,
-                filter_size=filter_size,
-                subpixel_mode=subpixel_mode,
-                frame_start=start,
-            )
-        )
-    loc_results_del = dd.from_delayed(
-        positions_dfs,
-        verify_meta=False,
-        meta={
-            "x": float,
-            "y": float,
-            "frame": int,
-            "sigma": float,
-            "ratio": float,
-            "total_intensity": float,
-        },
-    )
-    with ProgressBar():
-        loc_results = loc_results_del.compute()
-    loc_results.set_index(np.arange(loc_results.shape[0]), inplace=True)
-    logging.debug(loc_results.head(10))
-    logging.debug(loc_results.tail(10))
-    return loc_results
+        return spots
```

### Comparing `palmari-0.2.8/src/palmari.egg-info/PKG-INFO` & `palmari-0.3.0/src/palmari.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: palmari
-Version: 0.2.8
-Summary: A pipeline for PALM movies analysis (pre-processing, localization, drifft correction, tracking)
+Version: 0.3.0
+Summary: Palmari provides a plugin to analyze PALM movies, as well as microscope recordings of other SMLM-based SPT modalities. Set up your pipeline on one file, run it on a folder !
 Home-page: https://github.com/hippover/palmari
 Author: Hippolyte Verdier
 Author-email: hverdier@pasteur.fr
 License: "CeCILL"
 Project-URL: Bug Tracker, https://github.com/hippover/palmari/issues
 Project-URL: Documentation, https://palmari.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/hippover/palmari
 Project-URL: User Support, https://github.com/hippover/palmari/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
+Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -35,15 +36,15 @@
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/palmari)](https://napari-hub.org/plugins/palmari)
 [![License](https://img.shields.io/pypi/l/palmari.svg?color=green)](https://github.com/hippover/palmari/raw/main/LICENSE)
 
 A processing pipeline for PALM movies analysis (pre-processing, localization, drift correction, tracking).
 
 Check out the [documentation] to get started.
 
-![napari_plugin](docs/images/plugin_steps.png "Fine-tune your pipelines on a movie, run it on a batch easily !")
+![napari_plugin](https://github.com/hippover/palmari/raw/main/docs/images/plugin_steps.png "Fine-tune your pipelines on a movie, run it on a batch easily !")
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `palmari-0.2.8/src/palmari.egg-info/SOURCES.txt` & `palmari-0.3.0/src/palmari.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,24 @@
 src/palmari.egg-info/requires.txt
 src/palmari.egg-info/top_level.txt
 src/palmari/_tests/__init__.py
 src/palmari/_tests/test_widget.py
 src/palmari/data_structure/__init__.py
 src/palmari/data_structure/acquisition.py
 src/palmari/data_structure/experiment.py
+src/palmari/image_tools/__init__.py
+src/palmari/image_tools/cell_mask.py
+src/palmari/image_tools/correct_drift.py
+src/palmari/image_tools/density_filtering.py
+src/palmari/image_tools/intensity.py
+src/palmari/image_tools/localization.py
 src/palmari/processing/__init__.py
 src/palmari/processing/edit_pipeline_window.py
-src/palmari/processing/tif_pipeline.py
-src/palmari/processing/tif_pipeline_widget.py
+src/palmari/processing/image_pipeline.py
+src/palmari/processing/image_pipeline_widget.py
 src/palmari/processing/utils.py
 src/palmari/processing/steps/__init__.py
 src/palmari/processing/steps/base.py
 src/palmari/processing/steps/drift_corrector.py
 src/palmari/processing/steps/quot_localizer.py
 src/palmari/processing/steps/quot_tracker.py
 src/palmari/processing/steps/trackpy_tracker.py
@@ -39,14 +45,8 @@
 src/palmari/quot/helper.py
 src/palmari/quot/mask.py
 src/palmari/quot/measureGain.py
 src/palmari/quot/plot.py
 src/palmari/quot/read.py
 src/palmari/quot/subpixel.py
 src/palmari/quot/track.py
-src/palmari/quot/trajUtils.py
-src/palmari/tif_tools/__init__.py
-src/palmari/tif_tools/cell_mask.py
-src/palmari/tif_tools/correct_drift.py
-src/palmari/tif_tools/density_filtering.py
-src/palmari/tif_tools/intensity.py
-src/palmari/tif_tools/localization.py
+src/palmari/quot/trajUtils.py
```

