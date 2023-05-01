# Comparing `tmp/anonlink-0.8.1.tar.gz` & `tmp/anonlink-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anonlink-0.8.1.tar", last modified: Fri May 18 04:07:58 2018, max compression
+gzip compressed data, was "dist/anonlink-0.9.0.tar", last modified: Tue Aug 14 03:37:48 2018, max compression
```

## Comparing `anonlink-0.8.1.tar` & `anonlink-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,37 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-05-18 04:07:58.000000 anonlink-0.8.1/
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-05-18 04:07:58.000000 anonlink-0.8.1/anonlink/
--rwxrwxrwx   0 root         (0) root         (0)     6282 2018-05-18 03:35:15.000000 anonlink-0.8.1/anonlink/benchmark.py
--rwxrwxrwx   0 root         (0) root         (0)     2267 2018-05-18 03:35:15.000000 anonlink-0.8.1/anonlink/bloommatcher.py
--rwxrwxrwx   0 root         (0) root         (0)     1290 2018-05-18 03:35:15.000000 anonlink-0.8.1/anonlink/distributed_processing.py
--rwxrwxrwx   0 root         (0) root         (0)     6190 2018-05-18 03:35:15.000000 anonlink-0.8.1/anonlink/entitymatch.py
--rwxrwxrwx   0 root         (0) root         (0)     5366 2018-05-18 03:35:15.000000 anonlink-0.8.1/anonlink/network_flow.py
--rwxrwxrwx   0 root         (0) root         (0)     1719 2018-05-18 03:35:15.000000 anonlink-0.8.1/anonlink/util.py
--rwxrwxrwx   0 root         (0) root         (0)      217 2018-04-17 01:56:09.000000 anonlink-0.8.1/anonlink/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-05-18 04:07:58.000000 anonlink-0.8.1/anonlink.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2018-05-18 04:07:57.000000 anonlink-0.8.1/anonlink.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2018-04-17 03:10:00.000000 anonlink-0.8.1/anonlink.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)      934 2018-05-18 04:07:57.000000 anonlink-0.8.1/anonlink.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       55 2018-05-18 04:07:57.000000 anonlink-0.8.1/anonlink.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      467 2018-05-18 04:07:57.000000 anonlink-0.8.1/anonlink.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)       24 2018-05-18 04:07:57.000000 anonlink-0.8.1/anonlink.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      145 2018-04-17 01:56:09.000000 anonlink-0.8.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      934 2018-05-18 04:07:58.000000 anonlink-0.8.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6828 2018-04-17 01:56:09.000000 anonlink-0.8.1/README.rst
--rwxrwxrwx   0 root         (0) root         (0)       67 2018-05-18 04:07:58.000000 anonlink-0.8.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1472 2018-05-18 04:07:45.000000 anonlink-0.8.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-05-18 04:07:58.000000 anonlink-0.8.1/_cffi_build/
--rwxrwxrwx   0 root         (0) root         (0)      901 2018-04-17 01:56:09.000000 anonlink-0.8.1/_cffi_build/build_matcher.py
--rwxrwxrwx   0 root         (0) root         (0)    16844 2018-04-18 00:28:56.000000 anonlink-0.8.1/_cffi_build/dice_one_against_many.cpp
+drwxr-xr-x   0 jakub      (502) staff       (20)        0 2018-08-14 03:37:48.000000 anonlink-0.9.0/
+-rw-r--r--   0 jakub      (502) staff       (20)      884 2018-08-14 03:37:48.000000 anonlink-0.9.0/PKG-INFO
+drwxr-xr-x   0 jakub      (502) staff       (20)        0 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink/
+drwxr-xr-x   0 jakub      (502) staff       (20)        0 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink/similarities/
+-rw-r--r--   0 jakub      (502) staff       (20)     4376 2018-08-10 03:46:33.000000 anonlink-0.9.0/anonlink/similarities/_dice_x86.py
+-rw-r--r--   0 jakub      (502) staff       (20)      855 2018-08-02 00:32:20.000000 anonlink-0.9.0/anonlink/similarities/__init__.py
+-rw-r--r--   0 jakub      (502) staff       (20)     3846 2018-08-02 00:32:20.000000 anonlink-0.9.0/anonlink/similarities/_hamming.py
+-rw-r--r--   0 jakub      (502) staff       (20)     2797 2018-08-10 03:46:33.000000 anonlink-0.9.0/anonlink/similarities/_dice_python.py
+-rw-r--r--   0 jakub      (502) staff       (20)      787 2018-08-10 03:46:33.000000 anonlink-0.9.0/anonlink/similarities/_utils.py
+-rw-r--r--   0 jakub      (502) staff       (20)     4586 2018-08-02 00:32:20.000000 anonlink-0.9.0/anonlink/candidate_generation.py
+-rw-r--r--   0 jakub      (502) staff       (20)     6219 2018-08-14 00:19:10.000000 anonlink-0.9.0/anonlink/solving.py
+-rw-r--r--   0 jakub      (502) staff       (20)     6213 2018-08-08 06:09:34.000000 anonlink-0.9.0/anonlink/benchmark.py
+-rw-r--r--   0 jakub      (502) staff       (20)     1719 2018-08-05 04:45:15.000000 anonlink-0.9.0/anonlink/util.py
+-rw-r--r--   0 jakub      (502) staff       (20)     7108 2018-08-14 00:15:35.000000 anonlink-0.9.0/anonlink/concurrency.py
+-rw-r--r--   0 jakub      (502) staff       (20)     2267 2018-07-23 04:06:34.000000 anonlink-0.9.0/anonlink/bloommatcher.py
+-rw-r--r--   0 jakub      (502) staff       (20)     5366 2018-07-23 04:06:34.000000 anonlink-0.9.0/anonlink/network_flow.py
+-rw-r--r--   0 jakub      (502) staff       (20)      420 2018-08-02 00:32:20.000000 anonlink-0.9.0/anonlink/__init__.py
+-rw-r--r--   0 jakub      (502) staff       (20)     1290 2018-07-23 04:06:34.000000 anonlink-0.9.0/anonlink/distributed_processing.py
+-rw-r--r--   0 jakub      (502) staff       (20)     7958 2018-08-02 00:32:20.000000 anonlink-0.9.0/anonlink/blocking.py
+-rw-r--r--   0 jakub      (502) staff       (20)     1201 2018-08-14 00:15:35.000000 anonlink-0.9.0/anonlink/typechecking.py
+-rw-r--r--   0 jakub      (502) staff       (20)     9101 2018-08-02 00:32:20.000000 anonlink-0.9.0/anonlink/serialization.py
+-rw-r--r--   0 jakub      (502) staff       (20)     6178 2018-07-24 00:25:05.000000 anonlink-0.9.0/anonlink/entitymatch.py
+-rw-r--r--   0 jakub      (502) staff       (20)      145 2018-05-01 03:48:40.000000 anonlink-0.9.0/MANIFEST.in
+drwxr-xr-x   0 jakub      (502) staff       (20)        0 2018-08-14 03:37:48.000000 anonlink-0.9.0/_cffi_build/
+-rw-r--r--   0 jakub      (502) staff       (20)     6148 2018-05-01 05:42:38.000000 anonlink-0.9.0/_cffi_build/.DS_Store
+-rw-r--r--   0 jakub      (502) staff       (20)      901 2018-05-01 03:48:40.000000 anonlink-0.9.0/_cffi_build/build_matcher.py
+-rw-r--r--   0 jakub      (502) staff       (20)    17119 2018-08-03 04:54:40.000000 anonlink-0.9.0/_cffi_build/dice_one_against_many.cpp
+-rw-r--r--   0 jakub      (502) staff       (20)     1468 2018-08-14 00:36:00.000000 anonlink-0.9.0/setup.py
+drwxr-xr-x   0 jakub      (502) staff       (20)        0 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink.egg-info/
+-rw-r--r--   0 jakub      (502) staff       (20)      884 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink.egg-info/PKG-INFO
+-rw-r--r--   0 jakub      (502) staff       (20)        1 2018-07-20 01:46:10.000000 anonlink-0.9.0/anonlink.egg-info/not-zip-safe
+-rw-r--r--   0 jakub      (502) staff       (20)      811 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink.egg-info/SOURCES.txt
+-rw-r--r--   0 jakub      (502) staff       (20)       92 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink.egg-info/requires.txt
+-rw-r--r--   0 jakub      (502) staff       (20)       24 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink.egg-info/top_level.txt
+-rw-r--r--   0 jakub      (502) staff       (20)        1 2018-08-14 03:37:48.000000 anonlink-0.9.0/anonlink.egg-info/dependency_links.txt
+-rw-r--r--   0 jakub      (502) staff       (20)       67 2018-08-14 03:37:48.000000 anonlink-0.9.0/setup.cfg
+-rw-r--r--   0 jakub      (502) staff       (20)     6828 2018-05-01 03:48:40.000000 anonlink-0.9.0/README.rst
```

### Comparing `anonlink-0.8.1/anonlink/benchmark.py` & `anonlink-0.9.0/anonlink/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import random
 from timeit import default_timer as timer
 
 from clkhash.key_derivation import generate_key_lists
