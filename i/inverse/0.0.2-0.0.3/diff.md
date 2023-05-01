# Comparing `tmp/inverse-0.0.2-py2.py3-none-any.whl.zip` & `tmp/inverse-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,59 @@
-Zip file size: 17326 bytes, number of entries: 29
--rw-rw-rw-  2.0 fat      216 b- defN 23-Apr-29 10:29 inverse/__init__.py
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-29 14:24 inverse/__version__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-29 10:42 inverse/src/__init__.py
--rw-rw-rw-  2.0 fat     2705 b- defN 23-Apr-29 10:35 inverse/src/abstract_data.py
--rw-rw-rw-  2.0 fat     1872 b- defN 23-Apr-29 10:37 inverse/src/abstract_data2.py
--rw-rw-rw-  2.0 fat     5178 b- defN 23-Apr-29 14:11 inverse/src/buffer_ops.py
--rw-rw-rw-  2.0 fat      122 b- defN 23-Apr-28 22:08 inverse/src/check_result.py
--rw-rw-rw-  2.0 fat     4262 b- defN 23-Apr-29 10:56 inverse/src/db_ops.py
--rw-rw-rw-  2.0 fat      307 b- defN 23-Apr-29 08:57 inverse/src/inverse_typings.py
--rw-rw-rw-  2.0 fat     1573 b- defN 23-Apr-29 11:24 inverse/src/main.py
--rw-rw-rw-  2.0 fat     2794 b- defN 23-Apr-29 14:23 inverse/src/matrix_converters.py
--rw-rw-rw-  2.0 fat      428 b- defN 23-Apr-29 13:53 inverse/src/partition.py
--rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-29 10:36 inverse/src/pickle_file.py
--rw-rw-rw-  2.0 fat      863 b- defN 23-Apr-29 10:38 inverse/src/pickle_works.py
--rw-rw-rw-  2.0 fat     2466 b- defN 23-Apr-29 10:37 inverse/src/randomMatrix.py
--rw-rw-rw-  2.0 fat     1014 b- defN 23-Apr-28 22:08 inverse/src/sc1.py
--rw-rw-rw-  2.0 fat     2864 b- defN 23-Apr-29 14:23 inverse/src/sp_matrix_ops.py
--rw-rw-rw-  2.0 fat     2353 b- defN 23-Apr-28 22:08 inverse/src/sp_utils_inverse.py
--rw-rw-rw-  2.0 fat      529 b- defN 23-Apr-28 22:08 inverse/src/sure.py
--rw-rw-rw-  2.0 fat      739 b- defN 23-Apr-29 10:37 inverse/src/tuple_for_buffer.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-29 10:41 inverse/tests/__init__.py
--rw-rw-rw-  2.0 fat      496 b- defN 23-Apr-29 11:05 inverse/tests/main_test.py
--rw-rw-rw-  2.0 fat     1193 b- defN 23-Apr-29 11:04 inverse/tests/tests.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-Apr-29 14:24 inverse-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1952 b- defN 23-Apr-29 14:24 inverse-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-29 14:24 inverse-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       49 b- defN 23-Apr-29 14:24 inverse-0.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-29 14:24 inverse-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2353 b- defN 23-Apr-29 14:24 inverse-0.0.2.dist-info/RECORD
-29 files, 37960 bytes uncompressed, 13544 bytes compressed:  64.3%
+Zip file size: 259360 bytes, number of entries: 57
+-rw-r--r--  2.0 fat      311 b- defN 80-Jan-01 00:00 inverse/__init__.py
+-rw-r--r--  2.0 fat        9 b- defN 80-Jan-01 00:00 inverse/__version__.py
+-rw-r--r--  2.0 fat     1365 b- defN 80-Jan-01 00:00 inverse/c_ext/vector_ops.c
+-rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/__init__.py
+-rw-r--r--  2.0 fat     1575 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/cdeneme.py
+-rw-r--r--  2.0 fat    16728 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clib
+-rw-r--r--  2.0 fat      230 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clib.c
+-rw-r--r--  2.0 fat   222942 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clibrary.so
+-rw-r--r--  2.0 fat    16232 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clibSHARED.so
+-rw-r--r--  2.0 fat     4349 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/ctypes_class.py
+-rw-r--r--  2.0 fat     2395 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/ctypes_class_float.py
+-rw-r--r--  2.0 fat      491 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/deneme_sum.py
+-rw-r--r--  2.0 fat      654 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/deneme_vector.py
+-rw-r--r--  2.0 fat     1803 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/lu_comp.c
+-rw-r--r--  2.0 fat     5683 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/restats
+-rw-r--r--  2.0 fat      473 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/sum.c
+-rw-r--r--  2.0 fat    16912 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops
+-rw-r--r--  2.0 fat     1882 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops.c
+-rw-r--r--  2.0 fat    90494 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops.so
+-rw-r--r--  2.0 fat   224109 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops2.so
+-rw-r--r--  2.0 fat    16528 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_opsSHARED.so
+-rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 inverse/src/__init__.py
+-rw-r--r--  2.0 fat     2212 b- defN 80-Jan-01 00:00 inverse/src/abstract_data.py
+-rw-r--r--  2.0 fat     1872 b- defN 80-Jan-01 00:00 inverse/src/abstract_data2.py
+-rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/__init__.py
+-rw-r--r--  2.0 fat      626 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/vector_nonvector.py
+-rw-r--r--  2.0 fat     4215 b- defN 80-Jan-01 00:00 inverse/src/buffer_ops.py
+-rw-r--r--  2.0 fat     5376 b- defN 80-Jan-01 00:00 inverse/src/buffer_ops_yedek.py
+-rw-r--r--  2.0 fat       93 b- defN 80-Jan-01 00:00 inverse/src/check_result.py
+-rw-r--r--  2.0 fat     4427 b- defN 80-Jan-01 00:00 inverse/src/db_ops.py
+-rw-r--r--  2.0 fat       41 b- defN 80-Jan-01 00:00 inverse/src/initial_checks_matrix.py
+-rw-r--r--  2.0 fat      307 b- defN 80-Jan-01 00:00 inverse/src/inverse_typings.py
+-rw-r--r--  2.0 fat     1653 b- defN 80-Jan-01 00:00 inverse/src/main.py
+-rw-r--r--  2.0 fat     1338 b- defN 80-Jan-01 00:00 inverse/src/main_funcs_to_load.py
+-rw-r--r--  2.0 fat     6689 b- defN 80-Jan-01 00:00 inverse/src/matrix_converters.py
+-rw-r--r--  2.0 fat       87 b- defN 80-Jan-01 00:00 inverse/src/measure_calls.py
+-rw-r--r--  2.0 fat      499 b- defN 80-Jan-01 00:00 inverse/src/partition.py
+-rw-r--r--  2.0 fat      500 b- defN 80-Jan-01 00:00 inverse/src/pickle_file.py
+-rw-r--r--  2.0 fat      863 b- defN 80-Jan-01 00:00 inverse/src/pickle_works.py
+-rw-r--r--  2.0 fat     2466 b- defN 80-Jan-01 00:00 inverse/src/randomMatrix.py
+-rw-r--r--  2.0 fat     3681 b- defN 80-Jan-01 00:00 inverse/src/sp_matrix_ops.py
+-rw-r--r--  2.0 fat     2892 b- defN 80-Jan-01 00:00 inverse/src/sp_utils_inverse.py
+-rw-r--r--  2.0 fat      297 b- defN 80-Jan-01 00:00 inverse/src/sure.py
+-rw-r--r--  2.0 fat      739 b- defN 80-Jan-01 00:00 inverse/src/tuple_for_buffer.py
+-rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 inverse/tests/__init__.py
+-rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 inverse/tests/C_tests/__init__.py
+-rw-r--r--  2.0 fat     1193 b- defN 80-Jan-01 00:00 inverse/tests/C_tests/c_tests.py
+-rw-r--r--  2.0 fat      689 b- defN 80-Jan-01 00:00 inverse/tests/main_test.py
+-rw-r--r--  2.0 fat     3207 b- defN 80-Jan-01 00:00 inverse/tests/mini_tests.py
+-rw-r--r--  2.0 fat      212 b- defN 80-Jan-01 00:00 inverse/tests/test_classes/test_buffer.py
+-rw-r--r--  2.0 fat     1458 b- defN 80-Jan-01 00:00 inverse/tests/test_matrix_op_main.py
+-rw-r--r--  2.0 fat     1508 b- defN 80-Jan-01 00:00 inverse/tests/tests.py
+-rw-r--r--  2.0 fat      317 b- defN 80-Jan-01 00:00 inverse/tests/tests_main.py
+-rw-r--r--  2.0 fat     1090 b- defN 80-Jan-01 00:00 inverse-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 fat     1780 b- defN 80-Jan-01 00:00 inverse-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 inverse-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat     4823 b- defN 16-Jan-01 00:00 inverse-0.0.3.dist-info/RECORD
+57 files, 682403 bytes uncompressed, 251686 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,55 +1,127 @@
 Filename: inverse/__init__.py
 Comment: 
 
 Filename: inverse/__version__.py
 Comment: 
 
