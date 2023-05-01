# Comparing `tmp/souJpg-comm-1.0.0.tar.gz` & `tmp/souJpg-comm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souJpg-comm-1.0.0.tar", last modified: Mon May  1 01:24:29 2023, max compression
+gzip compressed data, was "souJpg-comm-1.0.1.tar", last modified: Mon May  1 01:41:39 2023, max compression
```

## Comparing `souJpg-comm-1.0.0.tar` & `souJpg-comm-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.0.0/README.md
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/setup.cfg
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      792 2023-05-01 01:24:26.000000 souJpg-comm-1.0.0/setup.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.284324 souJpg-comm-1.0.0/souJpg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:32.000000 souJpg-comm-1.0.0/souJpg/__init__.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.284324 souJpg-comm-1.0.0/souJpg/comm/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2645 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/apiResponse.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/cfg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/cfg/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/cfg/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/cfg/vcgCfg.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/contextManagers.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2026 2023-05-01 01:13:46.000000 souJpg-comm-1.0.0/souJpg/comm/cos.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1418 2023-05-01 01:13:46.000000 souJpg-comm-1.0.0/souJpg/comm/dbHelper.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.0.0/souJpg/comm/dbsCL.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/es/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/es/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15076 2023-05-01 01:13:46.000000 souJpg-comm-1.0.0/souJpg/comm/es/es.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/es/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/es/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.0.0/souJpg/comm/es/test/test.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/fs/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/fs/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/fs/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9760 2023-05-01 01:13:46.000000 souJpg-comm-1.0.0/souJpg/comm/fs/distributeFs.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/hdfsUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16569 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/imageUtils.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 01:13:46.000000 souJpg-comm-1.0.0/souJpg/comm/kafkaOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.0.0/souJpg/comm/labelUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/mathUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/ops/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/ops/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7783 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/ops/ops.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/ops/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/ops/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.0.0/souJpg/comm/ops/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.0.0/souJpg/comm/projectUitls.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.0.0/souJpg/comm/redisOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.0.0/souJpg/comm/sparkApp.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.0.0/souJpg/comm/sparkBase.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg/comm/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    19830 2023-05-01 01:12:37.000000 souJpg-comm-1.0.0/souJpg/comm/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1439 2023-05-01 01:12:39.000000 souJpg-comm-1.0.0/souJpg/comm/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/threadPools.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.0.0/souJpg/comm/vcgUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:24:29.294324 souJpg-comm-1.0.0/souJpg_comm.egg-info/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 01:24:29.000000 souJpg-comm-1.0.0/souJpg_comm.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1111 2023-05-01 01:24:29.000000 souJpg-comm-1.0.0/souJpg_comm.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-05-01 01:24:29.000000 souJpg-comm-1.0.0/souJpg_comm.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      492 2023-05-01 01:24:29.000000 souJpg-comm-1.0.0/souJpg_comm.egg-info/requires.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-05-01 01:24:29.000000 souJpg-comm-1.0.0/souJpg_comm.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.563965 souJpg-comm-1.0.1/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 01:41:39.563965 souJpg-comm-1.0.1/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.0.1/README.md
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-05-01 01:41:39.563965 souJpg-comm-1.0.1/setup.cfg
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      792 2023-05-01 01:41:35.000000 souJpg-comm-1.0.1/setup.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.543965 souJpg-comm-1.0.1/souJpg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:32.000000 souJpg-comm-1.0.1/souJpg/__init__.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2645 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/apiResponse.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/cfg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/cfg/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/cfg/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/cfg/vcgCfg.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/contextManagers.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2026 2023-05-01 01:13:46.000000 souJpg-comm-1.0.1/souJpg/comm/cos.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1418 2023-05-01 01:13:46.000000 souJpg-comm-1.0.1/souJpg/comm/dbHelper.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.0.1/souJpg/comm/dbsCL.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/es/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/es/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15076 2023-05-01 01:13:46.000000 souJpg-comm-1.0.1/souJpg/comm/es/es.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/es/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/es/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.0.1/souJpg/comm/es/test/test.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/fs/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/fs/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/fs/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9760 2023-05-01 01:13:46.000000 souJpg-comm-1.0.1/souJpg/comm/fs/distributeFs.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/hdfsUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16569 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/imageUtils.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 01:13:46.000000 souJpg-comm-1.0.1/souJpg/comm/kafkaOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.0.1/souJpg/comm/labelUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/mathUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/ops/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/ops/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7783 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/ops/ops.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.553965 souJpg-comm-1.0.1/souJpg/comm/ops/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/ops/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.0.1/souJpg/comm/ops/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.0.1/souJpg/comm/projectUitls.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.0.1/souJpg/comm/redisOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.0.1/souJpg/comm/sparkApp.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.0.1/souJpg/comm/sparkBase.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.563965 souJpg-comm-1.0.1/souJpg/comm/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    19830 2023-05-01 01:12:37.000000 souJpg-comm-1.0.1/souJpg/comm/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1439 2023-05-01 01:12:39.000000 souJpg-comm-1.0.1/souJpg/comm/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/threadPools.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.0.1/souJpg/comm/vcgUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 01:41:39.563965 souJpg-comm-1.0.1/souJpg_comm.egg-info/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 01:41:39.000000 souJpg-comm-1.0.1/souJpg_comm.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1111 2023-05-01 01:41:39.000000 souJpg-comm-1.0.1/souJpg_comm.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-05-01 01:41:39.000000 souJpg-comm-1.0.1/souJpg_comm.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      451 2023-05-01 01:41:39.000000 souJpg-comm-1.0.1/souJpg_comm.egg-info/requires.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-05-01 01:41:39.000000 souJpg-comm-1.0.1/souJpg_comm.egg-info/top_level.txt
```

### Comparing `souJpg-comm-1.0.0/PKG-INFO` & `souJpg-comm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.0
+Version: 1.0.1
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `souJpg-comm-1.0.0/README.md` & `souJpg-comm-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/setup.py` & `souJpg-comm-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requireds = f.read().splitlines()
 
 with open(here / "README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="souJpg-comm",
-    version="1.0.0",
+    version="1.0.1",
     author="zhaoyufei",
     author_email="",
     description="souJpg-comm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

### Comparing `souJpg-comm-1.0.0/souJpg/comm/apiResponse.py` & `souJpg-comm-1.0.1/souJpg/comm/apiResponse.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/cfg/utils.py` & `souJpg-comm-1.0.1/souJpg/comm/cfg/utils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/cfg/vcgCfg.py` & `souJpg-comm-1.0.1/souJpg/comm/cfg/vcgCfg.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/contextManagers.py` & `souJpg-comm-1.0.1/souJpg/comm/contextManagers.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/cos.py` & `souJpg-comm-1.0.1/souJpg/comm/cos.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/dbHelper.py` & `souJpg-comm-1.0.1/souJpg/comm/dbHelper.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/dbsCL.py` & `souJpg-comm-1.0.1/souJpg/comm/dbsCL.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/es/es.py` & `souJpg-comm-1.0.1/souJpg/comm/es/es.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/es/test/test.py` & `souJpg-comm-1.0.1/souJpg/comm/es/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/fs/distributeFs.py` & `souJpg-comm-1.0.1/souJpg/comm/fs/distributeFs.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/hdfsUtils.py` & `souJpg-comm-1.0.1/souJpg/comm/hdfsUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/imageUtils.py` & `souJpg-comm-1.0.1/souJpg/comm/imageUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/kafkaOps.py` & `souJpg-comm-1.0.1/souJpg/comm/kafkaOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/labelUtils.py` & `souJpg-comm-1.0.1/souJpg/comm/labelUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/mathUtils.py` & `souJpg-comm-1.0.1/souJpg/comm/mathUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/ops/ops.py` & `souJpg-comm-1.0.1/souJpg/comm/ops/ops.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/ops/test/test.py` & `souJpg-comm-1.0.1/souJpg/comm/ops/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/projectUitls.py` & `souJpg-comm-1.0.1/souJpg/comm/projectUitls.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/redisOps.py` & `souJpg-comm-1.0.1/souJpg/comm/redisOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/sparkApp.py` & `souJpg-comm-1.0.1/souJpg/comm/sparkApp.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/sparkBase.py` & `souJpg-comm-1.0.1/souJpg/comm/sparkBase.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/test/test.py` & `souJpg-comm-1.0.1/souJpg/comm/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/test.py` & `souJpg-comm-1.0.1/souJpg/comm/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg/comm/vcgUtils.py` & `souJpg-comm-1.0.1/souJpg/comm/vcgUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.0/souJpg_comm.egg-info/PKG-INFO` & `souJpg-comm-1.0.1/souJpg_comm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.0
+Version: 1.0.1
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `souJpg-comm-1.0.0/souJpg_comm.egg-info/SOURCES.txt` & `souJpg-comm-1.0.1/souJpg_comm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

