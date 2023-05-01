# Comparing `tmp/typeguard-4.0.0rc4.tar.gz` & `tmp/typeguard-4.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.0.0rc4.tar", last modified: Sat Apr 15 15:57:00 2023, max compression
+gzip compressed data, was "typeguard-4.0.0rc5.tar", last modified: Mon May  1 19:38:43 2023, max compression
```

## Comparing `typeguard-4.0.0rc4.tar` & `typeguard-4.0.0rc5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.720680 typeguard-4.0.0rc4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.724680 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.724680 typeguard-4.0.0rc4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.724680 typeguard-4.0.0rc4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.720680 typeguard-4.0.0rc4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.728680 typeguard-4.0.0rc4/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    40656 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.728680 typeguard-4.0.0rc4/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 15:57:00.000000 typeguard-4.0.0rc4/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:57:00.732680 typeguard-4.0.0rc4/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31486 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-15 15:56:49.000000 typeguard-4.0.0rc4/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.003793 typeguard-4.0.0rc5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.003793 typeguard-4.0.0rc5/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41301 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.003793 typeguard-4.0.0rc5/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31816 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16646 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/.github/workflows/publish.yml` & `typeguard-4.0.0rc5/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,22 @@
       - "[0-9]+.[0-9]+.[0-9]+.post[0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+[a-b][0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+rc[0-9]+"
 
 jobs:
   publish:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
       run: python -m build
     - name: Upload packages
       uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.pypi_password }}
```

### Comparing `typeguard-4.0.0rc4/.pre-commit-config.yaml` & `typeguard-4.0.0rc5/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.262
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
```

### Comparing `typeguard-4.0.0rc4/LICENSE` & `typeguard-4.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/PKG-INFO` & `typeguard-4.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc4
+Version: 4.0.0rc5
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc4/README.rst` & `typeguard-4.0.0rc5/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/docs/api.rst` & `typeguard-4.0.0rc5/docs/api.rst`

 * *Files 21% similar despite different names*

```diff
@@ -64,12 +64,14 @@
 .. autodecorator:: typeguard_ignore
 
 .. autofunction:: suppress_type_checks
 
 Exceptions and warnings
 -----------------------
 
+.. autoexception:: InstrumentationWarning
+
 .. autoexception:: TypeCheckError
 
 .. autoexception:: TypeCheckWarning
 
 .. autoexception:: TypeHintWarning
```

### Comparing `typeguard-4.0.0rc4/docs/conf.py` & `typeguard-4.0.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/docs/extending.rst` & `typeguard-4.0.0rc5/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/docs/features.rst` & `typeguard-4.0.0rc5/docs/features.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/docs/userguide.rst` & `typeguard-4.0.0rc5/docs/userguide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,27 @@
     @typeguard_ignore
     def f(x: int) -> int:
         return str(x)
 
 .. warning:: The :func:`@no_type_check_decorator <typing.no_type_check_decorator>`
     decorator is not currently recognized by Typeguard.
 
+Suppressing the ``@typechecked`` decorator in production
+--------------------------------------------------------
+
+If you're using the :func:`@typechecked <typechecked>` decorator to gradually introduce
+run-time type checks to your code base, you can disable the checks in production by
+running Python in optimized mode (as opposed to debug mode which is the default mode).
+You can do this by either starting Python with the ``-O`` or ``-OO`` option, or by
+setting the PYTHONOPTIMIZE_ environment variable. This will cause
+:func:`@typechecked <typechecked>` to become a no-op when the import hook is not being
+used to instrument the code.
+
+.. _PYTHONOPTIMIZE: https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE
+
 Debugging instrumented code
 ---------------------------
 
 If you find that your code behaves in an unexpected fashion with the Typeguard
 instrumentation in place, you should set the ``typeguard.config.debug_instrumentation``
 flag to ``True``. This will print all the instrumented code after the modifications,
 which you can check to find the reason for the unexpected behavior.
