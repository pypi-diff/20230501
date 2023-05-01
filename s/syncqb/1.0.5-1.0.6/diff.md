# Comparing `tmp/syncqb-1.0.5.tar.gz` & `tmp/syncqb-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.5.tar", last modified: Mon Apr 24 19:19:19 2023, max compression
+gzip compressed data, was "syncqb-1.0.6.tar", last modified: Mon May  1 15:34:48 2023, max compression
```

## Comparing `syncqb-1.0.5.tar` & `syncqb-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.691053 syncqb-1.0.5/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.5/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 19:19:19.691053 syncqb-1.0.5/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.5/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-04-24 19:18:47.000000 syncqb-1.0.5/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-24 19:19:19.691053 syncqb-1.0.5/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.5/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.669386 syncqb-1.0.5/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.669386 syncqb-1.0.5/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.5/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.5/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    16238 2023-04-21 17:31:28.000000 syncqb-1.0.5/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11395 2023-04-21 14:13:40.000000 syncqb-1.0.5/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-04-13 17:15:37.000000 syncqb-1.0.5/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.5/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.5/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.5/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2797 2023-04-24 18:59:22.000000 syncqb-1.0.5/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.5/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-04-13 17:16:23.000000 syncqb-1.0.5/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.5/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.680220 syncqb-1.0.5/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.691053 syncqb-1.0.5/tests/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1570 2023-04-24 16:41:50.000000 syncqb-1.0.5/tests/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.937323 syncqb-1.0.6/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.6/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-01 15:34:48.937323 syncqb-1.0.6/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.6/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-05-01 15:34:26.000000 syncqb-1.0.6/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-05-01 15:34:48.937323 syncqb-1.0.6/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.6/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.915656 syncqb-1.0.6/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.926489 syncqb-1.0.6/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.6/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.6/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16499 2023-05-01 15:30:52.000000 syncqb-1.0.6/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11395 2023-04-21 14:13:40.000000 syncqb-1.0.6/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-01 15:30:51.000000 syncqb-1.0.6/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.6/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.6/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.6/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3022 2023-05-01 15:30:50.000000 syncqb-1.0.6/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.6/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-05-01 15:30:49.000000 syncqb-1.0.6/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.6/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.937323 syncqb-1.0.6/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-05-01 15:34:48.000000 syncqb-1.0.6/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-01 15:34:48.937323 syncqb-1.0.6/tests/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4217 2023-05-01 15:18:47.000000 syncqb-1.0.6/tests/test.py
```

### Comparing `syncqb-1.0.5/LICENSE` & `syncqb-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/PKG-INFO` & `syncqb-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.5/README.md` & `syncqb-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/pyproject.toml` & `syncqb-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",'requests>=2.25.1','lxml>=4.6.3','chardet>=3.0.4']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syncqb"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Jacob Gearhardt", email="jacob@synctivate.com" },
 ]
 description = "A Python SDK for quickbase"
 readme = "README.md"
 license = { file="LICENSE" }
 dependencies = [
```

### Comparing `syncqb-1.0.5/src/syncqb/json_quickbase.py` & `syncqb-1.0.6/src/syncqb/json_quickbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         else:
             raise ValueError('Must provide either a query or a qid')
 
         if default == None:
             default = self.default
         
 
-        data = self.denest(response.get('data'))
+        data = self.denest(response)
         data = self.replace_empty_values(data, default)
 
         if round_ints:
             data = self.round_ints(data)
 
         return data
 
@@ -180,57 +180,61 @@
             return self._get_all_data(body, skip, top, report)
         else:
             return self._get_returned_data(body, skip, top, report)
 
     def _get_all_data(self, body, skip=None, top=None, report=False):
         offset = skip or 0
         goal = top or 0
+        database = body.get('from')
+        pk = self.get_primary_key(database)
+        body.get('select', []).append(pk)
 
-        response = self._get_returned_data(body, offset, goal, report)
+        response = self._get_returned_data(body, offset, goal, report, return_meta=True)
 
         metadata = response.get('metadata', {})
         num_records = metadata.get('numRecords', 0)
         total_records = metadata.get('totalRecords', 0)
 
         if goal and goal <= total_records - offset:
             goal -= num_records
         else:
             goal = total_records - num_records - offset
         
         offset += num_records
 
+        data = response.get('data', [])
+        if not data:
+            return data
         while goal > 0:
-            response['data'].extend(self._get_returned_data(body, offset, goal, report)['data'])
-
-            metadata = response.get('metadata', {})
-            num_records = metadata.get('numRecords', 0)
+            response = self._get_returned_data(body, offset, goal, report, return_meta=True)
+            data.extend(response.get('data', []))
+            num_records = response.get('metadata', {}).get('numRecords', 0)
 
             offset += num_records
             goal -= num_records
 
-        data = response['data']
         for index, record in enumerate(data):
             data[index] = json.dumps(record)
 
         data = list(set(data))
 
         for index, record in enumerate(data):
             data[index] = json.loads(record)
             
-        response['data'] = data
-
-        return response
+        return data
 
-    def _get_returned_data(self, body, skip=None, top=None, report=False):
+    def _get_returned_data(self, body, skip=None, top=None, report=False, return_meta=False):
         if report:
             response = self._run_report(body.pop('qid'), body.pop('database'), skip, top)
         else:
             response = self._run_query(body, skip, top)
-
-        return response
+        if return_meta:
+            return response
+        else:
+            return response.get('data', [])
     # ---------------------------------------- single record functions ----------------------------------------
     def add_record(self, fields, database=None, uploads=None, safemode=False, return_fields=None):
 
         if safemode:
             pk = self.get_primary_key(database)
             if pk in fields.keys():
                 raise ValueError(f'Primary key fid: {pk} cannot be set in safemode')
```

### Comparing `syncqb-1.0.5/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.6/src/syncqb/json_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/qb_client.py` & `syncqb-1.0.6/src/syncqb/qb_client.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/qb_client.pyi` & `syncqb-1.0.6/src/syncqb/qb_client.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/qb_errors.py` & `syncqb-1.0.6/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/qb_errors.pyi` & `syncqb-1.0.6/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/quickbase.py` & `syncqb-1.0.6/src/syncqb/quickbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,27 +45,31 @@
             raise QBConnectionError('Connection Error: Invalid URL')
         elif response.status_code == 400:
             raise QuickbaseError('Response Error: Invalid request', response)
         elif response.status_code == 429:
             raise QBResponseError('Response Error: Too many requests', response)
         elif response.status_code == 500:
             raise QBResponseError('Response Error: Internal Quickbase Server Error', response)
-        
+        elif response.status_code == 504:
+            raise QBResponseError('Response Error: Gateway Timeout', response)
         if json:
             try:
                 return response.json()
             except Exception as e:
                 raise QuickbaseError('Response Error: Invalid JSON or no data given', response) from e
         else:
             return response
         
     def _request(self, url, action, headers, data=None, params=None, json=False):
         tries = 0
 
         while tries < 10:
             try:
                 return self._make_request(url, action, headers, params=params, data=data, json=json)
-            except requests.exceptions.Timeout or QBResponseError:
+            except requests.exceptions.Timeout or QBResponseError as e:
                 tries += 1
-                time.sleep(1)
+                if type(e) == QBResponseError:
+                    time.sleep(30)
+                else:
+                    time.sleep(1)
                 pass
         raise QBConnectionError('Connection Error: Timeout')
```

### Comparing `syncqb-1.0.5/src/syncqb/quickbase.pyi` & `syncqb-1.0.6/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/xml_quickbase.py` & `syncqb-1.0.6/src/syncqb/xml_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.6/src/syncqb/xml_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.5/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.6/src/syncqb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.5/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.6/src/syncqb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

