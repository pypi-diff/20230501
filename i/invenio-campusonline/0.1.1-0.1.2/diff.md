# Comparing `tmp/invenio-campusonline-0.1.1.tar.gz` & `tmp/invenio-campusonline-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-campusonline-0.1.1.tar", last modified: Wed Jan 11 12:33:18 2023, max compression
+gzip compressed data, was "invenio-campusonline-0.1.2.tar", last modified: Mon May  1 20:21:04 2023, max compression
```

## Comparing `invenio-campusonline-0.1.1.tar` & `invenio-campusonline-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.199985 invenio-campusonline-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.187984 invenio-campusonline-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.195984 invenio-campusonline-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.195984 invenio-campusonline-0.1.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-01-11 12:33:18.199985 invenio-campusonline-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.195984 invenio-campusonline-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.195984 invenio-campusonline-0.1.1/invenio_campusonline/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/invenio_campusonline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.195984 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-11 12:33:18.000000 invenio-campusonline-0.1.1/invenio_campusonline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-11 12:33:18.199985 invenio-campusonline-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:33:18.199985 invenio-campusonline-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/tests/test_invenio_campusonline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-01-11 12:33:13.000000 invenio-campusonline-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.241347 invenio-campusonline-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.245348 invenio-campusonline-0.1.2/invenio_campusonline/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/invenio_campusonline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 20:21:04.000000 invenio-campusonline-0.1.2/invenio_campusonline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:21:04.249348 invenio-campusonline-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/tests/test_invenio_campusonline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-01 20:20:57.000000 invenio-campusonline-0.1.2/tests/test_utils.py
```

### Comparing `invenio-campusonline-0.1.1/.editorconfig` & `invenio-campusonline-0.1.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/.github/workflows/tests.yml` & `invenio-campusonline-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/.tx/config` & `invenio-campusonline-0.1.2/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/CONTRIBUTING.rst` & `invenio-campusonline-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/LICENSE` & `invenio-campusonline-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/MANIFEST.in` & `invenio-campusonline-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/PKG-INFO` & `invenio-campusonline-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-campusonline
-Version: 0.1.1
+Version: 0.1.2
 Summary: "This module is used to import/export from/to the CampusOnline System."
 Home-page: https://github.com/tu-graz-library/invenio-campusonline
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio TODO
 Platform: any
@@ -53,14 +53,19 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.2 (release 2023-05-01)
+
+- cli: move to secho way from logger
+
+
 Version v0.1.1 (release 2023-01-11)
 
 - setup: remove python3.8 add python3.11 support
 - setup: remove translation config
 
 
 Version v0.1.0 (release 2023-01-11)
