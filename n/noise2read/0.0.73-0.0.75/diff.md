# Comparing `tmp/noise2read-0.0.73.tar.gz` & `tmp/noise2read-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.73.tar", last modified: Thu Apr 20 02:54:47 2023, max compression
+gzip compressed data, was "noise2read-0.0.75.tar", last modified: Mon May  1 13:43:48 2023, max compression
```

## Comparing `noise2read-0.0.73.tar` & `noise2read-0.0.75.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.503448 noise2read-0.0.73/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2022-08-24 03:12:13.000000 noise2read-0.0.73/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     1192 2023-04-20 02:54:47.504825 noise2read-0.0.73/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      773 2023-04-20 02:54:36.000000 noise2read-0.0.73/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2022-12-28 02:32:35.000000 noise2read-0.0.73/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      950 2023-04-20 02:54:47.507504 noise2read-0.0.73/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.369931 noise2read-0.0.73/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.452598 noise2read-0.0.73/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-04-06 02:41:39.000000 noise2read-0.0.73/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    12784 2023-04-07 12:32:06.000000 noise2read-0.0.73/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16050 2023-02-16 00:10:21.000000 noise2read-0.0.73/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-02-16 00:10:34.000000 noise2read-0.0.73/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-11 07:09:30.000000 noise2read-0.0.73/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    45177 2023-04-07 11:41:15.000000 noise2read-0.0.73/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11181 2023-02-16 00:11:05.000000 noise2read-0.0.73/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    29580 2023-02-16 00:11:17.000000 noise2read-0.0.73/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-07 06:44:23.000000 noise2read-0.0.73/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-02-16 00:11:32.000000 noise2read-0.0.73/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26130 2023-04-05 07:34:22.000000 noise2read-0.0.73/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    34369 2023-04-07 06:47:06.000000 noise2read-0.0.73/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    12273 2023-02-16 00:11:52.000000 noise2read-0.0.73/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-02-16 00:12:17.000000 noise2read-0.0.73/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-07 07:22:18.000000 noise2read-0.0.73/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.483018 noise2read-0.0.73/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     1192 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      851 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-02-16 00:19:13.000000 noise2read-0.0.73/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      202 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-04-20 02:54:47.000000 noise2read-0.0.73/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-04-20 02:54:47.499028 noise2read-0.0.73/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)        0 2022-08-24 03:12:14.000000 noise2read-0.0.73/tests/test.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-02-16 00:04:36.000000 noise2read-0.0.73/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-02-16 00:05:10.000000 noise2read-0.0.73/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-02-16 00:05:25.000000 noise2read-0.0.73/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-01 13:43:48.084283 noise2read-0.0.75/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.75/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     1627 2023-05-01 13:43:48.088562 noise2read-0.0.75/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     1208 2023-05-01 13:35:09.000000 noise2read-0.0.75/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.75/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)     1000 2023-05-01 13:43:48.097016 noise2read-0.0.75/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-01 13:43:47.704235 noise2read-0.0.75/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-01 13:43:47.925626 noise2read-0.0.75/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-04-23 01:19:38.000000 noise2read-0.0.75/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    12784 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16050 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    45141 2023-04-23 06:01:09.000000 noise2read-0.0.75/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11181 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    29580 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30699 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26366 2023-04-25 08:21:29.000000 noise2read-0.0.75/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    34369 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    12273 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.75/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-01 13:43:48.038058 noise2read-0.0.75/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1627 2023-05-01 13:43:47.000000 noise2read-0.0.75/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-01 13:43:47.000000 noise2read-0.0.75/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-01 13:43:47.000000 noise2read-0.0.75/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-01 13:43:47.000000 noise2read-0.0.75/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.75/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      218 2023-05-01 13:43:47.000000 noise2read-0.0.75/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-01 13:43:47.000000 noise2read-0.0.75/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-01 13:43:48.071005 noise2read-0.0.75/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.75/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.75/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.75/tests/test_utils.py
```

### Comparing `noise2read-0.0.73/LICENSE` & `noise2read-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/setup.cfg` & `noise2read-0.0.75/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = noise2read
+project-logo = ./logo/logo.svg
 version = attr: noise2read.__version__
 author = Penagyao Ping
 author_email = ping.pengyao@gmail.com
 description = Turn noise to read
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/Jappy0/noise2read
@@ -28,14 +29,15 @@
 	networkx == 2.8.5
 	pandas == 1.4.3
 	optuna == 2.10.1
 	matplotlib == 3.5.2
 	mpire >= 2.5.0
 	editdistance == 0.6.0
 	imbalanced-learn == 0.9.1
