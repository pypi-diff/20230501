# Comparing `tmp/zadu-0.0.8.tar.gz` & `tmp/zadu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zadu-0.0.8.tar", last modified: Mon May  1 08:43:56 2023, max compression
+gzip compressed data, was "zadu-0.1.0.tar", last modified: Mon May  1 11:41:40 2023, max compression
```

## Comparing `zadu-0.0.8.tar` & `zadu-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.611116 zadu-0.0.8/
--rw-rw-r--   0 hj        (1010) hj        (1010)     7646 2023-05-01 08:43:56.611116 zadu-0.0.8/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)     5791 2023-05-01 08:32:45.000000 zadu-0.0.8/README.md
--rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-05-01 08:43:56.611116 zadu-0.0.8/setup.cfg
--rw-rw-r--   0 hj        (1010) hj        (1010)      856 2023-05-01 08:43:29.000000 zadu-0.0.8/setup.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.607116 zadu-0.0.8/src/
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.607116 zadu-0.0.8/src/zadu/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:34.000000 zadu-0.0.8/src/zadu/__init__.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.611116 zadu-0.0.8/src/zadu/measures/
--rw-rw-r--   0 hj        (1010) hj        (1010)      495 2023-04-30 14:16:48.000000 zadu-0.0.8/src/zadu/measures/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2685 2023-04-13 09:45:13.000000 zadu-0.0.8/src/zadu/measures/class_aware_trustworthiness_continuity.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1438 2023-04-13 09:45:25.000000 zadu-0.0.8/src/zadu/measures/clustering_and_external_validation_measure.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      920 2023-04-13 09:45:30.000000 zadu-0.0.8/src/zadu/measures/distance_consistency.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      867 2023-04-13 09:45:35.000000 zadu-0.0.8/src/zadu/measures/distance_to_measure.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      715 2023-04-13 09:45:42.000000 zadu-0.0.8/src/zadu/measures/internal_validation_measure.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      909 2023-04-13 09:45:48.000000 zadu-0.0.8/src/zadu/measures/kl_divergence.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1211 2023-04-13 09:45:53.000000 zadu-0.0.8/src/zadu/measures/local_continuity_meta_criteria.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2203 2023-04-13 09:45:59.000000 zadu-0.0.8/src/zadu/measures/mean_relative_rank_error.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1107 2023-04-13 09:46:04.000000 zadu-0.0.8/src/zadu/measures/neighbor_dissimilarity.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1025 2023-04-13 09:46:10.000000 zadu-0.0.8/src/zadu/measures/neighborhood_hit.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      775 2023-04-13 09:46:15.000000 zadu-0.0.8/src/zadu/measures/pearson_r.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1175 2023-05-01 08:38:08.000000 zadu-0.0.8/src/zadu/measures/procrustes.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      795 2023-04-13 09:46:20.000000 zadu-0.0.8/src/zadu/measures/spearman_rho.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2124 2023-05-01 08:40:11.000000 zadu-0.0.8/src/zadu/measures/steadiness_cohesiveness.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      808 2023-04-14 20:28:49.000000 zadu-0.0.8/src/zadu/measures/stress.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1650 2023-05-01 08:06:02.000000 zadu-0.0.8/src/zadu/measures/topographic_product.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2154 2023-05-01 08:40:05.000000 zadu-0.0.8/src/zadu/measures/trustworthiness_continuity.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.611116 zadu-0.0.8/src/zadu/measures/utils/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-06 03:59:50.000000 zadu-0.0.8/src/zadu/measures/utils/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     3200 2023-04-15 02:30:27.000000 zadu-0.0.8/src/zadu/measures/utils/knn.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1166 2023-04-06 15:35:44.000000 zadu-0.0.8/src/zadu/measures/utils/pairwise_dist.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     6706 2023-05-01 08:32:45.000000 zadu-0.0.8/src/zadu/zadu.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.611116 zadu-0.0.8/src/zadu.egg-info/
--rw-rw-r--   0 hj        (1010) hj        (1010)     7646 2023-05-01 08:43:56.000000 zadu-0.0.8/src/zadu.egg-info/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)     1154 2023-05-01 08:43:56.000000 zadu-0.0.8/src/zadu.egg-info/SOURCES.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-05-01 08:43:56.000000 zadu-0.0.8/src/zadu.egg-info/dependency_links.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       50 2023-05-01 08:43:56.000000 zadu-0.0.8/src/zadu.egg-info/requires.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-05-01 08:43:56.000000 zadu-0.0.8/src/zadu.egg-info/top_level.txt
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 08:43:56.611116 zadu-0.0.8/src/zaduvis/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:47.000000 zadu-0.0.8/src/zaduvis/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1629 2023-04-08 07:45:55.000000 zadu-0.0.8/src/zaduvis/colormap.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1798 2023-04-09 02:48:07.000000 zadu-0.0.8/src/zaduvis/zaduvis.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.067700 zadu-0.1.0/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     7666 2023-05-01 11:41:40.067700 zadu-0.1.0/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)     7219 2023-05-01 11:40:58.000000 zadu-0.1.0/README.md
+-rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-05-01 11:41:40.067700 zadu-0.1.0/setup.cfg
+-rw-rw-r--   0 hj        (1010) hj        (1010)      856 2023-05-01 11:39:05.000000 zadu-0.1.0/setup.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.063700 zadu-0.1.0/src/
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.063700 zadu-0.1.0/src/zadu/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:34.000000 zadu-0.1.0/src/zadu/__init__.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.067700 zadu-0.1.0/src/zadu/measures/
+-rw-rw-r--   0 hj        (1010) hj        (1010)      495 2023-04-30 14:16:48.000000 zadu-0.1.0/src/zadu/measures/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2685 2023-04-13 09:45:13.000000 zadu-0.1.0/src/zadu/measures/class_aware_trustworthiness_continuity.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1438 2023-04-13 09:45:25.000000 zadu-0.1.0/src/zadu/measures/clustering_and_external_validation_measure.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      921 2023-05-01 08:44:31.000000 zadu-0.1.0/src/zadu/measures/distance_consistency.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      867 2023-04-13 09:45:35.000000 zadu-0.1.0/src/zadu/measures/distance_to_measure.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      715 2023-04-13 09:45:42.000000 zadu-0.1.0/src/zadu/measures/internal_validation_measure.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      909 2023-04-13 09:45:48.000000 zadu-0.1.0/src/zadu/measures/kl_divergence.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1211 2023-04-13 09:45:53.000000 zadu-0.1.0/src/zadu/measures/local_continuity_meta_criteria.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2203 2023-04-13 09:45:59.000000 zadu-0.1.0/src/zadu/measures/mean_relative_rank_error.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1107 2023-04-13 09:46:04.000000 zadu-0.1.0/src/zadu/measures/neighbor_dissimilarity.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1025 2023-04-13 09:46:10.000000 zadu-0.1.0/src/zadu/measures/neighborhood_hit.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      775 2023-04-13 09:46:15.000000 zadu-0.1.0/src/zadu/measures/pearson_r.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1175 2023-05-01 08:38:08.000000 zadu-0.1.0/src/zadu/measures/procrustes.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      795 2023-04-13 09:46:20.000000 zadu-0.1.0/src/zadu/measures/spearman_rho.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2124 2023-05-01 08:40:11.000000 zadu-0.1.0/src/zadu/measures/steadiness_cohesiveness.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      808 2023-04-14 20:28:49.000000 zadu-0.1.0/src/zadu/measures/stress.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1650 2023-05-01 08:06:02.000000 zadu-0.1.0/src/zadu/measures/topographic_product.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2154 2023-05-01 08:40:05.000000 zadu-0.1.0/src/zadu/measures/trustworthiness_continuity.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.067700 zadu-0.1.0/src/zadu/measures/utils/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-06 03:59:50.000000 zadu-0.1.0/src/zadu/measures/utils/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     3200 2023-04-15 02:30:27.000000 zadu-0.1.0/src/zadu/measures/utils/knn.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1166 2023-04-06 15:35:44.000000 zadu-0.1.0/src/zadu/measures/utils/pairwise_dist.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     6662 2023-05-01 08:44:31.000000 zadu-0.1.0/src/zadu/zadu.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.063700 zadu-0.1.0/src/zadu.egg-info/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     7666 2023-05-01 11:41:40.000000 zadu-0.1.0/src/zadu.egg-info/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1154 2023-05-01 11:41:40.000000 zadu-0.1.0/src/zadu.egg-info/SOURCES.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-05-01 11:41:40.000000 zadu-0.1.0/src/zadu.egg-info/dependency_links.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       50 2023-05-01 11:41:40.000000 zadu-0.1.0/src/zadu.egg-info/requires.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-05-01 11:41:40.000000 zadu-0.1.0/src/zadu.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-01 11:41:40.067700 zadu-0.1.0/src/zaduvis/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-30 14:50:47.000000 zadu-0.1.0/src/zaduvis/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1629 2023-04-08 07:45:55.000000 zadu-0.1.0/src/zaduvis/colormap.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1798 2023-04-09 02:48:07.000000 zadu-0.1.0/src/zaduvis/zaduvis.py
```

### Comparing `zadu-0.0.8/PKG-INFO` & `zadu-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,185 +1,209 @@
-Metadata-Version: 2.1
-Name: zadu
-Version: 0.0.8
-Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
-Home-page: https://github.com/hj-n/zadu
-Author: Hyeon Jeon
-Author-email: hj@hcil.snu.ac.kr
-License: UNKNOWN
-Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
-        
-        ZADU is a Python library that provides a comprehensive suite of distortion measures for evaluating and analyzing dimensionality reduction (DR) embeddings. The library supports a diverse set of local, cluster-level, and global distortion measures, allowing users to assess DR techniques from various structural perspectives. By offering an optimized scheduling scheme and pointwise local distortions, ZADU enables efficient and in-depth analysis of DR embeddings.
-        
-        
-        ## Installation
-        
-        You can install ZADU via `pip`:
-        
-        ```bash
-        pip install zadu
-        ```
-        
-        ## Supported Distortion Measures
-        
-        ZADU currently supports a total of 17 distortion measures, including:
-        
-        - 7 local measures
-        - 4 cluster-level measures
-        - 6 global measures
-        
-        For a complete list of supported measures, refer to [measures](/src/zadu/measures).
-        
-        ## How To Use ZADU
-        
-        ZADU provides two different interfaces for executing distortion measures.
-        You can either use the main class that wraps the measures, or directly access and invoke the functions that define each distortion measure.
-        
-        ### Using the Main Class
-        
-        Use the main class of ZADU to compute distortion measures.
-        This approach benefits from the scheduling scheme, providing faster performance.
-        
-        
-        ```python
-        from zadu import zadu
-        
-        hd, ld = load_datasets()
-        spec = [{
-            "id"    : "tnc",
-            "params": { "k": 20 },
-        }, {
-            "id"    : "snc",
-            "params": { "k": 30, "clustering": "hdbscan" }
-        }]
-        
-        scores = zadu.ZADU(spec, hd).measure(ld)
-        print("T&C:", scores[0])
-        print("S&C:", scores[1])
-        
-        ```
-        
-        `hd` represents high-dimensional data, `ld` represents low-dimensional data
-        
-        ## zadu.ZADU Class
-        
-        The zadu.ZADU class provides the main interface for the Zadu library, allowing users to evaluate and analyze dimensionality reduction (DR) embeddings effectively and reliably.
-        
-        ### Class Constructor
-        
-        The Zadu.ZADU class constructor has the following signature:
-        
-        ```python
-        class ZADU(spec: List[Dict[str, Union[str, dict]]], hd: np.ndarray, return_local: bool = False)
-        
-        ```
-        
-        #### Parameters:
-        
-        ##### `spec` 
-        &nbsp;&nbsp;&nbsp;&nbsp;
-        A list of dictionaries that define the distortion measures to execute and their hyperparameters.
-        Each dictionary must contain the following keys:
-          * `"id"`: The identifier of the distortion measure, such as `"tnc"` or `"snc"`.
-        
-          * `"params"`: A dictionary containing hyperparameters specific to the chosen distortion measure.
-        
-        
-        ##### `hd`
-        &nbsp;&nbsp;&nbsp;&nbsp;
-        A high-dimensional dataset (numpy array) to register and reuse during the evaluation process.
-        
-        
-        ##### `return_local`
-        &nbsp;&nbsp;&nbsp;&nbsp;
-        A boolean flag that, when set to `True`, enables the computation of local pointwise distortions for each data point. The default value is `False`.
-        
-        
-        ### Directly Accessing Functions
-        
-        You can also directly access and invoke the functions defining each distortion measure for greater flexibility.
-        
-        ```python
-        from zadu.measures import *
-        
-        mrre = mean_relative_rank_error.run(hd, ld, k=20)
-        pr  = pearson_r.run(hd, ld)
-        nh  = neighborhood_hit.run(ld, label, k=20)
-        ```
-        
-        ## Advanced Features
-        
-        ### Scheduling the Execution
-        
-        ZADU optimizes the execution of multiple distortion measures through an effective scheduling scheme. It minimizes the computational overhead associated with preprocessing stages such as pairwise distance calculation, pointwise distance ranking determination, and k-nearest neighbor identification.
-        
-        ### Computing Pointwise Local Distortions
-        
-        Users can obtain local pointwise distortions by setting the return_local flag. If a specified distortion measure produces local pointwise distortion as intermediate results, it returns a list of pointwise distortions when the flag is raised.
-        
-        ```python
-        from zadu import zadu
-        
-        spec = [{
-            "id"    : "dtm",
-            "params": {}
-        }, {
-            "id"    : "mrre",
-            "params": { "k": 30 }
-        }]
-        
-        zadu_obj = zadu.ZADU(spec, hd, return_local=True)
-        global_, local_ = zadu_obj.measure(ld)
-        print("MRRE local distortions:", local_[1])
-        
-        ```
-        
-        ### Visualizing Local Distortions
-        
-        With the pointwise local distortions obtained from ZADU, users can visualize the distortions using various distortion visualizations. For example, CheckViz and the Reliability Map can be implemented using a Python visualization library with zaduvis.
-        
-        <img alt="image" src="https://user-images.githubusercontent.com/38465539/235427171-94dcc220-7cbb-4ee6-94b3-20cc96ffbfa8.png">
-        
-        ```python
-        from zadu import zadu
-        from zaduvis import zaduvis
-        import matplotlib.pyplot as plt
-        from sklearn.manifold import TSNE
-        from sklearn.datasets import fetch_openml
-        
-        ## load datasets and generate an embedding
-        hd = fetch_openml("mnist_784", version=1, cache=True).target.astype(int)[::7]
-        ld = TSNE.fit_transform(hd)
-        
-        ## Computing local pointwise distortions
-        specs = [{"id": "snc", "params": {"k": 50}}]
-        zadu_obj = zadu.ZADU(spec, hd, return_local=True)
-        global_, local_ = zadu_obj.measure(ld)
-        l_s = local_[0]["local_steadiness"]
-        l_c = local_[0]["local_cohesiveness"]
-        
-        ## Visualizing local distortions
-        fig, ax = plt.subplots(1, 2, figsize=(20, 10))
-        zaduvis.checkviz(ld, l_s, l_c, ax=ax[0])
-        zaduvis.reliability_map(ld, l_s, l_c, ax=ax[1])
-        
-        ```
-        
-        
-        The above code snippet demonstrates how to visualize local pointwise distortions using CheckViz and Reliability Map plots. `zaduvis.checkviz` generates a CheckViz plot, which shows local Steadiness (x-axis) vs. local Cohesiveness (y-axis) for each point in the embedding. `zaduvis.reliability_map` creates a Reliability Map plot, which colors each point in the embedding according to its local Steadiness and local Cohesiveness values.
-        
-        ## Documentation
-        
-        For more information about the available distortion measures, their use cases, and examples, please refer to our [paper](zadu.pdf).
-        
-        ##Citation
-        
-        ##License
-        
-        ##Contributing
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
+# ZADU: A Python Library for Evaluating the Reliability of Dimensionality Reduction Embeddings
+
+ZADU is a Python library that provides distortion measures for evaluating and analyzing dimensionality reduction (DR) embeddings. The library supports a diverse set of local, cluster-level, and global distortion measures, allowing users to assess DR techniques from various structural perspectives. By offering an optimized execution and pointwise local distortions, ZADU enables efficient and in-depth analysis of DR embeddings.
+
+
+## Installation
+
+You can install ZADU via `pip`:
+
+```bash
+pip install zadu
+```
+
+## Supported Distortion Measures
+
+ZADU currently supports a total of 17 distortion measures, including:
+
+- 7 local measures
+- 4 cluster-level measures
+- 6 global measures
+
+For a complete list of supported measures, refer to [measures](/src/zadu/measures).
+
+## How To Use ZADU
+
+ZADU provides two different interfaces for executing distortion measures.
+You can either use the main class that wraps the measures, or directly access and invoke the functions that define each distortion measure.
+
+### Using the Main Class
+
+Use the main class of ZADU to compute distortion measures.
+This approach benefits from the optimization, providing faster performance when executing multiple measures.
+
+
+```python
+from zadu import zadu
+
+hd, ld = load_datasets()
+spec = [{
+    "id"    : "tnc",
+    "params": { "k": 20 },
+}, {
+    "id"    : "snc",
+    "params": { "k": 30, "clustering": "hdbscan" }
+}]
+
+scores = zadu.ZADU(spec, hd).measure(ld)
+print("T&C:", scores[0])
+print("S&C:", scores[1])
+
+```
+
+`hd` represents high-dimensional data, `ld` represents low-dimensional data
+
+## ZADU Class
+
+The ZADU class provides the main interface for the Zadu library, allowing users to evaluate and analyze dimensionality reduction (DR) embeddings effectively and reliably.
+
+### Class Constructor
+
+The ZADU class constructor has the following signature:
+
+```python
+class ZADU(spec: List[Dict[str, Union[str, dict]]], hd: np.ndarray, return_local: bool = False)
+
+```
+
+#### Parameters:
+
+##### `spec` 
+&nbsp;&nbsp;&nbsp;&nbsp;
+A list of dictionaries that define the distortion measures to execute and their hyperparameters.
+Each dictionary must contain the following keys:
+  * `"id"`: The identifier of the distortion measure, such as `"tnc"` or `"snc"`.
+
+  * `"params"`: A dictionary containing hyperparameters specific to the chosen distortion measure.
+
+<details>
+<summary style="cursor: pointer; font-weight: bold; color: #0066cc;">List of ID/Parameters for Each Function</summary>
+
+### Local Measures
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Trustworthiness & Continuity | tnc | `k=20` | [0.5, 1] | 1 |
+| Mean Relative Rank Errors | mrre | `k=20` | [0, 1] | 1 | 
+| Local Continuity Meta-Criteria | lcmc | `k=20` | [0, 1] | 1 |
+| Neighborhood hit | nh | `k=20` | [0, 1] | 1 |
+| Neighbor Dissimilarity | nd | `k=20` | R+ | 0 |
+| Class-Aware Trustworthiness & Continuity | ca_tnc | `k=20` | [0.5, 1] | 1|
+| Procrustes Measure | proc | `k=20` | R+ | 0 |
+
+### Cluster-level
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Steadiness & Cohesiveness | snc | `iteration=150, walk_num_ratio=0.3, alpha=0.1, k=50, clustering_strategy="dbscan"` | [0, 1] | 1 |
+| Distance Consistency | dsc | | [0.5, 1] | 0.5 | 
+| Internal Validation Measures | ivm | `measure="silhouette"` | Depends on IVM | Depends on IVM |
+| Clustering + External Clustering Validation Measures | c_evm | `measure="arand", clustering="kmeans", clustering_args=None` | Depends on EVM | Depends on EVM |
+
+### Global
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Stress | stress | | R+ | 0 |
+| Kullback-Leibler Divergence | kl_div | `sigma=0.1` | R+ | 0 |
+| Distance-to-Measure | dtm | `sigma=0.1` | R+ | 0 |
+| Topographic Product | topo | `k=20` | R | 0 |
+| Pearson’s correlation coefficient | pr | | [-1, 1] | 1
+| Spearman’s rank correlation coefficient | srho | | [-1, 1] | 1
+
+
+</details>
+
+##### `hd`
+&nbsp;&nbsp;&nbsp;&nbsp;
+A high-dimensional dataset (numpy array) to register and reuse during the evaluation process.
+
+
+##### `return_local`
+&nbsp;&nbsp;&nbsp;&nbsp;
+A boolean flag that, when set to `True`, enables the computation of local pointwise distortions for each data point. The default value is `False`.
+
+
+### Directly Accessing Functions
+
+You can also directly access and invoke the functions defining each distortion measure for greater flexibility.
+
+```python
+from zadu.measures import *
+
+mrre = mean_relative_rank_error.measure(hd, ld, k=20)
+pr  = pearson_r.measure(hd, ld)
+nh  = neighborhood_hit.measure(ld, label, k=20)
+```
+
+## Advanced Features
+
+### Optimizing the Execution
+
+ZADU automatically optimizes the execution of multiple distortion measures. It minimizes the computational overhead associated with preprocessing stages such as pairwise distance calculation, pointwise distance ranking determination, and k-nearest neighbor identification.
+
+### Computing Pointwise Local Distortions
+
+Users can obtain local pointwise distortions by setting the return_local flag. If a specified distortion measure produces local pointwise distortion as intermediate results, it returns a list of pointwise distortions when the flag is raised.
+
+```python
+from zadu import zadu
+
+spec = [{
+    "id"    : "dtm",
+    "params": {}
+}, {
+    "id"    : "mrre",
+    "params": { "k": 30 }
+}]
+
+zadu_obj = zadu.ZADU(spec, hd, return_local=True)
+global_, local_ = zadu_obj.measure(ld)
+print("MRRE local distortions:", local_[1])
+
+```
+
+### Visualizing Local Distortions
+
+With the pointwise local distortions obtained from ZADU, users can visualize the distortions using various distortion visualizations. We provide ZADUVis, a python library that enables the rendering of two disotortion visualizations: [CheckViz](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1467-8659.2010.01835.x) and the [Reliability Map](https://arxiv.org/abs/2107.07859).
+
+
+![img](https://user-images.githubusercontent.com/38465539/235427171-94dcc220-7cbb-4ee6-94b3-20cc96ffbfa8.png)
+
+```python
+from zadu import zadu
+from zaduvis import zaduvis
+import matplotlib.pyplot as plt
+from sklearn.manifold import TSNE
+from sklearn.datasets import fetch_openml
+
+
+## load datasets and generate an embedding
+hd = fetch_openml('mnist_784', version=1, cache=True).target.astype(int)[::7]
+ld = TSNE.fit_transform(hd)
+
+## Computing local pointwise distortions
+specs = [{"id": "snc", "params": {"k": 50}}]
+zadu_obj = zadu.ZADU(spec, hd, return_local=True)
+global_, local_ = zadu_obj.measure(ld)
+l_s = local_[0]["local_steadiness"]
+l_c = local_[0]["local_cohesiveness"]
+
+## Visualizing local distortions
+fig, ax = plt.subplots(1, 2, figsize=(20, 10))
+zaduvis.checkviz(ld, l_s, l_c, ax=ax[0])
+zaduvis.reliability_map(ld, l_s, l_c, ax=ax[1])
+
+```
+
+
+The above code snippet demonstrates how to visualize local pointwise distortions using CheckViz and Reliability Map plots.
+
+## Documentation
+
+For more information about the available distortion measures, their use cases, and examples, please refer to our paper [TBD].
+
+## Citation
+
+## License
+
+## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zadu-0.0.8/README.md` & `zadu-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,23 @@
-# ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
+Metadata-Version: 2.1
+Name: zadu
+Version: 0.1.0
+Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
+Home-page: https://github.com/hj-n/zadu
+Author: Hyeon Jeon
+Author-email: hj@hcil.snu.ac.kr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
 
-ZADU is a Python library that provides a comprehensive suite of distortion measures for evaluating and analyzing dimensionality reduction (DR) embeddings. The library supports a diverse set of local, cluster-level, and global distortion measures, allowing users to assess DR techniques from various structural perspectives. By offering an optimized scheduling scheme and pointwise local distortions, ZADU enables efficient and in-depth analysis of DR embeddings.
+# ZADU: A Python Library for Evaluating the Reliability of Dimensionality Reduction Embeddings
+
+ZADU is a Python library that provides distortion measures for evaluating and analyzing dimensionality reduction (DR) embeddings. The library supports a diverse set of local, cluster-level, and global distortion measures, allowing users to assess DR techniques from various structural perspectives. By offering an optimized execution and pointwise local distortions, ZADU enables efficient and in-depth analysis of DR embeddings.
 
 
 ## Installation
 
 You can install ZADU via `pip`:
 
 ```bash
@@ -25,15 +38,15 @@
 
 ZADU provides two different interfaces for executing distortion measures.
 You can either use the main class that wraps the measures, or directly access and invoke the functions that define each distortion measure.
 
 ### Using the Main Class
 
 Use the main class of ZADU to compute distortion measures.
-This approach benefits from the scheduling scheme, providing faster performance.
+This approach benefits from the optimization, providing faster performance when executing multiple measures.
 
 
 ```python
 from zadu import zadu
 
 hd, ld = load_datasets()
 spec = [{
@@ -48,21 +61,21 @@
 print("T&C:", scores[0])
 print("S&C:", scores[1])
 
 ```
 
 `hd` represents high-dimensional data, `ld` represents low-dimensional data
 
-## zadu.ZADU Class
+## ZADU Class
 
-The zadu.ZADU class provides the main interface for the Zadu library, allowing users to evaluate and analyze dimensionality reduction (DR) embeddings effectively and reliably.
+The ZADU class provides the main interface for the Zadu library, allowing users to evaluate and analyze dimensionality reduction (DR) embeddings effectively and reliably.
 
 ### Class Constructor
 
-The Zadu.ZADU class constructor has the following signature:
+The ZADU class constructor has the following signature:
 
 ```python
 class ZADU(spec: List[Dict[str, Union[str, dict]]], hd: np.ndarray, return_local: bool = False)
 
 ```
 
 #### Parameters:
@@ -71,14 +84,51 @@
 &nbsp;&nbsp;&nbsp;&nbsp;
 A list of dictionaries that define the distortion measures to execute and their hyperparameters.
 Each dictionary must contain the following keys:
   * `"id"`: The identifier of the distortion measure, such as `"tnc"` or `"snc"`.
 
   * `"params"`: A dictionary containing hyperparameters specific to the chosen distortion measure.
 
+<details>
+<summary style="cursor: pointer; font-weight: bold; color: #0066cc;">List of ID/Parameters for Each Function</summary>
+
+### Local Measures
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Trustworthiness & Continuity | tnc | `k=20` | [0.5, 1] | 1 |
+| Mean Relative Rank Errors | mrre | `k=20` | [0, 1] | 1 | 
+| Local Continuity Meta-Criteria | lcmc | `k=20` | [0, 1] | 1 |
+| Neighborhood hit | nh | `k=20` | [0, 1] | 1 |
+| Neighbor Dissimilarity | nd | `k=20` | R+ | 0 |
+| Class-Aware Trustworthiness & Continuity | ca_tnc | `k=20` | [0.5, 1] | 1|
+| Procrustes Measure | proc | `k=20` | R+ | 0 |
+
+### Cluster-level
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Steadiness & Cohesiveness | snc | `iteration=150, walk_num_ratio=0.3, alpha=0.1, k=50, clustering_strategy="dbscan"` | [0, 1] | 1 |
+| Distance Consistency | dsc | | [0.5, 1] | 0.5 | 
+| Internal Validation Measures | ivm | `measure="silhouette"` | Depends on IVM | Depends on IVM |
+| Clustering + External Clustering Validation Measures | c_evm | `measure="arand", clustering="kmeans", clustering_args=None` | Depends on EVM | Depends on EVM |
+
+### Global
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Stress | stress | | R+ | 0 |
+| Kullback-Leibler Divergence | kl_div | `sigma=0.1` | R+ | 0 |
+| Distance-to-Measure | dtm | `sigma=0.1` | R+ | 0 |
+| Topographic Product | topo | `k=20` | R | 0 |
+| Pearson’s correlation coefficient | pr | | [-1, 1] | 1
+| Spearman’s rank correlation coefficient | srho | | [-1, 1] | 1
+
+
+</details>
 
 ##### `hd`
 &nbsp;&nbsp;&nbsp;&nbsp;
 A high-dimensional dataset (numpy array) to register and reuse during the evaluation process.
 
 
 ##### `return_local`
@@ -89,24 +139,24 @@
 ### Directly Accessing Functions
 
 You can also directly access and invoke the functions defining each distortion measure for greater flexibility.
 
 ```python
 from zadu.measures import *
 
-mrre = mean_relative_rank_error.run(hd, ld, k=20)
-pr  = pearson_r.run(hd, ld)
-nh  = neighborhood_hit.run(ld, label, k=20)
+mrre = mean_relative_rank_error.measure(hd, ld, k=20)
+pr  = pearson_r.measure(hd, ld)
+nh  = neighborhood_hit.measure(ld, label, k=20)
 ```
 
 ## Advanced Features
 
-### Scheduling the Execution
+### Optimizing the Execution
 
-ZADU optimizes the execution of multiple distortion measures through an effective scheduling scheme. It minimizes the computational overhead associated with preprocessing stages such as pairwise distance calculation, pointwise distance ranking determination, and k-nearest neighbor identification.
+ZADU automatically optimizes the execution of multiple distortion measures. It minimizes the computational overhead associated with preprocessing stages such as pairwise distance calculation, pointwise distance ranking determination, and k-nearest neighbor identification.
 
 ### Computing Pointwise Local Distortions
 
 Users can obtain local pointwise distortions by setting the return_local flag. If a specified distortion measure produces local pointwise distortion as intermediate results, it returns a list of pointwise distortions when the flag is raised.
 
 ```python
 from zadu import zadu
@@ -123,27 +173,29 @@
 global_, local_ = zadu_obj.measure(ld)
 print("MRRE local distortions:", local_[1])
 
 ```
 
 ### Visualizing Local Distortions
 
-With the pointwise local distortions obtained from ZADU, users can visualize the distortions using various distortion visualizations. For example, CheckViz and the Reliability Map can be implemented using a Python visualization library with zaduvis.
+With the pointwise local distortions obtained from ZADU, users can visualize the distortions using various distortion visualizations. We provide ZADUVis, a python library that enables the rendering of two disotortion visualizations: [CheckViz](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1467-8659.2010.01835.x) and the [Reliability Map](https://arxiv.org/abs/2107.07859).
+
 
-<img alt="image" src="https://user-images.githubusercontent.com/38465539/235427171-94dcc220-7cbb-4ee6-94b3-20cc96ffbfa8.png">
+![img](https://user-images.githubusercontent.com/38465539/235427171-94dcc220-7cbb-4ee6-94b3-20cc96ffbfa8.png)
 
 ```python
 from zadu import zadu
 from zaduvis import zaduvis
 import matplotlib.pyplot as plt
 from sklearn.manifold import TSNE
 from sklearn.datasets import fetch_openml
 
+
 ## load datasets and generate an embedding
-hd = fetch_openml("mnist_784", version=1, cache=True).target.astype(int)[::7]
+hd = fetch_openml('mnist_784', version=1, cache=True).target.astype(int)[::7]
 ld = TSNE.fit_transform(hd)
 
 ## Computing local pointwise distortions
 specs = [{"id": "snc", "params": {"k": 50}}]
 zadu_obj = zadu.ZADU(spec, hd, return_local=True)
 global_, local_ = zadu_obj.measure(ld)
 l_s = local_[0]["local_steadiness"]
@@ -153,18 +205,18 @@
 fig, ax = plt.subplots(1, 2, figsize=(20, 10))
 zaduvis.checkviz(ld, l_s, l_c, ax=ax[0])
 zaduvis.reliability_map(ld, l_s, l_c, ax=ax[1])
 
 ```
 
 
-The above code snippet demonstrates how to visualize local pointwise distortions using CheckViz and Reliability Map plots. `zaduvis.checkviz` generates a CheckViz plot, which shows local Steadiness (x-axis) vs. local Cohesiveness (y-axis) for each point in the embedding. `zaduvis.reliability_map` creates a Reliability Map plot, which colors each point in the embedding according to its local Steadiness and local Cohesiveness values.
+The above code snippet demonstrates how to visualize local pointwise distortions using CheckViz and Reliability Map plots.
 
 ## Documentation
 
-For more information about the available distortion measures, their use cases, and examples, please refer to our [paper](zadu.pdf).
+For more information about the available distortion measures, their use cases, and examples, please refer to our paper [TBD].
 
-##Citation
+## Citation
 
-##License
+## License
 
-##Contributing
+## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zadu-0.0.8/setup.py` & `zadu-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 print(setuptools.find_packages(where="src"))
 
 setuptools.setup(
 	name="zadu",
-	version="0.0.8",
+	version="0.1.0",
 	author="Hyeon Jeon",
 	author_email="hj@hcil.snu.ac.kr",
 	description="A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/hj-n/zadu",
 	classifiers=[
```

### Comparing `zadu-0.0.8/src/zadu/measures/class_aware_trustworthiness_continuity.py` & `zadu-0.1.0/src/zadu/measures/class_aware_trustworthiness_continuity.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/clustering_and_external_validation_measure.py` & `zadu-0.1.0/src/zadu/measures/clustering_and_external_validation_measure.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/distance_consistency.py` & `zadu-0.1.0/src/zadu/measures/distance_consistency.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def measure(emb, label):
   """
 	Compute distance consistency of the embedding
 	INPUT:
 		ndarray: emb: embedded data
 		ndarray: label: label of the original data
 	OUTPUT:
-		dict: distance consistency (dc)
+		dict: distance consistency (dsc)
   """
   
 	## compute centroids
   point_num = emb.shape[0]
   label_num = np.unique(label).shape[0]
 
   centroids = np.zeros((label_num, emb.shape[1]))
```

### Comparing `zadu-0.0.8/src/zadu/measures/distance_to_measure.py` & `zadu-0.1.0/src/zadu/measures/distance_to_measure.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/internal_validation_measure.py` & `zadu-0.1.0/src/zadu/measures/internal_validation_measure.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/kl_divergence.py` & `zadu-0.1.0/src/zadu/measures/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/local_continuity_meta_criteria.py` & `zadu-0.1.0/src/zadu/measures/local_continuity_meta_criteria.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/mean_relative_rank_error.py` & `zadu-0.1.0/src/zadu/measures/mean_relative_rank_error.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/neighbor_dissimilarity.py` & `zadu-0.1.0/src/zadu/measures/neighbor_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/neighborhood_hit.py` & `zadu-0.1.0/src/zadu/measures/neighborhood_hit.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/pearson_r.py` & `zadu-0.1.0/src/zadu/measures/pearson_r.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/procrustes.py` & `zadu-0.1.0/src/zadu/measures/procrustes.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/spearman_rho.py` & `zadu-0.1.0/src/zadu/measures/spearman_rho.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/steadiness_cohesiveness.py` & `zadu-0.1.0/src/zadu/measures/steadiness_cohesiveness.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/stress.py` & `zadu-0.1.0/src/zadu/measures/stress.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/topographic_product.py` & `zadu-0.1.0/src/zadu/measures/topographic_product.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/trustworthiness_continuity.py` & `zadu-0.1.0/src/zadu/measures/trustworthiness_continuity.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/utils/knn.py` & `zadu-0.1.0/src/zadu/measures/utils/knn.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/measures/utils/pairwise_dist.py` & `zadu-0.1.0/src/zadu/measures/utils/pairwise_dist.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zadu/zadu.py` & `zadu-0.1.0/src/zadu/zadu.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 		"tnc": "trustworthiness_continuity",
 		"mrre": "mean_relative_rank_error",
 		"lcmc": "local_continuity_meta_criteria",
 		"nh": "neighborhood_hit",
 		"ca_tnc": "class_aware_trustworthiness_continuity",
 		"nd": "neighbor_dissimilarity",
 		"dtm": "distance_to_measure",
-		"lcmc": "local_continuity_meta_criteria",
 		"kl_div": "kl_divergence",
 		"dsc": "distance_consistency",
 		"pr": "pearson_r",
 		"srho":	"spearman_rho",
 		"ivm": "internal_validation_measure",
 		"c_evm": "clustering_and_external_validation_measure",
 		"snc": "steadiness_cohesiveness",
```

### Comparing `zadu-0.0.8/src/zadu.egg-info/PKG-INFO` & `zadu-0.1.0/src/zadu.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,222 @@
 Metadata-Version: 2.1
 Name: zadu
-Version: 0.0.8
+Version: 0.1.0
 Summary: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
 Home-page: https://github.com/hj-n/zadu
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
-License: UNKNOWN
-Description: # ZADU: A Python Toolkit for Evaluating the Reliability of Dimensionality Reduction Embeddings
-        
-        ZADU is a Python library that provides a comprehensive suite of distortion measures for evaluating and analyzing dimensionality reduction (DR) embeddings. The library supports a diverse set of local, cluster-level, and global distortion measures, allowing users to assess DR techniques from various structural perspectives. By offering an optimized scheduling scheme and pointwise local distortions, ZADU enables efficient and in-depth analysis of DR embeddings.
-        
-        
-        ## Installation
-        
-        You can install ZADU via `pip`:
-        
-        ```bash
-        pip install zadu
-        ```
-        
-        ## Supported Distortion Measures
-        
-        ZADU currently supports a total of 17 distortion measures, including:
-        
-        - 7 local measures
-        - 4 cluster-level measures
-        - 6 global measures
-        
-        For a complete list of supported measures, refer to [measures](/src/zadu/measures).
-        
-        ## How To Use ZADU
-        
-        ZADU provides two different interfaces for executing distortion measures.
-        You can either use the main class that wraps the measures, or directly access and invoke the functions that define each distortion measure.
-        
-        ### Using the Main Class
-        
-        Use the main class of ZADU to compute distortion measures.
-        This approach benefits from the scheduling scheme, providing faster performance.
-        
-        
-        ```python
-        from zadu import zadu
-        
-        hd, ld = load_datasets()
-        spec = [{
-            "id"    : "tnc",
-            "params": { "k": 20 },
-        }, {
-            "id"    : "snc",
-            "params": { "k": 30, "clustering": "hdbscan" }
-        }]
-        
-        scores = zadu.ZADU(spec, hd).measure(ld)
-        print("T&C:", scores[0])
-        print("S&C:", scores[1])
-        
-        ```
-        
-        `hd` represents high-dimensional data, `ld` represents low-dimensional data
-        
-        ## zadu.ZADU Class
-        
-        The zadu.ZADU class provides the main interface for the Zadu library, allowing users to evaluate and analyze dimensionality reduction (DR) embeddings effectively and reliably.
-        
-        ### Class Constructor
-        
-        The Zadu.ZADU class constructor has the following signature:
-        
-        ```python
-        class ZADU(spec: List[Dict[str, Union[str, dict]]], hd: np.ndarray, return_local: bool = False)
-        
-        ```
-        
-        #### Parameters:
-        
-        ##### `spec` 
-        &nbsp;&nbsp;&nbsp;&nbsp;
-        A list of dictionaries that define the distortion measures to execute and their hyperparameters.
-        Each dictionary must contain the following keys:
-          * `"id"`: The identifier of the distortion measure, such as `"tnc"` or `"snc"`.
-        
-          * `"params"`: A dictionary containing hyperparameters specific to the chosen distortion measure.
-        
-        
-        ##### `hd`
-        &nbsp;&nbsp;&nbsp;&nbsp;
-        A high-dimensional dataset (numpy array) to register and reuse during the evaluation process.
-        
-        
-        ##### `return_local`
-        &nbsp;&nbsp;&nbsp;&nbsp;
-        A boolean flag that, when set to `True`, enables the computation of local pointwise distortions for each data point. The default value is `False`.
-        
-        
-        ### Directly Accessing Functions
-        
-        You can also directly access and invoke the functions defining each distortion measure for greater flexibility.
-        
-        ```python
-        from zadu.measures import *
-        
-        mrre = mean_relative_rank_error.run(hd, ld, k=20)
-        pr  = pearson_r.run(hd, ld)
-        nh  = neighborhood_hit.run(ld, label, k=20)
-        ```
-        
-        ## Advanced Features
-        
-        ### Scheduling the Execution
-        
-        ZADU optimizes the execution of multiple distortion measures through an effective scheduling scheme. It minimizes the computational overhead associated with preprocessing stages such as pairwise distance calculation, pointwise distance ranking determination, and k-nearest neighbor identification.
-        
-        ### Computing Pointwise Local Distortions
-        
-        Users can obtain local pointwise distortions by setting the return_local flag. If a specified distortion measure produces local pointwise distortion as intermediate results, it returns a list of pointwise distortions when the flag is raised.
-        
-        ```python
-        from zadu import zadu
-        
-        spec = [{
-            "id"    : "dtm",
-            "params": {}
-        }, {
-            "id"    : "mrre",
-            "params": { "k": 30 }
-        }]
-        
-        zadu_obj = zadu.ZADU(spec, hd, return_local=True)
-        global_, local_ = zadu_obj.measure(ld)
-        print("MRRE local distortions:", local_[1])
-        
-        ```
-        
-        ### Visualizing Local Distortions
-        
-        With the pointwise local distortions obtained from ZADU, users can visualize the distortions using various distortion visualizations. For example, CheckViz and the Reliability Map can be implemented using a Python visualization library with zaduvis.
-        
-        <img alt="image" src="https://user-images.githubusercontent.com/38465539/235427171-94dcc220-7cbb-4ee6-94b3-20cc96ffbfa8.png">
-        
-        ```python
-        from zadu import zadu
-        from zaduvis import zaduvis
-        import matplotlib.pyplot as plt
-        from sklearn.manifold import TSNE
-        from sklearn.datasets import fetch_openml
-        
-        ## load datasets and generate an embedding
-        hd = fetch_openml("mnist_784", version=1, cache=True).target.astype(int)[::7]
-        ld = TSNE.fit_transform(hd)
-        
-        ## Computing local pointwise distortions
-        specs = [{"id": "snc", "params": {"k": 50}}]
-        zadu_obj = zadu.ZADU(spec, hd, return_local=True)
-        global_, local_ = zadu_obj.measure(ld)
-        l_s = local_[0]["local_steadiness"]
-        l_c = local_[0]["local_cohesiveness"]
-        
-        ## Visualizing local distortions
-        fig, ax = plt.subplots(1, 2, figsize=(20, 10))
-        zaduvis.checkviz(ld, l_s, l_c, ax=ax[0])
-        zaduvis.reliability_map(ld, l_s, l_c, ax=ax[1])
-        
-        ```
-        
-        
-        The above code snippet demonstrates how to visualize local pointwise distortions using CheckViz and Reliability Map plots. `zaduvis.checkviz` generates a CheckViz plot, which shows local Steadiness (x-axis) vs. local Cohesiveness (y-axis) for each point in the embedding. `zaduvis.reliability_map` creates a Reliability Map plot, which colors each point in the embedding according to its local Steadiness and local Cohesiveness values.
-        
-        ## Documentation
-        
-        For more information about the available distortion measures, their use cases, and examples, please refer to our [paper](zadu.pdf).
-        
-        ##Citation
-        
-        ##License
-        
-        ##Contributing
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+
+# ZADU: A Python Library for Evaluating the Reliability of Dimensionality Reduction Embeddings
+
+ZADU is a Python library that provides distortion measures for evaluating and analyzing dimensionality reduction (DR) embeddings. The library supports a diverse set of local, cluster-level, and global distortion measures, allowing users to assess DR techniques from various structural perspectives. By offering an optimized execution and pointwise local distortions, ZADU enables efficient and in-depth analysis of DR embeddings.
+
+
+## Installation
+
+You can install ZADU via `pip`:
+
+```bash
+pip install zadu
+```
+
+## Supported Distortion Measures
+
+ZADU currently supports a total of 17 distortion measures, including:
+
+- 7 local measures
+- 4 cluster-level measures
+- 6 global measures
+
+For a complete list of supported measures, refer to [measures](/src/zadu/measures).
+
+## How To Use ZADU
+
+ZADU provides two different interfaces for executing distortion measures.
+You can either use the main class that wraps the measures, or directly access and invoke the functions that define each distortion measure.
+
+### Using the Main Class
+
+Use the main class of ZADU to compute distortion measures.
+This approach benefits from the optimization, providing faster performance when executing multiple measures.
+
+
+```python
+from zadu import zadu
+
+hd, ld = load_datasets()
+spec = [{
+    "id"    : "tnc",
+    "params": { "k": 20 },
+}, {
+    "id"    : "snc",
+    "params": { "k": 30, "clustering": "hdbscan" }
+}]
+
+scores = zadu.ZADU(spec, hd).measure(ld)
+print("T&C:", scores[0])
+print("S&C:", scores[1])
+
+```
+
+`hd` represents high-dimensional data, `ld` represents low-dimensional data
+
+## ZADU Class
+
+The ZADU class provides the main interface for the Zadu library, allowing users to evaluate and analyze dimensionality reduction (DR) embeddings effectively and reliably.
+
+### Class Constructor
+
+The ZADU class constructor has the following signature:
+
+```python
+class ZADU(spec: List[Dict[str, Union[str, dict]]], hd: np.ndarray, return_local: bool = False)
+
+```
+
+#### Parameters:
+
+##### `spec` 
+&nbsp;&nbsp;&nbsp;&nbsp;
+A list of dictionaries that define the distortion measures to execute and their hyperparameters.
+Each dictionary must contain the following keys:
+  * `"id"`: The identifier of the distortion measure, such as `"tnc"` or `"snc"`.
+
+  * `"params"`: A dictionary containing hyperparameters specific to the chosen distortion measure.
+
+<details>
+<summary style="cursor: pointer; font-weight: bold; color: #0066cc;">List of ID/Parameters for Each Function</summary>
+
+### Local Measures
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Trustworthiness & Continuity | tnc | `k=20` | [0.5, 1] | 1 |
+| Mean Relative Rank Errors | mrre | `k=20` | [0, 1] | 1 | 
+| Local Continuity Meta-Criteria | lcmc | `k=20` | [0, 1] | 1 |
+| Neighborhood hit | nh | `k=20` | [0, 1] | 1 |
+| Neighbor Dissimilarity | nd | `k=20` | R+ | 0 |
+| Class-Aware Trustworthiness & Continuity | ca_tnc | `k=20` | [0.5, 1] | 1|
+| Procrustes Measure | proc | `k=20` | R+ | 0 |
+
+### Cluster-level
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Steadiness & Cohesiveness | snc | `iteration=150, walk_num_ratio=0.3, alpha=0.1, k=50, clustering_strategy="dbscan"` | [0, 1] | 1 |
+| Distance Consistency | dsc | | [0.5, 1] | 0.5 | 
+| Internal Validation Measures | ivm | `measure="silhouette"` | Depends on IVM | Depends on IVM |
+| Clustering + External Clustering Validation Measures | c_evm | `measure="arand", clustering="kmeans", clustering_args=None` | Depends on EVM | Depends on EVM |
+
+### Global
+
+| Measure | ID | Parameters | Range | Optimum |
+|---------|----|------------|-------|---------|
+| Stress | stress | | R+ | 0 |
+| Kullback-Leibler Divergence | kl_div | `sigma=0.1` | R+ | 0 |
+| Distance-to-Measure | dtm | `sigma=0.1` | R+ | 0 |
+| Topographic Product | topo | `k=20` | R | 0 |
+| Pearson’s correlation coefficient | pr | | [-1, 1] | 1
+| Spearman’s rank correlation coefficient | srho | | [-1, 1] | 1
+
+
+</details>
+
+##### `hd`
+&nbsp;&nbsp;&nbsp;&nbsp;
+A high-dimensional dataset (numpy array) to register and reuse during the evaluation process.
+
+
+##### `return_local`
+&nbsp;&nbsp;&nbsp;&nbsp;
+A boolean flag that, when set to `True`, enables the computation of local pointwise distortions for each data point. The default value is `False`.
+
+
+### Directly Accessing Functions
+
+You can also directly access and invoke the functions defining each distortion measure for greater flexibility.
+
+```python
+from zadu.measures import *
+
+mrre = mean_relative_rank_error.measure(hd, ld, k=20)
+pr  = pearson_r.measure(hd, ld)
+nh  = neighborhood_hit.measure(ld, label, k=20)
+```
+
+## Advanced Features
+
+### Optimizing the Execution
+
+ZADU automatically optimizes the execution of multiple distortion measures. It minimizes the computational overhead associated with preprocessing stages such as pairwise distance calculation, pointwise distance ranking determination, and k-nearest neighbor identification.
+
+### Computing Pointwise Local Distortions
+
+Users can obtain local pointwise distortions by setting the return_local flag. If a specified distortion measure produces local pointwise distortion as intermediate results, it returns a list of pointwise distortions when the flag is raised.
+
+```python
+from zadu import zadu
+
+spec = [{
+    "id"    : "dtm",
+    "params": {}
+}, {
+    "id"    : "mrre",
+    "params": { "k": 30 }
+}]
+
+zadu_obj = zadu.ZADU(spec, hd, return_local=True)
+global_, local_ = zadu_obj.measure(ld)
+print("MRRE local distortions:", local_[1])
+
+```
+
+### Visualizing Local Distortions
+
+With the pointwise local distortions obtained from ZADU, users can visualize the distortions using various distortion visualizations. We provide ZADUVis, a python library that enables the rendering of two disotortion visualizations: [CheckViz](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1467-8659.2010.01835.x) and the [Reliability Map](https://arxiv.org/abs/2107.07859).
+
+
+![img](https://user-images.githubusercontent.com/38465539/235427171-94dcc220-7cbb-4ee6-94b3-20cc96ffbfa8.png)
+
+```python
+from zadu import zadu
+from zaduvis import zaduvis
+import matplotlib.pyplot as plt
+from sklearn.manifold import TSNE
+from sklearn.datasets import fetch_openml
+
+
+## load datasets and generate an embedding
+hd = fetch_openml('mnist_784', version=1, cache=True).target.astype(int)[::7]
+ld = TSNE.fit_transform(hd)
+
+## Computing local pointwise distortions
+specs = [{"id": "snc", "params": {"k": 50}}]
+zadu_obj = zadu.ZADU(spec, hd, return_local=True)
+global_, local_ = zadu_obj.measure(ld)
+l_s = local_[0]["local_steadiness"]
+l_c = local_[0]["local_cohesiveness"]
+
+## Visualizing local distortions
+fig, ax = plt.subplots(1, 2, figsize=(20, 10))
+zaduvis.checkviz(ld, l_s, l_c, ax=ax[0])
+zaduvis.reliability_map(ld, l_s, l_c, ax=ax[1])
+
+```
+
+
+The above code snippet demonstrates how to visualize local pointwise distortions using CheckViz and Reliability Map plots.
+
+## Documentation
+
+For more information about the available distortion measures, their use cases, and examples, please refer to our paper [TBD].
+
+## Citation
+
+## License
+
+## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zadu-0.0.8/src/zadu.egg-info/SOURCES.txt` & `zadu-0.1.0/src/zadu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zaduvis/colormap.py` & `zadu-0.1.0/src/zaduvis/colormap.py`

 * *Files identical despite different names*

### Comparing `zadu-0.0.8/src/zaduvis/zaduvis.py` & `zadu-0.1.0/src/zaduvis/zaduvis.py`

 * *Files identical despite different names*

