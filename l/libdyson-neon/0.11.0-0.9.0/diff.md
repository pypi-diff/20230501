# Comparing `tmp/libdyson-neon-0.11.0.tar.gz` & `tmp/libdyson-neon-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdyson-neon-0.11.0.tar", last modified: Mon May  1 01:04:08 2023, max compression
+gzip compressed data, was "libdyson-neon-0.9.0.tar", last modified: Tue Mar 14 02:58:23 2023, max compression
```

## Comparing `libdyson-neon-0.11.0.tar` & `libdyson-neon-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:04:08.862520 libdyson-neon-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-01 01:04:08.862520 libdyson-neon-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:04:08.858520 libdyson-neon-0.11.0/libdyson/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:04:08.858520 libdyson-neon-0.11.0/libdyson/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/cloud_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_pure_hot_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/dyson_vacuum_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/libdyson/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:04:08.858520 libdyson-neon-0.11.0/libdyson_neon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-01 01:04:08.000000 libdyson-neon-0.11.0/libdyson_neon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-01 01:04:08.000000 libdyson-neon-0.11.0/libdyson_neon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 01:04:08.000000 libdyson-neon-0.11.0/libdyson_neon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 01:04:08.000000 libdyson-neon-0.11.0/libdyson_neon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 01:04:08.000000 libdyson-neon-0.11.0/libdyson_neon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-01 01:04:08.862520 libdyson-neon-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:04:08.858520 libdyson-neon-0.11.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:04:08.858520 libdyson-neon-0.11.0/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/test_bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/test_cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/test_dyson_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/mocked_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_fan_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_heating_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_pure_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_pure_cool_missing_env_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_purifier_humidify_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 01:03:56.000000 libdyson-neon-0.11.0/tests/test_vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-14 02:58:23.776262 libdyson-neon-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/libdyson/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/libdyson/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/cloud_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_hot_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/dyson_vacuum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/libdyson/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/libdyson_neon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 02:58:23.000000 libdyson-neon-0.9.0/libdyson_neon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 02:58:23.776262 libdyson-neon-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:58:23.772262 libdyson-neon-0.9.0/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/test_bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/test_cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/test_dyson_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/mocked_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_fan_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_heating_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_purifier_humidify_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-14 02:58:12.000000 libdyson-neon-0.9.0/tests/test_vacuum.py
```

### Comparing `libdyson-neon-0.11.0/LICENSE` & `libdyson-neon-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/PKG-INFO` & `libdyson-neon-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 0.11.0
+Version: 0.9.0
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-0.11.0/libdyson/__init__.py` & `libdyson-neon-0.9.0/libdyson/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Dyson Python library."""
 
 from typing import Optional
+
 from .const import (
     DEVICE_TYPE_360_EYE,
     DEVICE_TYPE_360_HEURIST,
     DEVICE_TYPE_PURE_COOL,
-    DEVICE_TYPE_PURIFIER_COOL_E,
-    DEVICE_TYPE_PURIFIER_COOL_K,
+    DEVICE_TYPE_PURIFIER_COOL,
+    DEVICE_TYPE_PURE_COOL_FORMALDEHYDE,
     DEVICE_TYPE_PURE_COOL_DESK,
     DEVICE_TYPE_PURE_COOL_LINK,
     DEVICE_TYPE_PURE_COOL_LINK_DESK,
     DEVICE_TYPE_PURE_HOT_COOL,
-    DEVICE_TYPE_PURIFIER_HOT_COOL_E,
-    DEVICE_TYPE_PURIFIER_HOT_COOL_K,
+    DEVICE_TYPE_PURE_HOT_COOL_NEW,
     DEVICE_TYPE_PURE_HOT_COOL_LINK,
     DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E,
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_K,
+    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE,
+    DEVICE_TYPE_PURIFIER_HOT_COOL,
 )
-
 from .const import CleaningMode  # noqa: F401
 from .const import CleaningType  # noqa: F401
 from .const import DEVICE_TYPE_NAMES  # noqa: F401
 from .const import HumidifyOscillationMode  # noqa: F401
 from .const import MessageType  # noqa: F401
 from .const import VacuumEyePowerMode  # noqa: F401
 from .const import VacuumHeuristPowerMode  # noqa: F401
 from .const import VacuumState  # noqa: F401
 from .const import WaterHardness  # noqa: F401
 from .discovery import DysonDiscovery  # noqa: F401
 from .dyson_360_eye import Dyson360Eye
 from .dyson_360_heurist import Dyson360Heurist
 from .dyson_device import DysonDevice
 from .dyson_pure_cool import DysonPureCool
+from .dyson_pure_cool import DysonPureCoolFormaldehyde
 from .dyson_pure_cool_link import DysonPureCoolLink
 from .dyson_pure_hot_cool import DysonPureHotCool
 from .dyson_pure_hot_cool_link import DysonPureHotCoolLink
-from .dyson_pure_humidify_cool import DysonPurifierHumidifyCool
+from .dyson_pure_humidify_cool import DysonPureHumidifyCool, DysonPurifierHumidifyCoolFormaldehyde
 from .utils import get_mqtt_info_from_wifi_info  # noqa: F401
 
 
 def get_device(serial: str, credential: str, device_type: str) -> Optional[DysonDevice]:
     """Get a new DysonDevice instance."""
     if device_type == DEVICE_TYPE_360_EYE:
         return Dyson360Eye(serial, credential)
@@ -49,27 +49,26 @@
     if device_type in [
         DEVICE_TYPE_PURE_COOL_LINK_DESK,
         DEVICE_TYPE_PURE_COOL_LINK,
     ]:
         return DysonPureCoolLink(serial, credential, device_type)
     if device_type in [
         DEVICE_TYPE_PURE_COOL,
-        DEVICE_TYPE_PURIFIER_COOL_K,
-        DEVICE_TYPE_PURIFIER_COOL_E,
+        DEVICE_TYPE_PURIFIER_COOL,
         DEVICE_TYPE_PURE_COOL_DESK,
     ]:
         return DysonPureCool(serial, credential, device_type)
+    if device_type == DEVICE_TYPE_PURE_COOL_FORMALDEHYDE:
+        return DysonPureCoolFormaldehyde(serial, credential, device_type)
     if device_type == DEVICE_TYPE_PURE_HOT_COOL_LINK:
         return DysonPureHotCoolLink(serial, credential, device_type)
     if device_type in [
         DEVICE_TYPE_PURE_HOT_COOL,
-        DEVICE_TYPE_PURIFIER_HOT_COOL_E,
-        DEVICE_TYPE_PURIFIER_HOT_COOL_K,
+        DEVICE_TYPE_PURE_HOT_COOL_NEW,
+        DEVICE_TYPE_PURIFIER_HOT_COOL,
     ]:
         return DysonPureHotCool(serial, credential, device_type)
-    if device_type in [
-        DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-        DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_K,
-        DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E,
-    ]:
-        return DysonPurifierHumidifyCool(serial, credential, device_type)
+    if device_type == DEVICE_TYPE_PURE_HUMIDIFY_COOL:
+        return DysonPureHumidifyCool(serial, credential, device_type)
+    if device_type == DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE:
+        return DysonPurifierHumidifyCoolFormaldehyde(serial, credential, device_type)
     return None
```

### Comparing `libdyson-neon-0.11.0/libdyson/cloud/account.py` & `libdyson-neon-0.9.0/libdyson/cloud/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,26 +10,24 @@
     DysonAuthRequired,
     DysonInvalidAccountStatus,
     DysonInvalidAuth,
     DysonLoginFailure,
     DysonNetworkError,
     DysonOTPTooFrequently,
     DysonServerError,
-    DysonAPIProvisionFailure,
 )
 
 from .device_info import DysonDeviceInfo
 
 DYSON_API_HOST = "https://appapi.cp.dyson.com"
 DYSON_API_HOST_CN = "https://appapi.cp.dyson.cn"
 DYSON_API_HEADERS = {
     "User-Agent": "android client"
 }
 
-API_PATH_PROVISION_APP = "/v1/provisioningservice/application/Android/version"
 API_PATH_USER_STATUS = "/v3/userregistration/email/userstatus"
 API_PATH_EMAIL_REQUEST = "/v3/userregistration/email/auth"
 API_PATH_EMAIL_VERIFY = "/v3/userregistration/email/verify"
 API_PATH_MOBILE_REQUEST = "/v3/userregistration/mobile/auth"
 API_PATH_MOBILE_VERIFY = "/v3/userregistration/mobile/verify"
 API_PATH_DEVICES = "/v2/provisioningservice/manifest"
 
@@ -114,46 +112,17 @@
             raise DysonNetworkError
         if response.status_code in [401, 403]:
             raise DysonInvalidAuth
         if 500 <= response.status_code < 600:
             raise DysonServerError
         return response
 
-    def provision_api(self) -> None:
-        """Provision the client connection to the API
-
-        Calls an app provisioning API. This is expected by the Dyson App API and makes the API server ready to accept
-        other API calls from the current IP Address.
-
-        Basically, this unlocks the API - the return value is not needed, and we don't need to save any cookies or
-        session tokens. It seems like the API Server sets some internal flag allowing API Calls from a specific address
-        based solely on this endpoint being called.
-
-        This isn't likely to be a security measure. It returns a version number in a json-encoded string: `"5.0.21061"`
-        and that is likely consumed by an app. Presumably, an official Dyson mobile app could check the version against
-        some internal expected value and, for example, prompt a user that it is outdated and direct them to the app
-        store to download a new version in order to continue working.
-        """
-
-        response = self.request(
-            "GET",
-            API_PATH_PROVISION_APP,
-            params=None,
-            data=None,
-            auth=False,
-        )
-
-        if response.status_code != 200:
-            raise DysonAPIProvisionFailure
-
-    def login_email_otp(self, email: str, region: str) -> Callable[[str, str], dict]:
+    def login_email_otp(self, email: str, region: str) -> Callable[[str], dict]:
         """Login using email and OTP code."""
-        self.provision_api()
-
-        # Check account status. This tells us whether an account is active or not.
+        # Check account status first. This is expected by the cloud API.
         response = self.request(
             "POST",
             API_PATH_USER_STATUS,
             params={"country": region},
             data={"email": email},
             auth=False,
         )
@@ -193,15 +162,14 @@
             body = response.json()
             self._auth_info = body
             return self._auth_info
 
         return _verify
 
     def devices(self) -> List[DysonDeviceInfo]:
-        self.provision_api()
         """Get device info from cloud account."""
         devices = []
         response = self.request("GET", API_PATH_DEVICES)
         for raw in response.json():
             if raw.get("LocalCredentials") is None:
                 # Lightcycle lights don't have LocalCredentials.
                 # They're not supported so just skip.
@@ -213,16 +181,14 @@
 
 class DysonAccountCN(DysonAccount):
     """Dyson account in Mainland China."""
 
     _HOST = DYSON_API_HOST_CN
 
     def login_mobile_otp(self, mobile: str) -> Callable[[str], dict]:
-        self.provision_api()
-
         """Login using phone number and OTP code."""
         response = self.request(
             "POST",
             API_PATH_MOBILE_REQUEST,
             data={"mobile": mobile},
             auth=False,
         )
```

### Comparing `libdyson-neon-0.11.0/libdyson/cloud/cloud_360_eye.py` & `libdyson-neon-0.9.0/libdyson/cloud/cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/cloud/device_info.py` & `libdyson-neon-0.9.0/libdyson/cloud/device_info.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/cloud/regions.py` & `libdyson-neon-0.9.0/libdyson/cloud/regions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/cloud/utils.py` & `libdyson-neon-0.9.0/libdyson/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/const.py` & `libdyson-neon-0.9.0/libdyson/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 """Constants for Dyson Python library."""
 from enum import Enum, auto
 
 DEVICE_TYPE_360_EYE = "N223"
 DEVICE_TYPE_360_HEURIST = "276"
-DEVICE_TYPE_PURE_COOL_LINK_DESK = "469"  # DP01? DP02? This one's a bit older, and scraping the Dyson website is unclear
-DEVICE_TYPE_PURE_COOL_DESK = "520"  # AM06? This one's also a bit older, and also hard to scrape off the Dyson website
-DEVICE_TYPE_PURE_COOL_LINK = "475"  # TP02
-DEVICE_TYPE_PURE_COOL = "438"  # TP04
-DEVICE_TYPE_PURIFIER_COOL_K = "438K"  # TP07 AND TP09
-DEVICE_TYPE_PURIFIER_COOL_E = "438E"  # TP07 AND TP09
-DEVICE_TYPE_PURE_HUMIDIFY_COOL = "358"  # PH01 probably, but maybe PH02? Not 100% certain
-DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_K = "358K"  # PH03 AND PH04
-DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E = "358E"  # PH03 AND PH04
-DEVICE_TYPE_PURE_HOT_COOL_LINK = "455"  # HP02
-DEVICE_TYPE_PURE_HOT_COOL = "527"  # HP04
-DEVICE_TYPE_PURIFIER_HOT_COOL_E = "527E"  # HP07 AND HP09
-DEVICE_TYPE_PURIFIER_HOT_COOL_K = "527K"  # HP07 AND HP09
+DEVICE_TYPE_PURE_COOL_LINK = "475"
+DEVICE_TYPE_PURE_COOL_LINK_DESK = "469"
+DEVICE_TYPE_PURE_COOL = "438"
+DEVICE_TYPE_PURIFIER_COOL = "438K"
+DEVICE_TYPE_PURE_COOL_FORMALDEHYDE = "438E"
+DEVICE_TYPE_PURE_COOL_DESK = "520"
+DEVICE_TYPE_PURE_HUMIDIFY_COOL = "358"
+DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE = "358E"
+DEVICE_TYPE_PURE_HOT_COOL_LINK = "455"
+DEVICE_TYPE_PURE_HOT_COOL = "527"
+DEVICE_TYPE_PURE_HOT_COOL_NEW = "527E"
+DEVICE_TYPE_PURIFIER_HOT_COOL = "527K"
 
 DEVICE_TYPE_NAMES = {
     DEVICE_TYPE_360_EYE: "360 Eye robot vacuum",
     DEVICE_TYPE_360_HEURIST: "360 Heurist robot vacuum",
     DEVICE_TYPE_PURE_COOL: "Pure Cool",
-    DEVICE_TYPE_PURIFIER_COOL_K: "Purifier Cool",
-    DEVICE_TYPE_PURIFIER_COOL_E: "Purifier Cool",
-    DEVICE_TYPE_PURE_COOL_DESK: "Pure Cool Link Desk",
+    DEVICE_TYPE_PURIFIER_COOL: "Purifier Cool",
+    DEVICE_TYPE_PURE_COOL_FORMALDEHYDE: "Pure Cool Formaldehyde",
+    DEVICE_TYPE_PURE_COOL_DESK: "Pure Cool Desk",
     DEVICE_TYPE_PURE_COOL_LINK: "Pure Cool Link",
     DEVICE_TYPE_PURE_COOL_LINK_DESK: "Pure Cool Link Desk",
     DEVICE_TYPE_PURE_HOT_COOL: "Pure Hot+Cool",
-    DEVICE_TYPE_PURIFIER_HOT_COOL_E: "Pure Hot+Cool (New)",
+    DEVICE_TYPE_PURE_HOT_COOL_NEW: "Pure Hot+Cool (New)",
     DEVICE_TYPE_PURE_HOT_COOL_LINK: "Pure Hot+Cool Link",
     DEVICE_TYPE_PURE_HUMIDIFY_COOL: "Pure Humidify+Cool",
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_K: "Purifier Humidify+Cool",
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E: "Purifier Humidify+Cool",
-    DEVICE_TYPE_PURIFIER_HOT_COOL_K: "Purifier Hot+Cool",
+    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE: "Purifier Humidify+Cool Formaldehyde",
+    DEVICE_TYPE_PURIFIER_HOT_COOL: "Purifier Hot+Cool",
 }
 
 ENVIRONMENTAL_OFF = -1
 ENVIRONMENTAL_INIT = -2
 ENVIRONMENTAL_FAIL = -3
```

### Comparing `libdyson-neon-0.11.0/libdyson/discovery.py` & `libdyson-neon-0.9.0/libdyson/discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_360_eye.py` & `libdyson-neon-0.9.0/libdyson/dyson_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_360_heurist.py` & `libdyson-neon-0.9.0/libdyson/dyson_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_device.py` & `libdyson-neon-0.9.0/libdyson/dyson_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Dyson device."""
 from abc import abstractmethod
 import json
 import logging
 import threading