-from clkhash.schema import get_schema_types
-from clkhash.bloomfilter import calculate_bloom_filters
+from clkhash.bloomfilter import stream_bloom_filters
 from clkhash.randomnames import NameList
 
 from anonlink.entitymatch import *
 from anonlink.util import popcount_vector, generate_clks, generate_bitarray
 
 
 some_filters = generate_clks(10000)
@@ -116,17 +115,17 @@
     :return: dict with 'c' and 'python' keys with values of the total time taken
              for each implementation
     """
 
     nml = NameList(ntotal)
     sl1, sl2 = nml.generate_subsets(nsubset, frac)
 
-    keys = generate_key_lists(('test1', 'test2'), len(nml.schema))
-    filters1 = calculate_bloom_filters(sl1, get_schema_types(nml.schema), keys)
-    filters2 = calculate_bloom_filters(sl2, get_schema_types(nml.schema), keys)
+    keys = generate_key_lists(('test1', 'test2'), len(nml.schema_types))
+    filters1 = tuple(stream_bloom_filters(sl1, keys, nml.SCHEMA))
+    filters2 = tuple(stream_bloom_filters(sl2, keys, nml.SCHEMA))
 
     # Pure Python version
     start = timer()
     result = python_filter_similarity(filters1, filters2, 1, 0.0)
     end = timer()
     python_time = end - start
```

### Comparing `anonlink-0.8.1/anonlink/bloommatcher.py` & `anonlink-0.9.0/anonlink/bloommatcher.py`

 * *Files identical despite different names*

### Comparing `anonlink-0.8.1/anonlink/distributed_processing.py` & `anonlink-0.9.0/anonlink/distributed_processing.py`

 * *Files identical despite different names*

### Comparing `anonlink-0.8.1/anonlink/entitymatch.py` & `anonlink-0.9.0/anonlink/entitymatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     result = []
     for i, f1 in enumerate(filters1):
         def dicecoeff(x):
             return bm.dicecoeff_precount(f1[0], x[0], float(f1[2] + x[2]))
 
         coeffs = filter(lambda c: c[1] >= threshold,
                         enumerate(map(dicecoeff, filters2)))
-        top_k = sorted(coeffs, key=itemgetter(1), reverse=True)[:k]
+        top_k = sorted(coeffs, key=lambda x: -x[1])[:k]
         result.extend([(i, coeff, j) for j, coeff in top_k])
     return result
 
 
 def cffi_filter_similarity_k(filters1, filters2, k, threshold):
     """Accelerated method for determining Bloom Filter similarity.
