# Comparing `tmp/classgraphic-0.2.2.tar.gz` & `tmp/classgraphic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/classgraphic-0.2.2.tar", last modified: Wed Sep 21 01:12:50 2022, max compression
+gzip compressed data, was "classgraphic-0.3.0.tar", last modified: Mon May  1 18:14:09 2023, max compression
```

## Comparing `classgraphic-0.2.2.tar` & `classgraphic-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.769681 classgraphic-0.2.2/
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.757681 classgraphic-0.2.2/.github/
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.761680 classgraphic-0.2.2/.github/workflows/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     1799 2022-09-19 17:37:37.000000 classgraphic-0.2.2/.github/workflows/dev.yml
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     1291 2022-09-19 12:00:42.000000 classgraphic-0.2.2/.gitignore
--rw-rw-r--   0 fdion     (1000) fdion     (1000)       72 2022-09-19 12:00:42.000000 classgraphic-0.2.2/AUTHORS.md
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      277 2022-09-19 12:00:42.000000 classgraphic-0.2.2/CITATION.cff
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      922 2022-09-21 01:12:39.000000 classgraphic-0.2.2/HISTORY.md
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     1074 2022-09-19 12:00:42.000000 classgraphic-0.2.2/LICENSE
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      259 2022-09-19 12:00:42.000000 classgraphic-0.2.2/MANIFEST.in
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     6607 2022-09-21 01:12:50.769681 classgraphic-0.2.2/PKG-INFO
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     4839 2022-09-21 01:12:39.000000 classgraphic-0.2.2/README.md
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.761680 classgraphic-0.2.2/binder/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      141 2022-09-19 12:00:42.000000 classgraphic-0.2.2/binder/README.md
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      195 2022-09-19 12:00:42.000000 classgraphic-0.2.2/binder/environment.yml
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.761680 classgraphic-0.2.2/classgraphic/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      207 2022-09-21 01:12:39.000000 classgraphic-0.2.2/classgraphic/__init__.py
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     5075 2022-09-19 12:00:42.000000 classgraphic-0.2.2/classgraphic/common.py
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      749 2022-09-19 12:00:42.000000 classgraphic-0.2.2/classgraphic/essential.py
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    15627 2022-09-19 12:00:42.000000 classgraphic-0.2.2/classgraphic/table.py
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     2586 2022-09-19 12:00:42.000000 classgraphic-0.2.2/classgraphic/template.py
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    26426 2022-09-21 01:12:39.000000 classgraphic-0.2.2/classgraphic/viz.py
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.765680 classgraphic-0.2.2/classgraphic.egg-info/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     6607 2022-09-21 01:12:49.000000 classgraphic-0.2.2/classgraphic.egg-info/PKG-INFO
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     1030 2022-09-21 01:12:50.000000 classgraphic-0.2.2/classgraphic.egg-info/SOURCES.txt
--rw-rw-r--   0 fdion     (1000) fdion     (1000)        1 2022-09-21 01:12:49.000000 classgraphic-0.2.2/classgraphic.egg-info/dependency_links.txt
--rw-rw-r--   0 fdion     (1000) fdion     (1000)        1 2022-09-19 12:02:20.000000 classgraphic-0.2.2/classgraphic.egg-info/not-zip-safe
--rw-rw-r--   0 fdion     (1000) fdion     (1000)       38 2022-09-21 01:12:50.000000 classgraphic-0.2.2/classgraphic.egg-info/requires.txt
--rw-rw-r--   0 fdion     (1000) fdion     (1000)       13 2022-09-21 01:12:50.000000 classgraphic-0.2.2/classgraphic.egg-info/top_level.txt
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.765680 classgraphic-0.2.2/docs/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      638 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/Makefile
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      764 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/make.bat
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.769681 classgraphic-0.2.2/docs/source/
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.769681 classgraphic-0.2.2/docs/source/_static/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)        0 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/_static/.empty
--rw-rw-r--   0 fdion     (1000) fdion     (1000)   179466 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/class_imbalance.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     2011 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/classgraphic.md
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    46804 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/classification_table.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     2161 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/conf.py
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    43207 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/confusion.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    55061 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/describe.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    31036 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/feature.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    23308 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/imbalance_table.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      289 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/index.md
--rw-rw-r--   0 fdion     (1000) fdion     (1000)    26561 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/missing.png
--rw-rw-r--   0 fdion     (1000) fdion     (1000)   184788 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/sorter_patent.jpg
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      121 2022-09-19 12:00:42.000000 classgraphic-0.2.2/docs/source/usage.md
--rw-rw-r--   0 fdion     (1000) fdion     (1000)      115 2022-09-19 12:00:42.000000 classgraphic-0.2.2/environment.yml
-drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2022-09-21 01:12:50.769681 classgraphic-0.2.2/notebooks/
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     9323 2022-09-19 17:37:37.000000 classgraphic-0.2.2/notebooks/ClassGraphic_binary_demo.ipynb
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     8050 2022-09-19 12:00:42.000000 classgraphic-0.2.2/notebooks/ClassGraphic_iris_demo.ipynb
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     3989 2022-09-19 17:37:37.000000 classgraphic-0.2.2/notebooks/template_adjustments.ipynb
--rw-rw-r--   0 fdion     (1000) fdion     (1000)       38 2022-09-19 12:00:42.000000 classgraphic-0.2.2/requirements.txt
--rw-rw-r--   0 fdion     (1000) fdion     (1000)       38 2022-09-21 01:12:50.769681 classgraphic-0.2.2/setup.cfg
--rw-rw-r--   0 fdion     (1000) fdion     (1000)     1552 2022-09-21 01:12:39.000000 classgraphic-0.2.2/setup.py
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.769676 classgraphic-0.3.0/
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.737676 classgraphic-0.3.0/.github/
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.741676 classgraphic-0.3.0/.github/workflows/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     1799 2022-09-19 17:37:37.000000 classgraphic-0.3.0/.github/workflows/dev.yml
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     1291 2022-09-19 12:00:42.000000 classgraphic-0.3.0/.gitignore
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)       72 2022-09-19 12:00:42.000000 classgraphic-0.3.0/AUTHORS.md
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      277 2022-09-19 12:00:42.000000 classgraphic-0.3.0/CITATION.cff
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     1050 2023-05-01 17:54:40.000000 classgraphic-0.3.0/HISTORY.md
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     1074 2022-09-19 12:00:42.000000 classgraphic-0.3.0/LICENSE
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      259 2022-09-19 12:00:42.000000 classgraphic-0.3.0/MANIFEST.in
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     6844 2023-05-01 18:14:09.769676 classgraphic-0.3.0/PKG-INFO
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     4905 2023-05-01 17:54:40.000000 classgraphic-0.3.0/README.md
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.741676 classgraphic-0.3.0/binder/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      141 2022-09-19 12:00:42.000000 classgraphic-0.3.0/binder/README.md
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      195 2022-09-19 12:00:42.000000 classgraphic-0.3.0/binder/environment.yml
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.741676 classgraphic-0.3.0/classgraphic/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      207 2023-05-01 17:52:24.000000 classgraphic-0.3.0/classgraphic/__init__.py
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     5075 2022-09-19 12:00:42.000000 classgraphic-0.3.0/classgraphic/common.py
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      749 2022-09-19 12:00:42.000000 classgraphic-0.3.0/classgraphic/essential.py
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    15627 2022-09-19 12:00:42.000000 classgraphic-0.3.0/classgraphic/table.py
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     2586 2022-09-19 12:00:42.000000 classgraphic-0.3.0/classgraphic/template.py
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    31114 2023-05-01 18:10:13.000000 classgraphic-0.3.0/classgraphic/viz.py
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.753676 classgraphic-0.3.0/classgraphic.egg-info/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     6844 2023-05-01 18:14:09.000000 classgraphic-0.3.0/classgraphic.egg-info/PKG-INFO
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     1030 2023-05-01 18:14:09.000000 classgraphic-0.3.0/classgraphic.egg-info/SOURCES.txt
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)        1 2023-05-01 18:14:09.000000 classgraphic-0.3.0/classgraphic.egg-info/dependency_links.txt
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)        1 2022-09-19 12:02:20.000000 classgraphic-0.3.0/classgraphic.egg-info/not-zip-safe
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)       38 2023-05-01 18:14:09.000000 classgraphic-0.3.0/classgraphic.egg-info/requires.txt
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)       13 2023-05-01 18:14:09.000000 classgraphic-0.3.0/classgraphic.egg-info/top_level.txt
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.753676 classgraphic-0.3.0/docs/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      638 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/Makefile
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      764 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/make.bat
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.761676 classgraphic-0.3.0/docs/source/
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.761676 classgraphic-0.3.0/docs/source/_static/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)        0 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/_static/.empty
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)   179466 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/class_imbalance.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     2011 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/classgraphic.md
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    46804 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/classification_table.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     2161 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/conf.py
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    43207 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/confusion.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    55061 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/describe.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    31036 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/feature.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    23308 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/imbalance_table.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      289 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/index.md
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)    26561 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/missing.png
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)   184788 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/sorter_patent.jpg
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      121 2022-09-19 12:00:42.000000 classgraphic-0.3.0/docs/source/usage.md
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)      115 2022-09-19 12:00:42.000000 classgraphic-0.3.0/environment.yml
+drwxrwxr-x   0 fdion     (1000) fdion     (1000)        0 2023-05-01 18:14:09.769676 classgraphic-0.3.0/notebooks/
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     9323 2022-09-19 17:37:37.000000 classgraphic-0.3.0/notebooks/ClassGraphic_binary_demo.ipynb
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     8050 2022-09-19 12:00:42.000000 classgraphic-0.3.0/notebooks/ClassGraphic_iris_demo.ipynb
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     3989 2022-09-19 17:37:37.000000 classgraphic-0.3.0/notebooks/template_adjustments.ipynb
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)       38 2022-09-19 12:00:42.000000 classgraphic-0.3.0/requirements.txt
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)       38 2023-05-01 18:14:09.769676 classgraphic-0.3.0/setup.cfg
+-rw-rw-r--   0 fdion     (1000) fdion     (1000)     1616 2023-05-01 17:56:06.000000 classgraphic-0.3.0/setup.py
```

### Comparing `classgraphic-0.2.2/.github/workflows/dev.yml` & `classgraphic-0.3.0/.github/workflows/dev.yml`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/.gitignore` & `classgraphic-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/HISTORY.md` & `classgraphic-0.3.0/HISTORY.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.3.0 (2023-05-01)
+
+* added 2D clustering visualization
+* defaults to Voronoi tessalation
+* optional Delauney triangulation
+
 ## 0.2.1 (2022-09-20)
 
 * fixed image not showing on pypi
 * fixed feature importance error
 * warning = False didn't prevent warning to show
 
 ## 0.2.1 (2022-09-19)
```

