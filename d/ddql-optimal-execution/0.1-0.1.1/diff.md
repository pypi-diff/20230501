# Comparing `tmp/ddql_optimal_execution-0.1.tar.gz` & `tmp/ddql_optimal_execution-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddql_optimal_execution-0.1.tar", last modified: Sun Apr 30 22:23:58 2023, max compression
+gzip compressed data, was "ddql_optimal_execution-0.1.1.tar", last modified: Sun Apr 30 22:40:36 2023, max compression
```

## Comparing `ddql_optimal_execution-0.1.tar` & `ddql_optimal_execution-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,50 @@
-drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:23:58.597178 ddql_optimal_execution-0.1/
--rw-r--r--   0 g0bel1n    (501) staff       (20)     1059 2023-04-30 22:22:08.000000 ddql_optimal_execution-0.1/LICENSE.txt
--rw-r--r--   0 g0bel1n    (501) staff       (20)      820 2023-04-30 22:23:58.597328 ddql_optimal_execution-0.1/PKG-INFO
--rw-r--r--   0 g0bel1n    (501) staff       (20)      938 2023-04-24 11:55:02.000000 ddql_optimal_execution-0.1/README.md
-drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:23:58.589822 ddql_optimal_execution-0.1/ddql_optimal_execution/
--rw-r--r--   0 g0bel1n    (501) staff       (20)      493 2023-04-16 17:49:33.000000 ddql_optimal_execution-0.1/ddql_optimal_execution/__init__.py
--rw-r--r--   0 g0bel1n    (501) staff       (20)       98 2023-03-03 15:40:46.000000 ddql_optimal_execution-0.1/ddql_optimal_execution/_utils.py
-drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:23:58.591641 ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/
--rw-r--r--   0 g0bel1n    (501) staff       (20)      820 2023-04-30 22:23:58.000000 ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/PKG-INFO
--rw-r--r--   0 g0bel1n    (501) staff       (20)      477 2023-04-30 22:23:58.000000 ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/SOURCES.txt
--rw-r--r--   0 g0bel1n    (501) staff       (20)        1 2023-04-30 22:23:58.000000 ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/dependency_links.txt
--rw-r--r--   0 g0bel1n    (501) staff       (20)       24 2023-04-30 22:23:58.000000 ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/requires.txt
--rw-r--r--   0 g0bel1n    (501) staff       (20)       23 2023-04-30 22:23:58.000000 ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/top_level.txt
--rw-r--r--   0 g0bel1n    (501) staff       (20)       79 2023-04-30 22:23:58.597849 ddql_optimal_execution-0.1/setup.cfg
--rw-r--r--   0 g0bel1n    (501) staff       (20)      992 2023-04-30 22:20:07.000000 ddql_optimal_execution-0.1/setup.py
-drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:23:58.596984 ddql_optimal_execution-0.1/tests/
--rw-r--r--   0 g0bel1n    (501) staff       (20)     1277 2023-04-24 11:04:20.000000 ddql_optimal_execution-0.1/tests/test_MarketEnvironnement.py
--rw-r--r--   0 g0bel1n    (501) staff       (20)      964 2023-04-24 11:10:25.000000 ddql_optimal_execution-0.1/tests/test_State.py
--rw-r--r--   0 g0bel1n    (501) staff       (20)     2377 2023-04-24 11:37:03.000000 ddql_optimal_execution-0.1/tests/test_experience_replay.py
--rw-r--r--   0 g0bel1n    (501) staff       (20)      840 2023-04-24 11:17:50.000000 ddql_optimal_execution-0.1/tests/test_preprocessing.py
--rw-r--r--   0 g0bel1n    (501) staff       (20)        0 2023-03-03 15:52:29.000000 ddql_optimal_execution-0.1/tests/tests_data_utils.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.335792 ddql_optimal_execution-0.1.1/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1059 2023-04-30 22:22:08.000000 ddql_optimal_execution-0.1.1/LICENSE.txt
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      822 2023-04-30 22:40:36.335930 ddql_optimal_execution-0.1.1/PKG-INFO
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      938 2023-04-24 11:55:02.000000 ddql_optimal_execution-0.1.1/README.md
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.310140 ddql_optimal_execution-0.1.1/ddql_optimal_execution/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      493 2023-04-16 17:49:33.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       98 2023-03-03 15:40:46.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/_utils.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.315041 ddql_optimal_execution-0.1.1/ddql_optimal_execution/agent/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       76 2023-04-14 14:39:00.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/agent/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      453 2023-04-19 07:30:58.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/agent/_agent.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     9900 2023-04-26 15:30:10.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/agent/_ddql.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1564 2023-04-18 16:54:17.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/agent/_neural_net.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1511 2023-04-19 07:45:09.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/agent/_twap.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.319430 ddql_optimal_execution-0.1.1/ddql_optimal_execution/environnement/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       72 2023-04-14 11:42:19.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/environnement/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     3730 2023-04-14 17:17:06.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/environnement/_data_processing.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)    11434 2023-04-26 15:26:28.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/environnement/_env.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1007 2023-04-18 15:29:21.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/environnement/_exceptions.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     2353 2023-04-15 15:36:22.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/environnement/_utils.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.323343 ddql_optimal_execution-0.1.1/ddql_optimal_execution/experience_replay/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      156 2023-04-20 09:59:21.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/experience_replay/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      222 2023-04-24 11:25:19.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/experience_replay/_exceptions.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      306 2023-04-15 15:35:40.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/experience_replay/_experience_dict.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     5032 2023-04-24 11:25:39.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/experience_replay/_experience_replay.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      212 2023-04-20 09:58:23.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/experience_replay/_warnings.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.325578 ddql_optimal_execution-0.1.1/ddql_optimal_execution/preprocessing/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       75 2023-04-16 17:49:33.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/preprocessing/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     4522 2023-04-26 13:21:18.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/preprocessing/_preprocessor.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.328946 ddql_optimal_execution-0.1.1/ddql_optimal_execution/state/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       97 2023-04-14 11:38:57.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/state/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1435 2023-04-24 11:09:47.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/state/_state.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      844 2023-04-17 10:37:17.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/state/_state_array.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.331551 ddql_optimal_execution-0.1.1/ddql_optimal_execution/trainer/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       53 2023-04-16 17:49:33.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/trainer/__init__.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     8047 2023-04-26 15:04:37.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/trainer/_trainer.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      252 2023-04-18 15:53:09.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution/trainer/_warnings.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.312032 ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      822 2023-04-30 22:40:36.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/PKG-INFO
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1572 2023-04-30 22:40:36.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 g0bel1n    (501) staff       (20)        1 2023-04-30 22:40:36.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       24 2023-04-30 22:40:36.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/requires.txt
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      227 2023-04-30 22:40:36.000000 ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/top_level.txt
+-rw-r--r--   0 g0bel1n    (501) staff       (20)       79 2023-04-30 22:40:36.336392 ddql_optimal_execution-0.1.1/setup.cfg
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1218 2023-04-30 22:40:32.000000 ddql_optimal_execution-0.1.1/setup.py
+drwxr-xr-x   0 g0bel1n    (501) staff       (20)        0 2023-04-30 22:40:36.335601 ddql_optimal_execution-0.1.1/tests/
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     1277 2023-04-24 11:04:20.000000 ddql_optimal_execution-0.1.1/tests/test_MarketEnvironnement.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      964 2023-04-24 11:10:25.000000 ddql_optimal_execution-0.1.1/tests/test_State.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)     2377 2023-04-24 11:37:03.000000 ddql_optimal_execution-0.1.1/tests/test_experience_replay.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)      840 2023-04-24 11:17:50.000000 ddql_optimal_execution-0.1.1/tests/test_preprocessing.py
+-rw-r--r--   0 g0bel1n    (501) staff       (20)        0 2023-03-03 15:52:29.000000 ddql_optimal_execution-0.1.1/tests/tests_data_utils.py
```

### Comparing `ddql_optimal_execution-0.1/LICENSE.txt` & `ddql_optimal_execution-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddql_optimal_execution-0.1/PKG-INFO` & `ddql_optimal_execution-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddql_optimal_execution
-Version: 0.1
+Version: 0.1.1
 Summary: Double Deep Q Learning for Optimal Trading Execution
 Home-page: https://github.com/g0bel1n/DDQL-optimal-execution
 Download-URL: https://github.com/g0bel1n/DDQL-optimal-execution/archive/refs/tags/v0.1-beta.tar.gz
 Author: Lucas Saban
 Author-email: lucas.saban@icloud.com
 License: MIT
 Keywords: DDQL,OPTIMAL EXECUTION,TRADING