```

### Comparing `typeguard-4.0.0rc4/docs/versionhistory.rst` & `typeguard-4.0.0rc5/docs/versionhistory.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.0.0rc5** (2023-05-01)
+
+- Added ``InstrumentationWarning`` to the public API
+- Changed ``@typechecked`` to skip instrumentation in optimized mode, as in typeguard
+  2.x
+- Avoid type checks where the types in question are shadowed by local variables
+- Fixed instrumentation using ``typing.Optional`` without a subscript when the subscript
+  value was erased due to being an ignored import
+- Fixed ``TypeError: isinstance() arg 2 must be a type or tuple of types`` when
+  instrumented code tries to check a value against a naked (``str``, not ``ForwardRef``)
+  forward reference
+- Fixed instrumentation using the wrong "self" type in the ``__new__()`` method
+
 **4.0.0rc4** (2023-04-15)
 
 - Fixed imports guarded by ``if TYPE_CHECKING:`` when used with subscripts
   (``SomeType[...]``) being replaced with ``Any[...]`` instead of just ``Any``
 - Fixed instrumentation inadvertently mutating a function's annotations on Python 3.7
   and 3.8
 - Fixed ``Concatenate[...]`` in ``Callable`` parameters causing ``TypeError`` to be
```

### Comparing `typeguard-4.0.0rc4/pyproject.toml` & `typeguard-4.0.0rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/__init__.py` & `typeguard-4.0.0rc5/src/typeguard/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ._checkers import checker_lookup_functions as checker_lookup_functions
 from ._checkers import load_plugins as load_plugins
 from ._config import CollectionCheckStrategy as CollectionCheckStrategy
 from ._config import ForwardRefPolicy as ForwardRefPolicy
 from ._config import TypeCheckConfiguration as TypeCheckConfiguration
 from ._decorators import typechecked as typechecked
 from ._decorators import typeguard_ignore as typeguard_ignore
+from ._exceptions import InstrumentationWarning as InstrumentationWarning
 from ._exceptions import TypeCheckError as TypeCheckError
 from ._exceptions import TypeCheckWarning as TypeCheckWarning
 from ._exceptions import TypeHintWarning as TypeHintWarning
 from ._functions import TypeCheckFailCallback as TypeCheckFailCallback
 from ._functions import check_type as check_type
 from ._functions import warn_on_error as warn_on_error
 from ._importhook import ImportHookManager as ImportHookManager
```

### Comparing `typeguard-4.0.0rc4/src/typeguard/_checkers.py` & `typeguard-4.0.0rc5/src/typeguard/_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -752,16 +752,24 @@
 
     for lookup_func in checker_lookup_functions:
         checker = lookup_func(origin_type, args, extras)
         if checker:
             checker(value, origin_type, args, memo)
             return
 
-    if not isinstance(value, origin_type):
-        raise TypeCheckError(f"is not an instance of {qualified_name(origin_type)}")
+    if isclass(origin_type):
+        if not isinstance(value, origin_type):
+            raise TypeCheckError(f"is not an instance of {qualified_name(origin_type)}")
+    elif type(origin_type) is str:
+        warnings.warn(
+            f"Skipping type check against {origin_type!r}; this looks like a "
+            f"string-form forward reference imported from another module",
+            TypeHintWarning,
+            stacklevel=get_stacklevel(),
+        )
 
 
 # Equality checks are applied to these
 origin_type_checkers = {
     bytes: check_byteslike,
     AbstractSet: check_set,
     BinaryIO: check_io,
```

### Comparing `typeguard-4.0.0rc4/src/typeguard/_config.py` & `typeguard-4.0.0rc5/src/typeguard/_config.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_decorators.py` & `typeguard-4.0.0rc5/src/typeguard/_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,18 @@
     annotated local variables.
 
     This can also be used as a class decorator. This will instrument all type annotated
     methods, including :func:`@classmethod <classmethod>`,
     :func:`@staticmethod <staticmethod>`,  and :class:`@property <property>` decorated
     methods in the class.
 
+    .. note:: When Python is run in optimized mode (``-O`` or ``-OO``, this decorator
+        is a no-op). This is a feature meant for selectively introducing type checking
+        into a code base where the checks aren't meant to be run in production.
+
     :param target: the function or class to enable type checking for
     :param forward_ref_policy: override for
         :attr:`.TypeCheckConfiguration.forward_ref_policy`
     :param typecheck_fail_callback: override for
         :attr:`.TypeCheckConfiguration.typecheck_fail_callback`
     :param collection_check_strategy: override for
         :attr:`.TypeCheckConfiguration.collection_check_strategy`
@@ -166,14 +170,17 @@
             typechecked,
             forward_ref_policy=forward_ref_policy,
             typecheck_fail_callback=typecheck_fail_callback,
             collection_check_strategy=collection_check_strategy,
             debug_instrumentation=debug_instrumentation,
         )
 
