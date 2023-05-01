# Comparing `tmp/stochss-compute-1.0.1.tar.gz` & `tmp/stochss-compute-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stochss-compute-1.0.1.tar", last modified: Tue Feb 28 18:42:47 2023, max compression
+gzip compressed data, was "stochss-compute-1.0.2.tar", last modified: Mon May  1 21:43:49 2023, max compression
```

## Comparing `stochss-compute-1.0.1.tar` & `stochss-compute-1.0.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.235665 stochss-compute-1.0.1/
--rw-rw-r--   0 brian     (1000) brian     (1000)    35141 2021-11-22 16:17:30.000000 stochss-compute-1.0.1/LICENSE.md
--rw-rw-r--   0 brian     (1000) brian     (1000)     7044 2023-02-28 18:42:47.235665 stochss-compute-1.0.1/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     5154 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/README.md
--rw-rw-r--   0 brian     (1000) brian     (1000)      106 2023-02-28 18:42:47.235665 stochss-compute-1.0.1/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     3607 2023-02-09 20:15:35.000000 stochss-compute-1.0.1/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.215665 stochss-compute-1.0.1/stochss_compute/
--rw-rw-r--   0 brian     (1000) brian     (1000)      947 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1618 2023-02-28 18:41:54.000000 stochss-compute-1.0.1/stochss_compute/__version__.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.219665 stochss-compute-1.0.1/stochss_compute/client/
--rw-rw-r--   0 brian     (1000) brian     (1000)      851 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/client/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1570 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/client/compute_server.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      928 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/client/endpoint.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3865 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/client/server.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.219665 stochss-compute-1.0.1/stochss_compute/cloud/
--rw-rw-r--   0 brian     (1000) brian     (1000)      892 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/cloud/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25608 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/cloud/ec2.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3850 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/cloud/ec2_config.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1534 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/cloud/exceptions.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.223665 stochss-compute-1.0.1/stochss_compute/core/
--rw-rw-r--   0 brian     (1000) brian     (1000)      939 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/core/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      975 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/core/errors.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    10811 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/core/messages.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4505 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/core/remote_results.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     6054 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/core/remote_simulation.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     6598 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/launch.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.223665 stochss-compute-1.0.1/stochss_compute/server/
--rw-rw-r--   0 brian     (1000) brian     (1000)      836 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3268 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/api.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     5317 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/cache.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3240 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/is_cached.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2376 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/results.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4709 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/run.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1753 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/stochss_compute/server/sourceip.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     5933 2023-02-28 18:41:54.000000 stochss-compute-1.0.1/stochss_compute/server/status.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.219665 stochss-compute-1.0.1/stochss_compute.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7044 2023-02-28 18:42:46.000000 stochss-compute-1.0.1/stochss_compute.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     1813 2023-02-28 18:42:46.000000 stochss-compute-1.0.1/stochss_compute.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-02-28 18:42:46.000000 stochss-compute-1.0.1/stochss_compute.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      143 2023-02-28 18:42:46.000000 stochss-compute-1.0.1/stochss_compute.egg-info/entry_points.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      155 2023-02-28 18:42:46.000000 stochss-compute-1.0.1/stochss_compute.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       21 2023-02-28 18:42:46.000000 stochss-compute-1.0.1/stochss_compute.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.227665 stochss-compute-1.0.1/test/
--rw-rw-r--   0 brian     (1000) brian     (1000)      131 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/__init__.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.227665 stochss-compute-1.0.1/test/integration_tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)       55 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/integration_tests/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25268 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/integration_tests/gillespy2_models.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2569 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/integration_tests/test_cache.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1264 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/run_integration_tests.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1243 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/run_system_tests.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1235 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/run_unit_tests.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.227665 stochss-compute-1.0.1/test/system_tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)       83 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/system_tests/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25268 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/system_tests/gillespy2_models.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1374 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/system_tests/test_cli.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1814 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/system_tests/test_launch_cli.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-02-28 18:42:47.235665 stochss-compute-1.0.1/test/unit_tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)      265 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25268 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/gillespy2_models.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      519 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/mock_ssh.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1239 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_compute_server.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1451 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_ec2.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1368 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_hash.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2982 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_is_cached_handler.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1750 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_results_handler.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2750 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_run_handler.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1584 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_sourceip_handler.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3575 2023-02-09 20:15:30.000000 stochss-compute-1.0.1/test/unit_tests/test_status_handler.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.891020 stochss-compute-1.0.2/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    35141 2021-11-22 16:17:30.000000 stochss-compute-1.0.2/LICENSE.md
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7044 2023-05-01 21:43:49.891020 stochss-compute-1.0.2/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     5154 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/README.md
+-rw-rw-r--   0 brian     (1000) brian     (1000)      106 2023-05-01 21:43:49.891020 stochss-compute-1.0.2/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3607 2023-02-09 20:15:35.000000 stochss-compute-1.0.2/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.883020 stochss-compute-1.0.2/stochss_compute/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      947 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1618 2023-05-01 21:43:42.000000 stochss-compute-1.0.2/stochss_compute/__version__.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.883020 stochss-compute-1.0.2/stochss_compute/client/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      851 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/client/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1570 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/client/compute_server.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      928 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/client/endpoint.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3865 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/client/server.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.883020 stochss-compute-1.0.2/stochss_compute/cloud/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      892 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/cloud/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25608 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/cloud/ec2.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3850 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/cloud/ec2_config.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1534 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/cloud/exceptions.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.887019 stochss-compute-1.0.2/stochss_compute/core/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      939 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/core/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      975 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/core/errors.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    10811 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/core/messages.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4505 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/core/remote_results.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6054 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/core/remote_simulation.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6598 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/launch.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.887019 stochss-compute-1.0.2/stochss_compute/server/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      836 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3268 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/api.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     5317 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/cache.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3240 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/is_cached.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2376 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/results.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4709 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/run.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1753 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/stochss_compute/server/sourceip.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     5933 2023-02-28 18:41:54.000000 stochss-compute-1.0.2/stochss_compute/server/status.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.883020 stochss-compute-1.0.2/stochss_compute.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7044 2023-05-01 21:43:49.000000 stochss-compute-1.0.2/stochss_compute.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1813 2023-05-01 21:43:49.000000 stochss-compute-1.0.2/stochss_compute.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-05-01 21:43:49.000000 stochss-compute-1.0.2/stochss_compute.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      143 2023-05-01 21:43:49.000000 stochss-compute-1.0.2/stochss_compute.egg-info/entry_points.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      155 2023-05-01 21:43:49.000000 stochss-compute-1.0.2/stochss_compute.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       21 2023-05-01 21:43:49.000000 stochss-compute-1.0.2/stochss_compute.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.887019 stochss-compute-1.0.2/test/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      131 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/__init__.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.887019 stochss-compute-1.0.2/test/integration_tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       55 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/integration_tests/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25268 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/integration_tests/gillespy2_models.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2569 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/integration_tests/test_cache.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1264 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/run_integration_tests.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1243 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/run_system_tests.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1235 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/run_unit_tests.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.887019 stochss-compute-1.0.2/test/system_tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       83 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/system_tests/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25268 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/system_tests/gillespy2_models.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1374 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/system_tests/test_cli.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1814 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/system_tests/test_launch_cli.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-05-01 21:43:49.891020 stochss-compute-1.0.2/test/unit_tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      265 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    25268 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/gillespy2_models.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      519 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/mock_ssh.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1239 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_compute_server.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1451 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_ec2.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1368 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_hash.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2982 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_is_cached_handler.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1750 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_results_handler.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2750 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_run_handler.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1584 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_sourceip_handler.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3575 2023-02-09 20:15:30.000000 stochss-compute-1.0.2/test/unit_tests/test_status_handler.py
```

### Comparing `stochss-compute-1.0.1/LICENSE.md` & `stochss-compute-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/PKG-INFO` & `stochss-compute-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stochss-compute
-Version: 1.0.1
+Version: 1.0.2
 Summary: A compute delegation package for the StochSS family of stochastic simulators
 Home-page: https://github.com/StochSS/stochss-compute
 Author: See CONTRIBUTORS.md
 Author-email: briandrawert@gmail.com
 License: GPLv3
 Description: # StochSS-Compute
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stochss-compute Version: 1.0.1 Summary: A compute
+Metadata-Version: 2.1 Name: stochss-compute Version: 1.0.2 Summary: A compute
 delegation package for the StochSS family of stochastic simulators Home-page:
 https://github.com/StochSS/stochss-compute Author: See CONTRIBUTORS.md Author-
 email: briandrawert@gmail.com License: GPLv3 Description: # StochSS-Compute
 StochSS-Compute is a compute delegation server for the [StochSS](https://
 github.com/StochSS) family of stochastic simulation software. StochSS-Compute
 allows for one to run StochSS or GillesPy2 simulations on distributed cloud
 compute resources. ***
