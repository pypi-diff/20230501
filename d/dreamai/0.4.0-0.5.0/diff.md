# Comparing `tmp/dreamai-0.4.0.tar.gz` & `tmp/dreamai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-0.4.0.tar", last modified: Fri Apr 28 13:23:28 2023, max compression
+gzip compressed data, was "dreamai-0.5.0.tar", last modified: Mon May  1 20:38:28 2023, max compression
```

## Comparing `dreamai-0.4.0.tar` & `dreamai-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 13:23:28.502217 dreamai-0.4.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.4.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.4.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-04-28 13:23:28.502217 dreamai-0.4.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-01-18 23:32:17.000000 dreamai-0.4.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 13:23:28.502217 dreamai-0.4.0/dreamai/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-04-28 13:23:20.000000 dreamai-0.4.0/dreamai/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8319 2023-04-28 13:23:20.000000 dreamai-0.4.0/dreamai/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8852 2023-04-28 13:23:20.000000 dreamai-0.4.0/dreamai/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      632 2023-01-27 20:54:39.000000 dreamai-0.4.0/dreamai/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8252 2023-04-28 13:23:20.000000 dreamai-0.4.0/dreamai/vision.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 13:23:28.502217 dreamai-0.4.0/dreamai.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-04-28 13:23:28.000000 dreamai-0.4.0/dreamai.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-04-28 13:23:28.000000 dreamai-0.4.0/dreamai.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 13:23:28.000000 dreamai-0.4.0/dreamai.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-04-28 13:23:28.000000 dreamai-0.4.0/dreamai.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.4.0/dreamai.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      512 2023-04-28 13:23:28.000000 dreamai-0.4.0/dreamai.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-04-28 13:23:28.000000 dreamai-0.4.0/dreamai.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1172 2023-04-28 13:23:16.000000 dreamai-0.4.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-04-28 13:23:28.502217 dreamai-0.4.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.4.0/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-01 20:38:28.787012 dreamai-0.5.0/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.5.0/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.5.0/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-01 20:38:28.787012 dreamai-0.5.0/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-04-28 13:32:56.000000 dreamai-0.5.0/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-01 20:38:28.783012 dreamai-0.5.0/dreamai/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8109 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8778 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      636 2023-05-01 20:31:14.000000 dreamai-0.5.0/dreamai/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/vision.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-01 20:38:28.787012 dreamai-0.5.0/dreamai.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.5.0/dreamai.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1143 2023-05-01 20:34:56.000000 dreamai-0.5.0/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-01 20:38:28.787012 dreamai-0.5.0/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.5.0/setup.py
```

### Comparing `dreamai-0.4.0/LICENSE` & `dreamai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai-0.4.0/PKG-INFO` & `dreamai-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.4.0
+Version: 0.5.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.4.0/dreamai/_modidx.py` & `dreamai-0.5.0/dreamai/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/dreamai',
                 'doc_host': 'https://HamzaFarhan.github.io',
                 'git_url': 'https://github.com/HamzaFarhan/dreamai',
                 'lib_path': 'dreamai'},
   'syms': { 'dreamai.core': { 'dreamai.core._get_files': ('core.html#_get_files', 'dreamai/core.py'),
-                              'dreamai.core.default_device': ('core.html#default_device', 'dreamai/core.py'),
                               'dreamai.core.dict_keys': ('core.html#dict_keys', 'dreamai/core.py'),
                               'dreamai.core.dict_values': ('core.html#dict_values', 'dreamai/core.py'),
                               'dreamai.core.end_of_path': ('core.html#end_of_path', 'dreamai/core.py'),
                               'dreamai.core.extend_path_name': ('core.html#extend_path_name', 'dreamai/core.py'),
                               'dreamai.core.filter_dict': ('core.html#filter_dict', 'dreamai/core.py'),
                               'dreamai.core.flatten_list': ('core.html#flatten_list', 'dreamai/core.py'),
                               'dreamai.core.get_files': ('core.html#get_files', 'dreamai/core.py'),
@@ -27,15 +26,14 @@
                               'dreamai.core.is_norm': ('core.html#is_norm', 'dreamai/core.py'),
                               'dreamai.core.is_path': ('core.html#is_path', 'dreamai/core.py'),
                               'dreamai.core.is_pilimage': ('core.html#is_pilimage', 'dreamai/core.py'),
                               'dreamai.core.is_sequential': ('core.html#is_sequential', 'dreamai/core.py'),
                               'dreamai.core.is_set': ('core.html#is_set', 'dreamai/core.py'),
                               'dreamai.core.is_str': ('core.html#is_str', 'dreamai/core.py'),
                               'dreamai.core.is_subscriptable': ('core.html#is_subscriptable', 'dreamai/core.py'),
-                              'dreamai.core.is_tensor': ('core.html#is_tensor', 'dreamai/core.py'),
                               'dreamai.core.is_tuple': ('core.html#is_tuple', 'dreamai/core.py'),
                               'dreamai.core.is_unfrozen': ('core.html#is_unfrozen', 'dreamai/core.py'),
                               'dreamai.core.last_modified': ('core.html#last_modified', 'dreamai/core.py'),
                               'dreamai.core.list_map': ('core.html#list_map', 'dreamai/core.py'),
                               'dreamai.core.list_or_tuple': ('core.html#list_or_tuple', 'dreamai/core.py'),
                               'dreamai.core.load_obj': ('core.html#load_obj', 'dreamai/core.py'),
                               'dreamai.core.load_yaml': ('core.html#load_yaml', 'dreamai/core.py'),
```

### Comparing `dreamai-0.4.0/dreamai/core.py` & `dreamai-0.5.0/dreamai/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['default_device', 'flatten_list', 'noop', 'is_list', 'is_tuple', 'list_or_tuple', 'is_iter', 'is_dict', 'is_df',
-           'is_str', 'is_int', 'is_float', 'is_array', 'is_pilimage', 'is_img', 'is_tensor', 'is_set', 'is_path',
-           'path_or_str', 'is_norm', 'params', 'is_frozen', 'is_unfrozen', 'is_subscriptable', 'is_sequential',
-           'is_clip', 'path_name', 'path_stem', 'path_suffix', 'extend_path_name', 'end_of_path', 'last_modified',
-           'load_yaml', 'save_obj', 'load_obj', 'resolve_data_path', 'yml_to_pip', 'set_pip_req', 'merge_dicts',
-           'dict_values', 'dict_keys', 'sort_dict', 'locals_to_params', 'list_map', 'next_batch', 'model_children',
-           'replace_dict_key', 'proc_fn', 'filter_dict', 'setify', 'get_files']
+__all__ = ['flatten_list', 'noop', 'is_list', 'is_tuple', 'list_or_tuple', 'is_iter', 'is_dict', 'is_df', 'is_str', 'is_int',
+           'is_float', 'is_array', 'is_pilimage', 'is_img', 'is_set', 'is_path', 'path_or_str', 'is_norm', 'params',
+           'is_frozen', 'is_unfrozen', 'is_subscriptable', 'is_sequential', 'is_clip', 'path_name', 'path_stem',
+           'path_suffix', 'extend_path_name', 'end_of_path', 'last_modified', 'load_yaml', 'save_obj', 'load_obj',
+           'resolve_data_path', 'yml_to_pip', 'set_pip_req', 'merge_dicts', 'dict_values', 'dict_keys', 'sort_dict',
+           'locals_to_params', 'list_map', 'next_batch', 'model_children', 'replace_dict_key', 'proc_fn', 'filter_dict',
+           'setify', 'get_files']
 
 # %% ../nbs/00_core.ipynb 3
 from .imports import *
 
 # %% ../nbs/00_core.ipynb 4
-def default_device(device=None):
-    if device is None:
-        device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-    return device
+# def default_device(device=None):
+    # if device is None:
+        # device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+    # return device
 
 def flatten_list(l):
     "Flatten a list of lists."
     l2 = []
     for x in l:
         if is_list(x):
             l2 += flatten_list(x)
@@ -39,15 +39,14 @@
     return isinstance(x, tuple)
 
 def list_or_tuple(x):
     return (is_list(x) or is_tuple(x))
 
 def is_iter(o):
     "Test whether `o` can be used in a `for` loop."
-    #Rank 0 tensors in PyTorch are not really iterable
     return isinstance(o, (Iterable,Generator)) and getattr(o,'ndim',1)
 
 def is_dict(x):
     return isinstance(x, dict)
 
 def is_df(x):
     return isinstance(x, pd.core.frame.DataFrame)
@@ -66,16 +65,16 @@
 
 def is_pilimage(x):
     return 'PIL' in str(type(x))
 
 def is_img(x):
     return is_array(x) or is_pilimage(x)
 
-def is_tensor(x):
-    return isinstance(x, torch.Tensor)
+# def is_tensor(x):
+    # return isinstance(x, torch.Tensor)
 
 def is_set(x):
     return isinstance(x, set)
 
 def is_path(x):
     return isinstance(x, Path)
```

### Comparing `dreamai-0.4.0/dreamai/imports.py` & `dreamai-0.5.0/dreamai/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import torch
-from torch import nn
+# import torch
+# from torch import nn
 
 import os
 import cv2
 import json
 import copy
 import pickle
 import random
```

### Comparing `dreamai-0.4.0/dreamai/vision.py` & `dreamai-0.5.0/dreamai/vision.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     if t.dim() > 3:
         return [np.array(np.transpose(t_,(1,2,0))) for t_ in t]
     return np.array(np.transpose(t,(1,2,0)))
 
 def plt_show(im, cmap=None, title='', figsize=(7,7)):
     if path_or_str(im):
         im = rgb_read(im)
-    if is_tensor(im):
-        im = tensor_to_img(im)
-        if is_list(im): im = im[0]
+    # if is_tensor(im):
+        # im = tensor_to_img(im)
+        # if is_list(im): im = im[0]
     fig=plt.figure(figsize=figsize)
     plt.imshow(im, cmap=cmap)
     plt.title(title)
     plt.show()
 
 def show_img(img, cmap=None, title='', figsize=(7,7)):
     if not is_list(img):
```

### Comparing `dreamai-0.4.0/dreamai.egg-info/PKG-INFO` & `dreamai-0.5.0/dreamai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.4.0
+Version: 0.5.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.4.0/settings.ini` & `dreamai-0.5.0/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai
 lib_name = %(repo)s
-version = 0.4.0
+version = 0.5.0
 min_python = 3.8
 license = apache2
 doc_path = _docs
 lib_path = dreamai
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,9 +21,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = A bunch of cool and convenient utility functions.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = asttokens astunparse charset-normalizer contourpy cryptography cycler docutils execnb executing fastcore fonttools ghapi importlib-metadata imutils ipython jaraco-classes jedi jeepney keyring kiwisolver markdown-it-py matplotlib mdurl more-itertools nbdev numpy opencv-python packaging pandas pillow pip pkginfo pygments pyparsing pytz pyyaml readme-renderer requests requests-toolbelt rfc3986 rich secretstorage stack-data torch torchaudio torchvision traitlets twine urllib3 watchdog wcwidth wheel zipp
+pip_requirements = asttokens astunparse charset-normalizer contourpy cryptography cycler docutils execnb executing fastcore fonttools ghapi importlib-metadata imutils ipython jaraco-classes jedi jeepney keyring kiwisolver markdown-it-py matplotlib mdurl more-itertools nbdev numpy opencv-python packaging pandas pillow pip pkginfo pygments pyparsing pytz pyyaml readme-renderer requests requests-toolbelt rfc3986 rich secretstorage stack-data traitlets twine urllib3 watchdog wcwidth wheel zipp
```

### Comparing `dreamai-0.4.0/setup.py` & `dreamai-0.5.0/setup.py`

 * *Files identical despite different names*

