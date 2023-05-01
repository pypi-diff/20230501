# Comparing `tmp/dbm_database_service-0.2.4.tar.gz` & `tmp/dbm_database_service-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm_database_service-0.2.4.tar", max compression
+gzip compressed data, was "dbm_database_service-0.2.5.tar", max compression
```

## Comparing `dbm_database_service-0.2.4.tar` & `dbm_database_service-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.4/dbm_database_service/__init__.py
--rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.4/dbm_database_service/connectors.py
--rw-r--r--   0        0        0     3208 2023-04-20 19:41:30.227951 dbm_database_service-0.2.4/dbm_database_service/managers.py
--rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.4/dbm_database_service/models/__init__.py
--rw-r--r--   0        0        0     1616 2023-04-20 19:48:51.057728 dbm_database_service-0.2.4/dbm_database_service/models/column.py
--rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.4/dbm_database_service/models/config.py
--rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.4/dbm_database_service/models/datatype.py
--rw-r--r--   0        0        0      930 2023-04-20 19:41:30.108418 dbm_database_service-0.2.4/dbm_database_service/models/table.py
--rw-r--r--   0        0        0      655 2023-04-20 22:18:11.978518 dbm_database_service-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    13467 2023-04-18 09:36:53.242538 dbm_database_service-0.2.4/README.md
--rw-r--r--   0        0        0    13586 1970-01-01 00:00:00.000000 dbm_database_service-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.5/dbm_database_service/__init__.py
+-rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.5/dbm_database_service/connectors.py
+-rw-r--r--   0        0        0     3208 2023-04-20 19:41:30.227951 dbm_database_service-0.2.5/dbm_database_service/managers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.5/dbm_database_service/models/__init__.py
+-rw-r--r--   0        0        0     1616 2023-04-20 19:48:51.057728 dbm_database_service-0.2.5/dbm_database_service/models/column.py
+-rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.5/dbm_database_service/models/config.py
+-rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.5/dbm_database_service/models/datatype.py
+-rw-r--r--   0        0        0      930 2023-04-20 19:41:30.108418 dbm_database_service-0.2.5/dbm_database_service/models/table.py
+-rw-r--r--   0        0        0      655 2023-05-01 15:07:40.697753 dbm_database_service-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    13467 2023-04-18 09:36:53.242538 dbm_database_service-0.2.5/README.md
+-rw-r--r--   0        0        0    13586 1970-01-01 00:00:00.000000 dbm_database_service-0.2.5/PKG-INFO
```

### Comparing `dbm_database_service-0.2.4/dbm_database_service/connectors.py` & `dbm_database_service-0.2.5/dbm_database_service/connectors.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/dbm_database_service/managers.py` & `dbm_database_service-0.2.5/dbm_database_service/managers.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/dbm_database_service/models/column.py` & `dbm_database_service-0.2.5/dbm_database_service/models/column.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/dbm_database_service/models/config.py` & `dbm_database_service-0.2.5/dbm_database_service/models/config.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/dbm_database_service/models/datatype.py` & `dbm_database_service-0.2.5/dbm_database_service/models/datatype.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/dbm_database_service/models/table.py` & `dbm_database_service-0.2.5/dbm_database_service/models/table.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/README.md` & `dbm_database_service-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.4/PKG-INFO` & `dbm_database_service-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbm-database-service
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: easyvalid-data-validator (>=0.1.1,<0.2.0)
+Requires-Dist: easyvalid-data-validator (>=2.0.1,<3.0.0)
 Requires-Dist: gdown (>=4.7.1,<5.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.32,<9.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # dbm-database-service
```

