# Comparing `tmp/complex-network-link-prediction-1.0.1.tar.gz` & `tmp/complex-network-link-prediction-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex-network-link-prediction-1.0.1.tar", last modified: Fri Apr 28 19:55:19 2023, max compression
+gzip compressed data, was "complex-network-link-prediction-1.0.2.tar", last modified: Mon May  1 08:50:15 2023, max compression
```

## Comparing `complex-network-link-prediction-1.0.1.tar` & `complex-network-link-prediction-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/dimensionality_reduction_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/other_methods/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/other_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/other_methods/information_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/sbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/global_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/local_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/quasi_local_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:15.770084 complex-network-link-prediction-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-01 08:50:15.774084 complex-network-link-prediction-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:15.770084 complex-network-link-prediction-1.0.2/cnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/dimensionality_reduction_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:15.770084 complex-network-link-prediction-1.0.2/cnlp/other_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/other_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/other_methods/information_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:15.770084 complex-network-link-prediction-1.0.2/cnlp/probabilistic_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/probabilistic_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/probabilistic_methods/sbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:15.770084 complex-network-link-prediction-1.0.2/cnlp/similarity_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/similarity_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/similarity_methods/global_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/similarity_methods/local_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/similarity_methods/quasi_local_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/cnlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:50:15.770084 complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-01 08:50:15.000000 complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-01 08:50:15.000000 complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:50:15.000000 complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 08:50:15.000000 complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 08:50:15.000000 complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 08:50:15.774084 complex-network-link-prediction-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-01 08:50:14.000000 complex-network-link-prediction-1.0.2/setup.py
```

### Comparing `complex-network-link-prediction-1.0.1/LICENSE` & `complex-network-link-prediction-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/PKG-INFO` & `complex-network-link-prediction-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-network-link-prediction
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/Typing-Monkeys/social-network-link-prediction
 Author: Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani
 License: MIT
 Keywords: Link Prediction,Social Network,Complex Network Analisys
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `complex-network-link-prediction-1.0.1/README.md` & `complex-network-link-prediction-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/dimensionality_reduction_methods.py` & `complex-network-link-prediction-1.0.2/cnlp/dimensionality_reduction_methods.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/other_methods/information_theory.py` & `complex-network-link-prediction-1.0.2/cnlp/other_methods/information_theory.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/sbm.py` & `complex-network-link-prediction-1.0.2/cnlp/probabilistic_methods/sbm.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/__init__.py` & `complex-network-link-prediction-1.0.2/cnlp/similarity_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/global_similarity.py` & `complex-network-link-prediction-1.0.2/cnlp/similarity_methods/global_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/local_similarity.py` & `complex-network-link-prediction-1.0.2/cnlp/similarity_methods/local_similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,19 @@
     common neighbors between the two vertices considered. Some researcher
     (**Liben-Nowell et al.**) demonstrated that this similarity metric
     performs worse as compared to Common Neighbors.
     """
 
     def __jaccard(G: nx.Graph, x, y) -> float:
         """Compute the Jaccard Coefficient for 2 given nodes."""
-        return __common_neighbors(G, x, y) / len(set(G[x]).union(set(G[y])))
+        total_neighbor_number = len(set(G[x]).union(set(G[y])))
+        if total_neighbor_number == 0:
+            return 0
+        
+        return __common_neighbors(G, x, y) / total_neighbor_number
 
     size = G.number_of_nodes()
     S = lil_matrix((size, size))
     node_index_map = nodes_to_indexes(G)
 
     for x, y in nx.complement(G).edges():
         _x = node_index_map[x]
```

### Comparing `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/quasi_local_similarity.py` & `complex-network-link-prediction-1.0.2/cnlp/similarity_methods/quasi_local_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/cnlp/utils.py` & `complex-network-link-prediction-1.0.2/cnlp/utils.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/PKG-INFO` & `complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-network-link-prediction
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/Typing-Monkeys/social-network-link-prediction
 Author: Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani
 License: MIT
 Keywords: Link Prediction,Social Network,Complex Network Analisys
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/SOURCES.txt` & `complex-network-link-prediction-1.0.2/complex_network_link_prediction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0.1/setup.py` & `complex-network-link-prediction-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='complex-network-link-prediction',
-    version='1.0.1',
+    version='1.0.2',
     license='MIT',
     author=
     "Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani",
     packages=find_packages(where='.', include=['cnlp*']),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Typing-Monkeys/social-network-link-prediction',
```