```

### Comparing `anonlink-0.8.1/anonlink/network_flow.py` & `anonlink-0.9.0/anonlink/network_flow.py`

 * *Files identical despite different names*

### Comparing `anonlink-0.8.1/anonlink/util.py` & `anonlink-0.9.0/anonlink/util.py`

 * *Files identical despite different names*

### Comparing `anonlink-0.8.1/anonlink.egg-info/PKG-INFO` & `anonlink-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 1.1
 Name: anonlink
-Version: 0.8.1
+Version: 0.9.0
 Summary: Anonymous linkage using cryptographic hashes and bloom filters
 Home-page: https://github.com/n1analytics/anonlink
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
```

### Comparing `anonlink-0.8.1/PKG-INFO` & `anonlink-0.9.0/anonlink.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 1.1
 Name: anonlink
-Version: 0.8.1
+Version: 0.9.0
 Summary: Anonymous linkage using cryptographic hashes and bloom filters
 Home-page: https://github.com/n1analytics/anonlink
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
```

### Comparing `anonlink-0.8.1/README.rst` & `anonlink-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `anonlink-0.8.1/setup.py` & `anonlink-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 requirements = [
-        "bitarray==0.8.1",
-        "networkx==1.11",
+        "bitarray>=0.8.1",
+        "networkx>=1.11,<=2",
         "cffi>=1.7",
-        "clkhash>=0.10"
+        "clkhash>=0.11",
+        "numpy>=1.14",
+        "mypy-extensions>=0.3"
     ]
 
 setup(
     name="anonlink",
-    version='0.8.1',
+    version='0.9.0',
     description='Anonymous linkage using cryptographic hashes and bloom filters',
     url='https://github.com/n1analytics/anonlink',
     license='Apache',
     setup_requires=['cffi>=1.7'],
     install_requires=requirements,
     packages=find_packages(exclude=[
         '_cffi_build', '_cffi_build/*',
         'tests'
     ]),
-    package_data={'anonlink': ['data/*.csv', '_cffi_build']},
+    package_data={'anonlink': ['_cffi_build']},
 
     ext_package="anonlink",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Security :: Cryptography",
     ],
 
     # for cffi
     cffi_modules=["_cffi_build/build_matcher.py:ffibuilder"],
```

