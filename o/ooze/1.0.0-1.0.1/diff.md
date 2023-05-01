# Comparing `tmp/ooze-1.0.0.tar.gz` & `tmp/ooze-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooze-1.0.0.tar", last modified: Fri Apr 28 23:57:21 2023, max compression
+gzip compressed data, was "ooze-1.0.1.tar", last modified: Mon May  1 02:28:30 2023, max compression
```

## Comparing `ooze-1.0.0.tar` & `ooze-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.611228 ooze-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-28 23:56:58.000000 ooze-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-04-28 23:57:21.611228 ooze-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 23:56:58.000000 ooze-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.607228 ooze-1.0.0/ooze/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-28 23:56:58.000000 ooze-1.0.0/ooze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 23:56:58.000000 ooze-1.0.0/ooze/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.611228 ooze-1.0.0/ooze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 23:57:21.000000 ooze-1.0.0/ooze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-28 23:56:58.000000 ooze-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 23:57:21.611228 ooze-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 23:56:58.000000 ooze-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:57:21.611228 ooze-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-28 23:56:58.000000 ooze-1.0.0/tests/test_ooze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-28 23:56:58.000000 ooze-1.0.0/tests/test_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:28:30.119330 ooze-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 02:27:59.000000 ooze-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42690 2023-05-01 02:28:30.119330 ooze-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-01 02:27:59.000000 ooze-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:28:30.115330 ooze-1.0.1/ooze/
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-01 02:27:59.000000 ooze-1.0.1/ooze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-01 02:27:59.000000 ooze-1.0.1/ooze/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:28:30.119330 ooze-1.0.1/ooze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42690 2023-05-01 02:28:30.000000 ooze-1.0.1/ooze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 02:28:30.000000 ooze-1.0.1/ooze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:28:30.000000 ooze-1.0.1/ooze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 02:28:30.000000 ooze-1.0.1/ooze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 02:28:30.000000 ooze-1.0.1/ooze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-01 02:27:59.000000 ooze-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-01 02:28:30.119330 ooze-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 02:27:59.000000 ooze-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:28:30.119330 ooze-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-01 02:27:59.000000 ooze-1.0.1/tests/test_ooze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 02:27:59.000000 ooze-1.0.1/tests/test_pool.py
```

### Comparing `ooze-1.0.0/LICENSE` & `ooze-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ooze-1.0.0/PKG-INFO` & `ooze-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooze
-Version: 1.0.0
+Version: 1.0.1
 Summary: Brain-dead simple dependency injection
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,19 +663,24 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/brettschneider/ooze
 Project-URL: Bug Tracker, https://github.com/brettschneider/ooze/issues
-Project-URL: Documentation, https://github.com/brettschneider/ooze/blob/main/docs/en/index.rst
-Classifier: Programming Language :: Python :: 3
+Project-URL: Documentation, https://ooze.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Bottle
+Classifier: Framework :: FastAPI
+Classifier: Framework :: Flask
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OOZE - Brain-dead simple dependency injection #
 
 Ooze is an attempt to do depdency injection in Python in the simplest
@@ -736,9 +741,9 @@
 * factories
 * automatic environment variable injection
 * automatic configuration file parsing and settings injection
 * automatic (magic) integration with manually passed arguments
 * seamless integration with [bottlepy](https://bottlepy.org/)
 * injectable object pools (i.e. Database connection pools)
  
-Be sure to check out the [documentation](https://github.com/brettschneider/ooze/blob/main/docs/en/index.rst)
+Be sure to check out the [documentation](https://github.com/brettschneider/ooze/blob/main/docs/index.rst)
 or [examples](https://github.com/brettschneider/ooze/tree/main/examples) for more information.
```

### Comparing `ooze-1.0.0/README.md` & `ooze-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,9 @@
 * factories
 * automatic environment variable injection
 * automatic configuration file parsing and settings injection
 * automatic (magic) integration with manually passed arguments
 * seamless integration with [bottlepy](https://bottlepy.org/)
 * injectable object pools (i.e. Database connection pools)
  
-Be sure to check out the [documentation](https://github.com/brettschneider/ooze/blob/main/docs/en/index.rst)
+Be sure to check out the [documentation](https://github.com/brettschneider/ooze/blob/main/docs/index.rst)
 or [examples](https://github.com/brettschneider/ooze/tree/main/examples) for more information.
```

### Comparing `ooze-1.0.0/ooze/__init__.py` & `ooze-1.0.1/ooze/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,14 +204,36 @@
             else:
                 ooze_kwargs[key] = resolve(key)
         return func(*[], **ooze_kwargs)
 
     return wrapper
 
 
+def magic_dependable(func):
+    """A decorator that bridges a FastAPI Dependable with Ooze"""
+
+    def get_args():
+        needed_args = inspect.signature(func)
+        kwargs = {}
+        for idx, key in enumerate(needed_args.parameters.keys()):
+            kwargs[key] = resolve(key)
+        return kwargs
+
+    def wrapper():
+        ooze_kwargs = get_args()
+        return func(**ooze_kwargs)
+
+    async def async_wrapper():
+        ooze_kwargs = get_args()
+
+        return await func(**ooze_kwargs)
+
+    return async_wrapper if inspect.iscoroutinefunction(func) else wrapper
+
+
 class OozeBottlePlugin:
     api = 2
 
     def apply(self, callback, _):
         args = inspect.signature(callback)
         dependencies = {}
```

### Comparing `ooze-1.0.0/ooze/pool.py` & `ooze-1.0.1/ooze/pool.py`

 * *Files identical despite different names*

### Comparing `ooze-1.0.0/ooze.egg-info/PKG-INFO` & `ooze-1.0.1/ooze.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooze
-Version: 1.0.0
+Version: 1.0.1
 Summary: Brain-dead simple dependency injection
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,19 +663,24 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/brettschneider/ooze
 Project-URL: Bug Tracker, https://github.com/brettschneider/ooze/issues
-Project-URL: Documentation, https://github.com/brettschneider/ooze/blob/main/docs/en/index.rst
-Classifier: Programming Language :: Python :: 3
+Project-URL: Documentation, https://ooze.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Bottle
+Classifier: Framework :: FastAPI
+Classifier: Framework :: Flask
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OOZE - Brain-dead simple dependency injection #
 
 Ooze is an attempt to do depdency injection in Python in the simplest
@@ -736,9 +741,9 @@
 * factories
 * automatic environment variable injection
 * automatic configuration file parsing and settings injection
 * automatic (magic) integration with manually passed arguments
 * seamless integration with [bottlepy](https://bottlepy.org/)
 * injectable object pools (i.e. Database connection pools)
  
-Be sure to check out the [documentation](https://github.com/brettschneider/ooze/blob/main/docs/en/index.rst)
+Be sure to check out the [documentation](https://github.com/brettschneider/ooze/blob/main/docs/index.rst)
 or [examples](https://github.com/brettschneider/ooze/tree/main/examples) for more information.
```

### Comparing `ooze-1.0.0/tests/test_ooze.py` & `ooze-1.0.1/tests/test_ooze.py`

 * *Files identical despite different names*

### Comparing `ooze-1.0.0/tests/test_pool.py` & `ooze-1.0.1/tests/test_pool.py`

 * *Files identical despite different names*