-from typing import Any, Optional, List, Dict, Union
+from typing import Any, Optional
 
 import paho.mqtt.client as mqtt
 
 from .const import (
     ENVIRONMENTAL_FAIL,
     ENVIRONMENTAL_INIT,
     ENVIRONMENTAL_OFF,
     MessageType,
 )
 from .exceptions import (
     DysonConnectionRefused,
     DysonConnectTimeout,
     DysonInvalidCredential,
-    DysonNotConnected, DysonNoEnvironmentalData,
+    DysonNotConnected,
 )
 from .utils import mqtt_time
 
 _LOGGER = logging.getLogger(__name__)
 
 TIMEOUT = 10
 
@@ -160,27 +160,27 @@
             for callback in self._callbacks:
                 callback(MessageType.STATE)
 
     @abstractmethod
     def _update_status(self, payload: dict) -> None:
         """Update the device status."""
 
-    def _send_command(self, command: str, data: Optional[dict] = None) -> None:
+    def _send_command(self, command: str, data: Optional[dict] = None):
         if not self.is_connected:
             raise DysonNotConnected
         if data is None:
             data = {}
         payload = {
             "msg": command,
             "time": mqtt_time(),
         }
         payload.update(data)
         self._mqtt_client.publish(self._command_topic, json.dumps(payload))
 
