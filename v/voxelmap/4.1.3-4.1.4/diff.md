# Comparing `tmp/voxelmap-4.1.3.tar.gz` & `tmp/voxelmap-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-4.1.3.tar", max compression
+gzip compressed data, was "voxelmap-4.1.4.tar", max compression
```

## Comparing `voxelmap-4.1.3.tar` & `voxelmap-4.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.1.3/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.1.3/README.md
--rw-r--r--   0        0        0      526 2023-05-01 01:49:27.131152 voxelmap-4.1.3/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.1.3/voxelmap/__init__.py
--rw-r--r--   0        0        0    21518 2023-05-01 01:42:22.585166 voxelmap-4.1.3/voxelmap/annex.py
--rwxr-xr-x   0        0        0    28849 2023-05-01 01:44:24.008146 voxelmap-4.1.3/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 voxelmap-4.1.3/setup.py
--rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 voxelmap-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.1.4/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.1.4/README.md
+-rw-r--r--   0        0        0      526 2023-05-01 02:10:37.537702 voxelmap-4.1.4/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.1.4/voxelmap/__init__.py
+-rw-r--r--   0        0        0    21518 2023-05-01 01:42:22.585166 voxelmap-4.1.4/voxelmap/annex.py
+-rwxr-xr-x   0        0        0    28849 2023-05-01 01:44:24.008146 voxelmap-4.1.4/voxelmap/jotunn.py
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 voxelmap-4.1.4/setup.py
+-rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 voxelmap-4.1.4/PKG-INFO
```

### Comparing `voxelmap-4.1.3/LICENSE` & `voxelmap-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.3/README.md` & `voxelmap-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.3/pyproject.toml` & `voxelmap-4.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "4.1.3"
+version = "4.1.4"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `voxelmap-4.1.3/voxelmap/annex.py` & `voxelmap-4.1.4/voxelmap/annex.py`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.3/voxelmap/jotunn.py` & `voxelmap-4.1.4/voxelmap/jotunn.py`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.3/setup.py` & `voxelmap-4.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'pandas>=1.5.2,<2.0.0',
  'pyvista>=0.38.2,<0.39.0',
  'scikit-image>=0.19.3,<0.20.0',
  'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '4.1.3',
+    'version': '4.1.4',
     'description': 'A Python library for making voxel and 3D models from NumPy arrays.',
     'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making voxel and three-dimensional models from NumPy arrays. \n\n<a href="https://voxelmap.readthedocs.io/en/latest/">\n<img src="https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true" width="250"></a>\n\n## Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n\n## Just starting? Remote Usage with a Colab notebook (click below)\n\n<a href="https://colab.research.google.com/drive/1RMEMgZHlk_tKAzfS4QfXLJV9joDgdh8N?usp=sharing">\n<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/colaboratory.png" width="500" ></a>\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is free software. It comes without any warranty, to the extent permitted by applicable law. You can redistribute it and/or modify it under the terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.\n\n**[MIT license](./LICENSE)** Copyright 2022 © <a href="https://github.com/andrewrgarcia" target="_blank">Andrew Garcia</a>.\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
 python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pyvista>=0.38.2,<0.39.0',
 'scikit-image>=0.19.3,<0.20.0', 'scipy>=1.10.0,<2.0.0'] setup_kwargs =
-{ 'name': 'voxelmap', 'version': '4.1.3', 'description': 'A Python library for
+{ 'name': 'voxelmap', 'version': '4.1.4', 'description': 'A Python library for
 making voxel and 3D models from NumPy arrays.', 'long_description': '#
 voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-
 square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/
 LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/
 badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/
 ?badge=latest)\n\nA Python library for making voxel and three-dimensional
 models from NumPy arrays. \n\n\n[https://github.com/andrewrgarcia/voxelmap/
```

### Comparing `voxelmap-4.1.3/PKG-INFO` & `voxelmap-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 4.1.3
+Version: 4.1.4
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 4.1.3 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 4.1.4 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
```

