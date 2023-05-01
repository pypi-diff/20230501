# Comparing `tmp/proteus-6.6.2.tar.gz` & `tmp/proteus-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus-6.6.2.tar", last modified: Sun Feb  5 20:59:56 2023, max compression
+gzip compressed data, was "proteus-6.8.0.tar", last modified: Mon May  1 12:07:02 2023, max compression
```

## Comparing `proteus-6.6.2.tar` & `proteus-6.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 20:59:56.385787 proteus-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-02-05 20:59:53.000000 proteus-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-02-05 20:59:53.000000 proteus-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    42788 2022-12-19 12:02:59.000000 proteus-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2022-12-19 12:02:59.000000 proteus-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-02-05 20:59:56.385787 proteus-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4178 2022-12-19 12:02:59.000000 proteus-6.6.2/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 20:59:56.379120 proteus-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2022-12-19 12:02:59.000000 proteus-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4178 2022-12-19 12:02:59.000000 proteus-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:59.000000 proteus-6.6.2/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 20:59:56.379120 proteus-6.6.2/proteus/
--rw-r--r--   0 ced       (1000) ced       (1000)    48690 2023-02-05 20:48:28.000000 proteus-6.6.2/proteus/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12626 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21766 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 20:59:56.385787 proteus-6.6.2/proteus/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1484 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/test_config.py
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/test_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12536 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/test_readme.py
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2150 2022-12-19 12:02:59.000000 proteus-6.6.2/proteus/tests/test_wizard.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 20:59:56.382454 proteus-6.6.2/proteus.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-02-05 20:59:55.000000 proteus-6.6.2/proteus.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      569 2023-02-05 20:59:56.000000 proteus-6.6.2/proteus.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 20:59:55.000000 proteus-6.6.2/proteus.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-02-05 20:59:55.000000 proteus-6.6.2/proteus.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 20:59:55.000000 proteus-6.6.2/proteus.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 20:59:55.000000 proteus-6.6.2/proteus.egg-info/zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 20:59:56.385787 proteus-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2958 2022-12-19 12:02:59.000000 proteus-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2022-12-19 12:02:59.000000 proteus-6.6.2/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:02.218018 proteus-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4252 2023-05-01 11:18:51.000000 proteus-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-05-01 11:18:51.000000 proteus-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    42788 2023-01-16 14:00:21.000000 proteus-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-04-15 07:12:15.000000 proteus-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     5510 2023-05-01 12:07:02.218018 proteus-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-04-15 07:12:15.000000 proteus-6.8.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:02.211351 proteus-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-04-15 07:12:15.000000 proteus-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-04-15 07:12:15.000000 proteus-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 proteus-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:02.214684 proteus-6.8.0/proteus/
+-rw-r--r--   0 ced       (1000) ced       (1000)    49397 2023-05-01 11:18:45.000000 proteus-6.8.0/proteus/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13340 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21766 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:02.218018 proteus-6.8.0/proteus/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1484 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/test_config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-01-16 14:00:21.000000 proteus-6.8.0/proteus/tests/test_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12536 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/test_readme.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2150 2023-04-15 07:12:15.000000 proteus-6.8.0/proteus/tests/test_wizard.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:07:02.214684 proteus-6.8.0/proteus.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5510 2023-05-01 12:07:01.000000 proteus-6.8.0/proteus.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      569 2023-05-01 12:07:02.000000 proteus-6.8.0/proteus.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:07:01.000000 proteus-6.8.0/proteus.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-05-01 12:07:01.000000 proteus-6.8.0/proteus.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:07:01.000000 proteus-6.8.0/proteus.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 proteus-6.8.0/proteus.egg-info/zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:07:02.218018 proteus-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2938 2023-04-15 07:12:15.000000 proteus-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-04-15 07:12:15.000000 proteus-6.8.0/tox.ini
```

### Comparing `proteus-6.6.2/CHANGELOG` & `proteus-6.8.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-Version 6.6.2 - 2023-02-05
---------------------------
-* Bug fixes (see mercurial logs for details)
 
