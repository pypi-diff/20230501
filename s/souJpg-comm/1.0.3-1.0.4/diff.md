# Comparing `tmp/souJpg-comm-1.0.3.tar.gz` & `tmp/souJpg-comm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souJpg-comm-1.0.3.tar", last modified: Mon May  1 02:42:19 2023, max compression
+gzip compressed data, was "souJpg-comm-1.0.4.tar", last modified: Mon May  1 02:48:27 2023, max compression
```

## Comparing `souJpg-comm-1.0.3.tar` & `souJpg-comm-1.0.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.852706 souJpg-comm-1.0.3/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 02:42:19.852706 souJpg-comm-1.0.3/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.0.3/README.md
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-05-01 02:42:19.852706 souJpg-comm-1.0.3/setup.cfg
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      792 2023-05-01 02:42:13.000000 souJpg-comm-1.0.3/setup.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.832706 souJpg-comm-1.0.3/souJpg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      325 2023-05-01 02:11:40.000000 souJpg-comm-1.0.3/souJpg/__init__.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2645 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/apiResponse.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/cfg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/cfg/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/cfg/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/cfg/vcgCfg.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/contextManagers.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2026 2023-05-01 01:13:46.000000 souJpg-comm-1.0.3/souJpg/comm/cos.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1359 2023-05-01 01:46:23.000000 souJpg-comm-1.0.3/souJpg/comm/dbHelper.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.0.3/souJpg/comm/dbsCL.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/decorators/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:37:52.000000 souJpg-comm-1.0.3/souJpg/comm/decorators/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      264 2023-05-01 02:37:52.000000 souJpg-comm-1.0.3/souJpg/comm/decorators/base.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1071 2023-05-01 02:37:52.000000 souJpg-comm-1.0.3/souJpg/comm/decorators/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1747 2023-05-01 02:38:58.000000 souJpg-comm-1.0.3/souJpg/comm/decorators/methodRetry.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/es/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/es/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15076 2023-05-01 01:13:46.000000 souJpg-comm-1.0.3/souJpg/comm/es/es.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/es/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/es/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.0.3/souJpg/comm/es/test/test.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/fs/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/fs/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/fs/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9760 2023-05-01 01:13:46.000000 souJpg-comm-1.0.3/souJpg/comm/fs/distributeFs.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/hdfsUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16569 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/imageUtils.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 01:13:46.000000 souJpg-comm-1.0.3/souJpg/comm/kafkaOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.0.3/souJpg/comm/labelUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/mathUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/ops/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/ops/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7783 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/ops/ops.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/ops/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/ops/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.0.3/souJpg/comm/ops/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.0.3/souJpg/comm/projectUitls.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.0.3/souJpg/comm/redisOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.0.3/souJpg/comm/sparkApp.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.0.3/souJpg/comm/sparkBase.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.842706 souJpg-comm-1.0.3/souJpg/comm/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    19830 2023-05-01 01:12:37.000000 souJpg-comm-1.0.3/souJpg/comm/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1439 2023-05-01 01:12:39.000000 souJpg-comm-1.0.3/souJpg/comm/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/threadPools.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.0.3/souJpg/comm/vcgUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:42:19.852706 souJpg-comm-1.0.3/souJpg_comm.egg-info/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 02:42:19.000000 souJpg-comm-1.0.3/souJpg_comm.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1246 2023-05-01 02:42:19.000000 souJpg-comm-1.0.3/souJpg_comm.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-05-01 02:42:19.000000 souJpg-comm-1.0.3/souJpg_comm.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      451 2023-05-01 02:42:19.000000 souJpg-comm-1.0.3/souJpg_comm.egg-info/requires.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-05-01 02:42:19.000000 souJpg-comm-1.0.3/souJpg_comm.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.0.4/README.md
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/setup.cfg
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      792 2023-05-01 02:48:20.000000 souJpg-comm-1.0.4/setup.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.492583 souJpg-comm-1.0.4/souJpg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      325 2023-05-01 02:11:40.000000 souJpg-comm-1.0.4/souJpg/__init__.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2645 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/apiResponse.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/cfg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/cfg/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/cfg/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/cfg/vcgCfg.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/contextManagers.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2026 2023-05-01 01:13:46.000000 souJpg-comm-1.0.4/souJpg/comm/cos.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1383 2023-05-01 02:47:30.000000 souJpg-comm-1.0.4/souJpg/comm/dbHelper.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.0.4/souJpg/comm/dbsCL.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/decorators/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:37:52.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      264 2023-05-01 02:37:52.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/base.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1071 2023-05-01 02:37:52.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1747 2023-05-01 02:38:58.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/methodRetry.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/es/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/es/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15100 2023-05-01 02:47:49.000000 souJpg-comm-1.0.4/souJpg/comm/es/es.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/es/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/es/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/es/test/test.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/fs/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/fs/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/fs/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9760 2023-05-01 01:13:46.000000 souJpg-comm-1.0.4/souJpg/comm/fs/distributeFs.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/hdfsUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16569 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/imageUtils.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 02:47:39.000000 souJpg-comm-1.0.4/souJpg/comm/kafkaOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.0.4/souJpg/comm/labelUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/mathUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/ops/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/ops/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7783 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/ops/ops.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/ops/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/ops/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/ops/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.0.4/souJpg/comm/projectUitls.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/redisOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.0.4/souJpg/comm/sparkApp.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.0.4/souJpg/comm/sparkBase.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    19830 2023-05-01 01:12:37.000000 souJpg-comm-1.0.4/souJpg/comm/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1439 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/threadPools.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/vcgUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg_comm.egg-info/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1246 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      451 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/requires.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/top_level.txt
```

### Comparing `souJpg-comm-1.0.3/PKG-INFO` & `souJpg-comm-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.3
+Version: 1.0.4
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `souJpg-comm-1.0.3/README.md` & `souJpg-comm-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/setup.py` & `souJpg-comm-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requireds = f.read().splitlines()
 
 with open(here / "README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="souJpg-comm",
-    version="1.0.3",
+    version="1.0.4",
     author="zhaoyufei",
     author_email="",
     description="souJpg-comm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

### Comparing `souJpg-comm-1.0.3/souJpg/comm/apiResponse.py` & `souJpg-comm-1.0.4/souJpg/comm/apiResponse.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/cfg/utils.py` & `souJpg-comm-1.0.4/souJpg/comm/cfg/utils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/cfg/vcgCfg.py` & `souJpg-comm-1.0.4/souJpg/comm/cfg/vcgCfg.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/contextManagers.py` & `souJpg-comm-1.0.4/souJpg/comm/contextManagers.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/cos.py` & `souJpg-comm-1.0.4/souJpg/comm/cos.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/dbHelper.py` & `souJpg-comm-1.0.4/souJpg/comm/dbHelper.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import traceback
 from datetime import datetime
 
 from bson.binary import Binary as BsonBinary
 from loguru import logger as logger1
 from pymongo import InsertOne, MongoClient, UpdateMany, UpdateOne
 
