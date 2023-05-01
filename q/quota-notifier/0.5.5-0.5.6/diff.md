# Comparing `tmp/quota_notifier-0.5.5.tar.gz` & `tmp/quota_notifier-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quota_notifier-0.5.5.tar", max compression
+gzip compressed data, was "quota_notifier-0.5.6.tar", max compression
```

## Comparing `quota_notifier-0.5.5.tar` & `quota_notifier-0.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34906 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/LICENSE.md
--rw-r--r--   0        0        0      653 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/README.md
--rw-r--r--   0        0        0     1287 2023-04-16 17:28:01.067424 quota_notifier-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1476 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/__init__.py
--rw-r--r--   0        0        0      202 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/__main__.py
--rw-r--r--   0        0        0     6664 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/cli.py
--rw-r--r--   0        0        0      298 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/data/template.html
--rw-r--r--   0        0        0    10990 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/disk_utils.py
--rw-r--r--   0        0        0    10315 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/notify.py
--rw-r--r--   0        0        0     3220 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/orm.py
--rw-r--r--   0        0        0     8626 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/settings.py
--rw-r--r--   0        0        0     2874 2023-04-16 17:27:42.347251 quota_notifier-0.5.5/quota_notifier/shell.py
--rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 quota_notifier-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    34906 2023-05-01 16:10:25.970055 quota_notifier-0.5.6/LICENSE.md
+-rw-r--r--   0        0        0      653 2023-05-01 16:10:25.970055 quota_notifier-0.5.6/README.md
+-rw-r--r--   0        0        0     1288 2023-05-01 16:10:43.702262 quota_notifier-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1506 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/__init__.py
+-rw-r--r--   0        0        0      202 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/__main__.py
+-rw-r--r--   0        0        0     6662 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/cli.py
+-rw-r--r--   0        0        0      298 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/data/template.html
+-rw-r--r--   0        0        0    10990 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/disk_utils.py
+-rw-r--r--   0        0        0    10400 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/notify.py
+-rw-r--r--   0        0        0     3220 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/orm.py
+-rw-r--r--   0        0        0     8626 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/settings.py
+-rw-r--r--   0        0        0     2874 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/shell.py
+-rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 quota_notifier-0.5.6/PKG-INFO
```

### Comparing `quota_notifier-0.5.5/LICENSE.md` & `quota_notifier-0.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.5/README.md` & `quota_notifier-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.5/pyproject.toml` & `quota_notifier-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "quota-notifier"
-version = "0.5.5"  # Version is set dynamically by the CI tool on publication
+version = "0.5.6"  # Version is set dynamically by the CI tool on publication
 authors = ["Pitt Center for Research Computing", ]
 readme = "README.md"
 description = "Automatic email notification tool for disk quota usage."
 homepage = "https://github.com/pitt-crc/quota_notifier"
 repository = "https://github.com/pitt-crc/quota_notifier"
 documentation = "https://crc-pages.pitt.edu/quota_notifier/"
 keywords = ["disk", "usage", "quota", "notify", "email", ]
@@ -25,19 +25,19 @@
 
 [tool.poetry.scripts]
 notifier = "quota_notifier.cli:Application.execute"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pydantic = "1.10.7"
-sqlalchemy = "2.0.8"
+sqlalchemy = "2.0.12"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "5.3.0"
+sphinx = "6.2.1"
 sphinx-argparse = "0.4.0"
-sphinx-copybutton = "0.5.1"
+sphinx-copybutton = "0.5.2"
 sphinx-pydantic = "0.1.1"
 sphinx-rtd-theme = "1.2.0"
 sphinx-jsonschema = "1.15"
```

### Comparing `quota_notifier-0.5.5/quota_notifier/__init__.py` & `quota_notifier-0.5.6/quota_notifier/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 However, a user will receive additional notifications if their usage drops below
 a threshold before exceeding the threshold a second time.
 """
 
 import importlib.metadata
 
 try:
-    __version__ = importlib.metadata.version('asdf')
+    __version__ = importlib.metadata.version('quota-notifier')
 
-except importlib.metadata.PackageNotFoundError:
+except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = '0.0.0'
```

### Comparing `quota_notifier-0.5.5/quota_notifier/cli.py` & `quota_notifier-0.5.6/quota_notifier/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,8 +178,8 @@
                 debug=args.debug)
 
         except Exception as caught:
             logging.getLogger('file_logger').critical('Application crash', exc_info=caught)
             logging.getLogger('console_logger').critical(str(caught))
 
         else:
-            logging.info('Exiting application successfully')
+            logging.info('Exiting application gracefully')
```

### Comparing `quota_notifier-0.5.5/quota_notifier/disk_utils.py` & `quota_notifier-0.5.6/quota_notifier/disk_utils.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.5/quota_notifier/notify.py` & `quota_notifier-0.5.6/quota_notifier/notify.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,9 +285,10 @@
 
         logging.info('Scanning user quotas...')
         for user in users:
             try:
                 self.notify_user(user)
 
             except Exception as caught:
+                # Only include exception information in the logfile, not the console
                 logging.getLogger('file_logger').error(f'Error notifying {user}', exc_info=caught)
                 logging.getLogger('console_logger').error(f'Error notifying {user} - {caught}')
```

### Comparing `quota_notifier-0.5.5/quota_notifier/orm.py` & `quota_notifier-0.5.6/quota_notifier/orm.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.5/quota_notifier/settings.py` & `quota_notifier-0.5.6/quota_notifier/settings.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.5/quota_notifier/shell.py` & `quota_notifier-0.5.6/quota_notifier/shell.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.5/PKG-INFO` & `quota_notifier-0.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quota-notifier
-Version: 0.5.5
+Version: 0.5.6
 Summary: Automatic email notification tool for disk quota usage.
 Home-page: https://github.com/pitt-crc/quota_notifier
 Keywords: disk,usage,quota,notify,email
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Monitoring
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (==1.10.7)
-Requires-Dist: sqlalchemy (==2.0.8)
+Requires-Dist: sqlalchemy (==2.0.12)
 Project-URL: Documentation, https://crc-pages.pitt.edu/quota_notifier/
 Project-URL: Repository, https://github.com/pitt-crc/quota_notifier
 Description-Content-Type: text/markdown
 
 # Storage Quota Notifier
 
 [![](https://app.codacy.com/project/badge/Grade/583c607400c2429ebbc1554d777d26b4)](https://app.codacy.com/gh/pitt-crc/quota_notifier/dashboard)
```

