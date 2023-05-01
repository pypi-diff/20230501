# Comparing `tmp/optuna-distributed-0.4.0.tar.gz` & `tmp/optuna-distributed-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-distributed-0.4.0.tar", last modified: Wed Jan 25 20:07:27 2023, max compression
+gzip compressed data, was "optuna-distributed-0.5.0.tar", last modified: Mon May  1 11:53:50 2023, max compression
```

## Comparing `optuna-distributed-0.4.0.tar` & `optuna-distributed-0.5.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.823846 optuna-distributed-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.823846 optuna-distributed-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.github/ISSUE_TEMPLATE/general-question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.823846 optuna-distributed-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.github/workflows/format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.823846 optuna-distributed-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/examples/quadratic_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/examples/simple_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/examples/simple_storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.823846 optuna-distributed-0.4.0/optuna_distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/eventloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/optuna_distributed/ipc/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/ipc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/ipc/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/ipc/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/optuna_distributed/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/managers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/managers/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/optuna_distributed/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/completed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/failed.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/pruned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/setattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/shouldprune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/messages/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/optuna_distributed/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.823846 optuna-distributed-0.4.0/optuna_distributed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-01-25 20:07:27.000000 optuna-distributed-0.4.0/optuna_distributed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-01-25 20:07:27.000000 optuna-distributed-0.4.0/optuna_distributed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:07:27.000000 optuna-distributed-0.4.0/optuna_distributed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-25 20:07:27.000000 optuna-distributed-0.4.0/optuna_distributed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-25 20:07:27.000000 optuna-distributed-0.4.0/optuna_distributed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:27.827846 optuna-distributed-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/test_ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-01-25 20:07:16.000000 optuna-distributed-0.4.0/tests/test_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/general-question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/workflows/format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/disable_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/quadratic_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/simple_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/simple_storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/optuna_distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/eventloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed/ipc/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/pruned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/setattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/shouldprune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 11:53:50.488776 optuna-distributed-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_trial.py
```

### Comparing `optuna-distributed-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/.github/workflows/format.yaml` & `optuna-distributed-0.5.0/.github/workflows/format.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/.github/workflows/release.yaml` & `optuna-distributed-0.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/.github/workflows/test.yaml` & `optuna-distributed-0.5.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/.gitignore` & `optuna-distributed-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/LICENSE` & `optuna-distributed-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/PKG-INFO` & `optuna-distributed-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.4.0
+Version: 0.5.0
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `optuna-distributed-0.4.0/README.md` & `optuna-distributed-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/examples/quadratic_simple.py` & `optuna-distributed-0.5.0/examples/quadratic_simple.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/examples/simple_pruning.py` & `optuna-distributed-0.5.0/examples/simple_pruning.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/examples/simple_storages.py` & `optuna-distributed-0.5.0/examples/simple_storages.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/eventloop.py` & `optuna-distributed-0.5.0/optuna_distributed/eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/ipc/base.py` & `optuna-distributed-0.5.0/optuna_distributed/ipc/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/ipc/pipe.py` & `optuna-distributed-0.5.0/optuna_distributed/ipc/pipe.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/ipc/queue.py` & `optuna-distributed-0.5.0/optuna_distributed/ipc/queue.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/managers/__init__.py` & `optuna-distributed-0.5.0/optuna_distributed/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/managers/base.py` & `optuna-distributed-0.5.0/optuna_distributed/managers/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/managers/distributed.py` & `optuna-distributed-0.5.0/optuna_distributed/managers/distributed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/managers/local.py` & `optuna-distributed-0.5.0/optuna_distributed/managers/local.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/__init__.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/base.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/completed.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/completed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/failed.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/failed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/heartbeat.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/property.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/property.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/pruned.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/pruned.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/report.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/report.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/response.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/response.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/setattr.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/setattr.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/shouldprune.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/shouldprune.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/messages/suggest.py` & `optuna-distributed-0.5.0/optuna_distributed/messages/suggest.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/study.py` & `optuna-distributed-0.5.0/optuna_distributed/study.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/terminal.py` & `optuna-distributed-0.5.0/optuna_distributed/terminal.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed/trial.py` & `optuna-distributed-0.5.0/optuna_distributed/trial.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/optuna_distributed.egg-info/PKG-INFO` & `optuna-distributed-0.5.0/optuna_distributed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.4.0
+Version: 0.5.0
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `optuna-distributed-0.4.0/optuna_distributed.egg-info/SOURCES.txt` & `optuna-distributed-0.5.0/optuna_distributed.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 setup.cfg
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/general-question.md
 .github/workflows/format.yaml
 .github/workflows/release.yaml
 .github/workflows/test.yaml
+examples/disable_logging.py
 examples/quadratic_simple.py
 examples/simple_pruning.py
 examples/simple_storages.py
 optuna_distributed/__init__.py
+optuna_distributed/config.py
 optuna_distributed/eventloop.py
 optuna_distributed/study.py
 optuna_distributed/terminal.py
 optuna_distributed/trial.py
 optuna_distributed.egg-info/PKG-INFO
 optuna_distributed.egg-info/SOURCES.txt
 optuna_distributed.egg-info/dependency_links.txt
```

### Comparing `optuna-distributed-0.4.0/pyproject.toml` & `optuna-distributed-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 [tool.setuptools.dynamic]
 version = { attr = "optuna_distributed.__version__" }
 readme = { file = "README.md" }
 
 [tool.black]
 line-length = 99
