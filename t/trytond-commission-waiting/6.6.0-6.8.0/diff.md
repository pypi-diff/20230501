# Comparing `tmp/trytond_commission_waiting-6.6.0.tar.gz` & `tmp/trytond_commission_waiting-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_commission_waiting-6.6.0.tar", last modified: Mon Oct 31 16:14:39 2022, max compression
+gzip compressed data, was "trytond_commission_waiting-6.8.0.tar", last modified: Mon May  1 11:41:22 2023, max compression
```

## Comparing `trytond_commission_waiting-6.6.0.tar` & `trytond_commission_waiting-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:39.126603 trytond_commission_waiting-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_commission_waiting-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_commission_waiting-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-31 16:14:37.000000 trytond_commission_waiting-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_commission_waiting-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1315 2022-10-31 16:14:37.000000 trytond_commission_waiting-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:14:36.000000 trytond_commission_waiting-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:31.000000 trytond_commission_waiting-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_commission_waiting-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2612 2022-10-31 16:14:39.126603 trytond_commission_waiting-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2019-02-13 10:09:31.000000 trytond_commission_waiting-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2021-12-11 16:59:33.000000 trytond_commission_waiting-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2020-03-01 11:49:45.000000 trytond_commission_waiting-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3499 2022-04-10 15:40:35.000000 trytond_commission_waiting-6.6.0/commission.py
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2019-02-13 10:09:31.000000 trytond_commission_waiting-6.6.0/commission.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:39.123270 trytond_commission_waiting-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2019-02-13 10:09:31.000000 trytond_commission_waiting-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2224 2021-12-11 16:59:33.000000 trytond_commission_waiting-6.6.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:39.123270 trytond_commission_waiting-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-10-29 07:50:34.000000 trytond_commission_waiting-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:14:39.126603 trytond_commission_waiting-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5212 2022-10-29 07:39:10.000000 trytond_commission_waiting-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:39.123270 trytond_commission_waiting-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_commission_waiting-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4648 2020-07-09 09:37:05.000000 trytond_commission_waiting-6.6.0/tests/scenario_commission_waiting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2022-04-16 16:30:56.000000 trytond_commission_waiting-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_commission_waiting-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-10-31 15:10:09.000000 trytond_commission_waiting-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2022-10-31 16:14:35.000000 trytond_commission_waiting-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:39.126603 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2612 2022-10-31 16:14:38.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2022-10-31 16:14:39.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:14:38.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 16:14:38.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:51.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      133 2022-10-31 16:14:38.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:14:38.000000 trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:39.123270 trytond_commission_waiting-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2019-02-13 10:09:31.000000 trytond_commission_waiting-6.6.0/view/agent_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2019-02-13 10:09:31.000000 trytond_commission_waiting-6.6.0/view/commission_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:22.342242 trytond_commission_waiting-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1478 2023-05-01 11:01:01.000000 trytond_commission_waiting-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:01:01.000000 trytond_commission_waiting-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission_waiting-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2601 2023-05-01 11:41:22.342242 trytond_commission_waiting-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-01-16 14:00:20.000000 trytond_commission_waiting-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3496 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/commission.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_commission_waiting-6.8.0/commission.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:22.338908 trytond_commission_waiting-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-01-16 14:00:20.000000 trytond_commission_waiting-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2224 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:22.335575 trytond_commission_waiting-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-04-30 10:46:36.000000 trytond_commission_waiting-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-29 08:02:40.000000 trytond_commission_waiting-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:41:22.342242 trytond_commission_waiting-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4398 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:22.338908 trytond_commission_waiting-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4599 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/tests/scenario_commission_waiting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_commission_waiting-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2023-05-01 11:00:56.000000 trytond_commission_waiting-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:22.342242 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2601 2023-05-01 11:41:21.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-05-01 11:41:22.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:41:21.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:41:21.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      133 2023-05-01 11:41:21.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:41:21.000000 trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:22.338908 trytond_commission_waiting-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:20.000000 trytond_commission_waiting-6.8.0/view/agent_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:20.000000 trytond_commission_waiting-6.8.0/view/commission_form.xml
```

### Comparing `trytond_commission_waiting-6.6.0/CHANGELOG` & `trytond_commission_waiting-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
```

### Comparing `trytond_commission_waiting-6.6.0/COPYRIGHT` & `trytond_commission_waiting-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2014-2022 Cédric Krier.
-Copyright (C) 2014-2022 B2CK SPRL.
+Copyright (C) 2014-2023 Cédric Krier.
+Copyright (C) 2014-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_commission_waiting-6.6.0/LICENSE` & `trytond_commission_waiting-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-6.6.0/PKG-INFO` & `trytond_commission_waiting-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_commission_waiting
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for commission waiting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/commission_waiting
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton commission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,22 +38,22 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Commission Waiting
 ##################
 
 The commission_waiting module allows to generate account move for each
