# Comparing `tmp/hexo_inpainting-1.0.3.tar.gz` & `tmp/hexo_inpainting-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexo_inpainting-1.0.3.tar", last modified: Mon May  1 10:37:22 2023, max compression
+gzip compressed data, was "hexo_inpainting-1.0.4.tar", last modified: Mon May  1 10:57:00 2023, max compression
```

## Comparing `hexo_inpainting-1.0.3.tar` & `hexo_inpainting-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:37:22.222702 hexo_inpainting-1.0.3/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      290 2023-05-01 10:37:22.222702 hexo_inpainting-1.0.3/PKG-INFO
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:37:22.218703 hexo_inpainting-1.0.3/hexo_inpainting/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       80 2023-05-01 09:34:27.000000 hexo_inpainting-1.0.3/hexo_inpainting/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4755 2023-04-25 07:57:38.000000 hexo_inpainting-1.0.3/hexo_inpainting/const.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8284 2023-05-01 09:45:52.000000 hexo_inpainting-1.0.3/hexo_inpainting/helper.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3696 2023-05-01 09:45:21.000000 hexo_inpainting-1.0.3/hexo_inpainting/inpainting.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:37:22.218703 hexo_inpainting-1.0.3/hexo_inpainting/model/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9464 2023-05-01 09:47:10.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7279 2023-05-01 10:36:30.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/controlnet.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6868 2023-04-25 08:01:21.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/ddim_sampler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    57098 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/fcf.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3175 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/instruct_pix2pix.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1480 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/lama.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11197 2023-04-25 07:51:21.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/ldm.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2884 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/manga.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    62625 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/mat.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      716 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/opencv2.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2934 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/paint_by_example.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:37:22.222702 hexo_inpainting-1.0.3/hexo_inpainting/model/pipeline/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      108 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/pipeline/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    28149 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11838 2023-04-25 08:02:19.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/plms_sampler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6603 2023-04-25 07:53:47.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/sd.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    33799 2023-05-01 09:46:42.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/utils.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    15637 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/model/zits.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2423 2023-05-01 09:45:23.000000 hexo_inpainting-1.0.3/hexo_inpainting/model_manager.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5145 2023-05-01 08:35:33.000000 hexo_inpainting-1.0.3/hexo_inpainting/outpainting.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3306 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.3/hexo_inpainting/schema.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:37:22.218703 hexo_inpainting-1.0.3/hexo_inpainting.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      290 2023-05-01 10:37:22.000000 hexo_inpainting-1.0.3/hexo_inpainting.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1053 2023-05-01 10:37:22.000000 hexo_inpainting-1.0.3/hexo_inpainting.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 10:37:22.000000 hexo_inpainting-1.0.3/hexo_inpainting.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      194 2023-05-01 10:37:22.000000 hexo_inpainting-1.0.3/hexo_inpainting.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-01 10:37:22.000000 hexo_inpainting-1.0.3/hexo_inpainting.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 10:37:22.222702 hexo_inpainting-1.0.3/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      475 2023-05-01 10:37:13.000000 hexo_inpainting-1.0.3/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:57:00.357476 hexo_inpainting-1.0.4/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      290 2023-05-01 10:57:00.357476 hexo_inpainting-1.0.4/PKG-INFO
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:57:00.353477 hexo_inpainting-1.0.4/hexo_inpainting/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       80 2023-05-01 09:34:27.000000 hexo_inpainting-1.0.4/hexo_inpainting/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4755 2023-04-25 07:57:38.000000 hexo_inpainting-1.0.4/hexo_inpainting/const.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8284 2023-05-01 09:45:52.000000 hexo_inpainting-1.0.4/hexo_inpainting/helper.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3696 2023-05-01 09:45:21.000000 hexo_inpainting-1.0.4/hexo_inpainting/inpainting.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:57:00.357476 hexo_inpainting-1.0.4/hexo_inpainting/model/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9464 2023-05-01 09:47:10.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4755 2023-05-01 10:55:44.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/const.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7279 2023-05-01 10:36:30.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/controlnet.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6868 2023-04-25 08:01:21.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/ddim_sampler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    57098 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/fcf.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8284 2023-05-01 10:55:44.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/helper.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3175 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/instruct_pix2pix.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1480 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/lama.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11197 2023-04-25 07:51:21.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/ldm.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2884 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/manga.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    62625 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/mat.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      716 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/opencv2.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2934 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/paint_by_example.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:57:00.357476 hexo_inpainting-1.0.4/hexo_inpainting/model/pipeline/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      108 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/pipeline/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    28149 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11838 2023-04-25 08:02:19.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/plms_sampler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3306 2023-05-01 10:56:19.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/schema.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6603 2023-04-25 07:53:47.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/sd.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    33799 2023-05-01 09:46:42.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/utils.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    15637 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/model/zits.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2423 2023-05-01 09:45:23.000000 hexo_inpainting-1.0.4/hexo_inpainting/model_manager.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5145 2023-05-01 08:35:33.000000 hexo_inpainting-1.0.4/hexo_inpainting/outpainting.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3306 2023-04-25 07:45:35.000000 hexo_inpainting-1.0.4/hexo_inpainting/schema.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 10:57:00.353477 hexo_inpainting-1.0.4/hexo_inpainting.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      290 2023-05-01 10:57:00.000000 hexo_inpainting-1.0.4/hexo_inpainting.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1148 2023-05-01 10:57:00.000000 hexo_inpainting-1.0.4/hexo_inpainting.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 10:57:00.000000 hexo_inpainting-1.0.4/hexo_inpainting.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      194 2023-05-01 10:57:00.000000 hexo_inpainting-1.0.4/hexo_inpainting.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-01 10:57:00.000000 hexo_inpainting-1.0.4/hexo_inpainting.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 10:57:00.357476 hexo_inpainting-1.0.4/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      475 2023-05-01 10:56:54.000000 hexo_inpainting-1.0.4/setup.py
```

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/const.py` & `hexo_inpainting-1.0.4/hexo_inpainting/const.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/helper.py` & `hexo_inpainting-1.0.4/hexo_inpainting/helper.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/inpainting.py` & `hexo_inpainting-1.0.4/hexo_inpainting/inpainting.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/base.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/base.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/controlnet.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/ddim_sampler.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/ddim_sampler.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/fcf.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/fcf.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/instruct_pix2pix.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/lama.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/lama.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/ldm.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/ldm.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/manga.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/manga.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/mat.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/mat.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/opencv2.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/opencv2.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/paint_by_example.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/paint_by_example.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/plms_sampler.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/plms_sampler.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/sd.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/sd.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/utils.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/utils.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model/zits.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/zits.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/model_manager.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model_manager.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/outpainting.py` & `hexo_inpainting-1.0.4/hexo_inpainting/outpainting.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting/schema.py` & `hexo_inpainting-1.0.4/hexo_inpainting/model/schema.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-1.0.3/hexo_inpainting.egg-info/SOURCES.txt` & `hexo_inpainting-1.0.4/hexo_inpainting.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 hexo_inpainting.egg-info/PKG-INFO
 hexo_inpainting.egg-info/SOURCES.txt
 hexo_inpainting.egg-info/dependency_links.txt
 hexo_inpainting.egg-info/requires.txt
 hexo_inpainting.egg-info/top_level.txt
 hexo_inpainting/model/__init__.py
 hexo_inpainting/model/base.py
+hexo_inpainting/model/const.py
 hexo_inpainting/model/controlnet.py
 hexo_inpainting/model/ddim_sampler.py
 hexo_inpainting/model/fcf.py
+hexo_inpainting/model/helper.py
 hexo_inpainting/model/instruct_pix2pix.py
 hexo_inpainting/model/lama.py
 hexo_inpainting/model/ldm.py
 hexo_inpainting/model/manga.py
 hexo_inpainting/model/mat.py
 hexo_inpainting/model/opencv2.py
 hexo_inpainting/model/paint_by_example.py
 hexo_inpainting/model/plms_sampler.py
+hexo_inpainting/model/schema.py
 hexo_inpainting/model/sd.py
 hexo_inpainting/model/utils.py
 hexo_inpainting/model/zits.py
 hexo_inpainting/model/pipeline/__init__.py
 hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
```

