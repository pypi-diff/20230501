# Comparing `tmp/alacorder-80.1.0.tar.gz` & `tmp/alacorder-80.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.0.tar", max compression
+gzip compressed data, was "alacorder-80.1.1.tar", max compression
```

## Comparing `alacorder-80.1.0.tar` & `alacorder-80.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.0/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.0/README.md
--rw-r--r--   0        0        0      697 2023-05-01 17:51:49.328132 alacorder-80.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-30 22:12:00.468048 alacorder-80.1.0/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.1.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   215308 2023-05-01 17:50:16.582308 alacorder-80.1.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   215308 2023-05-01 17:50:11.453247 alacorder-80.1.0/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.1/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.1/README.md
+-rw-r--r--   0        0        0      697 2023-05-01 17:53:02.479122 alacorder-80.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-01 17:53:03.320152 alacorder-80.1.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.1.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   212262 2023-05-01 17:52:48.932648 alacorder-80.1.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   212262 2023-05-01 17:52:43.729760 alacorder-80.1.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.1/PKG-INFO
```

### Comparing `alacorder-80.1.0/LICENSE` & `alacorder-80.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.0/README.md` & `alacorder-80.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.0/pyproject.toml` & `alacorder-80.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.0"
+version = "80.1.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.0/src/alacorder/.DS_Store` & `alacorder-80.1.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.0/src/alacorder/__init__.py` & `alacorder-80.1.1/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.0/src/alacorder/__main__.py` & `alacorder-80.1.1/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.0"
+version = "80.1.1"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2185,53 +2185,14 @@
         'WarrantMailerDate',
         'EnforcementLastUpdate',
         'EnforcementUpdatedBy'
     )
     return cases, all_charges, all_fees
 
 
