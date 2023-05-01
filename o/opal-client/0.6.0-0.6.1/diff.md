# Comparing `tmp/opal-client-0.6.0.tar.gz` & `tmp/opal-client-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-client-0.6.0.tar", last modified: Fri Apr 21 07:57:01 2023, max compression
+gzip compressed data, was "opal-client-0.6.1.tar", last modified: Mon May  1 17:32:27 2023, max compression
```

## Comparing `opal-client-0.6.0.tar` & `opal-client-0.6.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.692385 opal-client-0.6.0/
--rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-04-21 07:57:01.692177 opal-client-0.6.0/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.683687 opal-client-0.6.0/opal_client/
--rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.684985 opal-client-0.6.0/opal_client/callbacks/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/callbacks/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/callbacks/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.6.0/opal_client/callbacks/register.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/callbacks/reporter.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2184 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    18405 2023-04-19 15:20:19.000000 opal-client-0.6.0/opal_client/client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10106 2023-04-20 15:05:49.000000 opal-client-0.6.0/opal_client/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.685579 opal-client-0.6.0/opal_client/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4286 2022-12-08 13:45:19.000000 opal-client-0.6.0/opal_client/data/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/data/rpc.py
--rw-r--r--   0 roekatz    (501) staff       (20)    19105 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/data/updater.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/limiter.py
--rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.686112 opal-client-0.6.0/opal_client/opa/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.686238 opal-client-0.6.0/opal_client/opa/healthcheck/
--rw-r--r--   0 roekatz    (501) staff       (20)     1123 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/healthcheck/opal.rego
--rw-r--r--   0 roekatz    (501) staff       (20)     3047 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3144 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8116 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/opa/runner.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.687993 opal-client-0.6.0/opal_client/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-01-19 13:43:15.000000 opal-client-0.6.0/opal_client/policy/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-01-19 13:43:15.000000 opal-client-0.6.0/opal_client/policy/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy/topics.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13408 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/policy/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.689461 opal-client-0.6.0/opal_client/policy_store/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy_store/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-03-12 10:36:51.000000 opal-client-0.6.0/opal_client/policy_store/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8610 2023-04-19 15:20:19.000000 opal-client-0.6.0/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2518 2023-03-27 20:28:44.000000 opal-client-0.6.0/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    31778 2023-04-20 15:05:49.000000 opal-client-0.6.0/opal_client/policy_store/opa_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5301 2023-03-27 20:28:44.000000 opal-client-0.6.0/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1795 2023-03-12 10:36:51.000000 opal-client-0.6.0/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.691938 opal-client-0.6.0/opal_client/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/tests/data_updater_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1960 2023-04-19 08:36:33.000000 opal-client-0.6.0/opal_client/tests/opa_client_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.684494 opal-client-0.6.0/opal_client.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1445 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      401 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-04-21 07:57:01.692428 opal-client-0.6.0/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2831 2022-12-08 13:40:17.000000 opal-client-0.6.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.699254 opal-client-0.6.1/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-05-01 17:32:27.699079 opal-client-0.6.1/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.692278 opal-client-0.6.1/opal_client/
+-rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.693941 opal-client-0.6.1/opal_client/callbacks/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/callbacks/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/callbacks/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.6.1/opal_client/callbacks/register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/callbacks/reporter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2184 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    18495 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10106 2023-04-20 15:05:49.000000 opal-client-0.6.1/opal_client/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.694868 opal-client-0.6.1/opal_client/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4286 2022-12-08 13:45:19.000000 opal-client-0.6.1/opal_client/data/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/data/rpc.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    19105 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/data/updater.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/limiter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.695634 opal-client-0.6.1/opal_client/opa/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.695803 opal-client-0.6.1/opal_client/opa/healthcheck/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1123 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/healthcheck/opal.rego
+-rw-r--r--   0 roekatz    (501) staff       (20)     3047 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3144 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8116 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/opa/runner.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.696776 opal-client-0.6.1/opal_client/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-01-19 13:43:15.000000 opal-client-0.6.1/opal_client/policy/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-01-19 13:43:15.000000 opal-client-0.6.1/opal_client/policy/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy/topics.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13408 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/policy/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.698011 opal-client-0.6.1/opal_client/policy_store/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy_store/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-03-12 10:36:51.000000 opal-client-0.6.1/opal_client/policy_store/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8421 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2352 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    32153 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5401 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1795 2023-03-12 10:36:51.000000 opal-client-0.6.1/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.698764 opal-client-0.6.1/opal_client/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1960 2023-04-19 08:36:33.000000 opal-client-0.6.1/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.693142 opal-client-0.6.1/opal_client.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1445 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      417 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-05-01 17:32:27.699295 opal-client-0.6.1/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2831 2022-12-08 13:40:17.000000 opal-client-0.6.1/setup.py
```

### Comparing `opal-client-0.6.0/PKG-INFO` & `opal-client-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.6.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.6.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
```

### Comparing `opal-client-0.6.0/opal_client/callbacks/api.py` & `opal-client-0.6.1/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/callbacks/register.py` & `opal-client-0.6.1/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/callbacks/reporter.py` & `opal-client-0.6.1/opal_client/callbacks/reporter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/cli.py` & `opal-client-0.6.1/opal_client/cli.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/client.py` & `opal-client-0.6.1/opal_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,18 +71,31 @@
             inline_opa_options or opal_client_config.INLINE_OPA_CONFIG
         )
         opal_client_identifier: str = (
             opal_client_config.OPAL_CLIENT_STAT_ID or f"CLIENT_{uuid.uuid4().hex}"
         )
         # set logs
         configure_logs()
