# Comparing `tmp/souJpg-comm-1.0.4.tar.gz` & `tmp/souJpg-comm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souJpg-comm-1.0.4.tar", last modified: Mon May  1 02:48:27 2023, max compression
+gzip compressed data, was "souJpg-comm-1.0.5.tar", last modified: Mon May  1 03:05:27 2023, max compression
```

## Comparing `souJpg-comm-1.0.4.tar` & `souJpg-comm-1.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.0.4/README.md
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/setup.cfg
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      792 2023-05-01 02:48:20.000000 souJpg-comm-1.0.4/setup.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.492583 souJpg-comm-1.0.4/souJpg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      325 2023-05-01 02:11:40.000000 souJpg-comm-1.0.4/souJpg/__init__.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2645 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/apiResponse.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/cfg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/cfg/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/cfg/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/cfg/vcgCfg.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/contextManagers.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2026 2023-05-01 01:13:46.000000 souJpg-comm-1.0.4/souJpg/comm/cos.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1383 2023-05-01 02:47:30.000000 souJpg-comm-1.0.4/souJpg/comm/dbHelper.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.0.4/souJpg/comm/dbsCL.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/decorators/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:37:52.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      264 2023-05-01 02:37:52.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/base.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1071 2023-05-01 02:37:52.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1747 2023-05-01 02:38:58.000000 souJpg-comm-1.0.4/souJpg/comm/decorators/methodRetry.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/es/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/es/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15100 2023-05-01 02:47:49.000000 souJpg-comm-1.0.4/souJpg/comm/es/es.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/es/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/es/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/es/test/test.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/fs/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/fs/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/fs/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9760 2023-05-01 01:13:46.000000 souJpg-comm-1.0.4/souJpg/comm/fs/distributeFs.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/hdfsUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16569 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/imageUtils.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 02:47:39.000000 souJpg-comm-1.0.4/souJpg/comm/kafkaOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.0.4/souJpg/comm/labelUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/mathUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/ops/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/ops/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7783 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/ops/ops.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/ops/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/ops/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/ops/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.0.4/souJpg/comm/projectUitls.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/redisOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.0.4/souJpg/comm/sparkApp.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.0.4/souJpg/comm/sparkBase.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg/comm/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    19830 2023-05-01 01:12:37.000000 souJpg-comm-1.0.4/souJpg/comm/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1439 2023-05-01 01:12:39.000000 souJpg-comm-1.0.4/souJpg/comm/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/threadPools.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.0.4/souJpg/comm/vcgUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:48:27.502583 souJpg-comm-1.0.4/souJpg_comm.egg-info/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1246 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      451 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/requires.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-05-01 02:48:27.000000 souJpg-comm-1.0.4/souJpg_comm.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.0.5/README.md
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/setup.cfg
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      792 2023-05-01 03:05:20.000000 souJpg-comm-1.0.5/setup.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.492224 souJpg-comm-1.0.5/souJpg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      325 2023-05-01 02:11:40.000000 souJpg-comm-1.0.5/souJpg/__init__.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.492224 souJpg-comm-1.0.5/souJpg/comm/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2645 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/apiResponse.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.492224 souJpg-comm-1.0.5/souJpg/comm/cfg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/cfg/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/cfg/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/cfg/vcgCfg.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/contextManagers.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2026 2023-05-01 01:13:46.000000 souJpg-comm-1.0.5/souJpg/comm/cos.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1383 2023-05-01 02:47:30.000000 souJpg-comm-1.0.5/souJpg/comm/dbHelper.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.0.5/souJpg/comm/dbsCL.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.492224 souJpg-comm-1.0.5/souJpg/comm/decorators/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:37:52.000000 souJpg-comm-1.0.5/souJpg/comm/decorators/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      264 2023-05-01 02:37:52.000000 souJpg-comm-1.0.5/souJpg/comm/decorators/base.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1071 2023-05-01 02:37:52.000000 souJpg-comm-1.0.5/souJpg/comm/decorators/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1747 2023-05-01 02:38:58.000000 souJpg-comm-1.0.5/souJpg/comm/decorators/methodRetry.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.492224 souJpg-comm-1.0.5/souJpg/comm/es/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/es/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15100 2023-05-01 02:47:49.000000 souJpg-comm-1.0.5/souJpg/comm/es/es.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.492224 souJpg-comm-1.0.5/souJpg/comm/es/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/es/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.0.5/souJpg/comm/es/test/test.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/souJpg/comm/fs/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/fs/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/fs/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9760 2023-05-01 01:13:46.000000 souJpg-comm-1.0.5/souJpg/comm/fs/distributeFs.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/hdfsUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16709 2023-05-01 03:02:12.000000 souJpg-comm-1.0.5/souJpg/comm/imageUtils.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 02:47:39.000000 souJpg-comm-1.0.5/souJpg/comm/kafkaOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.0.5/souJpg/comm/labelUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/mathUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/souJpg/comm/ops/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/ops/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7783 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/ops/ops.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/souJpg/comm/ops/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/ops/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.0.5/souJpg/comm/ops/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.0.5/souJpg/comm/projectUitls.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.0.5/souJpg/comm/redisOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.0.5/souJpg/comm/sparkApp.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.0.5/souJpg/comm/sparkBase.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/souJpg/comm/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    20061 2023-05-01 02:53:50.000000 souJpg-comm-1.0.5/souJpg/comm/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1439 2023-05-01 01:12:39.000000 souJpg-comm-1.0.5/souJpg/comm/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/threadPools.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.0.5/souJpg/comm/vcgUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 03:05:27.502224 souJpg-comm-1.0.5/souJpg_comm.egg-info/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1648 2023-05-01 03:05:27.000000 souJpg-comm-1.0.5/souJpg_comm.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1246 2023-05-01 03:05:27.000000 souJpg-comm-1.0.5/souJpg_comm.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-05-01 03:05:27.000000 souJpg-comm-1.0.5/souJpg_comm.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      451 2023-05-01 03:05:27.000000 souJpg-comm-1.0.5/souJpg_comm.egg-info/requires.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-05-01 03:05:27.000000 souJpg-comm-1.0.5/souJpg_comm.egg-info/top_level.txt
```

### Comparing `souJpg-comm-1.0.4/PKG-INFO` & `souJpg-comm-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.4
+Version: 1.0.5
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `souJpg-comm-1.0.4/README.md` & `souJpg-comm-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/setup.py` & `souJpg-comm-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requireds = f.read().splitlines()
 
 with open(here / "README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="souJpg-comm",
-    version="1.0.4",
+    version="1.0.5",
     author="zhaoyufei",
     author_email="",
     description="souJpg-comm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

### Comparing `souJpg-comm-1.0.4/souJpg/comm/apiResponse.py` & `souJpg-comm-1.0.5/souJpg/comm/apiResponse.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/cfg/utils.py` & `souJpg-comm-1.0.5/souJpg/comm/cfg/utils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/cfg/vcgCfg.py` & `souJpg-comm-1.0.5/souJpg/comm/cfg/vcgCfg.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/contextManagers.py` & `souJpg-comm-1.0.5/souJpg/comm/contextManagers.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/cos.py` & `souJpg-comm-1.0.5/souJpg/comm/cos.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/dbHelper.py` & `souJpg-comm-1.0.5/souJpg/comm/dbHelper.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/dbsCL.py` & `souJpg-comm-1.0.5/souJpg/comm/dbsCL.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/decorators/comm.py` & `souJpg-comm-1.0.5/souJpg/comm/decorators/comm.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/decorators/methodRetry.py` & `souJpg-comm-1.0.5/souJpg/comm/decorators/methodRetry.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/es/es.py` & `souJpg-comm-1.0.5/souJpg/comm/es/es.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/es/test/test.py` & `souJpg-comm-1.0.5/souJpg/comm/es/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/fs/distributeFs.py` & `souJpg-comm-1.0.5/souJpg/comm/fs/distributeFs.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/hdfsUtils.py` & `souJpg-comm-1.0.5/souJpg/comm/hdfsUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/imageUtils.py` & `souJpg-comm-1.0.5/souJpg/comm/imageUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 from PIL import Image
 from PIL import Image as pil_image
 from PIL import ImageColor
 from skimage.io import imsave
 from sklearn.metrics import euclidean_distances
 
 
