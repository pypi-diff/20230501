# Comparing `tmp/torch-scaler-0.0.1.tar.gz` & `tmp/torch-scaler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch-scaler-0.0.1.tar", last modified: Fri Apr 28 02:00:52 2023, max compression
+gzip compressed data, was "dist/torch-scaler-0.0.2.tar", last modified: Mon May  1 00:11:17 2023, max compression
```

## Comparing `torch-scaler-0.0.1.tar` & `torch-scaler-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 inhyukna   (501) staff       (20)        0 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/
--rw-r--r--   0 inhyukna   (501) staff       (20)     1067 2023-04-28 01:18:05.000000 torch-scaler-0.0.1/LICENSE
--rw-r--r--   0 inhyukna   (501) staff       (20)      318 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/PKG-INFO
--rw-r--r--   0 inhyukna   (501) staff       (20)      599 2023-04-28 01:53:47.000000 torch-scaler-0.0.1/README.md
--rw-r--r--   0 inhyukna   (501) staff       (20)       38 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/setup.cfg
--rw-r--r--   0 inhyukna   (501) staff       (20)      506 2023-04-28 01:27:58.000000 torch-scaler-0.0.1/setup.py
-drwxr-xr-x   0 inhyukna   (501) staff       (20)        0 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler/
--rw-r--r--   0 inhyukna   (501) staff       (20)       22 2023-04-28 01:33:07.000000 torch-scaler-0.0.1/torch_scaler/__init__.py
--rw-r--r--   0 inhyukna   (501) staff       (20)     1885 2023-04-28 01:50:50.000000 torch-scaler-0.0.1/torch_scaler/standard_scaler.py
-drwxr-xr-x   0 inhyukna   (501) staff       (20)        0 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/
--rw-r--r--   0 inhyukna   (501) staff       (20)      318 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/PKG-INFO
--rw-r--r--   0 inhyukna   (501) staff       (20)      297 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/SOURCES.txt
--rw-r--r--   0 inhyukna   (501) staff       (20)        1 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/dependency_links.txt
--rw-r--r--   0 inhyukna   (501) staff       (20)        1 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/not-zip-safe
--rw-r--r--   0 inhyukna   (501) staff       (20)       12 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/requires.txt
--rw-r--r--   0 inhyukna   (501) staff       (20)       13 2023-04-28 02:00:52.000000 torch-scaler-0.0.1/torch_scaler.egg-info/top_level.txt
+drwxr-xr-x   0 inhyukna   (501) staff       (20)        0 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/
+-rw-r--r--   0 inhyukna   (501) staff       (20)     1067 2023-04-28 01:18:05.000000 torch-scaler-0.0.2/LICENSE
+-rw-r--r--   0 inhyukna   (501) staff       (20)      335 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/PKG-INFO
+-rw-r--r--   0 inhyukna   (501) staff       (20)      670 2023-05-01 00:10:11.000000 torch-scaler-0.0.2/README.md
+-rw-r--r--   0 inhyukna   (501) staff       (20)       38 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/setup.cfg
+-rw-r--r--   0 inhyukna   (501) staff       (20)      523 2023-05-01 00:10:20.000000 torch-scaler-0.0.2/setup.py
+drwxr-xr-x   0 inhyukna   (501) staff       (20)        0 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler/
+-rw-r--r--   0 inhyukna   (501) staff       (20)       22 2023-05-01 00:10:27.000000 torch-scaler-0.0.2/torch_scaler/__init__.py
+-rw-r--r--   0 inhyukna   (501) staff       (20)     2116 2023-05-01 00:09:35.000000 torch-scaler-0.0.2/torch_scaler/standard_scaler.py
+drwxr-xr-x   0 inhyukna   (501) staff       (20)        0 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler.egg-info/
+-rw-r--r--   0 inhyukna   (501) staff       (20)      335 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler.egg-info/PKG-INFO
+-rw-r--r--   0 inhyukna   (501) staff       (20)      297 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler.egg-info/SOURCES.txt
+-rw-r--r--   0 inhyukna   (501) staff       (20)        1 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler.egg-info/dependency_links.txt
+-rw-r--r--   0 inhyukna   (501) staff       (20)        1 2023-04-28 02:00:52.000000 torch-scaler-0.0.2/torch_scaler.egg-info/not-zip-safe
+-rw-r--r--   0 inhyukna   (501) staff       (20)       12 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler.egg-info/requires.txt
+-rw-r--r--   0 inhyukna   (501) staff       (20)       13 2023-05-01 00:11:17.000000 torch-scaler-0.0.2/torch_scaler.egg-info/top_level.txt
```

### Comparing `torch-scaler-0.0.1/LICENSE` & `torch-scaler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-scaler-0.0.1/README.md` & `torch-scaler-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 
 ## How to use
 
 - Currently, we support standard scaler only.
 
 - We support `fit(x: torch.tensor)`, `partial_fit(x: torch.tensor)`, `transform(x: torch.tensor)`, `inverse_transform(x: torch.tensor)` similar to sklearn.preprocessing.StandardScaler.
   - x has to have shape of (batch_size, feature_dim)
+- We also support `cuda()` and `cpu()` for torch.tensor compatibility.
 - Please refer to https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html
 - You can see how-to-use example in `test.py`
```

### Comparing `torch-scaler-0.0.1/torch_scaler/standard_scaler.py` & `torch-scaler-0.0.2/torch_scaler/standard_scaler.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,7 +49,17 @@
         x /= (self.std + 1e-7)
         return x
     
     def inverse_transform(self, x):
         x *= (self.std + 1e-7)
         x += self.mean
         return x
+    
+    def cuda(self):
+        self.mean = self.mean.cuda()
+        self.std = self.std.cuda()
+        return self
+    
+    def cpu(self):
+        self.mean = self.mean.cpu()
+        self.std = self.std.cpu()
+        return self
```

