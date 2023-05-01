# Comparing `tmp/umbitlib-0.0.38.tar.gz` & `tmp/umbitlib-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umbitlib-0.0.38.tar", last modified: Wed Nov  2 16:57:32 2022, max compression
+gzip compressed data, was "umbitlib-0.0.39.tar", last modified: Mon May  1 21:39:50 2023, max compression
```

## Comparing `umbitlib-0.0.38.tar` & `umbitlib-0.0.39.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 16:57:32.791440 umbitlib-0.0.38/
--rw-rw-rw-   0        0        0     1091 2022-06-30 16:23:16.000000 umbitlib-0.0.38/LICENSE
--rw-rw-rw-   0        0        0     1370 2022-11-02 16:57:32.791440 umbitlib-0.0.38/PKG-INFO
--rw-rw-rw-   0        0        0      776 2022-06-30 16:23:16.000000 umbitlib-0.0.38/README.md
--rw-rw-rw-   0        0        0       86 2022-06-30 16:23:16.000000 umbitlib-0.0.38/pyproject.toml
--rw-rw-rw-   0        0        0      733 2022-11-02 16:57:32.793440 umbitlib-0.0.38/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-02 16:57:32.750442 umbitlib-0.0.38/src/
-drwxrwxrwx   0        0        0        0 2022-11-02 16:57:32.772443 umbitlib-0.0.38/src/umbitlib/
--rw-rw-rw-   0        0        0        0 2022-06-30 16:23:16.000000 umbitlib-0.0.38/src/umbitlib/__init__.py
--rw-rw-rw-   0        0        0     1371 2022-10-18 15:53:16.000000 umbitlib-0.0.38/src/umbitlib/constants.py
--rw-rw-rw-   0        0        0     3262 2022-06-30 16:23:16.000000 umbitlib-0.0.38/src/umbitlib/dates.py
--rw-rw-rw-   0        0        0        0 2022-06-30 16:23:16.000000 umbitlib-0.0.38/src/umbitlib/graphs.py
--rw-rw-rw-   0        0        0    17982 2022-11-02 16:55:52.000000 umbitlib-0.0.38/src/umbitlib/helpers.py
--rw-rw-rw-   0        0        0    20399 2022-11-02 16:55:59.000000 umbitlib-0.0.38/src/umbitlib/queries.py
--rw-rw-rw-   0        0        0     6542 2022-06-30 16:23:16.000000 umbitlib-0.0.38/src/umbitlib/science.py
-drwxrwxrwx   0        0        0        0 2022-11-02 16:57:32.789441 umbitlib-0.0.38/src/umbitlib.egg-info/
--rw-rw-rw-   0        0        0     1370 2022-11-02 16:57:32.000000 umbitlib-0.0.38/src/umbitlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2022-11-02 16:57:32.000000 umbitlib-0.0.38/src/umbitlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-02 16:57:32.000000 umbitlib-0.0.38/src/umbitlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-11-02 16:57:32.000000 umbitlib-0.0.38/src/umbitlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 21:39:50.079709 umbitlib-0.0.39/
+-rw-rw-rw-   0        0        0     1091 2022-06-30 16:23:16.000000 umbitlib-0.0.39/LICENSE
+-rw-rw-rw-   0        0        0     1370 2023-05-01 21:39:50.079709 umbitlib-0.0.39/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2022-06-30 16:23:16.000000 umbitlib-0.0.39/README.md
+-rw-rw-rw-   0        0        0       86 2022-06-30 16:23:16.000000 umbitlib-0.0.39/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2023-05-01 21:39:50.083699 umbitlib-0.0.39/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 21:39:49.996037 umbitlib-0.0.39/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 21:39:50.047700 umbitlib-0.0.39/src/umbitlib/
+-rw-rw-rw-   0        0        0        0 2022-06-30 16:23:16.000000 umbitlib-0.0.39/src/umbitlib/__init__.py
+-rw-rw-rw-   0        0        0     4116 2023-05-01 20:33:15.000000 umbitlib-0.0.39/src/umbitlib/constants.py
+-rw-rw-rw-   0        0        0     3262 2022-06-30 16:23:16.000000 umbitlib-0.0.39/src/umbitlib/dates.py
+-rw-rw-rw-   0        0        0        0 2022-06-30 16:23:16.000000 umbitlib-0.0.39/src/umbitlib/graphs.py
+-rw-rw-rw-   0        0        0    17982 2022-11-02 16:55:52.000000 umbitlib-0.0.39/src/umbitlib/helpers.py
+-rw-rw-rw-   0        0        0    20357 2023-05-01 21:29:10.000000 umbitlib-0.0.39/src/umbitlib/queries.py
+-rw-rw-rw-   0        0        0     7159 2023-03-31 16:34:51.000000 umbitlib-0.0.39/src/umbitlib/science.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:39:50.067742 umbitlib-0.0.39/src/umbitlib.egg-info/
+-rw-rw-rw-   0        0        0     1370 2023-05-01 21:39:49.000000 umbitlib-0.0.39/src/umbitlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-05-01 21:39:49.000000 umbitlib-0.0.39/src/umbitlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 21:39:49.000000 umbitlib-0.0.39/src/umbitlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 21:39:49.000000 umbitlib-0.0.39/src/umbitlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 21:39:50.077715 umbitlib-0.0.39/tests/
+-rw-rw-rw-   0        0        0        0 2022-06-30 16:23:16.000000 umbitlib-0.0.39/tests/test_dates.py
+-rw-rw-rw-   0        0        0        0 2022-06-30 16:23:16.000000 umbitlib-0.0.39/tests/test_graphs.py
+-rw-rw-rw-   0        0        0    18902 2023-05-01 19:05:28.000000 umbitlib-0.0.39/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     2092 2022-10-18 15:31:08.000000 umbitlib-0.0.39/tests/test_queries.py
+-rw-rw-rw-   0        0        0     2537 2022-06-30 16:23:16.000000 umbitlib-0.0.39/tests/test_science.py
```

### Comparing `umbitlib-0.0.38/LICENSE` & `umbitlib-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `umbitlib-0.0.38/PKG-INFO` & `umbitlib-0.0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbitlib
-Version: 0.0.38
+Version: 0.0.39
 Summary: A library containing functions and constants commonly used so they can be centrally hosted sourced and managed
 Home-page: https://gitlab.com/umbbiteam/umbitlib
 Author: Martin Smith
 Author-email: martin.smith@hsc.utah.edu
 Project-URL: Bug Tracker, https://gitlab.com/umbbiteam/umbitlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `umbitlib-0.0.38/README.md` & `umbitlib-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `umbitlib-0.0.38/setup.cfg` & `umbitlib-0.0.39/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6d62 6974 6c69 620d 0a76 6572   = umbitlib..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e33 380d 0a61  sion = 0.0.38..a
+00000020: 7369 6f6e 203d 2030 2e30 2e33 390d 0a61  sion = 0.0.39..a
 00000030: 7574 686f 7220 3d20 4d61 7274 696e 2053  uthor = Martin S
 00000040: 6d69 7468 0d0a 6175 7468 6f72 5f65 6d61  mith..author_ema
 00000050: 696c 203d 206d 6172 7469 6e2e 736d 6974  il = martin.smit
 00000060: 6840 6873 632e 7574 6168 2e65 6475 0d0a  h@hsc.utah.edu..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 6c69 6272 6172 7920 636f 6e74 6169 6e69  library containi
 00000090: 6e67 2066 756e 6374 696f 6e73 2061 6e64  ng functions and
```