### Comparing `classgraphic-0.2.2/LICENSE` & `classgraphic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/PKG-INFO` & `classgraphic-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: classgraphic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Interactive classification diagnostic plots
 Home-page: https://github.com/dionresearch/classgraphic
 Author: Francois Dion
 Author-email: fdion@dionresearch.com
 License: MIT license
-Keywords: classgraphic,classification,visualization,ml,machine learning,plotly,interactive
-Platform: UNKNOWN
+Keywords: classgraphic,classification,clustering,visualization,ml,machine learning,plotly,interactive
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # classgraphic
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
@@ -53,14 +53,18 @@
 - feature_importance
 - missing
 - precision_recall
 - roc
 - prediction_histogram
 - threshold
 
+For clustering:
+- Delauney triangulations
+- Voronoi tessalations
+
 # Try it
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dionresearch/classgraphic/HEAD?labpath=notebooks%2FClassGraphic_iris_demo.ipynb)
 
 By trying it on binder, you'll see all the details and interactivity. The quickstart below
 has static images, but if you run these commands in a jupyter notebook, ipython or IDE you will
 be able to interact with them.
@@ -178,14 +182,20 @@
 
 - [stemgraphic](https://github.com/dionresearch/stemgraphic) python package for visualization of data and text
 - [Hotelling](https://github.com/dionresearch/hotelling) one and two sample Hotelling T2 tests, T2 and f statistics and univariate and multivariate control charts and anomaly detection
 
 
 # History
 
+## 0.3.0 (2023-05-01)
+
+* added 2D clustering visualization
+* defaults to Voronoi tessalation
+* optional Delauney triangulation
+
 ## 0.2.1 (2022-09-20)
 
 * fixed image not showing on pypi
 * fixed feature importance error
 * warning = False didn't prevent warning to show
 
 ## 0.2.1 (2022-09-19)
@@ -210,8 +220,7 @@
 
 Inspired by Dion Research LLC Internal EDA/anomaly and end to end data science platform.
 A dozen charts and tables were initially designed to provide better diagnostic reporting.
 Some can also be used for exploratory or explanatory purposes.
 
 See:
 https://blog.dionresearch.com/2019/10/visualizations-explanatory-exploratory.html
-
```

### Comparing `classgraphic-0.2.2/README.md` & `classgraphic-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 - feature_importance
 - missing
 - precision_recall
 - roc
 - prediction_histogram
 - threshold
 
+For clustering:
+- Delauney triangulations
+- Voronoi tessalations
+
 # Try it
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dionresearch/classgraphic/HEAD?labpath=notebooks%2FClassGraphic_iris_demo.ipynb)
 
 By trying it on binder, you'll see all the details and interactivity. The quickstart below
 has static images, but if you run these commands in a jupyter notebook, ipython or IDE you will
 be able to interact with them.
```

### Comparing `classgraphic-0.2.2/classgraphic/common.py` & `classgraphic-0.3.0/classgraphic/common.py`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/classgraphic/essential.py` & `classgraphic-0.3.0/classgraphic/essential.py`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/classgraphic/table.py` & `classgraphic-0.3.0/classgraphic/table.py`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/classgraphic/template.py` & `classgraphic-0.3.0/classgraphic/template.py`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/classgraphic/viz.py` & `classgraphic-0.3.0/classgraphic/viz.py`

 * *Files 13% similar despite different names*

```diff
@@ -692,26 +692,121 @@
         legend_title=legend_title
     )
     if extended:
         return fig, df
     return fig
 
 
