# Comparing `tmp/optumi-api-3.15.6.tar.gz` & `tmp/optumi-api-3.15.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.15.6.tar", last modified: Thu Apr 20 17:47:32 2023, max compression
+gzip compressed data, was "optumi-api-3.15.7.tar", last modified: Fri Apr 28 23:43:25 2023, max compression
```

## Comparing `optumi-api-3.15.6.tar` & `optumi-api-3.15.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-04-20 17:47:32.071957 optumi-api-3.15.6/
--rw-rw-r--   0 jj        (1001) jj        (1001)      281 2023-04-17 18:17:12.000000 optumi-api-3.15.6/LICENSE
--rw-rw-r--   0 jj        (1001) jj        (1001)       58 2023-04-17 18:17:12.000000 optumi-api-3.15.6/MANIFEST.in
--rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-04-20 17:47:32.071957 optumi-api-3.15.6/PKG-INFO
--rw-rw-r--   0 jj        (1001) jj        (1001)      422 2023-04-17 18:17:12.000000 optumi-api-3.15.6/README.md
--rw-rw-r--   0 jj        (1001) jj        (1001)      322 2023-04-20 17:47:31.000000 optumi-api-3.15.6/core_version.py
-drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-04-20 17:47:32.071957 optumi-api-3.15.6/optumi_api/
--rw-rw-r--   0 jj        (1001) jj        (1001)     2883 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/CloudFile.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3677 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/CloudFileVersion.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     5148 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/CloudStorage.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3977 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Colab.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     5352 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Container.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     4402 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/ContainerRegistry.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     4179 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/EnvironmentVariables.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6563 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Executable.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1006 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/HoldoverTime.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3070 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/LocalFile.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     2401 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/LocalStorage.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1515 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Log.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6290 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/LoginServer.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6763 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Machine.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1956 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Machines.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      723 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Notebook.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     6568 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/NotebookConfig.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     2472 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Notifications.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      818 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Packages.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1620 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Program.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     5284 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Provider.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1359 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Providers.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3281 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Resource.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      696 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Script.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     4135 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Server.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1968 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Summary.py
--rw-rw-r--   0 jj        (1001) jj        (1001)    20470 2023-04-19 20:20:54.000000 optumi-api-3.15.6/optumi_api/Workload.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     3107 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Workloads.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      838 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/__init__.py
--rw-rw-r--   0 jj        (1001) jj        (1001)      323 2023-04-20 14:07:13.000000 optumi-api-3.15.6/optumi_api/_version.py
--rw-rw-r--   0 jj        (1001) jj        (1001)    11309 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/api.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1418 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/cli.py
--rw-rw-r--   0 jj        (1001) jj        (1001)     1786 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/utils.py
-drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-04-20 17:47:32.071957 optumi-api-3.15.6/optumi_api.egg-info/
--rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/PKG-INFO
--rw-rw-r--   0 jj        (1001) jj        (1001)     1086 2023-04-20 17:47:32.000000 optumi-api-3.15.6/optumi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)       47 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/entry_points.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/not-zip-safe
--rw-rw-r--   0 jj        (1001) jj        (1001)       41 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/requires.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)       11 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/top_level.txt
--rw-rw-r--   0 jj        (1001) jj        (1001)       38 2023-04-20 17:47:32.071957 optumi-api-3.15.6/setup.cfg
--rwxrwxr-x   0 jj        (1001) jj        (1001)     2612 2023-04-17 18:17:12.000000 optumi-api-3.15.6/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:25.357160 optumi-api-3.15.7/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-04-27 13:56:16.000000 optumi-api-3.15.7/LICENSE
+-rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-04-27 13:56:16.000000 optumi-api-3.15.7/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-28 23:43:25.357160 optumi-api-3.15.7/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-27 13:56:16.000000 optumi-api-3.15.7/README.md
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-28 23:43:25.000000 optumi-api-3.15.7/core_version.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:25.357160 optumi-api-3.15.7/optumi_api/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2883 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/CloudFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3677 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/CloudFileVersion.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5171 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/CloudStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4029 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Colab.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5352 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Container.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4402 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/ContainerRegistry.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/EnvironmentVariables.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6574 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Executable.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1006 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/HoldoverTime.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/LocalFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2402 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/LocalStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1515 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Log.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6281 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/LoginServer.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6734 2023-04-28 13:25:45.000000 optumi-api-3.15.7/optumi_api/Machine.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1957 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Machines.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Notebook.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6568 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/NotebookConfig.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2487 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Notifications.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      819 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Packages.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1620 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Program.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Provider.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1360 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Providers.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3283 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Resource.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Script.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4168 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Server.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1968 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Summary.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    20469 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Workload.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3108 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Workloads.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    11309 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/api.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/cli.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3523 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/utils.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:25.357160 optumi-api-3.15.7/optumi_api.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/entry_points.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)       41 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-28 23:43:25.357160 optumi-api-3.15.7/setup.cfg
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     2612 2023-04-27 13:56:16.000000 optumi-api-3.15.7/setup.py
```

### Comparing `optumi-api-3.15.6/PKG-INFO` & `optumi-api-3.15.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.6
+Version: 3.15.7
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.6/optumi_api/CloudFile.py` & `optumi-api-3.15.7/optumi_api/CloudFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/CloudFileVersion.py` & `optumi-api-3.15.7/optumi_api/CloudFileVersion.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/CloudStorage.py` & `optumi-api-3.15.7/optumi_api/CloudStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import optumi_core as optumi
 
 from .CloudFile import CloudFile
 from .CloudFileVersion import CloudFileVersion
 
 import json, datetime, time