```

### Comparing `trytond_commission_waiting-6.6.0/commission.py` & `trytond_commission_waiting-6.8.0/commission.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             return
         if self.waiting_move:
             return self.waiting_move
 
         if date is None:
             with Transaction().set_context(company=self.agent.company.id):
                 date = Date.today()
-        period = Period.find(self.agent.company.id, date=date)
+        period = Period.find(self.agent.company, date=date)
 
         move = Move(journal=self.get_journal(), origin=self,
             date=date, period=period, company=self.agent.company)
         amount = Currency.compute(self.currency, self.amount,
             self.agent.company.currency)
         line = Line()
         with Transaction().set_context(date=date):
```

### Comparing `trytond_commission_waiting-6.6.0/commission.xml` & `trytond_commission_waiting-6.8.0/commission.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-6.6.0/invoice.py` & `trytond_commission_waiting-6.8.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_commission_waiting-6.6.0/setup.py` & `trytond_commission_waiting-6.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 def read(fname):
     return io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 config = ConfigParser()
 config.read_file(open(os.path.join(os.path.dirname(__file__), 'tryton.cfg')))
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_commission_waiting'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-local_version = []
-if os.environ.get('CI_JOB_ID'):
-    local_version.append(os.environ['CI_JOB_ID'])
+    download_url = ''
 else:
-    for build in ['CI_BUILD_NUMBER', 'CI_JOB_NUMBER']:
-        if os.environ.get(build):
-            local_version.append(os.environ[build])
-        else:
-            local_version = []
-            break
-if local_version:
-    version += '+' + '.'.join(local_version)
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for commission waiting',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/commission_waiting',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton commission',
     package_dir={'trytond.modules.commission_waiting': '.'},
     packages=(
         ['trytond.modules.commission_waiting']
         + ['trytond.modules.commission_waiting.%s' % p
             for p in find_packages()]
@@ -124,28 +102,27 @@
         'Natural Language :: Russian',
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         'Topic :: Office/Business :: Financial :: Accounting',
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'test': tests_require,
         },
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     commission_waiting = trytond.modules.commission_waiting
     """,
     )
```

### Comparing `trytond_commission_waiting-6.6.0/tests/scenario_commission_waiting.rst` & `trytond_commission_waiting-6.8.0/tests/scenario_commission_waiting.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 ===================
 Commission Scenario
 ===================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('commission_waiting')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/PKG-INFO` & `trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-commission-waiting
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for commission waiting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/commission_waiting
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton commission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,22 +38,22 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Commission Waiting
 ##################
 
 The commission_waiting module allows to generate account move for each
```

### Comparing `trytond_commission_waiting-6.6.0/trytond_commission_waiting.egg-info/SOURCES.txt` & `trytond_commission_waiting-6.8.0/trytond_commission_waiting.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-.drone.yml
-.flake8
-.hgtags
-.isort.cfg
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 account.py
@@ -47,14 +43,15 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_commission_waiting.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/agent_form.xml
 ./view/commission_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