+def voronoi_diagram(centroid_source, data=None, labels=None, plot_voronoi=True, plot_delauney=False, **kwargs):
+    """Plot a 2D voronoi diagram.
+
+    Args:
+        centroid_source: either a fitted clustering alrorithm with cluster_centers, or cluster center coordinates
+        data: optional, original data (X) used for calculating the clusters
+        labels: labels (y) for the clusters
+        plot_voronoi: if False, will not plot boundaries, aka Voronoi tessalation
+        plot_delauney: if True, plots Delauney triangulation
+        **kwargs: for now, passed to initial scatter plot
+
+    Returns:
+        Plotly figure
+    """
+    try:
+        centers = centroid_source.cluster_centers
+    except AttributeError:
+        centers = centroid_source
+    voronoi = sp.spatial.Voronoi(centers)
+    if plot_delauney:
+        triangles = sp.spatial.Delaunay(centers)
+
+    voronoi_points = pd.DataFrame(voronoi.points)
+    voronoi_points["type"] = "centroids"
+    voronoi_vertices = pd.DataFrame(voronoi.vertices)
+    voronoi_vertices["type"] = "vertices"
+    if data is not None:
+        data_points = pd.DataFrame(X)
+        data_points["type"] = "data"
+        voronoi_df = pd.concat([data_points, voronoi_vertices, voronoi_points], axis=0)
+    else:
+        voronoi_df = pd.concat([voronoi_vertices, voronoi_points], axis=0)
+
+    center = voronoi.points.mean(axis=0)
+    ptp_bound = voronoi.points.ptp(axis=0)
+
+    # Voronoi
+    finite_segments = []
+    infinite_segments = []
+    for pointidx, simplex in zip(voronoi.ridge_points, voronoi.ridge_vertices):
+        simplex = np.asarray(simplex)
+        if np.all(simplex >= 0):
+            finite_segments.append(voronoi.vertices[simplex])
+        else:
+            i = simplex[simplex >= 0][0]  # finite end Voronoi vertex
+
+            t = voronoi.points[pointidx[1]] - voronoi.points[pointidx[0]]  # tangent
+            t /= np.linalg.norm(t)
+            n = np.array([-t[1], t[0]])  # normal
+
+            midpoint = voronoi.points[pointidx].mean(axis=0)
+            direction = np.sign(np.dot(midpoint - center, n)) * n
+            if (voronoi.furthest_site):
+                direction = -direction
+            far_point = voronoi.vertices[i] + direction * ptp_bound.max()
+            infinite_segments.append([voronoi.vertices[i], far_point])
+
+    if data is not None and labels is not None:
+        fig = px.scatter(data_points, x=0, y=1, color="type", hover_name=labels, **kwargs)
+        fig.add_trace(go.Scatter(x=voronoi_vertices[0], y=voronoi_vertices[1], mode="markers", name="vertices"))
+        fig.add_trace(go.Scatter(x=voronoi_points[0], y=voronoi_points[1], mode="markers", marker_symbol="x",
+                                 name="centroids"))
+    else:
+        fig = px.scatter(voronoi_df, x=0, y=1, color="type")
+
+    for plot in fig.data:
+        if plot["name"] == "vertices":
+            vertices_color = plot.marker.color
+        elif plot["name"] == "centroids":
+            centroids_color = plot.marker.color
+
+    if plot_delauney:
+        first = True
+        for triangleidx in triangles.simplices:
+            x, y = zip(triangles.points[triangleidx].T)
+            fig.add_trace(
+                go.Scatter(x=x[0], y=y[0], mode="lines+markers", line_color="red", marker_color=centroids_color,
+                           name="delauney", legendgroup="delauney", showlegend=first))
+            first = False
+
+    if plot_voronoi:
+        first = True
+        for line in finite_segments:
+            x, y = zip(*line)
+            fig.add_trace(go.Scatter(x=x, y=y, mode="lines+markers", line_color="black", marker_color=vertices_color,
+                                     name="boundary", legendgroup="boundary", showlegend=first))
+            first = False
+        for line in infinite_segments:
+            x, y = zip(*line)
+            fig.add_trace(go.Scatter(x=x, y=y, mode="lines+markers", line_color="black", marker_color=vertices_color,
+                                     name="boundary", legendgroup="boundary", showlegend=first))
+    return fig
+
+
 if __name__ == "__main__":
