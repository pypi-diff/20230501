# Comparing `tmp/edgar-analyzer-0.0.1rc2.tar.gz` & `tmp/edgar-analyzer-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgar-analyzer-0.0.1rc2.tar", last modified: Sat Apr  1 23:32:19 2023, max compression
+gzip compressed data, was "edgar-analyzer-0.0.1rc3.tar", last modified: Mon May  1 04:39:45 2023, max compression
```

## Comparing `edgar-analyzer-0.0.1rc2.tar` & `edgar-analyzer-0.0.1rc3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 23:32:19.308489 edgar-analyzer-0.0.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-01 23:32:19.304489 edgar-analyzer-0.0.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 23:32:19.304489 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-01 23:32:19.000000 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-01 23:32:19.000000 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 23:32:19.000000 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-01 23:32:19.000000 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-01 23:32:19.000000 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-01 23:32:19.000000 edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 23:32:19.304489 edgar-analyzer-0.0.1rc2/edgaranalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_build_database.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_download_filings.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_download_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_event_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_loans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_zipcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_sample_loans.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/edgaranalyzer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 23:32:19.308489 edgar-analyzer-0.0.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-01 23:32:16.000000 edgar-analyzer-0.0.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 04:39:45.735757 edgar-analyzer-0.0.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-01 04:39:45.735757 edgar-analyzer-0.0.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 04:39:45.735757 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-01 04:39:45.000000 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-01 04:39:45.000000 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 04:39:45.000000 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 04:39:45.000000 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 04:39:45.000000 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 04:39:45.000000 edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 04:39:45.735757 edgar-analyzer-0.0.1rc3/edgaranalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_build_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_download_filings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_download_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_event_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_loans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_zipcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_sample_loans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/edgaranalyzer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 04:39:45.735757 edgar-analyzer-0.0.1rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-01 04:39:38.000000 edgar-analyzer-0.0.1rc3/setup.py
```

### Comparing `edgar-analyzer-0.0.1rc2/LICENSE` & `edgar-analyzer-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/PKG-INFO` & `edgar-analyzer-0.0.1rc3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-analyzer
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Textual analysis on SEC filings from EDGAR
 Home-page: https://github.com/mgao6767/edgar-analyzer
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,30 +27,30 @@
 pip install edgar-analyzer
 ```
 
 ## Workflow
 
 ### Setup
 
-Download index files
+**Download index files**, which contain the firm CIK, name, filing date, type, and URL of the filing.
 
 ```bash
 edgar-analyzer download_index --user_agent "MyCompany name@mycompany.com" --output "./index"
 ```
 
-Download filings (to be integrated)
+**Build a database** of the previously download index files for more efficient queries.
 
 ```bash
-edgar_analyzer download_filings
+edgar_analyzer build_database --inputdir "./index" --database "edgar-idx.sqlite3"
 ```
 
-Build database (to be integrated)
+Download filings (to be integrated)
 
 ```bash
-edgar_analyzer build_database
+edgar_analyzer download_filings
 ```
 
 ### Run specific jobs
 
 These tasks can be executed once the database of filings is built.
 
 #### Find event date
```

### Comparing `edgar-analyzer-0.0.1rc2/README.md` & `edgar-analyzer-0.0.1rc3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 pip install edgar-analyzer
 ```
 
 ## Workflow
 
 ### Setup
 
-Download index files
+**Download index files**, which contain the firm CIK, name, filing date, type, and URL of the filing.
 
 ```bash
 edgar-analyzer download_index --user_agent "MyCompany name@mycompany.com" --output "./index"
 ```
 
-Download filings (to be integrated)
+**Build a database** of the previously download index files for more efficient queries.
 
 ```bash
-edgar_analyzer download_filings
+edgar_analyzer build_database --inputdir "./index" --database "edgar-idx.sqlite3"
 ```
 
-Build database (to be integrated)
+Download filings (to be integrated)
 
 ```bash
-edgar_analyzer build_database
+edgar_analyzer download_filings
 ```
 
 ### Run specific jobs
 
 These tasks can be executed once the database of filings is built.
 
 #### Find event date
```

### Comparing `edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/PKG-INFO` & `edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-analyzer
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Textual analysis on SEC filings from EDGAR
 Home-page: https://github.com/mgao6767/edgar-analyzer
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,30 +27,30 @@
 pip install edgar-analyzer
 ```
 
 ## Workflow
 
 ### Setup
 
-Download index files
+**Download index files**, which contain the firm CIK, name, filing date, type, and URL of the filing.
 
 ```bash
 edgar-analyzer download_index --user_agent "MyCompany name@mycompany.com" --output "./index"
 ```
 
-Download filings (to be integrated)
+**Build a database** of the previously download index files for more efficient queries.
 
 ```bash
-edgar_analyzer download_filings
+edgar_analyzer build_database --inputdir "./index" --database "edgar-idx.sqlite3"
 ```
 
-Build database (to be integrated)
+Download filings (to be integrated)
 
 ```bash
-edgar_analyzer build_database
+edgar_analyzer download_filings
 ```
 
 ### Run specific jobs
 
 These tasks can be executed once the database of filings is built.
 
 #### Find event date
```

### Comparing `edgar-analyzer-0.0.1rc2/edgar_analyzer.egg-info/SOURCES.txt` & `edgar-analyzer-0.0.1rc3/edgar_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/__init__.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import types
 import sys
 
-__version__ = "0.0.1rc2"
+__version__ = "0.0.1rc3"
 __description__ = "Textual analysis on SEC filings from EDGAR"
 __author__ = "Mingze Gao"
 __author_email__ = "mingze.gao@sydney.edu.au"
 __url__ = "https://github.com/mgao6767/edgar-analyzer"
 
 if sys.version_info.major < 3 and sys.version_info.minor < 10:
     print("Python3.10 or higher is required.")
```

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_event_date.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_event_date.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_items.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_items.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_loans.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_loans.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_find_zipcode.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_find_zipcode.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/cmd_sample_loans.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/cmd_sample_loans.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/main.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,29 @@
     )
     parser_sample_loans = subparsers.add_parser(
         CMD.SAMPLE_LOANS,
         description="Randomly sample loan contracts from filings",
         help="Sample loan contracts from filings",
     )
 
+    parser_build_db.add_argument(
+        "-db",
+        "--database",
+        metavar="database",
+        default="edgar-idx.sqlite3",
+        help="output sqlite database to store results. Defaults to `edgar-idx.sqlite3`",
+    )
+    required = parser_build_db.add_argument_group("required named arguments")
+    required.add_argument(
+        "-i",
+        "--inputdir",
+        metavar="inputdir",
+        help="input directory of index files from `download_index`",
+    )
+
     # subparser for `download_index` subcommand
     required = parser_download.add_argument_group("required named arguments")
     required.add_argument(
         "-ua",
         "--user_agent",
         required=True,
         metavar="user_agent",
```

### Comparing `edgar-analyzer-0.0.1rc2/edgaranalyzer/utils.py` & `edgar-analyzer-0.0.1rc3/edgaranalyzer/utils.py`

 * *Files identical despite different names*

### Comparing `edgar-analyzer-0.0.1rc2/setup.py` & `edgar-analyzer-0.0.1rc3/setup.py`

 * *Files identical despite different names*