+from uuid import uuid4
 
 from pathlib import Path
 
 from typing import List
 
 
 # Support downloading object under a different name
```

### Comparing `optumi-api-3.15.6/optumi_api/Colab.py` & `optumi-api-3.15.7/optumi_api/Colab.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .LocalStorage import LocalStorage
 from .Server import Server
 from .Resource import Resource
 from .Workload import Workload
 from .EnvironmentVariables import EnvironmentVariables
 from .Notifications import Notifications
 
+from optumi_core.exceptions import OptumiException
+
 import optumi_core as optumi
 
 import os, datetime, json
 from typing import Union, List
 
 
 class Colab:
```

### Comparing `optumi-api-3.15.6/optumi_api/Container.py` & `optumi-api-3.15.7/optumi_api/Container.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/ContainerRegistry.py` & `optumi-api-3.15.7/optumi_api/ContainerRegistry.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/EnvironmentVariables.py` & `optumi-api-3.15.7/optumi_api/EnvironmentVariables.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/Executable.py` & `optumi-api-3.15.7/optumi_api/Executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             program_type (str, optional): The type of the program. Can be one of "python notebook", "python script", "docker container" or "unknown". Defaults to "unknown".
 
         Raises:
             OptumiException: Raised if the program type is not specified properly.
         """
         self._path = optumi.utils.normalize_path(path)
         if not program_type in Executable.program_types:
-            raise OptumiException("Unexpected program type '" + program_type + "', expected one of " + str(program_types))
+            raise OptumiException("Unexpected program type '" + program_type + "', expected one of " + str(Executable.program_types))
         self._program_type = program_type
 
     def __utcnow(self):
         return datetime.datetime.utcnow().isoformat() + "Z"
 
     def launch(
         self,
```

### Comparing `optumi-api-3.15.6/optumi_api/HoldoverTime.py` & `optumi-api-3.15.7/optumi_api/HoldoverTime.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/LocalFile.py` & `optumi-api-3.15.7/optumi_api/LocalFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/LocalStorage.py` & `optumi-api-3.15.7/optumi_api/LocalStorage.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -66,8 +66,8 @@
                     time.sleep(0.2)
                     if progress[key]["progress"] < 0:
                         break
 
                 print("...completed")
 
     def __str__(self):
-        return str([str(x) for x in self])
+        return str([str(x) for x in self])
```

### Comparing `optumi-api-3.15.6/optumi_api/Log.py` & `optumi-api-3.15.7/optumi_api/Log.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/LoginServer.py` & `optumi-api-3.15.7/optumi_api/LoginServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## You may only use this code under license with Optumi Inc and any distribution or modification is strictly prohibited.
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at https://www.optumi.com.
 ##
 
 from ._version import __version__
 
 import json, time, os, base64, re, hashlib, random, requests, webbrowser
-from urllib import request, parse
+from urllib import parse
 import tornado.httpserver
 import tornado.ioloop
 import tornado.web
 
 from optumi_core.logging import optumi_format_and_log
 from optumi_core.utils import dev_version
```

### Comparing `optumi-api-3.15.6/optumi_api/Machine.py` & `optumi-api-3.15.7/optumi_api/Machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             promo (bool): Whether this machine is being given a promotional rate or not.
             app (str): The application name of the workload being executed on this machine.
             state (str): The current state of this machine, one of "Acquiring", "Configuring", "Busy", "Idle" or "Releasing"
         """
         self._uuid = uuid
         self._size = size
         self._dns_name = dns_name
-        self._rate = "$" + str(round(rate, 2)) + "/hr"
+        self._rate = rate
         self._promo = promo
         self._app = app
         self._state = state
         self._last_refresh = time.time()
 
     @classmethod
     def reconstruct(cls, machine_map):
```

### Comparing `optumi-api-3.15.6/optumi_api/Machines.py` & `optumi-api-3.15.7/optumi_api/Machines.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -50,8 +50,8 @@
         response = json.loads(optumi.core.get_machines().text)
 
         for machine in response["machines"]:
             machine = Machine(*Machine.reconstruct(machine))
             if (status is None and machine.is_visible()) or (machine.status == status):
                 machines.append(machine)
 
