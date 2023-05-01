# Comparing `tmp/reddit_edgecontext-1.6.2.tar.gz` & `tmp/reddit_edgecontext-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_edgecontext-1.6.2.tar", last modified: Tue Jul 12 15:42:23 2022, max compression
+gzip compressed data, was "reddit_edgecontext-1.6.3.tar", last modified: Fri Feb  3 23:32:27 2023, max compression
```

## Comparing `reddit_edgecontext-1.6.2.tar` & `reddit_edgecontext-1.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:42:23.560402 reddit_edgecontext-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-07-12 15:42:23.560402 reddit_edgecontext-1.6.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:42:23.556402 reddit_edgecontext-1.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:42:23.556402 reddit_edgecontext-1.6.2/reddit_edgecontext/
--rw-r--r--   0 runner    (1001) docker     (121)    21526 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/reddit_edgecontext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/reddit_edgecontext/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:42:23.560402 reddit_edgecontext-1.6.2/reddit_edgecontext/thrift/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/reddit_edgecontext/thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/reddit_edgecontext/thrift/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    28317 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/reddit_edgecontext/thrift/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:42:23.560402 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-07-12 15:42:23.000000 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-07-12 15:42:23.000000 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 15:42:23.000000 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-12 15:42:23.000000 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-12 15:42:23.000000 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 15:42:23.000000 reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-07-12 15:42:23.560402 reddit_edgecontext-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:42:23.560402 reddit_edgecontext-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    15959 2022-07-12 15:42:11.000000 reddit_edgecontext-1.6.2/tests/edge_context_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/reddit_edgecontext/
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28317 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 23:32:27.000000 reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-03 23:32:27.795765 reddit_edgecontext-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 23:32:27.791765 reddit_edgecontext-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-02-03 23:32:13.000000 reddit_edgecontext-1.6.3/tests/edge_context_tests.py
```

### Comparing `reddit_edgecontext-1.6.2/Makefile` & `reddit_edgecontext-1.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/PKG-INFO` & `reddit_edgecontext-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_edgecontext
-Version: 1.6.2
+Version: 1.6.3
 Summary: reddit edge request context baggage
 Home-page: https://github.com/reddit/edgecontext
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-edgecontext.readthedocs.io/
 Description: # edgecontext
```

### Comparing `reddit_edgecontext-1.6.2/docs/conf.py` & `reddit_edgecontext-1.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/docs/index.rst` & `reddit_edgecontext-1.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/reddit_edgecontext/__init__.py` & `reddit_edgecontext-1.6.3/reddit_edgecontext/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/reddit_edgecontext/thrift/ttypes.py` & `reddit_edgecontext-1.6.3/reddit_edgecontext/thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/PKG-INFO` & `reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-edgecontext
-Version: 1.6.2
+Version: 1.6.3
 Summary: reddit edge request context baggage
 Home-page: https://github.com/reddit/edgecontext
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-edgecontext.readthedocs.io/
 Description: # edgecontext
```

### Comparing `reddit_edgecontext-1.6.2/reddit_edgecontext.egg-info/SOURCES.txt` & `reddit_edgecontext-1.6.3/reddit_edgecontext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/requirements-transitive.txt` & `reddit_edgecontext-1.6.3/requirements-transitive.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 gevent==21.1.2
 greenlet==1.0.0
 idna==2.10
 imagesize==1.2.0
 iniconfig==1.1.1
 Jinja2==2.11.3
 MarkupSafe==1.1.1
-mccabe==0.6.1
+mccabe==0.7.0
 mypy-extensions==0.4.3
 packaging==20.9
 pathspec==0.8.1
 pluggy==0.13.1
 posix-ipc==1.0.5
 py==1.10.0
-pycodestyle==2.6.0
+pycodestyle==2.9.1
 pycparser==2.20
-pyflakes==2.2.0
+pyflakes==2.5.0
 Pygments==2.7.4
 pyparsing==2.4.7
 python-json-logger==2.0.1
 pytz==2021.1
 regex==2020.11.13
 requests==2.25.1
 six==1.15.0
```

### Comparing `reddit_edgecontext-1.6.2/setup.cfg` & `reddit_edgecontext-1.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `reddit_edgecontext-1.6.2/setup.py` & `reddit_edgecontext-1.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     packages=find_packages(),
     python_requires=">=3.7",
     setup_requires=["setuptools_scm"],
     install_requires=[
         "baseplate>=1.5,<3.0",
         "pyjwt>=2.0.0,<3.0",
         "thrift-unofficial>=0.14,<1.0",
-        "cryptography>=3.0,<4.0",
+        "cryptography>=3.0",
     ],
     package_data={"reddit_edgecontext": ["py.typed"]},
     zip_safe=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX :: Linux",
```

### Comparing `reddit_edgecontext-1.6.2/tests/edge_context_tests.py` & `reddit_edgecontext-1.6.3/tests/edge_context_tests.py`

 * *Files identical despite different names*

