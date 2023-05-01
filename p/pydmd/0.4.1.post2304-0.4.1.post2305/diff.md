# Comparing `tmp/pydmd-0.4.1.post2304.tar.gz` & `tmp/pydmd-0.4.1.post2305.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmd-0.4.1.post2304.tar", last modified: Sat Apr  1 02:53:09 2023, max compression
+gzip compressed data, was "pydmd-0.4.1.post2305.tar", last modified: Mon May  1 02:59:59 2023, max compression
```

## Comparing `pydmd-0.4.1.post2304.tar` & `pydmd-0.4.1.post2305.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:53:09.496740 pydmd-0.4.1.post2304/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-01 02:53:09.496740 pydmd-0.4.1.post2304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:53:09.492740 pydmd-0.4.1.post2304/pydmd/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41544 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/bopdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/cdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/dmd_modes_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/dmdbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/dmdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/dmdoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/fbdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/hankeldmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/havok.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/hodmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/mrdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/optdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/paramdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/pidmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/pidmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/rdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/spdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/subspacedmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pydmd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:53:09.492740 pydmd-0.4.1.post2304/pydmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-01 02:53:09.000000 pydmd-0.4.1.post2304/pydmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-01 02:53:09.000000 pydmd-0.4.1.post2304/pydmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 02:53:09.000000 pydmd-0.4.1.post2304/pydmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 02:53:09.000000 pydmd-0.4.1.post2304/pydmd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-01 02:53:09.000000 pydmd-0.4.1.post2304/pydmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-01 02:53:09.000000 pydmd-0.4.1.post2304/pydmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 02:53:09.496740 pydmd-0.4.1.post2304/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:53:09.496740 pydmd-0.4.1.post2304/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/tests/test_bopdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-04-01 02:52:54.000000 pydmd-0.4.1.post2304/tests/test_cdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_dmd_modes_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_dmdbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_dmdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_dmdoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_fbdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_hankeldmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_havok.py
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_hodmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_mrdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_optdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_paramdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_pidmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_rdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_spdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-01 02:52:55.000000 pydmd-0.4.1.post2304/tests/test_subspacedmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.471438 pydmd-0.4.1.post2305/pydmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42614 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/bopdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/cdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmd_modes_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/dmdoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/fbdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/hankeldmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/havok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/hodmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/mrdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/optdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/paramdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/pidmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/pidmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/rdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/spdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/subspacedmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pydmd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.471438 pydmd-0.4.1.post2305/pydmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 02:59:59.000000 pydmd-0.4.1.post2305/pydmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:59:59.475438 pydmd-0.4.1.post2305/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_bopdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_cdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmd_modes_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_dmdoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_fbdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_hankeldmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_havok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_hodmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_mrdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_optdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_paramdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_pidmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_rdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_spdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-01 02:59:47.000000 pydmd-0.4.1.post2305/tests/test_subspacedmd.py
```

### Comparing `pydmd-0.4.1.post2304/LICENSE.rst` & `pydmd-0.4.1.post2305/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/PKG-INFO` & `pydmd-0.4.1.post2305/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pydmd
-Version: 0.4.1.post2304
+Version: 0.4.1.post2305
 Summary: Python Dynamic Mode Decomposition.
 Home-page: https://github.com/mathLab/PyDMD
-Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi
-Author-email: demo.nicola@gmail.com, marcotez@gmail.com, andreuzzi.francesco@gmail.com
+Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi, Sara Ichinaga
+Author-email: pydmd.info@gmail.com
 License: MIT
 Keywords: dynamic-mode-decomposition dmd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pydmd-0.4.1.post2304/README.md` & `pydmd-0.4.1.post2305/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,29 +35,25 @@
 * [Documentation](#documentation)
 * [Testing](#testing)
 * [Examples and Tutorials](#examples-and-tutorials)
 * [Awards](#awards)
 * [How to cite](#how-to-cite)
 	* [References](#references)
 	* [Recent works with PyDMD](#recent-works-with-pydmd)
-* [Authors and contributors](#authors-and-contributors)
-* [How to contribute](#how-to-contribute)
-	* [Submitting a patch](#submitting-a-patch)
+* [Developers and contributors](#developers-and-contributors)
+* [Funding](#funding)
 * [License](#license)
 
 ## Description
 **PyDMD** is a Python package that uses **Dynamic Mode Decomposition** for a data-driven model simplification based on spatiotemporal coherent structures.
 
 Dynamic Mode Decomposition (DMD) is a model reduction algorithm developed by Schmid (see "Dynamic mode decomposition of numerical and experimental data"). Since then has emerged as a powerful tool for analyzing the dynamics of nonlinear systems. DMD relies only on the high-fidelity measurements, like experimental data and numerical simulations, so it is an equation-free algorithm. Its popularity is also due to the fact that it does not make any assumptions about the underlying system. See Kutz ("Dynamic Mode Decomposition: Data-Driven Modeling of Complex Systems") for a comprehensive overview of the algorithm and its connections to the Koopman-operator analysis, initiated in Koopman ("Hamiltonian systems and transformation in Hilbert space"), along with examples in computational fluid dynamics.
 
-In the last years many variants arose, such as multiresolution DMD, compressed DMD, forward backward DMD, and higher order DMD among others, in order to deal with noisy data, big dataset, or spurious data for example.
+In the last years many variants arose, such as multiresolution DMD, compressed DMD, forward backward DMD, higher order DMD, and physics-informed DMD among others, in order to deal with noisy data, big dataset, or spurius data for example. We implemented in Python the majority of the DMD extensions currently present in the literature with a user friendly interface. We also provide many tutorials that show all the characteristics of the software. See the [**Examples**](#examples) section below and the [**Tutorials**](tutorials/README.md) to have an idea of the potential of this package.
 
-In PyDMD we implemented the majority of the variants mentioned above with a user friendly interface. See the [**Examples**](#examples) section below and the [**Tutorials**](tutorials/README.md) to have an idea of the potential of this package.
-
-The research in the field is growing both in computational fluid dynamic and in structural mechanics, due to the equation-free nature of the model.
 <p align="center">
     <img src="readme/pydmd_capabilities.png" width="800" />
 </p>
 
 
 
 ## Dependencies and installation
@@ -81,16 +77,15 @@
 ```
 
 To install the package just type:
 ```bash
 > pip install -e .
 ```
 
-To uninstall the package you have to rerun the installation and record the installed files in order to remove them:
-
+To uninstall the package type:
 ```bash
 > pip uninstall pydmd
 ```
 
 ## Documentation
 **PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for code documentation. You can view the documentation online [here](http://mathlab.github.io/PyDMD/). To build the html version of the docs locally simply:
 
@@ -178,22 +173,39 @@
 
 * Demo, Tezzele, Mola, Rozza. *An efficient shape parametrisation by free-form deformation enhanced by active subspace for hull hydrodynamic ship design problems in open source environment*. 2018. [[arXiv](https://arxiv.org/abs/1801.06369)].
 
 * Tezzele, Demo, Stabile, Mola, Rozza. *Enhancing CFD predictions in shape design problems by model and parameter space reduction*. 2020. [[arXiv](https://arxiv.org/abs/2001.05237)].
 
 * Tezzele. *Data-driven parameter and model order reduction for industrial optimisation problems with applications in naval engineering*, PhD Thesis. 2021. [[Iris](http://hdl.handle.net/20.500.11767/124569)].
 
-## Contributing
-We warmly thank all the contributors that have supported PyDMD! The financial support of the [AROMA-CFD ERC CoG project](https://people.sissa.it/~grozza/aroma-cfd/) project is also gratefully acknowledged.
+## Developers and contributors
+The main developers are 
+<p align="center">
+    <img src="readme/main_developers.png" width="800" />
+</p>
+
+We warmly thank all the contributors that have supported PyDMD!
 
 Do you want to join the team? Read the [Contributing guidelines](.github/CONTRIBUTING.md) and the [Tutorials for Developers](tutorials#tutorials-for-developers) before starting to play!
 
 
 <a href="https://github.com/mathLab/PyDMD/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=mathLab/PyDMD" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
+
+## Funding
+A significant part of PyDMD has been written either as a by-product for other projects people were funded for, or by people on university-funded positions. There are probably many of such projects that have led to some development of PyDMD. We are very grateful for this support!
+
+Beyond this, PyDMD has also been supported by some dedicated projects that have allowed us to work on extensions, documentation, training and dissemination that would otherwise not have been possible. In particular, we acknowledge the following sources of support with great gratitude:
+
+* [H2020 ERC CoG 2015 AROMA-CFD project 681447](https://people.sissa.it/~grozza/aroma-cfd/), P.I. Professor [Gianluigi Rozza](https://people.sissa.it/~grozza) at [SISSA mathLab](https://mathlab.sissa.it/).
+* FSE HEaD project [Bulbous Bow Shape Optimization through Reduced Order Modelling](https://mathlab.sissa.it/project/ottimizzazione-di-forme-prodiere-e-poppiere-di-carena-mediante-luso-di-algoritmi-parametrici), FVG, Italy.
+<p align="center">
+    <img src="readme/logos_funding.png" width="800" />
+</p>
+
 ## License
 
 See the [LICENSE](LICENSE.rst) file for license rights and limitations (MIT).
```

#### html2text {}

```diff
@@ -4,53 +4,51 @@
     //app.codacy.com/project/badge/Grade/c36adbea2e4a44eb8c0e4505b75e8245]
 **PyDMD**: Python Dynamic Mode Decomposition ## Table of contents *
 [Description](#description) * [Dependencies and installation](#dependencies-
 and-installation) * [Installing via PIP](#installing-via-pip) * [Installing
 from source](#installing-from-source) * [Documentation](#documentation) *
 [Testing](#testing) * [Examples and Tutorials](#examples-and-tutorials) *
 [Awards](#awards) * [How to cite](#how-to-cite) * [References](#references) *
-[Recent works with PyDMD](#recent-works-with-pydmd) * [Authors and
-contributors](#authors-and-contributors) * [How to contribute](#how-to-
-contribute) * [Submitting a patch](#submitting-a-patch) * [License](#license)
-## Description **PyDMD** is a Python package that uses **Dynamic Mode
-Decomposition** for a data-driven model simplification based on spatiotemporal
-coherent structures. Dynamic Mode Decomposition (DMD) is a model reduction
-algorithm developed by Schmid (see "Dynamic mode decomposition of numerical and
-experimental data"). Since then has emerged as a powerful tool for analyzing
-the dynamics of nonlinear systems. DMD relies only on the high-fidelity
-measurements, like experimental data and numerical simulations, so it is an
-equation-free algorithm. Its popularity is also due to the fact that it does
-not make any assumptions about the underlying system. See Kutz ("Dynamic Mode
-Decomposition: Data-Driven Modeling of Complex Systems") for a comprehensive
-overview of the algorithm and its connections to the Koopman-operator analysis,
-initiated in Koopman ("Hamiltonian systems and transformation in Hilbert
-space"), along with examples in computational fluid dynamics. In the last years
-many variants arose, such as multiresolution DMD, compressed DMD, forward
-backward DMD, and higher order DMD among others, in order to deal with noisy
-data, big dataset, or spurious data for example. In PyDMD we implemented the
-majority of the variants mentioned above with a user friendly interface. See
+[Recent works with PyDMD](#recent-works-with-pydmd) * [Developers and
+contributors](#developers-and-contributors) * [Funding](#funding) * [License]
+(#license) ## Description **PyDMD** is a Python package that uses **Dynamic
+Mode Decomposition** for a data-driven model simplification based on
+spatiotemporal coherent structures. Dynamic Mode Decomposition (DMD) is a model
+reduction algorithm developed by Schmid (see "Dynamic mode decomposition of
+numerical and experimental data"). Since then has emerged as a powerful tool
+for analyzing the dynamics of nonlinear systems. DMD relies only on the high-
+fidelity measurements, like experimental data and numerical simulations, so it
+is an equation-free algorithm. Its popularity is also due to the fact that it
+does not make any assumptions about the underlying system. See Kutz ("Dynamic
+Mode Decomposition: Data-Driven Modeling of Complex Systems") for a
+comprehensive overview of the algorithm and its connections to the Koopman-
+operator analysis, initiated in Koopman ("Hamiltonian systems and
+transformation in Hilbert space"), along with examples in computational fluid
+dynamics. In the last years many variants arose, such as multiresolution DMD,
+compressed DMD, forward backward DMD, higher order DMD, and physics-informed
+DMD among others, in order to deal with noisy data, big dataset, or spurius
+data for example. We implemented in Python the majority of the DMD extensions
+currently present in the literature with a user friendly interface. We also
+provide many tutorials that show all the characteristics of the software. See
 the [**Examples**](#examples) section below and the [**Tutorials**](tutorials/
-README.md) to have an idea of the potential of this package. The research in
-the field is growing both in computational fluid dynamic and in structural
-mechanics, due to the equation-free nature of the model.
+README.md) to have an idea of the potential of this package.
                         [readme/pydmd_capabilities.png]
 ## Dependencies and installation **PyDMD** requires requires `numpy`, `scipy`,
 `matplotlib`, `future`, `sphinx` (for the documentation) and `pytest` (for
 local test). The code is tested for Python 3, while compatibility of Python 2
 is not guaranteed anymore. It can be installed using `pip` or directly from the
 source code. ### Installing via PIP Mac and Linux users can install pre-built
 binary packages using pip. To install the package just type: ```bash > pip
 install pydmd ``` To uninstall the package: ```bash > pip uninstall pydmd ```
 ### Installing from source The official distribution is on GitHub, and you can
 clone the repository using ```bash > git clone https://github.com/mathLab/PyDMD
 ``` To install the package just type: ```bash > pip install -e . ``` To
-uninstall the package you have to rerun the installation and record the
-installed files in order to remove them: ```bash > pip uninstall pydmd ``` ##
-Documentation **PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for
-code documentation. You can view the documentation online [here](http://
+uninstall the package type: ```bash > pip uninstall pydmd ``` ## Documentation
+**PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for code
+documentation. You can view the documentation online [here](http://
 mathlab.github.io/PyDMD/). To build the html version of the docs locally
 simply: ```bash > cd docs > make html ``` The generated html can be found in
 `docs/build/html`. Open up the `index.html` you find there to browse. ##
 Testing We are using GitHub actions for Continuous Integration. You can check
 the current status [here](https://github.com/mathLab/PyDMD/actions). To run
 tests locally (`pytest` is required): ```bash > pytest ``` ## Examples and
 Tutorials You can find useful tutorials on how to use the package in the
@@ -129,16 +127,31 @@
 by free-form deformation enhanced by active subspace for hull hydrodynamic ship
 design problems in open source environment*. 2018. [[arXiv](https://arxiv.org/
 abs/1801.06369)]. * Tezzele, Demo, Stabile, Mola, Rozza. *Enhancing CFD
 predictions in shape design problems by model and parameter space reduction*.
 2020. [[arXiv](https://arxiv.org/abs/2001.05237)]. * Tezzele. *Data-driven
 parameter and model order reduction for industrial optimisation problems with
 applications in naval engineering*, PhD Thesis. 2021. [[Iris](http://
-hdl.handle.net/20.500.11767/124569)]. ## Contributing We warmly thank all the
-contributors that have supported PyDMD! The financial support of the [AROMA-CFD
-ERC CoG project](https://people.sissa.it/~grozza/aroma-cfd/) project is also
-gratefully acknowledged. Do you want to join the team? Read the [Contributing
-guidelines](.github/CONTRIBUTING.md) and the [Tutorials for Developers]
-(tutorials#tutorials-for-developers) before starting to play! [https://
-contrib.rocks/image?repo=mathLab/PyDMD] Made with [contrib.rocks](https://
-contrib.rocks). ## License See the [LICENSE](LICENSE.rst) file for license
-rights and limitations (MIT).
+hdl.handle.net/20.500.11767/124569)]. ## Developers and contributors The main
+developers are
+                         [readme/main_developers.png]
+We warmly thank all the contributors that have supported PyDMD! Do you want to
+join the team? Read the [Contributing guidelines](.github/CONTRIBUTING.md) and
+the [Tutorials for Developers](tutorials#tutorials-for-developers) before
+starting to play! [https://contrib.rocks/image?repo=mathLab/PyDMD] Made with
+[contrib.rocks](https://contrib.rocks). ## Funding A significant part of PyDMD
+has been written either as a by-product for other projects people were funded
+for, or by people on university-funded positions. There are probably many of
+such projects that have led to some development of PyDMD. We are very grateful
+for this support! Beyond this, PyDMD has also been supported by some dedicated
+projects that have allowed us to work on extensions, documentation, training
+and dissemination that would otherwise not have been possible. In particular,
+we acknowledge the following sources of support with great gratitude: * [H2020
+ERC CoG 2015 AROMA-CFD project 681447](https://people.sissa.it/~grozza/aroma-
+cfd/), P.I. Professor [Gianluigi Rozza](https://people.sissa.it/~grozza) at
+[SISSA mathLab](https://mathlab.sissa.it/). * FSE HEaD project [Bulbous Bow
+Shape Optimization through Reduced Order Modelling](https://mathlab.sissa.it/
+project/ottimizzazione-di-forme-prodiere-e-poppiere-di-carena-mediante-luso-di-
+algoritmi-parametrici), FVG, Italy.
+                          [readme/logos_funding.png]
+## License See the [LICENSE](LICENSE.rst) file for license rights and
+limitations (MIT).
```

### Comparing `pydmd-0.4.1.post2304/pydmd/__init__.py` & `pydmd-0.4.1.post2305/pydmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/bopdmd.py` & `pydmd-0.4.1.post2305/pydmd/bopdmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -136,14 +136,15 @@
             use_fulljac,
             verbose,
         )
         self._varpro_opts_warn()
 
         self._modes = None
         self._eigenvalues = None
+        self._modes_std = None
         self._eigenvalues_std = None
         self._amplitudes_std = None
         self._Atilde = None
         self._A = None
 
     @property
     def varpro_opts(self):
@@ -189,14 +190,24 @@
         Get the eigenvalues standard deviation.
 
         :return: eigenvalues standard deviation.
         :rtype: numpy.ndarray
         """
         return self._eigenvalues_std
 
+    @property
+    def modes_std(self):
+        """
+        Get the modes standard deviation.
+
+        :return: modes standard deviation.
+        :rtype: numpy.ndarray
+        """
+        return self._modes_std
+
     def _varpro_opts_warn(self):
         """
         Checks the validity of the parameter values in _varpro_opts.
         Throws an error if any parameter value has an invalid type and
         generates a warning if any value lies outside of the recommended range.
         """
         # Generate dictionary of recommended value range for each parameter.
@@ -615,21 +626,24 @@
             self._modes = w_0
             self._eigenvalues = e_0
             self._Atilde = Atilde_0
             self._A = A_0
             return b_0
 
         # Perform BOP-DMD.
-        # Initialize bagging result storage.
-        all_w = np.empty((self._num_trials, *w_0.shape), dtype="complex")
-        all_e = np.empty((self._num_trials, *e_0.shape), dtype="complex")
-        all_b = np.empty((self._num_trials, *b_0.shape), dtype="complex")
+        # Initialize storage for values needed for stat computations.
+        w_sum = np.zeros(w_0.shape, dtype="complex")
+        e_sum = np.zeros(e_0.shape, dtype="complex")
+        b_sum = np.zeros(b_0.shape, dtype="complex")
+        w_sum2 = np.zeros(w_0.shape, dtype="complex")
+        e_sum2 = np.zeros(e_0.shape, dtype="complex")
+        b_sum2 = np.zeros(b_0.shape, dtype="complex")
 
         # Perform num_trials many trials of optimized dmd.
-        for i in range(self._num_trials):
+        for _ in range(self._num_trials):
             H_i, subset_inds = self._bag(H, self._trial_size)
             w_i, e_i, b_i, _, _ = self._single_trial_compute_operator(
                 H_i, t[subset_inds], e_0
             )
 
             # Set the sorting style if _eig_sort is "auto".
             if self._eig_sort == "auto":
@@ -651,21 +665,38 @@
                 e_i_real_imag_swapped = e_i.imag + (1j * e_i.real)
                 sorted_inds = np.argsort(e_i_real_imag_swapped)
             elif self._eig_sort == "abs":
                 sorted_inds = np.argsort(np.abs(e_i))
             else:
                 raise ValueError("Provided eig_sort method is not supported.")
 
-            all_w[i] = w_i[:, sorted_inds]
-            all_e[i] = e_i[sorted_inds]
-            all_b[i] = b_i[sorted_inds]
-
-        # Compute and use the average optimized dmd results.
-        self._modes = np.mean(all_w, axis=0)
-        self._eigenvalues = np.mean(all_e, axis=0)
+            # Add to iterative sums.
+            w_sum += w_i[:, sorted_inds]
+            e_sum += e_i[sorted_inds]
+            b_sum += b_i[sorted_inds]
+
+            # Add to iterative sums of squares.
+            w_sum2 += np.abs(w_i[:, sorted_inds]) ** 2
+            e_sum2 += np.abs(e_i[sorted_inds]) ** 2
+            b_sum2 += np.abs(b_i[sorted_inds]) ** 2
+
+        # Compute the BOP-DMD statistics.
+        w_mu = w_sum / self._num_trials
+        e_mu = e_sum / self._num_trials
+        b_mu = b_sum / self._num_trials
+        w_std = np.sqrt(np.abs(w_sum2 / self._num_trials - np.abs(w_mu) ** 2))
+        e_std = np.sqrt(np.abs(e_sum2 / self._num_trials - np.abs(e_mu) ** 2))
+        b_std = np.sqrt(np.abs(b_sum2 / self._num_trials - np.abs(b_mu) ** 2))
+
+        # Save the BOP-DMD statistics.
+        self._modes = w_mu
+        self._eigenvalues = e_mu
+        self._modes_std = w_std
+        self._eigenvalues_std = e_std
+        self._amplitudes_std = b_std
 
         # Compute Atilde using the average optimized dmd results.
         w_proj = self._proj_basis.conj().T.dot(self._modes)
         self._Atilde = np.linalg.multi_dot(
             [w_proj, np.diag(self._eigenvalues), np.linalg.pinv(w_proj)]
         )
         # Compute A if requested.
@@ -674,19 +705,15 @@
                 [
                     self._modes,
                     np.diag(self._eigenvalues),
                     np.linalg.pinv(self._modes),
                 ]
             )
 
-        # Compute and save the standard deviation of the optimized dmd results.
-        self._eigenvalues_std = np.std(all_e, axis=0)
-        self._amplitudes_std = np.std(all_b, axis=0)
-
-        return np.mean(all_b, axis=0)
+        return b_mu
 
 
 class BOPDMD(DMDBase):
     """
     Bagging, Optimized Dynamic Mode Decomposition.
 
     :param svd_rank: The rank for the truncation; If 0, the method computes the
@@ -894,25 +921,33 @@
         Get the amplitudes standard deviation.
 
         :return: amplitudes standard deviation.
         :rtype: numpy.ndarray
         """
         return self.operator.amplitudes_std
 
-
     @property
     def eigenvalues_std(self):
         """
         Get the eigenvalues standard deviation.
 
         :return: eigenvalues standard deviation.
         :rtype: numpy.ndarray
         """
         return self.operator.eigenvalues_std
 
+    @property
+    def modes_std(self):
+        """
+        Get the modes standard deviation.
+
+        :return: modes standard deviation.
+        :rtype: numpy.ndarray
+        """
+        return self.operator.modes_std
 
     def print_varpro_opts(self):
         """
         Prints a formatted information string that displays all chosen
         variable projection parameter values.
         """
         if self._Atilde is None:
@@ -992,15 +1027,15 @@
             msg = (
                 "The number of columns in the data matrix X must match "
                 "the number of time points in the time vector t."
             )
             raise ValueError(msg)
 
         # Compute the rank of the fit.
-        self._svd_rank = compute_rank(self.snapshots, self._svd_rank)
+        self._svd_rank = int(compute_rank(self.snapshots, self._svd_rank))
 
         # Set/check the projection basis.
         if self._proj_basis is None and self._use_proj:
             self._proj_basis = compute_svd(self.snapshots, self._svd_rank)[0]
         elif self._proj_basis is None and not self._use_proj:
             self._proj_basis = compute_svd(self.snapshots, -1)[0]
         elif (
```

### Comparing `pydmd-0.4.1.post2304/pydmd/cdmd.py` & `pydmd-0.4.1.post2305/pydmd/cdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/dmd.py` & `pydmd-0.4.1.post2305/pydmd/dmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/dmd_modes_tuner.py` & `pydmd-0.4.1.post2305/pydmd/dmd_modes_tuner.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/dmdbase.py` & `pydmd-0.4.1.post2305/pydmd/dmdbase.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/dmdc.py` & `pydmd-0.4.1.post2305/pydmd/dmdc.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/dmdoperator.py` & `pydmd-0.4.1.post2305/pydmd/dmdoperator.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/fbdmd.py` & `pydmd-0.4.1.post2305/pydmd/fbdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/hankeldmd.py` & `pydmd-0.4.1.post2305/pydmd/hankeldmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
     @property
     def operator(self):
         return self._sub_dmd.operator
 
     @property
     def svd_rank(self):
         return self._sub_dmd.svd_rank
-    
+
     @property
     def ho_snapshots(self):
         """
         Get the time-delay data matrix.
 
         :return: the matrix that contains the time-delayed data.
         :rtype: numpy.ndarray
```

### Comparing `pydmd-0.4.1.post2304/pydmd/havok.py` & `pydmd-0.4.1.post2305/pydmd/havok.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/hodmd.py` & `pydmd-0.4.1.post2305/pydmd/hodmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/mrdmd.py` & `pydmd-0.4.1.post2305/pydmd/mrdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/optdmd.py` & `pydmd-0.4.1.post2305/pydmd/optdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/paramdmd.py` & `pydmd-0.4.1.post2305/pydmd/paramdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/pidmd.py` & `pydmd-0.4.1.post2305/pydmd/pidmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/pidmd_utils.py` & `pydmd-0.4.1.post2305/pydmd/pidmd_utils.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/plotter.py` & `pydmd-0.4.1.post2305/pydmd/plotter.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/rdmd.py` & `pydmd-0.4.1.post2305/pydmd/rdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/snapshots.py` & `pydmd-0.4.1.post2305/pydmd/snapshots.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/spdmd.py` & `pydmd-0.4.1.post2305/pydmd/spdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/subspacedmd.py` & `pydmd-0.4.1.post2305/pydmd/subspacedmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd/utils.py` & `pydmd-0.4.1.post2305/pydmd/utils.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/pydmd.egg-info/PKG-INFO` & `pydmd-0.4.1.post2305/pydmd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pydmd
-Version: 0.4.1.post2304
+Version: 0.4.1.post2305
 Summary: Python Dynamic Mode Decomposition.
 Home-page: https://github.com/mathLab/PyDMD
-Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi
-Author-email: demo.nicola@gmail.com, marcotez@gmail.com, andreuzzi.francesco@gmail.com
+Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi, Sara Ichinaga
+Author-email: pydmd.info@gmail.com
 License: MIT
 Keywords: dynamic-mode-decomposition dmd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pydmd-0.4.1.post2304/pydmd.egg-info/SOURCES.txt` & `pydmd-0.4.1.post2305/pydmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/setup.py` & `pydmd-0.4.1.post2305/setup.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_bopdmd.py` & `pydmd-0.4.1.post2305/tests/test_bopdmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,81 +74,71 @@
     assert bopdmd.atilde.shape == (2, 2)
     assert bopdmd.A.shape == (2, 2)
 
 
 def test_eigs():
     """
     Tests that the computed eigenvalues are accurate for the following cases:
-    - standard optimized dmd, default parameters, even dataset
-    - standard optimized dmd, default parameters, uneven dataset
-    - standard optimized dmd, rank truncated
+    - standard optimized dmd, even dataset
+    - standard optimized dmd, uneven dataset
     - standard optimized dmd, fit full data
     - optimized dmd with bagging
     """
-    bopdmd = BOPDMD()
+    bopdmd = BOPDMD(svd_rank=2)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(sort_imag(bopdmd.eigs), expected_eigs)
 
-    bopdmd = BOPDMD()
-    bopdmd.fit(Z_uneven, t_uneven)
-    np.testing.assert_allclose(sort_imag(bopdmd.eigs), expected_eigs)
-
     bopdmd = BOPDMD(svd_rank=2)
-    bopdmd.fit(Z, t)
+    bopdmd.fit(Z_uneven, t_uneven)
     np.testing.assert_allclose(sort_imag(bopdmd.eigs), expected_eigs)
 
-    bopdmd = BOPDMD(use_proj=False)
+    bopdmd = BOPDMD(svd_rank=2, use_proj=False)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(sort_imag(bopdmd.eigs), expected_eigs)
 
-    bopdmd = BOPDMD(num_trials=100, trial_size=0.2)
+    bopdmd = BOPDMD(svd_rank=2, num_trials=100, trial_size=0.2)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(sort_imag(bopdmd.eigs), expected_eigs)
 
 
 def test_A():
     """
     Tests that the computed A matrix is accurate for the following cases:
-    - standard optimized dmd, default parameters, even dataset
-    - standard optimized dmd, default parameters, uneven dataset
-    - standard optimized dmd, rank truncated
+    - standard optimized dmd, even dataset
+    - standard optimized dmd, uneven dataset
     - standard optimized dmd, fit full data
     - optimized dmd with bagging
     """
-    bopdmd = BOPDMD(compute_A=True)
+    bopdmd = BOPDMD(svd_rank=2, compute_A=True)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(bopdmd.A, expected_A)
 
-    bopdmd = BOPDMD(compute_A=True)
-    bopdmd.fit(Z_uneven, t_uneven)
-    np.testing.assert_allclose(bopdmd.A, expected_A)
-
     bopdmd = BOPDMD(svd_rank=2, compute_A=True)
-    bopdmd.fit(Z, t)
+    bopdmd.fit(Z_uneven, t_uneven)
     np.testing.assert_allclose(bopdmd.A, expected_A)
 
-    bopdmd = BOPDMD(compute_A=True, use_proj=False)
+    bopdmd = BOPDMD(svd_rank=2, compute_A=True, use_proj=False)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(bopdmd.A, expected_A)
 
-    bopdmd = BOPDMD(compute_A=True, num_trials=100, trial_size=0.2)
+    bopdmd = BOPDMD(svd_rank=2, compute_A=True, num_trials=100, trial_size=0.2)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(bopdmd.A, expected_A)
 
 
 def test_reconstruction():
     """
-    Tests the accuracy of the reconstructed data for the default parameters.
+    Tests the accuracy of the reconstructed data.
     Tests for both standard optimized dmd and BOP-DMD.
     """
-    bopdmd = BOPDMD()
+    bopdmd = BOPDMD(svd_rank=2)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(bopdmd.reconstructed_data, Z, rtol=1e-5)
 
-    bopdmd = BOPDMD(num_trials=100, trial_size=0.2)
+    bopdmd = BOPDMD(svd_rank=2, num_trials=100, trial_size=0.2)
     bopdmd.fit(Z, t)
     np.testing.assert_allclose(bopdmd.reconstructed_data, Z, rtol=1e-5)
 
 
 def test_forecast():
     """
     Tests that the BOP-DMD model generalizes to data not used for training.
@@ -156,35 +146,35 @@
     - Generalizing to long dataset after training on short, even dataset
         without bagging.
     - Generalizing to long dataset after training on short, uneven dataset
         without bagging.
     - Generalizing to long dataset after training on short, even dataset
         with bagging.
     """
-    bopdmd = BOPDMD()
+    bopdmd = BOPDMD(svd_rank=2)
     bopdmd.fit(Z, t)
-    np.testing.assert_allclose(bopdmd.forecast(t_long), Z_long, rtol=1e-4)
+    np.testing.assert_allclose(bopdmd.forecast(t_long), Z_long, rtol=1e-3)
 
-    bopdmd = BOPDMD()
+    bopdmd = BOPDMD(svd_rank=2)
     bopdmd.fit(Z_uneven, t_uneven)
-    np.testing.assert_allclose(bopdmd.forecast(t_long), Z_long, rtol=1e-4)
+    np.testing.assert_allclose(bopdmd.forecast(t_long), Z_long, rtol=1e-3)
 
-    bopdmd = BOPDMD(num_trials=100, trial_size=0.2)
+    bopdmd = BOPDMD(svd_rank=2, num_trials=100, trial_size=0.2)
     bopdmd.fit(Z, t)
-    np.testing.assert_allclose(bopdmd.forecast(t_long)[0], Z_long, rtol=1e-4)
+    np.testing.assert_allclose(bopdmd.forecast(t_long)[0], Z_long, rtol=1e-3)
 
 
 def test_compute_A():
     """
     Tests that the BOPDMD module appropriately calculates or doesn't calculate
     A depending on the compute_A flag. Also tests that atilde, the dmd modes,
     and the dmd eigenvalues are not effected by the compute_A flag.
     """
-    bopdmd_with_A = BOPDMD(compute_A=True)
-    bopdmd_no_A = BOPDMD(compute_A=False)
+    bopdmd_with_A = BOPDMD(svd_rank=2, compute_A=True)
+    bopdmd_no_A = BOPDMD(svd_rank=2, compute_A=False)
     bopdmd_with_A.fit(Z, t)
     bopdmd_no_A.fit(Z, t)
 
     np.testing.assert_allclose(bopdmd_with_A.A, expected_A)
     with raises(ValueError):
         print(bopdmd_no_A.A)
```

### Comparing `pydmd-0.4.1.post2304/tests/test_cdmd.py` & `pydmd-0.4.1.post2305/tests/test_cdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_dmd.py` & `pydmd-0.4.1.post2305/tests/test_dmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_dmd_modes_tuner.py` & `pydmd-0.4.1.post2305/tests/test_dmd_modes_tuner.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_dmdbase.py` & `pydmd-0.4.1.post2305/tests/test_dmdbase.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_dmdc.py` & `pydmd-0.4.1.post2305/tests/test_dmdc.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_dmdoperator.py` & `pydmd-0.4.1.post2305/tests/test_dmdoperator.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_fbdmd.py` & `pydmd-0.4.1.post2305/tests/test_fbdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_hankeldmd.py` & `pydmd-0.4.1.post2305/tests/test_hankeldmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_havok.py` & `pydmd-0.4.1.post2305/tests/test_havok.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_hodmd.py` & `pydmd-0.4.1.post2305/tests/test_hodmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_mrdmd.py` & `pydmd-0.4.1.post2305/tests/test_mrdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_optdmd.py` & `pydmd-0.4.1.post2305/tests/test_optdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_paramdmd.py` & `pydmd-0.4.1.post2305/tests/test_paramdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_pidmd.py` & `pydmd-0.4.1.post2305/tests/test_pidmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_plotter.py` & `pydmd-0.4.1.post2305/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_rdmd.py` & `pydmd-0.4.1.post2305/tests/test_rdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_snapshots.py` & `pydmd-0.4.1.post2305/tests/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_spdmd.py` & `pydmd-0.4.1.post2305/tests/test_spdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2304/tests/test_subspacedmd.py` & `pydmd-0.4.1.post2305/tests/test_subspacedmd.py`

 * *Files identical despite different names*

