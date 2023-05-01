# Comparing `tmp/trytond_purchase_invoice_line_standalone-6.6.0.tar.gz` & `tmp/trytond_purchase_invoice_line_standalone-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_invoice_line_standalone-6.6.0.tar", last modified: Mon Oct 31 16:10:00 2022, max compression
+gzip compressed data, was "trytond_purchase_invoice_line_standalone-6.8.0.tar", last modified: Mon May  1 12:00:20 2023, max compression
```

## Comparing `trytond_purchase_invoice_line_standalone-6.6.0.tar` & `trytond_purchase_invoice_line_standalone-6.8.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_purchase_invoice_line_standalone-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_purchase_invoice_line_standalone-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-31 16:09:59.000000 trytond_purchase_invoice_line_standalone-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_purchase_invoice_line_standalone-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2213 2022-10-31 16:09:58.000000 trytond_purchase_invoice_line_standalone-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 16:09:58.000000 trytond_purchase_invoice_line_standalone-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:56.000000 trytond_purchase_invoice_line_standalone-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_purchase_invoice_line_standalone-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2463 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2019-06-04 16:49:45.000000 trytond_purchase_invoice_line_standalone-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      501 2021-12-11 16:59:33.000000 trytond_purchase_invoice_line_standalone-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2019-06-04 16:49:45.000000 trytond_purchase_invoice_line_standalone-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      900 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      753 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      778 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      764 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      783 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      785 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      781 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      801 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_purchase_invoice_line_standalone-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3465 2022-10-11 19:49:58.000000 trytond_purchase_invoice_line_standalone-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1311 2020-04-26 13:06:29.000000 trytond_purchase_invoice_line_standalone-6.6.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5337 2022-10-29 07:39:11.000000 trytond_purchase_invoice_line_standalone-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_purchase_invoice_line_standalone-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5034 2020-07-09 09:37:15.000000 trytond_purchase_invoice_line_standalone-6.6.0/tests/scenario_purchase_invoice_line_standalone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-04-16 16:30:57.000000 trytond_purchase_invoice_line_standalone-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_purchase_invoice_line_standalone-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2022-10-31 15:10:09.000000 trytond_purchase_invoice_line_standalone-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2022-10-31 16:09:57.000000 trytond_purchase_invoice_line_standalone-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2463 2022-10-31 16:09:59.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1676 2022-10-31 16:10:00.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:09:59.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2022-10-31 16:09:59.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:10.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2022-10-31 16:09:59.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:09:59.000000 trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:00.439218 trytond_purchase_invoice_line_standalone-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2019-10-11 23:09:48.000000 trytond_purchase_invoice_line_standalone-6.6.0/view/invoice_line_tree_invoice_type.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:20.656368 trytond_purchase_invoice_line_standalone-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3152 2023-05-01 11:13:49.000000 trytond_purchase_invoice_line_standalone-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:13:48.000000 trytond_purchase_invoice_line_standalone-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_invoice_line_standalone-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2483 2023-05-01 12:00:20.656368 trytond_purchase_invoice_line_standalone-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:20.653034 trytond_purchase_invoice_line_standalone-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3152 2023-05-01 11:13:49.000000 trytond_purchase_invoice_line_standalone-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:20.646368 trytond_purchase_invoice_line_standalone-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1707 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1484 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1741 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1507 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1273 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1422 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1466 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1660 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1486 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1537 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1542 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1546 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-30 10:46:36.000000 trytond_purchase_invoice_line_standalone-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1247 2023-04-28 07:46:16.000000 trytond_purchase_invoice_line_standalone-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3563 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1311 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:00:20.656368 trytond_purchase_invoice_line_standalone-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4607 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:20.649701 trytond_purchase_invoice_line_standalone-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2571 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/tests/scenario_purchase_invoice_line_not_standalone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4972 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/tests/scenario_purchase_invoice_line_standalone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      134 2023-05-01 11:13:43.000000 trytond_purchase_invoice_line_standalone-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:20.656368 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2483 2023-05-01 12:00:19.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-05-01 12:00:20.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:00:19.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-05-01 12:00:19.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-05-01 12:00:19.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:00:19.000000 trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:20.649701 trytond_purchase_invoice_line_standalone-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/view/invoice_line_tree_invoice_type.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_purchase_invoice_line_standalone-6.8.0/view/party_form.xml
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/COPYRIGHT` & `trytond_purchase_invoice_line_standalone-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/LICENSE` & `trytond_purchase_invoice_line_standalone-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/PKG-INFO` & `trytond_purchase_invoice_line_standalone-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_invoice_line_standalone
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for standalone invoice line from purchase
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_invoice_line_standalone
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase standalone invoice line
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
@@ -38,22 +38,24 @@
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
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
+#######################################
 Purchase Invoice Line Standalone Module
 #######################################
 