+
+        self.offline_mode_enabled = (
+            offline_mode_enabled or opal_client_config.OFFLINE_MODE_ENABLED
+        )
+        if self.offline_mode_enabled and not inline_opa_enabled:
+            logger.warning(
+                "Offline mode was enabled, but isn't supported when using an external policy store (inline OPA is disabled)"
+            )
+            self.offline_mode_enabled = False
+
         # Init policy store client
         self.policy_store_type: PolicyStoreTypes = policy_store_type
         self.policy_store: BasePolicyStoreClient = (
-            policy_store or PolicyStoreClientFactory.create(policy_store_type)
+            policy_store
+            or PolicyStoreClientFactory.create(
+                policy_store_type, offline_mode_enabled=self.offline_mode_enabled
+            )
         )
         # data fetcher
         self.data_fetcher = DataFetcher()
         # callbacks register
         if hasattr(opal_client_config.DEFAULT_UPDATE_CALLBACKS, "callbacks"):
             default_callbacks = opal_client_config.DEFAULT_UPDATE_CALLBACKS.callbacks
         else:
@@ -175,23 +188,14 @@
             )
         self.store_backup_path = (
             store_backup_path or opal_client_config.STORE_BACKUP_PATH
         )
         self.store_backup_interval = (
             store_backup_interval or opal_client_config.STORE_BACKUP_INTERVAL
         )
-
-        self.offline_mode_enabled = (
-            offline_mode_enabled or opal_client_config.OFFLINE_MODE_ENABLED
-        )
-        if self.offline_mode_enabled and not inline_opa_enabled:
-            logger.warning(
-                "Offline mode was enabled, but isn't supported when using an external policy store (inline OPA is disabled)"
-            )
-            self.offline_mode_enabled = False
         self._backup_loaded = False
 
         # init fastapi app
         self.app: FastAPI = self._init_fast_api_app()
 
     def _init_fast_api_app(self):
         """inits the fastapi app object."""
@@ -328,15 +332,15 @@
             logger.exception("exception while shutting down updaters")
 
     async def load_store_from_backup(self):
         """Imports the backup file, if exists, to the policy store."""
         try:
             if os.path.isfile(self.store_backup_path):
                 async with aiofiles.open(self.store_backup_path, "r") as backup_file:
-                    logger.debug("importing policy store from backup file...")
+                    logger.info("importing policy store from backup file...")
                     await self.policy_store.full_import(backup_file)
                     logger.debug("import completed")
                     self._backup_loaded = True
             else:
                 logger.warning("policy store backup file wasn't found")
         except Exception:
             logger.exception("failed to load backup data to policy store")
