# Comparing `tmp/sqlitemanager-0.7.1.tar.gz` & `tmp/sqlitemanager-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitemanager-0.7.1.tar", last modified: Sun Apr 30 19:27:45 2023, max compression
+gzip compressed data, was "sqlitemanager-0.7.2.tar", last modified: Mon May  1 08:45:09 2023, max compression
```

## Comparing `sqlitemanager-0.7.1.tar` & `sqlitemanager-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)    35149 2023-04-13 10:16:08.000000 sqlitemanager-0.7.1/LICENSE
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3532 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/PKG-INFO
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3030 2023-04-30 19:27:06.000000 sqlitemanager-0.7.1/README.md
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)       38 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/setup.cfg
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)      717 2023-04-30 19:24:45.000000 sqlitemanager-0.7.1/setup.py
-drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-30 19:27:45.215454 sqlitemanager-0.7.1/sqlitemanager/
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-13 10:16:08.000000 sqlitemanager-0.7.1/sqlitemanager/__init__.py
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)    32924 2023-04-30 14:45:01.000000 sqlitemanager-0.7.1/sqlitemanager/handler.py
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     7039 2023-04-30 18:25:11.000000 sqlitemanager-0.7.1/sqlitemanager/objects.py
-drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-30 19:27:45.216454 sqlitemanager-0.7.1/sqlitemanager.egg-info/
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3532 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/PKG-INFO
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)      250 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/SOURCES.txt
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        1 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/dependency_links.txt
--rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)       14 2023-04-30 19:27:45.000000 sqlitemanager-0.7.1/sqlitemanager.egg-info/top_level.txt
+drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-05-01 08:45:09.480743 sqlitemanager-0.7.2/
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)    35149 2023-04-13 10:16:08.000000 sqlitemanager-0.7.2/LICENSE
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3574 2023-05-01 08:45:09.480743 sqlitemanager-0.7.2/PKG-INFO
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3072 2023-05-01 08:44:42.000000 sqlitemanager-0.7.2/README.md
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)       38 2023-05-01 08:45:09.480743 sqlitemanager-0.7.2/setup.cfg
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)      717 2023-05-01 08:43:37.000000 sqlitemanager-0.7.2/setup.py
+drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-05-01 08:45:09.479743 sqlitemanager-0.7.2/sqlitemanager/
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-04-13 10:16:08.000000 sqlitemanager-0.7.2/sqlitemanager/__init__.py
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)    32717 2023-05-01 08:41:43.000000 sqlitemanager-0.7.2/sqlitemanager/handler.py
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     7039 2023-04-30 18:25:11.000000 sqlitemanager-0.7.2/sqlitemanager/objects.py
+drwxr-xr-x   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        0 2023-05-01 08:45:09.479743 sqlitemanager-0.7.2/sqlitemanager.egg-info/
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)     3574 2023-05-01 08:45:09.000000 sqlitemanager-0.7.2/sqlitemanager.egg-info/PKG-INFO
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)      250 2023-05-01 08:45:09.000000 sqlitemanager-0.7.2/sqlitemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)        1 2023-05-01 08:45:09.000000 sqlitemanager-0.7.2/sqlitemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 yongshi-fedora  (1000) yongshi-fedora  (1000)       14 2023-05-01 08:45:09.000000 sqlitemanager-0.7.2/sqlitemanager.egg-info/top_level.txt
```

### Comparing `sqlitemanager-0.7.1/LICENSE` & `sqlitemanager-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlitemanager-0.7.1/PKG-INFO` & `sqlitemanager-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlitemanager
-Version: 0.7.1
+Version: 0.7.2
 Summary: Handler object for easy sqlite manipulation
 Home-page: https://github.com/Michael-Yongshi/SQLiteManager
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,25 +13,30 @@
 License-File: LICENSE
 
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
-### 0.7.1
+### 0.7
+0.7.2
+- added get_latest_record function
+
+0.7.1
 - added Record.values (list of values)
 
-### 0.7.0
+0.7.0
 - Completely redone, not backwards compatible at all
 - Contains most of the previous functionality
 
-### 0.6.1
+### 0.6
+0.6.1
 - extra logging for printing path
 
-### 0.6.0
+0.6.0
 - Extension type can be given to the handler to discern between .sqlite and .sqlite3
 - changed many functions to depend on the location variables of the handler class (path, filename, extension)
 make sure the extension variable does not miss the dot!
 - removed redundent steps or functions, mostly from the database class and added to the handler
 - added some more comments for functions
 - other fixes
```

### Comparing `sqlitemanager-0.7.1/README.md` & `sqlitemanager-0.7.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
-### 0.7.1
+### 0.7
+0.7.2
+- added get_latest_record function
+
+0.7.1
 - added Record.values (list of values)
 
-### 0.7.0
+0.7.0
 - Completely redone, not backwards compatible at all
 - Contains most of the previous functionality
 