-def split_enforcement(df, debug=False):
-    en = df.select(
-        [
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Date\: (\d\d/\d\d/\d\d\d\d)').alias("TurnOverDate"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("TurnOverAmt"),
-            pl.col("AllPagesText").str.extract(r'Frequency Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("FrequencyAmt"),
-            pl.col("AllPagesText").str.extract(r'Due Date\: (\d\d/\d\d/\d\d\d\d)').alias("DueDate"),
-            pl.col("AllPagesText").str.extract(r'Last Paid Date\: (\d\d/\d\d/\d\d\d\d)').alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r'Payor\: ([A-Z0-9]{4})').alias("Payor"),
-            pl.col("AllPagesText").str.extract(r'Enforcement Status\: ([A-Z\:,\s]+)').str.replace_all(r'\s+',' ').str.replace(r' F$','').str.strip().alias("EnforcementStatus"),
-            pl.col("AllPagesText").str.extract(r'Frequency\: (.+)').str.replace(r'Cost Paid By\:','').str.strip().alias("Frequency"),
-            pl.col("AllPagesText").str.extract(r'Placement Status\: (.+)').str.strip().alias("PlacementStatus"),
-            pl.col("AllPagesText").str.extract(r'Comments\: (.+)').str.strip().alias("Comments"),
-            pl.col("AllPagesText").str.extract(r'Over/Under Paid\: \$(\d+\.\d\d)').alias("OverUnderPaid"),
-            pl.col("AllPagesText").str.extract(r'PreTrial\: (YES|NO)').alias("PreTrial"),
-            pl.col("AllPagesText").str.extract(r'PreTrail Date\: (.+)PreTrial').str.strip().alias("PreTrialDate"),
-            pl.col("AllPagesText").str.extract(r'PreTrial Terms\: (YES|NO)').alias("PreTrialTerms"),
-            pl.col("AllPagesText").str.extract(r'Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)').alias("PreTermsDate"),
-            pl.col("AllPagesText").str.extract(r'Delinquent\: (YES|NO)').alias("Delinquent"),
-            pl.col("AllPagesText").str.extract(r'Delinquent Date\: (\d\d/\d\d/\d\d\d\d)').alias("DelinquentDate"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer\: (YES|NO)').alias("DAMailer"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("DAMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer\: (YES|NO)').alias("WarrantMailer"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("WarrantMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Last Update\: (\d\d/\d\d/\d\d\d\d)').alias("EnforcementLastUpdate"),
-            pl.col("AllPagesText").str.extract(r'Updated By\: ([A-Z]{3})').alias("EnforcementUpdatedBy")
-        ]
-    )
-    return en
-
 def explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
```

### Comparing `alacorder-80.1.0/src/alacorder/alac.py` & `alacorder-80.1.1/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.0"
+version = "80.1.1"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2185,53 +2185,14 @@
         'WarrantMailerDate',
         'EnforcementLastUpdate',
         'EnforcementUpdatedBy'
     )
     return cases, all_charges, all_fees
 
 
-def split_enforcement(df, debug=False):
-    en = df.select(
-        [
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Date\: (\d\d/\d\d/\d\d\d\d)').alias("TurnOverDate"),
-            pl.col("AllPagesText").str.extract(r'TurnOver Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("TurnOverAmt"),
-            pl.col("AllPagesText").str.extract(r'Frequency Amt\: \$(\d+\.\d\d)').cast(pl.Float64, strict=False).alias("FrequencyAmt"),
-            pl.col("AllPagesText").str.extract(r'Due Date\: (\d\d/\d\d/\d\d\d\d)').alias("DueDate"),
-            pl.col("AllPagesText").str.extract(r'Last Paid Date\: (\d\d/\d\d/\d\d\d\d)').alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r'Payor\: ([A-Z0-9]{4})').alias("Payor"),
-            pl.col("AllPagesText").str.extract(r'Enforcement Status\: ([A-Z\:,\s]+)').str.replace_all(r'\s+',' ').str.replace(r' F$','').str.strip().alias("EnforcementStatus"),
-            pl.col("AllPagesText").str.extract(r'Frequency\: (.+)').str.replace(r'Cost Paid By\:','').str.strip().alias("Frequency"),
-            pl.col("AllPagesText").str.extract(r'Placement Status\: (.+)').str.strip().alias("PlacementStatus"),
-            pl.col("AllPagesText").str.extract(r'Comments\: (.+)').str.strip().alias("Comments"),
-            pl.col("AllPagesText").str.extract(r'Over/Under Paid\: \$(\d+\.\d\d)').alias("OverUnderPaid"),
-            pl.col("AllPagesText").str.extract(r'PreTrial\: (YES|NO)').alias("PreTrial"),
-            pl.col("AllPagesText").str.extract(r'PreTrail Date\: (.+)PreTrial').str.strip().alias("PreTrialDate"),
-            pl.col("AllPagesText").str.extract(r'PreTrial Terms\: (YES|NO)').alias("PreTrialTerms"),
-            pl.col("AllPagesText").str.extract(r'Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)').alias("PreTermsDate"),
-            pl.col("AllPagesText").str.extract(r'Delinquent\: (YES|NO)').alias("Delinquent"),
-            pl.col("AllPagesText").str.extract(r'Delinquent Date\: (\d\d/\d\d/\d\d\d\d)').alias("DelinquentDate"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer\: (YES|NO)').alias("DAMailer"),
-            pl.col("AllPagesText").str.extract(r'DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("DAMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer\: (YES|NO)').alias("WarrantMailer"),
-            pl.col("AllPagesText").str.extract(r'Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)').alias("WarrantMailerDate"),
-            pl.col("AllPagesText").str.extract(r'Last Update\: (\d\d/\d\d/\d\d\d\d)').alias("EnforcementLastUpdate"),
-            pl.col("AllPagesText").str.extract(r'Updated By\: ([A-Z]{3})').alias("EnforcementUpdatedBy")
-        ]
-    )
-    return en
-
 def explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
```

### Comparing `alacorder-80.1.0/PKG-INFO` & `alacorder-80.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.0
+Version: 80.1.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

