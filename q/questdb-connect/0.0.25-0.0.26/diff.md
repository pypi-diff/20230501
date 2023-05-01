# Comparing `tmp/questdb-connect-0.0.25.tar.gz` & `tmp/questdb-connect-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.25.tar", last modified: Thu Apr 27 16:19:49 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.26.tar", last modified: Mon May  1 20:23:27 2023, max compression
```

## Comparing `questdb-connect-0.0.25.tar` & `questdb-connect-0.0.26.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 16:19:49.143513 questdb-connect-0.0.25/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.25/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 16:19:49.143384 questdb-connect-0.0.25/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.25/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2446 2023-04-27 16:19:28.000000 questdb-connect-0.0.25/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-27 16:19:49.143547 questdb-connect-0.0.25/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 16:19:49.141100 questdb-connect-0.0.25/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 16:19:49.142102 questdb-connect-0.0.25/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.25/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    10187 2023-04-27 10:40:05.000000 questdb-connect-0.0.25/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.25/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10721 2023-04-27 16:18:46.000000 questdb-connect-0.0.25/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.25/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 16:19:49.142856 questdb-connect-0.0.25/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 16:19:49.000000 questdb-connect-0.0.25/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-04-27 16:19:49.000000 questdb-connect-0.0.25/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-27 16:19:49.000000 questdb-connect-0.0.25/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-27 16:19:49.000000 questdb-connect-0.0.25/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-27 16:19:49.000000 questdb-connect-0.0.25/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-27 16:19:49.000000 questdb-connect-0.0.25/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 16:19:49.143212 questdb-connect-0.0.25/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.25/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.25/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.25/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:23:27.659026 questdb-connect-0.0.26/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.26/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:23:27.658886 questdb-connect-0.0.26/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.26/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-01 20:23:11.000000 questdb-connect-0.0.26/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-01 20:23:27.659061 questdb-connect-0.0.26/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:23:27.654460 questdb-connect-0.0.26/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:23:27.656598 questdb-connect-0.0.26/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1956 2023-05-01 20:15:41.000000 questdb-connect-0.0.26/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10934 2023-05-01 20:15:41.000000 questdb-connect-0.0.26/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.26/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-01 20:15:41.000000 questdb-connect-0.0.26/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.26/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:23:27.657561 questdb-connect-0.0.26/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 20:23:27.000000 questdb-connect-0.0.26/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-01 20:23:27.000000 questdb-connect-0.0.26/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-01 20:23:27.000000 questdb-connect-0.0.26/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-01 20:23:27.000000 questdb-connect-0.0.26/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-01 20:23:27.000000 questdb-connect-0.0.26/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-01 20:23:27.000000 questdb-connect-0.0.26/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 20:23:27.658377 questdb-connect-0.0.26/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-01 20:18:00.000000 questdb-connect-0.0.26/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.26/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.26/tests/test_types.py
```

### Comparing `questdb-connect-0.0.25/LICENSE` & `questdb-connect-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.25/PKG-INFO` & `questdb-connect-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.25
+Version: 0.0.26
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.25/README.md` & `questdb-connect-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.25/pyproject.toml` & `questdb-connect-0.0.26/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.25"
+version = "0.0.26"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -76,7 +76,8 @@
 max-branches = 20
 max-args = 10
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
+"tests/conftest.py" = ["S608"]
```

### Comparing `questdb-connect-0.0.25/src/questdb_connect/dialect.py` & `questdb-connect-0.0.26/src/questdb_connect/dialect.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
+import re
 
 import sqlalchemy as sqla
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
-from questdb_connect.types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
+from . import public_schema_filter
+from .types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
@@ -97,31 +99,39 @@
 
     def __init__(
             self,
             dialect,
             initial_quote='"',
             final_quote=None,
             escape_quote='"',
-            quote_case_sensitive_collations=True,
-            omit_schema=False,
+            quote_case_sensitive_collations=False,
+            omit_schema=True,
     ):
         super().__init__(
-            dialect,
-            "'",
-            final_quote,
-            "'",
-            quote_case_sensitive_collations,
-            True)
+            dialect=dialect,
+            initial_quote=initial_quote,
+            final_quote=final_quote,
+            escape_quote=escape_quote,
+            quote_case_sensitive_collations=quote_case_sensitive_collations,
+            omit_schema=omit_schema)
 
     def quote_identifier(self, value):
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
         return True
 
+    def format_schema(self, name):
+        """Prepare a quoted schema name."""
+        return ""
+
+    def format_table(self, table, use_schema=True, name=None):
+        """Prepare a quoted table and schema name."""
+        return quote_identifier(name if name else table.name)
+
 
 class QDBDDLCompiler(DDLCompiler, abc.ABC):
     def visit_create_schema(self, create, **kw):
         raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
 
     def visit_drop_schema(self, drop, **kw):
         raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
@@ -138,14 +148,18 @@
         return column.type.column_spec(column.name)
 
 
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
+    def visit_textclause(self, textclause, add_to_result_map=None, **kw):
+        textclause.text = re.sub(public_schema_filter, '', textclause.text)
+        return super().visit_textclause(textclause, add_to_result_map, **kw)
+
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
             include_columns,
             exclude_columns=(),
@@ -193,28 +207,32 @@
             'name': row[0],
             'type': resolve_type_from_name(row[1])(),
             'nullable': True,
             'autoincrement': False,
             'persisted': True
         } for row in result_set]
 
+    def get_schema_names(self):
+        return ['public']
+
 
 # class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
 class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
     type_compiler = GenericTypeCompiler
     inspector = QDBInspector
     preparer = QDBIdentifierPreparer
     supports_schemas = False
     supports_statement_cache = False
     supports_server_side_cursors = False
+    supports_native_boolean = True
     supports_views = False
     supports_empty_insert = False
     supports_multivalues_insert = True
     supports_comments = True
     inline_comments = False
     postfetch_lastrowid = False
     non_native_boolean_check_constraint = False
```

### Comparing `questdb-connect-0.0.25/src/questdb_connect/function_names.py` & `questdb-connect-0.0.26/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.25/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.26/src/questdb_connect/superset_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
-from questdb_connect import types
-from questdb_connect.function_names import FUNCTION_NAMES
+
+from . import types
+from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
 _MATCH_PUBLIC_SCHEMA = r"(')?(public(?(1)\1)\.)"
```

### Comparing `questdb-connect-0.0.25/src/questdb_connect/types.py` & `questdb-connect-0.0.26/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.25/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.26/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.25
+Version: 0.0.26
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.25/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.26/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.25/tests/test_dialect.py` & `questdb-connect-0.0.26/tests/test_dialect.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,23 +132,23 @@
 
 
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
-    expected = ("(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+    expected = ("(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                 "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                 "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                 "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                 "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
     try:
         for idx in range(num_rows):
             session.add(test_model(
                 col_boolean=True,
@@ -176,23 +176,23 @@
 
 
 def test_bulk_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
-    expected = ("(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+    expected = ("(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                 "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                 "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                 "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
-                "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
+                "(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                 "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
     models = [
         test_model(
             col_boolean=True,
             col_byte=8,
```

### Comparing `questdb-connect-0.0.25/tests/test_superset.py` & `questdb-connect-0.0.26/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.25/tests/test_types.py` & `questdb-connect-0.0.26/tests/test_types.py`

 * *Files identical despite different names*

