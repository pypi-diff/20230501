# Comparing `tmp/opal-server-0.6.0.tar.gz` & `tmp/opal-server-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-server-0.6.0.tar", last modified: Fri Apr 21 07:57:02 2023, max compression
+gzip compressed data, was "opal-server-0.6.1.tar", last modified: Mon May  1 17:32:28 2023, max compression
```

## Comparing `opal-server-0.6.0.tar` & `opal-server-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.142644 opal-server-0.6.0/
--rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-04-21 07:57:02.142280 opal-server-0.6.0/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.138218 opal-server-0.6.0/opal_server/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-04-19 15:20:19.000000 opal-server-0.6.0/opal_server/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10418 2023-04-19 15:20:19.000000 opal-server-0.6.0/opal_server/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139596 opal-server-0.6.0/opal_server/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5297 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-03-27 15:01:56.000000 opal-server-0.6.0/opal_server/data/data_update_publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/git_fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/loadlimiting.py
--rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139745 opal-server-0.6.0/opal_server/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139947 opal-server-0.6.0/opal_server/policy/bundles/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4444 2023-02-14 09:43:53.000000 opal-server-0.6.0/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.140439 opal-server-0.6.0/opal_server/policy/watcher/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4459 2023-02-28 14:04:36.000000 opal-server-0.6.0/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5669 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/policy/watcher/factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.140941 opal-server-0.6.0/opal_server/policy/webhook/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5675 2023-03-12 07:32:46.000000 opal-server-0.6.0/opal_server/policy/webhook/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-02-14 09:43:53.000000 opal-server-0.6.0/opal_server/policy/webhook/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/webhook/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-04-18 15:25:03.000000 opal-server-0.6.0/opal_server/pubsub.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1390 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/redis.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.141658 opal-server-0.6.0/opal_server/scopes/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/scopes/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12600 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/loader.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1325 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/scopes/scope_repository.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7285 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/service.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.142059 opal-server-0.6.0/opal_server/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1423 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/security/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/security/jwks.py
--rw-r--r--   0 roekatz    (501) staff       (20)    16902 2023-04-19 10:07:30.000000 opal-server-0.6.0/opal_server/server.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-01-19 13:43:15.000000 opal-server-0.6.0/opal_server/statistics.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139207 opal-server-0.6.0/opal_server.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      546 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-04-21 07:57:02.142693 opal-server-0.6.0/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.6.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.175556 opal-server-0.6.1/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-05-01 17:32:28.175362 opal-server-0.6.1/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.170313 opal-server-0.6.1/opal_server/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-04-19 15:20:19.000000 opal-server-0.6.1/opal_server/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10418 2023-04-19 15:20:19.000000 opal-server-0.6.1/opal_server/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.171965 opal-server-0.6.1/opal_server/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5297 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-03-27 15:01:56.000000 opal-server-0.6.1/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/git_fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/loadlimiting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.172173 opal-server-0.6.1/opal_server/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.172454 opal-server-0.6.1/opal_server/policy/bundles/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4444 2023-02-14 09:43:53.000000 opal-server-0.6.1/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.173033 opal-server-0.6.1/opal_server/policy/watcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4459 2023-02-28 14:04:36.000000 opal-server-0.6.1/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5669 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-04-29 17:08:57.000000 opal-server-0.6.1/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.173801 opal-server-0.6.1/opal_server/policy/webhook/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5691 2023-05-01 10:44:58.000000 opal-server-0.6.1/opal_server/policy/webhook/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-02-14 09:43:53.000000 opal-server-0.6.1/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-04-18 15:25:03.000000 opal-server-0.6.1/opal_server/pubsub.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1390 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/redis.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.174748 opal-server-0.6.1/opal_server/scopes/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/scopes/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12600 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/loader.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1325 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7285 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/service.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.175128 opal-server-0.6.1/opal_server/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1423 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/security/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/security/jwks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17522 2023-05-01 10:44:58.000000 opal-server-0.6.1/opal_server/server.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-04-30 12:13:52.000000 opal-server-0.6.1/opal_server/statistics.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.171591 opal-server-0.6.1/opal_server.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      546 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-05-01 17:32:28.175598 opal-server-0.6.1/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.6.1/setup.py
```

### Comparing `opal-server-0.6.0/PKG-INFO` & `opal-server-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.6.0
+Version: 0.6.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.6.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.6.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
```

### Comparing `opal-server-0.6.0/opal_server/cli.py` & `opal-server-0.6.1/opal_server/cli.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/config.py` & `opal-server-0.6.1/opal_server/config.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/data/api.py` & `opal-server-0.6.1/opal_server/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/data/data_update_publisher.py` & `opal-server-0.6.1/opal_server/data/data_update_publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/git_fetcher.py` & `opal-server-0.6.1/opal_server/git_fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/loadlimiting.py` & `opal-server-0.6.1/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/policy/bundles/api.py` & `opal-server-0.6.1/opal_server/policy/bundles/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/policy/watcher/callbacks.py` & `opal-server-0.6.1/opal_server/policy/watcher/callbacks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/policy/watcher/factory.py` & `opal-server-0.6.1/opal_server/policy/watcher/factory.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/policy/watcher/task.py` & `opal-server-0.6.1/opal_server/policy/watcher/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/policy/webhook/api.py` & `opal-server-0.6.1/opal_server/policy/webhook/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,21 @@
 
     @router.post(
         "/webhook",
         status_code=status.HTTP_200_OK,
         dependencies=route_dependencies,
     )
     async def trigger_webhook(request: Request, git_changes: GitChanges = git_changes):