-The purchase invoice line standalone module makes purchase to generate invoice
-lines instead of invoices.
+The *Purchase Invoice Line Standalone Module* allows purchases to generate
+invoice lines instead of invoices.
+
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/bg.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/es.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr "Linea de factura de compra por separado"
+
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr "Lineas de factura de compra por separado"
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr "Tercero"
+
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr "Líneas de factura por separado"
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Редове от фактура"
+msgstr "Líneas de factura"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
-msgstr "Игнорирани редове от фактура"
+msgstr "Líneas de factura ignoradas"
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
-msgstr "Ред от фактура"
+msgstr "Línea de factura"
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "Покупки"
+msgstr "Compra"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
-msgstr "Редове от фактура"
+msgstr "Líneas de factura"
+
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr "Lineas de factura de compra por separado"
 
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
-msgstr "Покупка - Игнорирани редове от фактура"
+msgstr "Compra - Línea de factura ignorada"
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/ca.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/cs.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr ""
+
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr ""
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr ""
+
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr ""
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Línies de factura"
+msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
-msgstr "Línies de factura ignorades"
+msgstr ""
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
-msgstr "Línia de factura"
+msgstr ""
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "Compra"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
-msgstr "Línies de factura"
+msgstr ""
+
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr ""
 
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
-msgstr "Compra - Línia de factura ignorada"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/es.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/fr.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr "Ligne de facture d'achat autonome"
+
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr "Lignes de facture d'achat autonome"
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr "Tiers"
+
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr "Ligne de facture autonome"
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Líneas de factura"
+msgstr "Lignes de facture"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
-msgstr "Líneas de factura ignoradas"
+msgstr "Lignes de facture ignorées"
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
-msgstr "Línea de factura"
+msgstr "Ligne de facture"
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "Compra"
+msgstr "Achat"
 
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
-msgstr "Líneas de factura"
+msgstr "Lignes de facture"
+
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr "Ligne de facture d'achat autonome de tiers"
 
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
-msgstr "Compra - Línea de factura ignorada"
+msgstr "Achat - Ligne de facture ignorée"
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/hu.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/es_419.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr ""
+
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr ""
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr ""
+
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr ""
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
 msgstr ""
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "Vásárlás"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
 msgstr ""
 
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr ""
+
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/it.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/hu.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr ""
+
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr ""
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr ""
+
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr ""
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Righe fattura"
+msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
-msgstr "Righe fattura non considerate"
+msgstr ""
 
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
-msgstr "Riga fattura"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "Acquisto"
+msgstr "Vásárlás"
 
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
-msgstr "Righe fattura"
+msgstr ""
+
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr ""
 
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
-msgstr "Acquisto - riga fattura non considerata"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/lo.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/et.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr "Ost - ignoreeritud arve read"
+
+#, fuzzy
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr "Ost - ignoreeritud arve read"
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr ""
+
+#, fuzzy
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr "Ignoreeritud arve read"
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "ລາຍການເກັບເງິນ"
+msgstr "Arve read"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
-msgstr ""
+msgstr "Ignoreeritud arve read"
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
-msgstr "ລາຍການ"
+msgstr "Arve read"
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "ສັ່ງຊື້"
+msgstr "Ost"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
-msgstr "ລາຍການເກັບເງິນ"
+msgstr "Arve read"
+
+#, fuzzy
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr "Ost - ignoreeritud arve read"
 
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
-msgstr ""
+msgstr "Ost - ignoreeritud arve read"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/lt.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/lt.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr "Pirkimai - Sąskaitos faktūros ignoruota eilutė"
+
+#, fuzzy
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr "Pirkimai - Sąskaitos faktūros ignoruota eilutė"
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr ""
+
+#, fuzzy
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr "Sąskaitos faktūros ignoruotos eilutės"
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Sąskaitos faktūros eilutės"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
 msgstr "Sąskaitos faktūros ignoruotos eilutės"
@@ -19,10 +39,15 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
 msgstr "Sąskaitos faktūros eilutės"
 
+#, fuzzy
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr "Pirkimai - Sąskaitos faktūros ignoruota eilutė"
+
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
 msgstr "Pirkimai - Sąskaitos faktūros ignoruota eilutė"
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/nl.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/nl.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr "Losstaande Inkoop Factuur Regel"
+
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr "Losstaande Inkoop Factuur Regels"
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr "Relatie"
+
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr "Losstaande Factuur Regel"
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuurregels"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
 msgstr "Factuurregels genegeerd"