+Filename: inverse/c_ext/vector_ops.c
+Comment: 
+
+Filename: inverse/ctypes_loc/__init__.py
+Comment: 
+
+Filename: inverse/ctypes_loc/cdeneme.py
+Comment: 
+
+Filename: inverse/ctypes_loc/clib
+Comment: 
+
+Filename: inverse/ctypes_loc/clib.c
+Comment: 
+
+Filename: inverse/ctypes_loc/clibrary.so
+Comment: 
+
+Filename: inverse/ctypes_loc/clibSHARED.so
+Comment: 
+
+Filename: inverse/ctypes_loc/ctypes_class.py
+Comment: 
+
+Filename: inverse/ctypes_loc/ctypes_class_float.py
+Comment: 
+
+Filename: inverse/ctypes_loc/deneme_sum.py
+Comment: 
+
+Filename: inverse/ctypes_loc/deneme_vector.py
+Comment: 
+
+Filename: inverse/ctypes_loc/lu_comp.c
+Comment: 
+
+Filename: inverse/ctypes_loc/restats
+Comment: 
+
+Filename: inverse/ctypes_loc/sum.c
+Comment: 
+
+Filename: inverse/ctypes_loc/vector_ops
+Comment: 
+
+Filename: inverse/ctypes_loc/vector_ops.c
+Comment: 
+
+Filename: inverse/ctypes_loc/vector_ops.so
+Comment: 
+
+Filename: inverse/ctypes_loc/vector_ops2.so
+Comment: 
+
+Filename: inverse/ctypes_loc/vector_opsSHARED.so
+Comment: 
+
 Filename: inverse/src/__init__.py
 Comment: 
 
 Filename: inverse/src/abstract_data.py
 Comment: 
 
 Filename: inverse/src/abstract_data2.py
 Comment: 
 
+Filename: inverse/src/benchmarks/__init__.py
+Comment: 
+
+Filename: inverse/src/benchmarks/vector_nonvector.py
+Comment: 
+
 Filename: inverse/src/buffer_ops.py
 Comment: 
 
+Filename: inverse/src/buffer_ops_yedek.py
+Comment: 
+
 Filename: inverse/src/check_result.py
 Comment: 
 
 Filename: inverse/src/db_ops.py
 Comment: 
 
+Filename: inverse/src/initial_checks_matrix.py
+Comment: 
+
 Filename: inverse/src/inverse_typings.py
 Comment: 
 
 Filename: inverse/src/main.py
 Comment: 
 
+Filename: inverse/src/main_funcs_to_load.py
+Comment: 
+
 Filename: inverse/src/matrix_converters.py
 Comment: 
 
+Filename: inverse/src/measure_calls.py
+Comment: 
+
 Filename: inverse/src/partition.py
 Comment: 
 
 Filename: inverse/src/pickle_file.py
 Comment: 
 
 Filename: inverse/src/pickle_works.py
 Comment: 
 
 Filename: inverse/src/randomMatrix.py
 Comment: 
 
-Filename: inverse/src/sc1.py
-Comment: 
-
 Filename: inverse/src/sp_matrix_ops.py
 Comment: 
 
 Filename: inverse/src/sp_utils_inverse.py
 Comment: 
 
 Filename: inverse/src/sure.py
@@ -57,32 +129,44 @@
 
 Filename: inverse/src/tuple_for_buffer.py
 Comment: 
 
 Filename: inverse/tests/__init__.py
 Comment: 
 
+Filename: inverse/tests/C_tests/__init__.py
+Comment: 
+
+Filename: inverse/tests/C_tests/c_tests.py
+Comment: 
+
 Filename: inverse/tests/main_test.py
 Comment: 
 
-Filename: inverse/tests/tests.py
+Filename: inverse/tests/mini_tests.py
+Comment: 
+
+Filename: inverse/tests/test_classes/test_buffer.py
 Comment: 
 
-Filename: inverse-0.0.2.dist-info/LICENSE
+Filename: inverse/tests/test_matrix_op_main.py
+Comment: 
+
+Filename: inverse/tests/tests.py
 Comment: 
 
-Filename: inverse-0.0.2.dist-info/METADATA
+Filename: inverse/tests/tests_main.py
 Comment: 
 
-Filename: inverse-0.0.2.dist-info/WHEEL
+Filename: inverse-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: inverse-0.0.2.dist-info/entry_points.txt
+Filename: inverse-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: inverse-0.0.2.dist-info/top_level.txt
+Filename: inverse-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: inverse-0.0.2.dist-info/RECORD
+Filename: inverse-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inverse/__init__.py

```diff
@@ -1,7 +1,9 @@
 # ------------------------------------------------------
 #
 #       __init__
 #                           package: inverse @2023
 # ------------------------------------------------------
-
+# import inverse
 from .src.main import *
+from .src.main_funcs_to_load import *
+from .ctypes_loc.cdeneme import test_c
```

## inverse/__version__.py

```diff
@@ -1 +1 @@
-#0.0.2
+#0.0.3rc2
```

## inverse/src/abstract_data.py

```diff
@@ -35,41 +35,18 @@
         """ save_part """
 
     @abstractmethod
     def save_on_begin_rand(self, matrix: npar) -> None:
         """save_on_begin_rand"""
 
 
-class DataAbstract22(ABC):
-    @abstractmethod
-    def get_original_matrix(self, n):
-        ...
-
-    @abstractmethod
-    def get_current_matrix(self, n):
-        ...
-
-    @abstractmethod
-    def get_row(self, r: int, stable=False):
-        ...
-
-    @abstractmethod
-    def set_row(self, i: int, data, name="name"):
-        ...
-
-    @abstractmethod
-    def get_cell(self, r: int, c: int):
-        ...
-
-    @abstractmethod
-    def save_on_begin_rand(self, n):
-        ...
 
 
 class PickleData(DataAbstract):
+
     def get_original_matrix(self, n) -> npar:
         rows = []
         for i in range(n):
             row = read_pickle("name_original" + str(i))
             rows.append(row)
         array = np.array(rows)
         return array[:, :n]
```

## inverse/src/buffer_ops.py

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from .db_ops import DB_class_Opt
 from .partition import get_table_name_treshold, table_name_format, column_name_format, table_name_format_reverse
 from .inverse_typings import *
+from .tuple_for_buffer import get_tuple_for_buffer
 
 
 def get_table_names_from_tuple(liste: list_tuple, threshold: int) -> list_tuple:
     new_set = []
     for i in liste:
         num = get_table_name_treshold(i, threshold)
         if num not in new_set:
@@ -37,30 +38,21 @@
     def get_current_matrix(self) -> npar:
         n = self.bigmatrix.n
         new_set = get_table_names_from_tuple(tuple(x for x in range(n)), self.threshold)
         self.load_buffer(new_set)
         matrix = self.buffer_to_matrix()
         return matrix
 
-    def buffer_get_current_key_nums(self) -> tuple:
-        keys = tuple(self.buffer_data.keys())
-        result = tuple(map(table_name_format_reverse, keys))
-
-        return result
-
     def buffer_key_format(self, say: int) -> str:
         return table_name_format(self.name, say)
 
-    def load_buffer(self, diff_set: list_tuple) -> None:
+    def load_buffer(self, new_set: list_tuple) -> None:
         """burada desteleri yükleyecek"""
