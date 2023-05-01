# Comparing `tmp/microgue-1.0.9.tar.gz` & `tmp/microgue-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microgue-1.0.9.tar", last modified: Sat Apr 29 02:01:29 2023, max compression
+gzip compressed data, was "dist/microgue-2.0.0.tar", last modified: Mon May  1 14:35:37 2023, max compression
```

## Comparing `microgue-1.0.9.tar` & `microgue-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3017 2023-04-29 02:01:29.000000 microgue-1.0.9/PKG-INFO
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/storages/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/storages/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     3371 2022-09-23 01:04:52.000000 microgue-1.0.9/microgue/storages/abstract_storage.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/loggers/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/loggers/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1713 2023-04-29 01:51:16.000000 microgue-1.0.9/microgue/loggers/logger.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/security/
--rw-r--r--   0 mhudelso   (501) staff       (20)      343 2022-09-21 19:42:33.000000 microgue-1.0.9/microgue/security/generic.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/security/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/secrets/
--rw-r--r--   0 mhudelso   (501) staff       (20)      175 2022-09-21 19:42:32.000000 microgue-1.0.9/microgue/secrets/secrets_without_logging.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/secrets/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1213 2022-09-21 19:42:32.000000 microgue-1.0.9/microgue/secrets/secrets.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/constants/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/constants/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-1.0.9/microgue/constants/error_constants.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/objects/
--rw-r--r--   0 mhudelso   (501) staff       (20)     8636 2022-09-23 01:14:06.000000 microgue-1.0.9/microgue/objects/abstract_model_object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2374 2022-09-23 00:54:22.000000 microgue-1.0.9/microgue/objects/object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/objects/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1458 2022-09-23 00:49:49.000000 microgue-1.0.9/microgue/objects/abstract_expiring_model_object.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/models/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/models/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)    10587 2022-09-23 00:48:36.000000 microgue-1.0.9/microgue/models/abstract_model.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2682 2022-12-09 19:59:12.000000 microgue-1.0.9/microgue/utils.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/queues/
--rw-r--r--   0 mhudelso   (501) staff       (20)     2908 2022-09-23 01:15:31.000000 microgue-1.0.9/microgue/queues/abstract_queue.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/queues/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/events/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-1.0.9/microgue/events/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1442 2022-09-22 23:03:47.000000 microgue-1.0.9/microgue/events/abstract_event_bus.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     5526 2022-12-30 17:34:34.000000 microgue-1.0.9/microgue/abstract_app.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/services/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3317 2022-12-19 21:35:09.000000 microgue-1.0.9/microgue/services/service.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/services/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue/caches/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3043 2022-09-21 19:29:03.000000 microgue-1.0.9/microgue/caches/abstract_cache.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-1.0.9/microgue/caches/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-1.0.9/README.md
--rw-r--r--   0 mhudelso   (501) staff       (20)      597 2023-04-29 01:59:45.000000 microgue-1.0.9/setup.py
--rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-04-29 02:01:29.000000 microgue-1.0.9/setup.cfg
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3017 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/PKG-INFO
--rw-r--r--   0 mhudelso   (501) staff       (20)     1054 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/SOURCES.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/requires.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/top_level.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-04-29 02:01:29.000000 microgue-1.0.9/microgue.egg-info/dependency_links.txt
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-01 14:35:37.000000 microgue-2.0.0/PKG-INFO
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/storages/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/storages/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3324 2023-04-30 02:26:31.000000 microgue-2.0.0/microgue/storages/abstract_storage.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/loggers/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/loggers/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1381 2023-05-01 14:32:34.000000 microgue-2.0.0/microgue/loggers/logger.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/security/
+-rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.0/microgue/security/generic.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/security/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/secrets/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/secrets/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)      998 2023-04-30 02:26:31.000000 microgue-2.0.0/microgue/secrets/secrets.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/constants/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/constants/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.0/microgue/constants/error_constants.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/objects/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     8626 2023-04-29 23:27:06.000000 microgue-2.0.0/microgue/objects/abstract_model_object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2374 2022-09-23 00:54:22.000000 microgue-2.0.0/microgue/objects/object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/objects/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1459 2023-04-30 02:26:31.000000 microgue-2.0.0/microgue/objects/abstract_expiring_model_object.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/models/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/models/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)    10541 2023-04-30 02:26:31.000000 microgue-2.0.0/microgue/models/abstract_model.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2682 2022-12-09 19:59:12.000000 microgue-2.0.0/microgue/utils.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/queues/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2864 2023-04-30 17:37:32.000000 microgue-2.0.0/microgue/queues/abstract_queue.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/queues/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/events/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.0/microgue/events/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1420 2023-04-30 02:26:31.000000 microgue-2.0.0/microgue/events/abstract_event_bus.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     5204 2023-05-01 13:49:41.000000 microgue-2.0.0/microgue/abstract_app.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/services/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3687 2023-05-01 14:01:58.000000 microgue-2.0.0/microgue/services/service.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/services/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue/caches/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3015 2023-04-30 02:26:31.000000 microgue-2.0.0/microgue/caches/abstract_cache.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.0/microgue/caches/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.0/README.md
+-rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-01 14:35:18.000000 microgue-2.0.0/setup.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-01 14:35:37.000000 microgue-2.0.0/setup.cfg
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue.egg-info/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue.egg-info/PKG-INFO
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue.egg-info/SOURCES.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue.egg-info/requires.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue.egg-info/top_level.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-01 14:35:37.000000 microgue-2.0.0/microgue.egg-info/dependency_links.txt
```

### Comparing `microgue-1.0.9/PKG-INFO` & `microgue-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 1.0.9
-Summary: Quickly spin up microservices in AWS using flask
+Version: 2.0.0
+Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
         
         This project contains bootstrap code to speed up the development of AWS based microservices
