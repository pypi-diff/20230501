# Comparing `tmp/nutra-0.2.7.dev2.tar.gz` & `tmp/nutra-0.2.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutra-0.2.7.dev2.tar", last modified: Mon Mar 27 03:16:20 2023, max compression
+gzip compressed data, was "nutra-0.2.7.dev3.tar", last modified: Sat Apr  1 00:01:29 2023, max compression
```

## Comparing `nutra-0.2.7.dev2.tar` & `nutra-0.2.7.dev3.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.998526 nutra-0.2.7.dev2/
--rw-rw-r--   0 shane     (1000) shane     (1000)    35149 2022-06-25 20:31:39.000000 nutra-0.2.7.dev2/LICENSE
--rw-rw-r--   0 shane     (1000) shane     (1000)      258 2023-03-27 00:31:14.000000 nutra-0.2.7.dev2/MANIFEST.in
--rw-rw-r--   0 shane     (1000) shane     (1000)     9510 2023-03-27 03:16:19.998526 nutra-0.2.7.dev2/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     8034 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/README.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3025 2023-03-27 03:16:16.000000 nutra-0.2.7.dev2/ntclient/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4000 2023-03-27 03:08:49.000000 nutra-0.2.7.dev2/ntclient/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/argparser/
--rw-rw-r--   0 shane     (1000) shane     (1000)    10772 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/ntclient/argparser/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     9943 2023-03-27 03:14:02.000000 nutra-0.2.7.dev2/ntclient/argparser/funcs.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      622 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/argparser/types.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/core/
--rw-r--r--   0 shane     (1000) shane     (1000)        0 2022-04-10 22:14:58.000000 nutra-0.2.7.dev2/ntclient/core/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      404 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/core/nnest.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      189 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/core/nnr2.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1166 2023-03-26 21:17:21.000000 nutra-0.2.7.dev2/ntclient/core/nutprogbar.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/models/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1752 2023-03-27 03:11:04.000000 nutra-0.2.7.dev2/ntclient/models/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/ntsqlite/
--rw-rw-r--   0 shane     (1000) shane     (1000)      137 2023-03-26 15:43:10.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/
--rwxrwxr-x   0 shane     (1000) shane     (1000)     1849 2023-03-26 21:17:25.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      156 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/
--rw-rw-r--   0 shane     (1000) shane     (1000)       31 2022-07-12 18:26:52.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/bf_eq.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)       74 2022-07-12 18:26:52.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/bmr_eq.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      102 2022-07-10 22:12:56.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/meal_name.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      761 2022-07-10 22:12:56.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/rda.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      330 2023-03-26 15:43:10.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/version.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      690 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/functions.sql
--rw-rw-r--   0 shane     (1000) shane     (1000)     6566 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/ntsqlite/sql/tables.sql
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/persistence/
--rw-rw-r--   0 shane     (1000) shane     (1000)      218 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/persistence/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/persistence/sql/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3320 2023-03-27 03:14:02.000000 nutra-0.2.7.dev2/ntclient/persistence/sql/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/persistence/sql/nt/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3110 2023-03-26 21:17:21.000000 nutra-0.2.7.dev2/ntclient/persistence/sql/nt/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      301 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/persistence/sql/nt/funcs.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/persistence/sql/usda/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5053 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/ntclient/persistence/sql/usda/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3858 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/ntclient/persistence/sql/usda/funcs.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.990526 nutra-0.2.7.dev2/ntclient/resources/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.990526 nutra-0.2.7.dev2/ntclient/resources/recipe/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/resources/recipe/dinner/
--rw-rw-r--   0 shane     (1000) shane     (1000)      607 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/dinner/burrito-bowl.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      463 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/dinner/grass-fed-burger.csv
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/resources/recipe/snack/
--rw-rw-r--   0 shane     (1000) shane     (1000)      219 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/snack/baked-potato-wedges.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      642 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/snack/buckwheat-pancake.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      503 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/snack/fruit-smoothie.csv
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/resources/recipe/tmp/
--rw-rw-r--   0 shane     (1000) shane     (1000)      947 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/tmp/food_amounts.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      142 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/tmp/names.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)       34 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/resources/recipe/tmp/servings.csv
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/services/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1295 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/services/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    12484 2023-03-27 03:11:04.000000 nutra-0.2.7.dev2/ntclient/services/analyze.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    13935 2023-03-27 03:11:04.000000 nutra-0.2.7.dev2/ntclient/services/calculate.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/services/recipe/
--rw-rw-r--   0 shane     (1000) shane     (1000)      293 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/services/recipe/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      946 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/ntclient/services/recipe/csv_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2228 2023-03-26 23:18:54.000000 nutra-0.2.7.dev2/ntclient/services/recipe/utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8159 2023-03-27 03:11:04.000000 nutra-0.2.7.dev2/ntclient/services/usda.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.994526 nutra-0.2.7.dev2/ntclient/utils/
--rw-rw-r--   0 shane     (1000) shane     (1000)     4578 2023-03-27 03:07:39.000000 nutra-0.2.7.dev2/ntclient/utils/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      808 2023-03-27 03:13:57.000000 nutra-0.2.7.dev2/ntclient/utils/colors.py
--rw-r--r--   0 shane     (1000) shane     (1000)      574 2022-06-25 21:41:37.000000 nutra-0.2.7.dev2/ntclient/utils/exceptions.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3272 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/ntclient/utils/tree.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.998526 nutra-0.2.7.dev2/nutra.egg-info/
--rw-rw-r--   0 shane     (1000) shane     (1000)     9510 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     1892 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/SOURCES.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/dependency_links.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)       50 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/entry_points.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/not-zip-safe
--rw-rw-r--   0 shane     (1000) shane     (1000)      122 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/requires.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        9 2023-03-27 03:16:19.000000 nutra-0.2.7.dev2/nutra.egg-info/top_level.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)       69 2023-03-27 02:46:53.000000 nutra-0.2.7.dev2/requirements-old.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)       27 2023-03-26 23:18:56.000000 nutra-0.2.7.dev2/requirements-optional.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)       95 2023-03-27 02:42:06.000000 nutra-0.2.7.dev2/requirements.txt
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-03-27 03:16:19.998526 nutra-0.2.7.dev2/scripts/
--rwxrwxr-x   0 shane     (1000) shane     (1000)      286 2023-03-27 00:21:10.000000 nutra-0.2.7.dev2/scripts/n
--rw-rw-r--   0 shane     (1000) shane     (1000)      961 2023-03-27 03:16:19.998526 nutra-0.2.7.dev2/setup.cfg
--rw-rw-r--   0 shane     (1000) shane     (1000)     2752 2023-03-27 00:29:46.000000 nutra-0.2.7.dev2/setup.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.530451 nutra-0.2.7.dev3/
+-rw-rw-r--   0 shane     (1000) shane     (1000)    35149 2022-06-25 20:31:39.000000 nutra-0.2.7.dev3/LICENSE
+-rw-rw-r--   0 shane     (1000) shane     (1000)      258 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/MANIFEST.in
+-rw-rw-r--   0 shane     (1000) shane     (1000)     9533 2023-04-01 00:01:29.530451 nutra-0.2.7.dev3/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8034 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/README.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3025 2023-04-01 00:01:19.000000 nutra-0.2.7.dev3/ntclient/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4000 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/argparser/
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10770 2023-03-30 20:56:20.000000 nutra-0.2.7.dev3/ntclient/argparser/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     9943 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/argparser/funcs.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      622 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/argparser/types.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/core/
+-rw-r--r--   0 shane     (1000) shane     (1000)        0 2022-04-10 22:14:58.000000 nutra-0.2.7.dev3/ntclient/core/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      404 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/core/nnest.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      189 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/core/nnr2.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1166 2023-03-26 21:17:21.000000 nutra-0.2.7.dev3/ntclient/core/nutprogbar.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/models/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1752 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/models/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/ntsqlite/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      137 2023-03-26 15:43:10.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/
+-rwxrwxr-x   0 shane     (1000) shane     (1000)     1849 2023-03-26 21:17:25.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      156 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/
+-rw-rw-r--   0 shane     (1000) shane     (1000)       31 2022-07-12 18:26:52.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/bf_eq.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)       74 2022-07-12 18:26:52.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/bmr_eq.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      102 2022-07-10 22:12:56.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/meal_name.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      761 2022-07-10 22:12:56.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/rda.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      330 2023-03-26 15:43:10.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/version.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      690 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/functions.sql
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6566 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/ntsqlite/sql/tables.sql
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/persistence/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      218 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/persistence/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/persistence/sql/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3320 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/persistence/sql/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/persistence/sql/nt/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3110 2023-03-26 21:17:21.000000 nutra-0.2.7.dev3/ntclient/persistence/sql/nt/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      301 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/persistence/sql/nt/funcs.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/persistence/sql/usda/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5053 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/persistence/sql/usda/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3858 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/persistence/sql/usda/funcs.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/resources/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.522451 nutra-0.2.7.dev3/ntclient/resources/recipe/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/resources/recipe/dinner/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      607 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/dinner/burrito-bowl.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      463 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/dinner/grass-fed-burger.csv
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/resources/recipe/snack/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      219 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/snack/baked-potato-wedges.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      642 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/snack/buckwheat-pancake.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      503 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/snack/fruit-smoothie.csv
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/resources/recipe/tmp/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      947 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/tmp/food_amounts.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      142 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/tmp/names.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)       34 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/resources/recipe/tmp/servings.csv
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/services/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1295 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/services/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    12484 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/services/analyze.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    13935 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/services/calculate.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/services/recipe/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      293 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/services/recipe/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      946 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/services/recipe/csv_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2228 2023-03-26 23:18:54.000000 nutra-0.2.7.dev3/ntclient/services/recipe/utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8159 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/services/usda.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.526451 nutra-0.2.7.dev3/ntclient/utils/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4578 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/utils/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      808 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/utils/colors.py
+-rw-r--r--   0 shane     (1000) shane     (1000)      574 2022-06-25 21:41:37.000000 nutra-0.2.7.dev3/ntclient/utils/exceptions.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3272 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/ntclient/utils/tree.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.530451 nutra-0.2.7.dev3/nutra.egg-info/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     9533 2023-04-01 00:01:29.000000 nutra-0.2.7.dev3/nutra.egg-info/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1910 2023-04-01 00:01:29.000000 nutra-0.2.7.dev3/nutra.egg-info/SOURCES.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-04-01 00:01:29.000000 nutra-0.2.7.dev3/nutra.egg-info/dependency_links.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)       50 2023-04-01 00:01:29.000000 nutra-0.2.7.dev3/nutra.egg-info/entry_points.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-03-31 18:26:45.000000 nutra-0.2.7.dev3/nutra.egg-info/not-zip-safe
+-rw-rw-r--   0 shane     (1000) shane     (1000)      132 2023-04-01 00:01:29.000000 nutra-0.2.7.dev3/nutra.egg-info/requires.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        9 2023-04-01 00:01:29.000000 nutra-0.2.7.dev3/nutra.egg-info/top_level.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)       69 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/requirements-old.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)       27 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/requirements-optional.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)       95 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/requirements.txt
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.530451 nutra-0.2.7.dev3/scripts/
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      286 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/scripts/n
+-rw-rw-r--   0 shane     (1000) shane     (1000)      961 2023-04-01 00:01:29.530451 nutra-0.2.7.dev3/setup.cfg
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2588 2023-03-31 20:25:22.000000 nutra-0.2.7.dev3/setup.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-04-01 00:01:29.530451 nutra-0.2.7.dev3/tests/
+-rw-rw-r--   0 shane     (1000) shane     (1000)    15727 2023-03-27 20:47:24.000000 nutra-0.2.7.dev3/tests/test_cli.py
```

### Comparing `nutra-0.2.7.dev2/LICENSE` & `nutra-0.2.7.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/PKG-INFO` & `nutra-0.2.7.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutra
-Version: 0.2.7.dev2
+Version: 0.2.7.dev3
 Summary: Home and office nutrient tracking software
 Home-page: https://github.com/nutratech/cli
 Author: Shane Jaroch
 Author-email: chown_tee@proton.me
 License: GPL v3
 Platform: linux
 Platform: darwin