```

### Comparing `opal-client-0.6.0/opal_client/config.py` & `opal-client-0.6.1/opal_client/config.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/data/api.py` & `opal-client-0.6.1/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/data/fetcher.py` & `opal-client-0.6.1/opal_client/data/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/data/rpc.py` & `opal-client-0.6.1/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/data/updater.py` & `opal-client-0.6.1/opal_client/data/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/limiter.py` & `opal-client-0.6.1/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/opa/healthcheck/opal.rego` & `opal-client-0.6.1/opal_client/opa/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/opa/logger.py` & `opal-client-0.6.1/opal_client/opa/logger.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/opa/options.py` & `opal-client-0.6.1/opal_client/opa/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/opa/runner.py` & `opal-client-0.6.1/opal_client/opa/runner.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/policy/fetcher.py` & `opal-client-0.6.1/opal_client/policy/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/policy/options.py` & `opal-client-0.6.1/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/policy/topics.py` & `opal-client-0.6.1/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/policy/updater.py` & `opal-client-0.6.1/opal_client/policy/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/policy_store/api.py` & `opal-client-0.6.1/opal_client/policy_store/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/policy_store/base_policy_store_client.py` & `opal-client-0.6.1/opal_client/policy_store/base_policy_store_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,14 @@
         raise NotImplementedError()
 
     async def delete_policy_data(
         self, path: str = "", transaction_id: Optional[str] = None
     ):
         raise NotImplementedError()
 
-    async def patch_data(
-        self,
-        path: str,
-        patch_document: Dict[str, Any],
-        transaction_id: Optional[str] = None,
-    ):
-        raise NotImplementedError()
-
     async def get_data(self, path: str) -> Dict:
         raise NotImplementedError()
 
     async def get_data_with_input(self, path: str, input: BaseModel) -> Dict:
         raise NotImplementedError()
 
     async def init_healthcheck_policy(self, policy_id: str, policy_code: str):
```

### Comparing `opal-client-0.6.0/opal_client/policy_store/mock_policy_store_client.py` & `opal-client-0.6.1/opal_client/policy_store/mock_policy_store_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,22 +66,14 @@
         self, path: str = "", transaction_id: Optional[str] = None
     ):
         if not path:
             self._data = {}
         else:
             del self._data[path]
 
-    async def patch_data(
-        self,
-        path: str,
-        patch_document: Dict[str, Any],
-        transaction_id: Optional[str] = None,
-    ):
-        pass
-
     async def wait_for_data(self):
         """Wait until the store has data set in it."""
         await self.has_data_event.wait()
 
     async def init_healthcheck_policy(
         self, policy_id: str, policy_code: str, data_updater_enabled: bool = True
     ):
```

### Comparing `opal-client-0.6.0/opal_client/policy_store/opa_client.py` & `opal-client-0.6.1/opal_client/policy_store/opa_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import time
 from asyncio import StreamReader, StreamWriter
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Set
 from urllib.parse import urlencode
 
 import aiohttp
+import dpath
 from fastapi import Response, status
 from opal_client.config import opal_client_config
 from opal_client.logger import logger
 from opal_client.policy_store.base_policy_store_client import (
     BasePolicyStoreClient,
     JsonableValue,
 )
@@ -235,32 +236,61 @@
             transaction_policy_statistics=state.transaction_policy_statistics,
         )
         return await self._store.set_policy(
             policy_id=self._policy_id, policy_code=policy_code
         )
 
 
+class OpaStaticDataCache:
+    """Caching OPA's static data, so we can back it up without querying.
+
+    /v1/data which also includes virtual documents.
+    """
+
+    def __init__(self):
+        self._root_data = {}
+
+    def set(self, path, data):
+        if not path or path == "/":
+            assert isinstance(data, dict), ValueError(
+                "Setting root document must be a dict"
+            )
+            self._root_data = data.copy()
+        else:
+            # This would overwrite already existing paths
+            dpath.new(self._root_data, path, data)
+
+    def delete(self, path):
+        if not path or path == "/":
+            self._root_data = {}
+        else:
+            dpath.delete(self._root_data, path)
+
+    def get_data(self):
+        return self._root_data
+
+
 class OpaClient(BasePolicyStoreClient):
     """communicates with OPA via its REST API."""
 
     POLICY_NAME = "rbac"
 
     def __init__(
         self,
         opa_server_url=None,
         opa_auth_token: Optional[str] = None,
         auth_type: PolicyStoreAuth = PolicyStoreAuth.NONE,
         oauth_client_id: Optional[str] = None,
         oauth_client_secret: Optional[str] = None,
         oauth_server: Optional[str] = None,
         data_updater_enabled: bool = True,
+        cache_policy_data: bool = False,
     ):
         base_url = opa_server_url or opal_client_config.POLICY_STORE_URL
         self._opa_url = f"{base_url}/v1"
