# Comparing `tmp/carrot-cdm-0.6.8.tar.gz` & `tmp/carrot-cdm-0.6.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrot-cdm-0.6.8.tar", last modified: Tue Apr 18 07:23:55 2023, max compression
+gzip compressed data, was "carrot-cdm-0.6.85.tar", last modified: Mon May  1 14:55:32 2023, max compression
```

## Comparing `carrot-cdm-0.6.8.tar` & `carrot-cdm-0.6.85.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/analyses/example_serology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/objects/versions/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/death.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/specimen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/display.py
--rw-r--r--   0 runner    (1001) docker     (123)    41561 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/pseudonymise.py
--rw-r--r--   0 runner    (1001) docker     (123)    44828 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/io/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/bclink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/bash_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/bclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/tools/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/extract/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/mappingrules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/omopcdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/rules_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot_cdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.868241 carrot-cdm-0.6.85/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-01 14:55:32.868241 carrot-cdm-0.6.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.856241 carrot-cdm-0.6.85/carrot/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.856241 carrot-cdm-0.6.85/carrot/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/analyses/example_serology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.860241 carrot-cdm-0.6.85/carrot/cdm/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.860241 carrot-cdm-0.6.85/carrot/cdm/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.860241 carrot-cdm-0.6.85/carrot/cdm/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.860241 carrot-cdm-0.6.85/carrot/cdm/objects/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.860241 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/death.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/specimen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cdm/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.860241 carrot-cdm-0.6.85/carrot/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.864241 carrot-cdm-0.6.85/carrot/cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41561 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/pseudonymise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/cli/subcommands/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.864241 carrot-cdm-0.6.85/carrot/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/io/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.864241 carrot-cdm-0.6.85/carrot/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/io/plugins/bclink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/io/plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/io/plugins/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.864241 carrot-cdm-0.6.85/carrot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/bash_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/bclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.864241 carrot-cdm-0.6.85/carrot/tools/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/extract/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/mappingrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/omopcdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot/tools/rules_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:55:32.868241 carrot-cdm-0.6.85/carrot_cdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot_cdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot_cdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot_cdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot_cdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot_cdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/carrot_cdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:55:32.868241 carrot-cdm-0.6.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-01 14:55:32.000000 carrot-cdm-0.6.85/setup.py
```

### Comparing `carrot-cdm-0.6.8/LICENSE` & `carrot-cdm-0.6.85/LICENSE`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/PKG-INFO` & `carrot-cdm-0.6.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.6.8
+Version: 0.6.85
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: calmacx@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.6.8/carrot/analyses/example_serology.py` & `carrot-cdm-0.6.85/carrot/analyses/example_serology.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/__init__.py` & `carrot-cdm-0.6.85/carrot/cdm/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/decorators.py` & `carrot-cdm-0.6.85/carrot/cdm/decorators.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/model.py` & `carrot-cdm-0.6.85/carrot/cdm/model.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/__init__.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/common.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/death.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/death.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/measurement.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/measurement.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/observation.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/observation.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/person.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/person.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/specimen.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/specimen.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py` & `carrot-cdm-0.6.85/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cdm/operations.py` & `carrot-cdm-0.6.85/carrot/cdm/operations.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/cli.py` & `carrot-cdm-0.6.85/carrot/cli/cli.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/airflow.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/airflow.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/display.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/display.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/etl.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/etl.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/generate.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/generate.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/get.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/get.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/info.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/pseudonymise.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/pseudonymise.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/run.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import csv
 import inspect
 import os, time
 import datetime
 import fnmatch
 import sys
 import click
 import json
@@ -681,37 +682,38 @@
     for srcfilename in input_files:
         outcounts = {}
         rejcounts = {}
         rcount = 0
 
         try:
             fh = open(input_dir[0] + "/" + srcfilename, mode='r')
+            csvr = csv.reader(fh)
         except IOError as e:
             print("I/O error({0}): {1}".format(e.errno, e.strerror))
             exit()
 
         tgtfiles, src_to_tgt = mappingrules.parse_rules_src_to_tgt(srcfilename)
         infile_datetime_source, infile_person_id_source = mappingrules.get_infile_date_person_id(srcfilename)
         for tgtfile in tgtfiles:
             outcounts[tgtfile] = 0
             rejcounts[tgtfile] = 0
         datacolsall = []
-        hdrdata = fh.readline().strip().split(",")
+        hdrdata = next(csvr)
         dflist = mappingrules.get_infile_data_fields(srcfilename)
         for colname in hdrdata:
             datacolsall.append(colname)
         inputcolmap = omopcdm.get_column_map(hdrdata)
         pers_id_col = inputcolmap[infile_person_id_source]
         datetime_col = inputcolmap[infile_datetime_source]
         print("--------------------------------------------------------------------------------")
         print("Processing input: {0}".format(srcfilename))
 #        print("Processing input: {0}, All input cols = {1}, Data cols = {2}".format(srcfilename, str(datacolsall), str(dflist)))
 
-        for inputline in fh:
-            indata = inputline.strip().split(",")
+        for indata in csvr:
+            #indata = inputline.strip().split(",")
             key = srcfilename + "~all~all"
             metrics.increment_key_count(key, "input_count")
             rcount += 1
             strdate = indata[datetime_col].split(" ")[0]
             fulldate = parse_date(strdate)
             if fulldate != None:
                 #fulldate = "{0}-{1:02}-{2:02}".format(dt.year, dt.month, dt.day)
@@ -734,14 +736,15 @@
 
                 for datacol in datacols:
                     built_records, outrecords, metrics = get_target_records(tgtfile, tgtcolmap, src_to_tgt, datacol, indata, inputcolmap, srcfilename, date_col_data, date_component_data, metrics)
                     if built_records == True:
                         for outrecord in outrecords:
                             if auto_num_col != None:
                                 outrecord[tgtcolmap[auto_num_col]] = str(record_numbers[tgtfile])
+                                record_numbers[tgtfile] += 1
                             if (outrecord[tgtcolmap[pers_id_col]]) in person_lookup:
                                 outrecord[tgtcolmap[pers_id_col]] = person_lookup[outrecord[tgtcolmap[pers_id_col]]]
                                 outcounts[tgtfile] += 1
                                 key = srcfilename + "~all~all"
                                 metrics.increment_key_count(key, "output_count")
                                 key = "all~" + tgtfile + "~all"
                                 metrics.increment_key_count(key, "output_count")
```