@@ -29,14 +29,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Unix Shell
 Requires-Python: >=3.4.3
 Description-Content-Type: text/x-rst
+Provides-Extra: extras
 License-File: LICENSE
 
 ********************
  nutratracker (cli)
 ********************
 
 Command line tools for interacting with government food database,
```

### Comparing `nutra-0.2.7.dev2/README.rst` & `nutra-0.2.7.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/__init__.py` & `nutra-0.2.7.dev3/ntclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import shutil
 import sys
 
 from ntclient.ntsqlite.sql import NT_DB_NAME
 
 # Package info
 __title__ = "nutra"
-__version__ = "0.2.7.dev2"
+__version__ = "0.2.7.dev3"
 __author__ = "Shane Jaroch"
 __email__ = "chown_tee@proton.me"
 __license__ = "GPL v3"
 __copyright__ = "Copyright 2018-2022 Shane Jaroch"
 __url__ = "https://github.com/nutratech/cli"
 
 # Sqlite target versions
```

### Comparing `nutra-0.2.7.dev2/ntclient/__main__.py` & `nutra-0.2.7.dev3/ntclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/argparser/__init__.py` & `nutra-0.2.7.dev3/ntclient/argparser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 def build_calc_subcommand(subparsers: argparse._SubParsersAction) -> None:
     """BMR, 1 rep-max, and other calculators"""
 
     calc_parser = subparsers.add_parser(
         "calc", help="calculate 1-rep max, body fat, BMR, etc."
     )
 