+    from sklearn.cluster import KMeans
     from sklearn.linear_model import LogisticRegression
-    from sklearn.datasets import make_classification
+    from sklearn.datasets import make_classification, make_blobs
     from sklearn.model_selection import train_test_split
     from sklearn.svm import SVC
 
     set_default_template("dion")
 
     random_state = 0
     np.random.seed(random_state)
 
-    binary = True
+    binary = False
     if binary:
         # Data
         X, y = make_classification(n_samples=500, random_state=random_state)
 
         # Class split, pie chart
         fig = class_imbalance(y, reference=True)
         fig.show()
@@ -778,72 +873,83 @@
         index = np.random.choice(X.size, 50, replace=False)
         X.ravel()[index] = np.nan
 
         # Missing values
         fig = missing(X)
         fig.show()
 
-    df = px.data.iris()
-    X = df.drop(columns=["species", "species_id"])
-    y = df["species"]
-    X_train, X_test, y_train, y_test = train_test_split(
-        X, y, test_size=0.6, random_state=random_state
-    )
+    multivar = False
+    if multivar:
+        df = px.data.iris()
+        X = df.drop(columns=["species", "species_id"])
+        y = df["species"]
+        X_train, X_test, y_train, y_test = train_test_split(
+            X, y, test_size=0.6, random_state=random_state
+        )
 
