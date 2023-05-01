# Comparing `tmp/rdt-1.4.1.dev0.tar.gz` & `tmp/rdt-1.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.4.1.dev0.tar", last modified: Tue Apr 25 18:42:07 2023, max compression
+gzip compressed data, was "rdt-1.4.2.dev0.tar", last modified: Mon May  1 18:10:49 2023, max compression
```

## Comparing `rdt-1.4.1.dev0.tar` & `rdt-1.4.2.dev0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.535228 rdt-1.4.1.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42542 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50601 2023-04-25 18:42:07.535416 rdt-1.4.1.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.517852 rdt-1.4.1.dev0/rdt/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2577 2023-04-13 17:42:44.000000 rdt-1.4.1.dev0/rdt/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      861 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/rdt/_addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.519504 rdt-1.4.1.dev0/rdt/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/rdt/performance/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.521413 rdt-1.4.1.dev0/rdt/performance/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/rdt/performance/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/rdt/performance/datasets/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.4.1.dev0/rdt/performance/datasets/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/performance/datasets/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/performance/datasets/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/performance/datasets/numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/rdt/performance/datasets/pii.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/rdt/performance/datasets/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/rdt/performance/datasets/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3294 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/performance/performance.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.4.1.dev0/rdt/performance/profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.523398 rdt-1.4.1.dev0/rdt/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/rdt/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.523535 rdt-1.4.1.dev0/rdt/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3398 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/addons/addons_setup.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13951 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3023 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/rdt/transformers/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7653 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5166 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20097 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/numerical.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.524208 rdt-1.4.1.dev0/rdt/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.4.1.dev0/rdt/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12429 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/rdt/transformers/pii/anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/pii/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/rdt/transformers/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-25 18:41:37.000000 rdt-1.4.1.dev0/rdt/transformers/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.518966 rdt-1.4.1.dev0/rdt.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50601 2023-04-25 18:42:07.000000 rdt-1.4.1.dev0/rdt.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2987 2023-04-25 18:42:07.000000 rdt-1.4.1.dev0/rdt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-04-25 18:42:07.000000 rdt-1.4.1.dev0/rdt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-04-25 18:42:07.000000 rdt-1.4.1.dev0/rdt.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1454 2023-04-25 18:42:07.000000 rdt-1.4.1.dev0/rdt.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-04-25 18:42:07.000000 rdt-1.4.1.dev0/rdt.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-04-25 18:42:07.535940 rdt-1.4.1.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4191 2023-04-13 17:42:44.000000 rdt-1.4.1.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.524720 rdt-1.4.1.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.513805 rdt-1.4.1.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.525654 rdt-1.4.1.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.526246 rdt-1.4.1.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43118 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.527481 rdt-1.4.1.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.527813 rdt-1.4.1.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.528521 rdt-1.4.1.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.528859 rdt-1.4.1.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.4.1.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.529768 rdt-1.4.1.dev0/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10032 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.530518 rdt-1.4.1.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/unit/test__addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.533593 rdt-1.4.1.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.533782 rdt-1.4.1.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.534193 rdt-1.4.1.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:07.534930 rdt-1.4.1.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.4.1.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20962 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-25 18:41:38.000000 rdt-1.4.1.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.255604 rdt-1.4.2.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42880 2023-04-26 21:05:25.000000 rdt-1.4.2.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50939 2023-05-01 18:10:49.255756 rdt-1.4.2.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.238888 rdt-1.4.2.dev0/rdt/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2646 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/rdt/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      861 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/_addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.240742 rdt-1.4.2.dev0/rdt/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.242811 rdt-1.4.2.dev0/rdt/performance/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/rdt/performance/datasets/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/datasets/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/datasets/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/datasets/numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/pii.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/rdt/performance/datasets/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3294 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/performance/performance.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/rdt/performance/profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.244572 rdt-1.4.2.dev0/rdt/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.244851 rdt-1.4.2.dev0/rdt/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3398 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/addons/addons_setup.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13951 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3023 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/transformers/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7790 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/rdt/transformers/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5166 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/rdt/transformers/null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20097 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/numerical.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.245461 rdt-1.4.2.dev0/rdt/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/rdt/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12429 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/rdt/transformers/pii/anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/pii/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/rdt/transformers/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.4.2.dev0/rdt/transformers/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.240117 rdt-1.4.2.dev0/rdt.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50939 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2987 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-05-01 18:10:49.000000 rdt-1.4.2.dev0/rdt.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-05-01 18:10:49.256264 rdt-1.4.2.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.245932 rdt-1.4.2.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.234862 rdt-1.4.2.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.246762 rdt-1.4.2.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.247255 rdt-1.4.2.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.248385 rdt-1.4.2.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.248715 rdt-1.4.2.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.249385 rdt-1.4.2.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.249732 rdt-1.4.2.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.4.2.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.250566 rdt-1.4.2.dev0/tests/quality/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/quality/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/quality/dataset_info.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/tests/quality/test_quality.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/quality/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.251327 rdt-1.4.2.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.254095 rdt-1.4.2.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.254369 rdt-1.4.2.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.254693 rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:49.255340 rdt-1.4.2.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.4.2.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-01 18:10:03.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.4.2.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt-1.4.1.dev0/CONTRIBUTING.rst` & `rdt-1.4.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/HISTORY.md` & `rdt-1.4.2.dev0/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # History
 
