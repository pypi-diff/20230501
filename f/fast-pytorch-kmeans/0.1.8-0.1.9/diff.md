# Comparing `tmp/fast_pytorch_kmeans-0.1.8.tar.gz` & `tmp/fast_pytorch_kmeans-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_pytorch_kmeans-0.1.8.tar", last modified: Thu Mar  9 18:57:37 2023, max compression
+gzip compressed data, was "fast_pytorch_kmeans-0.1.9.tar", last modified: Wed Mar 15 18:09:18 2023, max compression
```

## Comparing `fast_pytorch_kmeans-0.1.8.tar` & `fast_pytorch_kmeans-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 18:57:37.759116 fast_pytorch_kmeans-0.1.8/
--rw-rw-rw-   0        0        0     1077 2023-03-09 18:32:36.000000 fast_pytorch_kmeans-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      933 2023-03-09 18:57:37.759116 fast_pytorch_kmeans-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2002 2023-03-09 18:32:36.000000 fast_pytorch_kmeans-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 18:57:37.752608 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans/
--rw-rw-rw-   0        0        0      105 2023-03-09 18:32:36.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans/__init__.py
--rw-rw-rw-   0        0        0     6980 2023-03-09 18:56:23.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans/kmeans.py
--rw-rw-rw-   0        0        0     5851 2023-03-09 18:56:43.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans/multi_kmeans.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:57:37.759116 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/
--rw-rw-rw-   0        0        0      933 2023-03-09 18:57:37.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-03-09 18:57:37.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 18:57:37.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-03-09 18:57:37.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-09 18:57:37.000000 fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-09 18:57:37.763116 fast_pytorch_kmeans-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1868 2023-03-09 18:57:29.000000 fast_pytorch_kmeans-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-15 18:09:18.642869 fast_pytorch_kmeans-0.1.9/
+-rw-rw-rw-   0        0        0     1077 2023-03-09 18:32:36.000000 fast_pytorch_kmeans-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      933 2023-03-15 18:09:18.642869 fast_pytorch_kmeans-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2002 2023-03-09 18:32:36.000000 fast_pytorch_kmeans-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-15 18:09:18.633362 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans/
+-rw-rw-rw-   0        0        0      105 2023-03-09 18:32:36.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans/__init__.py
+-rw-rw-rw-   0        0        0     7847 2023-03-15 18:08:01.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans/kmeans.py
+-rw-rw-rw-   0        0        0     6653 2023-03-15 17:26:17.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans/multi_kmeans.py
+drwxrwxrwx   0        0        0        0 2023-03-15 18:09:18.642869 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/
+-rw-rw-rw-   0        0        0      933 2023-03-15 18:09:18.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-03-15 18:09:18.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-15 18:09:18.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-03-15 18:09:18.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-03-15 18:09:18.000000 fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-03-15 18:09:18.643870 fast_pytorch_kmeans-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2023-03-15 17:27:40.000000 fast_pytorch_kmeans-0.1.9/setup.py
```

### Comparing `fast_pytorch_kmeans-0.1.8/LICENSE.txt` & `fast_pytorch_kmeans-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast_pytorch_kmeans-0.1.8/PKG-INFO` & `fast_pytorch_kmeans-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_pytorch_kmeans
-Version: 0.1.8
+Version: 0.1.9
 Summary: a fast kmeans clustering algorithm implemented in pytorch
 Home-page: https://github.com/DeMoriarty/fast_pytorch_kmeans
 Download-URL: https://github.com/DeMoriarty/fast_pytorch_kmeans/archive/v_018.tar.gz
 Author: demoriarty
 Author-email: sahbanjan@gmail.com
 License: MIT
 Keywords: KMeans,K-means,pytorch,machine learning
```

### Comparing `fast_pytorch_kmeans-0.1.8/README.md` & `fast_pytorch_kmeans-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans/kmeans.py` & `fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans/kmeans.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,14 +110,16 @@
       sim_func = self.euc_sim
 
     if device == 'cpu':
       sim = sim_func(a, b)
       max_sim_v, max_sim_i = sim.max(dim=-1)
       return max_sim_v, max_sim_i
     else:
+      if a.dtype == torch.double:
+        expected = a.shape[0] * a.shape[1] * b.shape[0] * 8
       if a.dtype == torch.float:
         expected = a.shape[0] * a.shape[1] * b.shape[0] * 4
       elif a.dtype == torch.half:
         expected = a.shape[0] * a.shape[1] * b.shape[0] * 2
       ratio = math.ceil(expected / self.remaining_memory())
       subbatch_size = math.ceil(batch_size / ratio)
       msv, msi = [], []