+	seaborn >= 0.12.1
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	noise2read = noise2read.noise2read:main
```

### Comparing `noise2read-0.0.73/src/noise2read/classifier.py` & `noise2read-0.0.75/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/config.py` & `noise2read-0.0.75/src/noise2read/config.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/coverage.py` & `noise2read-0.0.75/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/data_analysis.py` & `noise2read-0.0.75/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/data_generation.py` & `noise2read-0.0.75/src/noise2read/data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-04-07 21:41:15
+# @Last Modified time: 2023-04-23 16:01:09
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -272,15 +272,15 @@
         idx = 0
         self.logger.info("Extracting genuine and ambiguous errors...")
         with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
             for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num), progress_bar=self.config.verbose):
                 if genu_ambi_lst[0]:
                     genuine_lst.extend(genu_ambi_lst[0])
                     ambiguous_lst.extend(genu_ambi_lst[1])
-        self.logger.info("Extraction done.")                    
+        self.logger.info("Done!")                    
         # with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
         #     with tqdm(total=subgraph_num, desc=self.logger.info("Extract samples with genuine errors"), miniters=int(subgraph_num/self.config.min_iters)) as pbar:   
         #         for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num)):
         #             if genu_ambi_lst[0]:
         #                 genuine_lst.extend(genu_ambi_lst[0])
         #                 ambiguous_lst.extend(genu_ambi_lst[1])
         #             pbar.update()
@@ -470,30 +470,30 @@
             k_count = graph.nodes[k]['count']
             if k_count >= self.config.high_freq_thre:
                 k_degree = graph.degree[k]
                 line = [k, k_count, k_degree]
                 negative_df.loc[len(negative_df)] = line  
         if self.config.verbose:
             negative_df.to_csv(negative_csv, index=False) 
-        self.logger.info("Extraction done!")
+        self.logger.info("Done!")
         return negative_df
 
     def extract_isolates(self, graph, unique_seqs, seqs2id_dict):
         """
         split the source file into two files of isolates and non-isolates based on constructed graph
 
         Args:
             graph (object): A graph constructed using NetworkX.
             unique_seqs (list): All the unique reads in the dataset
             seqs2id_dict (dict): key: read, id: sequencing id
 
         Returns:
             files: two files of isolates and non-isolates based on constructed graph
         """
-        self.logger.info("Extracting isolated nodes.")
+        self.logger.info("Extracting isolated nodes...")
         if not nx.is_connected(graph):
             self.logger.debug("G is a connected graph: {}".format(nx.is_connected(graph)))
             isolates = set(list(nx.isolates(graph)))
         else:
             self.logger.debug("G is a connected graph: {}".format(nx.is_connected(graph)) )
 
         self.logger.debug("Isolated Nodes Number: {}".format(len(isolates)))
@@ -520,15 +520,15 @@
         elif self.file_type == 'fasta' or self.file_type == 'fa' or self.file_type == 'fasta.gz' or self.file_type == 'fas.gz':
             isolates_file = self.config.result_dir + base[0] + '_isolates.fasta'
             non_isolates_file = self.config.result_dir + base[0] + '_non_isolates.fasta' 
 
         extract_records(self.config.result_dir, name_lst, self.config.input_file, isolates_file)
         extract_records(self.config.result_dir, non_name_lst, self.config.input_file, non_isolates_file)
 