```

### Comparing `microgue-1.0.9/microgue/storages/abstract_storage.py` & `microgue-2.0.0/microgue/storages/abstract_storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 import boto3
-import logging
 import os
 import uuid
 from pathlib import Path
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
-class DownloadFailed(Exception):
-    pass
-
-
-class UploadFailed(Exception):
-    pass
-
-
-class DeleteFailed(Exception):
-    pass
+class DownloadFailed(Exception): pass
+class UploadFailed(Exception): pass
+class DeleteFailed(Exception): pass
 
 
 class AbstractStorage:
     class File:
         def __init__(self, remote_path=None, local_path=None, url=None):
             self.remote_path = remote_path
             self.local_path = local_path
             self.url = url
 
     storage = None
     bucket_name = ""
     bucket_public_url = ""
 
     def __init__(self, *args, **kwargs):
-        logger.debug(f"########## {self.__class__.__name__} __init__ ##########")
+        logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractStorage.storage: {AbstractStorage.storage}")
         if AbstractStorage.storage is None:
             logger.debug("connecting to s3")
             AbstractStorage.storage = boto3.client("s3")
         else:
             logger.debug("using existing connection to s3")
 
     def upload(self, local_file_path, remote_file_path=None):
         if remote_file_path is None:
             remote_file_path = str(uuid.uuid4()) + "-" + local_file_path.split("/")[-1]
 
