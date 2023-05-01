# Comparing `tmp/pycep_correios-5.1.0.tar.gz` & `tmp/pycep-correios-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycep_correios-5.1.0.tar", last modified: Wed Oct 12 13:44:19 2022, max compression
+gzip compressed data, was "pycep-correios-5.2.0.tar", last modified: Mon May  1 14:22:22 2023, max compression
```

## Comparing `pycep_correios-5.1.0.tar` & `pycep-correios-5.2.0.tar`

### file list

```diff
@@ -1,30 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios/
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/pycep_correios/viacep.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/pycep_correios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/pycep_correios/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/pycep_correios/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/pycep_correios/correios.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/pycep_correios/apicep.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4488 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/tests/test_viacep.py
--rw-r--r--   0 runner    (1001) docker     (121)     2861 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/tests/test_correios.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/tests/test_apicep.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2483 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-12 13:44:19.000000 pycep_correios-5.1.0/pycep_correios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5476 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-12 13:44:04.000000 pycep_correios-5.1.0/requirements.txt
+drwxrwxr-x   0 michell   (1000) michell   (1000)        0 2023-05-01 14:22:22.422404 pycep-correios-5.2.0/
+-rw-rw-r--   0 michell   (1000) michell   (1000)      340 2023-05-01 14:22:22.422404 pycep-correios-5.2.0/PKG-INFO
+-rw-rw-r--   0 michell   (1000) michell   (1000)      153 2023-05-01 14:21:29.000000 pycep-correios-5.2.0/README.md
+drwxrwxr-x   0 michell   (1000) michell   (1000)        0 2023-05-01 14:22:22.422404 pycep-correios-5.2.0/pycep_correios.egg-info/
+-rw-rw-r--   0 michell   (1000) michell   (1000)      340 2023-05-01 14:22:22.000000 pycep-correios-5.2.0/pycep_correios.egg-info/PKG-INFO
+-rw-rw-r--   0 michell   (1000) michell   (1000)      207 2023-05-01 14:22:22.000000 pycep-correios-5.2.0/pycep_correios.egg-info/SOURCES.txt
+-rw-rw-r--   0 michell   (1000) michell   (1000)        1 2023-05-01 14:22:22.000000 pycep-correios-5.2.0/pycep_correios.egg-info/dependency_links.txt
+-rw-rw-r--   0 michell   (1000) michell   (1000)       10 2023-05-01 14:22:22.000000 pycep-correios-5.2.0/pycep_correios.egg-info/requires.txt
+-rw-rw-r--   0 michell   (1000) michell   (1000)        1 2023-05-01 14:22:22.000000 pycep-correios-5.2.0/pycep_correios.egg-info/top_level.txt
+-rw-rw-r--   0 michell   (1000) michell   (1000)       38 2023-05-01 14:22:22.422404 pycep-correios-5.2.0/setup.cfg
+-rw-rw-r--   0 michell   (1000) michell   (1000)      543 2023-05-01 14:21:29.000000 pycep-correios-5.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