-        self.logger.info("Extraction done.")
+        self.logger.info("Done!")
         return isolates_file, non_isolates_file
 
     def generate_graph(self, data_set, edit_dis):
         """
         construct 1nt- or 2nt-edit-distance-based read graph
 
         Args:
@@ -556,15 +556,15 @@
         unique_seqs = set(total_seqs)
 
         graph = nx.Graph()
         read_count = Counter(total_seqs)
         high_freq = []
         low_freq = []
 
-        for read, frequency in tqdm(read_count.items(), desc=self.logger.info("Adding nodes to " + str(edit_dis) + "-edit-distance read graph..."), miniters=int(len(read_count)/self.config.min_iters)):
+        for read, frequency in tqdm(read_count.items(), desc=self.logger.info("Adding nodes to " + str(edit_dis) + "nt-edit-distance read graph..."), miniters=int(len(read_count)/self.config.min_iters)):
             if not graph.has_node(read):
                 graph.add_node(read, count = frequency, flag=False)  
             if frequency >= self.config.high_freq_thre:
                 high_freq.append(read)
             else:
                 low_freq.append(read)
         if len(high_freq) == 0:
@@ -575,15 +575,15 @@
         ######################################################
         edges_lst = []
         if edit_dis == 1:
             shared_unique_seqs = unique_seqs
         elif edit_dis == 2:
             shared_unique_seqs = low_freq
         
-        self.logger.info("Searching edges for constructing " + str(edit_dis) + "-edit-distance read graph...")
+        self.logger.info("Searching edges for constructing " + str(edit_dis) + "nt-edit-distance read graph...")
         with WorkerPool(self.config.num_workers, shared_objects=shared_unique_seqs, start_method='fork') as pool:
             if edit_dis == 1:
                 for edge_lst in pool.imap(self.real_ed1_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
             elif edit_dis == 2:
                 for edge_lst in pool.imap(self.real_ed2_seqs, high_freq, progress_bar=self.config.verbose):
                     edges_lst.extend(edge_lst)
@@ -598,15 +598,15 @@
         #             for edge_lst in pool.imap(self.real_ed2_seqs, high_freq):
         #                 edges_lst.extend(edge_lst)
         #                 pbar.update()
         if len(edges_lst) > 0:
             self.logger.debug(len(edges_lst))
             self.logger.debug(edges_lst[0])
             graph.add_edges_from(edges_lst)
-        self.logger.info(str(edit_dis) + "-edit-distance read graph construction finished.")
+        self.logger.info(str(edit_dis) + "nt-edit-distance read graph construction finished.")
         ########################################################
         # save graphs
         if self.config.graph_visualization or self.config.save_graph:
             if edit_dis == 1:
                 subdir = self.config.result_dir + "graph1/"                
             elif edit_dis == 2:
                 subdir = self.config.result_dir + "graph2/"
@@ -792,15 +792,15 @@
                         new_b2a.insert(0, idx)
                         high_ambiguous_df.loc[len(high_ambiguous_df)] = new_b2a
                         idx += 1
             del edges_lst
         if self.config.verbose:
             high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
             high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
-        self.logger.info("Extraction done!")
+        self.logger.info("Done!")
         return high_ambiguous_df
 
 '''
     def extract_genuine_ambi_errs(self, subgraphs, edit_dis):
         """
         extract genuine and ambiguous errors from read graph
```

### Comparing `noise2read-0.0.73/src/noise2read/data_preprocessing.py` & `noise2read-0.0.75/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/encoding.py` & `noise2read-0.0.75/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/error_orrection.py` & `noise2read-0.0.75/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/isolates_correction.py` & `noise2read-0.0.75/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/noise2read.py` & `noise2read-0.0.75/src/noise2read/noise2read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2022-12-29 23:04:12
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-04-05 17:34:22
+# @Last Modified time: 2023-04-25 18:21:29
 
 from noise2read.config import Config
 import sys, getopt
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 from noise2read.data_analysis import DataAnalysis
 import os
 from noise2read.simulation import Simulation
 from noise2read.utils import custom_logger, usage
 from noise2read.data_preprocessing import DataProcessing
-from contextlib import redirect_stdout
+# from contextlib import redirect_stdout
+import noise2read
 
 def main():
     argv = sys.argv[1:]
     # create logger
     logger = custom_logger("noise2read", debug_mode=False)
 
     ##############################################################
     try:
         # opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:o:l:h:", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "over_sampling", "libray_layout", "help"]) 
