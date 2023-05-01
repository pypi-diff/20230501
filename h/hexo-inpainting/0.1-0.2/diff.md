# Comparing `tmp/hexo_inpainting-0.1.tar.gz` & `tmp/hexo_inpainting-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexo_inpainting-0.1.tar", last modified: Mon May  1 09:16:39 2023, max compression
+gzip compressed data, was "hexo_inpainting-0.2.tar", last modified: Mon May  1 09:34:45 2023, max compression
```

## Comparing `hexo_inpainting-0.1.tar` & `hexo_inpainting-0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:16:39.643578 hexo_inpainting-0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-01 09:16:39.643578 hexo_inpainting-0.1/PKG-INFO
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:16:39.639579 hexo_inpainting-0.1/hexo_inpainting/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       77 2023-05-01 09:16:12.000000 hexo_inpainting-0.1/hexo_inpainting/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4755 2023-04-25 07:57:38.000000 hexo_inpainting-0.1/hexo_inpainting/const.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8283 2023-04-25 07:54:35.000000 hexo_inpainting-0.1/hexo_inpainting/helper.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3691 2023-05-01 08:35:19.000000 hexo_inpainting-0.1/hexo_inpainting/inpainting.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:16:39.639579 hexo_inpainting-0.1/hexo_inpainting/model/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9462 2023-04-25 07:59:38.000000 hexo_inpainting-0.1/hexo_inpainting/model/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7288 2023-04-25 07:59:00.000000 hexo_inpainting-0.1/hexo_inpainting/model/controlnet.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6868 2023-04-25 08:01:21.000000 hexo_inpainting-0.1/hexo_inpainting/model/ddim_sampler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    57098 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/fcf.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3175 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/instruct_pix2pix.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1480 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/lama.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11197 2023-04-25 07:51:21.000000 hexo_inpainting-0.1/hexo_inpainting/model/ldm.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2884 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/manga.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    62625 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/mat.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      716 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/opencv2.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2934 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/paint_by_example.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:16:39.643578 hexo_inpainting-0.1/hexo_inpainting/model/pipeline/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      108 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/pipeline/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    28149 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11838 2023-04-25 08:02:19.000000 hexo_inpainting-0.1/hexo_inpainting/model/plms_sampler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6603 2023-04-25 07:53:47.000000 hexo_inpainting-0.1/hexo_inpainting/model/sd.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    33798 2023-04-25 07:52:59.000000 hexo_inpainting-0.1/hexo_inpainting/model/utils.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    15637 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/model/zits.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2417 2023-04-25 08:03:42.000000 hexo_inpainting-0.1/hexo_inpainting/model_manager.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5145 2023-05-01 08:35:33.000000 hexo_inpainting-0.1/hexo_inpainting/outpainting.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3306 2023-04-25 07:45:35.000000 hexo_inpainting-0.1/hexo_inpainting/schema.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:16:39.639579 hexo_inpainting-0.1/hexo_inpainting.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-01 09:16:39.000000 hexo_inpainting-0.1/hexo_inpainting.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1053 2023-05-01 09:16:39.000000 hexo_inpainting-0.1/hexo_inpainting.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 09:16:39.000000 hexo_inpainting-0.1/hexo_inpainting.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      194 2023-05-01 09:16:39.000000 hexo_inpainting-0.1/hexo_inpainting.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-01 09:16:39.000000 hexo_inpainting-0.1/hexo_inpainting.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 09:16:39.643578 hexo_inpainting-0.1/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      473 2023-05-01 09:14:52.000000 hexo_inpainting-0.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:34:45.804102 hexo_inpainting-0.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-01 09:34:45.804102 hexo_inpainting-0.2/PKG-INFO
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:34:45.800102 hexo_inpainting-0.2/hexo_inpainting/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       80 2023-05-01 09:34:27.000000 hexo_inpainting-0.2/hexo_inpainting/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4755 2023-04-25 07:57:38.000000 hexo_inpainting-0.2/hexo_inpainting/const.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8283 2023-04-25 07:54:35.000000 hexo_inpainting-0.2/hexo_inpainting/helper.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3755 2023-05-01 09:34:17.000000 hexo_inpainting-0.2/hexo_inpainting/inpainting.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:34:45.804102 hexo_inpainting-0.2/hexo_inpainting/model/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9462 2023-04-25 07:59:38.000000 hexo_inpainting-0.2/hexo_inpainting/model/base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7288 2023-04-25 07:59:00.000000 hexo_inpainting-0.2/hexo_inpainting/model/controlnet.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6868 2023-04-25 08:01:21.000000 hexo_inpainting-0.2/hexo_inpainting/model/ddim_sampler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    57098 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/fcf.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3175 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/instruct_pix2pix.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1480 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/lama.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11197 2023-04-25 07:51:21.000000 hexo_inpainting-0.2/hexo_inpainting/model/ldm.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2884 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/manga.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    62625 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/mat.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      716 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/opencv2.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2934 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/paint_by_example.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:34:45.804102 hexo_inpainting-0.2/hexo_inpainting/model/pipeline/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      108 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/pipeline/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    28149 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11838 2023-04-25 08:02:19.000000 hexo_inpainting-0.2/hexo_inpainting/model/plms_sampler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6603 2023-04-25 07:53:47.000000 hexo_inpainting-0.2/hexo_inpainting/model/sd.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    33798 2023-04-25 07:52:59.000000 hexo_inpainting-0.2/hexo_inpainting/model/utils.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    15637 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/model/zits.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2417 2023-04-25 08:03:42.000000 hexo_inpainting-0.2/hexo_inpainting/model_manager.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5145 2023-05-01 08:35:33.000000 hexo_inpainting-0.2/hexo_inpainting/outpainting.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3306 2023-04-25 07:45:35.000000 hexo_inpainting-0.2/hexo_inpainting/schema.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 09:34:45.800102 hexo_inpainting-0.2/hexo_inpainting.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-01 09:34:45.000000 hexo_inpainting-0.2/hexo_inpainting.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1053 2023-05-01 09:34:45.000000 hexo_inpainting-0.2/hexo_inpainting.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 09:34:45.000000 hexo_inpainting-0.2/hexo_inpainting.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      194 2023-05-01 09:34:45.000000 hexo_inpainting-0.2/hexo_inpainting.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-01 09:34:45.000000 hexo_inpainting-0.2/hexo_inpainting.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 09:34:45.804102 hexo_inpainting-0.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      473 2023-05-01 09:34:41.000000 hexo_inpainting-0.2/setup.py
```

### Comparing `hexo_inpainting-0.1/hexo_inpainting/const.py` & `hexo_inpainting-0.2/hexo_inpainting/const.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/helper.py` & `hexo_inpainting-0.2/hexo_inpainting/helper.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/inpainting.py` & `hexo_inpainting-0.2/hexo_inpainting/inpainting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+
+import sys
+sys.path.append('inpainting_hexo/hexo_inpainting')
+
 from model_manager import ModelManager
 from skimage import exposure
 from schema import Config, HDStrategy, LDMSampler, SDSampler
 import cv2
 import numpy as np
 import math
 import numpy as np
