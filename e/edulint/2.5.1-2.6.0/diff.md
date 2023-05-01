# Comparing `tmp/edulint-2.5.1.tar.gz` & `tmp/edulint-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-ihs2rfr0/edulint-2.5.1.tar", last modified: Mon Apr 17 15:31:57 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-qlz22kih/edulint-2.6.0.tar", last modified: Mon May  1 19:28:22 2023, max compression
```

## Comparing `edulint-2.5.1.tar` & `edulint-2.6.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:31:42.000000 edulint-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 15:31:57.000000 edulint-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-17 15:31:42.000000 edulint-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/config/config_translations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-17 15:31:42.000000 edulint-2.5.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:31:57.000000 edulint-2.5.1/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 15:31:42.000000 edulint-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-17 15:31:57.000000 edulint-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-17 15:31:42.000000 edulint-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:57.000000 edulint-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-17 15:31:42.000000 edulint-2.5.1/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 19:28:11.000000 edulint-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-01 19:28:22.000000 edulint-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-01 19:28:11.000000 edulint-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/config/config_translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-01 19:28:11.000000 edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 19:28:22.000000 edulint-2.6.0/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 19:28:11.000000 edulint-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-01 19:28:22.000000 edulint-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-01 19:28:11.000000 edulint-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:22.000000 edulint-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-01 19:28:11.000000 edulint-2.6.0/tests/test_visitors.py
```

### Comparing `edulint-2.5.1/LICENSE` & `edulint-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/PKG-INFO` & `edulint-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.5.1
+Version: 2.6.0
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.5.1/README.md` & `edulint-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/config/config.py` & `edulint-2.6.0/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/config/config_translations.py` & `edulint-2.6.0/edulint/config/config_translations.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 
 
 CONFIG_TRANSLATIONS: Dict[Option, Translation] = {
     Option.ENHANCEMENT: Translation(
         Linter.PYLINT,
         ["--enable=no-self-use,superfluous-parens,consider-using-min-builtin,"
          "consider-using-max-builtin,consider-using-with,unspecified-encoding,"
-         "use-augmenting-assignment,shadowing-in-comprehension,"
-         "loop-shadows-control-variable,use-append,no-repeated-op,"
+         "loop-shadows-control-variable,no-repeated-op,"
          "forbidden-top-level-code,simplifiable-if-nested,simplifiable-if-seq,"
          "simplifiable-if-return-conj,simplifiable-if-assignment-conj,simplifiable-if-expr-conj,"]
     ),
     Option.PYTHON_SPECIFIC: Translation(
         Linter.PYLINT,
         ["--enable=unidiomatic-typecheck,misplaced-format-function,"
-         "unnecessary-lambda,multiple-imports,"
-         "improve-for-loop,consider-iterating-dictionary,"
+         "unnecessary-lambda,multiple-imports,use-enumerate,consider-iterating-dictionary,"
          "consider-using-dict-items,consider-using-f-string,"
          "inconsistent-return-statements,consider-swap-variables,"
          "consider-using-join,consider-using-set-comprehension,"
          "unnecessary-comprehension,use-a-generator,use-list-literal,"
          "use-dict-literal,consider-using-in,"]
     ),
     Option.COMPLEXITY: Translation(
```

### Comparing `edulint-2.5.1/edulint/edulint.py` & `edulint-2.6.0/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/explanations.toml` & `edulint-2.6.0/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linters.py` & `edulint-2.6.0/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/.pylintrc` & `edulint-2.6.0/edulint/linting/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,17 @@
        wildcard-import,
        reimported,
        invalid-for-target,
        one-iteration,
        no-is-bool,
        use-ord-letter,
        use-literal-letter,
+       use-foreach,
+       use-append,
+       use-augmenting-assignment,
 
 
 [REPORTS]
 
 # Python expression which should return a score less than or equal to 10. You
 # have access to the variables 'error', 'warning', 'refactor', and 'convention'
 # which contain the number of messages in each category, as well as 'statement'
```

### Comparing `edulint-2.5.1/edulint/linting/checkers/basic_checker.py` & `edulint-2.6.0/edulint/linting/checkers/basic_checker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,35 @@
-from astroid import nodes  # type: ignore
-from typing import TYPE_CHECKING, Optional, List, Union
+from astroid import nodes, Context  # type: ignore
+from typing import TYPE_CHECKING, Optional, List, Union, Tuple
+from enum import Enum, auto
+from functools import reduce
 
 from pylint.checkers import BaseChecker  # type: ignore
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter  # type: ignore
 
 from edulint.linting.checkers.utils import get_name, is_builtin, get_range_params
 from edulint.linting.checkers.modified_listener import ModifiedListener
 
 
+class UsesIndex(Enum):
+    OUTSIDE_SUBSCRIPT = auto()
+    INSIDE_SUBSCRIPT = auto()
+    NEVER = auto()
+
+    @classmethod
+    def combine(cls, lt: "UsesIndex", rt: "UsesIndex") -> "UsesIndex":
+        if lt == cls.INSIDE_SUBSCRIPT or rt == cls.INSIDE_SUBSCRIPT:
+            return cls.INSIDE_SUBSCRIPT
+        if lt == cls.OUTSIDE_SUBSCRIPT or rt == cls.OUTSIDE_SUBSCRIPT:
+            return cls.OUTSIDE_SUBSCRIPT
+        return cls.NEVER
+
+
 class ImproveForLoop(BaseChecker):  # type: ignore
 
     name = "improve-for-loop"
     msgs = {
         "R6101": (
             "Iterate directly: \"for var in %s\" (with appropriate name for \"var\")",
             "use-foreach",
@@ -25,74 +41,82 @@
             "Emitted when a for-range loop is used with the element at each index is accessed as well.",
         ),
     }
 
     def __init__(self, linter: Optional["PyLinter"] = None) -> None:
         super().__init__(linter)
 
-    class StructureIndexedVisitor(ModifiedListener[bool]):
-        default = False
+    class StructureIndexedVisitor(ModifiedListener[Tuple[bool, bool]]):
+        default = (False, False)
 
         @staticmethod
-        def combine(results: List[bool]) -> bool:
-            return any(results)
+        def combine(results: List[Tuple[bool, bool]]) -> Tuple[bool, bool]:
+            return any(loaded for loaded, _stored in results), any(stored for _loaded, stored in results)
 
         def __init__(self, structure: Union[nodes.Name, nodes.Attribute], index: nodes.Name):
+            super().__init__([structure, index])
             self.structure = structure
             self.index = index
-            super().__init__([structure, index])
 
-        def visit_subscript(self, subscript: nodes.Subscript) -> bool:
-            sub_result = self.visit_many(subscript.get_children())
-            if sub_result:
-                return sub_result
+        def visit_subscript(self, subscript: nodes.Subscript) -> Tuple[bool, bool]:
+            sub_loaded, sub_stored = self.visit_many(subscript.get_children())
 
-            parent = subscript.parent
             if self.was_reassigned(self.structure, allow_definition=False) \
                     or self.was_reassigned(self.index, allow_definition=False):
-                return False
-            if not isinstance(subscript.value, type(self.structure)) \
-                    or (isinstance(parent, nodes.Assign) and subscript in parent.targets) \
-                    or not isinstance(subscript.slice, nodes.Name):
-                return sub_result
-
-            return subscript.slice.name == self.index.name and (
-                (isinstance(self.structure, nodes.Name) and self.structure.name == subscript.value.name)
-                or (isinstance(self.structure, nodes.Attribute) and self.structure.attrname == subscript.value.attrname)
-            )
+                return False, False
+
+            used = subscript.value.as_string() == self.structure.as_string() \
+                and isinstance(subscript.slice, nodes.Name) \
+                and subscript.slice.as_string() == self.index.as_string()
 
-    class IndexUsedVisitor(ModifiedListener[bool]):
-        default = False
+            if subscript.ctx == Context.Store:
+                return sub_loaded, sub_stored or used
+
+            if subscript.ctx == Context.Load:
+                return sub_loaded or used, sub_stored
+
+            assert subscript.ctx == Context.Del
+            return sub_loaded, sub_stored or used
+
+    class IndexUsedVisitor(ModifiedListener[UsesIndex]):
+        default = UsesIndex.NEVER
 
         @staticmethod
-        def combine(results: List[bool]) -> bool:
-            return any(results)
+        def combine(results: List[UsesIndex]) -> UsesIndex:
+            return reduce(UsesIndex.combine, results, UsesIndex.NEVER)
 
         def __init__(self, structure: Union[nodes.Name, nodes.Attribute], index: nodes.Name):
+            super().__init__([structure, index])
             self.structure = structure
             self.index = index
-            super().__init__([structure, index])
 
-        def visit_name(self, name: nodes.Name) -> bool:
-            super().visit_name(name)
+        def visit_name(self, name: nodes.Name) -> UsesIndex:
             if name.name != self.index.name:
-                return False
+                return UsesIndex.NEVER
+
+            parent = name.parent
+            if isinstance(parent, nodes.Subscript) and parent.value.as_string() != self.structure.as_string():
+                return UsesIndex.INSIDE_SUBSCRIPT
+
             if not isinstance(name.parent, nodes.Subscript) \
                     or not isinstance(self.structure, type(name.parent.value)) \
                     or self.was_reassigned(name, allow_definition=False):
-                return True
+                return UsesIndex.OUTSIDE_SUBSCRIPT
 
             subscript = name.parent
             if not ((isinstance(subscript.value, nodes.Name)
                     and subscript.value.name == self.structure.name)
                     or (isinstance(subscript.value, nodes.Attribute)
                     and subscript.value.attrname == self.structure.attrname)):
-                return True
+                return UsesIndex.OUTSIDE_SUBSCRIPT
+
+            if isinstance(subscript.parent, nodes.Assign) and subscript in subscript.parent.targets:
+                return UsesIndex.OUTSIDE_SUBSCRIPT
 
-            return isinstance(subscript.parent, nodes.Assign) and subscript in subscript.parent.targets
+            return UsesIndex.NEVER
 
     def visit_for(self, node: nodes.For) -> None:
         range_params = get_range_params(node.iter)
         if range_params is None:
             return
 
         start, stop, step = range_params
@@ -102,20 +126,28 @@
             return
 
         structure = stop.args[0]
         index = node.target
         if not isinstance(structure, nodes.Name) and not isinstance(structure, nodes.Attribute):
             return
 
-        if self.StructureIndexedVisitor(structure, node.target).visit_many(node.body):
-            structure_name = get_name(structure)
-            if self.IndexUsedVisitor(structure, node.target).visit_many(node.body):
-                self.add_message("use-enumerate", args=(index.name, structure_name), node=node)
-            else:
-                self.add_message("use-foreach", args=structure_name, node=node)
+        loaded, stored = self.StructureIndexedVisitor(structure, node.target).visit_many(node.body)
+        if not loaded:
+            return
+
+        structure_name = get_name(structure)
+        uses_index = self.IndexUsedVisitor(structure, node.target).visit_many(node.body)
+
+        if uses_index == UsesIndex.INSIDE_SUBSCRIPT:
+            return
+        elif stored or uses_index == UsesIndex.OUTSIDE_SUBSCRIPT:
+            self.add_message("use-enumerate", args=(index.name, structure_name), node=node)
+        else:
+            assert uses_index == UsesIndex.NEVER
+            self.add_message("use-foreach", args=structure_name, node=node)
 
 
 class NoGlobalVars(BaseChecker):
     name = "no-global-variables"
     msgs = {
         "R6401": (
             "Do not use global variables; you use %s, modifying it for example at line %i.",
```

### Comparing `edulint-2.5.1/edulint/linting/checkers/improper_loop.py` & `edulint-2.6.0/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/checkers/modified_listener.py` & `edulint-2.6.0/edulint/linting/checkers/modified_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,8 +148,8 @@
                         target if type(target) in (nodes.DelName, nodes.DelAttr) else node
                     )
 
         return self.visit_many(node.get_children())
 
     def visit_for(self, node: nodes.For) -> T:
         self._visit_assigned_to(node.target)
-        return self.visit_many(node.body)
+        return self.visit_many(node.get_children())
```

### Comparing `edulint-2.5.1/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.6.0/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/checkers/short_problems.py` & `edulint-2.6.0/edulint/linting/checkers/short_problems.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,19 +204,34 @@
                 or (op in ("/", "//", "%")
                     and (isinstance(node, nodes.BinOp) and node.left.as_string() == node.right.as_string()
                          or isinstance(node, nodes.AugAssign) and node.target.as_string() == node.value.as_string())) \
                 or (op == "**" and right in (0, 1)):
             self.add_message("redundant-arithmetic", node=node, args=(node.as_string(),))
 
     def _check_augmentable(self, node: Union[nodes.Assign, nodes.AnnAssign]) -> None:
+        IMMUTABLE_OPS = ("-", "*", "/", "//", "%", "**", "<<", ">>")
+
         def add_message(target: str, param: nodes.BinOp) -> None:
             self.add_message("use-augmenting-assignment", node=node, args=(target, node.value.op, param.as_string()))
 
-        def is_mutable(node: nodes.NodeNG):
-            return type(node) in (nodes.List, nodes.Dict, nodes.Set, nodes.ListComp, nodes.DictComp)
+        def is_immutable(node: nodes.NodeNG):
+            if isinstance(node, (nodes.Const)) and isinstance(node.value, (int, float, bool, str, bytes, tuple)):
+                return True
+            if isinstance(node, nodes.BinOp):
+                return node.op in IMMUTABLE_OPS \
+                    or is_immutable(node.left) or is_immutable(node.right)
+            if isinstance(node, nodes.Call):
+                return any(node.func.as_string().endswith(n) for n in (
+                    "int", "float", "bool", "str", "bytes", "tuple",
+                    "len", "sum", "chr", "ord",
+                    "trunc", "round", "sqrt", "cos", "sin", "radians", "degrees",
+                ))
+            if isinstance(node, nodes.IfExp):
+                return is_immutable(node.body) or is_immutable(node.orelse)
+            return False
 
         if not isinstance(node.value, nodes.BinOp):
             return
         bin_op = node.value
 
         if isinstance(node, nodes.Assign):
             target = node.targets[0].as_string()
@@ -224,22 +239,20 @@
             target = node.target.as_string()
         else:
             assert False, "unreachable"
 
         left_value = infer_to_value(bin_op.left)
         right_value = infer_to_value(bin_op.right)
 
-        if is_mutable(left_value) or is_mutable(right_value):
-            return
-
-        if target == bin_op.left.as_string():
-            add_message(target, bin_op.right)
-        if bin_op.op in "+*|&" and target == bin_op.right.as_string():
-            if not isinstance(left_value, nodes.Const) or not isinstance(left_value.value, (str, bytes)):
-                add_message(target, bin_op.left)
+        if node.value.op in IMMUTABLE_OPS or is_immutable(left_value) or is_immutable(right_value):
+            if target == bin_op.left.as_string():
+                add_message(target, bin_op.right)
+            elif bin_op.op in "+*|&" and target == bin_op.right.as_string():
+                if not isinstance(left_value, nodes.Const) or not isinstance(left_value.value, (str, bytes, tuple)):
+                    add_message(target, bin_op.left)
 
     def _check_multiplied_list(self, node: nodes.BinOp) -> None:
         def is_mutable(elem: nodes.NodeNG) -> bool:
             return type(elem) in (nodes.List, nodes.Set, nodes.Dict) \
                 or (
                     isinstance(elem, nodes.Call)
                     and isinstance(elem.func, nodes.Name)
```

### Comparing `edulint-2.5.1/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.6.0/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/checkers/utils.py` & `edulint-2.6.0/edulint/linting/checkers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,11 +114,11 @@
 
 
 def infer_to_value(node: nodes.NodeNG) -> Optional[nodes.NodeNG]:
     if isinstance(node, nodes.Name):
         inferred = utils.safe_infer(node)
         return None if inferred is Uninferable else inferred
 
-    if type(node) in (nodes.Const, nodes.List, nodes.Set, nodes.Dict, nodes.ListComp, nodes.DictComp):
+    if isinstance(node, (nodes.Const, nodes.List, nodes.Set, nodes.Dict, nodes.ListComp, nodes.DictComp, nodes.Call)):
         return node
 
     return None
```

### Comparing `edulint-2.5.1/edulint/linting/linting.py` & `edulint-2.6.0/edulint/linting/linting.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 def lint_any(
         linter: Linter, filenames: List[str], linter_args: List[str], config_arg: ImmutableArg,
         result_getter: Callable[[Any], Any],
         out_to_problem: Callable[[ProblemJson], Problem]) -> List[Problem]:
     command = [sys.executable, "-m", str(linter)] + linter_args + list(config_arg) + filenames  # type: ignore
-    return_code, outs, errs = ProcessHandler.run(command, timeout=10)
+    return_code, outs, errs = ProcessHandler.run(command, timeout=1000)
 
     if ProcessHandler.is_status_code_by_timeout(return_code):
         print(f"edulint: {linter} was likely killed by timeout", file=sys.stderr)
         raise TimeoutError(f"Timeout from {linter}")
 
     print(errs, file=sys.stderr, end="")
     if (linter == Linter.FLAKE8 and return_code not in (0, 1)) or (linter == Linter.PYLINT and return_code == 32):
```

### Comparing `edulint-2.5.1/edulint/linting/overrides.py` & `edulint-2.6.0/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/problem.py` & `edulint-2.6.0/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/process_handler.py` & `edulint-2.6.0/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/linting/tweakers.py` & `edulint-2.6.0/edulint/linting/tweakers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/options.py` & `edulint-2.6.0/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/__init__.py` & `edulint-2.6.0/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.6.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.6.0/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.6.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.6.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.6.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/edulint.egg-info/PKG-INFO` & `edulint-2.6.0/edulint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.5.1
+Version: 2.6.0
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.5.1/edulint.egg-info/SOURCES.txt` & `edulint-2.6.0/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/setup.cfg` & `edulint-2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/setup.py` & `edulint-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/tests/test_config.py` & `edulint-2.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/tests/test_improper_loop.py` & `edulint-2.6.0/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/tests/test_lint.py` & `edulint-2.6.0/tests/test_lint.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,35 @@
 from utils import lazy_problem, lazy_equal, get_tests_path, apply_and_lint, create_apply_and_lint
 from typing import List
 
 
 @pytest.mark.parametrize("filename,config,expected_output", [
     ("hello_world.py", Config(), []),
     ("z202817-zkouska.py", Config(), [
+        lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6205").set_line(82),
+        lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("W0107").set_line(196)
     ]),
     ("z202817-zkouska.py", Config([Arg(Option.PYLINT, ["--enable=C0115"])]), [
+        lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6205").set_line(82),
         lazy_problem().set_code("C0115").set_line(122),
         lazy_problem().set_code("C0115").set_line(128),
+        lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("W0107").set_line(196)
     ]),
-    ("z202817-zkouska.py", Config([Arg(Option.PYLINT, ["--enable=C0115", "--disable=W0107"])]), [
+    ("z202817-zkouska.py", Config([Arg(Option.PYLINT, ["--enable=C0115", "--disable=W0107,R6609"])]), [
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6205").set_line(82),
         lazy_problem().set_code("C0115").set_line(122),
-        lazy_problem().set_code("C0115").set_line(128)
+        lazy_problem().set_code("C0115").set_line(128),
+        lazy_problem().set_code("R6101").set_line(171),
     ]),
     ("z202817-zkouska.py",
      Config([Arg(Option.PYLINT, ["--disable=all"])]), []),
     ("002814-p1_trapezoid.py", Config(), [
         lazy_problem().set_code("F401").set_line(1),
         lazy_problem().set_code("F401").set_line(1),
         lazy_problem().set_code("E501").set_line(1),
@@ -45,27 +50,28 @@
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("z202817-zkouska.py", [Arg(Option.ENHANCEMENT, "on")], [
         lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6208").set_line(76),
         lazy_problem().set_code("R6205").set_line(82),
+        lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("W0107").set_line(196),
     ]),
     ("z202817-zkouska.py", [Arg(Option.PYTHON_SPECIFIC, "on")], [
+        lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6102").set_line(80),
         lazy_problem().set_code("R6205").set_line(82),
         lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("C0123").set_line(172),
         lazy_problem().set_code("W0107").set_line(196),
     ]),
     ("z202817-zkouska.py", [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYTHON_SPECIFIC, "on")], [
         lazy_problem().set_code("R6102").set_line(80),
-        lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("C0123").set_line(172),
     ]),
     ("z202817-zkouska.py", [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYTHON_SPECIFIC, "off")], []),
     ("hw34406.py", [Arg(Option.PYLINT, "--disable=all"), Arg(Option.COMPLEXITY, "on")], [
         lazy_problem().set_line(240).set_code("R0913"),
         lazy_problem().set_line(266).set_code("R0911"),
         lazy_problem().set_line(266).set_code("R0912"),
@@ -150,15 +156,19 @@
     ("014180-p5_fibsum.py", [Arg(Option.ALLOWED_ONECHAR_NAMES, "i")], [
         lazy_problem().set_code("C0104").set_line(6)
     ]),
     ("014180-p5_fibsum.py", [Arg(Option.ALLOWED_ONECHAR_NAMES, "in")], [
     ])
 ])
 def test_allowed_onechar_names(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
-    apply_and_lint(filename, args, expected_output)
+    apply_and_lint(
+        filename,
+        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=disallowed-name")] + args,
+        expected_output
+    )
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("105119-p5_template.py", [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=R1714")], [
         lazy_problem().set_code("R1714").set_line(22)
         .set_text("Consider merging these comparisons with \"in\" to \"i not in '[]'\""),
         lazy_problem().set_code("R1714").set_line(35)
@@ -232,25 +242,29 @@
         create_apply_and_lint(
             lines,
             [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=improve-for-loop")],
             expected_output
         )
 
     @pytest.mark.parametrize("filename,args,expected_output", [
-        ("105119-p5_template.py", [Arg(Option.PYLINT, "--enable=iterate-directly")], [
+        ("105119-p5_template.py", [Arg(Option.PYLINT, "--enable=use-foreach")], [
         ]),
-        ("015080-p4_geometry.py", [Arg(Option.PYLINT, "--enable=iterate-directly"),
+        ("015080-p4_geometry.py", [Arg(Option.PYLINT, "--enable=use-foreach"),
                                    Arg(Option.PYLINT, "--disable=W0622,R1705,R1703,R6201,R6202")], [
         ]),
-        ("014771-p2_nested.py", [Arg(Option.PYTHON_SPECIFIC, "on")], [
+        ("014771-p2_nested.py", [Arg(Option.PYLINT, "--enable=use-foreach")], [
             lazy_problem().set_code("R6101").set_line(25)
             .set_text("Iterate directly: \"for var in A\" (with appropriate name for \"var\")"),
             lazy_problem().set_code("R6101").set_line(35)
             .set_text("Iterate directly: \"for var in A\" (with appropriate name for \"var\")"),
         ]),
+        ("045294-p4_vigenere.py", [Arg(Option.PYLINT, "--enable=use-foreach")], []),
+        ("03-d4_points.py", [Arg(Option.PYLINT, "--enable=improve-for-loop")], [
+            lazy_problem().set_code("R6102").set_line(92)
+        ]),
         ("umime_count_a.py", [Arg(Option.PYLINT, "--enable=improve-for-loop"),
                               Arg(Option.FLAKE8, "--extend-ignore=E225")], [
             lazy_problem().set_code("R6101").set_line(3)
             .set_text("Iterate directly: \"for var in text\" (with appropriate name for \"var\")"),
         ]),
     ])
     def test_improve_for(self, filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
```

### Comparing `edulint-2.5.1/tests/test_main.py` & `edulint-2.6.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/tests/test_short_problems.py` & `edulint-2.6.0/tests/test_short_problems.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
             lazy_problem().set_code("R6612").set_line(30).set_text("Unreachable else."),
             lazy_problem().set_code("R6611").set_line(41).set_text("Use else instead of elif."),
             lazy_problem().set_code("R6612").set_line(44).set_text("Unreachable else."),
         ]),
         ("104174-ipv4_restore.py", [
             lazy_problem().set_code("R6610").set_line(38).set_text("Do not multiply list with mutable content.")
         ]),
+        ("104584-p4_digits.py", []),
         ("hw14358.py", [
             lazy_problem().set_code("R6609").set_line(29).set_text("Use augmenting assignment: 'result -= element'"),
             lazy_problem().set_code("R6609").set_line(31).set_text("Use augmenting assignment: 'b += 1'"),
             lazy_problem().set_code("R6609").set_line(34).set_text("Use augmenting assignment: 'a += 1'"),
             lazy_problem().set_code("R6608").set_line(44).set_text("Redundant arithmetic: num // num"),
             lazy_problem().set_code("R6609").set_line(50).set_text("Use augmenting assignment: 'count += 1'"),
             lazy_problem().set_code("R6609").set_line(51).set_text("Use augmenting assignment: 'number //= n'"),
```

### Comparing `edulint-2.5.1/tests/test_simplifiable_if.py` & `edulint-2.6.0/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.5.1/tests/test_visitors.py` & `edulint-2.6.0/tests/test_visitors.py`

 * *Files identical despite different names*

