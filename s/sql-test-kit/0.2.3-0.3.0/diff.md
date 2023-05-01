# Comparing `tmp/sql_test_kit-0.2.3.tar.gz` & `tmp/sql_test_kit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_test_kit-0.2.3.tar", max compression
+gzip compressed data, was "sql_test_kit-0.3.0.tar", max compression
```

## Comparing `sql_test_kit-0.2.3.tar` & `sql_test_kit-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.2.3/LICENSE
--rw-r--r--   0        0        0      502 2023-04-23 14:57:57.897057 sql_test_kit-0.2.3/README.md
--rw-r--r--   0        0        0      580 2023-04-23 16:54:40.910606 sql_test_kit-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      229 2023-04-23 11:25:03.317853 sql_test_kit-0.2.3/sql_test_kit/__init__.py
--rw-r--r--   0        0        0      371 2023-04-23 16:54:17.063568 sql_test_kit-0.2.3/sql_test_kit/bigquery.py
--rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.2.3/sql_test_kit/column.py
--rw-r--r--   0        0        0     1576 2023-04-23 16:54:17.063881 sql_test_kit-0.2.3/sql_test_kit/query_interpolation.py
--rw-r--r--   0        0        0      390 2023-04-23 16:54:17.064138 sql_test_kit-0.2.3/sql_test_kit/table.py
--rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 sql_test_kit-0.2.3/setup.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 sql_test_kit-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.3.0/LICENSE
+-rw-r--r--   0        0        0      502 2023-04-23 14:57:57.897057 sql_test_kit-0.3.0/README.md
+-rw-r--r--   0        0        0      680 2023-05-01 20:30:40.896634 sql_test_kit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-05-01 19:40:26.357338 sql_test_kit-0.3.0/sql_test_kit/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-01 18:41:57.666535 sql_test_kit-0.3.0/sql_test_kit/bigquery.py
+-rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.3.0/sql_test_kit/column.py
+-rw-r--r--   0        0        0      893 2023-05-01 19:40:26.366078 sql_test_kit-0.3.0/sql_test_kit/data_literals.py
+-rw-r--r--   0        0        0      187 2023-05-01 19:40:18.408718 sql_test_kit-0.3.0/sql_test_kit/interpolation_data.py
+-rw-r--r--   0        0        0     1393 2023-05-01 19:44:04.943564 sql_test_kit-0.3.0/sql_test_kit/query_interpolation.py
+-rw-r--r--   0        0        0      390 2023-04-23 16:54:17.064138 sql_test_kit-0.3.0/sql_test_kit/table.py
+-rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 sql_test_kit-0.3.0/setup.py
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 sql_test_kit-0.3.0/PKG-INFO
```

### Comparing `sql_test_kit-0.2.3/LICENSE` & `sql_test_kit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.2.3/pyproject.toml` & `sql_test_kit-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "sql-test-kit"
-version = "0.2.3"
+version = "0.3.0"
 description = "Framework for testing SQL queries"
 authors = ["victorlandeau <vlandeau@gmail.com>"]
 readme = "README.md"
-packages = [{include = "sql_test_kit"}]
+packages = [
+    { include = "sql_test_kit" },
+]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pandas = "^2.0.0"
-google-cloud-bigquery = {version = "^3.10.0", extras = ["bigquery"]}
-db-dtypes = {version = "^1.1.1", extras = ["bigquery"]}
+python = ">=3.8 <3.12"
+pandas = ">=1.0.0"
+google-cloud-bigquery = { version = ">=3.0.0", optional = true, extras = ["bigquery"] }
+db-dtypes = { version = ">=1.0.0", optional = true, extras = ["bigquery"] }
 