+## 1.4.1 - 2023-04-25
+
+This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
+
+### Bugs
+
+* RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
+
 ## 1.4.0 - 2023-04-13
 
 This release adds a couple of new features including adding the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also adds a change that makes all generator type transformers in the `HyperTransformer` use a different random seed.
 
 Additionally, bugs were patched in the `RegexGenerator` that caused it to crash or take too long in certain cases. Finally, this release improved the detection of Faker functions in the `AnonymizedFaker`.
 
 ### Bugs
```

### Comparing `rdt-1.4.1.dev0/LICENSE` & `rdt-1.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/PKG-INFO` & `rdt-1.4.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.4.1.dev0
+Version: 1.4.2.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -222,14 +222,22 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
+## 1.4.1 - 2023-04-25
+
+This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
+
+### Bugs
+
+* RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
+
 ## 1.4.0 - 2023-04-13
 
 This release adds a couple of new features including adding the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also adds a change that makes all generator type transformers in the `HyperTransformer` use a different random seed.
 
 Additionally, bugs were patched in the `RegexGenerator` that caused it to crash or take too long in certain cases. Finally, this release improved the detection of Faker functions in the `AnonymizedFaker`.
 
 ### Bugs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.4.1.dev0 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.4.2.dev0 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -92,38 +92,42 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 1.4.0 - 2023-04-13 This release adds
