# Comparing `tmp/robotathome-1.1.8.tar.gz` & `tmp/robotathome-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotathome-1.1.8.tar", last modified: Thu Apr 20 19:00:15 2023, max compression
+gzip compressed data, was "robotathome-1.1.9.tar", last modified: Mon May  1 20:47:52 2023, max compression
```

## Comparing `robotathome-1.1.8.tar` & `robotathome-1.1.9.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.8/LICENSE
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    12789 2023-04-20 19:00:15.632561 robotathome-1.1.8/PKG-INFO
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12065 2023-04-09 20:16:48.000000 robotathome-1.1.8/README.md
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/notebooks/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.8/notebooks/05-Google-colab-drive.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.8/notebooks/10-Download-and-install.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   774991 2023-04-20 18:51:09.000000 robotathome-1.1.8/notebooks/100-Iterating-over-RGBD-images.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12108 2023-04-20 18:51:21.000000 robotathome-1.1.8/notebooks/110-Concatenating-images-from-multiple-cameras.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    37646 2023-04-20 18:51:35.000000 robotathome-1.1.8/notebooks/120-Making-a-video.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    26534 2023-04-20 18:51:46.000000 robotathome-1.1.8/notebooks/130-Processing-images-with-YOLO.ipynb
--rw-rw-r--   0 lightman  (1000) lightman  (1000)   208379 2023-04-20 18:53:12.000000 robotathome-1.1.8/notebooks/140-Loading-dataset-in-Google-Colab.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.8/notebooks/20-Before-starting-the-logging-system.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.8/notebooks/30-Getting-started-Framework-data.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.8/notebooks/40-Captured-data.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.8/notebooks/50-RGBD-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.8/notebooks/60-Lsrscan-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.8/notebooks/70-Scenes.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.8/notebooks/80-Characterized-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13896 2023-04-20 18:50:48.000000 robotathome-1.1.8/notebooks/90-The-config-file.ipynb
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/rh_schema_diagram/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.8/rh_schema_diagram/rh_schema_brief.pdf
--rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.8/rh_schema_diagram/rh_schema_full.pdf
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/robotathome/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      473 2023-04-20 18:59:44.000000 robotathome-1.1.8/robotathome/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.8/robotathome/_version.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/robotathome/core/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.8/robotathome/core/__init__.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.8/robotathome/core/df.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    46165 2023-04-16 16:14:10.000000 robotathome-1.1.8/robotathome/core/reader.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/robotathome/cv/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.8/robotathome/cv/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.8/robotathome/cv/_greetings.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.8/robotathome/cv/gluoncv.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.8/robotathome/cv/opencv.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.8/robotathome/helpers.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.8/robotathome/log.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/robotathome.egg-info/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12789 2023-04-20 19:00:15.000000 robotathome-1.1.8/robotathome.egg-info/PKG-INFO
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1383 2023-04-20 19:00:15.000000 robotathome-1.1.8/robotathome.egg-info/SOURCES.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-04-20 19:00:15.000000 robotathome-1.1.8/robotathome.egg-info/dependency_links.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-04-20 19:00:15.000000 robotathome-1.1.8/robotathome.egg-info/requires.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)       16 2023-04-20 19:00:15.000000 robotathome-1.1.8/robotathome.egg-info/top_level.txt
--rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-04-20 19:00:15.632561 robotathome-1.1.8/setup.cfg
--rw-r--r--   0 lightman  (1000) lightman  (1000)     3664 2023-04-20 18:55:12.000000 robotathome-1.1.8/setup.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/src/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      473 2023-04-20 18:59:44.000000 robotathome-1.1.8/src/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.8/src/_version.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/src/core/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.8/src/core/__init__.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.8/src/core/df.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    46165 2023-04-16 16:14:10.000000 robotathome-1.1.8/src/core/reader.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-20 19:00:15.632561 robotathome-1.1.8/src/cv/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.8/src/cv/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.8/src/cv/_greetings.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.8/src/cv/gluoncv.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.8/src/cv/opencv.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.8/src/helpers.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.8/src/log.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.9/LICENSE
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    12789 2023-05-01 20:47:52.071940 robotathome-1.1.9/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12065 2023-04-09 20:16:48.000000 robotathome-1.1.9/README.md
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.067940 robotathome-1.1.9/notebooks/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.9/notebooks/05-Google-colab-drive.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.9/notebooks/10-Download-and-install.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   774991 2023-04-20 18:51:09.000000 robotathome-1.1.9/notebooks/100-Iterating-over-RGBD-images.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12108 2023-04-20 18:51:21.000000 robotathome-1.1.9/notebooks/110-Concatenating-images-from-multiple-cameras.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    37646 2023-04-20 18:51:35.000000 robotathome-1.1.9/notebooks/120-Making-a-video.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    26534 2023-04-20 18:51:46.000000 robotathome-1.1.9/notebooks/130-Processing-images-with-YOLO.ipynb
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)   208379 2023-04-20 18:53:12.000000 robotathome-1.1.9/notebooks/140-Loading-dataset-in-Google-Colab.ipynb
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    24562 2023-05-01 20:46:25.000000 robotathome-1.1.9/notebooks/150-Segmentation-with-Detectron2.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.9/notebooks/20-Before-starting-the-logging-system.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.9/notebooks/30-Getting-started-Framework-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.9/notebooks/40-Captured-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.9/notebooks/50-RGBD-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.9/notebooks/60-Lsrscan-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.9/notebooks/70-Scenes.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.9/notebooks/80-Characterized-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13896 2023-04-20 18:50:48.000000 robotathome-1.1.9/notebooks/90-The-config-file.ipynb
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/rh_schema_diagram/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.9/rh_schema_diagram/rh_schema_brief.pdf
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.9/rh_schema_diagram/rh_schema_full.pdf
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/robotathome/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      473 2023-05-01 20:28:17.000000 robotathome-1.1.9/robotathome/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.9/robotathome/_version.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/robotathome/core/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.9/robotathome/core/__init__.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.9/robotathome/core/df.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    46165 2023-04-16 16:14:10.000000 robotathome-1.1.9/robotathome/core/reader.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/robotathome/cv/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.9/robotathome/cv/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.9/robotathome/cv/_greetings.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.9/robotathome/cv/gluoncv.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.9/robotathome/cv/opencv.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.9/robotathome/helpers.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.9/robotathome/log.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/robotathome.egg-info/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12789 2023-05-01 20:47:52.000000 robotathome-1.1.9/robotathome.egg-info/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1432 2023-05-01 20:47:52.000000 robotathome-1.1.9/robotathome.egg-info/SOURCES.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-05-01 20:47:52.000000 robotathome-1.1.9/robotathome.egg-info/dependency_links.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-05-01 20:47:52.000000 robotathome-1.1.9/robotathome.egg-info/requires.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)       16 2023-05-01 20:47:52.000000 robotathome-1.1.9/robotathome.egg-info/top_level.txt
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-05-01 20:47:52.071940 robotathome-1.1.9/setup.cfg
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     3726 2023-05-01 20:28:13.000000 robotathome-1.1.9/setup.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/src/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      473 2023-05-01 20:28:17.000000 robotathome-1.1.9/src/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.9/src/_version.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/src/core/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.9/src/core/__init__.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.9/src/core/df.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    46165 2023-04-16 16:14:10.000000 robotathome-1.1.9/src/core/reader.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-05-01 20:47:52.071940 robotathome-1.1.9/src/cv/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.9/src/cv/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.9/src/cv/_greetings.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.9/src/cv/gluoncv.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.9/src/cv/opencv.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.9/src/helpers.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.9/src/log.py
```

### Comparing `robotathome-1.1.8/LICENSE` & `robotathome-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/PKG-INFO` & `robotathome-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.8
+Version: 1.1.9
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
```

### Comparing `robotathome-1.1.8/README.md` & `robotathome-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/05-Google-colab-drive.ipynb` & `robotathome-1.1.9/notebooks/05-Google-colab-drive.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/10-Download-and-install.ipynb` & `robotathome-1.1.9/notebooks/10-Download-and-install.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/100-Iterating-over-RGBD-images.ipynb` & `robotathome-1.1.9/notebooks/100-Iterating-over-RGBD-images.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/110-Concatenating-images-from-multiple-cameras.ipynb` & `robotathome-1.1.9/notebooks/110-Concatenating-images-from-multiple-cameras.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/120-Making-a-video.ipynb` & `robotathome-1.1.9/notebooks/120-Making-a-video.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/130-Processing-images-with-YOLO.ipynb` & `robotathome-1.1.9/notebooks/130-Processing-images-with-YOLO.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/140-Loading-dataset-in-Google-Colab.ipynb` & `robotathome-1.1.9/notebooks/140-Loading-dataset-in-Google-Colab.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/20-Before-starting-the-logging-system.ipynb` & `robotathome-1.1.9/notebooks/20-Before-starting-the-logging-system.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/30-Getting-started-Framework-data.ipynb` & `robotathome-1.1.9/notebooks/30-Getting-started-Framework-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/40-Captured-data.ipynb` & `robotathome-1.1.9/notebooks/40-Captured-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/50-RGBD-observations.ipynb` & `robotathome-1.1.9/notebooks/50-RGBD-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/60-Lsrscan-observations.ipynb` & `robotathome-1.1.9/notebooks/60-Lsrscan-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/70-Scenes.ipynb` & `robotathome-1.1.9/notebooks/70-Scenes.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/80-Characterized-observations.ipynb` & `robotathome-1.1.9/notebooks/80-Characterized-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/notebooks/90-The-config-file.ipynb` & `robotathome-1.1.9/notebooks/90-The-config-file.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/rh_schema_diagram/rh_schema_brief.pdf` & `robotathome-1.1.9/rh_schema_diagram/rh_schema_brief.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/rh_schema_diagram/rh_schema_full.pdf` & `robotathome-1.1.9/rh_schema_diagram/rh_schema_full.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/_version.py` & `robotathome-1.1.9/robotathome/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/core/df.py` & `robotathome-1.1.9/robotathome/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/core/reader.py` & `robotathome-1.1.9/robotathome/core/reader.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/cv/gluoncv.py` & `robotathome-1.1.9/robotathome/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/cv/opencv.py` & `robotathome-1.1.9/robotathome/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/helpers.py` & `robotathome-1.1.9/robotathome/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome/log.py` & `robotathome-1.1.9/robotathome/log.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/robotathome.egg-info/PKG-INFO` & `robotathome-1.1.9/robotathome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.8
+Version: 1.1.9
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
```

### Comparing `robotathome-1.1.8/robotathome.egg-info/SOURCES.txt` & `robotathome-1.1.9/robotathome.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 notebooks/05-Google-colab-drive.ipynb
 notebooks/10-Download-and-install.ipynb
 notebooks/100-Iterating-over-RGBD-images.ipynb
 notebooks/110-Concatenating-images-from-multiple-cameras.ipynb
 notebooks/120-Making-a-video.ipynb
 notebooks/130-Processing-images-with-YOLO.ipynb
 notebooks/140-Loading-dataset-in-Google-Colab.ipynb
