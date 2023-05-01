# Comparing `tmp/limacharlie-4.4.4.tar.gz` & `tmp/limacharlie-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limacharlie-4.4.4.tar", last modified: Mon Apr 24 16:29:41 2023, max compression
+gzip compressed data, was "limacharlie-4.4.5.tar", last modified: Sun Apr 30 23:57:24 2023, max compression
```

## Comparing `limacharlie-4.4.4.tar` & `limacharlie-4.4.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-24 16:29:41.540562 limacharlie-4.4.4/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.4/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-24 16:29:41.540562 limacharlie-4.4.4/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.4.4/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-24 16:29:41.537562 limacharlie-4.4.4/limacharlie/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.4/limacharlie/Configs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.4/limacharlie/DRCli.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     5057 2023-04-24 15:42:48.000000 limacharlie-4.4.4/limacharlie/Extensions.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.4/limacharlie/Firehose.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10160 2023-04-24 16:27:39.000000 limacharlie-4.4.4/limacharlie/Hive.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.4/limacharlie/Jobs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.4/limacharlie/Logs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    52397 2023-04-24 15:42:45.000000 limacharlie-4.4.4/limacharlie/Manager.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.4/limacharlie/Payloads.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.4/limacharlie/Query.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.4/limacharlie/Replay.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.4/limacharlie/Replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.4/limacharlie/Search.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.4/limacharlie/Sensor.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.4/limacharlie/SpotCheck.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.4/limacharlie/Spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.4/limacharlie/Sync.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.4/limacharlie/Webhook.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-24 16:28:54.000000 limacharlie-4.4.4/limacharlie/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    13476 2023-04-12 22:28:28.000000 limacharlie-4.4.4/limacharlie/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.4/limacharlie/utils.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-24 16:29:41.539562 limacharlie-4.4.4/limacharlie.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-24 16:29:41.000000 limacharlie-4.4.4/limacharlie.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-24 16:29:41.000000 limacharlie-4.4.4/limacharlie.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-24 16:29:41.000000 limacharlie-4.4.4/limacharlie.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-24 16:29:41.000000 limacharlie-4.4.4/limacharlie.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-24 16:29:41.000000 limacharlie-4.4.4/limacharlie.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-24 16:29:41.000000 limacharlie-4.4.4/limacharlie.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.4/limacharlie.egg-info/zip-safe
--rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-24 16:29:41.541562 limacharlie-4.4.4/setup.cfg
--rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-24 16:28:54.000000 limacharlie-4.4.4/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-24 16:29:41.540562 limacharlie-4.4.4/tests/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.4/tests/test_artifacts.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.4/tests/test_core.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.4/tests/test_insight.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.4/tests/test_replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.4/tests/test_spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.4/tests/test_sync.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.266409 limacharlie-4.4.5/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.5/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-30 23:57:24.266409 limacharlie-4.4.5/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10845 2023-04-28 15:20:27.000000 limacharlie-4.4.5/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.261409 limacharlie-4.4.5/limacharlie/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.5/limacharlie/Configs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/DRCli.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     5057 2023-04-24 15:42:48.000000 limacharlie-4.4.5/limacharlie/Extensions.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.5/limacharlie/Firehose.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10160 2023-04-24 16:27:39.000000 limacharlie-4.4.5/limacharlie/Hive.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/Jobs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.5/limacharlie/Logs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    52973 2023-04-30 23:56:52.000000 limacharlie-4.4.5/limacharlie/Manager.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/Payloads.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.5/limacharlie/Query.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.5/limacharlie/Replay.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.5/limacharlie/Replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.5/limacharlie/Search.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.5/limacharlie/Sensor.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.5/limacharlie/SpotCheck.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.5/limacharlie/Spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.5/limacharlie/Sync.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/Webhook.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-30 23:56:52.000000 limacharlie-4.4.5/limacharlie/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16201 2023-04-30 23:56:52.000000 limacharlie-4.4.5/limacharlie/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.5/limacharlie/utils.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.263409 limacharlie-4.4.5/limacharlie.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.5/limacharlie.egg-info/zip-safe
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-30 23:57:24.267409 limacharlie-4.4.5/setup.cfg
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-30 23:56:52.000000 limacharlie-4.4.5/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.266409 limacharlie-4.4.5/tests/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_artifacts.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.5/tests/test_core.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_insight.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.5/tests/test_sync.py
```

### Comparing `limacharlie-4.4.4/LICENSE` & `limacharlie-4.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/README.md` & `limacharlie-4.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -242,8 +242,12 @@
 
 #### Detection & Response
 `limacharlie dr --help`
 Shortcut utility to manage Detection and Response rules over the CLI.
 
 #### Events & Detections
 `limacharlie events --help` and `limacharlie detections --help`