-a couple of new features including adding the `OrderedLabelEncoder` and
-deprecating the `CustomLabelEncoder`. It also adds a change that makes all
-generator type transformers in the `HyperTransformer` use a different random
-seed. Additionally, bugs were patched in the `RegexGenerator` that caused it to
-crash or take too long in certain cases. Finally, this release improved the
-detection of Faker functions in the `AnonymizedFaker`. ### Bugs * Find nested
-Faker provider submodules - PR [#630](https://github.com/sdv-dev/RDT/pull/630)
-by @frances-h * RegexGenerator fails to generate values if there are too many
-possibilities - Issue [#623](https://github.com/sdv-dev/RDT/issues/623) by @R-
-Palazzo * RegexGenerator takes too much time and runs out of memory if there
-are too many possibilities - Issue [#624](https://github.com/sdv-dev/RDT/
-issues/624) by @R-Palazzo ### New Features * Choose a different seed for each
-transformer - Issue [#619](https://github.com/sdv-dev/RDT/issues/619) by
-@fealho * Rename CustomLabelEncoder to OrderedLabelEncoder - Issue [#621]
-(https://github.com/sdv-dev/RDT/issues/621) by @R-Palazzo * Add functionality
-to find version add-on - Issue [#620](https://github.com/sdv-dev/RDT/issues/
-620) by @frances-h ## 1.3.0 - 2023-01-18 This release makes changes to the way
-that individual transformers are stored in the `HyperTransformer`. When
-accessing the config via `HyperTransformer.get_config()`, the transformers
-listed in the config are now the actual transformer instances used during
-fitting and transforming. These instances can now be accessed and used to
-examine their properties post fitting. For example, you can now view the
-mapping for a `PseudoAnonymizedFaker` instance using
+libraries for specific needs. # History ## 1.4.1 - 2023-04-25 This release
+patches an issue that prevented the `RegexGenerator` from working with regexes
+that had a very large number of possible combinations. ### Bugs *
+RegexGenerator continues to have problems if there are too many possibilities -
+Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer ##
+1.4.0 - 2023-04-13 This release adds a couple of new features including adding
+the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also
+adds a change that makes all generator type transformers in the
+`HyperTransformer` use a different random seed. Additionally, bugs were patched
+in the `RegexGenerator` that caused it to crash or take too long in certain
+cases. Finally, this release improved the detection of Faker functions in the
+`AnonymizedFaker`. ### Bugs * Find nested Faker provider submodules - PR [#630]
+(https://github.com/sdv-dev/RDT/pull/630) by @frances-h * RegexGenerator fails
+to generate values if there are too many possibilities - Issue [#623](https://
+github.com/sdv-dev/RDT/issues/623) by @R-Palazzo * RegexGenerator takes too
+much time and runs out of memory if there are too many possibilities - Issue
+[#624](https://github.com/sdv-dev/RDT/issues/624) by @R-Palazzo ### New
+Features * Choose a different seed for each transformer - Issue [#619](https://
+github.com/sdv-dev/RDT/issues/619) by @fealho * Rename CustomLabelEncoder to
+OrderedLabelEncoder - Issue [#621](https://github.com/sdv-dev/RDT/issues/621)
+by @R-Palazzo * Add functionality to find version add-on - Issue [#620](https:/
+/github.com/sdv-dev/RDT/issues/620) by @frances-h ## 1.3.0 - 2023-01-18 This
+release makes changes to the way that individual transformers are stored in the
+`HyperTransformer`. When accessing the config via `HyperTransformer.get_config
+()`, the transformers listed in the config are now the actual transformer
+instances used during fitting and transforming. These instances can now be
+accessed and used to examine their properties post fitting. For example, you
+can now view the mapping for a `PseudoAnonymizedFaker` instance using
 `PseudoAnonymizedFaker.get_mapping()` on the instance retrieved from the
 config. Additionally, the output of `reverse_tranform` no longer appends the
 `.value` suffix to every unnamed output column. Only output columns that are
 created from context extracted from the input columns will have suffixes (eg.
 `.normalized` in the `ClusterBasedNormalizer`). The `AnonymizedFaker` and
 `RegexGenerator` now have an `enforce_uniqueness` parameter, which controls
 whether the data returned by `reverse_transform` should be unique. The
```

### Comparing `rdt-1.4.1.dev0/README.md` & `rdt-1.4.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/RELEASE.md` & `rdt-1.4.2.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/__init__.py` & `rdt-1.4.2.dev0/rdt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for RDT."""
 
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.4.1.dev0'
+__version__ = '1.4.2.dev0'
 
 
 import numpy as np
 import pandas as pd
 
 from rdt import transformers
 from rdt._addons import _find_addons
@@ -36,23 +36,24 @@
         num_rows (int):
             Number of data rows to generate. Defaults to 5.
 
     Returns:
         pd.DataFrame
     """
     # Hard code first five rows
-    login_dates = ['2021-06-26', '2021-02-10', 'NAT', '2020-09-26', '2020-12-22']
-    last_login = [np.datetime64(i) for i in login_dates]
+    login_dates = pd.Series([
+        '2021-06-26', '2021-02-10', 'NAT', '2020-09-26', '2020-12-22'
+    ], dtype='datetime64[ns]')
     email_optin = pd.Series([False, False, False, True, np.nan], dtype='object')
     credit_card = ['VISA', 'VISA', 'AMEX', np.nan, 'DISCOVER']
     age = [29, 18, 21, 45, 32]
     dollars_spent = [99.99, np.nan, 2.50, 25.00, 19.99]
 
     data = pd.DataFrame({
-        'last_login': last_login,
+        'last_login': login_dates,
         'email_optin': email_optin,
         'credit_card': credit_card,
         'age': age,
         'dollars_spent': dollars_spent
     })
 
     if num_rows <= 5:
@@ -63,28 +64,31 @@
     np.random.set_state(np.random.RandomState(RANDOM_SEED).get_state())
     try:
         num_rows -= 5
 
         login_dates = np.array([
             np.datetime64('2000-01-01') + np.timedelta64(np.random.randint(0, 10000), 'D')
             for _ in range(num_rows)
-        ])
+        ], dtype='datetime64[ns]')
         login_dates[np.random.random(size=num_rows) > 0.8] = np.datetime64('NaT')
 
         email_optin = pd.Series([True, False, np.nan], dtype='object').sample(
             num_rows, replace=True)
         credit_card = np.random.choice(['VISA', 'AMEX', np.nan, 'DISCOVER'], size=num_rows)
         age = np.random.randint(18, 100, size=num_rows)
 
         dollars_spent = np.around(np.random.uniform(0, 100, size=num_rows), decimals=2)
         dollars_spent[np.random.random(size=num_rows) > 0.8] = np.nan
 
     finally:
         np.random.set_state(random_state)
 
-    return data.append(pd.DataFrame({
-        'last_login': login_dates,
-        'email_optin': email_optin,
-        'credit_card': credit_card,
-        'age': age,
-        'dollars_spent': dollars_spent
-    }), ignore_index=True)
+    return pd.concat([
+        data,
+        pd.DataFrame({
+            'last_login': login_dates,
+            'email_optin': email_optin,
+            'credit_card': credit_card,
+            'age': age,
+            'dollars_spent': dollars_spent
+        })
+    ], ignore_index=True)
```

### Comparing `rdt-1.4.1.dev0/rdt/_addons.py` & `rdt-1.4.2.dev0/rdt/_addons.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/errors.py` & `rdt-1.4.2.dev0/rdt/errors.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/hyper_transformer.py` & `rdt-1.4.2.dev0/rdt/hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/__init__.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/base.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/boolean.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/categorical.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/datetime.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/numerical.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/pii.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/pii.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/text.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/datasets/utils.py` & `rdt-1.4.2.dev0/rdt/performance/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/performance.py` & `rdt-1.4.2.dev0/rdt/performance/performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/performance/profiling.py` & `rdt-1.4.2.dev0/rdt/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/__init__.py` & `rdt-1.4.2.dev0/rdt/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/addons/addons_setup.py` & `rdt-1.4.2.dev0/rdt/transformers/addons/addons_setup.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/base.py` & `rdt-1.4.2.dev0/rdt/transformers/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/boolean.py` & `rdt-1.4.2.dev0/rdt/transformers/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/categorical.py` & `rdt-1.4.2.dev0/rdt/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/datetime.py` & `rdt-1.4.2.dev0/rdt/transformers/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 pandas_datetime_format = None
                 if self.datetime_format:
                     pandas_datetime_format = self.datetime_format.replace('%-', '%')
 
                 data = pd.to_datetime(data, format=pandas_datetime_format)
 
             except ValueError as error:
-                if 'Unknown string format:' in str(error):
+                if 'Unknown string' in str(error) or 'Unknown datetime string' in str(error):
                     message = 'Data must be of dtype datetime, or castable to datetime.'
                     raise TypeError(message) from None
 
                 raise ValueError('Data does not match specified datetime format.') from None
 
         return data
 
@@ -84,15 +84,15 @@
 
         Args:
             data (pandas.Series):
                 Data to fit the transformer to.
         """
         self._dtype = data.dtype
         if self.datetime_format is None:
-            datetime_array = data.astype(str).to_numpy()
+            datetime_array = data[data.notna()].astype(str).to_numpy()
             self.datetime_format = _guess_datetime_format_for_array(datetime_array)
 
         transformed = self._transform_helper(data)
         self.null_transformer = NullTransformer(
             self.missing_value_replacement,
             self.model_missing_values
         )
@@ -125,15 +125,18 @@
         """
         data = self._reverse_transform_helper(data)
         datetime_data = pd.to_datetime(data)
         if self.datetime_format:
             if self._dtype == 'object':
                 datetime_data = datetime_data.dt.strftime(self.datetime_format)
             elif is_datetime64_dtype(self._dtype) and '.%f' not in self.datetime_format:
-                datetime_data = pd.to_datetime(datetime_data.dt.strftime(self.datetime_format))
+                datetime_data = pd.to_datetime(
+                    datetime_data.dt.strftime(self.datetime_format),
+                    format=self.datetime_format,
+                )
 
         return datetime_data
 
 
 class OptimizedTimestampEncoder(UnixTimestampEncoder):
     """Optimized transformer for datetime data.
```

### Comparing `rdt-1.4.1.dev0/rdt/transformers/null.py` & `rdt-1.4.2.dev0/rdt/transformers/null.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Transformer for data that contains Null values."""
 
 import logging
 
 import numpy as np
 import pandas as pd
 
-from rdt.errors import TransformerInputError
-
 LOGGER = logging.getLogger(__name__)
 
 
 class NullTransformer():
     """Transformer for data that contains Null values.
 
     Args:
@@ -60,18 +58,20 @@
                 Error raised when data only contains nans and ``_missing_value_replacement``
                 is set to 'mean' or  'mode'.
         """
         if self._missing_value_replacement is None:
             return None
 
         if self._missing_value_replacement in {'mean', 'mode'} and pd.isna(data).all():
-            raise TransformerInputError(
+            msg = (
                 f"'missing_value_replacement' cannot be set to '{self._missing_value_replacement}'"
-                ' when the provided data only contains NaNs.'
+                ' when the provided data only contains NaNs. Using 0 instead.'
             )
+            LOGGER.info(msg)
+            return 0
 
         if self._missing_value_replacement == 'mean':
             return data.mean()
 
         if self._missing_value_replacement == 'mode':
             return data.mode(dropna=True)[0]
```

### Comparing `rdt-1.4.1.dev0/rdt/transformers/numerical.py` & `rdt-1.4.2.dev0/rdt/transformers/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/pii/anonymizer.py` & `rdt-1.4.2.dev0/rdt/transformers/pii/anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/pii/utils.py` & `rdt-1.4.2.dev0/rdt/transformers/pii/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/text.py` & `rdt-1.4.2.dev0/rdt/transformers/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt/transformers/utils.py` & `rdt-1.4.2.dev0/rdt/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt.egg-info/PKG-INFO` & `rdt-1.4.2.dev0/rdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.4.1.dev0
+Version: 1.4.2.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -222,14 +222,22 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
+## 1.4.1 - 2023-04-25
+
+This release patches an issue that prevented the `RegexGenerator` from working with regexes that had a very large number of possible combinations.
+
+### Bugs
+
+* RegexGenerator continues to have problems if there are too many possibilities - Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer
+
 ## 1.4.0 - 2023-04-13
 
 This release adds a couple of new features including adding the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also adds a change that makes all generator type transformers in the `HyperTransformer` use a different random seed.
 
 Additionally, bugs were patched in the `RegexGenerator` that caused it to crash or take too long in certain cases. Finally, this release improved the detection of Faker functions in the `AnonymizedFaker`.
 
 ### Bugs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.4.1.dev0 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.4.2.dev0 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -92,38 +92,42 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 1.4.0 - 2023-04-13 This release adds
-a couple of new features including adding the `OrderedLabelEncoder` and
-deprecating the `CustomLabelEncoder`. It also adds a change that makes all
-generator type transformers in the `HyperTransformer` use a different random
-seed. Additionally, bugs were patched in the `RegexGenerator` that caused it to
-crash or take too long in certain cases. Finally, this release improved the
-detection of Faker functions in the `AnonymizedFaker`. ### Bugs * Find nested
-Faker provider submodules - PR [#630](https://github.com/sdv-dev/RDT/pull/630)
-by @frances-h * RegexGenerator fails to generate values if there are too many
-possibilities - Issue [#623](https://github.com/sdv-dev/RDT/issues/623) by @R-
-Palazzo * RegexGenerator takes too much time and runs out of memory if there
-are too many possibilities - Issue [#624](https://github.com/sdv-dev/RDT/
-issues/624) by @R-Palazzo ### New Features * Choose a different seed for each
-transformer - Issue [#619](https://github.com/sdv-dev/RDT/issues/619) by
-@fealho * Rename CustomLabelEncoder to OrderedLabelEncoder - Issue [#621]
-(https://github.com/sdv-dev/RDT/issues/621) by @R-Palazzo * Add functionality
-to find version add-on - Issue [#620](https://github.com/sdv-dev/RDT/issues/
-620) by @frances-h ## 1.3.0 - 2023-01-18 This release makes changes to the way
-that individual transformers are stored in the `HyperTransformer`. When
-accessing the config via `HyperTransformer.get_config()`, the transformers
-listed in the config are now the actual transformer instances used during
-fitting and transforming. These instances can now be accessed and used to
-examine their properties post fitting. For example, you can now view the
-mapping for a `PseudoAnonymizedFaker` instance using
+libraries for specific needs. # History ## 1.4.1 - 2023-04-25 This release
+patches an issue that prevented the `RegexGenerator` from working with regexes
+that had a very large number of possible combinations. ### Bugs *
+RegexGenerator continues to have problems if there are too many possibilities -
+Issue [#635](https://github.com/sdv-dev/RDT/issues/635) by @pvk-developer ##
+1.4.0 - 2023-04-13 This release adds a couple of new features including adding
+the `OrderedLabelEncoder` and deprecating the `CustomLabelEncoder`. It also
+adds a change that makes all generator type transformers in the
+`HyperTransformer` use a different random seed. Additionally, bugs were patched
+in the `RegexGenerator` that caused it to crash or take too long in certain
+cases. Finally, this release improved the detection of Faker functions in the
+`AnonymizedFaker`. ### Bugs * Find nested Faker provider submodules - PR [#630]
+(https://github.com/sdv-dev/RDT/pull/630) by @frances-h * RegexGenerator fails
+to generate values if there are too many possibilities - Issue [#623](https://
+github.com/sdv-dev/RDT/issues/623) by @R-Palazzo * RegexGenerator takes too
+much time and runs out of memory if there are too many possibilities - Issue
+[#624](https://github.com/sdv-dev/RDT/issues/624) by @R-Palazzo ### New
+Features * Choose a different seed for each transformer - Issue [#619](https://
+github.com/sdv-dev/RDT/issues/619) by @fealho * Rename CustomLabelEncoder to
+OrderedLabelEncoder - Issue [#621](https://github.com/sdv-dev/RDT/issues/621)
+by @R-Palazzo * Add functionality to find version add-on - Issue [#620](https:/
+/github.com/sdv-dev/RDT/issues/620) by @frances-h ## 1.3.0 - 2023-01-18 This
+release makes changes to the way that individual transformers are stored in the
+`HyperTransformer`. When accessing the config via `HyperTransformer.get_config
+()`, the transformers listed in the config are now the actual transformer
+instances used during fitting and transforming. These instances can now be
+accessed and used to examine their properties post fitting. For example, you
+can now view the mapping for a `PseudoAnonymizedFaker` instance using
 `PseudoAnonymizedFaker.get_mapping()` on the instance retrieved from the
 config. Additionally, the output of `reverse_tranform` no longer appends the
 `.value` suffix to every unnamed output column. Only output columns that are
 created from context extracted from the input columns will have suffixes (eg.
 `.normalized` in the `ClusterBasedNormalizer`). The `AnonymizedFaker` and
 `RegexGenerator` now have an `enforce_uniqueness` parameter, which controls
 whether the data returned by `reverse_transform` should be unique. The
```

### Comparing `rdt-1.4.1.dev0/rdt.egg-info/SOURCES.txt` & `rdt-1.4.2.dev0/rdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/rdt.egg-info/requires.txt` & `rdt-1.4.2.dev0/rdt.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 psutil<6,>=5.7
 Faker>=10
 
 [:python_version < "3.10"]
 numpy<2,>=1.20.0
-pandas<2,>=1.1.3
+pandas>=1.1.3
 scipy<2,>=1.5.4
 scikit-learn<2,>=0.24
 
 [:python_version >= "3.10"]
 numpy<2,>=1.23.3
 scipy<2,>=1.9.2
 scikit-learn<2,>=1.1.3
 
 [:python_version >= "3.10" and python_version < "3.11"]
-pandas<2,>=1.3.4
+pandas>=1.3.4
 
 [:python_version >= "3.11"]
-pandas<2,>=1.5.0
+pandas>=1.5.0
 
 [copulas]
-copulas<0.9,>=0.8.0
+copulas<0.10,>=0.9.0
 
 [dev]
 bumpversion<0.6,>=0.5.3
 pip>=9.0.1
 watchdog<0.11,>=0.8.3
 pycodestyle<2.8.0,>=2.7.0
 pyflakes<2.4.0,>=2.3.0
@@ -59,16 +59,16 @@
 tabulate<1,>=0.8.9
 invoke
 pytest>=3.4.2
 pytest-cov>=2.6.0
 jupyter<2,>=1.0.0
 rundoc<0.5,>=0.4.3
 pytest-subtests<1.0,>=0.5
-copulas<0.9,>=0.8.0
+copulas<0.10,>=0.9.0
 
 [test]
 pytest>=3.4.2
 pytest-cov>=2.6.0
 jupyter<2,>=1.0.0
 rundoc<0.5,>=0.4.3
 pytest-subtests<1.0,>=0.5
-copulas<0.9,>=0.8.0
+copulas<0.10,>=0.9.0
```

### Comparing `rdt-1.4.1.dev0/setup.cfg` & `rdt-1.4.2.dev0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.1.dev0
+current_version = 1.4.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt-1.4.1.dev0/setup.py` & `rdt-1.4.2.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 with open('HISTORY.md', encoding='utf-8') as history_file:
     history = history_file.read()
 
 install_requires = [
     "numpy>=1.20.0,<2;python_version<'3.10'",
     "numpy>=1.23.3,<2;python_version>='3.10'",
-    "pandas>=1.1.3,<2;python_version<'3.10'",
-    "pandas>=1.3.4,<2;python_version>='3.10' and python_version<'3.11'",
-    "pandas>=1.5.0,<2;python_version>='3.11'",
+    "pandas>=1.1.3;python_version<'3.10'",
+    "pandas>=1.3.4;python_version>='3.10' and python_version<'3.11'",
+    "pandas>=1.5.0;python_version>='3.11'",
     "scipy>=1.5.4,<2;python_version<'3.10'",
     "scipy>=1.9.2,<2;python_version>='3.10'",
     "scikit-learn>=0.24,<2;python_version<'3.10'",
     "scikit-learn>=1.1.3,<2;python_version>='3.10'",
     'psutil>=5.7,<6',
     'Faker>=10',
 ]
 
 copulas_requires = [
-    'copulas>=0.8.0,<0.9',
+    'copulas>=0.9.0,<0.10',
 ]
 
 setup_requires = [
     'pytest-runner>=2.11.1',
 ]
 
 tests_require = [
@@ -136,10 +136,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.7,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.4.1.dev0',
+    version='1.4.2.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt-1.4.1.dev0/tests/__init__.py` & `rdt-1.4.2.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/code_style.py` & `rdt-1.4.2.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/contributing.py` & `rdt-1.4.2.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/datasets/tests/test_boolean.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/datasets/tests/test_categorical.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/datasets/tests/test_datetime.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/datasets/tests/test_numerical.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/datasets/tests/test_utils.py` & `rdt-1.4.2.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/test_hyper_transformer.py` & `rdt-1.4.2.dev0/tests/integration/test_hyper_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         pass
 
     def _transform(self, data):
         # Stringify input data
         return data.astype(str)
 
     def _reverse_transform(self, data):
-        return data.astype('datetime64')
+        return data.astype('datetime64[ns]')
 
 
 TEST_DATA_INDEX = [4, 6, 3, 8, 'a', 1.0, 2.0, 3.0]
 
 
 def get_input_data():
     datetimes = pd.to_datetime([
@@ -163,15 +163,15 @@
         'bool': [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 1.0, 0.0],
         'datetime': expected_datetimes,
         'names': [0.3125, 0.75, 0.75, 0.3125, 0.3125, 0.9375, 0.3125, 0.3125]
     }, index=TEST_DATA_INDEX)
     pd.testing.assert_frame_equal(transformed, expected_transformed)
 
     reversed_datetimes = pd.to_datetime([
-        '2010-01-09 20:34:17.142857216',
+        '2010-01-09',
         '2010-02-01',
         '2010-01-01',
         '2010-01-01',
         '2010-01-01',
         '2010-02-01',
         '2010-01-01',
         '2010-01-01',
```

### Comparing `rdt-1.4.1.dev0/tests/integration/test_transformers.py` & `rdt-1.4.2.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/test_base.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/test_boolean.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/test_categorical.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/test_datetime.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/test_numerical.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/integration/transformers/test_text.py` & `rdt-1.4.2.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/performance/test_performance.py` & `rdt-1.4.2.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/performance/tests/test_profiling.py` & `rdt-1.4.2.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/quality/dataset_info.csv` & `rdt-1.4.2.dev0/tests/quality/dataset_info.csv`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/quality/test_quality.py` & `rdt-1.4.2.dev0/tests/quality/test_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,28 @@
     model = LinearRegression()
     scores = cross_val_score(model, features, target)
     return np.mean(scores)
 
 
 def find_columns(data, sdtype, metadata=None):
     if metadata:
-        return {
+        columns = {
             column
             for column in metadata['fields']
             if metadata['fields'][column]['type'] == sdtype
         }
 
-    columns = set()
-    dtypes = TYPE_TO_DTYPE.get(sdtype, sdtype)
-    for dtype in dtypes:
-        selected = data.select_dtypes(dtype)
-        columns.update(set(selected.columns))
+    else:
+        columns = set()
+        dtypes = TYPE_TO_DTYPE.get(sdtype, sdtype)
+        for dtype in dtypes:
+            selected = data.select_dtypes(dtype)
+            columns.update(set(selected.columns))
 
-    return columns
+    return list(columns)
 
 
 def get_transformer_regression_scores(data, sdtype, dataset_name, transformers, metadata=None):
     """Returns regression scores for a list of transformers.
 
     Args:
         data (pandas.DataFrame):
@@ -104,15 +105,15 @@
             score = get_regression_score(transformed_features, target)
             row = pd.Series({
                 'transformer_name': transformer.get_name(),
                 'dataset_name': dataset_name,
                 'column': column,
                 'score': score
             })
-            scores = scores.append(row, ignore_index=True)
+            scores = pd.concat([scores, pd.DataFrame(row).T], ignore_index=True)
 
     return scores
 
 
 def get_test_cases(sdtypes):
     test_cases = []
     path = os.path.join(os.path.dirname(__file__), 'dataset_info.csv')
@@ -147,16 +148,16 @@
     all_scores = defaultdict(pd.DataFrame)
     for dataset_name, table_name, sdtypes in test_cases:
         (data, metadata) = download_single_table(dataset_name, table_name)
         for sdtype in sdtypes:
             transformers = transformers_by_type[sdtype]
             regression_scores = get_transformer_regression_scores(
                 data, sdtype, dataset_name, transformers, metadata)
-            all_scores[sdtype] = all_scores[sdtype].append(
-                regression_scores, ignore_index=True)
+            all_scores[sdtype] = pd.concat(
+                [all_scores[sdtype], pd.DataFrame(regression_scores).T], ignore_index=True)
 
     return all_scores
 
 
 def get_results_table(regression_scores):
     """Create a table of results for each transformer on each dataset.
 
@@ -193,15 +194,15 @@
 
             row = pd.Series({
                 'transformer_name': transformer_name,
                 'dataset_name': dataset_name,
                 'score': transformer_average,
                 'score_relative_to_average': transformer_average / average_without_transformer
             })
-            results = results.append(row, ignore_index=True)
+            results = pd.concat([results, pd.DataFrame(row).T], ignore_index=True)
 
     return results
 
 
 def test_quality(subtests):
     """Run all the quality test cases.
```

### Comparing `rdt-1.4.1.dev0/tests/quality/utils.py` & `rdt-1.4.2.dev0/tests/quality/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/test___init__.py` & `rdt-1.4.2.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/test__addons.py` & `rdt-1.4.2.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/test_hyper_transformer.py` & `rdt-1.4.2.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test___init__.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_base.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_boolean.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_categorical.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_datetime.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_null.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_null.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Unit tests for the NullTransformer."""
 
-import re
 from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
-import pytest
 
-from rdt.errors import TransformerInputError
 from rdt.transformers import NullTransformer
 
 
 class TestNullTransformer:
 
     def test___init__default(self):
         """Test the initialization without passing any default arguments.
@@ -178,27 +175,30 @@
         # Run
         data = pd.Series([1, 2, np.nan], name='abc')
         missing_value_replacement = transformer._get_missing_value_replacement(data)
 
         # Assert
         assert missing_value_replacement == 1.5
 
-    def test__get_missing_value_replacement_mean_only_nans(self):
+    @patch('rdt.transformers.null.LOGGER')
+    def test__get_missing_value_replacement_mean_only_nans(self, logger_mock):
         """Test when missing_value_replacement is mean and data only contains nans."""
         # Setup
         transformer = NullTransformer('mean')
         data = pd.Series([float('nan'), None, np.nan], name='abc')
 
-        # Run and Assert
-        err_msg = re.escape(
-            "'missing_value_replacement' cannot be set to 'mean' when "
-            'the provided data only contains NaNs.'
+        # Run
+        missing_value_replacement = transformer._get_missing_value_replacement(data)
+
+        # Assert
+        logger_mock.info.assert_called_once_with(
+            "'missing_value_replacement' cannot be set to 'mean'"
+            ' when the provided data only contains NaNs. Using 0 instead.'
         )
-        with pytest.raises(TransformerInputError, match=err_msg):
-            transformer._get_missing_value_replacement(data)
+        assert missing_value_replacement == 0
 
     def test__get_missing_value_replacement_mode(self):
         """Test _get_missing_value_replacement when missing_value_replacement is 'mode'.
 
         If the missing_value_replacement is 'mode' the output fill value should be the
         mode of the input data.
 
@@ -219,27 +219,30 @@
         # Run
         data = pd.Series([1, 2, 2, np.nan], name='abc')
         missing_value_replacement = transformer._get_missing_value_replacement(data)
 
         # Assert
         assert missing_value_replacement == 2
 
-    def test__get_missing_value_replacement_mode_only_nans(self):
+    @patch('rdt.transformers.null.LOGGER')
+    def test__get_missing_value_replacement_mode_only_nans(self, logger_mock):
         """Test when missing_value_replacement is mode and data only contains nans."""
         # Setup
         transformer = NullTransformer('mode')
         data = pd.Series([float('nan'), None, np.nan], name='abc')
 
-        # Run and Assert
-        err_msg = re.escape(
+        # Run
+        missing_value_replacement = transformer._get_missing_value_replacement(data)
+
+        # Assert
+        logger_mock.info.assert_called_once_with(
             "'missing_value_replacement' cannot be set to 'mode' when "
-            'the provided data only contains NaNs.'
+            'the provided data only contains NaNs. Using 0 instead.'
         )
-        with pytest.raises(TransformerInputError, match=err_msg):
-            transformer._get_missing_value_replacement(data)
+        assert missing_value_replacement == 0
 
     def test_fit_model_missing_values_none_and_nulls(self):
         """Test fit when null column is none and there are nulls.
 
         If there are nulls in the data and model_missing_values was given as None,
         then the _model_missing_values attribute should be set to True.
         Also validate that the null attribute and the _missing_value_replacement attributes
```

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_numerical.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_text.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.4.1.dev0/tests/unit/transformers/test_utils.py` & `rdt-1.4.2.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