@@ -148,14 +150,18 @@
       centroids: {torch.Tensor, None}, default: None
         if given, centroids will be initialized with given tensor
         if None, centroids will be randomly chosen from X
 
       Return:
       labels: torch.Tensor, shape: [n_samples]
     """
+    assert isinstance(X, torch.Tensor), "input must be torch.Tensor"
+    assert X.dtype in [torch.half, torch.float, torch.double], "input must be floating point"
+    assert X.ndim == 2, "input must be a 2d tensor with shape: [n_samples, n_features] "
+
     batch_size, emb_dim = X.shape
     device = X.device.type
     start_time = time()
     if centroids is None:
       self.centroids = X[np.random.choice(batch_size, size=[self.n_clusters], replace=False)]
     else:
       self.centroids = centroids
@@ -207,17 +213,25 @@
 
       Parameters:
       X: torch.Tensor, shape: [n_samples, n_features]
 
       Return:
       labels: torch.Tensor, shape: [n_samples]
     """
+    assert isinstance(X, torch.Tensor), "input must be torch.Tensor"
+    assert X.dtype in [torch.half, torch.float, torch.double], "input must be floating point"
+    assert X.ndim == 2, "input must be a 2d tensor with shape: [n_samples, n_features] "
+
     return self.max_sim(a=X, b=self.centroids)[1]
 
   def fit(self, X, centroids=None):
     """
       Perform kmeans clustering
 
       Parameters:
       X: torch.Tensor, shape: [n_samples, n_features]
     """
+    assert isinstance(X, torch.Tensor), "input must be torch.Tensor"
+    assert X.dtype in [torch.half, torch.float, torch.double], "input must be floating point"
+    assert X.ndim == 2, "input must be a 2d tensor with shape: [n_samples, n_features] "
+
     self.fit_predict(X, centroids)
```

### Comparing `fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans/multi_kmeans.py` & `fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans/multi_kmeans.py`

 * *Files 14% similar despite different names*

```diff
@@ -111,14 +111,18 @@
       X: torch.Tensor, shape: [n_samples, n_features]
       centroids: {torch.Tensor, None}, default: None
         if given, centroids will be initialized with given tensor
         if None, centroids will be randomly chosen from X
       Return:
       labels: torch.Tensor, shape: [n_samples]
     """
+    assert isinstance(X, torch.Tensor), "input must be torch.Tensor"
+    assert X.dtype in [torch.half, torch.float, torch.double], "input must be floating point"
+    assert X.ndim == 3, "input must be a 3d tensor with shape: [n_kmeans, n_samples, n_features]"
+    
     n_kmeans, n_samples, n_features = X.shape
     self.n_kmeans = n_kmeans
 
     device = X.device.type
     start_time = time()
     if self.centroids is None:
       self.centroids = X[:, np.random.choice(n_samples, size=[self.n_clusters], replace=False)]
@@ -163,16 +167,24 @@
     """
       Predict the closest cluster each sample in X belongs to
       Parameters:
       X: torch.Tensor, shape: [n_kmeans, n_samples, n_features]
       Return:
       labels: torch.Tensor, shape: [n_kmeans, n_samples]
     """
+    assert isinstance(X, torch.Tensor), "input must be torch.Tensor"
+    assert X.dtype in [torch.half, torch.float, torch.double], "input must be floating point"
+    assert X.ndim == 3, "input must be a 3d tensor with shape: [n_kmeans, n_samples, n_features]"
+
     return self.max_sim(a=X, b=self.centroids)[1]
 
   def fit(self, X, centroids=None):
     """
       Perform kmeans clustering
       Parameters:
       X: torch.Tensor, shape: [n_kmeans, n_samples, n_features]
     """
+    assert isinstance(X, torch.Tensor), "input must be torch.Tensor"
+    assert X.dtype in [torch.half, torch.float, torch.double], "input must be floating point"
+    assert X.ndim == 3, "input must be a 3d tensor with shape: [n_kmeans, n_samples, n_features]"
+
     self.fit_predict(X, centroids)
```

### Comparing `fast_pytorch_kmeans-0.1.8/fast_pytorch_kmeans.egg-info/PKG-INFO` & `fast_pytorch_kmeans-0.1.9/fast_pytorch_kmeans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-pytorch-kmeans
-Version: 0.1.8
+Version: 0.1.9
 Summary: a fast kmeans clustering algorithm implemented in pytorch
 Home-page: https://github.com/DeMoriarty/fast_pytorch_kmeans
 Download-URL: https://github.com/DeMoriarty/fast_pytorch_kmeans/archive/v_018.tar.gz
 Author: demoriarty
 Author-email: sahbanjan@gmail.com
 License: MIT
 Keywords: KMeans,K-means,pytorch,machine learning
```

### Comparing `fast_pytorch_kmeans-0.1.8/setup.py` & `fast_pytorch_kmeans-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'fast_pytorch_kmeans',         # How you named your package folder (MyLib)
   packages = ['fast_pytorch_kmeans'],   # Chose the same as "name"
-  version = '0.1.8',      # Start with a small number and increase it with every change you make
+  version = '0.1.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a fast kmeans clustering algorithm implemented in pytorch',   # Give a short description about your library
   author = 'demoriarty',                   # Type in your name
   author_email = 'sahbanjan@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/DeMoriarty/fast_pytorch_kmeans',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/DeMoriarty/fast_pytorch_kmeans/archive/v_018.tar.gz',    # I explain this later on
   keywords = ['KMeans', 'K-means', 'pytorch','machine learning'],   # Keywords that define your package best
```