+    if not __debug__:
+        return target
+
     if isclass(target):
         for key, attr in target.__dict__.items():
             if is_method_of(attr, target):
                 retval = instrument(attr)
                 if isfunction(retval):
                     setattr(target, key, retval)
             elif isinstance(attr, (classmethod, staticmethod)):
```

### Comparing `typeguard-4.0.0rc4/src/typeguard/_exceptions.py` & `typeguard-4.0.0rc5/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_functions.py` & `typeguard-4.0.0rc5/src/typeguard/_functions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_importhook.py` & `typeguard-4.0.0rc5/src/typeguard/_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_memo.py` & `typeguard-4.0.0rc5/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_pytest_plugin.py` & `typeguard-4.0.0rc5/src/typeguard/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_suppression.py` & `typeguard-4.0.0rc5/src/typeguard/_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_transformer.py` & `typeguard-4.0.0rc5/src/typeguard/_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,16 +406,19 @@
                         items[index] = self.transformer._get_import("typing", "Any")
 
                 slice_value.elts = items
             else:
                 self.generic_visit(node)
 
                 # If the transformer erased the slice entirely, just return the node
-                # value without the subscript
-                if sys.version_info >= (3, 9) and not hasattr(node, "slice"):
+                # value without the subscript (unless it's Optional, in which case erase
+                # the node entirely
+                if self._memo.name_matches(node.value, "typing.Optional"):
+                    return None
+                elif sys.version_info >= (3, 9) and not hasattr(node, "slice"):
                     return node.value
                 elif sys.version_info < (3, 9) and not hasattr(node.slice, "value"):
                     return node.value
 
         return node
 
     def visit_Name(self, node: Name) -> Any:
@@ -788,19 +791,24 @@
                         ):
                             memo_kwargs["self_type"] = Name(
                                 id=node.args.args[0].arg, ctx=Load()
                             )
                             break
                     else:
                         if node.args.args:
-                            memo_kwargs["self_type"] = Attribute(
-                                Name(id=node.args.args[0].arg, ctx=Load()),
-                                "__class__",
-                                ctx=Load(),
-                            )
+                            if node.name == "__new__":
+                                memo_kwargs["self_type"] = Name(
+                                    id=node.args.args[0].arg, ctx=Load()
+                                )
+                            else:
+                                memo_kwargs["self_type"] = Attribute(
+                                    Name(id=node.args.args[0].arg, ctx=Load()),
+                                    "__class__",
+                                    ctx=Load(),
+                                )
 
                 # Construct the function reference
                 # Nested functions get special treatment: the function name is added
                 # to free variables (and the closure of the resulting function)
                 names: list[str] = [node.name]
                 memo = self._memo.parent
                 while memo:
@@ -935,14 +943,15 @@
         self.generic_visit(node)
 
         if (
             isinstance(self._memo.node, (FunctionDef, AsyncFunctionDef))
             and node.annotation
             and isinstance(node.target, Name)
         ):
+            self._memo.ignored_names.add(node.target.id)
             annotation = self._convert_annotation(deepcopy(node.annotation))
             if annotation:
                 self._memo.variable_annotations[node.target.id] = annotation
                 if node.value:
                     func_name = self._get_import(
                         "typeguard._functions", "check_variable_assignment"
                     )
@@ -984,14 +993,15 @@
                 for exp in elts:
                     prefix = ""
                     if isinstance(exp, Starred):
                         exp = exp.value
                         prefix = "*"
 
                     if isinstance(exp, Name):
+                        self._memo.ignored_names.add(exp.id)
                         name = prefix + exp.id
                         annotation = self._memo.variable_annotations.get(exp.id)
                         if annotation:
                             annotations_[Constant(name)] = annotation
                             check_required = True
                         else:
                             annotations_[Constant(name)] = None