-    # Class split
-    fig = class_imbalance(y_train, y_test, condition="train,test", sort=True)
-    fig.show()
+        # Class split
+        fig = class_imbalance(y_train, y_test, condition="train,test", sort=True)
+        fig.show()
 
-    fig = class_imbalance(y_train, condition="train", sort=True)
-    fig.show()
+        fig = class_imbalance(y_train, condition="train", sort=True)
+        fig.show()
 
-    # Fit the model
-    lr_model = LogisticRegression(max_iter=200)
-    lr_model.fit(X_train, y_train)
-    y_probs = lr_model.predict_proba(X_test)
-    y_pred = lr_model.predict(X_test)
+        # Fit the model
+        lr_model = LogisticRegression(max_iter=200)
+        lr_model.fit(X_train, y_train)
+        y_probs = lr_model.predict_proba(X_test)
+        y_pred = lr_model.predict(X_test)
 
-    # class error
-    fig = class_error(lr_model, y_test, y_pred)
-    fig.show()
+        # class error
+        fig = class_error(lr_model, y_test, y_pred)
+        fig.show()
 
-    # confusion matrix
-    tab = confusion_matrix_table(lr_model, y_test, y_pred)
-    tab.show()
+        # confusion matrix
+        tab = confusion_matrix_table(lr_model, y_test, y_pred)
+        tab.show()
 