@@ -18,10 +35,14 @@
 msgid "Purchase"
 msgstr "Inkoop"
 
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
 msgstr "Factuurregels"
 
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr "Relatie Losstaande Inkoop Factuur regel"
+
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
 msgstr "Aankoop - Genegeerde factuurregel"
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/locale/ru.po` & `trytond_purchase_invoice_line_standalone-6.8.0/locale/pl.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
+msgctxt "field:party.party,purchase_invoice_line_standalone:"
+msgid "Purchase Invoice Line Standalone"
+msgstr "Zakup - Zignorowany wiersz faktury"
+
+#, fuzzy
+msgctxt "field:party.party,purchase_invoice_lines_standalone:"
+msgid "Purchase Invoice Lines Standalone"
+msgstr "Zakup - Zignorowany wiersz faktury"
+
+msgctxt "field:party.party.purchase_invoice_line_standalone,party:"
+msgid "Party"
+msgstr ""
+
+#, fuzzy
+msgctxt ""
+"field:party.party.purchase_invoice_line_standalone,purchase_invoice_line_standalone:"
+msgid "Invoice Line Standalone"
+msgstr "Wiersze faktury zignorowane"
+
 msgctxt "field:purchase.purchase,invoice_lines:"
 msgid "Invoice Lines"
-msgstr "Строки инвойса"
+msgstr "Wiersze faktury"
 
 msgctxt "field:purchase.purchase,invoice_lines_ignored:"
 msgid "Invoice Lines Ignored"
-msgstr ""
+msgstr "Wiersze faktury zignorowane"
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,invoice:"
 msgid "Invoice Line"
-msgstr "Строка инвойса"
+msgstr "Wiersz faktury"
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice.line,purchase:"
 msgid "Purchase"
-msgstr "Покупки"
+msgstr "Zakup"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_invoice_line_relate"
 msgid "Invoice Lines"
-msgstr "Строки инвойса"
+msgstr "Wiersze faktury"
+
+#, fuzzy
+msgctxt "model:party.party.purchase_invoice_line_standalone,name:"
+msgid "Party Purchase Invoice Line Standalone"
+msgstr "Zakup - Zignorowany wiersz faktury"
 
 msgctxt "model:purchase.purchase-ignored-account.invoice.line,name:"
 msgid "Purchase - Ignored Invoice Line"
-msgstr ""
+msgstr "Zakup - Zignorowany wiersz faktury"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/purchase.py` & `trytond_purchase_invoice_line_standalone-6.8.0/purchase.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,51 +9,56 @@
     invoice_lines = fields.Function(fields.Many2Many(
             'account.invoice.line', None, None, "Invoice Lines"),
         'get_invoice_lines', searcher='search_invoice_lines')
     invoice_lines_ignored = fields.Many2Many(
             'purchase.purchase-ignored-account.invoice.line',
             'purchase', 'invoice', 'Invoice Lines Ignored', readonly=True)
 
+    @property
+    def invoice_line_standalone(self):
+        party = self.invoice_party or self.party
+        return party.purchase_invoice_line_standalone
+
     def get_invoice_lines(self, name):
         return list({il.id for l in self.lines for il in l.invoice_lines})
 
     @classmethod
     def search_invoice_lines(cls, name, clause):
         return [('lines.' + clause[0],) + tuple(clause[1:])]
 
     @classmethod
     def _save_invoice(cls, invoices):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
 
         lines = []
-        for invoice in invoices.values():
-            for line in invoice.lines:
-                if line.type == 'line':
-                    line.invoice = None
-                    line.party = invoice.party
-                    lines.append(line)
+        non_standalone = {}
+        for purchase, invoice in invoices.items():
+            if purchase.invoice_line_standalone:
+                for line in invoice.lines:
+                    if line.type == 'line':
+                        line.invoice = None
+                        line.party = invoice.party
+                        lines.append(line)
+            else:
+                non_standalone[purchase] = invoice
         InvoiceLine.save(lines)
 
-        super()._save_invoice({})
+        super()._save_invoice(non_standalone)
 
     def get_invoice_state(self):
         state = super(Purchase, self).get_invoice_state()
