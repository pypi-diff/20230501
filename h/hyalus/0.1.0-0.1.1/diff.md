# Comparing `tmp/hyalus-0.1.0.tar.gz` & `tmp/hyalus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyalus-0.1.0.tar", last modified: Mon May  1 16:16:49 2023, max compression
+gzip compressed data, was "hyalus-0.1.1.tar", last modified: Mon May  1 16:41:01 2023, max compression
```

## Comparing `hyalus-0.1.0.tar` & `hyalus-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.709955 hyalus-0.1.0/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1083 2023-04-11 18:36:58.000000 hyalus-0.1.0/LICENSE
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1128 2023-05-01 16:16:49.710042 hyalus-0.1.0/PKG-INFO
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      542 2023-04-13 15:57:22.000000 hyalus-0.1.0/README.md
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     2404 2023-04-26 18:32:57.000000 hyalus-0.1.0/pyproject.toml
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      946 2023-05-01 16:16:49.710376 hyalus-0.1.0/setup.cfg
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.699845 hyalus-0.1.0/src/
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.701742 hyalus-0.1.0/src/hyalus/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      262 2023-04-25 18:14:42.000000 hyalus-0.1.0/src/hyalus/__init__.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.703147 hyalus-0.1.0/src/hyalus/assertions/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       75 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/assertions/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1045 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/assertions/apply.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     4607 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/assertions/compare.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.703486 hyalus-0.1.0/src/hyalus/bin/
--rwxr-xr-x   0 david.mcconnell (1107921037) 11842803    13711 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/bin/hyalus
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.704033 hyalus-0.1.0/src/hyalus/config/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       38 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1851 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/common.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     5108 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/loader.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.704730 hyalus-0.1.0/src/hyalus/config/steps/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      376 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/steps/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     8378 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/steps/assertions.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     5315 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/steps/base.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     4414 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/steps/run.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.705480 hyalus-0.1.0/src/hyalus/config/tags/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      254 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/tags/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1642 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/tags/base.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1906 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/tags/runtime.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1341 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/config/tags/types.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       25 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/metadata.json
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.706692 hyalus-0.1.0/src/hyalus/parse/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       78 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     6432 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/base.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      574 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/csv.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     2000 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/factory.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     3767 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/h5.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1234 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/json.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      576 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/parse/tsv.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803        0 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/py.typed
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.708341 hyalus-0.1.0/src/hyalus/run/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      309 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     3585 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/clean.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803    13824 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/common.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1542 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/list.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     9261 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/python.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     4082 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/runsuite.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     6733 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/runtest.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     9667 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/settings.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.708553 hyalus-0.1.0/src/hyalus/run/static/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      412 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/static/config_template
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     2531 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/run/template.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.708724 hyalus-0.1.0/src/hyalus/settings/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803        0 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/settings/.gitfood
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.709688 hyalus-0.1.0/src/hyalus/utils/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       30 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/utils/__init__.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      992 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/utils/file_utils.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     3149 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/utils/json_utils.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     4930 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/utils/logging_utils.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803      791 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/utils/pandas_utils.py
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     2176 2023-03-29 22:59:25.000000 hyalus-0.1.0/src/hyalus/utils/typing_utils.py
-drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:16:49.702476 hyalus-0.1.0/src/hyalus.egg-info/
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1128 2023-05-01 16:16:49.000000 hyalus-0.1.0/src/hyalus.egg-info/PKG-INFO
--rw-r--r--   0 david.mcconnell (1107921037) 11842803     1458 2023-05-01 16:16:49.000000 hyalus-0.1.0/src/hyalus.egg-info/SOURCES.txt
--rw-r--r--   0 david.mcconnell (1107921037) 11842803        1 2023-05-01 16:16:49.000000 hyalus-0.1.0/src/hyalus.egg-info/dependency_links.txt
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       39 2023-05-01 16:16:49.000000 hyalus-0.1.0/src/hyalus.egg-info/entry_points.txt
--rw-r--r--   0 david.mcconnell (1107921037) 11842803       18 2023-05-01 16:16:49.000000 hyalus-0.1.0/src/hyalus.egg-info/requires.txt
--rw-r--r--   0 david.mcconnell (1107921037) 11842803        7 2023-05-01 16:16:49.000000 hyalus-0.1.0/src/hyalus.egg-info/top_level.txt
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.777418 hyalus-0.1.1/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     5542 2023-04-11 18:36:58.000000 hyalus-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     6280 2023-05-01 16:40:41.000000 hyalus-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803    36615 2023-04-11 18:36:58.000000 hyalus-0.1.1/GETTING_STARTED.md
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1083 2023-04-11 18:36:58.000000 hyalus-0.1.1/LICENSE
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      140 2023-05-01 16:40:41.000000 hyalus-0.1.1/MANIFEST.in
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1128 2023-05-01 16:41:01.777489 hyalus-0.1.1/PKG-INFO
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      542 2023-04-13 15:57:22.000000 hyalus-0.1.1/README.md
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     2404 2023-05-01 16:40:41.000000 hyalus-0.1.1/pyproject.toml
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      946 2023-05-01 16:41:01.777793 hyalus-0.1.1/setup.cfg
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.769873 hyalus-0.1.1/src/
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.771881 hyalus-0.1.1/src/hyalus/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      262 2023-04-25 18:14:42.000000 hyalus-0.1.1/src/hyalus/__init__.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.773028 hyalus-0.1.1/src/hyalus/assertions/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       75 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/assertions/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1045 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/assertions/apply.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     4607 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/assertions/compare.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.773155 hyalus-0.1.1/src/hyalus/bin/
+-rwxr-xr-x   0 david.mcconnell (1107921037) 11842803    13711 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/bin/hyalus
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.773528 hyalus-0.1.1/src/hyalus/config/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       38 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1851 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/common.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     5108 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/loader.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.774012 hyalus-0.1.1/src/hyalus/config/steps/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      376 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/steps/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     8378 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/steps/assertions.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     5315 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/steps/base.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     4414 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/steps/run.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.774592 hyalus-0.1.1/src/hyalus/config/tags/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      254 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/tags/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1642 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/tags/base.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1906 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/tags/runtime.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1341 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/config/tags/types.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       25 2023-05-01 16:40:41.000000 hyalus-0.1.1/src/hyalus/metadata.json
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.775418 hyalus-0.1.1/src/hyalus/parse/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       78 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     6432 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/base.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      574 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/csv.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     2000 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/factory.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     3767 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/h5.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1234 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/json.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      576 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/parse/tsv.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803        0 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/py.typed
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.776450 hyalus-0.1.1/src/hyalus/run/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      309 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     3585 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/clean.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803    13824 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/common.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1542 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/list.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     9261 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/python.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     4082 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/runsuite.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     6733 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/runtest.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     9667 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/settings.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.776560 hyalus-0.1.1/src/hyalus/run/static/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      412 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/static/config_template
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     2531 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/run/template.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.776673 hyalus-0.1.1/src/hyalus/settings/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803        0 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/settings/.gitfood
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.777323 hyalus-0.1.1/src/hyalus/utils/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       30 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/utils/__init__.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      992 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/utils/file_utils.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     3149 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/utils/json_utils.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     4930 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/utils/logging_utils.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803      791 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/utils/pandas_utils.py
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     2176 2023-03-29 22:59:25.000000 hyalus-0.1.1/src/hyalus/utils/typing_utils.py
+drwxr-xr-x   0 david.mcconnell (1107921037) 11842803        0 2023-05-01 16:41:01.772595 hyalus-0.1.1/src/hyalus.egg-info/
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1128 2023-05-01 16:41:01.000000 hyalus-0.1.1/src/hyalus.egg-info/PKG-INFO
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803     1524 2023-05-01 16:41:01.000000 hyalus-0.1.1/src/hyalus.egg-info/SOURCES.txt
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803        1 2023-05-01 16:41:01.000000 hyalus-0.1.1/src/hyalus.egg-info/dependency_links.txt
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       39 2023-05-01 16:41:01.000000 hyalus-0.1.1/src/hyalus.egg-info/entry_points.txt
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803       18 2023-05-01 16:41:01.000000 hyalus-0.1.1/src/hyalus.egg-info/requires.txt
+-rw-r--r--   0 david.mcconnell (1107921037) 11842803        7 2023-05-01 16:41:01.000000 hyalus-0.1.1/src/hyalus.egg-info/top_level.txt
```

### Comparing `hyalus-0.1.0/LICENSE` & `hyalus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/PKG-INFO` & `hyalus-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyalus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test harness and utilities for Sequencing Health software testing
 Author: David McConnell
 Author-email: david.mcconnell@sequencinghealth.com
 Maintainer: David McConnell
 Maintainer-email: david.mcconnell@sequencinghealth.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyalus-0.1.0/README.md` & `hyalus-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/pyproject.toml` & `hyalus-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/setup.cfg` & `hyalus-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/assertions/apply.py` & `hyalus-0.1.1/src/hyalus/assertions/apply.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/assertions/compare.py` & `hyalus-0.1.1/src/hyalus/assertions/compare.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/bin/hyalus` & `hyalus-0.1.1/src/hyalus/bin/hyalus`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/common.py` & `hyalus-0.1.1/src/hyalus/config/common.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/loader.py` & `hyalus-0.1.1/src/hyalus/config/loader.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/steps/assertions.py` & `hyalus-0.1.1/src/hyalus/config/steps/assertions.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/steps/base.py` & `hyalus-0.1.1/src/hyalus/config/steps/base.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/steps/run.py` & `hyalus-0.1.1/src/hyalus/config/steps/run.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/tags/base.py` & `hyalus-0.1.1/src/hyalus/config/tags/base.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/tags/runtime.py` & `hyalus-0.1.1/src/hyalus/config/tags/runtime.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/config/tags/types.py` & `hyalus-0.1.1/src/hyalus/config/tags/types.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/parse/base.py` & `hyalus-0.1.1/src/hyalus/parse/base.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/parse/csv.py` & `hyalus-0.1.1/src/hyalus/parse/csv.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/parse/factory.py` & `hyalus-0.1.1/src/hyalus/parse/factory.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/parse/h5.py` & `hyalus-0.1.1/src/hyalus/parse/h5.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/parse/json.py` & `hyalus-0.1.1/src/hyalus/parse/json.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/parse/tsv.py` & `hyalus-0.1.1/src/hyalus/parse/tsv.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/clean.py` & `hyalus-0.1.1/src/hyalus/run/clean.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/common.py` & `hyalus-0.1.1/src/hyalus/run/common.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/list.py` & `hyalus-0.1.1/src/hyalus/run/list.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/python.py` & `hyalus-0.1.1/src/hyalus/run/python.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/runsuite.py` & `hyalus-0.1.1/src/hyalus/run/runsuite.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/runtest.py` & `hyalus-0.1.1/src/hyalus/run/runtest.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/settings.py` & `hyalus-0.1.1/src/hyalus/run/settings.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/run/template.py` & `hyalus-0.1.1/src/hyalus/run/template.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/utils/file_utils.py` & `hyalus-0.1.1/src/hyalus/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/utils/json_utils.py` & `hyalus-0.1.1/src/hyalus/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/utils/logging_utils.py` & `hyalus-0.1.1/src/hyalus/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/utils/pandas_utils.py` & `hyalus-0.1.1/src/hyalus/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus/utils/typing_utils.py` & `hyalus-0.1.1/src/hyalus/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `hyalus-0.1.0/src/hyalus.egg-info/PKG-INFO` & `hyalus-0.1.1/src/hyalus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyalus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test harness and utilities for Sequencing Health software testing
 Author: David McConnell
 Author-email: david.mcconnell@sequencinghealth.com
 Maintainer: David McConnell
 Maintainer-email: david.mcconnell@sequencinghealth.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyalus-0.1.0/src/hyalus.egg-info/SOURCES.txt` & `hyalus-0.1.1/src/hyalus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
+GETTING_STARTED.md
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/hyalus/__init__.py
 src/hyalus/metadata.json
 src/hyalus/py.typed
 src/hyalus.egg-info/PKG-INFO
```

