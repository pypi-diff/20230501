# Comparing `tmp/questdb-connect-0.0.28.tar.gz` & `tmp/questdb-connect-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.28.tar", last modified: Mon May  1 20:53:12 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.29.tar", last modified: Mon May  1 21:01:09 2023, max compression
```

## Comparing `questdb-connect-0.0.28.tar` & `questdb-connect-0.0.29.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.880790 questdb-connect-0.0.28/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.28/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:53:12.880650 questdb-connect-0.0.28/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.28/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-01 20:53:05.000000 questdb-connect-0.0.28/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-01 20:53:12.880828 questdb-connect-0.0.28/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.876927 questdb-connect-0.0.28/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.878826 questdb-connect-0.0.28/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1975 2023-05-01 20:29:06.000000 questdb-connect-0.0.28/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11085 2023-05-01 20:52:45.000000 questdb-connect-0.0.28/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.28/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-01 20:15:41.000000 questdb-connect-0.0.28/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.28/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.879704 questdb-connect-0.0.28/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-01 20:53:12.000000 questdb-connect-0.0.28/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:53:12.880361 questdb-connect-0.0.28/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-01 20:18:00.000000 questdb-connect-0.0.28/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.28/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.28/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.663452 questdb-connect-0.0.29/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.29/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 21:01:09.663311 questdb-connect-0.0.29/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.29/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-01 20:59:25.000000 questdb-connect-0.0.29/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-01 21:01:09.663486 questdb-connect-0.0.29/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.659530 questdb-connect-0.0.29/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.661480 questdb-connect-0.0.29/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1401 2023-05-01 20:59:25.000000 questdb-connect-0.0.29/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11147 2023-05-01 21:00:28.000000 questdb-connect-0.0.29/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.29/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-01 20:15:41.000000 questdb-connect-0.0.29/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.29/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.662384 questdb-connect-0.0.29/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.663008 questdb-connect-0.0.29/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-01 20:18:00.000000 questdb-connect-0.0.29/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.29/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.29/tests/test_types.py
```

### Comparing `questdb-connect-0.0.28/LICENSE` & `questdb-connect-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/PKG-INFO` & `questdb-connect-0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.28
+Version: 0.0.29
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.28/README.md` & `questdb-connect-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/pyproject.toml` & `questdb-connect-0.0.29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.28"
+version = "0.0.29"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.28/src/questdb_connect/__init__.py` & `questdb-connect-0.0.29/src/questdb_connect/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,53 +16,34 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import re
-
 import psycopg2
-import psycopg2.extras
-from psycopg2.extensions import cursor as _cursor
 
 # ===== DBAPI =====
 
 # https://peps.python.org/pep-0249/
 
 apilevel = '2.0'
 threadsafety = 2
 paramstyle = 'pyformat'
-public_schema_filter = re.compile(r"(')?(public(?(1)\1|)\.)", re.IGNORECASE | re.MULTILINE)
 
 
 class Error(Exception):
     pass
 
 
-class Cursor(_cursor):
-    def execute(self, query, vars=None):
-        if isinstance(query, str) and 'public' in query:
-            clean_query = re.sub(public_schema_filter, '', query)
-        else:
-            clean_query = query
-        return super().execute(clean_query, vars)
-
-
-def cursor_factory(*args, **kwargs):
-    return Cursor(*args, **kwargs)
-
-
 def connect(**kwargs):
     host = kwargs.get('host') or '127.0.0.1'
     port = kwargs.get('port') or 8812
     user = kwargs.get('username') or 'admin'
     password = kwargs.get('password') or 'quest'
     database = kwargs.get('database') or 'main'
     return psycopg2.connect(
-        cursor_factory=cursor_factory,
         host=host,
         port=port,
         user=user,
         password=password,
         database=database)
```

### Comparing `questdb-connect-0.0.28/src/questdb_connect/dialect.py` & `questdb-connect-0.0.29/src/questdb_connect/dialect.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
-from . import public_schema_filter
 from .types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
@@ -144,20 +143,24 @@
 
     def get_column_specification(self, column: sqla.Column, **_):
         if not isinstance(column.type, QDBTypeMixin):
             raise ArgumentError('Column type is not a valid QuestDB type')
         return column.type.column_spec(column.name)
 
 
+_public_schema_filter = re.compile(r"(')?(public(?(1)\1|)\.)", re.IGNORECASE | re.MULTILINE)
+
+
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
+
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
     def visit_textclause(self, textclause, add_to_result_map=None, **kw):
-        textclause.text = re.sub(public_schema_filter, '', textclause.text)
+        textclause.text = re.sub(_public_schema_filter, '', textclause.text)
         return super().visit_textclause(textclause, add_to_result_map, **kw)
 
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
```

### Comparing `questdb-connect-0.0.28/src/questdb_connect/function_names.py` & `questdb-connect-0.0.29/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.29/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/src/questdb_connect/types.py` & `questdb-connect-0.0.29/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.29/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.28
+Version: 0.0.29
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.28/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.29/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/tests/test_dialect.py` & `questdb-connect-0.0.29/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/tests/test_superset.py` & `questdb-connect-0.0.29/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.28/tests/test_types.py` & `questdb-connect-0.0.29/tests/test_types.py`

 * *Files identical despite different names*

