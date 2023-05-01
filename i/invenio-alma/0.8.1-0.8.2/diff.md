# Comparing `tmp/invenio-alma-0.8.1.tar.gz` & `tmp/invenio-alma-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.8.1.tar", last modified: Mon May  1 09:21:36 2023, max compression
+gzip compressed data, was "invenio-alma-0.8.2.tar", last modified: Mon May  1 09:39:37 2023, max compression
```

## Comparing `invenio-alma-0.8.1.tar` & `invenio-alma-0.8.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/invenio_alma/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.072981 invenio-alma-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.8.1/.editorconfig` & `invenio-alma-0.8.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/CHANGES.rst` & `invenio-alma-0.8.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.2 (release 2023-05-01)
+
+- ext: revert last change
+
+
 Version v0.8.1 (release 2023-05-01)
 
 - setup: add forgotten ruff configuration
 - ext: mock the resource and service properties
 - setup: re-add isort configuration
```

### Comparing `invenio-alma-0.8.1/CONTRIBUTING.rst` & `invenio-alma-0.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/LICENSE` & `invenio-alma-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/MANIFEST.in` & `invenio-alma-0.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/PKG-INFO` & `invenio-alma-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.8.1
+Version: 0.8.2
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.2 (release 2023-05-01)
+
+- ext: revert last change
+
+
 Version v0.8.1 (release 2023-05-01)
 
 - setup: add forgotten ruff configuration
 - ext: mock the resource and service properties
 - setup: re-add isort configuration
```

### Comparing `invenio-alma-0.8.1/README.rst` & `invenio-alma-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/docs/Makefile` & `invenio-alma-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/docs/conf.py` & `invenio-alma-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/docs/index.rst` & `invenio-alma-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/docs/make.bat` & `invenio-alma-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/api.py` & `invenio-alma-0.8.2/invenio_alma/api.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/cli.py` & `invenio-alma-0.8.2/invenio_alma/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/click_param_type.py` & `invenio-alma-0.8.2/invenio_alma/click_param_type.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/config.py` & `invenio-alma-0.8.2/invenio_alma/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/ext.py` & `invenio-alma-0.8.2/invenio_alma/ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,20 +67,19 @@
         app.extensions["invenio-alma"] = self
 
     def init_services(self, app: Flask) -> None:
         """Initialize service."""
         api_key = app.config.get("ALMA_API_KEY", "")
         api_host = app.config.get("ALMA_API_HOST", "")
 
-        if api_key and api_host:
-            self._alma_rest_service = AlmaRESTService.build(api_key, api_host)
+        self._alma_rest_service = AlmaRESTService.build(api_key, api_host)
 
     def init_resources(self, app: Flask) -> None:
         """Initialize resources."""
         search_key = "local_control_field_009"  # ac_number
         domain = app.config.get("ALMA_SRU_DOMAIN")
         institution_code = app.config.get("ALMA_SRU_INSTITUTION_CODE")
-        if domain and institution_code:
-            self._alma_resource = AlmaResource(
-                service=AlmaSRUService.build(search_key, domain, institution_code),
-                config=AlmaResourceConfig,
-            )
+
+        self._alma_resource = AlmaResource(
+            service=AlmaSRUService.build(search_key, domain, institution_code),
+            config=AlmaResourceConfig,
+        )
```

### Comparing `invenio-alma-0.8.1/invenio_alma/resources/config.py` & `invenio-alma-0.8.2/invenio_alma/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/resources/resources.py` & `invenio-alma-0.8.2/invenio_alma/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/services/base.py` & `invenio-alma-0.8.2/invenio_alma/services/base.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/services/config.py` & `invenio-alma-0.8.2/invenio_alma/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/services/errors.py` & `invenio-alma-0.8.2/invenio_alma/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/services/rest.py` & `invenio-alma-0.8.2/invenio_alma/services/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/services/sru.py` & `invenio-alma-0.8.2/invenio_alma/services/sru.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/tasks.py` & `invenio-alma-0.8.2/invenio_alma/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/utils.py` & `invenio-alma-0.8.2/invenio_alma/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma/views.py` & `invenio-alma-0.8.2/invenio_alma/views.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.8.2/invenio_alma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.8.1
+Version: 0.8.2
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.2 (release 2023-05-01)
+
+- ext: revert last change
+
+
 Version v0.8.1 (release 2023-05-01)
 
 - setup: add forgotten ruff configuration
 - ext: mock the resource and service properties
 - setup: re-add isort configuration
```

### Comparing `invenio-alma-0.8.1/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.8.2/invenio_alma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/run-tests.sh` & `invenio-alma-0.8.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/setup.cfg` & `invenio-alma-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/tests/conftest.py` & `invenio-alma-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/tests/test_invenio_alma.py` & `invenio-alma-0.8.2/tests/test_invenio_alma.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.1/tests/test_invenio_alma_service.py` & `invenio-alma-0.8.2/tests/test_invenio_alma_service.py`

 * *Files identical despite different names*