-        # look at values extracted from request
-        urls = git_changes.urls
-        branch = git_changes.branch
-        names = git_changes.names
 
         # TODO: breaking change: change "repo_url" to "remote_url" in next major
         if source_type == PolicySourceTypes.Git:
+            # look at values extracted from request
+            urls = git_changes.urls
+            branch = git_changes.branch
+            names = git_changes.names
 
             # Enforce branch matching (webhook to config) if turned on via config
             if (
                 opal_server_config.POLICY_REPO_WEBHOOK_ENFORCE_BRANCH
                 and opal_server_config.POLICY_REPO_MAIN_BRANCH != branch
             ):
                 logger.warning(
```

### Comparing `opal-server-0.6.0/opal_server/policy/webhook/deps.py` & `opal-server-0.6.1/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/policy/webhook/listener.py` & `opal-server-0.6.1/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/publisher.py` & `opal-server-0.6.1/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/pubsub.py` & `opal-server-0.6.1/opal_server/pubsub.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/redis.py` & `opal-server-0.6.1/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/scopes/api.py` & `opal-server-0.6.1/opal_server/scopes/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/scopes/loader.py` & `opal-server-0.6.1/opal_server/scopes/loader.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/scopes/scope_repository.py` & `opal-server-0.6.1/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/scopes/service.py` & `opal-server-0.6.1/opal_server/scopes/service.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/scopes/task.py` & `opal-server-0.6.1/opal_server/scopes/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/security/api.py` & `opal-server-0.6.1/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/security/jwks.py` & `opal-server-0.6.1/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server/server.py` & `opal-server-0.6.1/opal_server/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import os
+import signal
 import sys
 import traceback
 from functools import partial
 from typing import List, Optional
 
 from fastapi import Depends, FastAPI
 from fastapi_websocket_pubsub.event_broadcaster import EventBroadcasterContextManager
@@ -316,14 +317,18 @@
             async with self.publisher:
                 if self.opal_statistics is not None:
                     if self.broadcast_listening_context is not None:
                         logger.info(
                             "listening on broadcast channel for statistics events..."
                         )
                         await self.broadcast_listening_context.__aenter__()
+                        # if the broadcast channel is closed, we want to restart worker process because statistics can't be reliable anymore
+                        self.broadcast_listening_context._event_broadcaster.get_reader_task().add_done_callback(
+                            lambda _: self._graceful_shutdown()
+                        )
                     asyncio.create_task(self.opal_statistics.run())
                     self.pubsub.endpoint.notifier.register_unsubscribe_event(
                         self.opal_statistics.remove_client
                     )
 
                 # We want only one worker to run repo watchers
                 # (otherwise for each new commit, we will publish multiple updates via pub/sub).
@@ -359,14 +364,17 @@
                         self.watcher = setup_watcher_task(
                             self.publisher, self.pubsub.endpoint
                         )
                         # running the watcher, and waiting until it stops (until self.watcher.signal_stop() is called)
                         async with self.watcher:
                             await self.watcher.wait_until_should_stop()
 
+                            # Worker should restart when watcher stops
+                            self._graceful_shutdown()
+
                 if (
                     self.opal_statistics is not None
                     and self.broadcast_listening_context is not None
                 ):
                     await self.broadcast_listening_context.__aexit__()
                     logger.info(
                         "stopped listening for statistics events on the broadcast channel"
@@ -384,7 +392,11 @@
         if self.broadcast_keepalive is not None:
             tasks.append(asyncio.create_task(self.broadcast_keepalive.stop()))
 
         try:
             await asyncio.gather(*tasks)
         except Exception:
             logger.exception("exception while shutting down background tasks")
+
+    def _graceful_shutdown(self):
+        logger.info("Trigger worker graceful shutdown")
+        os.kill(os.getpid(), signal.SIGTERM)
```

### Comparing `opal-server-0.6.0/opal_server/statistics.py` & `opal-server-0.6.1/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server.egg-info/PKG-INFO` & `opal-server-0.6.1/opal_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.6.0
+Version: 0.6.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.6.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.6.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
```

### Comparing `opal-server-0.6.0/opal_server.egg-info/SOURCES.txt` & `opal-server-0.6.1/opal_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.0/opal_server.egg-info/requires.txt` & `opal-server-0.6.1/opal_server.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 websockets<11,>=10.3
 ddtrace<2,>=1.1.4
 slowapi<1,>=0.1.5
 aioredis<3,>=2.0.1
 pygit2<2,>=1.9.2
 asgiref<4,>=3.5.2
 redis<5,>=4.3.4
-opal-common==0.6.0
+opal-common==0.6.1
 charset-normalizer<3,>=2.0.12
 idna<4,>=3.3
 typer<1,>=0.4.1
 fastapi<1,>=0.78.0
 fastapi_websocket_pubsub==0.3.3
 fastapi_websocket_rpc<1,>=0.1.21
 gunicorn<21,>=20.1.0
```

### Comparing `opal-server-0.6.0/setup.py` & `opal-server-0.6.1/setup.py`

 * *Files identical despite different names*