-    calc_subparsers = calc_parser.add_subparsers(title="recipe subcommands")
+    calc_subparsers = calc_parser.add_subparsers(title="calc subcommands")
     calc_parser.set_defaults(func=calc_parser.print_help)
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     # 1-rep max
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     calc_1rm_parser = calc_subparsers.add_parser(
         "1rm", help="calculate 1 rep maxes, by different equations"
```

### Comparing `nutra-0.2.7.dev2/ntclient/argparser/funcs.py` & `nutra-0.2.7.dev3/ntclient/argparser/funcs.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/argparser/types.py` & `nutra-0.2.7.dev3/ntclient/argparser/types.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/core/nutprogbar.py` & `nutra-0.2.7.dev3/ntclient/core/nutprogbar.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/models/__init__.py` & `nutra-0.2.7.dev3/ntclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/ntsqlite/sql/__init__.py` & `nutra-0.2.7.dev3/ntclient/ntsqlite/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/ntsqlite/sql/data/rda.csv` & `nutra-0.2.7.dev3/ntclient/ntsqlite/sql/data/rda.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/ntsqlite/sql/functions.sql` & `nutra-0.2.7.dev3/ntclient/ntsqlite/sql/functions.sql`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/ntsqlite/sql/tables.sql` & `nutra-0.2.7.dev3/ntclient/ntsqlite/sql/tables.sql`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/persistence/sql/__init__.py` & `nutra-0.2.7.dev3/ntclient/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/persistence/sql/nt/__init__.py` & `nutra-0.2.7.dev3/ntclient/persistence/sql/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/persistence/sql/usda/__init__.py` & `nutra-0.2.7.dev3/ntclient/persistence/sql/usda/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/persistence/sql/usda/funcs.py` & `nutra-0.2.7.dev3/ntclient/persistence/sql/usda/funcs.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/resources/recipe/dinner/burrito-bowl.csv` & `nutra-0.2.7.dev3/ntclient/resources/recipe/dinner/burrito-bowl.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/resources/recipe/snack/buckwheat-pancake.csv` & `nutra-0.2.7.dev3/ntclient/resources/recipe/snack/buckwheat-pancake.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/resources/recipe/tmp/food_amounts.csv` & `nutra-0.2.7.dev3/ntclient/resources/recipe/tmp/food_amounts.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/services/__init__.py` & `nutra-0.2.7.dev3/ntclient/services/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/services/analyze.py` & `nutra-0.2.7.dev3/ntclient/services/analyze.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/services/calculate.py` & `nutra-0.2.7.dev3/ntclient/services/calculate.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/services/recipe/csv_utils.py` & `nutra-0.2.7.dev3/ntclient/services/recipe/csv_utils.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/services/recipe/utils.py` & `nutra-0.2.7.dev3/ntclient/services/recipe/utils.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/services/usda.py` & `nutra-0.2.7.dev3/ntclient/services/usda.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/utils/__init__.py` & `nutra-0.2.7.dev3/ntclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/utils/colors.py` & `nutra-0.2.7.dev3/ntclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/utils/exceptions.py` & `nutra-0.2.7.dev3/ntclient/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/ntclient/utils/tree.py` & `nutra-0.2.7.dev3/ntclient/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/nutra.egg-info/PKG-INFO` & `nutra-0.2.7.dev3/nutra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutra
-Version: 0.2.7.dev2
+Version: 0.2.7.dev3
 Summary: Home and office nutrient tracking software
 Home-page: https://github.com/nutratech/cli
 Author: Shane Jaroch
 Author-email: chown_tee@proton.me
 License: GPL v3
 Platform: linux
 Platform: darwin
@@ -29,14 +29,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Unix Shell
 Requires-Python: >=3.4.3
 Description-Content-Type: text/x-rst
+Provides-Extra: extras
 License-File: LICENSE
 
 ********************
  nutratracker (cli)
 ********************
 
 Command line tools for interacting with government food database,
```

### Comparing `nutra-0.2.7.dev2/nutra.egg-info/SOURCES.txt` & `nutra-0.2.7.dev3/nutra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,8 +54,9 @@
 nutra.egg-info/PKG-INFO
 nutra.egg-info/SOURCES.txt
 nutra.egg-info/dependency_links.txt
 nutra.egg-info/entry_points.txt
 nutra.egg-info/not-zip-safe
 nutra.egg-info/requires.txt
 nutra.egg-info/top_level.txt
-scripts/n
+scripts/n
+tests/test_cli.py
```

### Comparing `nutra-0.2.7.dev2/setup.cfg` & `nutra-0.2.7.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `nutra-0.2.7.dev2/setup.py` & `nutra-0.2.7.dev3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,27 +46,26 @@
     README = file.read()
 
 # Requirements
 # TODO: check PY_SYS_VER, and decide which requirements for e.g. 3.4, 3.6, 3.10, etc...
 with open("requirements.txt", encoding="utf-8") as file:
     REQUIREMENTS = file.read().split()
 
-if PLATFORM_SYSTEM != "Windows" or int(os.getenv("NUTRA_OS_FORCE_OPT_REQS", str(0))):
-    # python-Levenshtein builds natively on Unix; Windows needs vcvarsall.bat or vc++10
-    with open("requirements-optional.txt", encoding="utf-8") as file:
-        optional_reqs = file.read().split()
-    REQUIREMENTS.extend(optional_reqs)
+
+with open("requirements-optional.txt", encoding="utf-8") as file:
+    REQUIREMENTS_EXTRA = file.read().split()
 
 # Setup method
 setup(
     name=__title__,
     author=__author__,
     author_email=__email__,
     classifiers=CLASSIFIERS,
     install_requires=REQUIREMENTS,
+    extras_require={"extras": REQUIREMENTS_EXTRA},
     python_requires=">=%s" % PY_MIN_STR,
     zip_safe=False,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     # Linux / macOS argcomplete compatible script "n"
     scripts=glob.glob("scripts/*"),
     # Windows compatible nutra.exe
```