### Comparing `umbitlib-0.0.38/src/umbitlib/dates.py` & `umbitlib-0.0.39/src/umbitlib/dates.py`

 * *Files identical despite different names*

### Comparing `umbitlib-0.0.38/src/umbitlib/helpers.py` & `umbitlib-0.0.39/src/umbitlib/helpers.py`

 * *Files identical despite different names*

### Comparing `umbitlib-0.0.38/src/umbitlib/queries.py` & `umbitlib-0.0.39/src/umbitlib/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import psycopg2
 import pandas as pd
 import time
 import cx_Oracle
 import os
 import os.path
-from umbitlib.constants import *  # !!! Change this to 'import src.umbitlib.constants' for testing and back to 'import umbitlib.constants' for production upload
-from umbitlib.dates import TRGTMON_YYYYMMDD  # !!! Change this to 'import src.umbitlib.dates' for testing and back to 'import umbitlib.dates' for production upload
+from umbitlib.constants import * # !!! Change this to 'import src.umbitlib.constants' for testing and back to 'from umbitlib.constants import *' for production upload
+from umbitlib.dates import TRGTMON_YYYYMMDD # !!! Change this to 'import src.umbitlib.dates' for testing and back to 'from umbitlib.dates import TRGTMON_YYYYMMDD' for production upload
 import warnings
 
 
 ####################################################################################
 ## ORACLE CONNECTION FUNCTIONS
 ####################################################################################
 