-        # if diff_set == ("0",):
-        #     return
-        # print("loading", diff_set)
-
-        for set_say in diff_set:
+        # print("loading new set ...", new_set)
+        for set_say in new_set:
             # num = get_table_name_treshold(say, self.threshold)
             table_name = table_name_format(self.name, set_say)
             buffer_key = self.buffer_key_format(set_say)
             try:
                 df_gelen = DB_class_Opt.read_db(table_name)
                 for column in tuple(df_gelen.columns):
                     self.columns_tables_dict[column] = buffer_key
@@ -73,52 +65,33 @@
     def save_buffer(self) -> None:
         for table_name in tuple(self.buffer_data.keys()):
             try:
                 DB_class_Opt.write_db(table_name, self.buffer_data[table_name])
             except:
                 print("bunu bulamadım save_buffer ", table_name)
 
-    def empty_buffer(self, tuple_set=()) -> None:
+    def empty_buffer(self) -> None:
         self.save_buffer()
-        if tuple_set:
-            for item in tuple_set:
-                self.buffer_data.pop(item)
-        else:
-            self.buffer_data = {}
+        self.buffer_data = {}
 
     def refresh_buffer(self, new_set: list_tuple) -> None:
-        old_set = self.buffer_get_current_key_nums()
-        diff_set_garbage = tuple(x for x in old_set if x not in new_set)
-        diff_set_load = tuple(x for x in new_set if x not in old_set)
-
-        # print("old_set", old_set)
-        # print("diff_set_garbage", diff_set_garbage)
-        # print("diff_set_load", diff_set_load)
-        # print("new_set", new_set)
-        # exit()
-        # if not old_set :
-        #     diff_set_load = new_set
-        self.empty_buffer(diff_set_garbage)
-        self.load_buffer(diff_set_load)
+        self.empty_buffer()
+        self.load_buffer(new_set)
 
     def load_column_names_with_set(self, column_tuple: list_tuple) -> None:
-        column_tuple = tuple(set(column_tuple))
-
-        # print("load_column_names_with_set column_tuple", column_tuple)
         new_set = get_table_names_from_tuple(column_tuple, self.threshold)
-        # print("load_column_names_with_set new_set", new_set)
-
         self.refresh_buffer(new_set)
 
     def setItem(self, num: int, i: int, data: list_tuple) -> None:
         buffer_key = self.buffer_key_format(num)
         df = self.buffer_data[buffer_key]
+        new_df = df.copy()
         keyname = column_name_format(i)
-        df[keyname] = data
-        self.buffer_data[buffer_key] = df
+        new_df[keyname] = data
+        self.buffer_data[buffer_key] = new_df
 
     def get_column(self, i: int) -> pddf:
         column = column_name_format(i)
         keyName = self.columns_tables_dict[column]
         return self.buffer_data[keyName]
 
     def get_cell(self, j: int, i: int) -> int_float:
```

## inverse/src/check_result.py

```diff
@@ -1,6 +1,6 @@
 
-#filename:check_result.py
-#folder:
-import numpy as np
+
 def inverse_check(matrix ):
+    import numpy as np
+
     return np.linalg.inv(matrix)
```

## inverse/src/db_ops.py

```diff
@@ -3,14 +3,16 @@
 #   bkz README.md.
 import math
 import shutil
 from pathlib import Path
 import pandas as pd
 import sqlite3
 from dataclasses import dataclass
+
+from .measure_calls import CallStack
 from .partition import get_name_from_i, get_table_name_treshold
 from .inverse_typings import *
 
 import os
 
 
 @dataclass
@@ -81,19 +83,24 @@
 
 app_sql = APP_SQL()
 
 
 class DB_class_Opt(Protocol):
     @staticmethod
     def read_db(name: str) -> pddf:
+        global CallStack
+        CallStack["read_db"] += 1
         df = app_sql.read_table(name)
         return df
 
     @staticmethod
     def write_db(name: str, df: pddf) -> None:
+        global CallStack
+
+        CallStack["write_db"] += 1
         if "level_0" in tuple(df.columns):
             df = df.drop(['level_0'], axis=1)
         app_sql.add_table(name, df)
 
     @staticmethod
     def merge(df, columns, buffer):
         new_df = df
```

## inverse/src/main.py

```diff
@@ -1,19 +1,23 @@
 
-import numpy as np
-from .check_result import inverse_check
+# import numpy as np
+
 from .matrix_converters import BigMatrixConverter
 from .randomMatrix import get_rand_matrix_int_seed, get_rand_matrix_int_noseed
 from .sp_matrix_ops import display_matrix_ozet
 from .sp_utils_inverse import close_identity
 from .sure import tic, toc
+
+
 def get_matrix_for_test(n):
     return get_rand_matrix_int_seed(n)
     # return get_rand_matrix_int_noseed(n)
 def main():
+    from .check_result import inverse_check
+    import numpy as np
     n = 10 #                   100 : 16sn ,10:1sn
     threshold = 500
     matrix = get_matrix_for_test(n)
     print(matrix)
     matrix_check = inverse_check(matrix)
     converter = BigMatrixConverter("test")
     big_matrix = converter.convert_small_to_bigmatrix(matrix, threshold=threshold)  # class bigMatrix
@@ -38,8 +42,10 @@
 
 def a2():
     tic()
     n = 60
     threshold = 500
     matrix = get_matrix_for_test(n)
     
-    toc()
+    toc()
+
+__all__ = ["get_matrix_for_test" , "a2"]
```

## inverse/src/matrix_converters.py

```diff
@@ -1,16 +1,21 @@
 from typing import Protocol
 
-import numpy as np
+from rich.progress import Progress
 
+from inverse.ctypes_loc.ctypes_class import c_divide, c_multiply, py_operate_inside_double
 from .abstract_data import id_ekle
 from .abstract_data2 import DBDataOpt
 from .buffer_ops import Buffer
+from .check_result import inverse_check
+from .measure_calls import CallStack
 from .tuple_for_buffer import get_tuple_for_buffer
-from .sp_matrix_ops import combine_row_op, divide_pivot
+from .sp_matrix_ops import combine_row_op, divide_pivot, display_matrix_ozet, divide_pivot_eski, combine_row_op_eski
+
+import numpy as np
 
 
 class MatrixCreator(Protocol):
     ...
 
 
 class BigMatrix:
@@ -33,51 +38,154 @@
 
     def inverse(self):
         print("I am a big matrix")
         inverse_mat = self.sp_inverse()
         return self
 
     def save_on_begin_rand(self, matrix: np.array):
+
         self.db_rep.save_on_begin_rand(matrix)
 
+    def save_on_begin_bigmatrix_lines(self, lines):
+
+        self.db_rep.save_on_begin_bigmatrix_lines(lines)
+
     def sp_inverse(self) -> np.array:
         """TODO"""
+        global CallStack
+        from inverse import tic, toc
+
+        tic()
+        bucket = get_tuple_for_buffer(self.n, self.threshold)
+        for sira in bucket:
+            CallStack["dıs_dongu"] += 1
+            sira = tuple(int(x) for x in sira if x < self.n and x > -1)
+            i, *y = sira
+            y = tuple(set(y))
 
-        for sira in get_tuple_for_buffer(self.n, self.threshold):
-            sira = tuple(x for x in sira if x < self.n)
-            x, *y = sira
             self.buffer.load_column_names_with_set(sira)
