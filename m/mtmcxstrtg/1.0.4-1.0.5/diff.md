# Comparing `tmp/mtmcxstrtg-1.0.4.tar.gz` & `tmp/mtmcxstrtg-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmcxstrtg-1.0.4.tar", last modified: Tue Apr 25 15:59:49 2023, max compression
+gzip compressed data, was "mtmcxstrtg-1.0.5.tar", last modified: Mon May  1 13:13:35 2023, max compression
```

## Comparing `mtmcxstrtg-1.0.4.tar` & `mtmcxstrtg-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.395214 mtmcxstrtg-1.0.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/scripts/run.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.391214 mtmcxstrtg-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.395214 mtmcxstrtg-1.0.4/src/mtmcxstrtg/
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.399214 mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-04-25 15:59:40.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:49.395214 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 15:59:49.000000 mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:35.220467 mtmcxstrtg-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-01 13:13:35.220467 mtmcxstrtg-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:35.216467 mtmcxstrtg-1.0.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 13:13:35.220467 mtmcxstrtg-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:35.216467 mtmcxstrtg-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:35.216467 mtmcxstrtg-1.0.5/src/mtmcxstrtg/
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:35.220467 mtmcxstrtg-1.0.5/src/mtmcxstrtg/strategy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-05-01 13:13:22.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 13:13:35.220467 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-01 13:13:35.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-05-01 13:13:35.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 13:13:35.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 13:13:35.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-01 13:13:35.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-01 13:13:35.000000 mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/top_level.txt
```

### Comparing `mtmcxstrtg-1.0.4/PKG-INFO` & `mtmcxstrtg-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmcxstrtg
-Version: 1.0.4
+Version: 1.0.5
 Summary: imutum_cryptocurrency_strategy
 Home-page: https://github.com/imutum/imutum_cryptocurrency_strategy
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmcxstrtg-1.0.4/scripts/run.py` & `mtmcxstrtg-1.0.5/scripts/run.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.4/setup.py` & `mtmcxstrtg-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_cryptocurrency_strategy"
 abbreviation_name = "mtmcxstrtg"  # 缩写
 description = ""
-version = "1.0.4"
+version = "1.0.5"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmcxstrtg-1.0.4/src/mtmcxstrtg/account.py` & `mtmcxstrtg-1.0.5/src/mtmcxstrtg/account.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.4/src/mtmcxstrtg/config.py` & `mtmcxstrtg-1.0.5/src/mtmcxstrtg/config.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.4/src/mtmcxstrtg/flow.py` & `mtmcxstrtg-1.0.5/src/mtmcxstrtg/flow.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.4/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py` & `mtmcxstrtg-1.0.5/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # 准备工作, 从yaml中的流配置中创建需要的部分参数
     clients = {account_info["userId"]: Account(account_info) for account_info in accounts_info}
     envs["ccxt"] = clients
     for flow_item in config_dict["strategy"]["flow"]:
         envs[flow_item["var"]] = action(action_info=flow_item["action"], envs=envs)
 
     # 以下是策略逻辑
-    next_quantity = 0
+    next_quantity = envs["quote_coins"]
     next_amount = envs["base_coins"]
     for trigger_item in strategy_info["trigger"]:
         if envs[trigger_item["condition"]]:
             # 交易
             action(action_info=trigger_item["action"], envs=envs)
 
             # 记录本次交易信息
```

### Comparing `mtmcxstrtg-1.0.4/src/mtmcxstrtg/util.py` & `mtmcxstrtg-1.0.5/src/mtmcxstrtg/util.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.4/src/mtmcxstrtg.egg-info/PKG-INFO` & `mtmcxstrtg-1.0.5/src/mtmcxstrtg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmcxstrtg
-Version: 1.0.4
+Version: 1.0.5
 Summary: imutum_cryptocurrency_strategy
 Home-page: https://github.com/imutum/imutum_cryptocurrency_strategy
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

