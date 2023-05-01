# Comparing `tmp/valr-py-0.3.0.tar.gz` & `tmp/valr-py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valr-py-0.3.0.tar", last modified: Mon May  1 12:58:32 2023, max compression
+gzip compressed data, was "valr-py-0.3.1.tar", last modified: Mon May  1 20:04:16 2023, max compression
```

## Comparing `valr-py-0.3.0.tar` & `valr-py-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.028444 valr-py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-01 12:58:20.000000 valr-py-0.3.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-01 12:58:20.000000 valr-py-0.3.0/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-01 12:58:20.000000 valr-py-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-01 12:58:20.000000 valr-py-0.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 12:58:20.000000 valr-py-0.3.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-01 12:58:20.000000 valr-py-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-01 12:58:20.000000 valr-py-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-01 12:58:20.000000 valr-py-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 12:58:20.000000 valr-py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 12:58:20.000000 valr-py-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-01 12:58:32.028444 valr-py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-01 12:58:20.000000 valr-py-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.024444 valr-py-0.3.0/ci/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2885 2023-05-01 12:58:20.000000 valr-py-0.3.0/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 12:58:20.000000 valr-py-0.3.0/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.024444 valr-py-0.3.0/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-01 12:58:20.000000 valr-py-0.3.0/ci/templates/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-01 12:58:32.028444 valr-py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 12:58:20.000000 valr-py-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.020444 valr-py-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.024444 valr-py-0.3.0/src/valr_py/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58158 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/rest_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-05-01 12:58:20.000000 valr-py-0.3.0/src/valr_py/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.028444 valr-py-0.3.0/src/valr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-01 12:58:32.000000 valr-py-0.3.0/src/valr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-01 12:58:32.000000 valr-py-0.3.0/src/valr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:58:32.000000 valr-py-0.3.0/src/valr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:58:31.000000 valr-py-0.3.0/src/valr_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 12:58:32.000000 valr-py-0.3.0/src/valr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 12:58:32.000000 valr-py-0.3.0/src/valr_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.028444 valr-py-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.028444 valr-py-0.3.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (123)    34631 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/func/test_rest_sync_client_private_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/func/test_rest_sync_client_public_apis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.028444 valr-py-0.3.0/tests/integration_public/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/integration_public/test_rest_sync_client_live_public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:32.028444 valr-py-0.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/unit/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/unit/test_request_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/unit/test_rest_sync_client_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:58:20.000000 valr-py-0.3.0/tests/unit/test_ws_client_basic
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-01 12:58:20.000000 valr-py-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-01 20:04:04.000000 valr-py-0.3.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-01 20:04:04.000000 valr-py-0.3.1/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-01 20:04:04.000000 valr-py-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-01 20:04:04.000000 valr-py-0.3.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 20:04:04.000000 valr-py-0.3.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-01 20:04:04.000000 valr-py-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-01 20:04:04.000000 valr-py-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-01 20:04:04.000000 valr-py-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 20:04:04.000000 valr-py-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 20:04:04.000000 valr-py-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-01 20:04:16.440989 valr-py-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-01 20:04:04.000000 valr-py-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.436989 valr-py-0.3.1/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2885 2023-05-01 20:04:04.000000 valr-py-0.3.1/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 20:04:04.000000 valr-py-0.3.1/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-01 20:04:04.000000 valr-py-0.3.1/ci/templates/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-01 20:04:16.440989 valr-py-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 20:04:04.000000 valr-py-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.436989 valr-py-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/src/valr_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58158 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/rest_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-05-01 20:04:04.000000 valr-py-0.3.1/src/valr_py/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/src/valr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-01 20:04:16.000000 valr-py-0.3.1/src/valr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-01 20:04:16.000000 valr-py-0.3.1/src/valr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:04:16.000000 valr-py-0.3.1/src/valr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:04:16.000000 valr-py-0.3.1/src/valr_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 20:04:16.000000 valr-py-0.3.1/src/valr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 20:04:16.000000 valr-py-0.3.1/src/valr_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)    34631 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/func/test_rest_sync_client_private_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/func/test_rest_sync_client_public_apis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/tests/integration_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/integration_public/test_rest_sync_client_live_public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:16.440989 valr-py-0.3.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/unit/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/unit/test_request_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/unit/test_rest_sync_client_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:04:04.000000 valr-py-0.3.1/tests/unit/test_ws_client_basic
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-01 20:04:04.000000 valr-py-0.3.1/tox.ini
```

### Comparing `valr-py-0.3.0/.cookiecutterrc` & `valr-py-0.3.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/.travis.yml` & `valr-py-0.3.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/CHANGELOG.rst` & `valr-py-0.3.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/CONTRIBUTING.rst` & `valr-py-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/LICENSE` & `valr-py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/PKG-INFO` & `valr-py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valr-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for the VALR REST API
 Home-page: https://github.com/Quirky-Fox/valr-py
 Author: Jonathan Els
 Author-email: jonathanelscpt@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/jonathanelscpt/valr-python/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/jonathanelscpt/valr-python/issues
