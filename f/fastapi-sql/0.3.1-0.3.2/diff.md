# Comparing `tmp/fastapi_sql-0.3.1.tar.gz` & `tmp/fastapi_sql-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.3.1.tar", max compression
+gzip compressed data, was "fastapi_sql-0.3.2.tar", max compression
```

## Comparing `fastapi_sql-0.3.1.tar` & `fastapi_sql-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2675 2023-04-29 14:17:13.931355 fastapi_sql-0.3.1/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.1/fastapi_sql/middleware.py
--rw-r--r--   0        0        0     1633 2023-04-29 14:17:59.957045 fastapi_sql-0.3.1/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.1/fastapi_sql/model.py
--rw-r--r--   0        0        0      417 2023-04-29 13:28:56.702169 fastapi_sql-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2735 2023-04-29 15:45:15.036947 fastapi_sql-0.3.2/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.2/fastapi_sql/middleware.py
+-rw-r--r--   0        0        0     1562 2023-04-29 15:43:30.819501 fastapi_sql-0.3.2/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.2/fastapi_sql/model.py
+-rw-r--r--   0        0        0      417 2023-05-01 18:43:47.293365 fastapi_sql-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.2/PKG-INFO
```

### Comparing `fastapi_sql-0.3.1/fastapi_sql/__init__.py` & `fastapi_sql-0.3.2/fastapi_sql/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         )
         if kwargs.get('naming_convention') is not None:
             self.__naming_conventions__ = kwargs.get('naming_convention', {})
         self.__metadata__ = MetaData(naming_convention=self.__naming_conventions__)
         self.Model = self._make_declarative_base() # type: ignore
         self.__engine_uri__ = database_uri
         self.migration.cfg.set_main_option('sqlalchemy.url', database_uri)
+        self.migration.cfg.config_file_name = 'alembic.ini'
         if app is not None:
             app.add_middleware(self.middleware, sqlalchemy=self)
             
     def init_app(self, app: FastAPI):
         app.add_middleware(self.middleware, sqlalchemy=self)
     
     async def create_all(self):
```

### Comparing `fastapi_sql-0.3.1/fastapi_sql/middleware.py` & `fastapi_sql-0.3.2/fastapi_sql/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.1/fastapi_sql/migrate.py` & `fastapi_sql-0.3.2/fastapi_sql/migrate.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 class Migration:
     sqlalchemy = None
     cfg = Config()
     
     @staticmethod
     def init():
-        command.init(Migration.cfg, 'migrations', package=True, template='async')
-        Migration.cfg.set_main_option('script_location', 'migrations')
+        command.init(Migration.cfg, 'migrations', template='async', package=True)
         
     @staticmethod
     def revision():
         Migration.cfg.set_main_option('script_location', 'migrations')
         command.revision(Migration.cfg)
         
     @staticmethod
```

### Comparing `fastapi_sql-0.3.1/fastapi_sql/model.py` & `fastapi_sql-0.3.2/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.1/PKG-INFO` & `fastapi_sql-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

