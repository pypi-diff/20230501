# Comparing `tmp/ligo-scald-0.8.1.tar.gz` & `tmp/ligo-scald-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-scald-0.8.1.tar", last modified: Fri Jul 22 14:43:13 2022, max compression
+gzip compressed data, was "ligo-scald-0.8.4.tar", last modified: Mon May  1 21:16:42 2023, max compression
```

## Comparing `ligo-scald-0.8.1.tar` & `ligo-scald-0.8.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.823510 ligo-scald-0.8.1/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    18048 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/LICENSE
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/MANIFEST.in
--rw-r--r--   0 patrick   (1000) patrick   (1000)      991 2022-07-22 14:43:13.823510 ligo-scald-0.8.1/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5111 2022-07-22 14:42:31.000000 ligo-scald-0.8.1/README.md
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.821510 ligo-scald-0.8.1/debian/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      764 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/debian/README.Debian
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5925 2022-07-22 14:42:15.000000 ligo-scald-0.8.1/debian/changelog
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        2 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/debian/compat
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      993 2022-04-04 13:13:36.000000 ligo-scald-0.8.1/debian/control
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1086 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/debian/copyright
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       32 2022-04-04 13:13:36.000000 ligo-scald-0.8.1/debian/ligo-scald.install
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       21 2022-04-04 13:13:36.000000 ligo-scald-0.8.1/debian/python3-ligo-scald.install
--rwxrwxr-x   0 patrick   (1000) patrick   (1000)      618 2022-04-04 13:13:36.000000 ligo-scald-0.8.1/debian/rules
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.821510 ligo-scald-0.8.1/debian/source/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       12 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/debian/source/format
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.820510 ligo-scald-0.8.1/ligo/
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.821510 ligo-scald-0.8.1/ligo/scald/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       88 2022-07-22 14:42:50.000000 ligo-scald-0.8.1/ligo/scald/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1405 2022-02-11 21:36:25.000000 ligo-scald-0.8.1/ligo/scald/__main__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     6585 2022-07-13 20:26:25.000000 ligo-scald-0.8.1/ligo/scald/aggregator.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3998 2022-02-17 14:36:30.000000 ligo-scald-0.8.1/ligo/scald/deploy.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.822510 ligo-scald-0.8.1/ligo/scald/io/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/ligo/scald/io/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5115 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/ligo/scald/io/core.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    49322 2022-07-13 20:27:40.000000 ligo-scald-0.8.1/ligo/scald/io/influx.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5045 2022-06-15 14:28:41.000000 ligo-scald-0.8.1/ligo/scald/io/kafka.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4370 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/ligo/scald/io/line_protocol.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8959 2022-02-17 14:36:30.000000 ligo-scald-0.8.1/ligo/scald/mock.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14803 2022-02-17 14:36:30.000000 ligo-scald-0.8.1/ligo/scald/report.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    17778 2022-02-17 14:36:30.000000 ligo-scald-0.8.1/ligo/scald/serve.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.822510 ligo-scald-0.8.1/ligo/scald/tests/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      131 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      114 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/conftest.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1743 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/test_io.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3025 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/test_mock.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2520 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/test_report.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2058 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/test_transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1761 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/ligo/scald/tests/test_utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      801 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/ligo/scald/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6737 2022-02-17 14:36:30.000000 ligo-scald-0.8.1/ligo/scald/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1865 2022-07-22 14:36:03.000000 ligo-scald-0.8.1/ligo-scald.spec
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.822510 ligo-scald-0.8.1/ligo_scald.egg-info/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      991 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/PKG-INFO
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1342 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/SOURCES.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/dependency_links.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       52 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/entry_points.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        5 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/namespace_packages.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/not-zip-safe
--rw-r--r--   0 patrick   (1000) patrick   (1000)       67 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/requires.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       22 2022-07-22 14:43:13.000000 ligo-scald-0.8.1/ligo_scald.egg-info/top_level.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       38 2022-07-22 14:43:13.823510 ligo-scald-0.8.1/setup.cfg
--rwxrwxr-x   0 patrick   (1000) patrick   (1000)     1567 2022-07-22 14:35:39.000000 ligo-scald-0.8.1/setup.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.823510 ligo-scald-0.8.1/static/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)   261069 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/static/bns-light.jpg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1150 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/static/favicon.ico
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2522 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/static/scald.css
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    34407 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/static/scald.js
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2022-07-22 14:43:13.823510 ligo-scald-0.8.1/templates/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9204 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/templates/content.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2523 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/templates/dashboard.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1471 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/templates/ifar_table.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6039 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/templates/navbar.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1558 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/templates/plots.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2340 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/templates/report.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1319 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/templates/report_navbar.html
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2620 2022-02-04 19:11:00.000000 ligo-scald-0.8.1/templates/report_scripts.js
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11857 2021-08-26 15:13:05.000000 ligo-scald-0.8.1/templates/scripts.js
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.458418 ligo-scald-0.8.4/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    18048 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/LICENSE
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/MANIFEST.in
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1018 2023-05-01 21:16:42.458418 ligo-scald-0.8.4/PKG-INFO
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5111 2023-05-01 21:08:38.000000 ligo-scald-0.8.4/README.md
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.452418 ligo-scald-0.8.4/debian/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      764 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/debian/README.Debian
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     6841 2023-05-01 21:10:48.000000 ligo-scald-0.8.4/debian/changelog
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        2 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/debian/compat
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      993 2022-04-04 13:13:36.000000 ligo-scald-0.8.4/debian/control
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1086 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/debian/copyright
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       32 2022-04-04 13:13:36.000000 ligo-scald-0.8.4/debian/ligo-scald.install
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       21 2022-04-04 13:13:36.000000 ligo-scald-0.8.4/debian/python3-ligo-scald.install
+-rwxrwxr-x   0 patrick   (1000) patrick   (1000)      618 2022-04-04 13:13:36.000000 ligo-scald-0.8.4/debian/rules
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.452418 ligo-scald-0.8.4/debian/source/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       12 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/debian/source/format
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.451418 ligo-scald-0.8.4/ligo/
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.453418 ligo-scald-0.8.4/ligo/scald/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       88 2023-05-01 21:11:00.000000 ligo-scald-0.8.4/ligo/scald/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1405 2022-02-11 21:36:25.000000 ligo-scald-0.8.4/ligo/scald/__main__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     6984 2023-02-06 16:40:43.000000 ligo-scald-0.8.4/ligo/scald/aggregator.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3998 2022-02-17 14:36:30.000000 ligo-scald-0.8.4/ligo/scald/deploy.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.454418 ligo-scald-0.8.4/ligo/scald/io/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/ligo/scald/io/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5045 2022-12-06 18:45:25.000000 ligo-scald-0.8.4/ligo/scald/io/core.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    49432 2023-05-01 20:07:41.000000 ligo-scald-0.8.4/ligo/scald/io/influx.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5441 2023-05-01 20:07:41.000000 ligo-scald-0.8.4/ligo/scald/io/kafka.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4370 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/ligo/scald/io/line_protocol.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8959 2022-02-17 14:36:30.000000 ligo-scald-0.8.4/ligo/scald/mock.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14803 2022-02-17 14:36:30.000000 ligo-scald-0.8.4/ligo/scald/report.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    17778 2022-02-17 14:36:30.000000 ligo-scald-0.8.4/ligo/scald/serve.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.454418 ligo-scald-0.8.4/ligo/scald/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      131 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/ligo/scald/tests/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      114 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/ligo/scald/tests/conftest.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1437 2022-12-06 18:45:25.000000 ligo-scald-0.8.4/ligo/scald/tests/test_io.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3025 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/ligo/scald/tests/test_mock.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2520 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/ligo/scald/tests/test_report.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2058 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/ligo/scald/tests/test_transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1761 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/ligo/scald/tests/test_utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      801 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/ligo/scald/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6737 2022-02-17 14:36:30.000000 ligo-scald-0.8.4/ligo/scald/utils.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1865 2023-05-01 21:11:45.000000 ligo-scald-0.8.4/ligo-scald.spec
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.455418 ligo-scald-0.8.4/ligo_scald.egg-info/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1018 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/PKG-INFO
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1342 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       51 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/entry_points.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)        5 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/namespace_packages.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2022-07-22 14:43:13.000000 ligo-scald-0.8.4/ligo_scald.egg-info/not-zip-safe
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       67 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/requires.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       22 2023-05-01 21:16:42.000000 ligo-scald-0.8.4/ligo_scald.egg-info/top_level.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       38 2023-05-01 21:16:42.458418 ligo-scald-0.8.4/setup.cfg
+-rwxr-xr-x   0 patrick   (1000) patrick   (1000)     1660 2023-05-01 21:11:08.000000 ligo-scald-0.8.4/setup.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.456418 ligo-scald-0.8.4/static/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)   261069 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/static/bns-light.jpg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1150 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/static/favicon.ico
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2522 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/static/scald.css
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    34407 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/static/scald.js
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-01 21:16:42.458418 ligo-scald-0.8.4/templates/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9204 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/templates/content.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2523 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/templates/dashboard.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1471 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/templates/ifar_table.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6039 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/templates/navbar.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1558 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/templates/plots.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2340 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/templates/report.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1319 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/templates/report_navbar.html
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2620 2022-02-04 19:11:00.000000 ligo-scald-0.8.4/templates/report_scripts.js
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11857 2021-08-26 15:13:05.000000 ligo-scald-0.8.4/templates/scripts.js
```

### Comparing `ligo-scald-0.8.1/LICENSE` & `ligo-scald-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/PKG-INFO` & `ligo-scald-0.8.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ligo-scald
-Version: 0.8.1
+Version: 0.8.4
 Summary: SCalable Analytics for Ligo Data
 Home-page: https://git.ligo.org/gstlal-visualisation/ligo-scald.git
 Author: Patrick Godwin
 Author-email: patrick.godwin@ligo.org
 License: GPLv2+
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-UNKNOWN
-
+file: README.md
```

### Comparing `ligo-scald-0.8.1/README.md` & `ligo-scald-0.8.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 [![pipeline status](https://git.ligo.org/gstlal-visualisation/ligo-scald/badges/master/pipeline.svg)](https://git.ligo.org/gstlal-visualisation/ligo-scald/commits/master)
 [![coverage report](https://git.ligo.org/gstlal-visualisation/ligo-scald/badges/master/coverage.svg)](https://git.ligo.org/gstlal-visualisation/ligo-scald/commits/master)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/ligo-scald.svg)](https://anaconda.org/conda-forge/ligo-scald)
 [![PyPI](https://img.shields.io/pypi/v/ligo-scald)](https://pypi.org/project/ligo-scald/)
 
 |              |        |
 | ------------ | ------ |
-| **Version:** | 0.8.1  |
+| **Version:** | 0.8.4  |
 | **Web:**     | https://docs.ligo.org/gstlal-visualisation/ligo-scald  |
-| **Source:**  | http://software.igwn.org/lscsoft/source/ligo-scald-0.8.1.tar.gz  |
+| **Source:**  | http://software.igwn.org/lscsoft/source/ligo-scald-0.8.4.tar.gz  |
 
 
 **ligo-scald** is a dynamic data visualization and monitoring tool for gravitational-wave data.
 
 ## Features:
 
 * Provides a web-based dashboard for visualizing/exploring realtime and historical data.
```

### Comparing `ligo-scald-0.8.1/debian/README.Debian` & `ligo-scald-0.8.4/debian/README.Debian`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/debian/changelog` & `ligo-scald-0.8.4/debian/changelog`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+ligo-scald (0.8.4-1) unstable; urgency=low
+
+  * fix AttributeError in Consumer.retrieve_rows_by_tag
+  * address build warnings from missing long_description
+  * remove superfluous group.id from Kafka producer setttings
+  * fix issue in disabling insecure request warnings
+  * modify python_requires version to avoid build issue
+
+ -- Patrick Godwin <patrick.godwin@ligo.org>  Mon, 01 May 2023 14:08:43 -0700
+
+ligo-scald (0.8.3-1) unstable; urgency=low
+
+  * scald aggregate: subscribe to unique set of topics
+
+ -- Patrick Godwin <patrick.godwin@ligo.org>  Mon, 06 Feb 2023 11:16:35 -0500
+
+ligo-scald (0.8.2-1) unstable; urgency=low
+
+  * Fix tag order with Kafka client when consuming messages
+  * aggregator.py: address static type checker warnings
+  * Remove custom median aggregate implementation in favor of
+    statistics.median_high
+
+ -- Patrick Godwin <patrick.godwin@ligo.org>  Mon, 28 Nov 2022 12:45:29 -0800
+
 ligo-scald (0.8.1-1) unstable; urgency=low
 
   * Fix tag order with Kafka client when consuming messages
   * Allow filtering by tag within scald aggregate
   * Fix excessive sleep in scald aggregate
   * Fix issue when consuming messages via Kafka with empty tags
   * Return HTTP warnings from InfluxDB queries
```

### Comparing `ligo-scald-0.8.1/debian/control` & `ligo-scald-0.8.4/debian/control`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/debian/copyright` & `ligo-scald-0.8.4/debian/copyright`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/debian/rules` & `ligo-scald-0.8.4/debian/rules`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/__main__.py` & `ligo-scald-0.8.4/ligo/scald/__main__.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/aggregator.py` & `ligo-scald-0.8.4/ligo/scald/aggregator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Patrick Godwin (patrick.godwin@ligo.org)"
 __description__ = "utilities to aggregate and store incoming metrics"
 
 #-------------------------------------------------
 ### imports
 
+import argparse
 from collections import defaultdict
 import logging
 import os
-import sys
 import time
 import timeit
 
 import numpy
 import yaml
 
 from .io import influx, kafka
@@ -82,15 +82,15 @@
 
 def main(args=None):
     """Aggregates and stores metrics to a data backend
 
     """
     if not args:
         parser = argparse.ArgumentParser()
-        _parser_add_arguments(parser)
+        _add_parser_args(parser)
         args = parser.parse_args()
 
     topics = args.topic
 
     # set up logging
     log_level = logging.INFO if args.verbose else logging.WARNING
     logging.basicConfig(format='%(asctime)s | %(name)s : %(levelname)s : %(message)s')
@@ -118,49 +118,61 @@
     if not config_path:
         raise KeyError('no configuration file found, please set your SCALDRC_PATH correctly or add --config param')
     with open(config_path, 'r') as f:
         config = yaml.safe_load(f)
 
     # instantiate a consumer to subscribe to all of our topics, i.e., jobs
     client = kafka.Client(args.uri)
-    client.subscribe(topics)
+    client.subscribe(set(topics))
 
     # set up aggregator
     aggregator_settings = config['backends'][args.backend]
     aggregator_settings['reduce_across_tags'] = args.across_jobs
     aggregator = influx.Aggregator(**aggregator_settings)
 
     # register measurement schemas for aggregators
     aggregator.load(path=config_path)
 
-    # start an infinite loop to keep updating and aggregating data
-    while True:
-        logger.info("retrieving data from kafka")
-        start = timeit.default_timer()
-
-        msgs = [msg for msg in client.query(tags=args.tag, max_messages=2000)]
-        if args.data_type == 'timeseries':
-            data = parse_timeseries(msgs, topics)
-        elif args.data_type == 'triggers':
-            data = parse_triggers(msgs)
-
-        retrieve_elapsed = timeit.default_timer() - start
-        logger.info("time to retrieve data: %.1f s" % retrieve_elapsed)
-
-        # store and reduce data for each job
-        start = timeit.default_timer()
-        for topic, schema in zip(topics, schemas):
-            logger.info("storing and reducing metrics for schema: %s" % schema)
+    # update and aggregate data continuously
+    try:
+        while True:
+            logger.info("retrieving data from kafka")
+            start = timeit.default_timer()
+
+            msgs = [msg for msg in client.query(tags=args.tag, max_messages=2000)]
             if args.data_type == 'timeseries':
-                aggregator.store_columns(schema, data[topic], aggregate=config['schemas'][schema]['aggregate'])
+                data = parse_timeseries(msgs, topics)
             elif args.data_type == 'triggers':
-                far_key = config['schemas'][schema]['far_key']
-                time_key = config['schemas'][schema]['time_key']
-                aggregator.store_triggers(schema, [trg for trg in data if far_key in trg], far_key = far_key, time_key = time_key)
-
-        store_elapsed = timeit.default_timer() - start
-        logger.info("time to store/reduce %s: %.1f s" % (args.data_type, store_elapsed))
-
-        time.sleep(max(args.processing_cadence - store_elapsed - retrieve_elapsed, 0))
-
-    # close client connection
-    client.close()
+                data = parse_triggers(msgs)
+            else:
+                raise ValueError("--data-type not a valid option")
+
+            retrieve_elapsed = timeit.default_timer() - start
+            logger.info("time to retrieve data: %.1f s" % retrieve_elapsed)
+
+            # store and reduce data for each job
+            start = timeit.default_timer()
+            for topic, schema in zip(topics, schemas):
+                logger.info("storing and reducing metrics for schema: %s" % schema)
+                if args.data_type == 'timeseries':
+                    aggregator.store_columns(
+                        schema,
+                        data[topic],
+                        aggregate=config['schemas'][schema]['aggregate']
+                    )
+                elif args.data_type == 'triggers':
+                    far_key = config['schemas'][schema]['far_key']
+                    time_key = config['schemas'][schema]['time_key']
+                    aggregator.store_triggers(
+                        schema,
+                        [trg for trg in data if far_key in trg],
+                        far_key=far_key,
+                        time_key = time_key
+                    )
+
+            store_elapsed = timeit.default_timer() - start
+            logger.info("time to store/reduce %s: %.1f s" % (args.data_type, store_elapsed))
+
+            time.sleep(max(args.processing_cadence - store_elapsed - retrieve_elapsed, 0))
+    finally:
+        # close client connection
+        client.close()
```

### Comparing `ligo-scald-0.8.1/ligo/scald/deploy.py` & `ligo-scald-0.8.4/ligo/scald/deploy.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/io/core.py` & `ligo-scald-0.8.4/ligo/scald/io/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,48 +19,44 @@
 
 #-------------------------------------------------
 ### imports
 
 import collections
 import json
 import os
+import statistics
 
 import numpy
 
 
 #-------------------------------------------------
 ### constants
 
 MIN_TIME_QUANTA = 10000
 DIRS = 6
 
 
 #-------------------------------------------------
 ### common utilities
 
-def median(l):
-    """!
-    Return the median of a list on nearest value
-    """
-    return sorted(l)[len(l)//2]
+_aggregate_func_map = {
+    "median": statistics.median_high,
+    "min": min,
+    "max": max,
+}
 
 
 def aggregate_to_func(aggregate):
     """!
     Given an aggregate string, returns back a function that does that
     aggregation.
     """
-    if aggregate == 'median':
-        return median
-    elif aggregate == 'min':
-        return min
-    elif aggregate == 'max':
-        return max
-    else:
+    if aggregate not in _aggregate_func_map:
         raise NotImplementedError
+    return _aggregate_func_map[aggregate]
 
 
 def reduce_data(xarr, yarr, func, dt = 1):
     """!
     This function does a data reduction by powers of 10 where dt
     specifies the spacing.  Default is 1 e.g., data reduction over 1 second
     """
```

### Comparing `ligo-scald-0.8.1/ligo/scald/io/influx.py` & `ligo-scald-0.8.4/ligo/scald/io/influx.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging
 import os
 import netrc
 import urllib.parse
 
 import numpy
 import urllib3
+import urllib3.exceptions
 import yaml
 
 from . import core
 from . import line_protocol
 from .. import utils
 
 #-------------------------------------------------
@@ -28,15 +29,15 @@
 
 ### set up certificate verification
 try:
     import certifi
     import urllib3.contrib.pyopenssl
     urllib3.contrib.pyopenssl.inject_into_urllib3()
 except ImportError:
-    urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+    pass
 
 #-------------------------------------------------
 ### templates
 
 INFLUX_QUERY_TEMPLATE = 'SELECT {columns} FROM {measurement} {conditions}'
 INFLUX_MEASUREMENT_TEMPLATE = '"{db}".{retention_policy}."{measurement}"'
 
@@ -702,15 +703,15 @@
         data: `list` of `list`
             a list of timeseries, each one corresponding to a tag value ordered
             by tag_values
 
         NOTE: this method needs a schema to be registered for a particular measurement before use.
 
         """
-        return _retrieve_rows_by_tag(self.client, self.database, measurement, self.schema[measurement], start, end, tag, aggregate=aggregate, dt=dt, datetime=datetime)
+        return _retrieve_rows_by_tag(self.client, self.db, measurement, self.schema[measurement], start, end, tag, aggregate=aggregate, dt=dt, datetime=datetime)
 
 
     def retrieve_binnedtimeseries_by_tag(self, measurement, start, end, column, tag_key, tags=None, aggregate=None, dt=None, datetime=False):
         """Retrieve all timeseries with a given tag, binned by tag and dt.
 
         Parameters
         ----------
@@ -1170,14 +1171,16 @@
         else:
             ca_certs = certifi.where()
         return urllib3.HTTPSConnectionPool(
             host, port=port, maxsize=10, block=True, headers=headers,
             cert_reqs='CERT_REQUIRED', ca_certs=ca_certs
         )
     elif https:
+        # disable insecure request warnings when disabling cert verification
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         return urllib3.HTTPSConnectionPool(host, port=port, maxsize=10, block=True, headers=headers, cert_reqs='CERT_NONE')
     else:
         return urllib3.HTTPConnectionPool(host, port=port, maxsize=10, block=True, headers=headers)
 
 
 #-------------------------------------------------
 ### internal utilities
```

### Comparing `ligo-scald-0.8.1/ligo/scald/io/kafka.py` & `ligo-scald-0.8.4/ligo/scald/io/kafka.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 
 from collections import defaultdict, namedtuple
 import getpass
 import json
 import random
 import string
 import sys
+import logging
 from urllib.parse import urlparse
 
 from confluent_kafka import Consumer, Producer
 
+#-------------------------------------------------
+### logging
+
+logger = logging.getLogger('scald')
+
 
 #-------------------------------------------------
 ### classes
 
 Message = namedtuple("Message", "topic partition offset key value timestamp")
 
 class Client(object):
@@ -30,28 +36,28 @@
         kafka://[groupid@]hostname[:port][/topic1,topic2,...]
 
     """
     def __init__(self, uri):
         self.uri = uriparse(uri)
 
         ### kafka settings
-        self._kafka_settings = {
+        self._consumer_settings = {
             'bootstrap.servers': self.uri.broker,
             'group.id': self.uri.groupid,
         }
         self._producer_settings = {
+            'bootstrap.servers': self.uri.broker,
             'message.max.bytes': 5242880,  # 5 MB
-            **self._kafka_settings,
         }
 
         ### set up producer
         self._producer = Producer(self._producer_settings)
 
         ### set up consumer
-        self._consumer = Consumer(self._kafka_settings)
+        self._consumer = Consumer(self._consumer_settings)
         if self.uri.topics:
             self._consumer.subscribe([topic for topic in self.uri.topics])
         self.topics = self.uri.topics
 
     def subscribe(self, topic):
         """Subscribe to Kafka topics.
 
@@ -117,17 +123,25 @@
         """
         payload = json.dumps(data).encode("utf-8")
         if tags:
             if isinstance(tags, list):
                 tags = ".".join(tags).encode("utf-8")
             self._producer.produce(topic=topic, key=tags, value=payload)
         else:
-            self._producer.produce(topic=topic, value=payload)
+            self._producer.produce(topic=topic, value=payload, on_delivery=self._delivery_report)
         self._producer.poll(0)
 
+    @staticmethod
+    def _delivery_report(error, msg):
+        """
+        Handle response of each message produced.
+        """
+        if error is not None:
+            logger.warning(f"Message delivery failed: {error}")
+
     def close(self):
         """Close the connection to the client.
 
         """
         self._producer.flush()
         self._consumer.unsubscribe()
         self._consumer.close()
```

### Comparing `ligo-scald-0.8.1/ligo/scald/io/line_protocol.py` & `ligo-scald-0.8.4/ligo/scald/io/line_protocol.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/mock.py` & `ligo-scald-0.8.4/ligo/scald/mock.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/report.py` & `ligo-scald-0.8.4/ligo/scald/report.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/serve.py` & `ligo-scald-0.8.4/ligo/scald/serve.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/tests/test_io.py` & `ligo-scald-0.8.4/ligo/scald/tests/test_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,46 +2,37 @@
 
 __author__ = "Patrick Godwin (patrick.godwin@ligo.org)"
 __description__ = "a module that tests core I/O utilities"
 
 #-------------------------------------------------
 ### imports
 
-import sys
+import statistics
+
 import pytest
 
 import numpy
 
 from ligo.scald.io import core
 
 
 #-------------------------------------------------
 ### tests
 
 class TestIOCore(object):
     """
     Tests several aspects of mock.py to check basic functionality.
     """
-    def test_median(self):
-        arr1 = numpy.arange(0, 100)
-        median1 = core.median(arr1)
-        assert median1 == 50, 'expected median: {}, got: {}'.format(50, median1)
-
-        arr2 = numpy.arange(0, 101)
-        median1 = core.median(arr2)
-        assert median1 == 50, 'expected median: {}, got: {}'.format(50, median1)
-
-
-    @pytest.mark.parametrize("agg, func", [('min', min), ('median', core.median), ('max', max)])
+    @pytest.mark.parametrize("agg, func", [('min', min), ('median', statistics.median_high), ('max', max)])
     def test_aggregate_to_func(self, agg, func):
         expected = core.aggregate_to_func(agg)
         assert expected == func
 
 
-    @pytest.mark.parametrize("func, idx", [(min, 0), (core.median, 5), (max, 9)])
+    @pytest.mark.parametrize("func, idx", [(min, 0), (statistics.median_high, 5), (max, 9)])
     def test_reduce_data(self, func, idx):
         xarr = numpy.arange(10)
         yarr = numpy.arange(10)
         reduced_idx, reduced_x, reduced_y = core.reduce_data(xarr, yarr, func, dt=10)
         reduced_idx = reduced_idx[0] # checking only single idx
         assert len(reduced_x) == 1, 'expected x length: {}, got: {}'.format(1, len(reduced_x))
         assert len(reduced_y) == 1, 'expected y length: {}, got: {}'.format(1, len(reduced_y))
```

### Comparing `ligo-scald-0.8.1/ligo/scald/tests/test_mock.py` & `ligo-scald-0.8.4/ligo/scald/tests/test_mock.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/tests/test_report.py` & `ligo-scald-0.8.4/ligo/scald/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/tests/test_transforms.py` & `ligo-scald-0.8.4/ligo/scald/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/tests/test_utils.py` & `ligo-scald-0.8.4/ligo/scald/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/transforms.py` & `ligo-scald-0.8.4/ligo/scald/transforms.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo/scald/utils.py` & `ligo-scald-0.8.4/ligo/scald/utils.py`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/ligo-scald.spec` & `ligo-scald-0.8.4/ligo-scald.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 %define name              ligo-scald
-%define version           0.8.1
-%define unmangled_version 0.8.1
+%define version           0.8.4
+%define unmangled_version 0.8.4
 %define release           1
 
 Summary:   SCalable Analytics for Ligo/virgo/kagra Data
 Name:      %{name}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Source0:   http://software.igwn.org/lscsoft/source/%{name}-%{unmangled_version}.tar.gz
```

### Comparing `ligo-scald-0.8.1/ligo_scald.egg-info/PKG-INFO` & `ligo-scald-0.8.4/ligo_scald.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ligo-scald
-Version: 0.8.1
+Version: 0.8.4
 Summary: SCalable Analytics for Ligo Data
 Home-page: https://git.ligo.org/gstlal-visualisation/ligo-scald.git
 Author: Patrick Godwin
 Author-email: patrick.godwin@ligo.org
 License: GPLv2+
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-UNKNOWN
-
+file: README.md
```

### Comparing `ligo-scald-0.8.1/ligo_scald.egg-info/SOURCES.txt` & `ligo-scald-0.8.4/ligo_scald.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/setup.py` & `ligo-scald-0.8.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     'urllib3 >= 1.10',
     'python-dateutil',
 ]
 
 setup(
     name = 'ligo-scald',
     description = 'SCalable Analytics for Ligo Data',
-    version = '0.8.1',
+    long_description = "file: README.md",
+    long_description_content_type = "text/markdown",
+    version = '0.8.4',
     author = 'Patrick Godwin',
     author_email = 'patrick.godwin@ligo.org',
     url = 'https://git.ligo.org/gstlal-visualisation/ligo-scald.git',
     license = 'GPLv2+',
 
     packages = ['ligo', 'ligo.scald', 'ligo.scald.io', 'ligo.scald.tests', 'static', 'templates'],
     namespace_packages = ['ligo'],
@@ -27,15 +29,15 @@
 
     entry_points = {
         'console_scripts': [
             'scald = ligo.scald.__main__:main',
         ],
     },
 
-    python_requires = '>=3.6.*',
+    python_requires = '>=3.6',
     install_requires = install_requires,
     zip_safe = False,
 
     classifiers = [
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

### Comparing `ligo-scald-0.8.1/static/bns-light.jpg` & `ligo-scald-0.8.4/static/bns-light.jpg`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/static/favicon.ico` & `ligo-scald-0.8.4/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/static/scald.css` & `ligo-scald-0.8.4/static/scald.css`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/static/scald.js` & `ligo-scald-0.8.4/static/scald.js`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/content.html` & `ligo-scald-0.8.4/templates/content.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/dashboard.html` & `ligo-scald-0.8.4/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/ifar_table.html` & `ligo-scald-0.8.4/templates/ifar_table.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/navbar.html` & `ligo-scald-0.8.4/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/plots.html` & `ligo-scald-0.8.4/templates/plots.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/report.html` & `ligo-scald-0.8.4/templates/report.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/report_navbar.html` & `ligo-scald-0.8.4/templates/report_navbar.html`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/report_scripts.js` & `ligo-scald-0.8.4/templates/report_scripts.js`

 * *Files identical despite different names*

### Comparing `ligo-scald-0.8.1/templates/scripts.js` & `ligo-scald-0.8.4/templates/scripts.js`

 * *Files identical despite different names*