-    # feature importance
-    fig = feature_importance(lr_model, y)
-    fig.show()
+        # feature importance
+        fig = feature_importance(lr_model, y)
+        fig.show()
 
-    fig = feature_importance(lr_model, y, transpose=True)
-    fig.show()
+        fig = feature_importance(lr_model, y, transpose=True)
+        fig.show()
 
-    # view
-    fig = view(X_test, y_test, y_pred)
-    fig.show()
+        # view
+        fig = view(X_test, y_test, y_pred)
+        fig.show()
 
-    # prediction histogram
-    fig, ph_df = prediction_histogram(
-        lr_model, y_test, y_probs, extended=True, template="seaborn"
-    )
-    fig.show()
-    ph_df.to_csv("results.csv")
+        # prediction histogram
+        fig, ph_df = prediction_histogram(
+            lr_model, y_test, y_probs, extended=True, template="seaborn"
+        )
+        fig.show()
+        ph_df.to_csv("results.csv")
 
-    print(y_probs.shape)
-    # precision recall curve
-    fig = precision_recall(lr_model, y_test, y_probs)
-    fig.show()
+        print(y_probs.shape)
+        # precision recall curve
+        fig = precision_recall(lr_model, y_test, y_probs)
+        fig.show()
 
-    # multiclass roc
-    fig = roc(lr_model, y_test, y_probs)
-    fig.show()
+        # multiclass roc
+        fig = roc(lr_model, y_test, y_probs)
+        fig.show()
 
-    # threshold
-    fig = threshold(lr_model, y_test, y_probs)
-    fig.show()
+        # threshold
+        fig = threshold(lr_model, y_test, y_probs)
+        fig.show()
+
+        # add missing values
+        X = X.mask(np.random.random(X.shape) < 0.05)
 
-    # add missing values
-    X = X.mask(np.random.random(X.shape) < 0.05)
+        # Missing values
+        fig = missing(X, template="plotly_white")
+        fig.show()
+
+    # Clustering
+    X, y, centers = make_blobs(n_samples=300, n_features=2, centers=9, return_centers=True)
+    fig = voronoi_diagram(centers, X, y)
+    fig.show()
 
-    # Missing values
-    fig = missing(X, template="plotly_white")
+    _, _, centers = make_blobs(n_samples=144, n_features=2, centers=12, return_centers=True)
+    fig = voronoi_diagram(centers, plot_voronoi=False, plot_delauney=True)
     fig.show()
```

### Comparing `classgraphic-0.2.2/classgraphic.egg-info/PKG-INFO` & `classgraphic-0.3.0/classgraphic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: classgraphic
-Version: 0.2.2
+Version: 0.3.0
 Summary: Interactive classification diagnostic plots
 Home-page: https://github.com/dionresearch/classgraphic
 Author: Francois Dion
 Author-email: fdion@dionresearch.com
 License: MIT license