-        opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:l:h", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "libray_layout", "help"]) 
+        opts, args = getopt.getopt(argv, "m:c:i:u:t:r:d:p:a:g:l:hv", ["module=", "config=", "input=", "umi_file", "true", "rectification", "directory", "parallel", "high_ambiguous", "tree_method", "libray_layout", "help", "version"]) 
         script_name = sys.argv[0]
         input_commands = [script_name]
 
         for opt, arg in opts:
             input_commands.append(opt)
             if arg:
                 input_commands.append(arg)
@@ -38,17 +39,21 @@
         
         if opts:
             opts_dict = dict(opts)
             opts_keys = list(opts_dict.keys())
             tar_set = set(opts_keys)
 
             h_lst = list({'-h', '--help'}.intersection(tar_set))
+            v_lst = list({'-v', '--version'}.intersection(tar_set))
             if h_lst:
                 usage()           
-                sys.exit()  
+                sys.exit() 
+            elif v_lst: 
+                print("Version: " + noise2read.__version__)
+                sys.exit()
             else: 
                 m_lst = list({"-m", "--module"}.intersection(tar_set))
                 c_lst = list({"-c", "--config"}.intersection(tar_set)) 
                 i_lst = list({"-i", "--input"}.intersection(tar_set)) 
                 u_lst = list({"-u", "--umi_file"}.intersection(tar_set)) 
                 t_lst = list({"-t", "--true"}.intersection(tar_set)) 
                 r_lst = list({"-r", "--rectification"}.intersection(tar_set))   
@@ -103,30 +108,31 @@
                             logger.exception('Ground truth data does not exsit.')
                             raise
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
                     if p_lst:
                         config.num_workers = int(opts_dict[p_lst[0]])      
                     if a_lst:
-                        config.high_ambiguous = opts_dict[a_lst[0]]
+                        config.high_ambiguous = eval(opts_dict[a_lst[0]])
+                        # print(config.high_ambiguous)
                     if g_lst:
                         config.tree_method = opts_dict[g_lst[0]]
                     # if o_lst:
                     #     if opts_dict[o_lst[0]] == 'False' or 'false':
                     #         config.over_sampling = False
                     #     elif opts_dict[o_lst[0]] == 'True' or 'true':
                     #         config.over_sampling = True
                     #     else:
                     #         logger.exception("Wrongly set over_sampling")
                     #         raise
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     ##############################################################
                     DG = DataGneration(logger, config)
                     if config.high_ambiguous:
                         isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df, high_ambiguous_df = DG.data_files(edit_dis=1)
                     else:
                         isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df = DG.data_files(edit_dis=1)      
                     config.read_max_len = read_max_len
@@ -188,33 +194,33 @@
                             logger.exception('Ground truth data does not exsit.')
                             raise
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
                     if p_lst:
                         config.num_workers = int(opts_dict[p_lst[0]])    
                     if a_lst:
-                        config.high_ambiguous = opts_dict[a_lst[0]] 
+                        config.high_ambiguous = eval(opts_dict[a_lst[0]])
                     if g_lst:
                         config.tree_method = opts_dict[g_lst[0]] 
                     # if o_lst:
                     #     if opts_dict[o_lst[0]] == 'False' or 'false':
                     #         config.over_sampling = False
                     #     elif opts_dict[o_lst[0]] == 'True' or 'true':
                     #         config.over_sampling = True
                     #     else:
                     #         logger.exception("Wrongly set over_sampling")
                     #         raise
                     if not os.path.exists(config.input_file):
                         logger.exception('Input file does not exsit.')
                         raise
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     ##############################################################
                     DG = DataGneration(logger, config)
                     if config.high_ambiguous:
                         isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df, high_ambiguous_df = DG.data_files(edit_dis=1)
                     else:
                         isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df = DG.data_files(edit_dis=1)      
                     config.read_max_len = read_max_len
@@ -268,22 +274,22 @@
                         if not os.path.exists(config.ground_truth_data):
                             logger.exception('Ground truth data does not exsit.')
                             raise
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
                     if p_lst:
                         config.num_workers = int(opts_dict[p_lst[0]])  