-Print out to STDOUT events or detections matching the parameter.
+Print out to STDOUT events or detections matching the parameter.
+
+#### List Sensors
+`limacharlie sensors 'plat == windows'`
+Print out all basic sensor information for all sensors matching the selector.
```

### Comparing `limacharlie-4.4.4/limacharlie/Configs.py` & `limacharlie-4.4.5/limacharlie/Configs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/DRCli.py` & `limacharlie-4.4.5/limacharlie/DRCli.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Extensions.py` & `limacharlie-4.4.5/limacharlie/Extensions.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Firehose.py` & `limacharlie-4.4.5/limacharlie/Firehose.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Hive.py` & `limacharlie-4.4.5/limacharlie/Hive.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Jobs.py` & `limacharlie-4.4.5/limacharlie/Jobs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Logs.py` & `limacharlie-4.4.5/limacharlie/Logs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Manager.py` & `limacharlie-4.4.5/limacharlie/Manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,36 +365,45 @@
         s = Sensor( self, sid )
         if inv_id is not None:
             s.setInvId( inv_id )
         elif self._inv_id is not None:
             s.setInvId( self._inv_id )
         return s
 
-    def sensors( self, inv_id = None, selector = None ):
+    def sensors( self, inv_id = None, selector = None, limit = None, with_ip = None, with_hostname_prefix = None ):
         '''Gets all Sensors in the Organization.
 
         The sensors may or may not be online.
 
         Args:
             inv_id (str): investigation ID to add to all actions done using these objects.
             selector (str): sensor selector expression to use as filter.
+            limit (int): max number of sensors per page of result.
+            with_ip (str): list sensors with the specific internal or external ip.
+            with_hostname_prefix (str): list sensors with the specific hostname prefix.
 
         Returns:
             a generator of Sensor objects.
         '''
 
         continuationToken = None
 
         while True:
             params = {}
 
             if continuationToken is not None:
                 params[ 'continuation_token' ] = continuationToken
             if selector is not None:
                 params[ 'selector' ] = selector
+            if limit is not None:
+                params[ 'limit' ] = limit
+            if with_ip is not None:
+                params[ 'with_ip' ] = with_ip
+            if with_hostname_prefix is not None:
+                params[ 'with_hostname_prefix' ] = with_hostname_prefix
 
             resp = self._apiCall( 'sensors/%s' % self._oid, GET, queryParams = params )
             if inv_id is None:
                 inv_id = self._inv_id
 
             for s in resp[ 'sensors' ]:
                 yield self.sensor( s[ 'sid' ], inv_id )
```

### Comparing `limacharlie-4.4.4/limacharlie/Payloads.py` & `limacharlie-4.4.5/limacharlie/Payloads.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Query.py` & `limacharlie-4.4.5/limacharlie/Query.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Replay.py` & `limacharlie-4.4.5/limacharlie/Replay.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Replicants.py` & `limacharlie-4.4.5/limacharlie/Replicants.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Search.py` & `limacharlie-4.4.5/limacharlie/Search.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Sensor.py` & `limacharlie-4.4.5/limacharlie/Sensor.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/SpotCheck.py` & `limacharlie-4.4.5/limacharlie/SpotCheck.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Spout.py` & `limacharlie-4.4.5/limacharlie/Spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Sync.py` & `limacharlie-4.4.5/limacharlie/Sync.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/Webhook.py` & `limacharlie-4.4.5/limacharlie/Webhook.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie/__init__.py` & `limacharlie-4.4.5/limacharlie/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """limacharlie API for limacharlie.io"""
 
-__version__ = "4.4.4"
+__version__ = "4.4.5"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 # Global API Credentials
 import os