+from souJpg import gcf
+
 dbType2CollectionMap = {}
 connection_lock = threading.Lock()
 
 
 def createMongoDBConnection(dbType=None):
     global dbType2CollectionMap
```

### Comparing `souJpg-comm-1.0.3/souJpg/comm/dbsCL.py` & `souJpg-comm-1.0.4/souJpg/comm/dbsCL.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/decorators/comm.py` & `souJpg-comm-1.0.4/souJpg/comm/decorators/comm.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/decorators/methodRetry.py` & `souJpg-comm-1.0.4/souJpg/comm/decorators/methodRetry.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/es/es.py` & `souJpg-comm-1.0.4/souJpg/comm/es/es.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from typing import List
 
 import shortuuid
 from elasticsearch import Elasticsearch, helpers
 from loguru import logger as logger1
 
+from souJpg import gcf
 from souJpg.comm.utils import singleton
 
 
 @singleton
 class EsBasedOps:
     def __init__(self, params={}):
         self.params = params
```

### Comparing `souJpg-comm-1.0.3/souJpg/comm/es/test/test.py` & `souJpg-comm-1.0.4/souJpg/comm/es/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/fs/distributeFs.py` & `souJpg-comm-1.0.4/souJpg/comm/fs/distributeFs.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/hdfsUtils.py` & `souJpg-comm-1.0.4/souJpg/comm/hdfsUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/imageUtils.py` & `souJpg-comm-1.0.4/souJpg/comm/imageUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/kafkaOps.py` & `souJpg-comm-1.0.4/souJpg/comm/kafkaOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/labelUtils.py` & `souJpg-comm-1.0.4/souJpg/comm/labelUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/mathUtils.py` & `souJpg-comm-1.0.4/souJpg/comm/mathUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/ops/ops.py` & `souJpg-comm-1.0.4/souJpg/comm/ops/ops.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/ops/test/test.py` & `souJpg-comm-1.0.4/souJpg/comm/ops/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/projectUitls.py` & `souJpg-comm-1.0.4/souJpg/comm/projectUitls.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/redisOps.py` & `souJpg-comm-1.0.4/souJpg/comm/redisOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/sparkApp.py` & `souJpg-comm-1.0.4/souJpg/comm/sparkApp.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/sparkBase.py` & `souJpg-comm-1.0.4/souJpg/comm/sparkBase.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/test/test.py` & `souJpg-comm-1.0.4/souJpg/comm/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/test.py` & `souJpg-comm-1.0.4/souJpg/comm/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg/comm/vcgUtils.py` & `souJpg-comm-1.0.4/souJpg/comm/vcgUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.3/souJpg_comm.egg-info/PKG-INFO` & `souJpg-comm-1.0.4/souJpg_comm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.3
+Version: 1.0.4
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `souJpg-comm-1.0.3/souJpg_comm.egg-info/SOURCES.txt` & `souJpg-comm-1.0.4/souJpg_comm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

