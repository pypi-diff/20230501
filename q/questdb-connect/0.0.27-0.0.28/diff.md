# Comparing `tmp/questdb-connect-0.0.27.tar.gz` & `tmp/questdb-connect-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.27.tar", last modified: Mon May  1 20:29:34 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.28.tar", last modified: Mon May  1 20:53:12 2023, max compression
```

## Comparing `questdb-connect-0.0.27.tar` & `questdb-connect-0.0.28.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:29:34.848886 questdb-connect-0.0.27/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.27/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:29:34.848758 questdb-connect-0.0.27/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.27/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-01 20:29:06.000000 questdb-connect-0.0.27/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-01 20:29:34.848928 questdb-connect-0.0.27/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:29:34.844927 questdb-connect-0.0.27/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:29:34.846946 questdb-connect-0.0.27/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1975 2023-05-01 20:29:06.000000 questdb-connect-0.0.27/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    10934 2023-05-01 20:15:41.000000 questdb-connect-0.0.27/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.27/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-01 20:15:41.000000 questdb-connect-0.0.27/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.27/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:29:34.847857 questdb-connect-0.0.27/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:29:34.000000 questdb-connect-0.0.27/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-01 20:29:34.000000 questdb-connect-0.0.27/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-01 20:29:34.000000 questdb-connect-0.0.27/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-01 20:29:34.000000 questdb-connect-0.0.27/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-01 20:29:34.000000 questdb-connect-0.0.27/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-01 20:29:34.000000 questdb-connect-0.0.27/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:29:34.848491 questdb-connect-0.0.27/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-01 20:18:00.000000 questdb-connect-0.0.27/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.27/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.27/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.880790 questdb-connect-0.0.28/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.28/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:53:12.880650 questdb-connect-0.0.28/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.28/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-01 20:53:05.000000 questdb-connect-0.0.28/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-01 20:53:12.880828 questdb-connect-0.0.28/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.876927 questdb-connect-0.0.28/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.878826 questdb-connect-0.0.28/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1975 2023-05-01 20:29:06.000000 questdb-connect-0.0.28/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11085 2023-05-01 20:52:45.000000 questdb-connect-0.0.28/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.28/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-01 20:15:41.000000 questdb-connect-0.0.28/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.28/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.879704 questdb-connect-0.0.28/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.880361 questdb-connect-0.0.28/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-01 20:18:00.000000 questdb-connect-0.0.28/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.28/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.28/tests/test_types.py
```

### Comparing `questdb-connect-0.0.27/LICENSE` & `questdb-connect-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/PKG-INFO` & `questdb-connect-0.0.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.27
+Version: 0.0.28
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.27/README.md` & `questdb-connect-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/pyproject.toml` & `questdb-connect-0.0.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.27"
+version = "0.0.28"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.27/src/questdb_connect/__init__.py` & `questdb-connect-0.0.28/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/src/questdb_connect/dialect.py` & `questdb-connect-0.0.28/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,17 +178,22 @@
             _extend_on=None,
     ):
         table_name = table.name
         result_set = self.bind.execute(f"tables() WHERE name = '{table_name}'")
         if not result_set:
             raise NoResultFound(f"Table '{table_name}' does not exist")
         table_attrs = result_set.first()
-        col_ts_name = table_attrs['designatedTimestamp']
-        partition_by = PartitionBy[table_attrs['partitionBy']]
-        is_wal = True if table_attrs['walEnabled'] else False
+        if table_attrs:
+            col_ts_name = table_attrs['designatedTimestamp']
+            partition_by = PartitionBy[table_attrs['partitionBy']]
+            is_wal = True if table_attrs['walEnabled'] else False
+        else:
+            col_ts_name = None
+            partition_by = PartitionBy.NONE
+            is_wal = True
         for row in self.bind.execute(f"table_columns('{table_name}')"):
             col_name = row[0]
             if include_columns and col_name not in include_columns:
                 continue
             if exclude_columns and col_name in exclude_columns:
                 continue
             col_type = resolve_type_from_name(row[1])
```

### Comparing `questdb-connect-0.0.27/src/questdb_connect/function_names.py` & `questdb-connect-0.0.28/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.28/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/src/questdb_connect/types.py` & `questdb-connect-0.0.28/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.28/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.27
+Version: 0.0.28
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.27/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.28/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/tests/test_dialect.py` & `questdb-connect-0.0.28/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/tests/test_superset.py` & `questdb-connect-0.0.28/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.27/tests/test_types.py` & `questdb-connect-0.0.28/tests/test_types.py`

 * *Files identical despite different names*