-        return Machines(machines)
+        return Machines(machines)
```

### Comparing `optumi-api-3.15.6/optumi_api/Notebook.py` & `optumi-api-3.15.7/optumi_api/Notebook.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/NotebookConfig.py` & `optumi-api-3.15.7/optumi_api/NotebookConfig.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/Notifications.py` & `optumi-api-3.15.7/optumi_api/Notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
         Returns:
             bool: True if "job completed" notifications are enabled, False if not.
         """
         return self._job_completed
 
     def __str__(self):
-        return "job_started=" + str(job_started) + ", job_failed=" + str(job_failed) + ", job_completed=" + str(job_completed)
+        return "job_started=" + str(self.job_started) + ", job_failed=" + str(self.job_failed) + ", job_completed=" + str(self.job_completed)
```

### Comparing `optumi-api-3.15.6/optumi_api/Packages.py` & `optumi-api-3.15.7/optumi_api/Packages.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
         Args:
             packages (list of str, optional): List of packages to install before running a workload. Defaults to [].
         """
         super().__init__(packages)
 
     def __str__(self):
-        return str(self.packages)
+        return str(self.packages)
```

### Comparing `optumi-api-3.15.6/optumi_api/Program.py` & `optumi-api-3.15.7/optumi_api/Program.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/Provider.py` & `optumi-api-3.15.7/optumi_api/Provider.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/Providers.py` & `optumi-api-3.15.7/optumi_api/Providers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 
         user_information = json.loads(optumi.core.get_user_information(True).text)
 
         for provider in user_information["providers"]:
             provider = Provider(*Provider.reconstruct(provider))
             providers.append(provider)
 
-        return providers
+        return providers
```

### Comparing `optumi-api-3.15.6/optumi_api/Resource.py` & `optumi-api-3.15.7/optumi_api/Resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ##
 ## You may only use this code under license with Optumi Inc and any distribution or modification is strictly prohibited.
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at https://www.optumi.com.
 ##
 
 from .Server import Server
 from .Provider import Provider
-from .Provider import Provider
+from .Providers import Providers
 
 from typing import Union, List
 
 from optumi_core.exceptions import (
     OptumiException,
 )
```

### Comparing `optumi-api-3.15.6/optumi_api/Script.py` & `optumi-api-3.15.7/optumi_api/Script.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/Server.py` & `optumi-api-3.15.7/optumi_api/Server.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ## Copyright (C) Optumi Inc - All rights reserved.
 ##
 ## You may only use this code under license with Optumi Inc and any distribution or modification is strictly prohibited.
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at https://www.optumi.com.
 ##
 
 from .Provider import Provider
+from .Providers import Providers
 
 import optumi_core as optumi
 from optumi_core.exceptions import OptumiException
 
 import json
 
 _machines = None
```

### Comparing `optumi-api-3.15.6/optumi_api/Summary.py` & `optumi-api-3.15.7/optumi_api/Summary.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/Workload.py` & `optumi-api-3.15.7/optumi_api/Workload.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,14 @@
                 optumi.core.stop_notebook(self._workload_uuid)
                 if wait and self.status == "running":
                     self.wait(progress="silent")
                 print("...completed")
             else:
                 print("Workload not running")
 
-
     def remove(self, wait: bool = True):
         """Remove the current workload."""
         if self.status != "completed":
             self.stop(wait)
         print("Removing workload " + self.name + "...")
         optumi.core.teardown_notebook(self._workload_uuid)
         print("...completed")
```

### Comparing `optumi-api-3.15.6/optumi_api/Workloads.py` & `optumi-api-3.15.7/optumi_api/Workloads.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,8 @@
         # Add apps from user information if they don't already exist
         if "jobs" in user_information:
             for app_map in user_information["jobs"]:
                 for module in app_map["modules"]:
                     if module["uuid"] == os.environ["OPTUMI_MOD"]:
                         return Workload.reconstruct(app_map)
 
-        raise OptumiException("No current workload")
+        raise OptumiException("No current workload")
```

### Comparing `optumi-api-3.15.6/optumi_api/__init__.py` & `optumi-api-3.15.7/optumi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/api.py` & `optumi-api-3.15.7/optumi_api/api.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api/cli.py` & `optumi-api-3.15.7/optumi_api/cli.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/optumi_api.egg-info/PKG-INFO` & `optumi-api-3.15.7/optumi_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.6
+Version: 3.15.7
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.6/optumi_api.egg-info/SOURCES.txt` & `optumi-api-3.15.7/optumi_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.6/setup.py` & `optumi-api-3.15.7/setup.py`

 * *Files identical despite different names*