+def rgb2gray(rgb):
+    r, g, b = rgb[:, :, 0], rgb[:, :, 1], rgb[:, :, 2]
+    gray = 0.2989 * r + 0.5870 * g + 0.1140 * b
+
+    return gray
+
+
 def getImageBytesListFromFolder(folderName: str, ifRgb=True, format="JPEG"):
     _, _, testPaths = next(os.walk(folderName))
 
     logger1.debug(testPaths)
     imageByteses = []
     imageNames = []
 
@@ -178,15 +185,14 @@
     inverse=False,
     ifSmallerNoResize=False,
     ifRgb=True,
     format="JPEG",
 ):
     newImageBytes = None
     try:
-
         imageBytes = None
         with open(imagePath, "rb") as image:
             imageBytes = image.read()
 
         # if targetSize is not None:
         #     newImageBytes = resizeImageBytes(imageBytes=imageBytes, targetSize=targetSize, inverse=inverse,ifSmallerNoResize=ifSmallerNoResize)
         # else:
@@ -227,15 +233,14 @@
         width = shape[1]
 
         splitedHeight = int(height / verticalSplitParts)
         splitedWidth = int(width / horizontalSplitParts)
 
         for horizontalSplitIndex in range(0, horizontalSplitParts):
             for verticalSplitIndex in range(0, verticalSplitParts):
