# Comparing `tmp/dexhub-0.6.2.tar.gz` & `tmp/dexhub-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.6.2.tar", last modified: Mon May  1 18:44:08 2023, max compression
+gzip compressed data, was "dexhub-0.6.3.tar", last modified: Mon May  1 18:48:56 2023, max compression
```

## Comparing `dexhub-0.6.2.tar` & `dexhub-0.6.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.594726 dexhub-0.6.2/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-01 18:44:08.594530 dexhub-0.6.2/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.2/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.590243 dexhub-0.6.2/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1136 2023-05-01 18:38:07.000000 dexhub-0.6.2/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.592573 dexhub-0.6.2/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.2/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.2/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    67846 2023-05-01 18:02:06.000000 dexhub-0.6.2/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.2/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.2/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.2/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.593551 dexhub-0.6.2/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.2/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.2/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.2/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.2/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.2/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.2/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.2/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)   141917 2023-04-01 13:32:00.000000 dexhub-0.6.2/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.593979 dexhub-0.6.2/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.2/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.2/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.594313 dexhub-0.6.2/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       40 2023-01-17 19:51:41.000000 dexhub-0.6.2/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    13947 2022-12-05 20:29:28.000000 dexhub-0.6.2/dexhub/util/helper.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:44:08.590943 dexhub-0.6.2/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-01 18:44:08.000000 dexhub-0.6.2/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      657 2023-05-01 18:44:08.000000 dexhub-0.6.2/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-01 18:44:08.000000 dexhub-0.6.2/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-01 18:44:08.000000 dexhub-0.6.2/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-01 18:44:08.000000 dexhub-0.6.2/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-01 18:44:08.594791 dexhub-0.6.2/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-01 18:44:06.000000 dexhub-0.6.2/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.287376 dexhub-0.6.3/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-01 18:48:56.287241 dexhub-0.6.3/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.3/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.279996 dexhub-0.6.3/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1148 2023-05-01 18:47:11.000000 dexhub-0.6.3/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.281447 dexhub-0.6.3/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.3/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.3/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    67846 2023-05-01 18:02:06.000000 dexhub-0.6.3/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.3/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.3/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.3/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.286523 dexhub-0.6.3/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.3/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.3/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.3/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.3/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.3/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.3/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.3/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)   141917 2023-04-01 13:32:00.000000 dexhub-0.6.3/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.286755 dexhub-0.6.3/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.3/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.3/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.287032 dexhub-0.6.3/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       40 2023-01-17 19:51:41.000000 dexhub-0.6.3/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    13947 2022-12-05 20:29:28.000000 dexhub-0.6.3/dexhub/util/helper.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-01 18:48:56.280645 dexhub-0.6.3/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-01 18:48:56.000000 dexhub-0.6.3/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      657 2023-05-01 18:48:56.000000 dexhub-0.6.3/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-01 18:48:56.000000 dexhub-0.6.3/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-01 18:48:56.000000 dexhub-0.6.3/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-01 18:48:56.000000 dexhub-0.6.3/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-01 18:48:56.287421 dexhub-0.6.3/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-01 18:48:49.000000 dexhub-0.6.3/setup.py
```

### Comparing `dexhub-0.6.2/PKG-INFO` & `dexhub-0.6.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.2
+Version: 0.6.3
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.2/dexhub/__init__.py` & `dexhub-0.6.3/dexhub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,13 @@
 )
 
 from dexhub.abi.eth_abi import(
     AbiUniswapV3
 )
 
 from dexhub.abi.avax_abi import(
-    AbiJoe
+    AbiJoe,AbiPangolin
 )
 
 from dexhub.abi.arbitrum_abi import(
     AbiArbitrumJoe,AbiSushi
 )
```

### Comparing `dexhub-0.6.2/dexhub/abi/arbitrum_abi.py` & `dexhub-0.6.3/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/abi/avax_abi.py` & `dexhub-0.6.3/dexhub/abi/avax_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/abi/dfk_abi.py` & `dexhub-0.6.3/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/abi/eth_abi.py` & `dexhub-0.6.3/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/abi/klay_abi.py` & `dexhub-0.6.3/dexhub/abi/klay_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/address/arbitrum_address.py` & `dexhub-0.6.3/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/address/avax_address.py` & `dexhub-0.6.3/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/address/dfk_address.py` & `dexhub-0.6.3/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/address/eth_address.py` & `dexhub-0.6.3/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/address/klay_address.py` & `dexhub-0.6.3/dexhub/address/klay_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/address/polygon_address.py` & `dexhub-0.6.3/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/dex.py` & `dexhub-0.6.3/dexhub/dex.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/interface/joe.py` & `dexhub-0.6.3/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub/util/helper.py` & `dexhub-0.6.3/dexhub/util/helper.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/dexhub.egg-info/PKG-INFO` & `dexhub-0.6.3/dexhub.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.2
+Version: 0.6.3
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.2/dexhub.egg-info/SOURCES.txt` & `dexhub-0.6.3/dexhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.2/setup.py` & `dexhub-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.6.2",
+    version="0.6.3",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

