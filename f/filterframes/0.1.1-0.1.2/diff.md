# Comparing `tmp/filterframes-0.1.1.tar.gz` & `tmp/filterframes-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filterframes-0.1.1.tar", last modified: Tue Apr 25 00:38:59 2023, max compression
+gzip compressed data, was "filterframes-0.1.2.tar", last modified: Mon May  1 06:46:16 2023, max compression
```

## Comparing `filterframes-0.1.1.tar` & `filterframes-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.837158 filterframes-0.1.1/
--rw-rw-rw-   0        0        0     2437 2023-04-25 00:38:59.836062 filterframes-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-04-24 23:05:38.000000 filterframes-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.815257 filterframes-0.1.1/filterframes/
--rw-rw-rw-   0        0        0       70 2023-04-25 00:22:58.000000 filterframes-0.1.1/filterframes/__init__.py
--rw-rw-rw-   0        0        0    10483 2023-04-25 00:04:18.000000 filterframes-0.1.1/filterframes/filterframes.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.834059 filterframes-0.1.1/filterframes.egg-info/
--rw-rw-rw-   0        0        0     2437 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 00:38:59.837158 filterframes-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-04-25 00:38:00.000000 filterframes-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.835061 filterframes-0.1.1/test/
--rw-rw-rw-   0        0        0     2174 2023-04-25 00:05:20.000000 filterframes-0.1.1/test/test_filterframes.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.899396 filterframes-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-01 06:00:47.000000 filterframes-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5832 2023-05-01 06:46:16.891358 filterframes-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3950 2023-05-01 06:23:52.000000 filterframes-0.1.2/README.md
+-rw-rw-rw-   0        0        0      929 2023-05-01 06:19:29.000000 filterframes-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 06:46:16.899396 filterframes-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-05-01 03:56:38.000000 filterframes-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.874764 filterframes-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.882762 filterframes-0.1.2/src/filterframes/
+-rw-rw-rw-   0        0        0      249 2023-05-01 04:47:21.000000 filterframes-0.1.2/src/filterframes/__init__.py
+-rw-rw-rw-   0        0        0    10679 2023-05-01 06:00:47.000000 filterframes-0.1.2/src/filterframes/filterframes.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.891358 filterframes-0.1.2/src/filterframes.egg-info/
+-rw-rw-rw-   0        0        0     5832 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.891358 filterframes-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1907 2023-05-01 04:56:24.000000 filterframes-0.1.2/tests/test_filterframes.py
```

### Comparing `filterframes-0.1.1/filterframes/filterframes.py` & `filterframes-0.1.2/src/filterframes/filterframes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module providing function for converting between DTASelectFilter.tx files and pandas DataFrame objects"""
 import os
 from enum import Enum
 from io import TextIOWrapper, StringIO
 from typing import List, Union, Any, TextIO
 
 import pandas as pd
 
@@ -18,24 +19,24 @@
 
     Returns:
         list: A list of lines from the input source.
 
     Raises:
         ValueError: If the input type is not supported.
     """
-    if type(file_input) is str:
+    if isinstance(file_input, str):
         if os.path.exists(file_input):
-            with open(file_input) as f:
-                lines = f.read().split('\n')
+            with open(file=file_input, mode='r', encoding='UTF-8') as file:
+                lines = file.read().split('\n')
         else:
             lines = file_input.split('\n')
-    elif type(file_input) is TextIOWrapper or type(file_input) is TextIO:
+    elif isinstance(file_input, (TextIOWrapper, TextIO)):
         lines = file_input.read().split('\n')
 
-    elif type(file_input) is StringIO:
+    elif isinstance(file_input, StringIO):
         lines = file_input.getvalue().split('\n')
     else:
         raise ValueError(f'Unsupported input type: {type(file_input)}!')
 
     return lines[:-1]
 
 
@@ -77,41 +78,39 @@
     Returns:
         str: The constructed file name string.
     """
 
     return f"{peptide_row['FileName']}.{peptide_row['LowScan']}.{peptide_row['HighScan']}.{peptide_row['Charge']}"
 
 
-def _reorder_columns(df: pd.DataFrame, column: str, new_position: int) -> pd.DataFrame:
+def _reorder_columns(dataframe: pd.DataFrame, column: str, new_position: int) -> pd.DataFrame:
     """
     Reorder columns in a dataframe by moving a specified column to a new position.
 
     Args:
         df (pd.DataFrame): The input dataframe.
         column (str): The column to be moved.
         new_position (int): The new position for the specified column.
 
     Returns:
         pd.DataFrame: A dataframe with reordered columns.
     """
 
-    columns = df.columns.tolist()
+    columns = dataframe.columns.tolist()
     columns.insert(new_position, columns.pop(columns.index(column)))
-    return df[columns]
+    return dataframe[columns]
 
 
 def _write_lines(file_output, lines):
     """
     Write a list of lines to a given file output.
 
-
     Args:
         file_output (TextIOWrapper or StringIO): The output file object.
         lines (list): A list of lines to be written.
-        newline (bool, optional): If True, a newline is added at the end of each line. Default is False.
     """
 
     for line in lines:
         file_output.write(line + '\n')
 
 
 def from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO, TextIO]) -> (
@@ -132,39 +131,39 @@
             - protein_df (pd.DataFrame): A dataframe containing protein data.
             - end_lines (List[str]): A list of end lines (information lines).
     """
 
     lines = _get_lines(file_input)
 
     class FileState(Enum):
+        """
+        Enum for specifying the different parts of the DTASelect-filter.txt file
+        """
         HEADER = 1
         DATA = 2
         INFO = 3
 
     file_state = FileState.HEADER
 
     header_lines, end_lines = [], []
-
-    peptide_data = None
-    protein_data = None
-
-    current_protein_grp = 0
-    peptide_line_cnt = 0
+    peptide_data, protein_data = None, None
+    current_protein_grp, peptide_line_cnt = 0, 0
 
     for line in lines:
         line_elements = line.rstrip().split("\t")
 
-        if line.startswith('Locus'):
+        if line.startswith('Locus'):  # Protein Line Header
             protein_data = {key: [] for key in line_elements}
             protein_data['ProteinGroup'] = []
-        if line.startswith('Unique'):
+
+        if line.startswith('Unique'):  # Peptide Line Header
             peptide_data = {key: [] for key in line_elements}
             peptide_data['ProteinGroup'] = []
 
-        # update file state
+        # Update file state
         if len(line_elements) > 0 and line_elements[0] == 'Unique':
             header_lines.append(line)
             file_state = FileState.DATA
             continue
 
         if len(line_elements) > 1 and line_elements[1] == "Proteins":
             file_state = FileState.INFO
```