@@ -1043,14 +1053,16 @@
         """This injects a type check into an assignment expression (a := foo())."""
         self.generic_visit(node)
 
         # Only instrument function-local assignments
         if isinstance(self._memo.node, (FunctionDef, AsyncFunctionDef)) and isinstance(
             node.target, Name
         ):
+            self._memo.ignored_names.add(node.target.id)
+
             # Bail out if no matching annotation is found
             annotation = self._memo.variable_annotations.get(node.target.id)
             if annotation is None:
                 return node
 
             func_name = self._get_import(
                 "typeguard._functions", "check_variable_assignment"
```

### Comparing `typeguard-4.0.0rc4/src/typeguard/_union_transformer.py` & `typeguard-4.0.0rc5/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard/_utils.py` & `typeguard-4.0.0rc5/src/typeguard/_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.0.0rc5/src/typeguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc4
+Version: 4.0.0rc5
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc4/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.0.0rc5/src/typeguard.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/features_request.yaml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/api.rst
 docs/conf.py
+docs/contributing.rst
 docs/extending.rst
 docs/features.rst
 docs/index.rst
 docs/userguide.rst
 docs/versionhistory.rst
 src/typeguard/__init__.py
 src/typeguard/_checkers.py
```

### Comparing `typeguard-4.0.0rc4/tests/__init__.py` & `typeguard-4.0.0rc5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/conftest.py` & `typeguard-4.0.0rc5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/dummymodule.py` & `typeguard-4.0.0rc5/tests/dummymodule.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/mypy/negative.py` & `typeguard-4.0.0rc5/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/mypy/positive.py` & `typeguard-4.0.0rc5/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/mypy/test_type_annotations.py` & `typeguard-4.0.0rc5/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_checkers.py` & `typeguard-4.0.0rc5/tests/test_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 
 import pytest
 
 from typeguard import (
     CollectionCheckStrategy,
     ForwardRefPolicy,
     TypeCheckError,
+    TypeCheckMemo,
     TypeHintWarning,
     check_type,
+    check_type_internal,
     suppress_type_checks,
 )
 from typeguard._utils import qualified_name
 
 from . import (
     Child,
     Employee,
@@ -1033,7 +1035,15 @@
 def test_none():
     check_type(None, None)
 
 
 def test_return_checked_value():
     value = {"foo": 1}
     assert check_type(value, Dict[str, int]) is value
+
+
+def test_imported_str_forward_ref():
+    value = {"foo": 1}
+    memo = TypeCheckMemo(globals(), locals())
+    pattern = r"Skipping type check against 'Dict\[str, int\]'"
+    with pytest.warns(TypeHintWarning, match=pattern):
+        check_type_internal(value, "Dict[str, int]", memo)
```

### Comparing `typeguard-4.0.0rc4/tests/test_importhook.py` & `typeguard-4.0.0rc5/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_instrumentation.py` & `typeguard-4.0.0rc5/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_plugins.py` & `typeguard-4.0.0rc5/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_suppression.py` & `typeguard-4.0.0rc5/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_transformer.py` & `typeguard-4.0.0rc5/tests/test_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -588,14 +588,46 @@
                     check_argument_types('Foo.foo', {'x': (x, int)}, memo)
                     return check_return_type('Foo.foo', x, int, memo)
             """
         ).strip()
     )
 
 
+def test_new() -> None:
+    node = parse(
+        dedent(
+            """
+            from typing import Self
+
+            class Foo:
+                def __new__(cls) -> Self:
+                    return super().__new__(cls)
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from typeguard import TypeCheckMemo
+            from typeguard._functions import check_return_type
+            from typing import Self
+
+            class Foo:
+
+                def __new__(cls) -> Self:
+                    memo = TypeCheckMemo(globals(), locals(), self_type=cls)
+                    return check_return_type('Foo.__new__', super().__new__(cls), \
+Self, memo)
+            """
+        ).strip()
+    )
+
+
 def test_local_function() -> None:
     node = parse(
         dedent(
             """
             def wrapper():
                 def foo(x: int) -> int:
                     return x
@@ -917,14 +949,44 @@
 typing.Collection, Sequence]:
                     yield 'foo'
                     return (1, 2)
                 """
             ).strip()
         )
 
+    def test_optional(self) -> None:
+        node = parse(
+            dedent(
+                """
+                from typing import Any, Optional, TYPE_CHECKING
+                from collections.abc import Generator
+                if TYPE_CHECKING:
+                    from typing import Hashable
+
+                def foo(x: Optional[Hashable]) -> Optional[Hashable]:
+                    return x
+                """
+            )
+        )
+        TypeguardTransformer().visit(node)
+        assert (
+            unparse(node)
+            == dedent(
+                """
+                from typing import Any, Optional, TYPE_CHECKING
+                from collections.abc import Generator
+                if TYPE_CHECKING:
+                    from typing import Hashable
+
+                def foo(x: Optional[Hashable]) -> Optional[Hashable]:
+                    return x
+                """
+            ).strip()
+        )
+
 
 class TestAssign:
     def test_annotated_assign(self) -> None:
         node = parse(
             dedent(
                 """
                 def foo() -> None:
@@ -1311,7 +1373,86 @@
             def foo(x: kwargs, /, y: args, *args: x, baz: x, **kwargs: y) -> \
 Generator[args, x, kwargs]:
                 yield y
                 return x
             """
         ).strip()
     )
+
+
+def test_local_assignment_typename_conflicts() -> None:
+    node = parse(
+        dedent(
+            """
+            def foo() -> int:
+                int = 6
+                return int
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            def foo() -> int:
+                int = 6
+                return int
+            """
+        ).strip()
+    )
+
+
+def test_local_ann_assignment_typename_conflicts() -> None:
+    node = parse(
+        dedent(
+            """
+            from typing import Any
+
+            def foo() -> int:
+                int: Any = 6
+                return int
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from typing import Any
+
+            def foo() -> int:
+                int: Any = 6
+                return int
+            """
+        ).strip()
+    )
+
+
+def test_local_named_expr_typename_conflicts() -> None:
+    node = parse(
+        dedent(
+            """
+            from typing import Any
+
+            def foo() -> int:
+                if (int := 6):
+                    pass
+                return int
+            """
+        )
+    )
+    TypeguardTransformer().visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from typing import Any
+
+            def foo() -> int:
+                if (int := 6):
+                    pass
+                return int
+            """
+        ).strip()
+    )
```

### Comparing `typeguard-4.0.0rc4/tests/test_typechecked.py` & `typeguard-4.0.0rc5/tests/test_typechecked.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
+import subprocess
 import sys
 from contextlib import contextmanager