```

### Comparing `limacharlie-4.4.4/limacharlie/__main__.py` & `limacharlie-4.4.5/limacharlie/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     import argparse
     import getpass
     import uuid
     import sys
     import stat
     import os
     import yaml
+    import time
 
     parser = argparse.ArgumentParser( prog = 'limacharlie' )
     parser.add_argument( 'action',
                          type = str,
                          help = 'management action, currently supported "login" (store credentials), "use" (use specific credentials), "dr" (manage Detection & Response rules), "search" (search for Indicators of Compromise), "replay" (replay D&R rules on data), "sync" (synchronize configurations from/to an org), "who" get current SDK authentication in effect, "detections" (download detections), "events" (download events), "artifacts" (get or upload artifacts)' )
     parser.add_argument( 'opt_arg',
                          type = str,
@@ -280,12 +281,66 @@
                     sensor.tag( tag, ttl = args.ttl )
                     print( "done" )
                 else:
                     print( "removing tag %s from sensor %s..." % ( tag, sensor.sid ) )
                     sensor.untag( tag )
                     print( "done" )
         print( "all done" )
+    elif args.action.lower() == 'sensors':
+        from . import Manager
+        import json
+        parser = argparse.ArgumentParser( prog = 'limacharlie sensors' )
+        parser.add_argument( '--selector',
+                             default = None,
+                             type = str,
+                             dest = 'sensor_selector',
+                             help = 'sensor selector expression.' )
+        parser.add_argument( '--limit',
+                             type = int,
+                             default = None,
+                             dest = 'limit',
+                             help = 'limit number of result per underlying query.' )
+        parser.add_argument( '--with-ip',
+                             type = str,
+                             default = None,
+                             dest = 'with_ip',
+                             help = 'list sensors with the given internal or external ip.' )
+        parser.add_argument( '--with-hostname-prefix',
+                             type = str,
+                             default = None,
+                             dest = 'with_hostname_prefix',
+                             help = 'list sensors with the given hostname prefix.' )
+        args = parser.parse_args( sys.argv[ 2: ] )
+        _man = Manager()
+        for sensor in _man.sensors( selector = args.sensor_selector, limit = args.limit, with_ip = args.with_ip, with_hostname_prefix = args.with_hostname_prefix ):
+            print( json.dumps( sensor.getInfo(), indent = 2 ) )
+    elif args.action.lower() == 'sensors_with_ip':
+        from . import Manager
+        import json
+        parser = argparse.ArgumentParser( prog = 'limacharlie sensors_with_ip' )
+        parser.add_argument( 'ip',
+                             type = str,
+                             help = 'IP address to look for.' )
+        parser.add_argument( '--start',
+                             type = int,
+                             default = None,
+                             dest = 'start',
+                             help = 'optional start second epoch.' )
+        parser.add_argument( '--end',
+                             type = int,
+                             default = None,
+                             dest = 'end',
+                             help = 'optional end second epoch.' )
+        args = parser.parse_args( sys.argv[ 2: ] )
+        _man = Manager()
+        if args.start is not None and args.end is not None:
+            start = args.start
+            end = args.end
+        else:
+            start = int(time.time() - (4*60*60))
+            end = int(time.time())
+        print( json.dumps( _man.getSensorsWithIp( args.ip, start, end ), indent = 2 ) )
     else:
         raise Exception( 'invalid action' )
 
 if __name__ == "__main__":
     main()
```

### Comparing `limacharlie-4.4.4/limacharlie/utils.py` & `limacharlie-4.4.5/limacharlie/utils.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/limacharlie.egg-info/SOURCES.txt` & `limacharlie-4.4.5/limacharlie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/setup.py` & `limacharlie-4.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "4.4.4"
+__version__ = "4.4.5"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 setup( name = 'limacharlie',
        version = __version__,
```

### Comparing `limacharlie-4.4.4/tests/test_artifacts.py` & `limacharlie-4.4.5/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/tests/test_core.py` & `limacharlie-4.4.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/tests/test_insight.py` & `limacharlie-4.4.5/tests/test_insight.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/tests/test_spout.py` & `limacharlie-4.4.5/tests/test_spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.4/tests/test_sync.py` & `limacharlie-4.4.5/tests/test_sync.py`

 * *Files identical despite different names*