-### 0.6.1
+### 0.6
+0.6.1
 - extra logging for printing path
 
-### 0.6.0
+0.6.0
 - Extension type can be given to the handler to discern between .sqlite and .sqlite3
 - changed many functions to depend on the location variables of the handler class (path, filename, extension)
 make sure the extension variable does not miss the dot!
 - removed redundent steps or functions, mostly from the database class and added to the handler
 - added some more comments for functions
 - other fixes
```

### Comparing `sqlitemanager-0.7.1/setup.py` & `sqlitemanager-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlitemanager",
-    version="0.7.1",
+    version="0.7.2",
     author="Michael-Yongshi",
     author_email="4registration@outlook.com",
     description="Handler object for easy sqlite manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Michael-Yongshi/SQLiteManager",
     packages=setuptools.find_packages(),
```

### Comparing `sqlitemanager-0.7.1/sqlitemanager/handler.py` & `sqlitemanager-0.7.2/sqlitemanager/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,31 @@
 
     records = get_records(db, table_name, columns, where)
     if len(records) == 1:
         return records[0]
     else:
         logging.warning("No or multiple records found, please use 'get_records' when fetching multiple records or provide a unique where clause")
 
+def get_latest_record(db, table_name, column_name):
+
+    query = f"SELECT MAX({column_name}) FROM {table_name}"
+    cursor = db.execute_query(query)
+    result = cursor.fetchone()
+
+    # if no record is found return 0
+    if result == []:
+        return None
+
+    # else return the found value
+    else:
+        where = {column_name:{
+        "operator":"=",
+        "values":result[0]}}
+        return get_record(db=db, table_name=table_name, where=where)
+
 def get_records(db, table_name, columns=[], where={}):
     """
     fetches a selection of records of a table with optionally a selection of the columns and a where clause
 
     column selection is just an array of the column names or a string for just a single column
 
     where can be collected as {
@@ -677,18 +694,14 @@
 #     # records = self.table_read_records(table_name=table_name, where=where)
 #     # foreign_keys = []
 #     # for record in records:
 #     #     foreign_keys += [record.recorddict[column]]
 
 #     return records
 
-# def table_max_row(self, table_name):
-#     lastrow = self.database.get_max_row(table_name)
-#     return lastrow
-
 
 # def crossref_get(self, table_name1, table_name2):
 #     """
 #     Gets a crossreference table for tables with given table names if it exists.
 #     will check first the following combination
 #     "CROSSREF_table_name1_table_name2"
 #     and if table != found will check
@@ -965,26 +978,7 @@
 #         table_name = table.name,
 #         column_names = table.column_names[1:],
 #         valuepairs = values,
 #     )
 
 
 
-# def get_max_row(self, table_name):
-
-#     cursor = self.execute_query(f"SELECT COUNT(id) FROM {table_name}")
-#     lastrow = cursor.fetchall()[0][0]
-#     if lastrow == None:
-#         lastrow = 0
-
-#     return lastrow
-
-# def get_max_columncontent(self, table, column):
-
-        # query = f"SELECT MAX({column}) FROM {table}"
-
-        # cursor = self.execute_query(query)
-        # max_columncontent = cursor.fetchall()
-        # if max_columncontent[0][0] == None:
-        #     max_columncontent = [(0,)]
-
-        # return max_columncontent[0][0]
```

### Comparing `sqlitemanager-0.7.1/sqlitemanager/objects.py` & `sqlitemanager-0.7.2/sqlitemanager/objects.py`

 * *Files identical despite different names*

### Comparing `sqlitemanager-0.7.1/sqlitemanager.egg-info/PKG-INFO` & `sqlitemanager-0.7.2/sqlitemanager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlitemanager
-Version: 0.7.1
+Version: 0.7.2
 Summary: Handler object for easy sqlite manipulation
 Home-page: https://github.com/Michael-Yongshi/SQLiteManager
 Author: Michael-Yongshi
 Author-email: 4registration@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,25 +13,30 @@
 License-File: LICENSE
 
 # SQLiteManager
 Use a convenient SQLiteHandler object to manipulate SQLite(3) databases.
 
 ## Version
 
-### 0.7.1
+### 0.7
+0.7.2
+- added get_latest_record function
+
+0.7.1
 - added Record.values (list of values)
 
-### 0.7.0
+0.7.0
 - Completely redone, not backwards compatible at all
 - Contains most of the previous functionality
 
-### 0.6.1
+### 0.6
+0.6.1
 - extra logging for printing path
 
-### 0.6.0
+0.6.0
 - Extension type can be given to the handler to discern between .sqlite and .sqlite3
 - changed many functions to depend on the location variables of the handler class (path, filename, extension)
 make sure the extension variable does not miss the dot!
 - removed redundent steps or functions, mostly from the database class and added to the handler
 - added some more comments for functions
 - other fixes
```