```

### Comparing `stochss-compute-1.0.1/README.md` & `stochss-compute-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/setup.py` & `stochss-compute-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/__init__.py` & `stochss-compute-1.0.2/stochss_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/__version__.py` & `stochss-compute-1.0.2/stochss_compute/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # @file    __version__.py
 # @brief   stochss-compute version info
 # @license Please see the file named LICENSE.md in parent directory
 # @website https://github.com/StochSS/stochss-compute
 # =============================================================================
 
 
-__version__      = '1.0.1'
+__version__      = '1.0.2'
 
 __title__        = "stochss-compute"
 __description__  = "A compute delegation package for the StochSS family of stochastic simulators"
 __url__          = "https://github.com/StochSS/stochss-compute"
 __download_url__ = "https://pypi.org/project/stochss-compute/#files"
 __author__       = "See CONTRIBUTORS.md"
 __email__        = "briandrawert@gmail.com"
```

### Comparing `stochss-compute-1.0.1/stochss_compute/client/__init__.py` & `stochss-compute-1.0.2/stochss_compute/client/__init__.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/client/compute_server.py` & `stochss-compute-1.0.2/stochss_compute/client/compute_server.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/client/endpoint.py` & `stochss-compute-1.0.2/stochss_compute/client/endpoint.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/client/server.py` & `stochss-compute-1.0.2/stochss_compute/client/server.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/cloud/__init__.py` & `stochss-compute-1.0.2/stochss_compute/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/cloud/ec2.py` & `stochss-compute-1.0.2/stochss_compute/cloud/ec2.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/cloud/ec2_config.py` & `stochss-compute-1.0.2/stochss_compute/cloud/ec2_config.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/cloud/exceptions.py` & `stochss-compute-1.0.2/stochss_compute/cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/core/__init__.py` & `stochss-compute-1.0.2/stochss_compute/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/core/errors.py` & `stochss-compute-1.0.2/stochss_compute/core/errors.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/core/messages.py` & `stochss-compute-1.0.2/stochss_compute/core/messages.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/core/remote_results.py` & `stochss-compute-1.0.2/stochss_compute/core/remote_results.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/core/remote_simulation.py` & `stochss-compute-1.0.2/stochss_compute/core/remote_simulation.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/launch.py` & `stochss-compute-1.0.2/stochss_compute/launch.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/__init__.py` & `stochss-compute-1.0.2/stochss_compute/server/__init__.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/api.py` & `stochss-compute-1.0.2/stochss_compute/server/api.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/cache.py` & `stochss-compute-1.0.2/stochss_compute/server/cache.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/is_cached.py` & `stochss-compute-1.0.2/stochss_compute/server/is_cached.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/results.py` & `stochss-compute-1.0.2/stochss_compute/server/results.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/run.py` & `stochss-compute-1.0.2/stochss_compute/server/run.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/sourceip.py` & `stochss-compute-1.0.2/stochss_compute/server/sourceip.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute/server/status.py` & `stochss-compute-1.0.2/stochss_compute/server/status.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/stochss_compute.egg-info/PKG-INFO` & `stochss-compute-1.0.2/stochss_compute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stochss-compute
-Version: 1.0.1
+Version: 1.0.2
 Summary: A compute delegation package for the StochSS family of stochastic simulators
 Home-page: https://github.com/StochSS/stochss-compute
 Author: See CONTRIBUTORS.md
 Author-email: briandrawert@gmail.com
 License: GPLv3
 Description: # StochSS-Compute
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stochss-compute Version: 1.0.1 Summary: A compute
+Metadata-Version: 2.1 Name: stochss-compute Version: 1.0.2 Summary: A compute
 delegation package for the StochSS family of stochastic simulators Home-page:
 https://github.com/StochSS/stochss-compute Author: See CONTRIBUTORS.md Author-
 email: briandrawert@gmail.com License: GPLv3 Description: # StochSS-Compute
 StochSS-Compute is a compute delegation server for the [StochSS](https://
 github.com/StochSS) family of stochastic simulation software. StochSS-Compute
 allows for one to run StochSS or GillesPy2 simulations on distributed cloud
 compute resources. ***