-Keywords: classgraphic,classification,visualization,ml,machine learning,plotly,interactive
-Platform: UNKNOWN
+Keywords: classgraphic,classification,clustering,visualization,ml,machine learning,plotly,interactive
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # classgraphic
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
@@ -53,14 +53,18 @@
 - feature_importance
 - missing
 - precision_recall
 - roc
 - prediction_histogram
 - threshold
 
+For clustering:
+- Delauney triangulations
+- Voronoi tessalations
+
 # Try it
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dionresearch/classgraphic/HEAD?labpath=notebooks%2FClassGraphic_iris_demo.ipynb)
 
 By trying it on binder, you'll see all the details and interactivity. The quickstart below
 has static images, but if you run these commands in a jupyter notebook, ipython or IDE you will
 be able to interact with them.
@@ -178,14 +182,20 @@
 
 - [stemgraphic](https://github.com/dionresearch/stemgraphic) python package for visualization of data and text
 - [Hotelling](https://github.com/dionresearch/hotelling) one and two sample Hotelling T2 tests, T2 and f statistics and univariate and multivariate control charts and anomaly detection
 
 
 # History
 
+## 0.3.0 (2023-05-01)
+
+* added 2D clustering visualization
+* defaults to Voronoi tessalation
+* optional Delauney triangulation
+
 ## 0.2.1 (2022-09-20)
 
 * fixed image not showing on pypi
 * fixed feature importance error
 * warning = False didn't prevent warning to show
 
 ## 0.2.1 (2022-09-19)
@@ -210,8 +220,7 @@
 
 Inspired by Dion Research LLC Internal EDA/anomaly and end to end data science platform.
 A dozen charts and tables were initially designed to provide better diagnostic reporting.
 Some can also be used for exploratory or explanatory purposes.
 
 See:
 https://blog.dionresearch.com/2019/10/visualizations-explanatory-exploratory.html
-
```

### Comparing `classgraphic-0.2.2/classgraphic.egg-info/SOURCES.txt` & `classgraphic-0.3.0/classgraphic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/Makefile` & `classgraphic-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/make.bat` & `classgraphic-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/class_imbalance.png` & `classgraphic-0.3.0/docs/source/class_imbalance.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/classgraphic.md` & `classgraphic-0.3.0/docs/source/classgraphic.md`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/classification_table.png` & `classgraphic-0.3.0/docs/source/classification_table.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/conf.py` & `classgraphic-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/confusion.png` & `classgraphic-0.3.0/docs/source/confusion.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/describe.png` & `classgraphic-0.3.0/docs/source/describe.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/feature.png` & `classgraphic-0.3.0/docs/source/feature.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/imbalance_table.png` & `classgraphic-0.3.0/docs/source/imbalance_table.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/missing.png` & `classgraphic-0.3.0/docs/source/missing.png`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/docs/source/sorter_patent.jpg` & `classgraphic-0.3.0/docs/source/sorter_patent.jpg`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/notebooks/ClassGraphic_binary_demo.ipynb` & `classgraphic-0.3.0/notebooks/ClassGraphic_binary_demo.ipynb`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/notebooks/ClassGraphic_iris_demo.ipynb` & `classgraphic-0.3.0/notebooks/ClassGraphic_iris_demo.ipynb`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/notebooks/template_adjustments.ipynb` & `classgraphic-0.3.0/notebooks/template_adjustments.ipynb`

 * *Files identical despite different names*

### Comparing `classgraphic-0.2.2/setup.py` & `classgraphic-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,25 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="Interactive classification diagnostic plots",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
-    keywords=["classgraphic", "classification", "visualization", "ml", "machine learning", "plotly", "interactive"],
+    keywords=["classgraphic", "classification", "clustering", "visualization", "ml", "machine learning", "plotly", "interactive"],
     name="classgraphic",
     packages=find_packages(include=["classgraphic", "classgraphic.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/dionresearch/classgraphic",
-    version="0.2.2",
+    version="0.3.0",
     zip_safe=False,
 )
```