-            # print("now x " , x , sira )
-            for i in [x]:
-                # print("Sıradaki satır numarası : ", i, "*" * 10)
-                row = tuple(self.buffer.get_row(i))
-                pivot = row[i]
-                row = divide_pivot(row, pivot)
-                self.buffer.set_row(i, row)
-                for j in y:
-                    if i != j:
-                        number_j = self.buffer.get_cell(j, i)
-                        number_i = self.buffer.get_cell(i, i)
-                        if number_i != 0:
-                            factor = number_j / number_i
-                        else:
-                            factor = 0
-                        row_J = self.buffer.get_row(j)
-                        row_i = self.buffer.get_row(i)
-                        nrow = combine_row_op(row_J, row_i, factor)
-                        self.buffer.set_row(j, nrow)
-            self.buffer.final_save()
+            # for i in [x]:
+            row = tuple(self.buffer.get_row(i))
+            pivot = row[i]
+
+            row = c_divide(row, pivot)
+
+            # SET Calculation
+            self.buffer.set_row(i, row)
+
+            for j in (a for a in y if a != i):
+                CallStack["ic_dongu"] += 1
+                number_j = self.buffer.get_cell(j, i)  # 1 number
+                number_i = self.buffer.get_cell(i, i)  # 2 number
+
+                # factor = number_j / number_i if number_i != 0 else 0
+                row_J = np.array(self.buffer.get_row(j))  # 3 array
+                row_i = np.array(self.buffer.get_row(i))  # 4 array
+                # nrow = row_J - c_multiply(row_i, factor)
+
+                nrow = py_operate_inside_double(number_j, number_i, row_J, row_i, len(row_J))
+
+                # SET Calculation
+
+                self.buffer.set_row(j, nrow)
+
+        self.buffer.final_save()
+        toc()
         inv_matrix = self.buffer.get_current_matrix()
         self.id_and_inv = inv_matrix
+        # print(inv_matrix)
+
         return inv_matrix[:, self.n:]
 
+    def sp_inverse_progress(self) -> np.array:
+        """TODO"""
+        global CallStack
+
+        with Progress() as progress:
+            bucket = get_tuple_for_buffer(self.n, self.threshold)
+            task1 = progress.add_task("[red]Calculating...", total=len(bucket))
+            for sira in bucket:
+                CallStack["dıs_dongu"] += 1
+                progress.update(task1, advance=1)
+                # sira = tuple(x for x in sira if x < self.n)
+                sira = tuple(int(x) for x in sira if x < self.n and x > -1)
+                x, *y = sira
+                y = tuple(set(y))
+
+                self.buffer.load_column_names_with_set(sira)
+                print("now x ", x, sira)
+                for i in [x]:
+
+                    row = tuple(self.buffer.get_row(i))
+                    pivot = row[i]
+
+                    print("Sıradaki satır numarası : ", i, "pivot :  ", pivot, "row", row, "*" * 10)
+                    # exit()
+                    row = divide_pivot(row, pivot)
+                    self.buffer.set_row(i, row)
+                    for j in y:
+                        if i != j:
+
+                            CallStack["ic_dongu"] += 1
+
+                            number_j = self.buffer.get_cell(j, i)
+                            number_i = self.buffer.get_cell(i, i)
+                            if number_i != 0:
+                                factor = number_j / number_i
+                            else:
+                                factor = 0
+                            row_J = self.buffer.get_row(j)
+                            row_i = self.buffer.get_row(i)
+                            nrow = combine_row_op(row_J, row_i, factor)
+                            self.buffer.set_row(j, nrow)
+                            # print("setting nrow " , nrow )
+        self.buffer.final_save()
+        inv_matrix = self.buffer.get_current_matrix()
+        self.id_and_inv = inv_matrix
+        # print(inv_matrix)
+        # return inv_matrix[:, self.n:]
+        return inv_matrix
+
 
 class BigMatrixConverter:
     def __init__(self, name):
         self.name = name
 
     def convert_small_to_bigmatrix(self,
                                    matrix: np.array,
                                    threshold: int) -> BigMatrix:
         big_matrix = BigMatrix(self.name, len(matrix), threshold)
         big_matrix.db_rep.save_on_begin_rand(matrix)
         return big_matrix
+
+    def create_bigmatrix_from_lines(self, lines, name="test", threshold: int = 5) -> BigMatrix:
+        ...
+        big_matrix = BigMatrix(self.name, len(lines), threshold)
+        big_matrix.db_rep.save_on_begin_rand(lines)
+        return big_matrix
+
+
+def test_small_matrix():
+    from inverse import tic, toc, close_identity
+    threshold = 500
+    matrix = np.array([[19, 2, 3],
+                       [8, 3, 6],
+                       [7, 8, 15]])
+    big_matrix = BigMatrixConverter("test").convert_small_to_bigmatrix(matrix, threshold)
+    inverse_mat = big_matrix.sp_inverse()
+    # inverse_mat2 = big_matrix.sp_inverse_progress()
+    matrix_check = inverse_check(matrix)
+
+    print(matrix, "matrix")
+    print(inverse_mat, "inverse_mat")
+    # print(inverse_mat2, "inverse_mat2")
+    print(matrix_check, "matrix_check")
+
+    sonuc1 = np.matmul(matrix, inverse_mat)
+    # sonuc2 = np.matmul(matrix, inverse_mat2)
+    sonuc3 = np.matmul(matrix, matrix_check)
+
+    eps = 0.0001
+    kontrol = close_identity(matrix=sonuc1, eps=eps)
+    # kontrol2 = close_identity(matrix=sonuc2, eps=eps)
+    kontrol2 = close_identity(matrix=sonuc3, eps=eps)
+    print(CallStack)
```

## inverse/src/partition.py

```diff
@@ -1,18 +1,19 @@
 import math
+from functools import lru_cache
 
 
 def table_name_format(name, say):
     return f"{name}_{say}"
 
 
 def table_name_format_reverse(name: str) -> int:
     return int(name.split("_")[1])
 
-
+# @lru_cache(maxsize=128, typed=False)
 def column_name_format(i):
     return f"column_{i}"
 
 
 def get_table_name_treshold(i, treshold):
     i = int(i)
     return math.floor(i / treshold)
```

## inverse/src/pickle_file.py

```diff
@@ -1,14 +1,17 @@
 
 
 import pickle
 from pathlib import Path
 pickle_folder = "pickles"
 from .inverse_typings import *
 
+import os
+if not os.path.exists(pickle_folder):
+    os.makedirs(pickle_folder)
 
 def save_pickle(name, data):
     with open(Path(pickle_folder) / (str(name) + '.pickle'), 'wb') as f:
         pickle.dump(data, f)
 def read_pickle(name):
     new_data = False
     with open(Path(pickle_folder) / (str(name) + '.pickle'), 'rb') as f:
```

## inverse/src/sp_matrix_ops.py

```diff
@@ -35,15 +35,15 @@
 
 def ozet_show(items: list_tuple,
               limit=5, all=False) -> None:
     if len(items) < limit or all:
         a = items[:]
     else:
         a = items[0:limit]
-    b = (str(round(x, 2)) for x in list(a))
+    b = (str(round(x, 2)) for x in a if type(x) !=type(None )  )
     c = " ".join(b)
     if len(items) > limit:
         print(f"[{c}...]")
     else:
         print(f"[{c}]")
 
 
@@ -78,32 +78,62 @@
 
 # --------------------------- Abstract ------------------
 def save_on_begin(matrix: npar) -> None:
     n = len(matrix)
     for i in range(n):
         save_pickle("name" + str(i), matrix[i])
 
-#@njit
+
+from inverse.ctypes_loc.ctypes_class import c_divide, c_multiply
+
+
 def divide_pivot(row: list_tuple, pivot: int_float) -> tuple:
+    if pivot == 0:
+        raise ZeroDivisionError
+    return c_divide(row, pivot)
+
     # print(pivot ,"pivot")
     assert isinstance(row, (tuple, list))
     assert isinstance(pivot, (int, float))
     row = np.array(row)
     if pivot != 0:
-        #row = (x / pivot for x in row)
-        row = row / pivot # (x / pivot for x in row)
+        # row = (x / pivot for x in row)
+        row = row / pivot  # (x / pivot for x in row)
+    else:
+        raise ZeroDivisionError
+
+    return tuple(row)
+
+
+def divide_pivot_eski(row: list_tuple, pivot: int_float) -> tuple:
+    assert isinstance(row, (tuple, list))
+    assert isinstance(pivot, (int, float))
+    row = np.array(row)
+    if pivot != 0:
+        # row = (x / pivot for x in row)
+        row = row / pivot  # (x / pivot for x in row)
     else:
-        row = (0 for _ in row)
+        raise ZeroDivisionError
+
     return tuple(row)
 
-#@njit
 def combine_row_op(row_J: list_tuple,
                    row_i: list_tuple,
                    factor: int_float) -> list:
     row_J = np.array(row_J)
     row_i = np.array(row_i)
