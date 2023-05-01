# Comparing `tmp/mmlab_lightning-1.0.1.tar.gz` & `tmp/mmlab_lightning-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmlab_lightning-1.0.1.tar", last modified: Mon May  1 08:20:39 2023, max compression
+gzip compressed data, was "mmlab_lightning-1.0.2.tar", last modified: Mon May  1 09:48:00 2023, max compression
```

## Comparing `mmlab_lightning-1.0.1.tar` & `mmlab_lightning-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/datasets/mmlab_dataset_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/models/mmlab_model_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/tools/config/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/tools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/tools/config/get_mmconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/mmlab_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/mmlab_lightning/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/datasets/mmlab_dataset_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/mmlab_lightning/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/models/mmlab_model_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/mmlab_lightning/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/mmlab_lightning/tools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/mmlab_lightning/tools/config/get_mmconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 09:48:00.000000 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-01 09:48:00.000000 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:48:00.000000 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 09:48:00.000000 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 09:48:00.000000 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 09:48:00.000000 mmlab_lightning-1.0.2/mmlab_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 09:48:00.847554 mmlab_lightning-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-01 09:47:49.000000 mmlab_lightning-1.0.2/setup.py
```

### Comparing `mmlab_lightning-1.0.1/LICENSE` & `mmlab_lightning-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.1/PKG-INFO` & `mmlab_lightning-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab_lightning
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab_lightning-1.0.1/README.md` & `mmlab_lightning-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.1/mmlab_lightning/datasets/mmlab_dataset_adapter.py` & `mmlab_lightning-1.0.2/mmlab_lightning/datasets/mmlab_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.1/mmlab_lightning/models/mmlab_model_adapter.py` & `mmlab_lightning-1.0.2/mmlab_lightning/models/mmlab_model_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 import torch
 from lightning_template.models import LightningModule
 from mmengine.model import BaseModule
 from torch import nn
 
 
 class MMLabModelAdapter(LightningModule, BaseModule, ABC):
-    def __init__(
-        self,
-        visualizer_kwargs=None,
-        *args,
-        **kwargs,
-    ):
+    def __init__(self, visualizer_kwargs=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if visualizer_kwargs is None:
             self.visualizer_kwargs = {}
         else:
             self.visualizer_kwargs = visualizer_kwargs
```

### Comparing `mmlab_lightning-1.0.1/mmlab_lightning.egg-info/PKG-INFO` & `mmlab_lightning-1.0.2/mmlab_lightning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab_lightning-1.0.1/mmlab_lightning.egg-info/SOURCES.txt` & `mmlab_lightning-1.0.2/mmlab_lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.1/setup.py` & `mmlab_lightning-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mmlab_lightning",
-    version="1.0.1",
+    version="1.0.2",
     description="A wrapper for mmlab repos to use in project_template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/mmlab_lightning",
     project_urls={
```