+notebooks/150-Segmentation-with-Detectron2.ipynb
 notebooks/20-Before-starting-the-logging-system.ipynb
 notebooks/30-Getting-started-Framework-data.ipynb
 notebooks/40-Captured-data.ipynb
 notebooks/50-RGBD-observations.ipynb
 notebooks/60-Lsrscan-observations.ipynb
 notebooks/70-Scenes.ipynb
 notebooks/80-Characterized-observations.ipynb
```

### Comparing `robotathome-1.1.8/setup.py` & `robotathome-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,16 @@
           'notebooks/70-Scenes.ipynb',
           'notebooks/80-Characterized-observations.ipynb',
           'notebooks/90-The-config-file.ipynb',
           'notebooks/100-Iterating-over-RGBD-images.ipynb',
           'notebooks/110-Concatenating-images-from-multiple-cameras.ipynb',
           'notebooks/120-Making-a-video.ipynb',
           'notebooks/130-Processing-images-with-YOLO.ipynb',
-          'notebooks/140-Loading-dataset-in-Google-Colab.ipynb']
+          'notebooks/140-Loading-dataset-in-Google-Colab.ipynb',
+          'notebooks/150-Segmentation-with-Detectron2.ipynb']
          )
     ],
     # sql files from robotathome package will be included in the installation package
     # located at ~/<anaconda-dir>/envs/<env-name>/lib/<python>/site-packages/robotathome
     package_data={'robotathome': ['*.sql']},
 
 )
```

### Comparing `robotathome-1.1.8/src/_version.py` & `robotathome-1.1.9/src/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/src/core/df.py` & `robotathome-1.1.9/src/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/src/core/reader.py` & `robotathome-1.1.9/src/core/reader.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/src/cv/gluoncv.py` & `robotathome-1.1.9/src/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/src/cv/opencv.py` & `robotathome-1.1.9/src/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/src/helpers.py` & `robotathome-1.1.9/src/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.8/src/log.py` & `robotathome-1.1.9/src/log.py`

 * *Files identical despite different names*