@@ -37,19 +37,19 @@
 
 
 Installation
 ============
 
 ::
 
-    pip install valr-python
+    pip install valr-py
 
 You can also install the in-development version with::
 
-    pip install https://github.com/jonathanelscpt/valr-python/archive/master.zip
+    pip install https://github.com/Quirky-Fox/valr-py/archive/master.zip
 
 
 
 Authentication
 ==============
 
 Authenticating to VALR API private resources requires a valid API Key from the `VALR exchange <https://www.valr.com/>`_.
@@ -59,16 +59,16 @@
 ===========================
 
 
 To use the **synchronous** REST API client:
 
 .. code-block:: python
 
-    >>> from valr_python import Client
-    >>> from valr_python.exceptions import IncompleteOrderWarning
+    >>> from valr_py import Client
+    >>> from valr_py.exceptions import IncompleteOrderWarning
     >>> from decimal import Decimal
     >>>
     >>> c = Client(api_key='api_key', api_secret='api_secret')
     >>> c.rate_limiting_support = True # honour HTTP 429 "Retry-After" header values
     >>> limit_order = {
     ...     "side": "SELL",
     ...     "quantity": Decimal('0.1'),
@@ -101,17 +101,17 @@
 
 
 .. code-block:: python
 
     >>> import asyncio
     >>> from typing import Dict
     >>> from pprint import pprint
-    >>> from valr_python import WebSocketClient
-    >>> from valr_python.enum import TradeEvent
-    >>> from valr_python.enum import WebSocketType
+    >>> from valr_py import WebSocketClient
+    >>> from valr_py.enum import TradeEvent
+    >>> from valr_py.enum import WebSocketType
     >>>
     >>> def pretty_hook(data: Dict):
     ...    pprint(data)
     >>>
     >>> c = WebSocketClient(api_key='api_key', api_secret='api_secret', currency_pairs=['BTCZAR'],
     ...                     ws_type=WebSocketType.TRADE.name,
     ...                     trade_subscriptions=[TradeEvent.MARKET_SUMMARY_UPDATE.name],
```

### Comparing `valr-py-0.3.0/README.rst` & `valr-py-0.3.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -61,19 +61,19 @@
 
 
 Installation
 ============
 
 ::
 
-    pip install valr-python
+    pip install valr-py
 
 You can also install the in-development version with::
 
-    pip install https://github.com/jonathanelscpt/valr-python/archive/master.zip
+    pip install https://github.com/Quirky-Fox/valr-py/archive/master.zip
 
 
 
 Authentication
 ==============
 
 Authenticating to VALR API private resources requires a valid API Key from the `VALR exchange <https://www.valr.com/>`_.
@@ -83,16 +83,16 @@
 ===========================
 
 
 To use the **synchronous** REST API client:
 
 .. code-block:: python
 
-    >>> from valr_python import Client
-    >>> from valr_python.exceptions import IncompleteOrderWarning
+    >>> from valr_py import Client
+    >>> from valr_py.exceptions import IncompleteOrderWarning
     >>> from decimal import Decimal
     >>>
     >>> c = Client(api_key='api_key', api_secret='api_secret')
     >>> c.rate_limiting_support = True # honour HTTP 429 "Retry-After" header values
     >>> limit_order = {
     ...     "side": "SELL",
     ...     "quantity": Decimal('0.1'),
@@ -125,17 +125,17 @@
 
 
 .. code-block:: python
 
     >>> import asyncio
     >>> from typing import Dict
     >>> from pprint import pprint
-    >>> from valr_python import WebSocketClient
-    >>> from valr_python.enum import TradeEvent
-    >>> from valr_python.enum import WebSocketType
+    >>> from valr_py import WebSocketClient
+    >>> from valr_py.enum import TradeEvent
+    >>> from valr_py.enum import WebSocketType
     >>>
     >>> def pretty_hook(data: Dict):
     ...    pprint(data)
     >>>
     >>> c = WebSocketClient(api_key='api_key', api_secret='api_secret', currency_pairs=['BTCZAR'],
     ...                     ws_type=WebSocketType.TRADE.name,
     ...                     trade_subscriptions=[TradeEvent.MARKET_SUMMARY_UPDATE.name],
```

### Comparing `valr-py-0.3.0/ci/bootstrap.py` & `valr-py-0.3.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/ci/templates/.travis.yml` & `valr-py-0.3.1/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/setup.py` & `valr-py-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='valr-py',
-    version='0.3.0',
+    version='0.3.1',
     license='MIT',
     description='Python SDK for the VALR REST API',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
     author='Jonathan Els',
```

### Comparing `valr-py-0.3.0/src/valr_py/decorators.py` & `valr-py-0.3.1/src/valr_py/decorators.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/src/valr_py/enum.py` & `valr-py-0.3.1/src/valr_py/enum.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/src/valr_py/exceptions.py` & `valr-py-0.3.1/src/valr_py/exceptions.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/src/valr_py/rest_base.py` & `valr-py-0.3.1/src/valr_py/rest_base.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/src/valr_py/rest_client.py` & `valr-py-0.3.1/src/valr_py/rest_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,18 @@
         args = dict(timeout=self._timeout, data=data, headers=headers)
         if params_str:
             args['params'] = params_str
         res = self._session.request(method, url, **args)
 
         try:
             res.raise_for_status()
-            e = res.json()
+            try:
+                e = res.json()
+            except:
+                e = {}
             self._raise_for_api_error(e)
             # provide warning with bundled response dict for incomplete transactions
             if res.status_code == 202:
                 warnings.warn(IncompleteOrderWarning(data=e, message="Order processing incomplete"))
             return e
         except HTTPError as he:
             print(he)
```

### Comparing `valr-py-0.3.0/src/valr_py/utils.py` & `valr-py-0.3.1/src/valr_py/utils.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/src/valr_py/ws_client.py` & `valr-py-0.3.1/src/valr_py/ws_client.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/src/valr_py.egg-info/PKG-INFO` & `valr-py-0.3.1/src/valr_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valr-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for the VALR REST API
 Home-page: https://github.com/Quirky-Fox/valr-py
 Author: Jonathan Els
 Author-email: jonathanelscpt@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/jonathanelscpt/valr-python/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/jonathanelscpt/valr-python/issues
@@ -37,19 +37,19 @@
 
 
 Installation
 ============
 
 ::
 
-    pip install valr-python
+    pip install valr-py
 
 You can also install the in-development version with::
 
-    pip install https://github.com/jonathanelscpt/valr-python/archive/master.zip
+    pip install https://github.com/Quirky-Fox/valr-py/archive/master.zip
 
 
 
 Authentication
 ==============
 
 Authenticating to VALR API private resources requires a valid API Key from the `VALR exchange <https://www.valr.com/>`_.
@@ -59,16 +59,16 @@
 ===========================
 
 
 To use the **synchronous** REST API client:
 
 .. code-block:: python
 
-    >>> from valr_python import Client
-    >>> from valr_python.exceptions import IncompleteOrderWarning
+    >>> from valr_py import Client
+    >>> from valr_py.exceptions import IncompleteOrderWarning
     >>> from decimal import Decimal
     >>>
     >>> c = Client(api_key='api_key', api_secret='api_secret')
     >>> c.rate_limiting_support = True # honour HTTP 429 "Retry-After" header values
     >>> limit_order = {
     ...     "side": "SELL",
     ...     "quantity": Decimal('0.1'),
@@ -101,17 +101,17 @@
 
 
 .. code-block:: python
 
     >>> import asyncio
     >>> from typing import Dict
     >>> from pprint import pprint
-    >>> from valr_python import WebSocketClient
-    >>> from valr_python.enum import TradeEvent
-    >>> from valr_python.enum import WebSocketType
+    >>> from valr_py import WebSocketClient
+    >>> from valr_py.enum import TradeEvent
+    >>> from valr_py.enum import WebSocketType
     >>>
     >>> def pretty_hook(data: Dict):
     ...    pprint(data)
     >>>
     >>> c = WebSocketClient(api_key='api_key', api_secret='api_secret', currency_pairs=['BTCZAR'],
     ...                     ws_type=WebSocketType.TRADE.name,
     ...                     trade_subscriptions=[TradeEvent.MARKET_SUMMARY_UPDATE.name],
```

### Comparing `valr-py-0.3.0/src/valr_py.egg-info/SOURCES.txt` & `valr-py-0.3.1/src/valr_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/conftest.py` & `valr-py-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/func/test_rest_sync_client_private_apis.py` & `valr-py-0.3.1/tests/func/test_rest_sync_client_private_apis.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/func/test_rest_sync_client_public_apis.py` & `valr-py-0.3.1/tests/func/test_rest_sync_client_public_apis.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/integration_public/test_rest_sync_client_live_public_api.py` & `valr-py-0.3.1/tests/integration_public/test_rest_sync_client_live_public_api.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/unit/test_decorators.py` & `valr-py-0.3.1/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/unit/test_request_signature.py` & `valr-py-0.3.1/tests/unit/test_request_signature.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tests/unit/test_rest_sync_client_basic.py` & `valr-py-0.3.1/tests/unit/test_rest_sync_client_basic.py`

 * *Files identical despite different names*

### Comparing `valr-py-0.3.0/tox.ini` & `valr-py-0.3.1/tox.ini`

 * *Files identical despite different names*

