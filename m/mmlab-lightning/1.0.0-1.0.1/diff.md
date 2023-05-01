# Comparing `tmp/mmlab_lightning-1.0.0.tar.gz` & `tmp/mmlab_lightning-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmlab_lightning-1.0.0.tar", last modified: Sun Apr 30 14:47:06 2023, max compression
+gzip compressed data, was "mmlab_lightning-1.0.1.tar", last modified: Mon May  1 08:20:39 2023, max compression
```

## Comparing `mmlab_lightning-1.0.0.tar` & `mmlab_lightning-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 14:47:06.738243 mmlab_lightning-1.0.0/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1069 2023-04-30 14:38:46.000000 mmlab_lightning-1.0.0/LICENSE
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1378 2023-04-30 14:47:06.730243 mmlab_lightning-1.0.0/PKG-INFO
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      206 2023-04-30 14:46:40.000000 mmlab_lightning-1.0.0/README.md
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 14:47:06.526243 mmlab_lightning-1.0.0/mmlab_lightning/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 14:38:45.000000 mmlab_lightning-1.0.0/mmlab_lightning/__init__.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 14:47:06.658243 mmlab_lightning-1.0.0/mmlab_lightning/datasets/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       78 2023-04-30 14:41:40.000000 mmlab_lightning-1.0.0/mmlab_lightning/datasets/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1682 2023-04-30 14:41:18.000000 mmlab_lightning-1.0.0/mmlab_lightning/datasets/mmlab_dataset_adapter.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 14:47:06.714243 mmlab_lightning-1.0.0/mmlab_lightning/models/
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)       72 2023-04-30 14:42:26.000000 mmlab_lightning-1.0.0/mmlab_lightning/models/__init__.py
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     3138 2023-04-30 14:42:10.000000 mmlab_lightning-1.0.0/mmlab_lightning/models/mmlab_model_adapter.py
-drwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)        0 2023-04-30 14:47:06.594243 mmlab_lightning-1.0.0/mmlab_lightning.egg-info/
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)     1378 2023-04-30 14:47:06.000000 mmlab_lightning-1.0.0/mmlab_lightning.egg-info/PKG-INFO
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)      416 2023-04-30 14:47:06.000000 mmlab_lightning-1.0.0/mmlab_lightning.egg-info/SOURCES.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)        1 2023-04-30 14:47:06.000000 mmlab_lightning-1.0.0/mmlab_lightning.egg-info/dependency_links.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       19 2023-04-30 14:47:06.000000 mmlab_lightning-1.0.0/mmlab_lightning.egg-info/requires.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       16 2023-04-30 14:47:06.000000 mmlab_lightning-1.0.0/mmlab_lightning.egg-info/top_level.txt
--rw-rw-r--   0 zhengwenhao  (3017) zhengwenhao  (3017)       38 2023-04-30 14:47:06.738243 mmlab_lightning-1.0.0/setup.cfg
--rwxrwxr-x   0 zhengwenhao  (3017) zhengwenhao  (3017)     1505 2023-04-30 14:44:48.000000 mmlab_lightning-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/datasets/mmlab_dataset_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/models/mmlab_model_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning/tools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/mmlab_lightning/tools/config/get_mmconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 08:20:39.000000 mmlab_lightning-1.0.1/mmlab_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:20:39.608574 mmlab_lightning-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-01 08:20:19.000000 mmlab_lightning-1.0.1/setup.py
```

### Comparing `mmlab_lightning-1.0.0/LICENSE` & `mmlab_lightning-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.0/PKG-INFO` & `mmlab_lightning-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab_lightning
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
@@ -24,7 +24,25 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
 A wrapper based on [lightning-template](https://github.com/shenmishajing/lightning_template) for mmlab repos to use in [project-template](https://github.com/shenmishajing/project_template)
+
+## Feature
+
+All features from [lightning-template](https://github.com/shenmishajing/lightning_template)
+
+## Installation
+
+See [installation docs](docs/installation/installation.md) for details.
+
+## Usage
+
+### CLI
+
+See [tool docs](docs/tools/cli.md) for details.
+
+### Models and Datasets
+
+See [model doc](docs/core/model.md) and [dataset doc](docs/core/dataset.md) for details.
```

### Comparing `mmlab_lightning-1.0.0/mmlab_lightning/datasets/mmlab_dataset_adapter.py` & `mmlab_lightning-1.0.1/mmlab_lightning/datasets/mmlab_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.0/mmlab_lightning/models/mmlab_model_adapter.py` & `mmlab_lightning-1.0.1/mmlab_lightning/models/mmlab_model_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from abc import ABC
 
 import torch
+from lightning_template.models import LightningModule
 from mmengine.model import BaseModule
 from torch import nn
 
-from lightning_template.models import LightningModule
-
 
 class MMLabModelAdapter(LightningModule, BaseModule, ABC):
     def __init__(
         self,
-        model: nn.Module,
         visualizer_kwargs=None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.model = model
-
         if visualizer_kwargs is None:
             self.visualizer_kwargs = {}
         else:
             self.visualizer_kwargs = visualizer_kwargs
 
     def _dump_init_info(self, *args, **kwargs):
         pass
```

### Comparing `mmlab_lightning-1.0.0/mmlab_lightning.egg-info/PKG-INFO` & `mmlab_lightning-1.0.1/mmlab_lightning.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
@@ -24,7 +24,25 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
 A wrapper based on [lightning-template](https://github.com/shenmishajing/lightning_template) for mmlab repos to use in [project-template](https://github.com/shenmishajing/project_template)
+
+## Feature
+
+All features from [lightning-template](https://github.com/shenmishajing/lightning_template)
+
+## Installation
+
+See [installation docs](docs/installation/installation.md) for details.
+
+## Usage
+
+### CLI
+
+See [tool docs](docs/tools/cli.md) for details.
+
+### Models and Datasets
+
+See [model doc](docs/core/model.md) and [dataset doc](docs/core/dataset.md) for details.
```

### Comparing `mmlab_lightning-1.0.0/setup.py` & `mmlab_lightning-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mmlab_lightning",
-    version="1.0.0",
+    version="1.0.1",
     description="A wrapper for mmlab repos to use in project_template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/mmlab_lightning",
     project_urls={
@@ -20,14 +20,19 @@
     },
     python_requires=">=3.8",
     install_requires=[
         "lightning_template",
     ],
     license="MIT License",
     packages=find_packages(),  # 包
+    entry_points={
+        "console_scripts": [
+            "get_mmconfig = mmlab_lightning.tools.config.get_mmconfig:main",
+        ]
+    },
     platforms=["all"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Environment :: GPU :: NVIDIA CUDA",
```

