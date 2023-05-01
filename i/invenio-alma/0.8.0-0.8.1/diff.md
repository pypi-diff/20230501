# Comparing `tmp/invenio-alma-0.8.0.tar.gz` & `tmp/invenio-alma-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.8.0.tar", last modified: Sat Apr 29 20:29:04 2023, max compression
+gzip compressed data, was "invenio-alma-0.8.1.tar", last modified: Mon May  1 09:21:36 2023, max compression
```

## Comparing `invenio-alma-0.8.0.tar` & `invenio-alma-0.8.1.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.974420 invenio-alma-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.974420 invenio-alma-0.8.0/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/invenio_alma/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/invenio_alma/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 20:29:04.000000 invenio-alma-0.8.0/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:29:04.978420 invenio-alma-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 20:28:55.000000 invenio-alma-0.8.0/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.841332 invenio-alma-0.8.1/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 09:21:36.000000 invenio-alma-0.8.1/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:21:36.845332 invenio-alma-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-01 09:21:26.000000 invenio-alma-0.8.1/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.8.0/.editorconfig` & `invenio-alma-0.8.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/CHANGES.rst` & `invenio-alma-0.8.1/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-05-01)
+
+- setup: add forgotten ruff configuration
+- ext: mock the resource and service properties
+- setup: re-add isort configuration
+
+
 Version v0.8.0 (release 2023-04-29)
 
 - ext: add existence check before resource creation
 - global: use ruff instead of pylint
 - global: add services to export
 - tasks: add option to use update func
 - sru: add search_key on the search
```

### Comparing `invenio-alma-0.8.0/CONTRIBUTING.rst` & `invenio-alma-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/LICENSE` & `invenio-alma-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/MANIFEST.in` & `invenio-alma-0.8.1/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 include .dockerignore
 include .editorconfig
+include .ruff.toml
 include *.rst
 include *.sh
 include *.txt
 prune docs/_build
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
```

### Comparing `invenio-alma-0.8.0/PKG-INFO` & `invenio-alma-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.8.0
+Version: 0.8.1
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,21 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-05-01)
+
+- setup: add forgotten ruff configuration
+- ext: mock the resource and service properties
+- setup: re-add isort configuration
+
+
 Version v0.8.0 (release 2023-04-29)
 
 - ext: add existence check before resource creation
 - global: use ruff instead of pylint
 - global: add services to export
 - tasks: add option to use update func
 - sru: add search_key on the search