-    def request_current_status(self) -> None:
+    def request_current_status(self):
         """Request current status."""
         if not self.is_connected:
             raise DysonNotConnected
         payload = {
             "msg": "REQUEST-CURRENT-STATE",
             "time": mqtt_time(),
         }
@@ -191,15 +191,15 @@
     """Dyson fan device."""
 
     def __init__(self, serial: str, credential: str, device_type: str):
         """Initialize the device."""
         super().__init__(serial, credential)
         self._device_type = device_type
 
-        self._environmental_data = {}
+        self._environmental_data = None
         self._environmental_data_available = threading.Event()
 
     @property
     def device_type(self) -> str:
         """Device type."""
         return self._device_type
 
@@ -253,23 +253,14 @@
 
     @property
     def warning_code(self) -> str:
         """Return warning code."""
         return self._get_field_value(self._status, "wacd")
 
     @property
-    def formaldehyde(self) -> Optional[int]:
-        """Return formaldehyde reading."""
-        val = self._get_environmental_field_value("hcho")
-        if val is None:
-            return None
-
-        return int(val)
-
-    @property
     def humidity(self) -> int:
         """Return humidity in percentage."""
         return self._get_environmental_field_value("hact")
 
     @property
     def temperature(self) -> int:
         """Return temperature in kelvin."""