-target-version = ["py38"]
+target-version = ["py310"]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.mypy_cache
   | \.vscode
   | env
```

### Comparing `optuna-distributed-0.4.0/tests/test_eventloop.py` & `optuna-distributed-0.5.0/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/tests/test_ipc.py` & `optuna-distributed-0.5.0/tests/test_ipc.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.4.0/tests/test_managers.py` & `optuna-distributed-0.5.0/tests/test_managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 
         if manager.should_end_optimization():
             break
 
     assert closing_messages_recieved == n_trials
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="Requires Python 3.8 or higher")
-def test_distributed_stops_optimziation(client: Client) -> None:
+def test_distributed_stops_optimization(client: Client) -> None:
     uninterrupted_execution_time = 100
 
     def _objective(trial: DistributedTrial) -> float:
         # Sleep needs to be fragemnted to read error indicator.
         for _ in range(uninterrupted_execution_time):
             time.sleep(1.0)
         return 0.0
@@ -88,17 +87,14 @@
     stopped_at = time.time()
     manager.stop_optimization(patience=10.0)
     interrupted_execution_time = time.time() - stopped_at
     assert interrupted_execution_time < uninterrupted_execution_time
     for future in manager._futures:
         assert future.cancelled()
 
-    for task_state in manager._synchronizer._task_states:
-        assert _TaskState(task_state.get()) is not _TaskState.RUNNING
-
 
 def test_distributed_connection_management(client: Client) -> None:
     def _objective(trial: DistributedTrial) -> float:
         requested = trial.connection.get()
         assert isinstance(requested, ResponseMessage)
         data = {"requested": requested.data, "actual": trial.trial_id}
         trial.connection.put(ResponseMessage(trial.trial_id, data))
```

### Comparing `optuna-distributed-0.4.0/tests/test_messages.py` & `optuna-distributed-0.5.0/tests/test_messages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from contextlib import contextmanager
 import logging
 from typing import Any
 from typing import Generator
 from unittest.mock import MagicMock
 
 from optuna.distributions import BaseDistribution
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.exceptions import TrialPruned
 from optuna.study import Study
 from optuna.trial import TrialState
 import pytest
 
+import optuna_distributed
 from optuna_distributed.eventloop import EventLoop
 from optuna_distributed.ipc import IPCPrimitive
 from optuna_distributed.managers import ObjectiveFuncType
 from optuna_distributed.managers import OptimizationManager
 from optuna_distributed.messages import CompletedMessage
 from optuna_distributed.messages import FailedMessage
 from optuna_distributed.messages import HeartbeatMessage
@@ -76,24 +78,35 @@
 
 
 @pytest.fixture
 def manager() -> MockOptimizationManager:
     return MockOptimizationManager()
 
 
+@contextmanager
+def _forced_log_propagation(logger_name: str) -> Generator[None, None, None]:
+    try:
+        # Local fix for https://github.com/pytest-dev/pytest/issues/3697
+        logging.getLogger(logger_name).propagate = True
+        yield
+    finally:
+        logging.getLogger(logger_name).propagate = False
+
+
 def _message_responds_with(value: Any, manager: MockOptimizationManager) -> bool:
     return manager.message_response == value
 
 
 def test_completed_with_correct_value(
     study: Study, manager: MockOptimizationManager, caplog: pytest.LogCaptureFixture
 ) -> None:
     msg = CompletedMessage(0, 0.0)
     assert msg.closing
-    msg.process(study, manager)
+    with _forced_log_propagation(logger_name=optuna_distributed.__name__):
+        msg.process(study, manager)
     assert manager.trial_exit_called
     assert len(caplog.records) == 1
     assert caplog.records[0].levelno == logging.INFO
     trial = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
     assert len(trial) == 1
     assert trial[0].value == 0.0
 
@@ -107,31 +120,32 @@
 
 
 def test_pruned(
     study: Study, manager: MockOptimizationManager, caplog: pytest.LogCaptureFixture
 ) -> None:
     msg = PrunedMessage(0, TrialPruned())
     assert msg.closing
-    msg.process(study, manager)
+    with _forced_log_propagation(logger_name=optuna_distributed.__name__):
+        msg.process(study, manager)
     assert manager.trial_exit_called
     assert len(caplog.records) == 1
     assert caplog.records[0].levelno == logging.INFO
     trial = study.get_trials(deepcopy=False, states=(TrialState.PRUNED,))
     assert len(trial) == 1
 
 
 def test_failed(
     study: Study, manager: MockOptimizationManager, caplog: pytest.LogCaptureFixture
 ) -> None:
     exc = ValueError("foo")
     msg = FailedMessage(0, exc, exc_info=MagicMock())
     assert msg.closing
-    with pytest.raises(ValueError):
+    logger_name = optuna_distributed.__name__
+    with pytest.raises(ValueError), _forced_log_propagation(logger_name):
         msg.process(study, manager)
-
     assert manager.trial_exit_called
     assert len(caplog.records) == 1
     assert caplog.records[0].levelno == logging.WARNING
     trial = study.get_trials(deepcopy=False, states=(TrialState.FAIL,))
     assert len(trial) == 1
```

### Comparing `optuna-distributed-0.4.0/tests/test_trial.py` & `optuna-distributed-0.5.0/tests/test_trial.py`

 * *Files identical despite different names*