```

### Comparing `ddql_optimal_execution-0.1/README.md` & `ddql_optimal_execution-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ddql_optimal_execution-0.1/ddql_optimal_execution.egg-info/PKG-INFO` & `ddql_optimal_execution-0.1.1/ddql_optimal_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddql-optimal-execution
-Version: 0.1
+Version: 0.1.1
 Summary: Double Deep Q Learning for Optimal Trading Execution
 Home-page: https://github.com/g0bel1n/DDQL-optimal-execution
 Download-URL: https://github.com/g0bel1n/DDQL-optimal-execution/archive/refs/tags/v0.1-beta.tar.gz
 Author: Lucas Saban
 Author-email: lucas.saban@icloud.com
 License: MIT
 Keywords: DDQL,OPTIMAL EXECUTION,TRADING
```

### Comparing `ddql_optimal_execution-0.1/tests/test_MarketEnvironnement.py` & `ddql_optimal_execution-0.1.1/tests/test_MarketEnvironnement.py`

 * *Files identical despite different names*

### Comparing `ddql_optimal_execution-0.1/tests/test_State.py` & `ddql_optimal_execution-0.1.1/tests/test_State.py`

 * *Files identical despite different names*

### Comparing `ddql_optimal_execution-0.1/tests/test_experience_replay.py` & `ddql_optimal_execution-0.1.1/tests/test_experience_replay.py`

 * *Files identical despite different names*

### Comparing `ddql_optimal_execution-0.1/tests/test_preprocessing.py` & `ddql_optimal_execution-0.1.1/tests/test_preprocessing.py`

 * *Files identical despite different names*