### Comparing `carrot-cdm-0.6.8/carrot/cli/subcommands/search.py` & `carrot-cdm-0.6.85/carrot/cli/subcommands/search.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/io/common.py` & `carrot-cdm-0.6.85/carrot/io/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/io/plugins/bclink.py` & `carrot-cdm-0.6.85/carrot/io/plugins/bclink.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/io/plugins/local.py` & `carrot-cdm-0.6.85/carrot/io/plugins/local.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/io/plugins/sql.py` & `carrot-cdm-0.6.85/carrot/io/plugins/sql.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/__init__.py` & `carrot-cdm-0.6.85/carrot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/bash_helpers.py` & `carrot-cdm-0.6.85/carrot/tools/bash_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/bclink_helpers.py` & `carrot-cdm-0.6.85/carrot/tools/bclink_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/dag.py` & `carrot-cdm-0.6.85/carrot/tools/dag.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/extract/__init__.py` & `carrot-cdm-0.6.85/carrot/tools/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/extract/templates.py` & `carrot-cdm-0.6.85/carrot/tools/extract/templates.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/file_helpers.py` & `carrot-cdm-0.6.85/carrot/tools/file_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/logger.py` & `carrot-cdm-0.6.85/carrot/tools/logger.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/mappingrules.py` & `carrot-cdm-0.6.85/carrot/tools/mappingrules.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/metrics.py` & `carrot-cdm-0.6.85/carrot/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/omopcdm.py` & `carrot-cdm-0.6.85/carrot/tools/omopcdm.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/profiling.py` & `carrot-cdm-0.6.85/carrot/tools/profiling.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot/tools/rules_helpers.py` & `carrot-cdm-0.6.85/carrot/tools/rules_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/carrot_cdm.egg-info/PKG-INFO` & `carrot-cdm-0.6.85/carrot_cdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.6.8
+Version: 0.6.85
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: calmacx@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.6.8/carrot_cdm.egg-info/SOURCES.txt` & `carrot-cdm-0.6.85/carrot_cdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.8/setup.py` & `carrot-cdm-0.6.85/setup.py`

 * *Files identical despite different names*