@@ -282,30 +273,25 @@
 
     @property
     def sleep_timer(self) -> int:
         """Return sleep timer in minutes."""
         return self._get_environmental_field_value("sltm")
 
     @staticmethod
-    def _get_field_value(state: Dict[str, Any], field: str):
-        try:
-            return  state[field][1] if isinstance(state[field], list) else state[field]
-        except:
-            return None
+    def _get_field_value(state, field):
+        return state[field][1] if isinstance(state[field], list) else state[field]
 
-    def _get_environmental_field_value(self, field, divisor=1) -> Optional[Union[int, float]]:
+    def _get_environmental_field_value(self, field, divisor=1):
         value = self._get_field_value(self._environmental_data, field)
         if value == "OFF":
             return ENVIRONMENTAL_OFF
         if value == "INIT":
             return ENVIRONMENTAL_INIT
         if value == "FAIL":
             return ENVIRONMENTAL_FAIL
-        if value == "NONE" or value is None:
-            return None
         if divisor == 1:
             return int(value)
         return float(value) / divisor
 
     def _handle_message(self, payload: dict) -> None:
         super()._handle_message(payload)
         if payload["msg"] == "ENVIRONMENTAL-CURRENT-SENSOR-DATA":
```

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_pure_cool.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_cool.py`

 * *Files 7% similar despite different names*

```diff
@@ -171,7 +171,24 @@
         """Turn off oscillation."""
         current_oscillation_raw = self._get_field_value(self._status, "oson")
         if current_oscillation_raw in ["OION", "OIOF"]:
             oson = "OIOF"
         else:
             oson = "OFF"
         self._set_configuration(oson=oson)
+
+
+class DysonPureCoolFormaldehyde(DysonPureCool):
+    """This model is compatible with PureCool but has one additional sensor."""
+
+    @property
+    def formaldehyde(self) -> Optional[int]:
+        """Return formaldehyde reading."""
+        # Dyson documentation for Dyson Pure Cool Formaldehyde refers to
+        # the formaldehyde reading as HCHO (pp5).
+        # https://www.dyson.com/content/dam/dyson/maintenance/user-guides/en_US/airtreatment/purifiers/TP09/497043-01.pdf
+        #
+        # H-CHO is also a common way to refer to formaldehyde.
+        #
+        # This is part of environmental data as per:
+        # https://github.com/seanrees/prometheus-dyson/issues/13#issue-923525150
+        return self._get_environmental_field_value("hcho")
```

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_pure_cool_link.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_pure_hot_cool_link.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_pure_humidify_cool.py` & `libdyson-neon-0.9.0/libdyson/dyson_pure_humidify_cool.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     WaterHardness.HARD: "0675",
 }
 WATER_HARDNESS_STR_TO_ENUM = {
     str_: enum for enum, str_ in WATER_HARDNESS_ENUM_TO_STR.items()
 }
 
 
-class DysonPurifierHumidifyCool(DysonPureCoolBase):
+class DysonPureHumidifyCool(DysonPureCoolBase):
     """Dyson Pure Humidify+Cool device."""
 
     @property
     def oscillation(self) -> bool:
         """Return oscillation status."""
         return self._get_field_value(self._status, "oson") == "ON"
 
@@ -96,7 +96,15 @@
         """Set target humidity."""
         self._set_configuration(humt=f"{target_humidity:04d}", haut="OFF")
 
     def set_water_hardness(self, water_hardness: WaterHardness) -> None:
         """Set water hardness."""
         self._set_configuration(wath=WATER_HARDNESS_ENUM_TO_STR[water_hardness])
 
+
+class DysonPurifierHumidifyCoolFormaldehyde(DysonPureHumidifyCool):
+    """Dyson Purifier Humidify+Cool Formaldehyde device."""
+
+    @property
+    def formaldehyde(self):
+        """Return formaldehyde reading."""
+        return int(self._get_environmental_field_value("hcho"))
```

### Comparing `libdyson-neon-0.11.0/libdyson/dyson_vacuum_device.py` & `libdyson-neon-0.9.0/libdyson/dyson_vacuum_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson/exceptions.py` & `libdyson-neon-0.9.0/libdyson/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,14 @@
     """Represents invalid account status."""
 
 
 class DysonLoginFailure(DysonException):
     """Represents failure during logging in."""
 
 
-class DysonAPIProvisionFailure(DysonException):
-    """Represents failure during logging in."""
-
-
 class DysonOTPTooFrequently(DysonException):
     """Represents requesting OTP code too frequently."""
 
 
 class DysonAuthRequired(DysonException):
     """Represents not logged into could."""
 
