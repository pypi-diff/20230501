# Comparing `tmp/alacorder-80.0.7.tar.gz` & `tmp/alacorder-80.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.0.7.tar", max compression
+gzip compressed data, was "alacorder-80.0.8.tar", max compression
```

## Comparing `alacorder-80.0.7.tar` & `alacorder-80.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.7/LICENSE
--rw-r--r--   0        0        0     6821 2023-04-29 16:14:55.778453 alacorder-80.0.7/README.md
--rw-r--r--   0        0        0      697 2023-04-30 03:42:35.284273 alacorder-80.0.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-30 15:52:51.221060 alacorder-80.0.7/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.7/src/alacorder/__init__.py
--rw-r--r--   0        0        0   214489 2023-04-30 15:52:18.026304 alacorder-80.0.7/src/alacorder/__main__.py
--rw-r--r--   0        0        0   214489 2023-04-30 15:52:10.300994 alacorder-80.0.7/src/alacorder/alac.py
--rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 alacorder-80.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.8/LICENSE
+-rw-r--r--   0        0        0     6821 2023-04-29 16:14:55.778453 alacorder-80.0.8/README.md
+-rw-r--r--   0        0        0      697 2023-04-30 22:11:45.489044 alacorder-80.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-30 15:52:56.348120 alacorder-80.0.8/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.8/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   214847 2023-04-30 22:11:19.081069 alacorder-80.0.8/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   214847 2023-04-30 22:10:51.515736 alacorder-80.0.8/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 alacorder-80.0.8/PKG-INFO
```

### Comparing `alacorder-80.0.7/LICENSE` & `alacorder-80.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.7/README.md` & `alacorder-80.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.7/pyproject.toml` & `alacorder-80.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.0.7"
+version = "80.0.8"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.0.7/src/alacorder/.DS_Store` & `alacorder-80.0.8/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.7/src/alacorder/__init__.py` & `alacorder-80.0.8/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.7/src/alacorder/__main__.py` & `alacorder-80.0.8/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.7"
+version = "80.0.8"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3195,14 +3195,15 @@
         )
         return None
 
 
 def fetch(
     querypath="",
     dirpath="",
+    criminal=False,
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
     cf=None,
     no_update=False,
@@ -3211,14 +3212,15 @@
 ):
     """
     Fetch case PDFs from Alacourt.com.
     Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
     Args:
        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
        dirpath (str): Path to PDF output directory
+       criminal (bool): Only search criminal cases
        cID (str): Customer ID on Alacourt.com
        uID (str): User ID on Alacourt.com
        pwd (str): Password on Alacourt.com
        qmax (int): Maximum queries to conduct on Alacourt.com
        qskip (int): Skip entries at top of query file
        no_update (bool): Do not update query template after completion
        debug (bool): Print detailed runtime information to console
@@ -3255,14 +3257,17 @@
             "plugins.always_open_pdf_externally": True,  # It will not display PDF directly in chrome
         },
     )
     print("Starting browser... Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
+    if criminal:
+        query["TEMP_DIVISION"] == "Criminal Only"
+
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
             login(driver, cID, uID, pwd, window=window)
         driver.implicitly_wait(1)
         results = party_search(
@@ -4353,15 +4358,15 @@
     return append_archive(in_path, out_path)
 
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
 @click.option(
     "--input-path",
     "-in",
-    "listpath",
+    "querypath",
     required=True,
     prompt="Path to query table",
     help="Path to query table/spreadsheet (.xls, .xlsx)",
     type=click.Path(),
 )
 @click.option(
     "--output-path",
@@ -4369,14 +4374,20 @@
     "path",
     required=True,
     prompt="PDF download path",
     type=click.Path(),
     help="Desired PDF output directory",
 )
 @click.option(
+    "--criminal-only",
+    "-criminal",
+    is_flag=True,
+    help="Only search criminal cases"
+    )
+@click.option(
     "--customer-id",
     "-c",
     "cID",
     required=True,
     prompt="Alacourt Customer ID",
     help="Customer ID on Alacourt.com",
 )
@@ -4425,31 +4436,33 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def cli_fetch(listpath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
+def cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
-        listpath (str): Path to query table/spreadsheet (.xls, .xlsx)
+        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
+        criminal (bool, optional): only search criminal cases
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
         qmax (int): Maximum queries to conduct on Alacourt.com
         qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
         debug (bool): Print detailed runtime information to console
     """
     fetch(
         querypath=listpath,
         dirpath=path,
+        criminal=criminal,
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
         debug=debug,
```

### Comparing `alacorder-80.0.7/src/alacorder/alac.py` & `alacorder-80.0.8/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.7"
+version = "80.0.8"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3195,14 +3195,15 @@
         )
         return None
 
 
 def fetch(
     querypath="",
     dirpath="",
+    criminal=False,
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
     cf=None,
     no_update=False,
@@ -3211,14 +3212,15 @@
 ):
     """
     Fetch case PDFs from Alacourt.com.
     Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
     Args:
        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
        dirpath (str): Path to PDF output directory
+       criminal (bool): Only search criminal cases
        cID (str): Customer ID on Alacourt.com
        uID (str): User ID on Alacourt.com
        pwd (str): Password on Alacourt.com
        qmax (int): Maximum queries to conduct on Alacourt.com
        qskip (int): Skip entries at top of query file
        no_update (bool): Do not update query template after completion
        debug (bool): Print detailed runtime information to console
@@ -3255,14 +3257,17 @@
             "plugins.always_open_pdf_externally": True,  # It will not display PDF directly in chrome
         },
     )
     print("Starting browser... Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
+    if criminal:
+        query["TEMP_DIVISION"] == "Criminal Only"
+
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
             login(driver, cID, uID, pwd, window=window)
         driver.implicitly_wait(1)
         results = party_search(
@@ -4353,15 +4358,15 @@
     return append_archive(in_path, out_path)
 
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
 @click.option(
     "--input-path",
     "-in",
-    "listpath",
+    "querypath",
     required=True,
     prompt="Path to query table",
     help="Path to query table/spreadsheet (.xls, .xlsx)",
     type=click.Path(),
 )
 @click.option(
     "--output-path",
@@ -4369,14 +4374,20 @@
     "path",
     required=True,
     prompt="PDF download path",
     type=click.Path(),
     help="Desired PDF output directory",
 )
 @click.option(
+    "--criminal-only",
+    "-criminal",
+    is_flag=True,
+    help="Only search criminal cases"
+    )
+@click.option(
     "--customer-id",
     "-c",
     "cID",
     required=True,
     prompt="Alacourt Customer ID",
     help="Customer ID on Alacourt.com",
 )
@@ -4425,31 +4436,33 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def cli_fetch(listpath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
+def cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
-        listpath (str): Path to query table/spreadsheet (.xls, .xlsx)
+        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
+        criminal (bool, optional): only search criminal cases
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
         qmax (int): Maximum queries to conduct on Alacourt.com
         qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
         debug (bool): Print detailed runtime information to console
     """
     fetch(
         querypath=listpath,
         dirpath=path,
+        criminal=criminal,
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
         debug=debug,
```

### Comparing `alacorder-80.0.7/PKG-INFO` & `alacorder-80.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.0.7
+Version: 80.0.8
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

