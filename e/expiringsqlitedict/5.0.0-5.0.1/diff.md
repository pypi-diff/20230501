# Comparing `tmp/expiringsqlitedict-5.0.0.tar.gz` & `tmp/expiringsqlitedict-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-5.0.0.tar", last modified: Sat Apr 29 13:13:00 2023, max compression
+gzip compressed data, was "expiringsqlitedict-5.0.1.tar", last modified: Mon May  1 15:44:14 2023, max compression
```

## Comparing `expiringsqlitedict-5.0.0.tar` & `expiringsqlitedict-5.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-5.0.0/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-5.0.0/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-5.0.0/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-5.0.0/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-5.0.0/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-5.0.0/Makefile
--rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-5.0.0/README.rst
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-5.0.0/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-5.0.0/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-5.0.0/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-5.0.0/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-5.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-5.0.0/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-5.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      972 2023-04-29 13:00:17.351526 expiringsqlitedict-5.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      415 2023-04-29 12:33:42.701348 expiringsqlitedict-5.0.0/run_all_tests.sh
--rwxr-xr-x   0        0        0    10897 2023-04-29 13:12:01.647417 expiringsqlitedict-5.0.0/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-5.0.0/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0     7186 2023-04-29 13:11:14.086617 expiringsqlitedict-5.0.0/test.py
--rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 expiringsqlitedict-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-5.0.1/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-5.0.1/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-5.0.1/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-5.0.1/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-5.0.1/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-5.0.1/Makefile
+-rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-5.0.1/README.rst
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-5.0.1/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-5.0.1/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-5.0.1/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-5.0.1/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-5.0.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-5.0.1/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-5.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0      972 2023-05-01 15:38:14.470875 expiringsqlitedict-5.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      920 2023-05-01 15:43:23.632313 expiringsqlitedict-5.0.1/run_all_tests.sh
+-rwxr-xr-x   0        0        0    10878 2023-05-01 15:38:14.470875 expiringsqlitedict-5.0.1/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-5.0.1/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0     7186 2023-04-29 13:11:14.086617 expiringsqlitedict-5.0.1/test.py
+-rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 expiringsqlitedict-5.0.1/PKG-INFO
```

### Comparing `expiringsqlitedict-5.0.0/CHANGELOG.txt` & `expiringsqlitedict-5.0.1/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/LICENSE.apache` & `expiringsqlitedict-5.0.1/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/README.rst` & `expiringsqlitedict-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/bench.py` & `expiringsqlitedict-5.0.1/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/docs/Makefile` & `expiringsqlitedict-5.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/docs/conf.py` & `expiringsqlitedict-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/docs/index.rst` & `expiringsqlitedict-5.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/docs/make.bat` & `expiringsqlitedict-5.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/pyproject.toml` & `expiringsqlitedict-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '5.0.0'
+version = '5.0.1'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `expiringsqlitedict-5.0.0/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-5.0.1/src/expiringsqlitedict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,25 @@
         table=table,
     )
 
     finalize(connection, _close, db)
 
     return connection
 
+_trailers = []
 if sqlite3.sqlite_version_info >= (3, 8, 2):
-    _create_table_trailer = ' WITHOUT ROWID'
-else:
-    _create_table_trailer = ''
+    _trailers.append('WITHOUT ROWID')
 
 if sqlite3.sqlite_version_info >= (3, 37):
-    _create_table_trailer += ' STRICT'
-    _valuetype = 'ANY' 
+    _trailers.append('STRICT')
+    _valuetype = 'ANY'
 else:
-    _valuetype = 'BLOB' 
+    _valuetype = 'BLOB'
+
+_trailer = ', '.join(_trailers)
 
 if sqlite3.sqlite_version_info >= (3, 38):
     _unixepoch = 'UNIXEPOCH()'
 else:
     _unixepoch = "CAST(strftime('%s', 'now') AS INTEGER)"
 
 class Connection(MutableMapping):
@@ -187,15 +188,15 @@
         self._safe_table = table.replace('"', '""')
 
         with closing(self._connection.cursor()) as cursor:
             create_statement = f'''
             CREATE TABLE IF NOT EXISTS "{self._safe_table}" (
                 key TEXT PRIMARY KEY NOT NULL,
                 expire INTEGER NOT NULL,
-                value {_valuetype} NOT NULL){_create_table_trailer}'''
+                value {_valuetype} NOT NULL){_trailer}'''
 
 
             cursor.execute(create_statement)
             cursor.execute(
                 f'CREATE INDEX IF NOT EXISTS "{self._safe_table}_expire_index"'
                 f' ON "{self._safe_table}" (expire)'
             )
```

### Comparing `expiringsqlitedict-5.0.0/test.py` & `expiringsqlitedict-5.0.1/test.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.0/PKG-INFO` & `expiringsqlitedict-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 5.0.0
+Version: 5.0.1
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

