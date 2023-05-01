# Comparing `tmp/pytailor-0.6.1.tar.gz` & `tmp/pytailor-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytailor-0.6.1.tar", max compression
+gzip compressed data, was "pytailor-0.6.2.tar", max compression
```

## Comparing `pytailor-0.6.1.tar` & `pytailor-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1517 2023-04-11 12:43:15.550480 pytailor-0.6.1/LICENSE
--rw-r--r--   0        0        0      873 2023-04-11 12:43:15.558480 pytailor-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/__init__.py
--rw-r--r--   0        0        0      314 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/__init__.py
--rw-r--r--   0        0        0     1000 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/account.py
--rw-r--r--   0        0        0      104 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/base.py
--rw-r--r--   0        0        0    22572 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/dag.py
--rw-r--r--   0        0        0     2622 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/fileset.py
--rw-r--r--   0        0        0      844 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/local_files.py
--rw-r--r--   0        0        0     4260 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/parameterization.py
--rw-r--r--   0        0        0     3182 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/project.py
--rw-r--r--   0        0        0      173 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/__init__.py
--rw-r--r--   0        0        0     5744 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/description.py
--rw-r--r--   0        0        0     6199 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/files_schema.py
--rw-r--r--   0        0        0     6976 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/inputs_schema.py
--rw-r--r--   0        0        0        0 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/strategies/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/strategies/additionalProperties.py
--rw-r--r--   0        0        0      427 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/strategies/tailorschemabuilder.py
--rw-r--r--   0        0        0    10825 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/workflow.py
--rw-r--r--   0        0        0     5221 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/workflow_definition.py
--rw-r--r--   0        0        0        0 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/cli/__init__.py
--rw-r--r--   0        0        0     3585 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/cli/main.py
--rw-r--r--   0        0        0      119 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/__init__.py
--rw-r--r--   0        0        0     4141 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/async_rest_client.py
--rw-r--r--   0        0        0     4303 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/auth.py
--rw-r--r--   0        0        0     1439 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/file_client.py
--rw-r--r--   0        0        0     3812 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/handling.py
--rw-r--r--   0        0        0    10560 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/rest_client.py
--rw-r--r--   0        0        0     1971 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/config.py
--rw-r--r--   0        0        0      371 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/exceptions.py
--rw-r--r--   0        0        0       74 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/__init__.py
--rw-r--r--   0        0        0     1398 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/serialrunner.py
--rw-r--r--   0        0        0    18170 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/taskrunner.py
--rw-r--r--   0        0        0     3631 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/worker.py
--rw-r--r--   0        0        0     3503 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/worker_checks.py
--rw-r--r--   0        0        0    19407 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/models.py
--rw-r--r--   0        0        0     7873 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/utils.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 pytailor-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-05-01 17:52:28.244821 pytailor-0.6.2/LICENSE
+-rw-r--r--   0        0        0      884 2023-05-01 17:52:28.252822 pytailor-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/__init__.py
+-rw-r--r--   0        0        0     1000 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/account.py
+-rw-r--r--   0        0        0      104 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/base.py
+-rw-r--r--   0        0        0    22572 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/dag.py
+-rw-r--r--   0        0        0     2688 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/fileset.py
+-rw-r--r--   0        0        0      844 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/local_files.py
+-rw-r--r--   0        0        0     4260 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/parameterization.py
+-rw-r--r--   0        0        0     3182 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/project.py
+-rw-r--r--   0        0        0      173 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/__init__.py
+-rw-r--r--   0        0        0     5744 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/description.py
+-rw-r--r--   0        0        0     6199 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/files_schema.py
+-rw-r--r--   0        0        0     6976 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/inputs_schema.py
+-rw-r--r--   0        0        0        0 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/strategies/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/strategies/additionalProperties.py
+-rw-r--r--   0        0        0      427 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/schema/strategies/tailorschemabuilder.py
+-rw-r--r--   0        0        0    10825 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/workflow.py
+-rw-r--r--   0        0        0     5221 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/api/workflow_definition.py
+-rw-r--r--   0        0        0        0 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/cli/__init__.py
+-rw-r--r--   0        0        0     3585 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/cli/main.py
+-rw-r--r--   0        0        0      119 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/__init__.py
+-rw-r--r--   0        0        0     4141 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/async_rest_client.py
+-rw-r--r--   0        0        0     4303 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/auth.py
+-rw-r--r--   0        0        0     3025 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/file_client.py
+-rw-r--r--   0        0        0     3812 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/handling.py
+-rw-r--r--   0        0        0    10560 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/clients/rest_client.py
+-rw-r--r--   0        0        0     1971 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/config.py
+-rw-r--r--   0        0        0      371 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/exceptions.py
+-rw-r--r--   0        0        0       74 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/__init__.py
+-rw-r--r--   0        0        0     1398 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/serialrunner.py
+-rw-r--r--   0        0        0    18262 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/taskrunner.py
+-rw-r--r--   0        0        0     3631 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/worker.py
+-rw-r--r--   0        0        0     3503 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/execution/worker_checks.py
+-rw-r--r--   0        0        0    19407 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/models.py
+-rw-r--r--   0        0        0     7873 2023-05-01 17:52:28.252822 pytailor-0.6.2/src/pytailor/utils.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 pytailor-0.6.2/PKG-INFO
```

### Comparing `pytailor-0.6.1/LICENSE` & `pytailor-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/pyproject.toml` & `pytailor-0.6.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytailor"
-version = "0.6.1"
+version = "0.6.2"
 description = "pyTailor orchestrates your existing python code as *workflows*"
 authors = ["Audun Gravdal Johansen <audun@entail.no>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/entailor/pytailor/"
 include = [
     "LICENSE",
 ]
@@ -30,10 +30,9 @@
 markdown = "^3.2.2"
 mkautodoc = "^0.1.0"
 nox = "^2022.8.7"
 
 [tool.poetry.scripts]
 tailor = 'pytailor.cli.main:cli'
 [build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
-
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pytailor-0.6.1/src/pytailor/api/account.py` & `pytailor-0.6.2/src/pytailor/api/account.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/dag.py` & `pytailor-0.6.2/src/pytailor/api/dag.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/fileset.py` & `pytailor-0.6.2/src/pytailor/api/fileset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partial
 from typing import List
 
 from pytailor.api.base import APIBase
 from .project import Project
 from pytailor.clients import RestClient, FileClient
 from pytailor.models import FileSetDownload, FileSetUpload
 from pytailor.utils import check_local_files_exist, get_basenames
@@ -39,22 +40,19 @@
 
     def download(self, task_id: str = None, tags: List[str] = None, use_storage_dirs: bool = True):
         """
         Download files with specified filenames, task_id and/or tags.
 
         If use_storage_dirs=False all files are downloaded to the current directory
         """
-
         fileset_download = FileSetDownload(task_id=task_id, tags=tags)
-
-        with RestClient() as client:
-            fileset_model = client.get_download_urls(self.project.id, self.id, fileset_download)
-
-        with FileClient() as client:
-            handle_file_client_call(client.download_files, fileset_model, use_storage_dirs)
+        with RestClient() as rest_client:
+            fileset_getter = partial(rest_client.get_download_urls, self.project.id, self.id, fileset_download)
+            with FileClient() as file_client:
+                handle_file_client_call(file_client.download_files, fileset_getter, use_storage_dirs)
 
     def list_files(self, task_id: str = None, tags: List[str] = None):
         """List files with specified task_id and/or tags"""
 
         fileset_download = FileSetDownload(task_id=task_id, tags=tags)
 
         with RestClient() as client:
```

### Comparing `pytailor-0.6.1/src/pytailor/api/local_files.py` & `pytailor-0.6.2/src/pytailor/api/local_files.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/parameterization.py` & `pytailor-0.6.2/src/pytailor/api/parameterization.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/project.py` & `pytailor-0.6.2/src/pytailor/api/project.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/schema/description.py` & `pytailor-0.6.2/src/pytailor/api/schema/description.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/schema/files_schema.py` & `pytailor-0.6.2/src/pytailor/api/schema/files_schema.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/schema/inputs_schema.py` & `pytailor-0.6.2/src/pytailor/api/schema/inputs_schema.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/schema/strategies/additionalProperties.py` & `pytailor-0.6.2/src/pytailor/api/schema/strategies/additionalProperties.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/workflow.py` & `pytailor-0.6.2/src/pytailor/api/workflow.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/api/workflow_definition.py` & `pytailor-0.6.2/src/pytailor/api/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/cli/main.py` & `pytailor-0.6.2/src/pytailor/cli/main.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/clients/async_rest_client.py` & `pytailor-0.6.2/src/pytailor/clients/async_rest_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/clients/auth.py` & `pytailor-0.6.2/src/pytailor/clients/auth.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/clients/handling.py` & `pytailor-0.6.2/src/pytailor/clients/handling.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/clients/rest_client.py` & `pytailor-0.6.2/src/pytailor/clients/rest_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/config.py` & `pytailor-0.6.2/src/pytailor/config.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/execution/serialrunner.py` & `pytailor-0.6.2/src/pytailor/execution/serialrunner.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/execution/taskrunner.py` & `pytailor-0.6.2/src/pytailor/execution/taskrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import os
 import random
 import shutil
+from functools import partial
 from itertools import chain
 from pathlib import Path
 
 import httpx
 from jsonpath_ng import parse
 
 from pytailor.api.dag import TaskType
@@ -17,15 +18,16 @@
     create_rundir,
     extract_real_filenames,
     get_logger,
     list_files,
     as_query,
     format_traceback,
     get_basenames,
-    walk_and_apply, get_or_create_node_id,
+    walk_and_apply,
+    get_or_create_node_id,
 )
 
 
 def _resolve_callable(function_name):
     parts = function_name.split(".")
     func_name = parts[-1]
     module_name = ".".join(parts[:-1])
@@ -279,29 +281,29 @@
                             pass
                     if not found:
                         raise
 
     def __download_filetag_from_own_fileset(self, filetag: str, use_storage_dirs: bool):
 
         fileset_download = FileSetDownload(task_id=self.__task_id, tags=[filetag])
-        # get download links
-        with RestClient() as client:
-            fileset = client.get_download_urls(self.__project_id, self.__fileset_id, fileset_download)
-        # do downloads
-        with FileClient() as client:
-            handle_file_client_call(client.download_files, fileset, use_storage_dirs)
+        with RestClient() as rest_client:
+            fileset_getter = partial(
+                rest_client.get_download_urls, self.__project_id, self.__fileset_id, fileset_download
+            )
+            with FileClient() as file_client:
+                handle_file_client_call(file_client.download_files, fileset_getter, use_storage_dirs)
 
     def __download_filetag_from_other_workflow(self, wf_id: str, filetag: str, use_storage_dirs: bool):
         fileset_download = FileSetDownload(tags=[filetag])
-        # get download links
-        with RestClient() as client:
-            fileset = client.get_download_urls_from_wf_id(self.__project_id, wf_id, fileset_download)
-        # do downloads
-        with FileClient() as client:
-            handle_file_client_call(client.download_files, fileset, use_storage_dirs)
+        with RestClient() as rest_client:
+            fileset_getter = partial(
+                rest_client.get_download_urls_from_wf_id, self.__project_id, wf_id, fileset_download
+            )
+            with FileClient() as file_client:
+                handle_file_client_call(file_client.download_files, fileset_getter, use_storage_dirs)
 
         # add file info to context
         self.__update_context_with_file_info(wf_id, filetag, use_storage_dirs)
 
     def __update_context_with_file_info(self, wf_id: str, filetag: str, use_storage_dirs: bool):
         # get workflow details
         with RestClient() as client:
```

### Comparing `pytailor-0.6.1/src/pytailor/execution/worker.py` & `pytailor-0.6.2/src/pytailor/execution/worker.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/execution/worker_checks.py` & `pytailor-0.6.2/src/pytailor/execution/worker_checks.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/models.py` & `pytailor-0.6.2/src/pytailor/models.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/src/pytailor/utils.py` & `pytailor-0.6.2/src/pytailor/utils.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.1/PKG-INFO` & `pytailor-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytailor
-Version: 0.6.1
+Version: 0.6.2
 Summary: pyTailor orchestrates your existing python code as *workflows*
 Home-page: https://github.com/entailor/pytailor/
 License: BSD-3-Clause
 Author: Audun Gravdal Johansen
 Author-email: audun@entail.no
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

