# Comparing `tmp/image-reward-1.1.tar.gz` & `tmp/image-reward-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-1.1.tar", last modified: Sun Apr 16 14:37:53 2023, max compression
+gzip compressed data, was "dist/image-reward-1.2.tar", last modified: Mon May  1 02:43:28 2023, max compression
```

## Comparing `image-reward-1.1.tar` & `image-reward-1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     5437 2023-04-16 14:33:13.000000 image-reward-1.1/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-16 14:34:13.000000 image-reward-1.1/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-04-16 14:34:23.000000 image-reward-1.1/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-04-16 14:35:17.000000 image-reward-1.1/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 13:56:03.000000 image-reward-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4481 2023-04-16 14:37:53.000000 image-reward-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4172 2023-04-16 13:56:03.000000 image-reward-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4481 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 14:37:53.000000 image-reward-1.1/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 14:37:53.000000 image-reward-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      980 2023-04-16 14:37:22.000000 image-reward-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-05-01 02:33:51.000000 image-reward-1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7185 2023-05-01 02:43:28.000000 image-reward-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6876 2023-05-01 02:33:51.000000 image-reward-1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7185 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 02:43:28.000000 image-reward-1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-01 02:42:34.000000 image-reward-1.2/setup.py
```

### Comparing `image-reward-1.1/ImageReward/ImageReward.py` & `image-reward-1.2/ImageReward/ImageReward.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @Contact    :   xjz22@mails.tsinghua.edu.cn
 @Description:   ImageReward Reward model.
 * Based on CLIP code base and improved-aesthetic-predictor code base
 * https://github.com/openai/CLIP
 * https://github.com/christophschuhmann/improved-aesthetic-predictor
 '''
 
+import os
 import torch
 import torch.nn as nn
 from PIL import Image
 from .models.BLIP.blip_pretrain import BLIP_Pretrain
 from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor, Normalize
 
 try:
@@ -76,25 +77,32 @@
         self.preprocess = _transform(224)
         self.mlp = MLP(768)
         
         self.mean = 0.16717362830052426
         self.std = 1.0333394966054072
 
 
-    def score(self, prompt, image_path):
+    def score(self, prompt, image):
         
-        if (type(image_path).__name__=='list'):
-            _, rewards = self.inference_rank(prompt, image_path)
+        if (type(image).__name__=='list'):
+            _, rewards = self.inference_rank(prompt, image)
             return rewards
             
         # text encode
         text_input = self.blip.tokenizer(prompt, padding='max_length', truncation=True, max_length=35, return_tensors="pt").to(self.device)
         
         # image encode
-        pil_image = Image.open(image_path)
+        if isinstance(image, Image.Image):
+            pil_image = image
+        elif isinstance(image, str):
+            if os.path.isfile(image):
+                pil_image = Image.open(image)
+        else:
+            raise TypeError(r'This image parameter type has not been supportted yet. Please pass PIL.Image or file path str.')
+            
         image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
         image_embeds = self.blip.visual_encoder(image)
         
         # text encode cross attention with image
         image_atts = torch.ones(image_embeds.size()[:-1],dtype=torch.long).to(self.device)
         text_output = self.blip.text_encoder(text_input.input_ids,
                                                 attention_mask = text_input.attention_mask,
@@ -111,18 +119,23 @@
 
 
     def inference_rank(self, prompt, generations_list):
         
         text_input = self.blip.tokenizer(prompt, padding='max_length', truncation=True, max_length=35, return_tensors="pt").to(self.device)
         
         txt_set = []
-        for generations in generations_list:
+        for generation in generations_list:
             # image encode
-            img_path = generations
-            pil_image = Image.open(img_path)
+            if isinstance(generation, Image.Image):
+                pil_image = generation
+            elif isinstance(generation, str):
+                if os.path.isfile(generation):
+                    pil_image = Image.open(generation)
+            else:
+                raise TypeError(r'This image parameter type has not been supportted yet. Please pass PIL.Image or file path str.')
             image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
             image_embeds = self.blip.visual_encoder(image)
             
             # text encode cross attention with image
             image_atts = torch.ones(image_embeds.size()[:-1],dtype=torch.long).to(self.device)
             text_output = self.blip.text_encoder(text_input.input_ids,
                                                     attention_mask = text_input.attention_mask,
```

### Comparing `image-reward-1.1/ImageReward/models/AestheticScore.py` & `image-reward-1.2/ImageReward/models/AestheticScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/models/BLIP/blip.py` & `image-reward-1.2/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-1.2/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/models/BLIP/med.py` & `image-reward-1.2/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/models/BLIP/vit.py` & `image-reward-1.2/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/models/BLIPScore.py` & `image-reward-1.2/ImageReward/models/BLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/models/CLIPScore.py` & `image-reward-1.2/ImageReward/models/CLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/ImageReward/utils.py` & `image-reward-1.2/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/LICENSE` & `image-reward-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/image_reward.egg-info/SOURCES.txt` & `image-reward-1.2/image_reward.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-reward-1.1/setup.py` & `image-reward-1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="1.1",
+        version="1.2",
         author="Jiazheng Xu, et al.",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         url="https://github.com/THUDM/ImageReward",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
```