-        skips = set(x.id for x in self.invoice_lines_ignored)
-        invoice_lines = [l for l in self.invoice_lines if l.id not in skips]
-        if invoice_lines:
-            if any(l.invoice and l.invoice.state == 'cancelled'
-                    for l in invoice_lines):
-                return 'exception'
-            elif (state == 'paid'
-                    and all(l.invoice for l in invoice_lines)
-                    and all(l.invoice.state == 'paid' for l in invoice_lines)):
-                return 'paid'
-            else:
-                return 'waiting'
+        skips = set(self.invoice_lines_ignored)
+        standalone_lines = [
+            l for l in self.invoice_lines if l not in skips and not l.invoice]
+        if standalone_lines:
+            state = {
+                'paid': 'partially paid',
+                'none': 'pending',
+                }.get(state, state)
         return state
 
     @classmethod
     def copy(cls, purchases, default=None):
         if default is None:
             default = {}
         else:
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/purchase.xml` & `trytond_purchase_invoice_line_standalone-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/setup.py` & `trytond_purchase_invoice_line_standalone-6.8.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
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
@@ -34,61 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_invoice_line_standalone'
 
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
 
 requires = ['python-sql']
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
     description='Tryton module for standalone invoice line from purchase',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/purchase_invoice_line_standalone'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase standalone invoice line',
     package_dir={'trytond.modules.purchase_invoice_line_standalone': '.'},
     packages=(
         ['trytond.modules.purchase_invoice_line_standalone']
         + ['trytond.modules.purchase_invoice_line_standalone.%s' % p
             for p in find_packages()]
@@ -126,28 +106,27 @@
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
     purchase_invoice_line_standalone = \
         trytond.modules.purchase_invoice_line_standalone
     """,
     )
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/tests/scenario_purchase_invoice_line_standalone.rst` & `trytond_purchase_invoice_line_standalone-6.8.0/tests/scenario_purchase_invoice_line_standalone.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 =========================================
 Purchase Invoice Line Standalone Scenario
 =========================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> current_config = activate_modules('purchase_invoice_line_standalone')
 
 Create company::
 
@@ -52,14 +49,15 @@
     >>> revenue = accounts['revenue']
     >>> expense = accounts['expense']
 
 Create parties::
 
     >>> Party = Model.get('party.party')
     >>> supplier = Party(name='Supplier')
+    >>> supplier.purchase_invoice_line_standalone = True
     >>> supplier.save()
     >>> customer = Party(name='Customer')
     >>> customer.save()
 
 Create account category::
 
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO` & `trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-purchase-invoice-line-standalone
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for standalone invoice line from purchase
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_invoice_line_standalone
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase standalone invoice line
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
@@ -38,22 +38,24 @@
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
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
+#######################################
 Purchase Invoice Line Standalone Module
 #######################################
 
-The purchase invoice line standalone module makes purchase to generate invoice
-lines instead of invoices.
+The *Purchase Invoice Line Standalone Module* allows purchases to generate
+invoice lines instead of invoices.
+
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt` & `trytond_purchase_invoice_line_standalone-6.8.0/trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
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
+party.py
+party.xml
 purchase.py
 purchase.xml
 setup.py
 tox.ini
 tryton.cfg
 ./__init__.py
+./party.py
+./party.xml
 ./purchase.py
 ./purchase.xml
 ./tryton.cfg
 ./locale/bg.po
 ./locale/ca.po
 ./locale/cs.po
 ./locale/de.po
@@ -38,19 +38,24 @@
 ./locale/ro.po
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
+./tests/scenario_purchase_invoice_line_not_standalone.rst
 ./tests/scenario_purchase_invoice_line_standalone.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/invoice_line_tree_invoice_type.xml
+./view/party_form.xml
+doc/conf.py
 doc/index.rst
+doc/releases.rst
+doc/usage.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
 locale/et.po
@@ -68,18 +73,20 @@
 locale/ro.po
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
+tests/scenario_purchase_invoice_line_not_standalone.rst
 tests/scenario_purchase_invoice_line_standalone.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_purchase_invoice_line_standalone.egg-info/PKG-INFO
 trytond_purchase_invoice_line_standalone.egg-info/SOURCES.txt
 trytond_purchase_invoice_line_standalone.egg-info/dependency_links.txt
 trytond_purchase_invoice_line_standalone.egg-info/entry_points.txt
 trytond_purchase_invoice_line_standalone.egg-info/not-zip-safe
 trytond_purchase_invoice_line_standalone.egg-info/requires.txt
 trytond_purchase_invoice_line_standalone.egg-info/top_level.txt
-view/invoice_line_tree_invoice_type.xml
+view/invoice_line_tree_invoice_type.xml
+view/party_form.xml
```

### Comparing `trytond_purchase_invoice_line_standalone-6.6.0/view/invoice_line_tree_invoice_type.xml` & `trytond_purchase_invoice_line_standalone-6.8.0/view/invoice_line_tree_invoice_type.xml`

 * *Files identical despite different names*

