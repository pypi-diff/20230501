# Comparing `tmp/hansken-2023.3.6.tar.gz` & `tmp/hansken-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hansken-2023.3.6.tar", last modified: Mon Mar  6 14:30:00 2023, max compression
+gzip compressed data, was "hansken-2023.5.1.tar", last modified: Mon May  1 09:18:09 2023, max compression
```

## Comparing `hansken-2023.3.6.tar` & `hansken-2023.5.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.862832 hansken-2023.3.6/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-03-06 14:29:51.000000 hansken-2023.3.6/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-03-06 14:29:51.000000 hansken-2023.3.6/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-03-06 14:30:00.862832 hansken-2023.3.6/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-06 14:29:51.000000 hansken-2023.3.6/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.858832 hansken-2023.3.6/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-03-06 14:29:56.000000 hansken-2023.3.6/hansken/VERSION
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2358 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/abstract_trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/admin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    31922 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/auth.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/connect.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26374 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/query.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.858832 hansken-2023.3.6/hansken/recipes/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21581 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/export.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.858832 hansken-2023.3.6/hansken/recipes/report/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/report/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.854832 hansken-2023.3.6/hansken/recipes/report/templates/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.858832 hansken-2023.3.6/hansken/recipes/report/templates/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/report/templates/hansken/base.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/report/templates/hansken/default.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/report/templates/hansken/macros.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/report/templates/hansken/print.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/recipes/report/templates/hansken/table.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   132064 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/remote.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.862832 hansken-2023.3.6/hansken/tool/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/_webhdfs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_backup.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_extract.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_grant.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_mount.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11094 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_quickstart.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_shell.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_stats.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_tasks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_tools.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_upload.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/tool/command_versions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59342 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-03-06 14:29:51.000000 hansken-2023.3.6/hansken/util.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-03-06 14:30:00.858832 hansken-2023.3.6/hansken.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-03-06 14:30:00.000000 hansken-2023.3.6/hansken.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-03-06 14:30:00.000000 hansken-2023.3.6/hansken.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-03-06 14:30:00.000000 hansken-2023.3.6/hansken.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-03-06 14:30:00.000000 hansken-2023.3.6/hansken.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      247 2023-03-06 14:30:00.000000 hansken-2023.3.6/hansken.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-03-06 14:30:00.000000 hansken-2023.3.6/hansken.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-03-06 14:30:00.862832 hansken-2023.3.6/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1809 2023-03-06 14:29:51.000000 hansken-2023.3.6/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.341517 hansken-2023.5.1/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-05-01 09:18:00.000000 hansken-2023.5.1/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-05-01 09:18:00.000000 hansken-2023.5.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-01 09:18:09.341517 hansken-2023.5.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-05-01 09:18:00.000000 hansken-2023.5.1/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-05-01 09:18:05.000000 hansken-2023.5.1/hansken/VERSION
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2358 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/abstract_trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/admin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    31922 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/auth.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/connect.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26374 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/query.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/recipes/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/export.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/recipes/report/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.333517 hansken-2023.5.1/hansken/recipes/report/templates/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/recipes/report/templates/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/base.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/default.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/macros.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/print.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/table.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   134425 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/remote.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.341517 hansken-2023.5.1/hansken/tool/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/_webhdfs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_backup.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_extract.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_grant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_mount.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11094 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_quickstart.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_shell.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_stats.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_tasks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_tools.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_upload.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_versions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59342 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/util.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      247 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-05-01 09:18:09.341517 hansken-2023.5.1/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1809 2023-05-01 09:18:00.000000 hansken-2023.5.1/setup.py
```

### Comparing `hansken-2023.3.6/LICENSE` & `hansken-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/PKG-INFO` & `hansken-2023.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.3.6
+Version: 2023.5.1
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hansken-2023.3.6/README.md` & `hansken-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/__init__.py` & `hansken-2023.5.1/hansken/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/abstract_trace.py` & `hansken-2023.5.1/hansken/abstract_trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/admin.py` & `hansken-2023.5.1/hansken/admin.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/auth.py` & `hansken-2023.5.1/hansken/auth.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/connect.py` & `hansken-2023.5.1/hansken/connect.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/query.py` & `hansken-2023.5.1/hansken/query.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/recipes/export.py` & `hansken-2023.5.1/hansken/recipes/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,17 @@
         or `False` to turn parallel processing of *traces* off
     :raises ValueError: on the first error result when *on_error* is not
         supplied (the error is set as the cause)
     """
     if jobs is True or not isinstance(jobs, int):
         raise TypeError('an int or False is required for arguments jobs')
 
-    num_total = len(traces)
+    # determine the number of traces, preferring results.num_results over len(results)
+    num_total = getattr(traces, 'num_results', None) or len(traces)
+
     # determine the ideal length of the folder names for split sets
     order = len(str(num_total // split)) if split else 1
 
     try:
         executor = ThreadPoolExecutor(max_workers=jobs or 1, thread_name_prefix='bulk_export_worker')
     except TypeError:
         # thread_name_prefix is not supported for Python 3.5 (backport for 2.7 *does* have this argument)
```

### Comparing `hansken-2023.3.6/hansken/recipes/report/__init__.py` & `hansken-2023.5.1/hansken/recipes/report/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/recipes/report/templates/hansken/base.html` & `hansken-2023.5.1/hansken/recipes/report/templates/hansken/base.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/recipes/report/templates/hansken/macros.html` & `hansken-2023.5.1/hansken/recipes/report/templates/hansken/macros.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/remote.py` & `hansken-2023.5.1/hansken/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1132,14 +1132,42 @@
                              'overwrite': overwrite,
                              'trace': trace,
                              'properties': properties,
                              'data': data})
         )
         return _expect_ok(response).json()
 
+    def add_trace_data(self, project_id, trace_uid, data_type, data, key=fetch):
+        """
+        Uploads a single data stream for a specific trace.
+
+        :param project_id: the project to import *data* into
+        :param trace_uid: uid of the trace
+        :param data_type: the name of the data stream to upload data to. Allowed data types can be found in the
+                          trace model
+        :param data: the data to be uploaded, either `bytes`, a file-like object or an iterable providing bytes
+        :param key: the key data for image *trace* belongs to, must be `fetch`, `None` or binary (`bytes`)
+        :return: True on success (failure will likely result in an HTTPError)
+        """
+        if key is fetch:
+            # auto-fetch key if there's data to be imported and key is not provided
+            key = self._maybe_fetch_key(image_from_uid(trace_uid), key=key)
+
+        response = self._session.post(
+            self.url(self.path.projects, project_id, 'traces', trace_uid, 'data', data_type),
+            headers=omit_empty({
+                'Content-type': 'application/octet-stream',
+                'Hansken-Image-Key': b64encode(key) if key else None
+            }),
+            data=data
+        )
+
+        with drain(response):
+            return _expect_ok(response, ok=codes.created) is response
+
     def create_trace(self, project_id, parent_uid, child, data=None, key=fetch):
         """
         Requests a new trace to be indexed as a child trace of an existing
         trace.
 
         :param project_id: id of the project to index the trace into
         :param parent_uid: the trace uid of the trace to attach the new child