```

### Comparing `stochss-compute-1.0.1/stochss_compute.egg-info/SOURCES.txt` & `stochss-compute-1.0.2/stochss_compute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/integration_tests/gillespy2_models.py` & `stochss-compute-1.0.2/test/integration_tests/gillespy2_models.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/integration_tests/test_cache.py` & `stochss-compute-1.0.2/test/integration_tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/run_integration_tests.py` & `stochss-compute-1.0.2/test/run_integration_tests.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/run_system_tests.py` & `stochss-compute-1.0.2/test/run_system_tests.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/run_unit_tests.py` & `stochss-compute-1.0.2/test/run_unit_tests.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/system_tests/gillespy2_models.py` & `stochss-compute-1.0.2/test/system_tests/gillespy2_models.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/system_tests/test_cli.py` & `stochss-compute-1.0.2/test/system_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/system_tests/test_launch_cli.py` & `stochss-compute-1.0.2/test/system_tests/test_launch_cli.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/gillespy2_models.py` & `stochss-compute-1.0.2/test/unit_tests/gillespy2_models.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/mock_ssh.py` & `stochss-compute-1.0.2/test/unit_tests/mock_ssh.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_compute_server.py` & `stochss-compute-1.0.2/test/unit_tests/test_compute_server.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_ec2.py` & `stochss-compute-1.0.2/test/unit_tests/test_ec2.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_hash.py` & `stochss-compute-1.0.2/test/unit_tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_is_cached_handler.py` & `stochss-compute-1.0.2/test/unit_tests/test_is_cached_handler.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_results_handler.py` & `stochss-compute-1.0.2/test/unit_tests/test_results_handler.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_run_handler.py` & `stochss-compute-1.0.2/test/unit_tests/test_run_handler.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_sourceip_handler.py` & `stochss-compute-1.0.2/test/unit_tests/test_sourceip_handler.py`

 * *Files identical despite different names*

### Comparing `stochss-compute-1.0.1/test/unit_tests/test_status_handler.py` & `stochss-compute-1.0.2/test/unit_tests/test_status_handler.py`

 * *Files identical despite different names*