@@ -51,11 +47,7 @@
 
 class DysonConnectionRefused(DysonException):
     """Represents mqtt connection refused by the server."""
 
 
 class DysonFailedToParseWifiInfo(DysonException):
     """Represents failed to parse WiFi information."""
-
-
-class DysonNoEnvironmentalData(DysonException):
-    """Represents mqtt not connected."""
```

### Comparing `libdyson-neon-0.11.0/libdyson/utils.py` & `libdyson-neon-0.9.0/libdyson/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/libdyson_neon.egg-info/PKG-INFO` & `libdyson-neon-0.9.0/libdyson_neon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 0.11.0
+Version: 0.9.0
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-0.11.0/libdyson_neon.egg-info/SOURCES.txt` & `libdyson-neon-0.9.0/libdyson_neon.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 tests/test_discovery.py
 tests/test_fan_device.py
 tests/test_heating_device.py
 tests/test_init.py
 tests/test_pure_cool.py
 tests/test_pure_cool_formaldehyde.py
 tests/test_pure_cool_link.py
-tests/test_pure_cool_missing_env_data.py
 tests/test_pure_hot_cool_link.py
 tests/test_pure_humidify_cool.py
 tests/test_purifier_humidify_cool_formaldehyde.py
 tests/test_utils.py
 tests/test_vacuum.py
 tests/cloud/__init__.py
 tests/cloud/conftest.py
```

### Comparing `libdyson-neon-0.11.0/pyproject.toml` & `libdyson-neon-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/setup.cfg` & `libdyson-neon-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libdyson-neon
-version = 0.11.0
+version = 0.9.0
 author = The libdyson Working Group
 author_email = dotvezz@gmail.com
 license = MIT License
 license_file = LICENSE
 platforms = any
 description = A Python library for Dyson devices.
 long_description = file: README.md
```

### Comparing `libdyson-neon-0.11.0/tests/cloud/mocked_requests.py` & `libdyson-neon-0.9.0/tests/cloud/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/cloud/test_bearer_auth.py` & `libdyson-neon-0.9.0/tests/cloud/test_bearer_auth.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/cloud/test_cloud_360_eye.py` & `libdyson-neon-0.9.0/tests/cloud/test_cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/cloud/test_dyson_account.py` & `libdyson-neon-0.9.0/tests/cloud/test_dyson_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 from libdyson.cloud.account import (
     API_PATH_DEVICES,
     API_PATH_EMAIL_REQUEST,
     API_PATH_EMAIL_VERIFY,
     API_PATH_MOBILE_REQUEST,
     API_PATH_MOBILE_VERIFY,
     API_PATH_USER_STATUS,
-    API_PATH_PROVISION_APP,
     DYSON_API_HOST_CN,
     DysonAccountCN,
     HTTPBearerAuth,
 )
 from libdyson.exceptions import (
     DysonAuthRequired,
     DysonInvalidAccountStatus,
     DysonInvalidAuth,
     DysonLoginFailure,
     DysonNetworkError,
     DysonOTPTooFrequently,
     DysonServerError,
-    DysonAPIProvisionFailure,
 )
 
 from . import AUTH_ACCOUNT, AUTH_INFO, AUTH_PASSWORD
 from .mocked_requests import MockedRequests
 from .utils import encrypt_credential
 
 EMAIL = "user@example.com"
@@ -97,26 +95,14 @@
         "NewVersionAvailable": False,
         "ProductType": "552",
         "ConnectionType": "wss",
     },
 ]
 
 
-def _app_provision_handler(
-        params: dict, json: dict, auth: Optional[AuthBase], **kwargs
-) -> Tuple[int, Optional[str]]:
-    return 200, '"5.0.21061"'
-
-
-def _app_provision_handler_error(
-        params: dict, json: dict, auth: Optional[AuthBase], **kwargs
-) -> Tuple[int, Optional[str]]:
-    return 404, ''
-
-
 @pytest.fixture(autouse=True)
 def mocked_requests(mocked_requests: MockedRequests) -> MockedRequests:
     """Return mocked requests library."""
 
     def _user_status_handler(
         params: dict, json: dict, auth: Optional[AuthBase], **kwargs
     ) -> Tuple[int, Optional[dict]]:
@@ -172,15 +158,14 @@
             or auth.username != AUTH_ACCOUNT
             or auth.password != AUTH_PASSWORD
         ) and (not isinstance(auth, HTTPBearerAuth) or auth.token != BEARER_TOKEN):
             return (401, None)
         return (200, DEVICES)
 
     mocked_requests.register_handler("POST", API_PATH_USER_STATUS, _user_status_handler)