### Comparing `anonlink-0.8.1/_cffi_build/build_matcher.py` & `anonlink-0.9.0/_cffi_build/build_matcher.py`

 * *Files identical despite different names*

### Comparing `anonlink-0.8.1/_cffi_build/dice_one_against_many.cpp` & `anonlink-0.9.0/_cffi_build/dice_one_against_many.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     // Constructor with default
     Node( int n_index = -1, double n_score = -1.0 )
         :index(n_index), score( n_score ) { }
 };
 
 struct score_cmp {
     bool operator()(const Node& a, const Node& b) const {
-        return a.score >= b.score;
+        return a.score > b.score || (a.score == b.score && a.index < b.index);
     }
 };
 
 
 /**
  *
  */
@@ -461,16 +461,26 @@
         typedef std::vector<Node> node_vector;
         typedef std::priority_queue<Node, std::vector<Node>, score_cmp> node_queue;
         node_vector vec;
         vec.reserve(k + 1);
         node_queue top_k_scores(score_cmp(), std::move(vec));
 
         uint32_t count_one = _popcount_array(comp1, keywords);
-        if (count_one == 0)
-            return 0;
+        if (count_one == 0) {
+            if (threshold > 0) {
+                return 0;
+            }
+
+            for (uint32_t j = 0; j < k; ++j) {
+                scores[j] = 0.0;
+                indices[j] = j;
+            }
+
+            return static_cast<int>(k);
+        }
 
         uint32_t max_popcnt_delta = keybytes * CHAR_BIT; // = bits per key
         if(threshold > 0) {
             max_popcnt_delta = calculate_max_difference(count_one, threshold);
         }
 
         auto push_score = [&](double score, int idx) {
```