@@ -21,16 +21,15 @@
     Returns:
         username and password from Excel doc in tuple.
 
     Example:        
         username, password = excel_credentials()
     """    
     try:  
-        data_source_file_oracle = "\\\\hsc-evs03.ad.utah.edu\\users\\" + \
-            os.getlogin() + "\\Data Sources\\UIDPWD.xlsx"
+        data_source_file_oracle = r"G:\Data Sources\UIDPWD.xlsx"
         wb_credentials_oracle = load_workbook(data_source_file_oracle)
         sheet_oracle = wb_credentials_oracle['Sheet1']
         username = sheet_oracle['A2'].value
         password = sheet_oracle['B2'].value
         return username, password
     except:
         raise TypeError('Excel workbook with credentials not found.')
```

### Comparing `umbitlib-0.0.38/src/umbitlib/science.py` & `umbitlib-0.0.39/src/umbitlib/science.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,30 @@
         pvalue (float, optional): the p-value or level of significance to test against. Defaults to .05.
         zscore (float, optional): the z-score or test statistic to test against. Defaults to 1.96.
         
     Returns:
         multiple strings and graphs with test results
     """
 
+    # Code to remove nan values
+    intNanCount = len([x for x in series if str(x) == 'nan'])
+    if intNanCount > 0:
+        print(f'Removed {intNanCount} nan values')
+    series = [x for x in series if str(x) != 'nan']
+
+    # Code to remove +/- infinity values
+    infCount = len([x for x in series if x == np.inf])
+    negInfCount = len([x for x in series if x == -np.inf])
+    intInfCount = infCount + negInfCount
+    if intInfCount > 0:
+        print(f'Removed { intInfCount } infinity values')  
+    series = [x for x in series if x != -np.inf]
+    series = [x for x in series if x != np.inf]
+
+
     # Skewness check
     skewness_result = stats.skewtest(series)
     print(f"{p_pass_fail(skewness_result.pvalue, pvalue)}Skewness p-value: {skewness_result.pvalue:.3f} (Should be > {pvalue} to pass)")
     print(f"{z_pass_fail(skewness_result.statistic, zscore)}Skewness Z-Score: {skewness_result.statistic:.3f} (Should be between +/- {zscore} to pass)\n")
 
 
     # Kurtosis check
```

### Comparing `umbitlib-0.0.38/src/umbitlib.egg-info/PKG-INFO` & `umbitlib-0.0.39/src/umbitlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbitlib
-Version: 0.0.38
+Version: 0.0.39
 Summary: A library containing functions and constants commonly used so they can be centrally hosted sourced and managed
 Home-page: https://gitlab.com/umbbiteam/umbitlib
 Author: Martin Smith
 Author-email: martin.smith@hsc.utah.edu
 Project-URL: Bug Tracker, https://gitlab.com/umbbiteam/umbitlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