@@ -2797,14 +2825,29 @@
         :rtype: `.TraceletSearchResult`
         """
         fd = self.connection.singlefile_tracelets(singlefile_id=self.project_id, tracelet_type=tracelet_type)
         return TraceletSearchResult(fd, DictView, model=self.model,
                                     project_id=self.project_id, tracelet_type=tracelet_type,
                                     connection=self.connection)
 
+    @_auto_open
+    def add_trace_data(self, trace_uid, data_type, data, key=fetch):
+        """
+        Uploads a single data stream for a specific trace.
+
+        :param trace_uid: uid of the trace
+        :param data_type: the name of the data stream to upload data to. Allowed data types can be found in the
+                          trace model
+        :param data: the data to be uploaded, either `bytes`, a file-like object or an iterable providing bytes
+        :param key: the key data for image *trace* belongs to, must be `fetch`, `None` or binary (`bytes`)
+        :return: True on success (failure will likely result in an HTTPError)
+        """
+        return self.connection.add_trace_data(project_id=self.project_id, trace_uid=trace_uid,
+                                              data_type=data_type, data=data, key=key)
+
     def __repr__(self):
         return '<{0.__class__.__module__}.{0.__class__.__name__} project_id={0.project_id}>'.format(self)
 
 
 class MultiProjectContext(ProjectContext):
     """
     Utility class adding a set of project ids to each rest call that
@@ -2894,7 +2937,10 @@
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
 
     def child_builder(self, parent_uid):
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
 
     def update_trace(self, trace, updates=None, data=None, key=fetch, overwrite=False):
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
+
+    def add_trace_data(self, trace_uid, data_type, data, key=fetch):
+        raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
```

### Comparing `hansken-2023.3.6/hansken/tool/__init__.py` & `hansken-2023.5.1/hansken/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/_webhdfs.py` & `hansken-2023.5.1/hansken/tool/_webhdfs.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_backup.py` & `hansken-2023.5.1/hansken/tool/command_backup.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_extract.py` & `hansken-2023.5.1/hansken/tool/command_extract.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_grant.py` & `hansken-2023.5.1/hansken/tool/command_grant.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_mount.py` & `hansken-2023.5.1/hansken/tool/command_mount.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_quickstart.py` & `hansken-2023.5.1/hansken/tool/command_quickstart.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_shell.py` & `hansken-2023.5.1/hansken/tool/command_shell.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_stats.py` & `hansken-2023.5.1/hansken/tool/command_stats.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_tasks.py` & `hansken-2023.5.1/hansken/tool/command_tasks.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_tools.py` & `hansken-2023.5.1/hansken/tool/command_tools.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_upload.py` & `hansken-2023.5.1/hansken/tool/command_upload.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/tool/command_versions.py` & `hansken-2023.5.1/hansken/tool/command_versions.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/trace.py` & `hansken-2023.5.1/hansken/trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken/util.py` & `hansken-2023.5.1/hansken/util.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/hansken.egg-info/PKG-INFO` & `hansken-2023.5.1/hansken.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.3.6
+Version: 2023.5.1
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hansken-2023.3.6/hansken.egg-info/SOURCES.txt` & `hansken-2023.5.1/hansken.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hansken-2023.3.6/setup.py` & `hansken-2023.5.1/setup.py`

 * *Files identical despite different names*