+from pathlib import Path
 from textwrap import dedent
 from typing import (
     Any,
     AsyncGenerator,
     AsyncIterable,
     AsyncIterator,
     Generator,
@@ -581,7 +583,42 @@
     class Foo:
         @contextmanager
         def method(self, x: int) -> None:
             yield x + 1
 
     with Foo().method(6) as value:
         assert value == 7
+
+
+@pytest.mark.parametrize(
+    "flags, expected_return_code",
+    [
+        pytest.param([], 1, id="debug"),
+        pytest.param(["-O"], 0, id="O"),
+        pytest.param(["-OO"], 0, id="OO"),
+    ],
+)
+def test_typechecked_disabled_in_optimized_mode(
+    tmp_path: Path, flags: List[str], expected_return_code: int
+):
+    code = dedent(
+        """
+        from typeguard import typechecked
+
+        @typechecked
+        def foo(x: int) -> None:
+            pass
+
+        foo("a")
+        """
+    )
+    script_path = tmp_path / "code.py"
+    script_path.write_text(code)
+    process = subprocess.run(
+        [sys.executable, *flags, str(script_path)], capture_output=True
+    )
+    assert process.returncode == expected_return_code
+    if process.returncode == 1:
+        assert process.stderr.endswith(
+            b'typeguard.TypeCheckError: argument "x" (str) is not an instance of '
+            b"int\n"
+        )
```

### Comparing `typeguard-4.0.0rc4/tests/test_union_transformer.py` & `typeguard-4.0.0rc5/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_utils.py` & `typeguard-4.0.0rc5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc4/tests/test_warn_on_error.py` & `typeguard-4.0.0rc5/tests/test_warn_on_error.py`

 * *Files identical despite different names*