```

### Comparing `invenio-campusonline-0.1.1/README.rst` & `invenio-campusonline-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/babel.ini` & `invenio-campusonline-0.1.2/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/docs/Makefile` & `invenio-campusonline-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/docs/conf.py` & `invenio-campusonline-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/docs/index.rst` & `invenio-campusonline-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/docs/make.bat` & `invenio-campusonline-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/__init__.py` & `invenio-campusonline-0.1.2/invenio_campusonline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """This module is used to import/export from/to the CampusOnline System."""
 
 from .api import fetch_all_ids, import_from_campusonline
 from .ext import InvenioCampusonline
 from .types import ThesesFilter, ThesesState
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __all__ = (
     "__version__",
     "InvenioCampusonline",
     "import_from_campusonline",
     "fetch_all_ids",
     "ThesesFilter",
```

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/api.py` & `invenio-campusonline-0.1.2/invenio_campusonline/api.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/cli.py` & `invenio-campusonline-0.1.2/invenio_campusonline/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-campusonline is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Command line interface to interact with the CampusOnline-Connector module."""
 
 
-import click
+from click import STRING, group, option, secho
 from click_params import URL
 from flask import current_app
 from flask.cli import with_appcontext
 
 from .api import fetch_all_ids, import_from_campusonline
-from .types import CampusOnlineConfigs
+from .types import CampusOnlineConfigs, Color
 
 
-@click.group()
+@group()
 def campusonline():
     """Campusonline CLI."""
 
 
 @campusonline.command()
 @with_appcontext
-@click.option("--endpoint", type=URL)
-@click.option("--campusonline-id", type=click.STRING)
-@click.option("--token", type=click.STRING)
-@click.option("--user-email", type=click.STRING, default="cms@tugraz.at")
-def import_thesis(endpoint, campusonline_id, token, user_email):
+@option("--endpoint", type=URL)
+@option("--campusonline-id", type=STRING)
+@option("--token", type=STRING)
+@option("--user-email", type=STRING, default="cms@tugraz.at")
+@option("--no-color", is_flag=True)
+def import_thesis(endpoint, campusonline_id, token, user_email, no_color=False):
     """Import metadata and file (aka one thesis) from campusonline."""
     import_func = current_app.config["CAMPUSONLINE_IMPORT_FUNC"]
     theses_filters = current_app.config["CAMPUSONLINE_THESES_FILTERS"]
     recipients = current_app.config["CAMPUSONLINE_ERROR_MAIL_RECIPIENTS"]
     sender = current_app.config["CAMPUSONLINE_ERROR_MAIL_SENDER"]
 
     configs = CampusOnlineConfigs(
         endpoint, token, user_email, theses_filters, recipients, sender
     )
     record = import_from_campusonline(import_func, campusonline_id, configs)
 
-    current_app.logger.info(f"record.id: {record.id}")
+    color = Color.success if not no_color else Color.neutral
+    secho(f"record.id: {record.id}", fg=color)
 
 
 @campusonline.command()
 @with_appcontext
-@click.option("--endpoint", type=URL)
-@click.option("--token", type=click.STRING)
-def fetch_ids(endpoint, token):
+@option("--endpoint", type=URL)
+@option("--token", type=STRING)
+@option("--no-color", is_flag=True)
+def fetch_ids(endpoint, token, no_color):
     """Fetch all to import ids."""
     theses_filters = current_app.config["CAMPUSONLINE_THESES_FILTERS"]
     ids = fetch_all_ids(endpoint, token, theses_filters)
 
-    current_app.logger.info(ids)
+    color = Color.success if not no_color else Color.neutral
+    secho(f"ids: {ids}", fg=color)
```

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/config.py` & `invenio-campusonline-0.1.2/invenio_campusonline/config.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/ext.py` & `invenio-campusonline-0.1.2/invenio_campusonline/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/tasks.py` & `invenio-campusonline-0.1.2/invenio_campusonline/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/types.py` & `invenio-campusonline-0.1.2/invenio_campusonline/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,26 @@
 EmailAddress = str
 """The email address.
 
 The address does not have to have a special format, but it has to be an email.
 """
 
 
+@dataclass(frozen=True)
+class Color:
+    """This class is for the output color management."""
+
+    neutral = "black"
+    error = "red"
+    warning = "yellow"
+    abort = "magenta"
+    success = "green"
+    alternate = ["blue", "cyan"]
+
+
 class ThesesState(Enum):
     """Theses State class."""
 
     LOCKED = 1
     OPEN = 2
```

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline/utils.py` & `invenio-campusonline-0.1.2/invenio_campusonline/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline.egg-info/PKG-INFO` & `invenio-campusonline-0.1.2/invenio_campusonline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-campusonline
-Version: 0.1.1
+Version: 0.1.2
 Summary: "This module is used to import/export from/to the CampusOnline System."
 Home-page: https://github.com/tu-graz-library/invenio-campusonline
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio TODO
 Platform: any
@@ -53,14 +53,19 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.1.2 (release 2023-05-01)
+
+- cli: move to secho way from logger
+
+
 Version v0.1.1 (release 2023-01-11)
 
 - setup: remove python3.8 add python3.11 support
 - setup: remove translation config
 
 
 Version v0.1.0 (release 2023-01-11)
```

### Comparing `invenio-campusonline-0.1.1/invenio_campusonline.egg-info/SOURCES.txt` & `invenio-campusonline-0.1.2/invenio_campusonline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/setup.cfg` & `invenio-campusonline-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/tests/conftest.py` & `invenio-campusonline-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/tests/test_invenio_campusonline.py` & `invenio-campusonline-0.1.2/tests/test_invenio_campusonline.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.1.1/tests/test_utils.py` & `invenio-campusonline-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

