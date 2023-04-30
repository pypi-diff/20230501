# Comparing `tmp/report_manager-0.7.0-py2.py3-none-any.whl.zip` & `tmp/report_manager-0.8.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10806 bytes, number of entries: 9
--rw-r--r--  2.0 unx      317 b- defN 22-Dec-23 07:05 report_manager/__init__.py
--rw-r--r--  2.0 unx    30241 b- defN 22-Dec-23 07:05 report_manager/report_manager.py
--rw-r--r--  2.0 unx      116 b- defN 22-Dec-23 19:03 report_manager/version.py
--rw-r--r--  2.0 unx     1210 b- defN 22-Dec-23 19:03 report_manager-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2988 b- defN 22-Dec-23 19:03 report_manager-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-23 19:03 report_manager-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 22-Dec-23 19:03 report_manager-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 22-Dec-23 19:03 report_manager-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      777 b- defN 22-Dec-23 19:03 report_manager-0.7.0.dist-info/RECORD
-9 files, 35845 bytes uncompressed, 9452 bytes compressed:  73.6%
+Zip file size: 10816 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      317 b- defN 23-Apr-30 23:11 report_manager/__init__.py
+-rw-r--r--  2.0 unx    30240 b- defN 23-Apr-30 23:11 report_manager/report_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-30 23:11 report_manager/version.py
+-rw-r--r--  2.0 unx     1210 b- defN 23-Apr-30 23:11 report_manager-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2987 b- defN 23-Apr-30 23:11 report_manager-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-30 23:11 report_manager-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-30 23:11 report_manager-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-30 23:11 report_manager-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      777 b- defN 23-Apr-30 23:11 report_manager-0.8.0.dist-info/RECORD
+9 files, 35843 bytes uncompressed, 9462 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: report_manager/report_manager.py
 Comment: 
 
 Filename: report_manager/version.py
 Comment: 
 
-Filename: report_manager-0.7.0.dist-info/LICENSE
+Filename: report_manager-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: report_manager-0.7.0.dist-info/METADATA
+Filename: report_manager-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: report_manager-0.7.0.dist-info/WHEEL
+Filename: report_manager-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: report_manager-0.7.0.dist-info/entry_points.txt
+Filename: report_manager-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: report_manager-0.7.0.dist-info/top_level.txt
+Filename: report_manager-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: report_manager-0.7.0.dist-info/RECORD
+Filename: report_manager-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## report_manager/report_manager.py

```diff
@@ -13,15 +13,15 @@
 import numpy as np
 from scipy import stats
 from scipy.stats import linregress
 from scipy.stats import chi2_contingency
 import statsmodels.api as sm
 from statsmodels.formula.api import ols
 import pandas as pd
-import pandas_profiling as pp
+import ydata_profiling as pp
 import seaborn as sns
 import itertools
 from sklearn.preprocessing import LabelEncoder
 import matplotlib.pyplot as plt
 sns.set(font_scale=.3)
 plt.xticks(rotation=45)
```

## report_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `report_manager-0.7.0.dist-info/LICENSE` & `report_manager-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `report_manager-0.7.0.dist-info/METADATA` & `report_manager-0.8.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-manager
-Version: 0.7.0
+Version: 0.8.0
 Summary: Manage your reports
 Home-page: https://github.com/Knuckles-Team/report-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipywidgets (>=8.0.4)
 Requires-Dist: matplotlib (>=3.6.2)
 Requires-Dist: numpy (>=1.23.5)
 Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: pandas-profiling (>=3.6.0)
 Requires-Dist: scikit-learn (>=1.2.0)
 Requires-Dist: scipy (>=1.9.3)
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: xlsxwriter (>=3.0.3)
+Requires-Dist: ydata-profiling (>=4.1.2)
 
 # Report Manager
-*Version: 0.7.0*
+*Version: 0.8.0*
 
 Manage your reports
 - Merge reports based off specified columns
 - Generate analysis on data set
 - Pandas profiling
 
 ### Usage:
```