+[tool.poetry.extras]
+bigquery = ["bigquery"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 assertpy = "^1.1"
 pytest = "^7.3.1"
 
 [build-system]
```

### Comparing `sql_test_kit-0.2.3/sql_test_kit/query_interpolation.py` & `sql_test_kit-0.3.0/sql_test_kit/query_interpolation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,38 @@
-from dataclasses import dataclass
+from __future__ import annotations
+
 from typing import List
 
 import pandas as pd
 
+from sql_test_kit.data_literals import DataLiteralsBuilder
+from sql_test_kit.interpolation_data import InterpolationData
 from sql_test_kit.table import AbstractTable
 
 
-@dataclass
-class InterpolationData:
-    table: AbstractTable
-    data: pd.DataFrame
-
-
-def replace_table_names_in_string_by_data_literals(
-    query: str,
-    interpolation_data_list: List[InterpolationData],
-    check_tables_in_query: bool = True,
-) -> str:
-    interpolated_query = query
-    for interpolation_data in interpolation_data_list:
-        table_path = interpolation_data.table.table_path
-        if check_tables_in_query and table_path not in interpolated_query:
-            raise ValueError(
-                f"You are trying to interpolate {table_path} data, "
-                f"but this table is not used in the query."
-            )
-        interpolated_query = interpolated_query.replace(
-            table_path,
-            get_data_literals_query(interpolation_data),
-        )
-    return interpolated_query
-
-
-def get_data_literals_query(interpolation_data: InterpolationData) -> str:
-    records = interpolation_data.data.to_dict(orient="records")
-    columns = interpolation_data.table.columns
-
-    return (
-        "(\n\t\t\t"
-        + "\n\t\t\tUNION ALL\n\t\t\t".join(
-            [
-                "SELECT "
-                + ", ".join(
-                    [
-                        f'CAST("{record[column.name]}" AS {column.type}) AS {column.name}'
-                        for column in columns
-                    ]
+class QueryInterpolator:
+    interpolation_data: List[InterpolationData]
+    data_literals_builder: DataLiteralsBuilder = DataLiteralsBuilder()
+
+    def __init__(self):
+        self.interpolation_data = []
+
+    def add_input_table(
+        self, table: AbstractTable, data: pd.DataFrame
+    ) -> QueryInterpolator:
+        self.interpolation_data.append(InterpolationData(table, data))
+        return self
+
+    def interpolate_query(self, query: str, check_tables_in_query: bool = True) -> str:
+        interpolated_query = query
+        for interpolation_data in self.interpolation_data:
+            table_path = interpolation_data.table.table_path
+            if check_tables_in_query and table_path not in interpolated_query:
+                raise ValueError(
+                    f"You are trying to interpolate {table_path} data, "
+                    f"but this table is not used in the query."
                 )
-                for record in records
-            ]
-        )
-        + "\n\t\t)"
-    )
+            interpolated_query = interpolated_query.replace(
+                table_path,
+                self.data_literals_builder.get_data_literals_query(interpolation_data),
+            )
+        return interpolated_query
```

### Comparing `sql_test_kit-0.2.3/setup.py` & `sql_test_kit-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 packages = \
 ['sql_test_kit']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['db-dtypes[bigquery]>=1.1.1,<2.0.0',
- 'google-cloud-bigquery[bigquery]>=3.10.0,<4.0.0',
- 'pandas>=2.0.0,<3.0.0']
+['pandas>=1.0.0']
 
 setup_kwargs = {
     'name': 'sql-test-kit',
-    'version': '0.2.3',
+    'version': '0.3.0',
     'description': 'Framework for testing SQL queries',
     'long_description': '# sql-test-kit\n\nThis is a framework for testing SQL queries.\nIt works by directly running the queries against the targeted engine, thus being robust to any change in the\ncorresponding SQL dialect.\nMoreover, it is currently focused on interpolating test data directly inside the SQL queries, making the test much\nquicker than if it were creating temporary tables.\n\n# Application example\n\nYou can find an example in applying the framework to bigquery in the [test_bigquery](tests/test_bigquery.py) file.\n',
     'author': 'victorlandeau',
     'author_email': 'vlandeau@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `sql_test_kit-0.2.3/PKG-INFO` & `sql_test_kit-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: sql-test-kit
-Version: 0.2.3
+Version: 0.3.0
 Summary: Framework for testing SQL queries
 Author: victorlandeau
 Author-email: vlandeau@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: db-dtypes[bigquery] (>=1.1.1,<2.0.0)
-Requires-Dist: google-cloud-bigquery[bigquery] (>=3.10.0,<4.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Provides-Extra: bigquery
+Requires-Dist: db-dtypes[bigquery] (>=1.0.0)
+Requires-Dist: google-cloud-bigquery[bigquery] (>=3.0.0)
+Requires-Dist: pandas (>=1.0.0)
 Description-Content-Type: text/markdown
 
 # sql-test-kit
 
 This is a framework for testing SQL queries.
 It works by directly running the queries against the targeted engine, thus being robust to any change in the
 corresponding SQL dialect.
```

