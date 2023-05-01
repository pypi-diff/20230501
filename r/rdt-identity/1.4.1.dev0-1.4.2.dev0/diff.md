# Comparing `tmp/rdt_identity-1.4.1.dev0.tar.gz` & `tmp/rdt_identity-1.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.4.1.dev0.tar", last modified: Tue Apr 25 18:42:16 2023, max compression
+gzip compressed data, was "rdt_identity-1.4.2.dev0.tar", last modified: Mon May  1 18:10:53 2023, max compression
```

## Comparing `rdt_identity-1.4.1.dev0.tar` & `rdt_identity-1.4.2.dev0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.198709 rdt_identity-1.4.1.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42542 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-04-25 18:42:16.198814 rdt_identity-1.4.1.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.187019 rdt_identity-1.4.1.dev0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.187088 rdt_identity-1.4.1.dev0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.187154 rdt_identity-1.4.1.dev0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.190437 rdt_identity-1.4.1.dev0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-04-25 18:42:16.199362 rdt_identity-1.4.1.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4191 2023-04-13 17:42:44.000000 rdt_identity-1.4.1.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.190888 rdt_identity-1.4.1.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.187405 rdt_identity-1.4.1.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.191599 rdt_identity-1.4.1.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.192099 rdt_identity-1.4.1.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43118 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.193133 rdt_identity-1.4.1.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.193428 rdt_identity-1.4.1.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.193885 rdt_identity-1.4.1.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.194182 rdt_identity-1.4.1.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.4.1.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.194823 rdt_identity-1.4.1.dev0/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10032 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.195426 rdt_identity-1.4.1.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/unit/test__addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.197478 rdt_identity-1.4.1.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.197651 rdt_identity-1.4.1.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.198007 rdt_identity-1.4.1.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-25 18:42:16.198558 rdt_identity-1.4.1.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20962 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-25 18:41:38.000000 rdt_identity-1.4.1.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.139033 rdt_identity-1.4.2.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42880 2023-04-26 21:05:25.000000 rdt_identity-1.4.2.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-05-01 18:10:53.139134 rdt_identity-1.4.2.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.127908 rdt_identity-1.4.2.dev0/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.127971 rdt_identity-1.4.2.dev0/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.128033 rdt_identity-1.4.2.dev0/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.131330 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-05-01 18:10:53.139824 rdt_identity-1.4.2.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4183 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.131804 rdt_identity-1.4.2.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.128281 rdt_identity-1.4.2.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.132518 rdt_identity-1.4.2.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.133022 rdt_identity-1.4.2.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43103 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134071 rdt_identity-1.4.2.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134360 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.134809 rdt_identity-1.4.2.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.135130 rdt_identity-1.4.2.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.4.2.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.135715 rdt_identity-1.4.2.dev0/tests/quality/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/dataset_info.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10137 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/quality/test_quality.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/quality/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.136295 rdt_identity-1.4.2.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.137949 rdt_identity-1.4.2.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138108 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138407 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-05-01 18:10:53.138889 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21103 2023-05-01 18:10:03.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.4.2.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.4.1.dev0/CONTRIBUTING.rst` & `rdt_identity-1.4.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/HISTORY.md` & `rdt_identity-1.4.2.dev0/HISTORY.md`

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

### Comparing `rdt_identity-1.4.1.dev0/LICENSE` & `rdt_identity-1.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/PKG-INFO` & `rdt_identity-1.4.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.4.1.dev0
+Version: 1.4.2.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.4.1.dev0 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.4.2.dev0 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `rdt_identity-1.4.1.dev0/README.md` & `rdt_identity-1.4.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/RELEASE.md` & `rdt_identity-1.4.2.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.4.2.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/setup.cfg` & `rdt_identity-1.4.2.dev0/setup.cfg`

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

### Comparing `rdt_identity-1.4.1.dev0/setup.py` & `rdt_identity-1.4.2.dev0/setup.py`

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

### Comparing `rdt_identity-1.4.1.dev0/tests/__init__.py` & `rdt_identity-1.4.2.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/code_style.py` & `rdt_identity-1.4.2.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/contributing.py` & `rdt_identity-1.4.2.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.4.2.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.4.2.dev0/tests/integration/test_hyper_transformer.py`

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

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/test_transformers.py` & `rdt_identity-1.4.2.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/test_base.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/integration/transformers/test_text.py` & `rdt_identity-1.4.2.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/performance/test_performance.py` & `rdt_identity-1.4.2.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.4.2.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/quality/dataset_info.csv` & `rdt_identity-1.4.2.dev0/tests/quality/dataset_info.csv`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/quality/test_quality.py` & `rdt_identity-1.4.2.dev0/tests/quality/test_quality.py`

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

### Comparing `rdt_identity-1.4.1.dev0/tests/quality/utils.py` & `rdt_identity-1.4.2.dev0/tests/quality/utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/test___init__.py` & `rdt_identity-1.4.2.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/test__addons.py` & `rdt_identity-1.4.2.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.4.2.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_base.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_null.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_null.py`

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

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_text.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.4.1.dev0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.4.2.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

