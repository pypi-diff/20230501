# Comparing `tmp/acquire-3.6.dev5.tar.gz` & `tmp/acquire-3.6.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.6.dev5.tar", last modified: Thu Apr 13 07:09:21 2023, max compression
+gzip compressed data, was "acquire-3.6.dev6.tar", last modified: Mon May  1 10:59:54 2023, max compression
```

## Comparing `acquire-3.6.dev5.tar` & `acquire-3.6.dev6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.131761 acquire-3.6.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 07:09:02.000000 acquire-3.6.dev5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 07:09:02.000000 acquire-3.6.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 07:09:02.000000 acquire-3.6.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-13 07:09:21.131761 acquire-3.6.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 07:09:02.000000 acquire-3.6.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.115761 acquire-3.6.dev5/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75219 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.119761 acquire-3.6.dev5/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.123761 acquire-3.6.dev5/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.123761 acquire-3.6.dev5/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.123761 acquire-3.6.dev5/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.127761 acquire-3.6.dev5/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-13 07:09:02.000000 acquire-3.6.dev5/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 07:09:20.000000 acquire-3.6.dev5/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.119761 acquire-3.6.dev5/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:09:21.000000 acquire-3.6.dev5/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-13 07:09:09.000000 acquire-3.6.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:09:21.131761 acquire-3.6.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:21.131761 acquire-3.6.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 07:09:02.000000 acquire-3.6.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-01 10:59:41.000000 acquire-3.6.dev6/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 10:59:41.000000 acquire-3.6.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 10:59:41.000000 acquire-3.6.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-01 10:59:54.687075 acquire-3.6.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-01 10:59:41.000000 acquire-3.6.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.683075 acquire-3.6.dev6/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75219 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.683075 acquire-3.6.dev6/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.683075 acquire-3.6.dev6/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 10:59:44.000000 acquire-3.6.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:59:54.687075 acquire-3.6.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tox.ini
```

### Comparing `acquire-3.6.dev5/LICENSE` & `acquire-3.6.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/PKG-INFO` & `acquire-3.6.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev5
+Version: 3.6.dev6
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev5/README.md` & `acquire-3.6.dev6/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/acquire.py` & `acquire-3.6.dev6/acquire/acquire.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/collector.py` & `acquire-3.6.dev6/acquire/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             raise ValueError("Module name must be provided or Collector needs to be bound to a module")
 
         log.info("- Collecting glob %s", pattern)
         try:
             glob_is_empty = True
             for entry in self.target.fs.path("/").glob(pattern.lstrip("/")):
                 glob_is_empty = False
-                self.collect_path(entry)
+                self.collect_path(entry, module_name=module_name)
         except Exception:
             log.error("- Failed to collect glob %s", pattern, exc_info=True)
             self.report.add_glob_failed(module_name, pattern)
         else:
             if glob_is_empty:
                 self.report.add_glob_empty(module_name, pattern)
             else:
```

### Comparing `acquire-3.6.dev5/acquire/crypt.py` & `acquire-3.6.dev6/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/dynamic/windows/collect.py` & `acquire-3.6.dev6/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/dynamic/windows/handles.py` & `acquire-3.6.dev6/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/dynamic/windows/named_objects.py` & `acquire-3.6.dev6/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/dynamic/windows/ntdll.py` & `acquire-3.6.dev6/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/dynamic/windows/types.py` & `acquire-3.6.dev6/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/esxi.py` & `acquire-3.6.dev6/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/hashes.py` & `acquire-3.6.dev6/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/log.py` & `acquire-3.6.dev6/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/outputs/base.py` & `acquire-3.6.dev6/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/outputs/dir.py` & `acquire-3.6.dev6/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/outputs/tar.py` & `acquire-3.6.dev6/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/tools/decrypter.py` & `acquire-3.6.dev6/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/uploaders/minio.py` & `acquire-3.6.dev6/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/uploaders/plugin.py` & `acquire-3.6.dev6/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/uploaders/plugin_registry.py` & `acquire-3.6.dev6/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire/utils.py` & `acquire-3.6.dev6/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/acquire.egg-info/PKG-INFO` & `acquire-3.6.dev6/acquire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev5
+Version: 3.6.dev6
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev5/acquire.egg-info/SOURCES.txt` & `acquire-3.6.dev6/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/pyproject.toml` & `acquire-3.6.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tests/test_acquire_command.py` & `acquire-3.6.dev6/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tests/test_collector.py` & `acquire-3.6.dev6/tests/test_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,24 @@
             follow=True,
             seen_paths=MOCK_SEEN_PATHS,
             module_name=MOCK_MODULE_NAME,
         )
         mock_collector.collect_symlink.assert_called()
 
 
+def test_collector_collect_glob(mock_collector) -> None:
+    with patch.object(mock_collector, "collect_file", autospec=True):
+        mock_collector.collect_glob(
+            "/foo/bar/*",
+            module_name=MOCK_MODULE_NAME,
+        )
+        mock_collector.collect_file.assert_called_once()
+        assert mock_collector.collect_file.call_args.kwargs.get("module_name", None) == MOCK_MODULE_NAME
+
+
 def test_collector_collect_path_non_existing_file(mock_collector) -> None:
     with patch("acquire.collector.log", autospec=True) as mock_log:
         with patch.object(mock_collector, "report", autospec=True) as mock_report:
             mock_collector.collect_path(
                 "/foo/bar/non-existing-file",
                 seen_paths=MOCK_SEEN_PATHS,
                 module_name=MOCK_MODULE_NAME,
```

### Comparing `acquire-3.6.dev5/tests/test_esxi_memory.py` & `acquire-3.6.dev6/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tests/test_file_sorting.py` & `acquire-3.6.dev6/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tests/test_minio_uploader.py` & `acquire-3.6.dev6/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tests/test_plugin.py` & `acquire-3.6.dev6/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tests/test_utils.py` & `acquire-3.6.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev5/tox.ini` & `acquire-3.6.dev6/tox.ini`

 * *Files identical despite different names*

