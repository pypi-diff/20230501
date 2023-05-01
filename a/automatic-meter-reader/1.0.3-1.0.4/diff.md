# Comparing `tmp/automatic-meter-reader-1.0.3.tar.gz` & `tmp/automatic-meter-reader-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-meter-reader-1.0.3.tar", last modified: Sun Apr 16 19:43:05 2023, max compression
+gzip compressed data, was "automatic-meter-reader-1.0.4.tar", last modified: Mon May  1 10:34:58 2023, max compression
```

## Comparing `automatic-meter-reader-1.0.3.tar` & `automatic-meter-reader-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.132523 automatic-meter-reader-1.0.3/automatic_meter_reader/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.132523 automatic-meter-reader-1.0.3/automatic_meter_reader/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/cameras/espcam_120_deg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.132523 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.132523 automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 19:43:05.000000 automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-16 19:43:05.000000 automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:43:05.000000 automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 19:43:05.000000 automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-16 19:43:05.000000 automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:43:05.136523 automatic-meter-reader-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    40523 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/tests/test_image.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/tests/test_image2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 19:42:33.000000 automatic-meter-reader-1.0.3/tests/test_readout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.813225 automatic-meter-reader-1.0.4/automatic_meter_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.813225 automatic-meter-reader-1.0.4/automatic_meter_reader/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/cameras/espcam_120_deg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.809225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.817225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.817225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.817225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.813225 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    40523 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/tests/test_image.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/tests/test_image2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/tests/test_readout.py
```

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/__init__.py` & `automatic-meter-reader-1.0.4/automatic_meter_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/cameras/espcam_120_deg.json` & `automatic-meter-reader-1.0.4/automatic_meter_reader/cameras/espcam_120_deg.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/meter_config.json` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg` & `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/automatic_meter_reader.egg-info/SOURCES.txt` & `automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/dev-requirements.txt` & `automatic-meter-reader-1.0.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/pyproject.toml` & `automatic-meter-reader-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
     "opencv-python",
-    "meter-digits-recognizer==0.1.12",
+    "meter-digits-recognizer==0.1.13",
 ]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/ardiloot/automatic-meter-reader"
 
 [project.optional-dependencies]
```

### Comparing `automatic-meter-reader-1.0.3/tests/test_image.jpg` & `automatic-meter-reader-1.0.4/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.3/tests/test_image2.jpg` & `automatic-meter-reader-1.0.4/tests/test_image2.jpg`

 * *Files identical despite different names*

