# Comparing `tmp/mitm-1.4.3.tar.gz` & `tmp/mitm-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitm-1.4.3.tar", last modified: Sat Apr 29 16:11:24 2023, max compression
+gzip compressed data, was "mitm-1.5.0.tar", last modified: Mon May  1 00:11:37 2023, max compression
```

## Comparing `mitm-1.4.3.tar` & `mitm-1.5.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.114853 mitm-1.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-29 16:11:09.000000 mitm-1.4.3/.github/workflows/docs-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 16:11:09.000000 mitm-1.4.3/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-29 16:11:09.000000 mitm-1.4.3/.github/workflows/pytest-cover-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 16:11:09.000000 mitm-1.4.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 16:11:24.000000 mitm-1.4.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 16:11:24.000000 mitm-1.4.3/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 16:11:09.000000 mitm-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-29 16:11:24.118852 mitm-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-29 16:11:09.000000 mitm-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/docs/internals.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/docs/trusting-mitm.rst
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/introduction/
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/introduction/how-mitm-works.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/introduction/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/crypto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-29 16:11:09.000000 mitm-1.4.3/docs/source/module/mitm.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/mitm/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/mitm/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/extension/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/extension/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-04-29 16:11:09.000000 mitm-1.4.3/mitm/mitm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/mitm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:11:19.000000 mitm-1.4.3/mitm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 16:11:24.000000 mitm-1.4.3/mitm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 16:11:09.000000 mitm-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-29 16:11:09.000000 mitm-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 16:11:24.122852 mitm-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 16:11:09.000000 mitm-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:24.118852 mitm-1.4.3/tests/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/extension/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/extension/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-29 16:11:09.000000 mitm-1.4.3/tests/test_mitm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.586891 mitm-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-01 00:11:12.000000 mitm-1.5.0/.github/workflows/docs-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-01 00:11:12.000000 mitm-1.5.0/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-01 00:11:12.000000 mitm-1.5.0/.github/workflows/pytest-cover-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 00:11:12.000000 mitm-1.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-01 00:11:37.000000 mitm-1.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 00:11:37.000000 mitm-1.5.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 00:11:12.000000 mitm-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-01 00:11:37.590891 mitm-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-01 00:11:12.000000 mitm-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/docs/source/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/docs/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/docs/trusting-mitm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/docs/source/introduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/introduction/how-mitm-works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/introduction/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/module/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/module/crypto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/module/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 00:11:12.000000 mitm-1.5.0/docs/source/module/mitm.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/mitm/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/mitm/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/extension/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/extension/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-05-01 00:11:12.000000 mitm-1.5.0/mitm/mitm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/mitm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-01 00:11:37.000000 mitm-1.5.0/mitm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-01 00:11:37.000000 mitm-1.5.0/mitm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:11:37.000000 mitm-1.5.0/mitm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:11:31.000000 mitm-1.5.0/mitm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 00:11:37.000000 mitm-1.5.0/mitm.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 00:11:37.000000 mitm-1.5.0/mitm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 00:11:37.000000 mitm-1.5.0/mitm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 00:11:12.000000 mitm-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 00:11:12.000000 mitm-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 00:11:37.594891 mitm-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-01 00:11:12.000000 mitm-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:37.590891 mitm-1.5.0/tests/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/extension/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/extension/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-01 00:11:12.000000 mitm-1.5.0/tests/test_mitm.py
```

### Comparing `mitm-1.4.3/.github/workflows/docs-publish.yaml` & `mitm-1.5.0/.github/workflows/docs-publish.yaml`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/.github/workflows/pypi-publish.yaml` & `mitm-1.5.0/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/.github/workflows/pytest-cover-run.yaml` & `mitm-1.5.0/.github/workflows/pytest-cover-run.yaml`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/LICENSE` & `mitm-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/PKG-INFO` & `mitm-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitm
-Version: 1.4.3
+Version: 1.5.0
 Summary: Man-in-the-middle proxy with customizable options.
 Home-page: https://github.com/synchronizing/mitm
 Author: Felipe Faria
 Author-email: felipefaria@me.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues
 Project-URL: Documentation, https://synchronizing.github.io/mitm/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitm Version: 1.4.3 Summary: Man-in-the-middle
+Metadata-Version: 2.1 Name: mitm Version: 1.5.0 Summary: Man-in-the-middle
 proxy with customizable options. Home-page: https://github.com/synchronizing/
 mitm Author: Felipe Faria Author-email: felipefaria@me.com License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues Project-
 URL: Documentation, https://synchronizing.github.io/mitm/ Project-URL: Source
 Code, https://github.com/synchronizing/mitm/tree/master Keywords: mitm
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

### Comparing `mitm-1.4.3/README.md` & `mitm-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/Makefile` & `mitm-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/make.bat` & `mitm-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/source/conf.py` & `mitm-1.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/source/docs/internals.rst` & `mitm-1.5.0/docs/source/docs/internals.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/source/docs/trusting-mitm.rst` & `mitm-1.5.0/docs/source/docs/trusting-mitm.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/source/introduction/how-mitm-works.rst` & `mitm-1.5.0/docs/source/introduction/how-mitm-works.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/source/introduction/quickstart.rst` & `mitm-1.5.0/docs/source/introduction/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/docs/source/module/mitm.rst` & `mitm-1.5.0/docs/source/module/mitm.rst`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm/__init__.py` & `mitm-1.5.0/mitm/__init__.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm/core.py` & `mitm-1.5.0/mitm/core.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm/crypto.py` & `mitm-1.5.0/mitm/crypto.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm/extension/middleware.py` & `mitm-1.5.0/mitm/extension/middleware.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm/extension/protocol.py` & `mitm-1.5.0/mitm/extension/protocol.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm/mitm.py` & `mitm-1.5.0/mitm/mitm.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/mitm.egg-info/PKG-INFO` & `mitm-1.5.0/mitm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitm
-Version: 1.4.3
+Version: 1.5.0
 Summary: Man-in-the-middle proxy with customizable options.
 Home-page: https://github.com/synchronizing/mitm
 Author: Felipe Faria
 Author-email: felipefaria@me.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues
 Project-URL: Documentation, https://synchronizing.github.io/mitm/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitm Version: 1.4.3 Summary: Man-in-the-middle
+Metadata-Version: 2.1 Name: mitm Version: 1.5.0 Summary: Man-in-the-middle
 proxy with customizable options. Home-page: https://github.com/synchronizing/
 mitm Author: Felipe Faria Author-email: felipefaria@me.com License: MIT
 Project-URL: Bug Tracker, https://github.com/synchronizing/mitm/issues Project-
 URL: Documentation, https://synchronizing.github.io/mitm/ Project-URL: Source
 Code, https://github.com/synchronizing/mitm/tree/master Keywords: mitm
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

### Comparing `mitm-1.4.3/mitm.egg-info/SOURCES.txt` & `mitm-1.5.0/mitm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/setup.cfg` & `mitm-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/tests/conftest.py` & `mitm-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/tests/extension/test_middleware.py` & `mitm-1.5.0/tests/extension/test_middleware.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/tests/extension/test_protocol.py` & `mitm-1.5.0/tests/extension/test_protocol.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/tests/test_core.py` & `mitm-1.5.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/tests/test_crypto.py` & `mitm-1.5.0/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `mitm-1.4.3/tests/test_mitm.py` & `mitm-1.5.0/tests/test_mitm.py`

 * *Files identical despite different names*

