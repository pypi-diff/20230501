# Comparing `tmp/treecluster-1.0.3.tar.gz` & `tmp/treecluster-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treecluster-1.0.3.tar", last modified: Thu Oct  1 16:38:35 2020, max compression
+gzip compressed data, was "treecluster-1.0.4.tar", last modified: Mon May  1 14:39:20 2023, max compression
```

## Comparing `treecluster-1.0.3.tar` & `treecluster-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-10-01 16:38:35.000000 treecluster-1.0.3/
--rw-rw-rw-   0 niema     (1000) niema     (1000)     3219 2020-10-01 16:38:16.000000 treecluster-1.0.3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 niema     (1000) niema     (1000)    35149 2020-10-01 16:38:16.000000 treecluster-1.0.3/LICENSE
--rw-rw-rw-   0 niema     (1000) niema     (1000)      121 2020-10-01 16:38:16.000000 treecluster-1.0.3/MANIFEST.in
--rw-rw-rw-   0 niema     (1000) niema     (1000)      567 2020-10-01 16:38:35.000000 treecluster-1.0.3/PKG-INFO
--rw-rw-rw-   0 niema     (1000) niema     (1000)     8448 2020-10-01 16:38:16.000000 treecluster-1.0.3/README.md
--rwxrwxrwx   0 niema     (1000) niema     (1000)    25349 2020-10-01 16:38:16.000000 treecluster-1.0.3/TreeCluster.py
--rw-rw-rw-   0 niema     (1000) niema     (1000)        6 2020-10-01 16:38:16.000000 treecluster-1.0.3/VERSION
--rw-rw-rw-   0 niema     (1000) niema     (1000)       38 2020-10-01 16:38:35.000000 treecluster-1.0.3/setup.cfg
--rw-rw-rw-   0 niema     (1000) niema     (1000)     1007 2020-10-01 16:38:26.000000 treecluster-1.0.3/setup.py
-drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/
--rw-rw-rw-   0 niema     (1000) niema     (1000)      567 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/PKG-INFO
--rw-rw-rw-   0 niema     (1000) niema     (1000)      288 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/SOURCES.txt
--rw-rw-rw-   0 niema     (1000) niema     (1000)        1 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/dependency_links.txt
--rw-rw-rw-   0 niema     (1000) niema     (1000)        1 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/not-zip-safe
--rw-rw-rw-   0 niema     (1000) niema     (1000)       18 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/requires.txt
--rw-rw-rw-   0 niema     (1000) niema     (1000)        1 2020-10-01 16:38:35.000000 treecluster-1.0.3/treecluster.egg-info/top_level.txt
+drwxr-xr-x   0 niema     (1000) niema     (1000)        0 2023-05-01 14:39:20.828649 treecluster-1.0.4/
+-rw-r--r--   0 niema     (1000) niema     (1000)     3219 2023-05-01 14:34:43.000000 treecluster-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 niema     (1000) niema     (1000)    35149 2023-05-01 14:34:43.000000 treecluster-1.0.4/LICENSE
+-rw-r--r--   0 niema     (1000) niema     (1000)      121 2023-05-01 14:34:43.000000 treecluster-1.0.4/MANIFEST.in
+-rw-r--r--   0 niema     (1000) niema     (1000)      542 2023-05-01 14:39:20.828649 treecluster-1.0.4/PKG-INFO
+-rw-r--r--   0 niema     (1000) niema     (1000)     8704 2023-05-01 14:34:43.000000 treecluster-1.0.4/README.md
+-rwxr-xr-x   0 niema     (1000) niema     (1000)    25286 2023-05-01 14:38:37.000000 treecluster-1.0.4/TreeCluster.py
+-rw-r--r--   0 niema     (1000) niema     (1000)        6 2023-05-01 14:38:02.000000 treecluster-1.0.4/VERSION
+-rw-r--r--   0 niema     (1000) niema     (1000)       38 2023-05-01 14:39:20.828649 treecluster-1.0.4/setup.cfg
+-rw-r--r--   0 niema     (1000) niema     (1000)     1007 2023-05-01 14:38:13.000000 treecluster-1.0.4/setup.py
+drwxr-xr-x   0 niema     (1000) niema     (1000)        0 2023-05-01 14:39:20.828649 treecluster-1.0.4/treecluster.egg-info/
+-rw-r--r--   0 niema     (1000) niema     (1000)      542 2023-05-01 14:39:20.000000 treecluster-1.0.4/treecluster.egg-info/PKG-INFO
+-rw-r--r--   0 niema     (1000) niema     (1000)      288 2023-05-01 14:39:20.000000 treecluster-1.0.4/treecluster.egg-info/SOURCES.txt
+-rw-r--r--   0 niema     (1000) niema     (1000)        1 2023-05-01 14:39:20.000000 treecluster-1.0.4/treecluster.egg-info/dependency_links.txt
+-rw-r--r--   0 niema     (1000) niema     (1000)        1 2023-05-01 14:39:20.000000 treecluster-1.0.4/treecluster.egg-info/not-zip-safe
+-rw-r--r--   0 niema     (1000) niema     (1000)       18 2023-05-01 14:39:20.000000 treecluster-1.0.4/treecluster.egg-info/requires.txt
+-rw-r--r--   0 niema     (1000) niema     (1000)        1 2023-05-01 14:39:20.000000 treecluster-1.0.4/treecluster.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `treecluster-1.0.3/CODE_OF_CONDUCT.md` & `treecluster-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `treecluster-1.0.3/LICENSE` & `treecluster-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `treecluster-1.0.3/README.md` & `treecluster-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 ```bash
 usage: TreeCluster.py [-h] [-i INPUT] -t THRESHOLD [-s SUPPORT] [-m METHOD] [-tf THRESHOLD_FREE]
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input Tree File (default: stdin)
+  -o OUTPUT, --output OUTPUT
+                        Output File (default: stdout)
   -t THRESHOLD, --threshold THRESHOLD
                         Length Threshold (default: None)
   -s SUPPORT, --support SUPPORT
                         Branch Support Threshold (default: -inf)
   -m METHOD, --method METHOD