-    return row_J - row_i * factor
-    result = []
-    for j_number, i_number in zip(row_J, row_i):
 
-        result.append(j_number - i_number * factor)
-    return result
+    return row_J - c_multiply(row_i, factor)
+
+
+# @njit
+def combine_row_op_eski(row_J: list_tuple,
+                          row_i: list_tuple,
+                          factor: int_float) -> list:
+    row_J = np.array(row_J)
+    row_i = np.array(row_i)
+    return row_J - row_i * factor
+    # result = []
+    # for j_number, i_number in zip(row_J, row_i):
+    #
+    #     result.append(j_number - i_number * factor)
+    # return result
```

## inverse/src/sp_utils_inverse.py

```diff
@@ -1,148 +1,181 @@
-00000000: 0d0a 2366 696c 656e 616d 653a 7370 5f75  ..#filename:sp_u
-00000010: 7469 6c73 5f69 6e76 6572 7365 2e70 790d  tils_inverse.py.
-00000020: 0a23 666f 6c64 6572 3a0d 0a23 2020 2053  .#folder:..#   S
-00000030: 6572 6d65 742e 5065 6b69 6e20 3230 3233  ermet.Pekin 2023
-00000040: 0d0a 2320 2020 6d61 7472 6978 206f 7073  ..#   matrix ops
-00000050: 0d0a 2320 2020 626b 7a20 5245 4144 4d45  ..#   bkz README
-00000060: 2e6d 642e 0d0a 696d 706f 7274 2072 616e  .md...import ran
-00000070: 646f 6d0d 0a69 6d70 6f72 7420 6e75 6d70  dom..import nump
-00000080: 7920 6173 206e 700d 0a64 6566 206b 6579  y as np..def key
-00000090: 5f66 6f72 6d61 7428 722c 206e 616d 653d  _format(r, name=
-000000a0: 226e 616d 6522 293a 0d0a 2020 2020 7265  "name"):..    re
-000000b0: 7475 726e 2066 227b 6e61 6d65 7d5f 7b72  turn f"{name}_{r
-000000c0: 7d22 0d0a 6465 6620 6d65 6d6f 7279 5f74  }"..def memory_t
-000000d0: 6573 7428 6e2c 2072 6f77 3d31 3029 3a0d  est(n, row=10):.
-000000e0: 0a20 2020 2023 206e 756d 6265 7273 203d  .    # numbers =
-000000f0: 206c 6973 7428 7261 6e64 6f6d 2e72 616e   list(random.ran
-00000100: 6469 6e74 2830 2c20 3130 3029 2066 6f72  dint(0, 100) for
-00000110: 205f 2069 6e20 7261 6e67 6528 6e29 290d   _ in range(n)).
-00000120: 0a20 2020 2062 6967 5f6e 756d 6265 7273  .    big_numbers
-00000130: 203d 205b 5d0d 0a20 2020 2066 6f72 2069   = []..    for i
-00000140: 2069 6e20 7261 6e67 6528 726f 7729 3a0d   in range(row):.
-00000150: 0a20 2020 2020 2020 2023 206e 756d 6265  .        # numbe
-00000160: 7273 203d 206c 6973 7428 726f 756e 6428  rs = list(round(
-00000170: 7261 6e64 6f6d 2e75 6e69 666f 726d 2830  random.uniform(0
-00000180: 2c20 3130 3030 3030 3029 2c20 3229 2066  , 1000000), 2) f
-00000190: 6f72 205f 2069 6e20 7261 6e67 6528 6e29  or _ in range(n)
-000001a0: 290d 0a20 2020 2020 2020 206e 756d 6265  )..        numbe
-000001b0: 7273 203d 206c 6973 7428 7261 6e64 6f6d  rs = list(random
-000001c0: 2e72 616e 6469 6e74 2830 2c20 315f 3030  .randint(0, 1_00
-000001d0: 305f 3030 3029 2066 6f72 205f 2069 6e20  0_000) for _ in 
-000001e0: 7261 6e67 6528 6e29 290d 0a20 2020 2020  range(n))..     
-000001f0: 2020 2070 7269 6e74 286c 656e 286e 756d     print(len(num
-00000200: 6265 7273 2929 0d0a 2020 2020 2020 2020  bers))..        
-00000210: 6269 675f 6e75 6d62 6572 732e 6170 7065  big_numbers.appe
-00000220: 6e64 286e 756d 6265 7273 290d 0a20 2020  nd(numbers)..   
-00000230: 2070 7269 6e74 286c 656e 2862 6967 5f6e   print(len(big_n
-00000240: 756d 6265 7273 2929 0d0a 2020 2020 6220  umbers))..    b 
-00000250: 3d20 6e70 2e61 7272 6179 2862 6967 5f6e  = np.array(big_n
-00000260: 756d 6265 7273 290d 0a20 2020 2072 6574  umbers)..    ret
-00000270: 7572 6e20 620d 0a64 6566 2063 6c6f 7365  urn b..def close
-00000280: 5f65 6e6f 7567 6828 7361 7969 2c20 6275  _enough(sayi, bu
-00000290: 6e61 2c20 6570 7329 3a0d 0a20 2020 2072  na, eps):..    r
-000002a0: 6574 7572 6e20 6162 7328 7361 7969 202d  eturn abs(sayi -
-000002b0: 2062 756e 6129 203c 2065 7073 0d0a 6465   buna) < eps..de
-000002c0: 6620 696e 7665 7273 6528 6d61 7429 3a0d  f inverse(mat):.
-000002d0: 0a20 2020 2066 726f 6d20 7363 6970 7920  .    from scipy 
-000002e0: 696d 706f 7274 206c 696e 616c 670d 0a20  import linalg.. 
-000002f0: 2020 2072 6574 7572 6e20 6c69 6e61 6c67     return linalg
-00000300: 2e69 6e76 286d 6174 2c20 6f76 6572 7772  .inv(mat, overwr
-00000310: 6974 655f 613d 5472 7565 290d 0a20 2020  ite_a=True)..   
-00000320: 2023 2072 6574 7572 6e20 6e70 2e6c 696e   # return np.lin
-00000330: 616c 672e 696e 7628 6d61 7429 0d0a 636c  alg.inv(mat)..cl
-00000340: 6173 7320 4e6f 7449 6465 6e74 6974 7928  ass NotIdentity(
-00000350: 4261 7365 4578 6365 7074 696f 6e29 3a0d  BaseException):.
-00000360: 0a20 2020 2022 2222 4e6f 7420 616e 2049  .    """Not an I
-00000370: 6465 6e74 6974 7920 4d61 7472 6978 2222  dentity Matrix""
-00000380: 220d 0a64 6566 2063 6c6f 7365 5f69 6465  "..def close_ide
-00000390: 6e74 6974 795f 6f70 7469 6d69 7a65 6428  ntity_optimized(
-000003a0: 6e2c 2065 7073 2c20 6461 7461 5f73 6f75  n, eps, data_sou
-000003b0: 7263 6529 3a0d 0a20 2020 2023 2061 7567  rce):..    # aug
-000003c0: 5f6d 6174 7269 7820 3d20 6e70 2e63 6f6c  _matrix = np.col
-000003d0: 756d 6e5f 7374 6163 6b28 286d 6174 7269  umn_stack((matri
-000003e0: 782c 206e 702e 6964 656e 7469 7479 286e  x, np.identity(n
-000003f0: 2929 290d 0a20 2020 2066 6f72 2069 2069  )))..    for i i
-00000400: 6e20 7261 6e67 6528 6e29 3a0d 0a20 2020  n range(n):..   
-00000410: 2020 2020 2070 6976 6f74 203d 2064 6174       pivot = dat
-00000420: 615f 736f 7572 6365 2e67 6574 5f72 6f77  a_source.get_row
-00000430: 2869 295b 695d 0d0a 2020 2020 2020 2020  (i)[i]..        
-00000440: 6966 2063 6c6f 7365 5f65 6e6f 7567 6828  if close_enough(
-00000450: 7069 766f 742c 2031 2c20 6570 7329 3a0d  pivot, 1, eps):.
-00000460: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
-00000470: 7567 5f6d 6174 7269 785b 695d 203d 2061  ug_matrix[i] = a
-00000480: 7567 5f6d 6174 7269 785b 695d 202f 2070  ug_matrix[i] / p
-00000490: 6976 6f74 0d0a 2020 2020 2020 2020 2020  ivot..          
-000004a0: 2020 2e2e 2e0d 0a20 2020 2020 2020 2065    .....        e
-000004b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000004c0: 2020 7261 6973 6520 4e6f 7449 6465 6e74    raise NotIdent
-000004d0: 6974 790d 0a20 2020 2020 2020 2066 6f72  ity..        for
-000004e0: 206a 2069 6e20 7261 6e67 6528 6e29 3a0d   j in range(n):.
-000004f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000500: 6920 213d 206a 3a0d 0a20 2020 2020 2020  i != j:..       
-00000510: 2020 2020 2020 2020 206e 756d 6265 7220           number 
-00000520: 3d20 6461 7461 5f73 6f75 7263 652e 6765  = data_source.ge
-00000530: 745f 726f 7728 6929 5b6a 5d0d 0a20 2020  t_row(i)[j]..   
-00000540: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000550: 636c 6f73 655f 656e 6f75 6768 286e 756d  close_enough(num
-00000560: 6265 722c 2030 2c20 6570 7329 3a0d 0a20  ber, 0, eps):.. 
-00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000580: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
-00000590: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2072 6169 7365 204e 6f74 4964 656e     raise NotIden
-000005c0: 7469 7479 0d0a 2020 2020 7072 696e 7428  tity..    print(
-000005d0: 2245 7665 7420 4275 2062 6972 2049 6465  "Evet Bu bir Ide
-000005e0: 6e74 6974 7920 6d61 7472 6978 2229 0d0a  ntity matrix")..
-000005f0: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-00000600: 0a64 6566 206e 6f74 5f72 6169 7365 2864  .def not_raise(d
-00000610: 6f6e 745f 7261 6973 6529 3a0d 0a20 2020  ont_raise):..   
-00000620: 2069 6620 646f 6e74 5f72 6169 7365 3a0d   if dont_raise:.
-00000630: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00000640: 4e6f 7420 4964 656e 7469 7479 206d 6174  Not Identity mat
-00000650: 7269 7822 290d 0a20 2020 2020 2020 2072  rix")..        r
-00000660: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-00000670: 656c 7365 3a0d 0a20 2020 2020 2020 2072  else:..        r
-00000680: 6169 7365 204e 6f74 4964 656e 7469 7479  aise NotIdentity
-00000690: 0d0a 6465 6620 636c 6f73 655f 6964 656e  ..def close_iden
-000006a0: 7469 7479 286d 6174 7269 782c 2065 7073  tity(matrix, eps
-000006b0: 293a 0d0a 2020 2020 6e20 3d20 6c65 6e28  ):..    n = len(
-000006c0: 6d61 7472 6978 290d 0a20 2020 2023 2061  matrix)..    # a
-000006d0: 7567 5f6d 6174 7269 7820 3d20 6e70 2e63  ug_matrix = np.c
-000006e0: 6f6c 756d 6e5f 7374 6163 6b28 286d 6174  olumn_stack((mat
-000006f0: 7269 782c 206e 702e 6964 656e 7469 7479  rix, np.identity
-00000700: 286e 2929 290d 0a20 2020 2066 6f72 2069  (n)))..    for i
-00000710: 2069 6e20 7261 6e67 6528 6e29 3a0d 0a20   in range(n):.. 
-00000720: 2020 2020 2020 2070 6976 6f74 203d 206d         pivot = m
-00000730: 6174 7269 785b 695d 5b69 5d0d 0a20 2020  atrix[i][i]..   
-00000740: 2020 2020 2069 6620 636c 6f73 655f 656e       if close_en
-00000750: 6f75 6768 2870 6976 6f74 2c20 312c 2065  ough(pivot, 1, e
-00000760: 7073 293a 0d0a 2020 2020 2020 2020 2020  ps):..          
-00000770: 2020 2320 6175 675f 6d61 7472 6978 5b69    # aug_matrix[i
-00000780: 5d20 3d20 6175 675f 6d61 7472 6978 5b69  ] = aug_matrix[i
-00000790: 5d20 2f20 7069 766f 740d 0a20 2020 2020  ] / pivot..     
-000007a0: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
-000007b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000007c0: 2020 2020 2020 206e 6f74 5f72 6169 7365         not_raise
-000007d0: 2854 7275 6529 0d0a 2020 2020 2020 2020  (True)..        
-000007e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000007f0: 0d0a 2020 2020 2020 2020 666f 7220 6a20  ..        for j 
-00000800: 696e 2072 616e 6765 286e 293a 0d0a 2020  in range(n):..  
-00000810: 2020 2020 2020 2020 2020 6966 2069 2021            if i !
-00000820: 3d20 6a3a 0d0a 2020 2020 2020 2020 2020  = j:..          
-00000830: 2020 2020 2020 6e75 6d62 6572 203d 206d        number = m
-00000840: 6174 7269 785b 695d 5b6a 5d0d 0a20 2020  atrix[i][j]..   
-00000850: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000860: 636c 6f73 655f 656e 6f75 6768 286e 756d  close_enough(num
-00000870: 6265 722c 2030 2c20 6570 7329 3a0d 0a20  ber, 0, eps):.. 
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
-000008a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2020 206e 6f74 5f72 6169 7365 2854 7275     not_raise(Tru
-000008d0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-000008e0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000008f0: 616c 7365 0d0a 2020 2020 7072 696e 7428  alse..    print(
-00000900: 2245 7665 7420 4275 2062 6972 2049 6465  "Evet Bu bir Ide
-00000910: 6e74 6974 7920 6d61 7472 6978 2229 0d0a  ntity matrix")..
-00000920: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-00000930: 0a                                       .
+00000000: 2320 2020 5365 726d 6574 2e50 656b 696e  #   Sermet.Pekin
+00000010: 2032 3032 330d 0a23 2020 206d 6174 7269   2023..#   matri
+00000020: 7820 6f70 730d 0a23 2020 2062 6b7a 2052  x ops..#   bkz R
+00000030: 4541 444d 452e 6d64 2e0d 0a69 6d70 6f72  EADME.md...impor
+00000040: 7420 7261 6e64 6f6d 0d0a 696d 706f 7274  t random..import
+00000050: 206e 756d 7079 2061 7320 6e70 0d0a 0d0a   numpy as np....
+00000060: 6d73 675f 636f 7272 6563 746f 203d 2022  msg_correcto = "
+00000070: 436f 7272 6563 742c 2074 6869 7320 6973  Correct, this is
+00000080: 2049 6465 6e74 6974 7920 6d61 7472 6978   Identity matrix
+00000090: 220d 0a6d 7367 5f6e 6f74 5f63 6f72 7265  "..msg_not_corre
+000000a0: 6374 6f20 3d20 2254 6869 7320 6973 2049  cto = "This is I
+000000b0: 6465 6e74 6974 7920 6d61 7472 6978 220d  dentity matrix".
+000000c0: 0a0d 0a0d 0a64 6566 206b 6579 5f66 6f72  .....def key_for
+000000d0: 6d61 7428 722c 206e 616d 653d 226e 616d  mat(r, name="nam
+000000e0: 6522 293a 0d0a 2020 2020 7265 7475 726e  e"):..    return
+000000f0: 2066 227b 6e61 6d65 7d5f 7b72 7d22 0d0a   f"{name}_{r}"..
+00000100: 0d0a 0d0a 6465 6620 6d65 6d6f 7279 5f74  ....def memory_t
+00000110: 6573 7428 6e2c 2072 6f77 3d31 3029 3a0d  est(n, row=10):.
+00000120: 0a20 2020 2023 206e 756d 6265 7273 203d  .    # numbers =
+00000130: 206c 6973 7428 7261 6e64 6f6d 2e72 616e   list(random.ran
+00000140: 6469 6e74 2830 2c20 3130 3029 2066 6f72  dint(0, 100) for
+00000150: 205f 2069 6e20 7261 6e67 6528 6e29 290d   _ in range(n)).
+00000160: 0a20 2020 2062 6967 5f6e 756d 6265 7273  .    big_numbers
+00000170: 203d 205b 5d0d 0a20 2020 2066 6f72 2069   = []..    for i
+00000180: 2069 6e20 7261 6e67 6528 726f 7729 3a0d   in range(row):.
+00000190: 0a20 2020 2020 2020 2023 206e 756d 6265  .        # numbe
+000001a0: 7273 203d 206c 6973 7428 726f 756e 6428  rs = list(round(
+000001b0: 7261 6e64 6f6d 2e75 6e69 666f 726d 2830  random.uniform(0
+000001c0: 2c20 3130 3030 3030 3029 2c20 3229 2066  , 1000000), 2) f
+000001d0: 6f72 205f 2069 6e20 7261 6e67 6528 6e29  or _ in range(n)
+000001e0: 290d 0a20 2020 2020 2020 206e 756d 6265  )..        numbe
+000001f0: 7273 203d 206c 6973 7428 7261 6e64 6f6d  rs = list(random
+00000200: 2e72 616e 6469 6e74 2830 2c20 315f 3030  .randint(0, 1_00
+00000210: 305f 3030 3029 2066 6f72 205f 2069 6e20  0_000) for _ in 
+00000220: 7261 6e67 6528 6e29 290d 0a20 2020 2020  range(n))..     
+00000230: 2020 2070 7269 6e74 286c 656e 286e 756d     print(len(num
+00000240: 6265 7273 2929 0d0a 2020 2020 2020 2020  bers))..        
+00000250: 6269 675f 6e75 6d62 6572 732e 6170 7065  big_numbers.appe
+00000260: 6e64 286e 756d 6265 7273 290d 0a20 2020  nd(numbers)..   
+00000270: 2070 7269 6e74 286c 656e 2862 6967 5f6e   print(len(big_n
+00000280: 756d 6265 7273 2929 0d0a 2020 2020 6220  umbers))..    b 
+00000290: 3d20 6e70 2e61 7272 6179 2862 6967 5f6e  = np.array(big_n
+000002a0: 756d 6265 7273 290d 0a20 2020 2072 6574  umbers)..    ret
+000002b0: 7572 6e20 620d 0a0d 0a0d 0a64 6566 2063  urn b......def c
+000002c0: 6c6f 7365 5f65 6e6f 7567 6828 7361 7969  lose_enough(sayi
+000002d0: 2c20 6275 6e61 2c20 6570 7329 3a0d 0a20  , buna, eps):.. 
+000002e0: 2020 2072 6574 7572 6e20 6162 7328 7361     return abs(sa
+000002f0: 7969 202d 2062 756e 6129 203c 2065 7073  yi - buna) < eps
+00000300: 0d0a 0d0a 0d0a 6465 6620 696e 7665 7273  ......def invers
+00000310: 6528 6d61 7429 3a0d 0a20 2020 2066 726f  e(mat):..    fro
+00000320: 6d20 7363 6970 7920 696d 706f 7274 206c  m scipy import l
+00000330: 696e 616c 670d 0a20 2020 2072 6574 7572  inalg..    retur
+00000340: 6e20 6c69 6e61 6c67 2e69 6e76 286d 6174  n linalg.inv(mat
+00000350: 2c20 6f76 6572 7772 6974 655f 613d 5472  , overwrite_a=Tr
+00000360: 7565 290d 0a20 2020 2023 2072 6574 7572  ue)..    # retur
+00000370: 6e20 6e70 2e6c 696e 616c 672e 696e 7628  n np.linalg.inv(
+00000380: 6d61 7429 0d0a 0d0a 0d0a 636c 6173 7320  mat)......class 
+00000390: 4e6f 7449 6465 6e74 6974 7928 4261 7365  NotIdentity(Base
+000003a0: 4578 6365 7074 696f 6e29 3a0d 0a20 2020  Exception):..   
+000003b0: 2022 2222 4e6f 7420 616e 2049 6465 6e74   """Not an Ident
+000003c0: 6974 7920 4d61 7472 6978 2222 220d 0a0d  ity Matrix"""...
+000003d0: 0a0d 0a64 6566 2063 6c6f 7365 5f69 6465  ...def close_ide
+000003e0: 6e74 6974 795f 6f70 7469 6d69 7a65 6428  ntity_optimized(
+000003f0: 6e2c 2065 7073 2c20 6461 7461 5f73 6f75  n, eps, data_sou
+00000400: 7263 6529 3a0d 0a20 2020 2023 2061 7567  rce):..    # aug
+00000410: 5f6d 6174 7269 7820 3d20 6e70 2e63 6f6c  _matrix = np.col
+00000420: 756d 6e5f 7374 6163 6b28 286d 6174 7269  umn_stack((matri
+00000430: 782c 206e 702e 6964 656e 7469 7479 286e  x, np.identity(n
+00000440: 2929 290d 0a20 2020 2066 6f72 2069 2069  )))..    for i i
+00000450: 6e20 7261 6e67 6528 6e29 3a0d 0a20 2020  n range(n):..   
+00000460: 2020 2020 2070 6976 6f74 203d 2064 6174       pivot = dat
+00000470: 615f 736f 7572 6365 2e67 6574 5f72 6f77  a_source.get_row
+00000480: 2869 295b 695d 0d0a 2020 2020 2020 2020  (i)[i]..        
+00000490: 6966 2063 6c6f 7365 5f65 6e6f 7567 6828  if close_enough(
+000004a0: 7069 766f 742c 2031 2c20 6570 7329 3a0d  pivot, 1, eps):.
+000004b0: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
+000004c0: 7567 5f6d 6174 7269 785b 695d 203d 2061  ug_matrix[i] = a
+000004d0: 7567 5f6d 6174 7269 785b 695d 202f 2070  ug_matrix[i] / p
+000004e0: 6976 6f74 0d0a 2020 2020 2020 2020 2020  ivot..          
+000004f0: 2020 2e2e 2e0d 0a20 2020 2020 2020 2065    .....        e
+00000500: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00000510: 2020 7261 6973 6520 4e6f 7449 6465 6e74    raise NotIdent
+00000520: 6974 790d 0a20 2020 2020 2020 2066 6f72  ity..        for
+00000530: 206a 2069 6e20 7261 6e67 6528 6e29 3a0d   j in range(n):.
+00000540: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000550: 6920 213d 206a 3a0d 0a20 2020 2020 2020  i != j:..       
+00000560: 2020 2020 2020 2020 206e 756d 6265 7220           number 
+00000570: 3d20 6461 7461 5f73 6f75 7263 652e 6765  = data_source.ge
+00000580: 745f 726f 7728 6929 5b6a 5d0d 0a20 2020  t_row(i)[j]..   
+00000590: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000005a0: 636c 6f73 655f 656e 6f75 6768 286e 756d  close_enough(num
+000005b0: 6265 722c 2030 2c20 6570 7329 3a0d 0a20  ber, 0, eps):.. 
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
+000005e0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 2020 2072 6169 7365 204e 6f74 4964 656e     raise NotIden
+00000610: 7469 7479 0d0a 2020 2020 7072 696e 7428  tity..    print(
+00000620: 6d73 675f 636f 7272 6563 746f 290d 0a20  msg_correcto).. 
+00000630: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00000640: 0d0a 0d0a 6465 6620 6e6f 745f 7261 6973  ....def not_rais
+00000650: 6528 646f 6e74 5f72 6169 7365 293a 0d0a  e(dont_raise):..
+00000660: 2020 2020 6966 2064 6f6e 745f 7261 6973      if dont_rais
+00000670: 653a 0d0a 2020 2020 2020 2020 7072 696e  e:..        prin
+00000680: 7428 6d73 675f 6e6f 745f 636f 7272 6563  t(msg_not_correc
+00000690: 746f 290d 0a20 2020 2020 2020 2072 6574  to)..        ret
+000006a0: 7572 6e20 5472 7565 0d0a 2020 2020 656c  urn True..    el
+000006b0: 7365 3a0d 0a20 2020 2020 2020 2072 6169  se:..        rai
+000006c0: 7365 204e 6f74 4964 656e 7469 7479 0d0a  se NotIdentity..
+000006d0: 0d0a 0d0a 6465 6620 636c 6f73 655f 6964  ....def close_id
+000006e0: 656e 7469 7479 286d 6174 7269 782c 2065  entity(matrix, e
+000006f0: 7073 293a 0d0a 2020 2020 6e20 3d20 6c65  ps):..    n = le
+00000700: 6e28 6d61 7472 6978 290d 0a20 2020 2023  n(matrix)..    #
+00000710: 2061 7567 5f6d 6174 7269 7820 3d20 6e70   aug_matrix = np
+00000720: 2e63 6f6c 756d 6e5f 7374 6163 6b28 286d  .column_stack((m
+00000730: 6174 7269 782c 206e 702e 6964 656e 7469  atrix, np.identi
+00000740: 7479 286e 2929 290d 0a20 2020 2066 6f72  ty(n)))..    for
+00000750: 2069 2069 6e20 7261 6e67 6528 6e29 3a0d   i in range(n):.
+00000760: 0a20 2020 2020 2020 2070 6976 6f74 203d  .        pivot =
+00000770: 206d 6174 7269 785b 695d 5b69 5d0d 0a20   matrix[i][i].. 
+00000780: 2020 2020 2020 2069 6620 636c 6f73 655f         if close_
+00000790: 656e 6f75 6768 2870 6976 6f74 2c20 312c  enough(pivot, 1,
+000007a0: 2065 7073 293a 0d0a 2020 2020 2020 2020   eps):..        
+000007b0: 2020 2020 2320 6175 675f 6d61 7472 6978      # aug_matrix
+000007c0: 5b69 5d20 3d20 6175 675f 6d61 7472 6978  [i] = aug_matrix
+000007d0: 5b69 5d20 2f20 7069 766f 740d 0a20 2020  [i] / pivot..   
+000007e0: 2020 2020 2020 2020 202e 2e2e 0d0a 2020           .....  
+000007f0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000800: 2020 2020 2020 2020 206e 6f74 5f72 6169           not_rai
+00000810: 7365 2854 7275 6529 0d0a 2020 2020 2020  se(True)..      
+00000820: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00000830: 7365 0d0a 2020 2020 2020 2020 666f 7220  se..        for 
+00000840: 6a20 696e 2072 616e 6765 286e 293a 0d0a  j in range(n):..
+00000850: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00000860: 2021 3d20 6a3a 0d0a 2020 2020 2020 2020   != j:..        
+00000870: 2020 2020 2020 2020 6e75 6d62 6572 203d          number =
+00000880: 206d 6174 7269 785b 695d 5b6a 5d0d 0a20   matrix[i][j].. 
+00000890: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000008a0: 6620 636c 6f73 655f 656e 6f75 6768 286e  f close_enough(n
+000008b0: 756d 6265 722c 2030 2c20 6570 7329 3a0d  umber, 0, eps):.
+000008c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008d0: 2020 2020 202e 2e2e 0d0a 2020 2020 2020       .....      
+000008e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+000008f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000900: 2020 2020 206e 6f74 5f72 6169 7365 2854       not_raise(T
+00000910: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00000920: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000930: 2046 616c 7365 0d0a 2020 2020 7072 696e   False..    prin
+00000940: 7428 6d73 675f 636f 7272 6563 746f 290d  t(msg_correcto).
+00000950: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
+00000960: 0d0a 0d0a 0d0a 6465 6620 636c 6f73 655f  ......def close_
+00000970: 7477 6f5f 6d61 7472 6963 6573 286d 6174  two_matrices(mat
+00000980: 7269 7831 2c20 6d61 7472 6978 322c 2065  rix1, matrix2, e
+00000990: 7073 3d31 652d 3130 293a 0d0a 2020 2020  ps=1e-10):..    
+000009a0: 6e20 3d20 6c65 6e28 6d61 7472 6978 3129  n = len(matrix1)
+000009b0: 0d0a 2020 2020 666f 7220 6920 696e 2072  ..    for i in r
+000009c0: 616e 6765 286e 293a 0d0a 2020 2020 2020  ange(n):..      
+000009d0: 2020 6966 2063 6c6f 7365 5f65 6e6f 7567    if close_enoug
+000009e0: 6828 6d61 7472 6978 315b 695d 5b69 5d2c  h(matrix1[i][i],
+000009f0: 206d 6174 7269 7832 5b69 5d5b 695d 2c20   matrix2[i][i], 
+00000a00: 6570 7329 3a0d 0a20 2020 2020 2020 2020  eps):..         
+00000a10: 2020 202e 2e2e 0d0a 2020 2020 2020 2020     .....        
+00000a20: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00000a30: 2020 206e 6f74 5f72 6169 7365 2854 7275     not_raise(Tru
+00000a40: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00000a50: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+00000a60: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+00000a70: 616e 6765 286e 293a 0d0a 2020 2020 2020  ange(n):..      
+00000a80: 2020 2020 2020 6966 2063 6c6f 7365 5f65        if close_e
+00000a90: 6e6f 7567 6828 6d61 7472 6978 315b 695d  nough(matrix1[i]
+00000aa0: 5b69 5d2c 206d 6174 7269 7832 5b69 5d5b  [i], matrix2[i][
+00000ab0: 695d 2c20 6570 7329 3a0d 0a20 2020 2020  i], eps):..     
+00000ac0: 2020 2020 2020 2020 2020 202e 2e2e 0d0a             .....
+00000ad0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000af0: 2020 206e 6f74 5f72 6169 7365 2854 7275     not_raise(Tru
+00000b00: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00000b10: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00000b20: 0d0a 2020 2020 7072 696e 7428 6d73 675f  ..    print(msg_
+00000b30: 636f 7272 6563 746f 290d 0a20 2020 2072  correcto)..    r
+00000b40: 6574 7572 6e20 5472 7565 0d0a            eturn True..
```

## inverse/src/sure.py

```diff
@@ -1,16 +1,12 @@
 
-#filename:sure.py
-#folder:
-# To measure timing
-# ' http://stackoverflow.com/questions/5849800/tic-toc-functions-analog-in-python
+
 def tic():
-    # Homemade version of matlab tic and toc functions
     import time
-    global startTime_for_tictoc
-    startTime_for_tictoc = time.time()
+    global start_time_tictoc
+    start_time_tictoc = time.time()
 def toc():
     import time
-    if 'startTime_for_tictoc' in globals():
-        print("Toplam çalışma süresi :" + str(round(time.time() - startTime_for_tictoc)) + " saniye.")
+    if 'start_time_tictoc' in globals():
+        print("Elapsed time :" + str(round(time.time() - start_time_tictoc)) + " seconds.")
     else:
-        print("tic çalıştırılmadı")
+        print("...")
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## inverse/tests/main_test.py

```diff
@@ -1,9 +1,10 @@
 import random
 
+from inverse import inverse_random_matrix
 from inverse.src.abstract_data import id_ekle
 from inverse.src.sp_matrix_ops import save_on_begin, save_pickle
 
 
 def save_on_begin_rand(n):
     for i in range(n):
         numbers = list(random.randint(0, 100) for _ in range(n))
@@ -16,7 +17,13 @@
     # save_on_begin_rand(10)
     print("test")
 
 
 def test_main2():
     # test_siralar()
     ...
+
+
+def test_inverse_random_matrix(capsys):
+    with capsys.disabled():
+        inverse_random_matrix(5, 50)
+        inverse_random_matrix(4, 12)
```

## inverse/tests/tests.py

```diff
@@ -1,12 +1,19 @@
 from inverse.src.tuple_for_buffer import get_tuple_for_buffer
 from inverse import *
 
 
 def test_main():
+    import numpy as np
+    from inverse.src.matrix_converters import BigMatrixConverter
+    from inverse.src.sp_matrix_ops import display_matrix_ozet
+    from inverse.src.sp_utils_inverse import close_identity
+    from inverse.src.sure import tic, toc
+
+    from inverse.src.check_result import inverse_check
     n = 10  # 100 : 16sn ,10:1sn
     threshold = 500
     matrix = get_matrix_for_test(n)
     print(matrix)
     matrix_check = inverse_check(matrix)
     converter = BigMatrixConverter("test")
     big_matrix = converter.convert_small_to_bigmatrix(matrix, threshold=threshold)  # class bigMatrix
```

## Comparing `inverse-0.0.2.dist-info/LICENSE` & `inverse-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