```

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/base.py` & `hexo_inpainting-0.2/hexo_inpainting/model/base.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/controlnet.py` & `hexo_inpainting-0.2/hexo_inpainting/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/ddim_sampler.py` & `hexo_inpainting-0.2/hexo_inpainting/model/ddim_sampler.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/fcf.py` & `hexo_inpainting-0.2/hexo_inpainting/model/fcf.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/instruct_pix2pix.py` & `hexo_inpainting-0.2/hexo_inpainting/model/instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/lama.py` & `hexo_inpainting-0.2/hexo_inpainting/model/lama.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/ldm.py` & `hexo_inpainting-0.2/hexo_inpainting/model/ldm.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/manga.py` & `hexo_inpainting-0.2/hexo_inpainting/model/manga.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/mat.py` & `hexo_inpainting-0.2/hexo_inpainting/model/mat.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/opencv2.py` & `hexo_inpainting-0.2/hexo_inpainting/model/opencv2.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/paint_by_example.py` & `hexo_inpainting-0.2/hexo_inpainting/model/paint_by_example.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py` & `hexo_inpainting-0.2/hexo_inpainting/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/plms_sampler.py` & `hexo_inpainting-0.2/hexo_inpainting/model/plms_sampler.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/sd.py` & `hexo_inpainting-0.2/hexo_inpainting/model/sd.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/utils.py` & `hexo_inpainting-0.2/hexo_inpainting/model/utils.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model/zits.py` & `hexo_inpainting-0.2/hexo_inpainting/model/zits.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/model_manager.py` & `hexo_inpainting-0.2/hexo_inpainting/model_manager.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/outpainting.py` & `hexo_inpainting-0.2/hexo_inpainting/outpainting.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting/schema.py` & `hexo_inpainting-0.2/hexo_inpainting/schema.py`

 * *Files identical despite different names*

### Comparing `hexo_inpainting-0.1/hexo_inpainting.egg-info/SOURCES.txt` & `hexo_inpainting-0.2/hexo_inpainting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

