# Comparing `tmp/trytond_account_invoice_stock-6.6.0.tar.gz` & `tmp/trytond_account_invoice_stock-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_stock-6.6.0.tar", last modified: Mon Oct 31 16:02:25 2022, max compression
+gzip compressed data, was "trytond_account_invoice_stock-6.8.0.tar", last modified: Mon May  1 11:42:07 2023, max compression
```

## Comparing `trytond_account_invoice_stock-6.6.0.tar` & `trytond_account_invoice_stock-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:25.269267 trytond_account_invoice_stock-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2196 2022-04-25 16:35:01.000000 trytond_account_invoice_stock-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_invoice_stock-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2022-10-31 16:02:23.000000 trytond_account_invoice_stock-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_invoice_stock-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2298 2022-10-31 16:02:22.000000 trytond_account_invoice_stock-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:02:22.000000 trytond_account_invoice_stock-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:05.000000 trytond_account_invoice_stock-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_invoice_stock-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2623 2022-10-31 16:02:25.269267 trytond_account_invoice_stock-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2022-10-27 11:24:44.000000 trytond_account_invoice_stock-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2021-12-11 16:59:32.000000 trytond_account_invoice_stock-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5162 2022-10-11 19:49:57.000000 trytond_account_invoice_stock-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2019-02-13 10:09:05.000000 trytond_account_invoice_stock-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:25.269267 trytond_account_invoice_stock-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-02-18 23:10:26.000000 trytond_account_invoice_stock-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2022-10-27 11:24:44.000000 trytond_account_invoice_stock-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_account_invoice_stock-6.6.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:25.265933 trytond_account_invoice_stock-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1302 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1320 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1309 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1317 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1071 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1290 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1159 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1291 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1277 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1237 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1321 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2022-10-29 07:50:34.000000 trytond_account_invoice_stock-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:02:25.269267 trytond_account_invoice_stock-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5410 2022-10-29 07:39:10.000000 trytond_account_invoice_stock-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4448 2022-04-10 15:40:34.000000 trytond_account_invoice_stock-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2019-02-13 10:09:05.000000 trytond_account_invoice_stock-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:25.265933 trytond_account_invoice_stock-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_invoice_stock-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4004 2022-09-29 07:07:37.000000 trytond_account_invoice_stock-6.6.0/tests/scenario_account_invoice_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3785 2022-09-29 07:07:37.000000 trytond_account_invoice_stock-6.6.0/tests/scenario_account_invoice_stock_correction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-04-16 16:30:56.000000 trytond_account_invoice_stock-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_invoice_stock-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 15:10:09.000000 trytond_account_invoice_stock-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2022-10-31 16:02:20.000000 trytond_account_invoice_stock-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:25.269267 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2623 2022-10-31 16:02:24.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1764 2022-10-31 16:02:25.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:02:24.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:02:24.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:52.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2022-10-31 16:02:24.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:02:24.000000 trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:25.265933 trytond_account_invoice_stock-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2021-04-03 16:10:54.000000 trytond_account_invoice_stock-6.6.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2022-10-11 19:49:57.000000 trytond_account_invoice_stock-6.6.0/view/move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.689471 trytond_account_invoice_stock-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2461 2023-05-01 11:01:33.000000 trytond_account_invoice_stock-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:01:33.000000 trytond_account_invoice_stock-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2609 2023-05-01 11:42:07.686138 trytond_account_invoice_stock-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5162 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.686138 trytond_account_invoice_stock-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.682804 trytond_account_invoice_stock-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1302 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1320 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1317 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1071 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1298 2023-04-30 10:46:36.000000 trytond_account_invoice_stock-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1159 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1291 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1277 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-04-30 10:46:36.000000 trytond_account_invoice_stock-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1321 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:07.689471 trytond_account_invoice_stock-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4593 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4448 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.682804 trytond_account_invoice_stock-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4004 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3792 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock_correction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-05-01 11:01:27.000000 trytond_account_invoice_stock-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.686138 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2609 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-01 11:42:07.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.682804 trytond_account_invoice_stock-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/view/move_form.xml
```

### Comparing `trytond_account_invoice_stock-6.6.0/CHANGELOG` & `trytond_account_invoice_stock-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

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
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_invoice_stock-6.6.0/COPYRIGHT` & `trytond_account_invoice_stock-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_invoice_stock-6.6.0/LICENSE` & `trytond_account_invoice_stock-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/PKG-INFO` & `trytond_account_invoice_stock-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_stock
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to link stock and invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-stock/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_stock
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice stock
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
 
 ############################
 Account Invoice Stock Module
 ############################