-                        Clustering Method (options: avg_clade, length,
-                        length_clade, max, max_clade, med_clade, root_dist,
-                        single_linkage_clade) (default: max_clade)
+                        Clustering Method (options: avg_clade, leaf_dist_avg, leaf_dist_max, leaf_dist_min, length, length_clade, max, max_clade,
+                        med_clade, root_dist, single_linkage, single_linkage_cut, single_linkage_union, sum_branch, sum_branch_clade) (default: max_clade)
   -tf THRESHOLD_FREE, --threshold_free THRESHOLD_FREE
-                        Threshold-Free Approach (options: argmax_clusters)
-                        (default: None)
+                        Threshold-Free Approach (options: argmax_clusters) (default: None)
+  -v, --verbose         Verbose Mode (default: False)
+  --version             Display Version (default: False)
 ```
 
 ## Clustering Methods
 * **Avg Clade:** Cluster the leaves such that the following conditions hold for each cluster:
     1. The average pairwise distance between leaves in the cluster is at most *t*
     2. Leaves cannot be connected by branches with support less than or equal to *s*
     3. The leaves in the cluster must define a clade in *T*
@@ -112,15 +114,15 @@
     2. Leaves cannot be connected by branches with support less than or equal to *s*
     3. The leaves in the cluster must define a clade in *T*
     * For a tree with *n* leaves, this algorithm is O(*n*) in the worst case
     * If verbose mode is enabled (`-v`), the clades defined by the clusters will be printed to standard error
 
 ## Threshold-Free Approaches
 * **Argmax Clusters:** Choose the threshold that maximizes the number of non-singleton clusters over all thresholds from 0 to *t*
-    * Currently, for the sake of speed, only every 0.0001 threshold is tested (i.e., 0, 0.001, 0.002, ..., *t*)
+    * Currently, for the sake of speed, only every 0.001 threshold is tested (i.e., 0, 0.001, 0.002, ..., *t*)
 
 ## Requirements
 * [NiemaDS](https://github.com/niemasd/NiemaDS)
 * [TreeSwift](https://github.com/niemasd/TreeSwift)
 
 ## Citing TreeCluster
 If you use TreeCluster in your work, please cite:
```

### Comparing `treecluster-1.0.3/TreeCluster.py` & `treecluster-1.0.4/TreeCluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 from math import log
 from niemads import DisjointSet
 from queue import PriorityQueue,Queue
 from treeswift import read_tree_newick
 from sys import argv,stderr
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 NUM_THRESH = 1000 # number of thresholds for the threshold-free methods to use
 VERBOSE = False
 
 # check if user is just printing version
 if '--version' in argv:
     print("TreeCluster version %s" % VERSION); exit()
 
@@ -585,28 +585,26 @@
     assert args.threshold_free is None or args.threshold_free in THRESHOLDFREE, "ERROR: Invalid threshold-free approach: %s" % args.threshold_free
     assert args.threshold >= 0, "ERROR: Length threshold must be at least 0"
     assert args.support >= 0 or args.support == float('-inf'), "ERROR: Branch support must be at least 0"
     VERBOSE = args.verbose
     if args.input == 'stdin':
         from sys import stdin; infile = stdin
     elif args.input.lower().endswith('.gz'):
-        from gzip import open as gopen; infile = gopen(args.input)
+        from gzip import open as gopen; infile = gopen(args.input, 'rt')
     else:
         infile = open(args.input)
     if args.output == 'stdout':
         from sys import stdout; outfile = stdout
     else:
         outfile = open(args.output,'w')
-    trees = list()
-    for line in infile:
-        if isinstance(line,bytes):
-            l = line.decode().strip()
-        else:
-            l = line.strip()
-        trees.append(read_tree_newick(l))
+    tmp = read_tree_newick(infile.read().strip())
+    if isinstance(tmp, list):
+        trees = tmp
+    else:
+        trees = [tmp]
 
     # run algorithm
     for t,tree in enumerate(trees):
         if args.threshold_free is None:
             clusters = METHODS[args.method.lower()](tree,args.threshold,args.support)
         else:
             clusters = THRESHOLDFREE[args.threshold_free](METHODS[args.method.lower()],tree,args.threshold,args.support)
```

### Comparing `treecluster-1.0.3/setup.py` & `treecluster-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
         name='treecluster',    # This is the name of your PyPI-package.
-        version='1.0.3',    # Update the version number for new releases
+        version='1.0.4',    # Update the version number for new releases
         scripts=['TreeCluster.py',], # The name of your script, and also the command you'll be using for calling it
         description='TreeCluster: a tool for clustering biological sequences using phylogenetic trees.',
         long_description='TreeCluster is a tool that, given a tree T (Newick format) and a distance threshold t, \
          finds the minimum number of clusters of the leaves of T such that some user-specified constraint is met \
          in each cluster. ',
         long_description_content_type='text/plain',
         url='https://github.com/niemasd/TreeCluster',
```