-        self._cached_policies: Dict[str, str] = {}
         self._policy_version: Optional[str] = None
         self._lock = asyncio.Lock()
         self._token = opa_auth_token
         self._auth_type: PolicyStoreAuth = auth_type
         self._oauth_client_id = oauth_client_id
         self._oauth_client_secret = oauth_client_secret
         self._oauth_server = oauth_server
@@ -290,14 +320,18 @@
 
         logger.info(f"Authentication mode for policy store: {auth_type}")
 
         self._transaction_state = OpaTransactionLogState(data_updater_enabled)
         # as long as this is null, persisting transaction log to OPA is disabled
         self._transaction_state_writer: Optional[OpaTransactionLogState] = None
 
+        self._policy_data_cache: Optional[OpaStaticDataCache] = None
+        if cache_policy_data:
+            self._policy_data_cache = OpaStaticDataCache()
+
     async def get_policy_version(self) -> Optional[str]:
         return self._policy_version
 
     @retry(**RETRY_CONFIG)
     async def _get_oauth_token(self):
         logger.info("Retrieving a new OAuth access_token.")
 
@@ -361,15 +395,14 @@
         if should_ignore_path(
             policy_id, opal_client_config.POLICY_STORE_POLICY_PATHS_TO_IGNORE
         ):
             logger.info(
                 f"Ignoring setting policy - {policy_id}, set in POLICY_PATHS_TO_IGNORE."
             )
             return