-Version 6.6.1 - 2022-11-17
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Manage RPCReturnException
+* Run action from button
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 --------------------------
```

### Comparing `proteus-6.6.2/COPYRIGHT` & `proteus-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/LICENSE` & `proteus-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/PKG-INFO` & `proteus-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: proteus
-Version: 6.6.2
+Version: 6.8.0
 Summary: Library to access Tryton server as a client
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: LGPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/proteus
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton library cli
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: trytond
 Provides-Extra: test
 License-File: LICENSE
 
 =======================
 Tryton Scripting Client
 =======================
```

### Comparing `proteus-6.6.2/README.rst` & `proteus-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/doc/conf.py` & `proteus-6.8.0/doc/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     return info
```

### Comparing `proteus-6.6.2/doc/index.rst` & `proteus-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/__init__.py` & `proteus-6.8.0/proteus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import datetime
 import functools
 import threading
 from decimal import Decimal
 
 import proteus.config
 
-__version__ = "6.6.2"
+__version__ = "6.8.0"
 __all__ = ['Model', 'Wizard', 'Report']
 
 _MODELS = threading.local()
 
 
 class _EvalEnvironment(dict):
     'Dictionary for evaluation'
@@ -909,15 +909,23 @@
             assert proxy == record._proxy
             assert config == record._config
             assert context == record._context
 
         if change is None:
             cls.save(records)
             cls.reload(records)  # Force reload because save doesn't always
-            return getattr(proxy, button)([r.id for r in records], context)
+            record_ids = [r.id for r in records]
+            action = getattr(proxy, button)(record_ids, context)
+            if action and not isinstance(action, str):
+                if isinstance(action, int):
+                    action = config.get_proxy('ir.action').get_action_value(
+                        action, context)
+                return _convert_action(
+                    action, records, context=context, config=config)
+            return action
         else:
             record, = records
             values = record._on_change_args(change)
             changes = getattr(proxy, button)(values, context)
             record._set_on_change(changes)
 
     def _get_values(self, fields=None):
@@ -1298,16 +1306,24 @@
                 data['model'] = models[0].__class__.__name__
         return self._proxy.execute(ids, data, self._context)
 
 
 def _convert_action(action, data=None, context=None, config=None):
     if config is None:
         config = proteus.config.get_config()
+    records = None
     if data is None:
         data = {}
+    elif isinstance(data, (list, tuple)):
+        records = data
+        data = {
+            'model': records[0].__class__.__name__,
+            'id': records[0].id,
+            'ids': [r.id for r in records],
+            }
     else:
         data = data.copy()
 
     if 'type' not in (action or {}):
         return None
 
     data['action_id'] = action['id']
@@ -1348,15 +1364,17 @@
                 return [Model_(id_) for id_ in res_id]
     elif action['type'] == 'ir.action.wizard':
         kwargs = {
             'action': action,
             'config': config,
             'context': context,
             }
-        if 'model' in data:
+        if records is not None:
+            kwargs['models'] = records
+        elif 'model' in data:
             Model_ = Model.get(data['model'], config)
             config = Model_._config
             with config.reset_context(), config.set_context(context):
                 kwargs['models'] = [Model_(id_) for id_ in data.get('ids', [])]
         return Wizard(action['wiz_name'], **kwargs)
     elif action['type'] == 'ir.action.report':
         ActionReport = Report(action['report_name'], context=context)
```

### Comparing `proteus-6.6.2/proteus/config.py` & `proteus-6.8.0/proteus/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,43 +177,59 @@
     def __init__(self, name, model, config):
         super(_TrytondMethod, self).__init__()
         self._name = name
         self._object = model
         self._config = config
 
     def __call__(self, *args, **kwargs):
-        from trytond.rpc import RPC
+        from trytond.rpc import RPC, RPCReturnException
         from trytond.tools import is_instance_method
-        from trytond.transaction import Transaction
+        from trytond.transaction import Transaction, TransactionError
         from trytond.worker import run_task
 
         if self._name in self._object.__rpc__:
             rpc = self._object.__rpc__[self._name]
         elif self._name in getattr(self._object, '_buttons', {}):
             rpc = RPC(readonly=False, instantiate=0)
         else:
             raise TypeError('%s is not callable' % self._name)
 
