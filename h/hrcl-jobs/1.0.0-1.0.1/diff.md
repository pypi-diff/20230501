# Comparing `tmp/hrcl_jobs-1.0.0.tar.gz` & `tmp/hrcl_jobs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrcl_jobs-1.0.0.tar", last modified: Fri Feb 24 20:37:38 2023, max compression
+gzip compressed data, was "hrcl_jobs-1.0.1.tar", last modified: Mon May  1 14:12:13 2023, max compression
```

## Comparing `hrcl_jobs-1.0.0.tar` & `hrcl_jobs-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:37:38.668086 hrcl_jobs-1.0.0/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     1074 2023-01-18 19:26:42.000000 hrcl_jobs-1.0.0/LICENSE
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      962 2023-02-24 20:37:38.669086 hrcl_jobs-1.0.0/PKG-INFO
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      342 2023-02-03 23:37:54.000000 hrcl_jobs-1.0.0/README.md
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      665 2023-02-24 20:37:27.000000 hrcl_jobs-1.0.0/pyproject.toml
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      295 2023-02-24 20:37:38.671086 hrcl_jobs-1.0.0/setup.cfg
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:37:38.629086 hrcl_jobs-1.0.0/src/
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:37:38.656086 hrcl_jobs-1.0.0/src/hrcl_jobs/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        0 2023-01-18 20:51:45.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/__init__.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    14404 2023-01-18 19:27:30.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/data.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      900 2023-02-21 20:06:25.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/jobspec.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     5818 2023-02-21 20:13:36.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/parallel.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    19831 2023-01-18 19:27:30.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/s22.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     2092 2023-01-18 20:55:52.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/serial.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     9135 2023-01-18 20:54:23.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/setup.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    16133 2023-02-22 00:52:12.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/sqlt.py
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     2929 2023-01-18 19:27:30.000000 hrcl_jobs-1.0.0/src/hrcl_jobs/tools_og.py
-drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-02-24 20:37:38.667086 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      962 2023-02-24 20:37:38.000000 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/PKG-INFO
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      473 2023-02-24 20:37:38.000000 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-02-24 20:37:38.000000 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       69 2023-02-24 20:37:38.000000 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/requires.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       10 2023-02-24 20:37:38.000000 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/top_level.txt
--rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-01-18 19:35:58.000000 hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/zip-safe
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.529474 hrcl_jobs-1.0.1/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1803 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/.gitignore
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/LICENSE
+-rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-01 14:12:13.529631 hrcl_jobs-1.0.1/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      342 2023-02-03 23:39:01.000000 hrcl_jobs-1.0.1/README.md
+-rw-r--r--   0 austinwallace   (501) staff       (20)      116 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/main.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      665 2023-05-01 14:11:50.000000 hrcl_jobs-1.0.1/pyproject.toml
+-rw-r--r--   0 austinwallace   (501) staff       (20)      295 2023-05-01 14:12:13.530125 hrcl_jobs-1.0.1/setup.cfg
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.518910 hrcl_jobs-1.0.1/src/
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.526480 hrcl_jobs-1.0.1/src/hrcl_jobs/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      105 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    14404 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/data.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      892 2023-05-01 14:11:35.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     5818 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/parallel.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    19831 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/s22.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2093 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/serial.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     9082 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/setup.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    17798 2023-05-01 14:11:35.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/sqlt.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2929 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/tools_og.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.528047 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      554 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       69 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/requires.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       10 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/top_level.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-02-02 20:26:18.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/zip-safe
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.529103 hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      842 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    22675 2023-03-30 13:05:54.000000 hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/psi4_inps.py
```

### Comparing `hrcl_jobs-1.0.0/LICENSE` & `hrcl_jobs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.0/PKG-INFO` & `hrcl_jobs-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl_jobs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.0.0/pyproject.toml` & `hrcl_jobs-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hrcl_jobs"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Runs python functions on worker threads with main thread communicating with sql db"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/data.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/data.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/jobspec.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/jobspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 """
 All dataclass_js should have id_label for ms_sl() usage to update sql db
 correctly
 
 TODO: make own repo to consume in both hrcl submodules
 """
 
-
-
 @dataclass
 class example_js:
     id_label: int
     val: float
 
 
 @dataclass
 class mp_js:
     id_label: int
     RA: np.array
     RB: np.array
     ZA: np.array
     ZB: np.array
-    TQA: np.array
-    TQB: np.array
+    TQA: float
+    TQB: float
     level_theory: str
     mem: str
 
 
 @dataclass
 class mp_mon_js:
     id_label: int