```

### Comparing `trytond_account_invoice_stock-6.6.0/account.py` & `trytond_account_invoice_stock-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/doc/conf.py` & `trytond_account_invoice_stock-6.8.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-modules_url = 'https://docs.tryton.org/projects/modules-{module}/en/{series}/'
-trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+import os
+
+base_url = os.environ.get('DOC_BASE_URL')
+if base_url:
+    modules_url = base_url + '/modules-{module}/'
+    trytond_url = base_url + '/server/'
+else:
+    modules_url = (
+        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
+    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
 
 
 def get_info():
     import configparser
-    import os
     import subprocess
     import sys
 
     module_dir = os.path.dirname(os.path.dirname(__file__))
 
     config = configparser.ConfigParser()
     config.read_file(open(os.path.join(module_dir, 'tryton.cfg')))
@@ -22,15 +29,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     for key in {'depends', 'extras_depend'}:
         info[key] = info.get(key, '').strip().splitlines()
     info['modules'] = set(info['depends'] + info['extras_depend'])
@@ -53,9 +63,10 @@
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
+linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
-del get_info, info, modules_url, trytond_url
+del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_account_invoice_stock-6.6.0/locale/bg.po` & `trytond_account_invoice_stock-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/ca.po` & `trytond_account_invoice_stock-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/cs.po` & `trytond_account_invoice_stock-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/de.po` & `trytond_account_invoice_stock-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/es.po` & `trytond_account_invoice_stock-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/es_419.po` & `trytond_account_invoice_stock-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/et.po` & `trytond_account_invoice_stock-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/fa.po` & `trytond_account_invoice_stock-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/fi.po` & `trytond_account_invoice_stock-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/fr.po` & `trytond_account_invoice_stock-6.8.0/locale/fr.po`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 msgctxt "field:stock.move,invoice_types:"
 msgid "Invoice Types"
 msgstr "Types de factures"
 
 msgctxt "help:account.invoice.line,correction:"
 msgid "Check to correct price of already posted invoice."
-msgstr "Cocher pour corriger le prix de la facture déjà postée."
+msgstr "Cocher pour corriger le prix de la facture déjà comptabilisées."
 
 msgctxt "model:account.invoice.line-stock.move,name:"
 msgid "Invoice Line - Stock Move"
 msgstr "Ligne de facture - Mouvement de stock"
 
 msgctxt "view:account.invoice.line:"
 msgid "Stock"
```

### Comparing `trytond_account_invoice_stock-6.6.0/locale/hu.po` & `trytond_account_invoice_stock-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/id.po` & `trytond_account_invoice_stock-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/it.po` & `trytond_account_invoice_stock-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/lo.po` & `trytond_account_invoice_stock-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/lt.po` & `trytond_account_invoice_stock-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/nl.po` & `trytond_account_invoice_stock-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/pl.po` & `trytond_account_invoice_stock-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/pt.po` & `trytond_account_invoice_stock-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/ro.po` & `trytond_account_invoice_stock-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice,shipments:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:account.invoice.line,correction:"
 msgid "Correction"
 msgstr "Corecţie"
 
 msgctxt "field:account.invoice.line,shipments:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:account.invoice.line,stock_moves:"
 msgid "Stock Moves"
 msgstr "Mişcări Stoc"
 
 msgctxt "field:account.invoice.line,warehouse:"
 msgid "Warehouse"
```

### Comparing `trytond_account_invoice_stock-6.6.0/locale/ru.po` & `trytond_account_invoice_stock-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/sl.po` & `trytond_account_invoice_stock-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/tr.po` & `trytond_account_invoice_stock-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/uk.po` & `trytond_account_invoice_stock-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/locale/zh_CN.po` & `trytond_account_invoice_stock-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/setup.py` & `trytond_account_invoice_stock-6.8.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     content = re.sub(
         r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
     return content
 
 
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
@@ -37,61 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_invoice_stock'
 
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
     description='Tryton module to link stock and invoice',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
         'https://docs.tryton.org/projects/modules-account-invoice-stock/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_invoice_stock',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice stock',
     package_dir={'trytond.modules.account_invoice_stock': '.'},
     packages=(
         ['trytond.modules.account_invoice_stock']
         + ['trytond.modules.account_invoice_stock.%s' % p
             for p in find_packages()]
@@ -128,28 +106,27 @@
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
     account_invoice_stock = trytond.modules.account_invoice_stock
     """,
     )
```

### Comparing `trytond_account_invoice_stock-6.6.0/stock.py` & `trytond_account_invoice_stock-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/tests/scenario_account_invoice_stock.rst` & `trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.6.0/tests/scenario_account_invoice_stock_correction.rst` & `trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock_correction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
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

### Comparing `trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/PKG-INFO` & `trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-stock
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to link stock and invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-stock/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_stock
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice stock
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
 
 ############################
 Account Invoice Stock Module
 ############################
```

### Comparing `trytond_account_invoice_stock-6.6.0/trytond_account_invoice_stock.egg-info/SOURCES.txt` & `trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

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
```

### Comparing `trytond_account_invoice_stock-6.6.0/view/invoice_line_form.xml` & `trytond_account_invoice_stock-6.8.0/view/invoice_line_form.xml`

 * *Files identical despite different names*