-
                 startCloumns = horizontalSplitIndex * splitedWidth
                 endCloumns = (horizontalSplitIndex + 1) * splitedWidth
                 startRows = verticalSplitIndex * splitedHeight
                 endRows = (verticalSplitIndex + 1) * splitedHeight
 
                 block = img[startRows:endRows, startCloumns:endCloumns]
                 splitsArray.append(block)
@@ -311,15 +316,14 @@
 def getWH(imageBytes=None):
     img = pil_image.open(io.BytesIO(imageBytes))
     w, h = img.size
     return (w, h)
 
 
 def imagesMaker(imageBytes=None):
-
     """
     resolution: small, preview, medium, large
     small < 500*800
     preview < 1000*1500   webp
     medium  < 2000*3000  webp
     large  > 2000*3000   webp
 
@@ -355,15 +359,14 @@
         resolution = "preview"
     elif size > previewSize and size < mediumSize:
         resolution = "medium"
     elif size >= mediumSize:
         resolution = "large"
 
     if resolution == "preview":
-
         previewBytes = resizeImageBytes(
             imageBytes=imageBytes,
             format="webp",
             quality=previewQuality,
         )
 
         mediumBytes = imageBytes
```

### Comparing `souJpg-comm-1.0.4/souJpg/comm/kafkaOps.py` & `souJpg-comm-1.0.5/souJpg/comm/kafkaOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/labelUtils.py` & `souJpg-comm-1.0.5/souJpg/comm/labelUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/mathUtils.py` & `souJpg-comm-1.0.5/souJpg/comm/mathUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/ops/ops.py` & `souJpg-comm-1.0.5/souJpg/comm/ops/ops.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/ops/test/test.py` & `souJpg-comm-1.0.5/souJpg/comm/ops/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/projectUitls.py` & `souJpg-comm-1.0.5/souJpg/comm/projectUitls.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/redisOps.py` & `souJpg-comm-1.0.5/souJpg/comm/redisOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/sparkApp.py` & `souJpg-comm-1.0.5/souJpg/comm/sparkApp.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/sparkBase.py` & `souJpg-comm-1.0.5/souJpg/comm/sparkBase.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/test/test.py` & `souJpg-comm-1.0.5/souJpg/comm/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from numpy import linalg as LA
 from omegaconf import OmegaConf
 from PIL import Image as pil_image
 
 from souJpg.comm import imageUtils
 from souJpg.comm.cfg.utils import initGcf
 from souJpg.comm.cfg.vcgCfg import VcgCfg
+from souJpg.comm.dbHelper import createMongoDBConnection
 from souJpg.comm.fs.distributeFs import MinioFs
 from souJpg.comm.kafkaOps import ConsumerParams, KafkaOps, Message
 from souJpg.comm.labelUtils import MongoLabelUtils
 from souJpg.comm.redisOps import RedisOps, cached
 
 
 class MongoLabelUtilsTest(unittest.TestCase):
@@ -257,15 +258,19 @@
         )
         with pil_image.open(io.BytesIO(imageBytes)) as img:
             # if img.mode != "RGB":
             #     img = img.convert("RGB")
             logger1.info(img.size)
             img.save("testImages/test1.png", format="PNG", quality=quality)
 
-
+class CommTest(unittest.TestCase):
+    def test_createMongoDBConnection(self):
+        db=createMongoDBConnection(dbType='imagesCoreDBURI')
+        logger1.info(db)
+    
 from souJpg.comm.dbsCL import batchPut
 
 
 class DbsClTest(unittest.TestCase):
     def setUp(self) -> None:
         host = "gpu0.dev.yufei.com"
```

### Comparing `souJpg-comm-1.0.4/souJpg/comm/test.py` & `souJpg-comm-1.0.5/souJpg/comm/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg/comm/vcgUtils.py` & `souJpg-comm-1.0.5/souJpg/comm/vcgUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.0.4/souJpg_comm.egg-info/PKG-INFO` & `souJpg-comm-1.0.5/souJpg_comm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souJpg-comm
-Version: 1.0.4
+Version: 1.0.5
 Summary: souJpg-comm
 Home-page: 
 Author: zhaoyufei
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `souJpg-comm-1.0.4/souJpg_comm.egg-info/SOURCES.txt` & `souJpg-comm-1.0.5/souJpg_comm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

