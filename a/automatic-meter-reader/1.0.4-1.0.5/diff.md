# Comparing `tmp/automatic-meter-reader-1.0.4.tar.gz` & `tmp/automatic-meter-reader-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-meter-reader-1.0.4.tar", last modified: Mon May  1 10:34:58 2023, max compression
+gzip compressed data, was "automatic-meter-reader-1.0.5.tar", last modified: Mon May  1 10:38:57 2023, max compression
```

## Comparing `automatic-meter-reader-1.0.4.tar` & `automatic-meter-reader-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.813225 automatic-meter-reader-1.0.4/automatic_meter_reader/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.813225 automatic-meter-reader-1.0.4/automatic_meter_reader/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/cameras/espcam_120_deg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.809225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.817225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.817225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.817225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.813225 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 10:34:58.000000 automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:34:58.821225 automatic-meter-reader-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    40523 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/tests/test_image.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/tests/test_image2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 10:34:26.000000 automatic-meter-reader-1.0.4/tests/test_readout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 10:38:26.000000 automatic-meter-reader-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 10:38:26.000000 automatic-meter-reader-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.914995 automatic-meter-reader-1.0.5/automatic_meter_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/automatic_meter_reader/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/cameras/espcam_120_deg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.914995 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 10:38:57.000000 automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-01 10:38:57.000000 automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:38:57.000000 automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 10:38:57.000000 automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 10:38:57.000000 automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:38:57.918995 automatic-meter-reader-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    40523 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/tests/test_image.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/tests/test_image2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 10:38:27.000000 automatic-meter-reader-1.0.5/tests/test_readout.py
```

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/__init__.py` & `automatic-meter-reader-1.0.5/automatic_meter_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/cameras/espcam_120_deg.json` & `automatic-meter-reader-1.0.5/automatic_meter_reader/cameras/espcam_120_deg.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/meter_config.json` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg` & `automatic-meter-reader-1.0.5/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/automatic_meter_reader.egg-info/SOURCES.txt` & `automatic-meter-reader-1.0.5/automatic_meter_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/dev-requirements.txt` & `automatic-meter-reader-1.0.5/dev-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # via pytest
 ipykernel==6.22.0
     # via
     #   automatic-meter-reader (setup.py)
     #   ipywidgets
 ipympl==0.9.3
     # via automatic-meter-reader (setup.py)
-ipython==8.12.0
+ipython==8.13.1
     # via
     #   ipykernel
     #   ipympl
     #   ipywidgets
 ipython-genutils==0.2.0
     # via ipympl
 ipywidgets==8.0.6
@@ -69,19 +69,19 @@
     #   ipympl
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
     # via flake8
-meter-digits-recognizer==0.1.12
+meter-digits-recognizer==0.1.13
     # via automatic-meter-reader (setup.py)
 nest-asyncio==1.5.6
     # via ipykernel
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   automatic-meter-reader (setup.py)
     #   contourpy
     #   ipympl
     #   matplotlib
     #   meter-digits-recognizer
     #   opencv-python
@@ -101,29 +101,29 @@
     # via ipython
 pillow==9.5.0
     # via
     #   ipympl
     #   matplotlib
 pip-tools==6.13.0
     # via automatic-meter-reader (setup.py)
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via jupyter-core
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 pure-eval==0.2.2
     # via stack-data
 pycodestyle==2.10.0
     # via flake8
 pyflakes==3.0.1
     # via flake8
-pygments==2.15.0
+pygments==2.15.1
     # via ipython
 pyparsing==3.0.9
     # via matplotlib
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via automatic-meter-reader (setup.py)
@@ -137,15 +137,15 @@
     # via
     #   ipykernel
     #   jupyter-client
 six==1.16.0
     # via python-dateutil
 stack-data==0.6.2
     # via ipython
-tornado==6.2
+tornado==6.3.1
     # via
     #   ipykernel
     #   jupyter-client
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
```

### Comparing `automatic-meter-reader-1.0.4/pyproject.toml` & `automatic-meter-reader-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/tests/test_image.jpg` & `automatic-meter-reader-1.0.5/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.0.4/tests/test_image2.jpg` & `automatic-meter-reader-1.0.5/tests/test_image2.jpg`

 * *Files identical despite different names*