-        logger.debug(f"########## {self.__class__.__name__} Upload ##########")
+        logger.debug(f"{self.__class__.__name__}.upload", priority=2)
         logger.debug(f"local_file_path: {local_file_path}")
         logger.debug(f"remote_file_path: {remote_file_path}")
 
         try:
             self.storage.upload_file(local_file_path, self.bucket_name, remote_file_path)
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Upload Error")
+            logger.error(f"{self.__class__.__name__}.upload - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise UploadFailed(str(e))
 
         return self.File(
             remote_path=remote_file_path,
             local_path=local_file_path,
             url=self.bucket_public_url + "/" + remote_file_path
@@ -63,36 +56,36 @@
     def download(self, remote_file_path, local_file_path=None):
         if local_file_path is None:
             local_file_path = os.getcwd() + "/" + remote_file_path
 
         # ensure local_file_path directories exist
         Path(os.path.dirname(local_file_path)).mkdir(parents=True, exist_ok=True)
 
-        logger.debug(f"########## {self.__class__.__name__} Download ##########")
+        logger.debug(f"{self.__class__.__name__}.download", priority=2)
         logger.debug(f"remote_file_path: {remote_file_path}")
         logger.debug(f"local_file_path: {local_file_path}")
 
         try:
             self.storage.download_file(self.bucket_name, remote_file_path, local_file_path)
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Download Error")
+            logger.error(f"{self.__class__.__name__}.download - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise DownloadFailed(str(e))
 
         return self.File(
             remote_path=remote_file_path,
             local_path=local_file_path,
             url=self.bucket_public_url + "/" + remote_file_path
         )
 
     def delete(self, remote_file_path):
-        logger.debug(f"########## {self.__class__.__name__} Delete ##########")
+        logger.debug(f"{self.__class__.__name__}.delete", priority=2)
         logger.debug(f"remote_file_path: {remote_file_path}")
 
         try:
             self.storage.delete_object(Bucket=self.bucket_name, Key=remote_file_path)
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Delete Error")
+            logger.error(f"{self.__class__.__name__}.delete - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise DeleteFailed(str(e))
 
         return True
```

### Comparing `microgue-1.0.9/microgue/loggers/logger.py` & `microgue-2.0.0/microgue/loggers/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 import logging
 import uuid
 
 
 class Logger:
-    trace_id = None
-    _instance = None
+    __instance = None
+    logger = None
 
-    def __new__(cls, name=None, level=logging.DEBUG, trace_id=None, *args, **kwargs):
-        if not cls._instance:
-            logging.basicConfig()
-            cls._instance = super().__new__(cls)
-            cls._instance.__logger = logging.getLogger(name)
-            cls._instance.__logger.setLevel(level)
-            cls._instance.trace_id = uuid.uuid4()
-        return cls._instance
-
-    def start_trace(self, trace_id=None):
-        if trace_id:
-            self.trace_id = trace_id
-        else:
-            self.trace_id = uuid.uuid4()
+    def __new__(cls, name=None, level=logging.DEBUG, *args, **kwargs):
+        if not cls.__instance:
+            cls.__instance = super().__new__(cls)
+            cls.__instance.logger = logging.getLogger(name)
+            cls.__instance.logger.setLevel(level)
+        return cls.__instance
 
     def debug(self, message, priority=None):
         self.log(message, priority=priority, level=logging.DEBUG)
 
     def info(self, message, priority=None):
         self.log(message, priority=priority, level=logging.INFO)
 
@@ -34,14 +26,14 @@
         self.log(message, priority=priority, level=logging.WARNING)
 
     def critical(self, message, priority=None):
         self.log(message, priority=priority, level=logging.CRITICAL)
 
     def log(self, message, priority=None, level=logging.DEBUG):
         if priority == 1:
-            self.__logger.log(level, f"{self.trace_id} ########## {message} ########################################")
+            self.logger.log(level, f"########## {message} ########################################")
         elif priority == 2:
-            self.__logger.log(level, f"{self.trace_id} ########## {message} ##########")
+            self.logger.log(level, f"########## {message} ##########")
         elif priority == 3:
-            self.__logger.log(level, f"{self.trace_id} ########## {message}")
+            self.logger.log(level, f"########## {message}")
         else:
-            self.__logger.log(level, f"{self.trace_id} {message}")
+            self.logger.log(level, message)
```

### Comparing `microgue-1.0.9/microgue/objects/abstract_model_object.py` & `microgue-2.0.0/microgue/objects/abstract_model_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import uuid
 from ..models.abstract_model import *
 from .object import *
 
 
-class RequiredAttributes(Exception):
-    pass
-
-
-class UniqueAttributes(Exception):
-    pass
+class RequiredAttributes(Exception): pass
+class UniqueAttributes(Exception): pass
 
 
 class AbstractModelObject(Object):
     """
     attributes: defined on Object
 
     hidden_attributes: defined on Object
```

### Comparing `microgue-1.0.9/microgue/objects/object.py` & `microgue-2.0.0/microgue/objects/object.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.9/microgue/objects/abstract_expiring_model_object.py` & `microgue-2.0.0/microgue/objects/abstract_expiring_model_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import datetime
-import logging
 import time
 from .abstract_model_object import *
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
 class AbstractExpiringModelObject(AbstractModelObject):
     expiration_seconds = 0
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.expires_in and self.expires_in < int(time.mktime(datetime.datetime.utcnow().timetuple())):
-            logger.debug(f"########## {self.__class__.__name__} Expired ##########")
+            logger.debug(f"{self.__class__.__name__}.__init__ - expired", priority=2)
             raise GetFailed("item expired")
 
     def insert(self):
         # add expires_in
         expires_in = datetime.datetime.utcnow() + datetime.timedelta(seconds=self.expiration_seconds)
         self.expires_in = int((expires_in - datetime.datetime(1970, 1, 1)).total_seconds())
         super().insert()
```

### Comparing `microgue-1.0.9/microgue/models/abstract_model.py` & `microgue-2.0.0/microgue/models/abstract_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import boto3
 import datetime
-import logging
 import uuid
 from boto3.dynamodb.conditions import Key
 from boto3.dynamodb.types import Decimal
 from ..utils import mask_fields_in_data
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
 class DatabaseConnectionFailed(Exception): pass
 class DeleteFailed(Exception): pass
 class GetFailed(Exception): pass
 class ItemAlreadyExists(Exception): pass
 class MissingKey(Exception): pass
@@ -47,55 +47,55 @@
     auto_generate_sk = True
 
     indexes = {}
 
     mask_attributes = []
 
     def __init__(self, *args, **kwargs):
-        logger.debug(f"########## {self.__class__.__name__} __init__ ##########")
+        logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractModel.database: {AbstractModel.database}")
         try:
             if AbstractModel.database is None:
                 logger.debug("connecting to dynamodb")
                 AbstractModel.database = boto3.resource("dynamodb")
             else:
                 logger.debug("using existing connection to dynamodb")
 
             self.table = AbstractModel.database.Table(self.table_name)
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Error")
+            logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise DatabaseConnectionFailed(str(e))
         super().__init__(*args, **kwargs)
 
     def get(self, pk_value, sk_value=None):
-        logger.debug(f"########## {self.__class__.__name__} Get ##########")
+        logger.debug(f"{self.__class__.__name__}.get", priority=2)
         logger.debug(f"{self.pk}: {pk_value}")
         if self.sk:
             logger.debug(f"{self.sk}: {sk_value}")
 
         # create key based on presence of pk and sk
         key = {self.pk: pk_value}
         if self.sk:
             key[self.sk] = sk_value
 
         try:
             item = self.table.get_item(Key=key)["Item"]
         except Exception as e:
-            logger.debug(f"########## {self.__class__.__name__} Get Failed")
+            logger.debug(f"{self.__class__.__name__}.get - failed", priority=3)
             logger.debug(f"{e.__class__.__name__}: {str(e)}")
             raise GetFailed("failed to get item")
 
         logger.debug(f"return: {mask_fields_in_data(item, self.mask_attributes)}")
 
         return self.__replace_decimals(item)
 
     def insert(self, item):
         item = item.copy()
-        logger.debug(f"########## {self.__class__.__name__} Insert ##########")
+        logger.debug(f"{self.__class__.__name__}.insert", priority=2)
         logger.debug(f"item: {mask_fields_in_data(item, self.mask_attributes)}")
 
         # add created on to item
         item["created_on"] = datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
 
         # check if pk should be generated or if an error should be raise
         if item.get(self.pk) is None:
@@ -119,29 +119,29 @@
         try:
             # convert floats to decimals for sending to dynamodb
             self.table.put_item(
                 Item=self.__replace_floats(item),
                 ConditionExpression=condition_expression
             )
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Insert Error")
+            logger.error(f"{self.__class__.__name__}.insert - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             if self.sk:
                 error = f"{self.pk} and {self.sk} key combo ({item[self.pk]} and {item[self.sk]}) already exists"
             else:
                 error = f"{self.pk} ({item[self.pk]}) already exists"
             raise ItemAlreadyExists(error)
 
         logger.debug(f"return: {mask_fields_in_data(item, self.mask_attributes)}")
 
         return self.__replace_decimals(item)
 
     def update(self, updated_item):
         updated_item = updated_item.copy()
-        logger.debug(f"########## {self.__class__.__name__} Update ##########")
+        logger.debug(f"{self.__class__.__name__}.update", priority=2)
         logger.debug(f"updated_item: {mask_fields_in_data(updated_item, self.mask_attributes)}")
 
         # convert floats to decimals for sending to dynamodb
         updated_item = self.__replace_floats(updated_item)
 
         # verify the pk exists
         if self.pk and not updated_item.get(self.pk):
@@ -172,50 +172,50 @@
             item = self.table.update_item(
                 Key=key,
                 UpdateExpression="set {}".format(", ".join(update_expressions)),
                 ExpressionAttributeValues=expression_attribute_values,
                 ReturnValues="ALL_NEW"
             )["Attributes"]
         except Exception as e:
-            logger.debug(f"########## {self.__class__.__name__} Update Failed")
+            logger.debug(f"{self.__class__.__name__}.update - failed", priority=3)
             logger.debug(f"{e.__class__.__name__}: {str(e)}")
             raise UpdateFailed("failed to update item")
 
         logger.debug(f"return: {mask_fields_in_data(item, self.mask_attributes)}")
 
         return self.__replace_decimals(item)
 
     def delete(self, pk_value, sk_value=None):
-        logger.debug(f"########## {self.__class__.__name__} Delete ##########")
+        logger.debug(f"{self.__class__.__name__}.delete", priority=2)
         logger.debug(f"{self.pk}: {pk_value}")
         if self.sk:
             logger.debug(f"{self.sk}: {sk_value}")
 
         # create key based on presence of pk and sk
         key = {self.pk: pk_value}
         if self.sk:
             key[self.sk] = sk_value
 
         try:
             self.table.delete_item(Key=key)
         except Exception as e:
-            logger.debug(f"########## {self.__class__.__name__} Delete Failed")
+            logger.debug(f"{self.__class__.__name__}.delete - failed", priority=3)
             logger.debug(f"{e.__class__.__name__}: {str(e)}")
             raise DeleteFailed("failed to delete item")
 
         return True
 
     def get_all_by_pk(self, pk_value):
-        logger.debug(f"########## {self.__class__.__name__} Get All By PK ##########")
+        logger.debug(f"{self.__class__.__name__}.get_all_by_pk", priority=2)
         logger.debug(f"{self.pk}: {pk_value}")
         return self.query(Key(self.pk).eq(pk_value))
 
     def get_all_by_index(self, index, pk_value, sk_value=None):
         pk, sk = self._get_pk_and_sk_for_index(index)
-        logger.debug(f"########## {self.__class__.__name__} Get All By Index ##########")
+        logger.debug(f"{self.__class__.__name__}.get_all_by_index", priority=2)
         logger.debug(f"index: {index}")
         logger.debug(f"{pk}: {pk_value}")
         if sk and sk_value:
             logger.debug(f"{sk}: {sk_value}")
 
         # create key condition expression based on presence of pk and sk for the index
         key_condition_expression = Key(pk).eq(pk_value)
```

### Comparing `microgue-1.0.9/microgue/utils.py` & `microgue-2.0.0/microgue/utils.py`

 * *Files identical despite different names*

### Comparing `microgue-1.0.9/microgue/queues/abstract_queue.py` & `microgue-2.0.0/microgue/queues/abstract_queue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 import boto3
 import json
-import logging
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
-class QueueConnectionFailed(Exception):
-    pass
-
-
-class DeleteFailed(Exception):
-    pass
+class QueueConnectionFailed(Exception): pass
+class DeleteFailed(Exception): pass
 
 
 class AbstractQueue:
     queue = None
     queue_url = ""
 
     def __init__(self, *args, **kwargs):
-        logger.debug(f"########## {self.__class__.__name__} __init__ ##########")
+        logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractQueue.queue: {AbstractQueue.queue}")
         try:
             if AbstractQueue.queue is None:
                 logger.debug("connecting to sqs")
                 AbstractQueue.queue = boto3.client("sqs")
             else:
                 logger.debug("using existing connection to sqs")
         except Exception as e:
             raise QueueConnectionFailed(str(e))
 
     def send(self, message):
-        logger.debug(f"########## {self.__class__.__name__} Send ##########")
+        logger.debug(f"{self.__class__.__name__}.send", priority=2)
         if type(message) is dict:
             message = json.dumps(message)
         try:
             self.queue.send_message(
                 QueueUrl=self.queue_url,
                 MessageBody=message
             )
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Send Failed")
+            logger.error(f"{self.__class__.__name__}.send - failed", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             return False
         return True
 
     def receive(self, max_number_of_messages=1, visibility_timeout=1, wait_time=1):
-        logger.debug(f"########## {self.__class__.__name__} Receive ##########")
+        logger.debug(f"{self.__class__.__name__}.receive", priority=2)
         logger.debug(f"max_number_of_messages: {max_number_of_messages}")
         logger.debug(f"visibility_timeout: {visibility_timeout}")
         logger.debug(f"wait_time: {wait_time}")
         response = self.queue.receive_message(
             QueueUrl=self.queue_url,
             MaxNumberOfMessages=max_number_of_messages,
             VisibilityTimeout=visibility_timeout,
@@ -66,21 +62,21 @@
                 }
                 messages.append(message)
             except:
                 pass
         return messages
 
     def delete(self, message):
-        logger.debug(f"########## {self.__class__.__name__} Delete ##########")
+        logger.debug(f"{self.__class__.__name__}.delete", priority=2)
         logger.debug(f"message: {message}")
 
         try:
             self.queue.delete_message(
                 QueueUrl=self.queue_url,
                 ReceiptHandle=message.get("id")
             )
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Delete Failed")
+            logger.error(f"{self.__class__.__name__}.delete - failed", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise DeleteFailed(str(e))
 
         return True
```

### Comparing `microgue-1.0.9/microgue/events/abstract_event_bus.py` & `microgue-2.0.0/microgue/events/abstract_event_bus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import boto3
 import json
-import logging
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
 class AbstractEventBus:
     event_bus = None
     event_bus_name = None
     event_bus_region = None
     event_source = None
 
     def __init__(self, *args, **kwargs):
-        logger.debug(f"########## {self.__class__.__name__} __init__ ##########")
+        logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractEventBus.event_bus: {AbstractEventBus.event_bus}")
         if AbstractEventBus.event_bus is None:
             logger.debug("connecting to eventbridge")
             AbstractEventBus.event_bus = boto3.client(service_name="events", region_name=self.event_bus_region)
         else:
             logger.debug("using existing connection to eventbridge")
 
     def publish(self, event_type, event_data={}):
-        logger.debug(f"########## {self.__class__.__name__} Publish ##########")
+        logger.debug(f"{self.__class__.__name__}.publish", priority=2)
         logger.debug(f"event_type: {event_type}")
         logger.debug(f"event_data: {event_data}")
 
         response = self.event_bus.put_events(
             Entries=[{
                 "Source": self.event_source,
                 "DetailType": event_type,
@@ -33,9 +33,9 @@
                 "EventBusName": self.event_bus_name
             }]
         )
 
         if response.get("ResponseMetadata", {}).get("HTTPStatusCode") == 200:
             return True
         else:
-            logger.critical(f"{self.__class__.__name__} - publish - failed")
+            logger.critical(f"{self.__class__.__name__}.publish - failed")
             return False
```

### Comparing `microgue-1.0.9/microgue/abstract_app.py` & `microgue-2.0.0/microgue/abstract_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
-import logging
 import traceback
 from .constants.error_constants import ErrorConstants
 from flask import Flask, request, Response, g
+from .loggers.logger import Logger
 from .security.generic import is_allowed_by_all
 from werkzeug.exceptions import Unauthorized, Forbidden, NotFound, MethodNotAllowed
 from .utils import JSONResponse
 
-logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
 class AbstractApp:
     app = None
     views = []
     blueprints = []
     mask_request_headers_fields = []
@@ -64,29 +63,29 @@
             request_data = json.loads(request.data.decode("utf-8"))
             for mask_request_data_field in cls.mask_request_data_fields:
                 if mask_request_data_field in request_data:
                     request_data[mask_request_data_field] = "*****"
         except:
             request_data = {}
 
-        logger.debug("########## Request Received ########################################")
+        logger.debug("Request Received", priority=1)
         logger.debug(f"method: {request.method}")
         logger.debug(f"url: {request.url}")
         logger.debug(f"headers: {request_headers}")
         logger.debug(f"body: {request_data}")
 
     def register_after_request_handler(self):
         self.app.after_request(self.after_request_handler)
 
     @staticmethod
     def after_request_handler(response):
         if not g.get("authenticated") and int(response.status_code) < 400:
             response = Response(json.dumps({"error": ErrorConstants.App.UNABLE_TO_AUTHENTICATE}), status=401)
 
-        logger.debug("########## Response Sent ########################################")
+        logger.debug("Response Sent", priority=1)
         logger.debug(f"status: {response.status}")
         logger.debug(f"headers: {response.headers}")
         logger.debug(f"body: {response.response}")
 
         return response
 
     def register_error_handlers(self):
@@ -97,47 +96,47 @@
         self.register_internal_server_error()
 
     def register_unauthorized_error(self):
         self.app.register_error_handler(Unauthorized, self.unauthorized_error)
 
     @staticmethod
     def unauthorized_error(e):
-        logger.debug("########## Authentication Error ########################################")
+        logger.debug("Authentication Error", priority=1)
         logger.debug(f"{e.__class__.__name__}: {e}")
         return JSONResponse({"error": ErrorConstants.App.UNABLE_TO_AUTHENTICATE}, status=401)
 
     def register_forbidden_error(self):
         self.app.register_error_handler(Forbidden, self.forbidden_error)
 
     @staticmethod
     def forbidden_error(e):
-        logger.debug("########## Authorization Error ########################################")
+        logger.debug("Authorization Error", priority=1)
         logger.debug(f"{e.__class__.__name__}: {e}")
         return JSONResponse({"error": ErrorConstants.App.UNABLE_TO_AUTHORIZE}, status=403)
 
     def register_not_found_error(self):
         self.app.register_error_handler(NotFound, self.not_found_error)
 
     @staticmethod
     def not_found_error(e):
-        logger.debug("########## Not Found Error ########################################")
+        logger.debug("Not Found Error", priority=1)
         logger.debug(f"{e.__class__.__name__}: {e}")
         return JSONResponse({"error": ErrorConstants.App.REQUESTED_URL_NOT_FOUND}, status=404)
 
     def register_method_not_allowed_error(self):
         self.app.register_error_handler(MethodNotAllowed, self.method_not_allowed_error)
 
     @staticmethod
     def method_not_allowed_error(e):
-        logger.debug("########## Method Not Allowed Error ########################################")
+        logger.debug("Method Not Allowed Error", priority=1)
         logger.debug(f"{e.__class__.__name__}: {e}")
         return JSONResponse({"error": ErrorConstants.App.METHOD_NOT_ALLOWED}, status=405)
 
     def register_internal_server_error(self):
         self.app.register_error_handler(Exception, self.internal_server_error)
 
     @staticmethod
     def internal_server_error(e):
-        logger.error("########## Internal Server Error ########################################")
+        logger.error("Internal Server Error", priority=1)
         logger.error(f"{e.__class__.__name__}: {e}")
         logger.error(traceback.format_exc())
         return JSONResponse({"error": ErrorConstants.App.INTERNAL_SERVER_ERROR}, status=500)
```

### Comparing `microgue-1.0.9/microgue/services/service.py` & `microgue-2.0.0/microgue/services/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,96 @@
 import json
-import logging
 import requests
 import traceback
 from collections import OrderedDict
 from ..constants.error_constants import ErrorConstants
 from ..utils import mask_fields_in_data
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
 class Service:
+    class Request:
+        def __init__(self,
+            url="",
+            parameters={},
+            method="GET",
+            headers={},
+            cookies={},
+            data={},
+            files={},
+            verify_ssl=True
+        ):
+            self.url = url
+            self.parameters = parameters
+            self.method = method
+            self.headers = headers
+            self.cookies = cookies
+            self.data = data
+            self.files = files
+            self.verify_ssl = verify_ssl
+
     class Response:
         def __init__(self, status_code=400, headers={}, cookies={}, data={}):
             self.status_code = status_code
             self.headers = headers
             self.cookies = cookies
             self.data = data
 
     def __init__(self, *args, **kwargs):
         self.request_base_url = ""
         self.mask_request_headers_fields = []
         self.mask_request_data_fields = []
 
-    def invoke(
-            self,
-            request_url="",
-            request_parameters={},
-            request_method="GET",
-            request_headers={},
-            request_cookies={},
-            request_data={},
-            request_files={},
-            verify_ssl=True
-    ):
-        logger.debug(f"########## {self.__class__.__name__} Invoke ##########")
-        logger.debug(f"request url: {request_url}")
-        logger.debug(f"request method: {request_method}")
-        logger.debug(f"request headers: {mask_fields_in_data(request_headers, self.mask_request_headers_fields)}")
-        logger.debug(f"request cookies: {request_cookies}")
-        logger.debug(f"request data: {mask_fields_in_data(request_data, self.mask_request_data_fields)}")
+    def request(self, *args, **kwargs):
+        return self.invoke(Service.Request(*args, **kwargs))
+
+    def invoke(self, request):
+        logger.debug(f"{self.__class__.__name__}.invoke", priority=2)
+        logger.debug(f"request url: {request.url}")
+        logger.debug(f"request method: {request.method}")
+        logger.debug(f"request headers: {mask_fields_in_data(request.headers, self.mask_request_headers_fields)}")
+        logger.debug(f"request cookies: {request.cookies}")
+        logger.debug(f"request data: {mask_fields_in_data(request.data, self.mask_request_data_fields)}")
 
         # open all files before sending them
         opened_request_files = OrderedDict()
-        for key, file in request_files.items():
+        for key, file in request.files.items():
             opened_request_files[key] = open(file, "rb")
 
         try:
             requests_response = requests.request(
-                url=self.request_base_url + request_url,
-                params=request_parameters,
-                method=request_method,
-                headers=request_headers,
-                cookies=request_cookies,
-                json=request_data,
+                url=self.request_base_url + request.url,
+                params=request.parameters,
+                method=request.method,
+                headers=request.headers,
+                cookies=request.cookies,
+                json=request.data,
                 files=opened_request_files,
-                verify=verify_ssl
+                verify=request.verify_ssl
             )
 
             response_status_code = requests_response.status_code
             response_headers = dict(requests_response.headers)
             response_cookies = dict(requests_response.cookies)
 
             try:
                 response_data = requests_response.json()
             except:
                 response_data = requests_response.text
 
-            logger.debug(f"########## {self.__class__.__name__} Invoke Response")
+            logger.debug(f"{self.__class__.__name__}.invoke - Response", priority=3)
             logger.debug(f"response status code: {response_status_code}")
             logger.debug(f"response headers: {response_headers}")
             logger.debug(f"response cookies: {response_cookies}")
             logger.debug(f"response data: {response_data}")
 
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Invoke Error")
+            logger.error(f"{self.__class__.__name__}.invoke - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             logger.error(traceback.format_exc())
             response_status_code = 500
             response_headers = {}
             response_cookies = {}
             response_data = {"error": ErrorConstants.App.INTERNAL_SERVER_ERROR}
```

### Comparing `microgue-1.0.9/microgue/caches/abstract_cache.py` & `microgue-2.0.0/microgue/caches/abstract_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import datetime
 import json
-import logging
 import redis
+from ..loggers.logger import Logger
 
-logger = logging.getLogger("microgue")
+logger = Logger()
 
 
-class CacheConnectionFailed(Exception):
-    pass
+class CacheConnectionFailed(Exception): pass
 
 
 class AbstractCache:
     cache = None
     host = ""
     port = ""
     prefix = ""
     ttl = 900
     connection_timeout = 1
     connection_required = True
 
     def __init__(self, *args, **kwargs):
-        logger.debug(f"########## {self.__class__.__name__} __init__ ##########")
+        logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"self.__class__.cache: {self.__class__.cache}")
         try:
             if self.__class__.cache is None:
                 logger.debug("connecting to redis")
                 self.__class__.cache = redis.StrictRedis(host=self.host, port=self.port, socket_connect_timeout=self.connection_timeout)
                 self.__class__.cache.ping()
             else:
                 logger.debug("using existing connection to redis")
         except Exception as e:
-            logger.error(f"########## {self.__class__.__name__} Error")
+            logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
             logger.error(f"{e.__class__.__name__}: {str(e)}")
             if self.connection_required:
                 raise CacheConnectionFailed(str(e))
             else:
                 self.__class__.cache = None
 
     def _prefix_key(self, key):
@@ -43,15 +42,15 @@
         else:
             return key
 
     def get(self, key):
         if self.cache:
             prefixed_key = self._prefix_key(key)
             value = self.cache.get(prefixed_key)
-            logger.debug(f"########## {self.__class__.__name__} Get ##########")
+            logger.debug(f"{self.__class__.__name__}.get", priority=2)
             logger.debug(f"Key: {prefixed_key}")
             logger.debug(f"Value: {value}")
             try:
                 return json.loads(value)
             except:
                 pass
             try:
@@ -61,30 +60,30 @@
             return value
 
     def set(self, key, value, ttl=None):
         if self.cache:
             value = value if type(value) is str else json.dumps(value)
             prefixed_key = self._prefix_key(key)
             ttl = ttl if ttl is not None else self.ttl
-            logger.debug(f"########## {self.__class__.__name__} Set ##########")
+            logger.debug(f"{self.__class__.__name__}.set", priority=2)
             logger.debug(f"Key: {prefixed_key}")
             logger.debug(f"Value: {value}")
             self.cache.set(prefixed_key, value, ex=ttl)
             return True
 
     def delete(self, key):
         if self.cache:
             prefixed_key = self._prefix_key(key)
-            logger.debug(f"########## {self.__class__.__name__} Delete ##########")
+            logger.debug(f"{self.__class__.__name__}.delete", priority=2)
             logger.debug(f"Key: {prefixed_key}")
             return bool(self.cache.delete(prefixed_key))
 
     def expires_at(self, key):
         if self.cache:
             prefixed_key = self._prefix_key(key)
             expire_time = self.cache.ttl(prefixed_key)
             return str(datetime.timedelta(seconds=expire_time))
 
     def clear(self):
         if self.cache:
-            logger.debug("########## Clearing All Cache ##########")
+            logger.debug(f"{self.__class__.__name__}.clear", priority=2)
             return bool(self.cache.flushdb())
```

### Comparing `microgue-1.0.9/README.md` & `microgue-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `microgue-1.0.9/setup.py` & `microgue-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="microgue",
-    version="1.0.9",
+    version="2.0.0",
     author="Michael Hudelson",
     author_email="michaelhudelson@gmail.com",
-    description="Quickly spin up microservices in AWS using flask",
+    description="This project contains bootstrap code to speed up the development of AWS based microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "boto3",
         "flask",
```

### Comparing `microgue-1.0.9/microgue.egg-info/PKG-INFO` & `microgue-2.0.0/microgue.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 1.0.9
-Summary: Quickly spin up microservices in AWS using flask
+Version: 2.0.0
+Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
         
         This project contains bootstrap code to speed up the development of AWS based microservices
```

### Comparing `microgue-1.0.9/microgue.egg-info/SOURCES.txt` & `microgue-2.0.0/microgue.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 microgue/objects/abstract_expiring_model_object.py
 microgue/objects/abstract_model_object.py
 microgue/objects/object.py
 microgue/queues/__init__.py
 microgue/queues/abstract_queue.py
 microgue/secrets/__init__.py
 microgue/secrets/secrets.py
-microgue/secrets/secrets_without_logging.py
 microgue/security/__init__.py
 microgue/security/generic.py
 microgue/services/__init__.py
 microgue/services/service.py
 microgue/storages/__init__.py
 microgue/storages/abstract_storage.py
```