-    mocked_requests.register_handler("GET", API_PATH_PROVISION_APP, _app_provision_handler)
     mocked_requests.register_handler(
         "POST", API_PATH_EMAIL_REQUEST, _email_request_handler
     )
     mocked_requests.register_handler(
         "POST", API_PATH_EMAIL_VERIFY, _email_verify_handler
     )
     mocked_requests.register_handler(
@@ -189,26 +174,14 @@
     mocked_requests.register_handler(
         "POST", API_PATH_MOBILE_VERIFY, _mobile_verify_handler
     )
     mocked_requests.register_handler("GET", API_PATH_DEVICES, _devices_handler)
     return mocked_requests
 
 
-def test_account_provision_api(mocked_requests: MockedRequests):
-    account = DysonAccount()
-
-    assert account.provision_api() is None
-
-    mocked_requests.register_handler("GET", API_PATH_PROVISION_APP, _app_provision_handler_error)
-
-    with pytest.raises(DysonAPIProvisionFailure):
-        account.provision_api()
-
-    mocked_requests.register_handler("GET", API_PATH_PROVISION_APP, _app_provision_handler)
-
 def test_account():
     """Test account functionalities."""
     account = DysonAccount()
 
     # Incorrect email
     with pytest.raises(DysonInvalidAccountStatus):
         account.login_email_otp("unregistered@example.com", REGION)
```

### Comparing `libdyson-neon-0.11.0/tests/cloud/utils.py` & `libdyson-neon-0.9.0/tests/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/conftest.py` & `libdyson-neon-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/mocked_mqtt.py` & `libdyson-neon-0.9.0/tests/mocked_mqtt.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_360_eye.py` & `libdyson-neon-0.9.0/tests/test_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_360_heurist.py` & `libdyson-neon-0.9.0/tests/test_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_device.py` & `libdyson-neon-0.9.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_discovery.py` & `libdyson-neon-0.9.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_fan_device.py` & `libdyson-neon-0.9.0/tests/test_fan_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_heating_device.py` & `libdyson-neon-0.9.0/tests/test_heating_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_init.py` & `libdyson-neon-0.9.0/tests/test_init.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,58 +3,56 @@
 
 import pytest
 
 from libdyson import (
     DEVICE_TYPE_360_EYE,
     DEVICE_TYPE_360_HEURIST,
     DEVICE_TYPE_PURE_COOL,
-    DEVICE_TYPE_PURIFIER_COOL_E,
-    DEVICE_TYPE_PURIFIER_COOL_K,
+    DEVICE_TYPE_PURE_COOL_FORMALDEHYDE,
     DEVICE_TYPE_PURE_COOL_DESK,
     DEVICE_TYPE_PURE_COOL_LINK,
     DEVICE_TYPE_PURE_COOL_LINK_DESK,
     DEVICE_TYPE_PURE_HOT_COOL,
-    DEVICE_TYPE_PURIFIER_HOT_COOL_E,
-    DEVICE_TYPE_PURIFIER_HOT_COOL_K,
+    DEVICE_TYPE_PURE_HOT_COOL_NEW,
     DEVICE_TYPE_PURE_HOT_COOL_LINK,
     DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E,
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_K,
+    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE,
+    DEVICE_TYPE_PURIFIER_HOT_COOL,
     Dyson360Eye,
     Dyson360Heurist,
     DysonDevice,
     DysonPureCool,
+    DysonPureCoolFormaldehyde,
     DysonPureCoolLink,
     DysonPureHotCool,
     DysonPureHotCoolLink,
-    DysonPurifierHumidifyCool,
+    DysonPureHumidifyCool,
+    DysonPurifierHumidifyCoolFormaldehyde,
     get_device,
 )
 
 from . import CREDENTIAL, SERIAL
 
 
 @pytest.mark.parametrize(
     "device_type,class_type",
     [
         (DEVICE_TYPE_360_EYE, Dyson360Eye),
         (DEVICE_TYPE_360_HEURIST, Dyson360Heurist),
         (DEVICE_TYPE_PURE_COOL_LINK_DESK, DysonPureCoolLink),
         (DEVICE_TYPE_PURE_COOL_LINK, DysonPureCoolLink),
         (DEVICE_TYPE_PURE_COOL, DysonPureCool),
-        (DEVICE_TYPE_PURIFIER_COOL_E, DysonPureCool),
-        (DEVICE_TYPE_PURIFIER_COOL_K, DysonPureCool),
+        (DEVICE_TYPE_PURE_COOL_FORMALDEHYDE, DysonPureCoolFormaldehyde),
         (DEVICE_TYPE_PURE_COOL_DESK, DysonPureCool),
         (DEVICE_TYPE_PURE_HOT_COOL_LINK, DysonPureHotCoolLink),
         (DEVICE_TYPE_PURE_HOT_COOL, DysonPureHotCool),
-        (DEVICE_TYPE_PURIFIER_HOT_COOL_E, DysonPureHotCool),
-        (DEVICE_TYPE_PURIFIER_HOT_COOL_K, DysonPureHotCool),
-        (DEVICE_TYPE_PURE_HUMIDIFY_COOL, DysonPurifierHumidifyCool),
-        (DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E, DysonPurifierHumidifyCool),
-        (DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_K, DysonPurifierHumidifyCool),
+        (DEVICE_TYPE_PURE_HOT_COOL_NEW, DysonPureHotCool),
+        (DEVICE_TYPE_PURE_HUMIDIFY_COOL, DysonPureHumidifyCool),
+        (DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE, DysonPurifierHumidifyCoolFormaldehyde),
+        (DEVICE_TYPE_PURIFIER_HOT_COOL, DysonPureHotCool),
     ],
 )
 def test_get_device(device_type: str, class_type: Type[DysonDevice]):
     """Test get_device."""
     device = get_device(SERIAL, CREDENTIAL, device_type)
     assert isinstance(device, class_type)
     assert device.serial == SERIAL
```

### Comparing `libdyson-neon-0.11.0/tests/test_pure_cool.py` & `libdyson-neon-0.9.0/tests/test_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_pure_cool_formaldehyde.py` & `libdyson-neon-0.9.0/tests/test_pure_cool_formaldehyde.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Tests for Pure Cool Formaldehyde"""
 
 import pytest
 
 from libdyson.const import (
-    DEVICE_TYPE_PURIFIER_COOL_E,
+    DEVICE_TYPE_PURE_COOL_FORMALDEHYDE,
     ENVIRONMENTAL_FAIL,
     ENVIRONMENTAL_INIT,
     ENVIRONMENTAL_OFF,
 )
-from libdyson.dyson_pure_cool import DysonPureCool
+from libdyson.dyson_pure_cool import DysonPureCoolFormaldehyde
 
 from . import CREDENTIAL, HOST, SERIAL
 from .mocked_mqtt import MockedMQTT
 from .test_pure_cool import STATUS as TEST_PURE_COOL_STATUS
 
-DEVICE_TYPE = DEVICE_TYPE_PURIFIER_COOL_E
+DEVICE_TYPE = DEVICE_TYPE_PURE_COOL_FORMALDEHYDE
 
 STATUS = TEST_PURE_COOL_STATUS
 ENVIRONMENTAL_DATA = {
     "data": {
         "tact": "OFF",
         "hact": "OFF",
         "pm25": "OFF",
@@ -32,15 +32,15 @@
         "hchr": "OFF",
     }
 }
 
 
 def test_properties(mqtt_client: MockedMQTT):
     """Test properties of Pure Cool Link Formaldehyde."""
-    device = DysonPureCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
+    device = DysonPureCoolFormaldehyde(SERIAL, CREDENTIAL, DEVICE_TYPE)
     device.connect(HOST)
 
     # Environmental
     assert device.particulate_matter_2_5 == ENVIRONMENTAL_OFF
     assert device.particulate_matter_10 == ENVIRONMENTAL_OFF
     assert device.volatile_organic_compounds == ENVIRONMENTAL_INIT
     assert device.nitrogen_dioxide == ENVIRONMENTAL_FAIL
```

### Comparing `libdyson-neon-0.11.0/tests/test_pure_cool_link.py` & `libdyson-neon-0.9.0/tests/test_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_pure_cool_missing_env_data.py` & `libdyson-neon-0.9.0/tests/test_purifier_humidify_cool_formaldehyde.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""Tests for Pure Cool Formaldehyde"""
+"""Tests for Purifier Humidify+Cool Formaldehyde"""
 
 import pytest
 
 from libdyson.const import (
-    DEVICE_TYPE_PURIFIER_COOL_E,
+    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE,
     ENVIRONMENTAL_FAIL,
     ENVIRONMENTAL_INIT,
     ENVIRONMENTAL_OFF,
 )
-from libdyson.dyson_pure_cool import DysonPureCool
+from libdyson.dyson_pure_humidify_cool import DysonPurifierHumidifyCoolFormaldehyde
 
 from . import CREDENTIAL, HOST, SERIAL
 from .mocked_mqtt import MockedMQTT
-from .test_pure_cool import STATUS as TEST_PURE_COOL_STATUS
+from .test_pure_humidify_cool import STATUS as TEST_PURE_HUMIDIFY_COOL_STATUS
 
-DEVICE_TYPE = DEVICE_TYPE_PURIFIER_COOL_E
+DEVICE_TYPE = DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_FORMALDEHYDE
 
-STATUS = TEST_PURE_COOL_STATUS
+STATUS = TEST_PURE_HUMIDIFY_COOL_STATUS
 ENVIRONMENTAL_DATA = {
     "data": {
         "tact": "OFF",
         "hact": "OFF",
         "pm25": "OFF",
         "pm10": "OFF",
         "va10": "INIT",
@@ -30,17 +30,17 @@
         "sltm": "OFF",
         "hcho": "OFF",
         "hchr": "OFF",
     }
 }
 
 
-def test_no_hcho(mqtt_client: MockedMQTT):
-    """Test properties of Pureifier Cool without Formaldehyde."""
-    device = DysonPureCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
+def test_properties(mqtt_client: MockedMQTT):
+    """Test properties of Purifier Humidify+Cool Formaldehyde."""
+    device = DysonPurifierHumidifyCoolFormaldehyde(SERIAL, CREDENTIAL, DEVICE_TYPE)
     device.connect(HOST)
 
     # Environmental
     assert device.particulate_matter_2_5 == ENVIRONMENTAL_OFF
     assert device.particulate_matter_10 == ENVIRONMENTAL_OFF
     assert device.volatile_organic_compounds == ENVIRONMENTAL_INIT
     assert device.nitrogen_dioxide == ENVIRONMENTAL_FAIL
@@ -53,51 +53,17 @@
             "pm25": "0009",
             "pm10": "0005",
             "va10": "0004",
             "noxl": "0011",
             "p25r": "0010",
             "p10r": "0009",
             "sltm": "OFF",
-            "hcho": "NONE",
+            "hcho": "0001",
             "hchr": "0002",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
     assert device.volatile_organic_compounds == 4
     assert device.nitrogen_dioxide == 11
-    assert device.formaldehyde is None
-
-
-def test_missing_data(mqtt_client: MockedMQTT):
-    """Test properties of a case where (hcho in this case) data is missing for some reason."""
-    device = DysonPureCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
-    device.connect(HOST)
-
-    # Environmental
-    assert device.particulate_matter_2_5 == ENVIRONMENTAL_OFF
-    assert device.particulate_matter_10 == ENVIRONMENTAL_OFF
-    assert device.volatile_organic_compounds == ENVIRONMENTAL_INIT
-    assert device.nitrogen_dioxide == ENVIRONMENTAL_FAIL
-    assert device.formaldehyde == ENVIRONMENTAL_OFF
-
-    mqtt_client._environmental_data = {
-        "data": {
-            "tact": "2977",
-            "hact": "0058",
-            "pm25": "0009",
-            "pm10": "0005",
-            "va10": "0004",
-            "noxl": "0011",
-            "p25r": "0010",
-            "p10r": "0009",
-            "sltm": "OFF",
-            "hchr": "0002",
-        }
-    }
-    device.request_environmental_data()
-    assert device.particulate_matter_2_5 == 9
-    assert device.particulate_matter_10 == 5
-    assert device.volatile_organic_compounds == 4
-    assert device.nitrogen_dioxide == 11
-    assert device.formaldehyde is None
+    assert device.formaldehyde == 1
```

### Comparing `libdyson-neon-0.11.0/tests/test_pure_hot_cool_link.py` & `libdyson-neon-0.9.0/tests/test_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-0.11.0/tests/test_pure_humidify_cool.py` & `libdyson-neon-0.9.0/tests/test_pure_humidify_cool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for Dyson Pure Humidity+Cool device."""
 
 import pytest
 
 from libdyson import (
     DEVICE_TYPE_PURE_HUMIDIFY_COOL,
-    DysonPurifierHumidifyCool,
+    DysonPureHumidifyCool,
     HumidifyOscillationMode,
     WaterHardness,
 )
 
 from . import CREDENTIAL, HOST, SERIAL
 from .mocked_mqtt import MockedMQTT
 from .test_fan_device import assert_command
@@ -29,15 +29,15 @@
         "cdrr": "0060",
     }
 }
 
 
 def test_properties(mqtt_client: MockedMQTT):
     """Test properties of Pure Hot+Cool Link."""
-    device = DysonPurifierHumidifyCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
+    device = DysonPureHumidifyCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
     device.connect(HOST)
 
     assert device.oscillation is True
     assert device.oscillation_mode == HumidifyOscillationMode.BREEZE
     assert device.humidification is True
     assert device.humidification_auto_mode is True
     assert device.target_humidity == 50
@@ -105,13 +105,13 @@
     mqtt_client: MockedMQTT,
     command: str,
     command_args: list,
     msg_data: dict,
 ):
     """Test commands of Pure Hot+Cool Link."""
     assert_command(
-        DysonPurifierHumidifyCool(SERIAL, CREDENTIAL, DEVICE_TYPE),
+        DysonPureHumidifyCool(SERIAL, CREDENTIAL, DEVICE_TYPE),
         mqtt_client,
         command,
         command_args,
         msg_data,
     )
```

### Comparing `libdyson-neon-0.11.0/tests/test_purifier_humidify_cool_formaldehyde.py` & `libdyson-neon-0.9.0/tests/test_vacuum.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,62 @@
-"""Tests for Purifier Humidify+Cool Formaldehyde"""
+"""Tests for Dyson vacuum base class."""
+from unittest.mock import patch
 
 import pytest
 
-from libdyson.const import (
-    DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E,
-    ENVIRONMENTAL_FAIL,
-    ENVIRONMENTAL_INIT,
-    ENVIRONMENTAL_OFF,
-)
-from libdyson.dyson_pure_humidify_cool import DysonPurifierHumidifyCool
+from libdyson import DEVICE_TYPE_360_EYE, CleaningType, Dyson360Eye, VacuumState
 
 from . import CREDENTIAL, HOST, SERIAL
 from .mocked_mqtt import MockedMQTT
-from .test_pure_humidify_cool import STATUS as TEST_PURE_HUMIDIFY_COOL_STATUS
 
-DEVICE_TYPE = DEVICE_TYPE_PURIFIER_HUMIDIFY_COOL_E
-
-STATUS = TEST_PURE_HUMIDIFY_COOL_STATUS
-ENVIRONMENTAL_DATA = {
-    "data": {
-        "tact": "OFF",
-        "hact": "OFF",
-        "pm25": "OFF",
-        "pm10": "OFF",
-        "va10": "INIT",
-        "noxl": "FAIL",
-        "p25r": "OFF",
-        "p10r": "OFF",
-        "sltm": "OFF",
-        "hcho": "OFF",
-        "hchr": "OFF",
-    }
+STATUS = {
+    "state": "INACTIVE_CHARGED",
+    "fullCleanType": "",
+    "cleanId": "",
+    "globalPosition": [0, 0],
+    "batteryChargeLevel": 100,
 }
 
 
+@pytest.fixture(autouse=True)
+def mqtt_client() -> MockedMQTT:
+    """Return mocked mqtt client."""
+    mocked_mqtt = MockedMQTT(
+        HOST,
+        SERIAL,
+        CREDENTIAL,
+        f"{DEVICE_TYPE_360_EYE}/{SERIAL}/command",
+        f"{DEVICE_TYPE_360_EYE}/{SERIAL}/status",
+        STATUS,
+    )
+    with patch("libdyson.dyson_device.mqtt.Client", mocked_mqtt.refersh):
+        yield mocked_mqtt
+
+
 def test_properties(mqtt_client: MockedMQTT):
-    """Test properties of Purifier Humidify+Cool Formaldehyde."""
-    device = DysonPurifierHumidifyCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
+    """Test properties of vaccums."""
+    device = Dyson360Eye(SERIAL, CREDENTIAL)
     device.connect(HOST)
 
-    # Environmental
-    assert device.particulate_matter_2_5 == ENVIRONMENTAL_OFF
-    assert device.particulate_matter_10 == ENVIRONMENTAL_OFF
-    assert device.volatile_organic_compounds == ENVIRONMENTAL_INIT
-    assert device.nitrogen_dioxide == ENVIRONMENTAL_FAIL
-    assert device.formaldehyde == ENVIRONMENTAL_OFF
-
-    mqtt_client._environmental_data = {
-        "data": {
-            "tact": "2977",
-            "hact": "0058",
-            "pm25": "0009",
-            "pm10": "0005",
-            "va10": "0004",
-            "noxl": "0011",
-            "p25r": "0010",
-            "p10r": "0009",
-            "sltm": "OFF",
-            "hcho": "0001",
-            "hchr": "0002",
-        }
+    assert device.state == VacuumState.INACTIVE_CHARGED
+    assert device.cleaning_type is None
+    assert device.cleaning_id is None
+    assert device.position == (0, 0)
+    assert device.is_charging is True
+    assert device.battery_level == 100
+
+    clean_id = "b599d00f-6f3b-401a-9c05-69877251e843"
+    new_status = {
+        "oldstate": "INACTIVE_CHARGED",
+        "newstate": "FULL_CLEAN_RUNNING",
+        "fullCleanType": "immediate",
+        "cleanId": clean_id,
+        "globalPosition": [],
+        "batteryChargeLevel": 30,
     }
-    device.request_environmental_data()
-    assert device.particulate_matter_2_5 == 9
-    assert device.particulate_matter_10 == 5
-    assert device.volatile_organic_compounds == 4
-    assert device.nitrogen_dioxide == 11
-    assert device.formaldehyde == 1
+    mqtt_client.state_change(new_status)
+    assert device.state == VacuumState.FULL_CLEAN_RUNNING
+    assert device.cleaning_type == CleaningType.IMMEDIATE
+    assert device.cleaning_id == clean_id
+    assert device.position is None
+    assert device.is_charging is False
+    assert device.battery_level == 30
```

### Comparing `libdyson-neon-0.11.0/tests/test_utils.py` & `libdyson-neon-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