```

### Comparing `invenio-alma-0.8.0/README.rst` & `invenio-alma-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/docs/Makefile` & `invenio-alma-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/docs/conf.py` & `invenio-alma-0.8.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,22 @@
 from invenio_alma import __version__
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
-nitpick_ignore = [("py:class", "Flask")]
+nitpick_ignore = [
+    ("py:class", "Flask"),
+    ("py:class", "flask.blueprints.Blueprint"),
+    ("py:class", "invenio_alma.resources.resources.AlmaResource"),
+    ("py:class", "invenio_alma.services.rest.AlmaRESTService"),
+    ("py:class", "AlmaResource"),
+    ("py:class", "AlmaResourceMock"),
+]
 
 
 # Do not warn on external images.
 suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `invenio-alma-0.8.0/docs/index.rst` & `invenio-alma-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/docs/make.bat` & `invenio-alma-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/api.py` & `invenio-alma-0.8.1/invenio_alma/api.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/cli.py` & `invenio-alma-0.8.1/invenio_alma/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/click_param_type.py` & `invenio-alma-0.8.1/invenio_alma/click_param_type.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/config.py` & `invenio-alma-0.8.1/invenio_alma/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/ext.py` & `invenio-alma-0.8.1/invenio_alma/ext.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,43 +10,77 @@
 from __future__ import annotations
 
 import typing as t
 
 if t.TYPE_CHECKING:
     from flask import Flask
 
+from dataclasses import dataclass
+
+from flask import Blueprint, current_app
+
 from .resources import AlmaResource, AlmaResourceConfig
 from .services import AlmaRESTService, AlmaSRUService
 
 
+@dataclass(frozen=True)
+class AlmaResourceMock:
+    """Alma Resource Mock class. It is used if the alma resource is not initialized."""
+
+    def as_blueprint(self) -> Blueprint:
+        """Return a mocked Blueprint object."""
+        return Blueprint("AlmaResourceMockBlueprint", __name__)
+
+
 class InvenioAlma:
     """invenio-alma extension."""
 
     def __init__(self, app: Flask = None) -> None:
         """Extension initialization."""
+        self._alma_rest_service = None
+        self._alma_resource = None
+
         if app:
             self.init_app(app)
 
+    @property
+    def alma_rest_service(self) -> AlmaRESTService:
+        """Return the alma rest service."""
+        if not self._alma_rest_service:
+            current_app.logger.warn("AlmaRESTService was not initialized correctly.")
+            return AlmaRESTService.build("", "")
+
+        return self._alma_rest_service
+
+    @property
+    def alma_resource(self) -> AlmaResource | AlmaResourceMock:
+        """Return the alma resource."""
+        if not self._alma_resource:
+            current_app.logger.warn("AlmaResources was not initialized correctly.")
+            return AlmaResourceMock()
+
+        return self._alma_resource
+
     def init_app(self, app: Flask) -> None:
         """Flask application initialization."""
         self.init_services(app)
         self.init_resources(app)
         app.extensions["invenio-alma"] = self
 
     def init_services(self, app: Flask) -> None:
         """Initialize service."""
         api_key = app.config.get("ALMA_API_KEY", "")
         api_host = app.config.get("ALMA_API_HOST", "")
 
         if api_key and api_host:
-            self.alma_rest_service = AlmaRESTService.build(api_key, api_host)
+            self._alma_rest_service = AlmaRESTService.build(api_key, api_host)
 
     def init_resources(self, app: Flask) -> None:
         """Initialize resources."""
         search_key = "local_control_field_009"  # ac_number
         domain = app.config.get("ALMA_SRU_DOMAIN")
         institution_code = app.config.get("ALMA_SRU_INSTITUTION_CODE")
         if domain and institution_code:
-            self.alma_resource = AlmaResource(
+            self._alma_resource = AlmaResource(
                 service=AlmaSRUService.build(search_key, domain, institution_code),
                 config=AlmaResourceConfig,
             )
```

### Comparing `invenio-alma-0.8.0/invenio_alma/resources/config.py` & `invenio-alma-0.8.1/invenio_alma/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/resources/resources.py` & `invenio-alma-0.8.1/invenio_alma/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/services/base.py` & `invenio-alma-0.8.1/invenio_alma/services/base.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/services/config.py` & `invenio-alma-0.8.1/invenio_alma/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/services/errors.py` & `invenio-alma-0.8.1/invenio_alma/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/services/rest.py` & `invenio-alma-0.8.1/invenio_alma/services/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/services/sru.py` & `invenio-alma-0.8.1/invenio_alma/services/sru.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/tasks.py` & `invenio-alma-0.8.1/invenio_alma/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/utils.py` & `invenio-alma-0.8.1/invenio_alma/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma/views.py` & `invenio-alma-0.8.1/invenio_alma/views.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.8.1/invenio_alma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.8.0
+Version: 0.8.1
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,21 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-05-01)
+
+- setup: add forgotten ruff configuration
+- ext: mock the resource and service properties
+- setup: re-add isort configuration
+
+
 Version v0.8.0 (release 2023-04-29)
 
 - ext: add existence check before resource creation
 - global: use ruff instead of pylint
 - global: add services to export
 - tasks: add option to use update func
 - sru: add search_key on the search
```

### Comparing `invenio-alma-0.8.0/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.8.1/invenio_alma.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .dockerignore
 .editorconfig
+.ruff.toml
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
```

### Comparing `invenio-alma-0.8.0/run-tests.sh` & `invenio-alma-0.8.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/setup.cfg` & `invenio-alma-0.8.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
+[tool:isort]
+profile = black
+
 [check-manifest]
 ignore = 
 	*-requirements.txt
 
 [tool:pytest]
 addopts = --black --doctest-glob="*.rst" --doctest-modules --cov=invenio_alma --cov-report=term-missing
 testpaths = tests invenio_alma
```

### Comparing `invenio-alma-0.8.0/tests/conftest.py` & `invenio-alma-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/tests/test_invenio_alma.py` & `invenio-alma-0.8.1/tests/test_invenio_alma.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.0/tests/test_invenio_alma_service.py` & `invenio-alma-0.8.1/tests/test_invenio_alma_service.py`

 * *Files identical despite different names*