-        self._cached_policies[policy_id] = policy_code
         async with aiohttp.ClientSession() as session:
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.put(
                     f"{self._opa_url}/policies/{policy_id}",
                     data=policy_code,
@@ -499,29 +532,34 @@
 
         This overcomes issues of misordering (e.g. setting a renamed
         policy before deleting the old one, or setting a policy before
         its dependencies)
         """
         while True:
             failed_ops = []
+            failure_msgs = []
             for op in ops:
                 # Only expected errors are retried (such as 400), so exceptions are not caught
                 response = await op()
                 if response and response.status_code != status.HTTP_200_OK:
-                    logger.warning(
-                        f"Failed policy operation, would retry again after the rest. status: {response.status_code}, body: {response.body.decode()}"
+                    # Delay error logging until we know retrying won't help
+                    failure_msgs.append(
+                        f"Failed policy operation. status: {response.status_code}, body: {response.body.decode()}"
                     )
                     failed_ops.append(op)
 
             if len(failed_ops) == 0:
                 # all ops succeeded
                 return
 
             if len(failed_ops) == len(ops):
                 # all ops failed on this iteration, no point at retrying
+                for failure_msg in failure_msgs:
+                    logger.error(failure_msg)
+
                 raise RuntimeError("Giving up setting / deleting failed modules to OPA")
 
             ops = failed_ops  # retry failed ops
 
     async def _set_policies_from_complete_bundle(self, bundle: PolicyBundle):
         module_ids_in_store: Set[str] = set(await self.get_policy_module_ids())
         module_ids_in_bundle: Set[str] = {
@@ -642,21 +680,24 @@
                 headers = await self._get_auth_headers()
 
                 async with session.put(
                     f"{self._opa_url}/data{path}",
                     data=json.dumps(policy_data, default=str),
                     headers=headers,
                 ) as opa_response:
-                    return await proxy_response_unless_invalid(
+                    response = await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_204_NO_CONTENT,
                             status.HTTP_304_NOT_MODIFIED,
                         ],
                     )
+                    if self._policy_data_cache:
+                        self._policy_data_cache.set(path, policy_data)
+                    return response
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
     @affects_transaction
     @retry(**RETRY_CONFIG)
     async def delete_policy_data(
@@ -669,50 +710,24 @@
         async with aiohttp.ClientSession() as session:
             try:
                 headers = await self._get_auth_headers()
 
                 async with session.delete(
                     f"{self._opa_url}/data{path}", headers=headers
                 ) as opa_response:
-                    return await proxy_response_unless_invalid(
+                    response = await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_204_NO_CONTENT,
                             status.HTTP_404_NOT_FOUND,
                         ],
                     )
-            except aiohttp.ClientError as e:
-                logger.warning("Opa connection error: {err}", err=repr(e))
-                raise
-
-    @affects_transaction
-    async def patch_data(
-        self,
-        path: str,
-        patch_document: JSONPatchDocument,
-        transaction_id: Optional[str] = None,
-    ):
-        path = self._safe_data_module_path(path)
-        # a patch document is a list of actions
-        # we render each action with pydantic, and then dump the doc into json
-        json_document = json.dumps([action.dict() for action in patch_document])
-
-        async with aiohttp.ClientSession() as session:
-            try:
-                headers = await self._get_auth_headers()
-
-                async with session.patch(
-                    f"{self._opa_url}/data{path}",
-                    data=json_document,
-                    headers=headers,
-                ) as opa_response:
-                    return await proxy_response_unless_invalid(
-                        opa_response,
-                        accepted_status_codes=[status.HTTP_204_NO_CONTENT],
-                    )
+                    if self._policy_data_cache:
+                        self._policy_data_cache.delete(path)
+                    return response
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
     @fail_silently()
     @retry(**RETRY_CONFIG)
     async def get_data(self, path: str) -> Dict:
@@ -728,15 +743,16 @@
         try:
             headers = await self._get_auth_headers()
 
             async with aiohttp.ClientSession() as session:
                 async with session.get(
                     f"{self._opa_url}/data{path}", headers=headers
                 ) as opa_response:
-                    return await opa_response.json()
+                    json_response = await opa_response.json()
+                    return json_response.get("result", {})
         except aiohttp.ClientError as e:
             logger.warning("Opa connection error: {err}", err=repr(e))
             raise
 
     @retry(**RETRY_CONFIG)
     async def get_data_with_input(self, path: str, input: BaseModel) -> Dict:
         """evaluates a data document against an input. that is how OPA "runs
@@ -801,16 +817,18 @@
         return self._transaction_state.ready
 
     async def is_healthy(self) -> bool:
         return self._transaction_state.healthy
 
     async def full_export(self, writer: StreamWriter) -> None:
         policies = await self.get_policies()
-        data = await self.get_data("")
-        await writer.write(json.dumps({"policies": policies, "data": data}))
+        data = self._policy_data_cache.get_data()
+        await writer.write(
+            json.dumps({"policies": policies, "data": data}, default=str)
+        )
 
     async def full_import(self, reader: StreamReader) -> None:
         import_data = json.loads(await reader.read())
 
         await OpaClient._attempt_operations_with_postponed_failure_retry(
             [
                 functools.partial(self.set_policy, policy_id=id, policy_code=raw)
```

### Comparing `opal-client-0.6.0/opal_client/policy_store/policy_store_client_factory.py` & `opal-client-0.6.1/opal_client/policy_store/policy_store_client_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         save_to_cache=True,
         token: Optional[str] = None,
         auth_type: PolicyStoreAuth = None,
         oauth_client_id: Optional[str] = None,
         oauth_client_secret: Optional[str] = None,
         oauth_server: Optional[str] = None,
         data_updater_enabled: Optional[bool] = None,
+        offline_mode_enabled: bool = False,
     ) -> BasePolicyStoreClient:
         """
         Factory method - create a new policy store by type.
 
         Args:
             store_type (PolicyStoreTypes, optional): The type of policy-store to use. Defaults to opal_client_config.POLICY_STORE_TYPE.
             url (str, optional): the URL of the policy store. Defaults to opal_client_config.POLICY_STORE_URL.
@@ -113,14 +114,15 @@
                 url,
                 opa_auth_token=store_token,
                 auth_type=auth_type,
                 oauth_client_id=oauth_client_id,
                 oauth_client_secret=oauth_client_secret,
                 oauth_server=oauth_server,
                 data_updater_enabled=data_updater_enabled,
+                cache_policy_data=offline_mode_enabled,
             )
         # MOCK
         elif PolicyStoreTypes.MOCK == store_type:
             from opal_client.policy_store.mock_policy_store_client import (
                 MockPolicyStoreClient,
             )
```

### Comparing `opal-client-0.6.0/opal_client/policy_store/schemas.py` & `opal-client-0.6.1/opal_client/policy_store/schemas.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/tests/data_updater_test.py` & `opal-client-0.6.1/opal_client/tests/data_updater_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/tests/opa_client_test.py` & `opal-client-0.6.1/opal_client/tests/opa_client_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client/tests/server_to_client_intergation_test.py` & `opal-client-0.6.1/opal_client/tests/server_to_client_intergation_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/opal_client.egg-info/PKG-INFO` & `opal-client-0.6.1/opal_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.6.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.6.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
```

### Comparing `opal-client-0.6.0/opal_client.egg-info/SOURCES.txt` & `opal-client-0.6.1/opal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.0/setup.py` & `opal-client-0.6.1/setup.py`

 * *Files identical despite different names*