```

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/parallel.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/parallel.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/s22.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/s22.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/serial.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .sql import (
+from .sqlt import (
     establish_connection,
     update_mp_rows,
     update_rows,
     collect_rows_into_js_ls_mp,
     collect_row_specific_into_js_mp,
     read_example_output,
     collect_id_into_js,
```

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/setup.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sqlite3 as sql
 import pandas as pd
 from .parallel import ms_sl
-from .sql import (
+from .sqlt import (
     establish_connection,
     convert_df_into_sql,
     convert_df_into_sql_mp,
     collect_rows_into_js_ls_mp,
     create_new_induction_table,
     subset_df,
     collect_rows_index_range,
     select_table_by_column_match,
 )
-# from .tools import np_carts_to_string, string_carts_to_np
-from qm_tools_aw import np_carts_to_string, string_carts_to_np
+from qm_tools_aw.tools import np_carts_to_string, string_carts_to_np
 
 from mpi4py import MPI
 import numpy as np
 from .s22 import s22_testing
 
 
 def tasks() -> None:
```

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/sqlt.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/sqlt.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,30 +60,32 @@
     conn, cur = establish_connection(db_path)
     headers = ",\n".join([f"{k} {v}" for k, v in table.items()])
     if not conn:
         return
     table_format = f""" CREATE TABLE IF NOT EXISTS {table_name} (
             {headers}
             );"""
-    print(table_format)
+    # print(table_format)
     create_table(conn, table_format)
     return
 
 
 def create_table(conn, create_table_sql):
     """create a table from the create_table_sql statement
     :param conn: Connection object
     :param create_table_sql: a CREATE TABLE statement
     :return:
     """
-    # try:
-    c = conn.cursor()
-    c.execute(create_table_sql)
-    # except Error as e:
-    #     print(e)
+    try:
+        c = conn.cursor()
+        c.execute(create_table_sql)
+    except Error as e:
+        # print("\nTable already exists. Skipping generation\n")
+        print(e)
+    return
 
 
 def create_new_db(
     db_name="db/main.db",
     table_name="main",
     table={
         "Dimer": "TEXT",
@@ -471,14 +473,42 @@
         print(
             "ERROR:\n\tEXITING FROM collect_id_into_js\n\n\tCheck that id is valid!\n"
         )
         os.sys.exit()
     return js
 
 
+def return_id_list(cur, column, table_name, id_name="id", values=[0]) -> [int]:
+    """
+    return_id_list queries db for matches with column and returns id
+    """
+    if len(values) == 1:
+        sql_cmd = (
+            f"""SELECT {id_name} FROM {table_name} WHERE {column}=={values[0]};"""
+        )
+    else:
+        sql_cmd = (
+            f"""SELECT {id_name} FROM {table_name} WHERE {column} IN {tuple(values)};"""
+        )
+    cur.execute(sql_cmd)
+    id_list = [i for i, *_ in cur.fetchall()]
+    return id_list
+
+def return_id_list_full_table(cur, table_name, id_name="id") -> [int]:
+    """
+    return_id_list queries db for matches with column and returns id
+    """
+    sql_cmd = (
+        f"""SELECT {id_name} FROM {table_name};"""
+    )
+    cur.execute(sql_cmd)
+    id_list = [i for i, *_ in cur.fetchall()]
+    return id_list
+
+
 def collect_ids_into_ls(
     cursor: object,
     id_list: [] = [0, 1],
     id_label: str = "main_id",
     table="main",
     outputs="*",
 ) -> []:
@@ -516,14 +546,41 @@
             extra_info,
             mem=mem,
         )
         for i in cursor.fetchall()
     ]
     return js_ls
 
+def collect_ids_into_ls(
+    cursor: object,
+    headers: [] = ["id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
+    id_list: [] = [0, 1],
+    id_label: str = "id",
+    table="tcase",
+    process_func=None,
+) -> []:
+    """
+    collect_rows collects a range of rows for a table with requested headers.
+    The headers list must match the dataclass_obj's fields.
+    """
+    cols = ", ".join(headers)
+    sql_cmd = (
+        f"""SELECT {cols} FROM {table} WHERE {table}.{id_label} IN {tuple(id_list)};"""
+    )
+    cursor.execute(sql_cmd)
+    if process_func:
+        ls = [
+            process_func(i)
+            for i in cursor.fetchall()
+        ]
+    else:
+        ls = [
+                i for i in cursor.fetchall()
+        ]
+    return ls
 
 def collect_rows_into_js_ls_mp(
     cursor: object,
     headers: [] = ["main_id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
     mem: str = "4gb",
     extra_info: [] = ["hf/aug-cc-pV(D+d)Z"],
     dataclass_obj: mp_js = mp_js,
```

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs/tools_og.py` & `hrcl_jobs-1.0.1/src/hrcl_jobs/tools_og.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.0/src/hrcl_jobs.egg-info/PKG-INFO` & `hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl-jobs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