-        with Transaction().start(self._config.database_name,
-                self._config.user, readonly=rpc.readonly) as transaction:
-            args, kwargs, transaction.context, transaction.timestamp = \
-                rpc.convert(self._object, *args, **kwargs)
-            meth = getattr(self._object, self._name)
-            if (rpc.instantiate is None
-                    or not is_instance_method(self._object, self._name)):
-                result = rpc.result(meth(*args, **kwargs))
-            else:
-                assert rpc.instantiate == 0
-                inst = args.pop(0)
-                if hasattr(inst, self._name):
-                    result = rpc.result(meth(inst, *args, **kwargs))
-                else:
-                    result = [rpc.result(meth(i, *args, **kwargs))
-                        for i in inst]
-            transaction.commit()
+        extras = {}
+        while True:
+            with Transaction().start(self._config.database_name,
+                    self._config.user, readonly=rpc.readonly,
+                    **extras) as transaction:
+                try:
+                    (c_args, c_kwargs,
+                        transaction.context, transaction.timestamp) \
+                            = rpc.convert(self._object, *args, **kwargs)
+                    meth = getattr(self._object, self._name)
+                    if (rpc.instantiate is None
+                            or not is_instance_method(
+                                self._object, self._name)):
+                        result = rpc.result(meth(*c_args, **c_kwargs))
+                    else:
+                        assert rpc.instantiate == 0
+                        inst = c_args.pop(0)
+                        if hasattr(inst, self._name):
+                            result = rpc.result(
+                                meth(inst, *c_args, **c_kwargs))
+                        else:
+                            result = [rpc.result(meth(i, *c_args, **c_kwargs))
+                                for i in inst]
+                except TransactionError as e:
+                    transaction.rollback()
+                    e.fix(extras)
+                    continue
+                except RPCReturnException as e:
+                    transaction.rollback()
+                    transaction.tasks.clear()
+                    result = e.result()
+                transaction.commit()
+            break
         while transaction.tasks:
             task_id = transaction.tasks.pop()
             run_task(self._config.database_name, task_id)
         return result
 
 
 class TrytondProxy(object):
```

### Comparing `proteus-6.6.2/proteus/pyson.py` & `proteus-6.8.0/proteus/pyson.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/tests/test_config.py` & `proteus-6.8.0/proteus/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/tests/test_context.py` & `proteus-6.8.0/proteus/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/tests/test_model.py` & `proteus-6.8.0/proteus/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/tests/test_readme.py` & `proteus-6.8.0/proteus/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/tests/test_report.py` & `proteus-6.8.0/proteus/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus/tests/test_wizard.py` & `proteus-6.8.0/proteus/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/proteus.egg-info/PKG-INFO` & `proteus-6.8.0/proteus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: proteus
-Version: 6.6.2
+Version: 6.8.0
 Summary: Library to access Tryton server as a client
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: LGPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/proteus
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton library cli
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: trytond
 Provides-Extra: test
 License-File: LICENSE
 
 =======================
 Tryton Scripting Client
 =======================
```

### Comparing `proteus-6.6.2/proteus.egg-info/SOURCES.txt` & `proteus-6.8.0/proteus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteus-6.6.2/setup.py` & `proteus-6.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,69 +23,69 @@
 
 def get_version():
     init = read(os.path.join('proteus', '__init__.py'))
     return re.search('__version__ = "([0-9.]*)"', init).group(1)
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 name = 'proteus'
 version = get_version()
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 setup(name=name,
     version=version,
     description='Library to access Tryton server as a client',
     long_description=readme(),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/proteus',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton library cli',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Framework :: Tryton',
         'Intended Audience :: Developers',
         'Intended Audience :: Financial and Insurance Industry',
         'Intended Audience :: Legal Industry',
         'License :: OSI Approved :: '
         'GNU Library or Lesser General Public License (LGPL)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     platforms='any',
     license='LGPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'defusedxml',
         "python-dateutil",
         ],
     extras_require={
         'trytond': [get_require_version('trytond')],
         'test': [
```