-                    if a_lst:
-                        config.high_ambiguous = opts_dict[a_lst[0]] 
+                    # if a_lst:
+                    #     config.high_ambiguous = eval(opts_dict[a_lst[0]])
 
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     ##############################################################
                     config.high_ambiguous=False
                     DG = DataGneration(logger, config)
                     genuine_df = DG.extract_umi_genuine_errs()
                     # ##############################################################
                     EC = ErrorCorrection(logger, config)
                     config.correct_data = EC.umi_correction(config.input_file, genuine_df)
@@ -304,18 +310,18 @@
                         logger.error("Must input raw and true datasets simultaneously or set them in the configuration file.")
                         sys.exit()
 
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
 
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                 #############################################################
                     DP = DataProcessing( 
                         logger,
                         config.num_workers,
                         config.result_dir,
                         config.umi_start,
                         config.umi_end,
@@ -334,18 +340,18 @@
                         sys.exit()
 
                     if u_lst:
                         config.umi_file = opts_dict[u_lst[0]] 
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     DP = DataProcessing( 
                         logger,
                         config.num_workers,
                         config.result_dir,
                         config.umi_start,
                         config.umi_end,
                         config.non_umi_start)
@@ -382,18 +388,18 @@
                         if d_lst:
                             config.result_dir = opts_dict[d_lst[0]]
                     else:
                         logger.error("Must input raw, true and rectified datasets or raw and rectified datasets simultaneously or set them in the configuration file.")
                         sys.exit()
 
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                 #############################################################
                     DataAnalysis(logger, config).evaluation()
 ############################################################################################################################
                 elif module_arg == "simulation":  
                     if c_lst:
                         config = Config(opts_dict[c_lst[0]], logger) 
                         if i_lst:
@@ -410,30 +416,30 @@
                     else:
                         logger.error('Must input configuration file or sequencing dataset.')
                         sys.exit()
 
                     if d_lst:
                         config.result_dir = opts_dict[d_lst[0]] 
                     if a_lst:
-                        config.high_ambiguous = opts_dict[a_lst[0]]
+                        config.high_ambiguous = eval(opts_dict[a_lst[0]])
                     if g_lst:
                         config.tree_method = opts_dict[g_lst[0]]
                     # if o_lst:
                     #     if opts_dict[o_lst[0]] == 'False' or 'false':
                     #         config.over_sampling = False
                     #     elif opts_dict[o_lst[0]] == 'True' or 'true':
                     #         config.over_sampling = True
                     #     else:
                     #         logger.exception("Wrongly set over_sampling")
                     #         raise
                     if config.num_workers <= 0:
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
-                        config.num_workers = available_cpu_cores - 2
+                        config.num_workers = available_cpu_cores
                     Simulation(logger, config).simulation()
 ############################################################################################################################
                 # elif module_arg == "extract_isolates": 
 
                 else:
                     # logger.error("Invalid module name, please check.")
                     logger.error("Input wrong module name, using command noise2read -h/--help for usage.")
```

### Comparing `noise2read-0.0.73/src/noise2read/reads2vectors.py` & `noise2read-0.0.75/src/noise2read/reads2vectors.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/simulation.py` & `noise2read-0.0.75/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/umitest.py` & `noise2read-0.0.75/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read/utils.py` & `noise2read-0.0.75/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.75/src/noise2read.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,11 +20,10 @@
 src/noise2read.egg-info/PKG-INFO
 src/noise2read.egg-info/SOURCES.txt
 src/noise2read.egg-info/dependency_links.txt
 src/noise2read.egg-info/entry_points.txt
 src/noise2read.egg-info/not-zip-safe
 src/noise2read.egg-info/requires.txt
 src/noise2read.egg-info/top_level.txt
-tests/test.py
 tests/test_data_generation.py
 tests/test_reads2vector.py
 tests/test_utils.py
```

### Comparing `noise2read-0.0.73/tests/test_data_generation.py` & `noise2read-0.0.75/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/tests/test_reads2vector.py` & `noise2read-0.0.75/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.73/tests/test_utils.py` & `noise2read-0.0.75/tests/test_utils.py`

 * *Files identical despite different names*

