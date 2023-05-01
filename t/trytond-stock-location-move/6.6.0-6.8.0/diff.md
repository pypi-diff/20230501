# Comparing `tmp/trytond_stock_location_move-6.6.0.tar.gz` & `tmp/trytond_stock_location_move-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_location_move-6.6.0.tar", last modified: Mon Oct 31 16:21:55 2022, max compression
+gzip compressed data, was "trytond_stock_location_move-6.8.0.tar", last modified: Mon May  1 11:36:46 2023, max compression
```

## Comparing `trytond_stock_location_move-6.6.0.tar` & `trytond_stock_location_move-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:55.639871 trytond_stock_location_move-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_stock_location_move-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_location_move-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-31 16:21:54.000000 trytond_stock_location_move-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_location_move-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2022-10-31 16:21:53.000000 trytond_stock_location_move-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:21:53.000000 trytond_stock_location_move-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_stock_location_move-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_location_move-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2730 2022-10-31 16:21:55.639871 trytond_stock_location_move-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2019-06-04 16:49:46.000000 trytond_stock_location_move-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2021-12-11 16:59:34.000000 trytond_stock_location_move-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:55.629870 trytond_stock_location_move-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2019-06-04 16:49:46.000000 trytond_stock_location_move-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:55.603203 trytond_stock_location_move-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1240 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1223 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1073 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1295 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1291 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2022-10-29 07:50:32.000000 trytond_stock_location_move-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2019-08-09 14:52:50.000000 trytond_stock_location_move-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2021-12-11 16:59:34.000000 trytond_stock_location_move-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:21:55.639871 trytond_stock_location_move-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5223 2022-10-29 07:39:12.000000 trytond_stock_location_move-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9001 2022-10-11 19:49:58.000000 trytond_stock_location_move-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3438 2019-06-04 16:49:46.000000 trytond_stock_location_move-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:55.619870 trytond_stock_location_move-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_location_move-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3735 2022-10-11 19:49:58.000000 trytond_stock_location_move-6.6.0/tests/scenario_stock_location_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-09-29 07:07:38.000000 trytond_stock_location_move-6.6.0/tests/scenario_stock_location_move_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3252 2020-07-09 09:37:30.000000 trytond_stock_location_move-6.6.0/tests/scenario_stock_location_move_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2022-04-16 16:30:57.000000 trytond_stock_location_move-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_location_move-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-31 15:10:09.000000 trytond_stock_location_move-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2022-10-31 16:21:52.000000 trytond_stock_location_move-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:55.639871 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2730 2022-10-31 16:21:54.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1815 2022-10-31 16:21:55.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:21:54.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2022-10-31 16:21:54.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:49.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       99 2022-10-31 16:21:54.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:21:54.000000 trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:55.623204 trytond_stock_location_move-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2019-06-04 16:49:46.000000 trytond_stock_location_move-6.6.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2019-06-04 16:49:46.000000 trytond_stock_location_move-6.6.0/view/shipment_internal_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:46.985491 trytond_stock_location_move-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-05-01 10:57:58.000000 trytond_stock_location_move-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 10:57:58.000000 trytond_stock_location_move-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_location_move-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2718 2023-05-01 11:36:46.985491 trytond_stock_location_move-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-01-16 14:00:21.000000 trytond_stock_location_move-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:46.985491 trytond_stock_location_move-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-01-16 14:00:21.000000 trytond_stock_location_move-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:46.982158 trytond_stock_location_move-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1223 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1073 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1295 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1291 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-29 08:02:39.000000 trytond_stock_location_move-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:36:46.985491 trytond_stock_location_move-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4408 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9001 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3438 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:46.982158 trytond_stock_location_move-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3735 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tests/scenario_stock_location_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5101 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tests/scenario_stock_location_move_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3253 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tests/scenario_stock_location_move_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_location_move-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-05-01 10:57:53.000000 trytond_stock_location_move-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:46.985491 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2718 2023-05-01 11:36:46.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1789 2023-05-01 11:36:46.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:36:46.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 11:36:46.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       99 2023-05-01 11:36:46.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:36:46.000000 trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:46.982158 trytond_stock_location_move-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:21.000000 trytond_stock_location_move-6.8.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-01-16 14:00:21.000000 trytond_stock_location_move-6.8.0/view/shipment_internal_form.xml
```

### Comparing `trytond_stock_location_move-6.6.0/CHANGELOG` & `trytond_stock_location_move-6.8.0/CHANGELOG`

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

### Comparing `trytond_stock_location_move-6.6.0/COPYRIGHT` & `trytond_stock_location_move-6.8.0/COPYRIGHT`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2017-2022 Cédric Krier
+Copyright (C) 2017-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_location_move-6.6.0/LICENSE` & `trytond_stock_location_move-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/PKG-INFO` & `trytond_stock_location_move-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_location_move
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to move storage locations
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_location_move
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock location
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Stock Location Move Module
 ##########################
 
 The stock location move module allows to define some *Locations* as movable
```

### Comparing `trytond_stock_location_move-6.6.0/README.rst` & `trytond_stock_location_move-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/__init__.py` & `trytond_stock_location_move-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/doc/index.rst` & `trytond_stock_location_move-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/bg.po` & `trytond_stock_location_move-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/ca.po` & `trytond_stock_location_move-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/cs.po` & `trytond_stock_location_move-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/de.po` & `trytond_stock_location_move-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/es.po` & `trytond_stock_location_move-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/es_419.po` & `trytond_stock_location_move-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/et.po` & `trytond_stock_location_move-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/fa.po` & `trytond_stock_location_move-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/fi.po` & `trytond_stock_location_move-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/fr.po` & `trytond_stock_location_move-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/hu.po` & `trytond_stock_location_move-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/id.po` & `trytond_stock_location_move-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/it.po` & `trytond_stock_location_move-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/lo.po` & `trytond_stock_location_move-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/lt.po` & `trytond_stock_location_move-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/nl.po` & `trytond_stock_location_move-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/pl.po` & `trytond_stock_location_move-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/pt.po` & `trytond_stock_location_move-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/ro.po` & `trytond_stock_location_move-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/ru.po` & `trytond_stock_location_move-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/sl.po` & `trytond_stock_location_move-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/tr.po` & `trytond_stock_location_move-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/uk.po` & `trytond_stock_location_move-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/locale/zh_CN.po` & `trytond_stock_location_move-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/product.py` & `trytond_stock_location_move-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/setup.py` & `trytond_stock_location_move-6.8.0/setup.py`

 * *Files 26% similar despite different names*

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
@@ -34,62 +31,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_location_move'
 
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
 for dep in info.get('extras_depend', []):
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to move storage locations',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_location_move',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock location',
     package_dir={'trytond.modules.stock_location_move': '.'},
     packages=(
         ['trytond.modules.stock_location_move']
         + ['trytond.modules.stock_location_move.%s' % p
             for p in find_packages()]
@@ -125,27 +103,26 @@
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
     stock_location_move = trytond.modules.stock_location_move
     """,
     )
```

### Comparing `trytond_stock_location_move-6.6.0/stock.py` & `trytond_stock_location_move-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/stock.xml` & `trytond_stock_location_move-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-6.6.0/tests/scenario_stock_location_move.rst` & `trytond_stock_location_move-6.8.0/tests/scenario_stock_location_move.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ============================
 Stock Location Move Scenario
 ============================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + datetime.timedelta(1)
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_location_move')
 
 Create company::
 
@@ -39,15 +39,14 @@
     >>> shipment = Shipment()
     >>> shipment.from_location = storage1
     >>> shipment.to_location = storage2
     >>> shipment.locations.append(Location(pallet.id))
     >>> shipment.click('wait')
 
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> pallet.reload()
     >>> pallet.assigned_by == shipment
     True
     >>> pallet.parent == storage1
     True
@@ -83,15 +82,16 @@
     >>> shipment2 = Shipment()
     >>> shipment2.from_location = storage2
     >>> shipment2.to_location = storage1
     >>> shipment2.locations.append(Location(pallet.id))
     >>> shipment2.click('wait')
 
     >>> shipment1.click('assign_try')
-    True
+    >>> shipment1.state
+    'assigned'
     >>> shipment2.click('assign_try')  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     AssignError: ...
 
     >>> shipment1.click('done')
 
@@ -100,28 +100,27 @@
     >>> warehouse1 = storage_loc.warehouse
     >>> warehouse2, = warehouse1.duplicate()
 
     >>> LeadTime = Model.get('stock.location.lead_time')
     >>> lead_time = LeadTime()
     >>> lead_time.warehouse_from = warehouse1
     >>> lead_time.warehouse_to = warehouse2
-    >>> lead_time.lead_time = datetime.timedelta(1)
+    >>> lead_time.lead_time = dt.timedelta(1)
     >>> lead_time.save()
 
 Move pallet from storage1 to storage2 with lead_time::
 
     >>> Shipment = Model.get('stock.shipment.internal')
     >>> shipment = Shipment()
     >>> shipment.planned_date = tomorrow
     >>> shipment.from_location = warehouse1.storage_location
     >>> shipment.to_location = warehouse2.storage_location
     >>> shipment.locations.append(Location(pallet.id))
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
-    True
 
     >>> shipment.click('ship')
     >>> pallet.reload()
     >>> pallet.parent == shipment.transit_location
     True
 
     >>> shipment.click('done')
```

### Comparing `trytond_stock_location_move-6.6.0/tests/scenario_stock_location_move_empty.rst` & `trytond_stock_location_move-6.8.0/tests/scenario_stock_location_move_empty.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ==================================
 Stock Location Move Empty Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> yesterday = today - datetime.timedelta(1)
-    >>> tomorrow = today + datetime.timedelta(1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(1)
+    >>> tomorrow = today + dt.timedelta(1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_location_move')
 
 Create company::
 
@@ -128,15 +129,14 @@
     >>> move.quantity = 1
     >>> move.unit_price = Decimal('0')
     >>> move.currency = company.currency
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> shipment.click('pack')
     >>> shipment.click('done')
 
 Check empty non movable location are still active::
 
     >>> storage1.reload()
```

### Comparing `trytond_stock_location_move-6.6.0/tests/scenario_stock_location_move_supply.rst` & `trytond_stock_location_move-6.8.0/tests/scenario_stock_location_move_supply.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 ==========================
 Stock Location Move Supply
 ==========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['stock_location_move', 'stock_supply'])
 
 Create customer::
```

### Comparing `trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/PKG-INFO` & `trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-location-move
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to move storage locations
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_location_move
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock location
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Stock Location Move Module
 ##########################
 
 The stock location move module allows to define some *Locations* as movable
```

### Comparing `trytond_stock_location_move-6.6.0/trytond_stock_location_move.egg-info/SOURCES.txt` & `trytond_stock_location_move-6.8.0/trytond_stock_location_move.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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
 message.xml
@@ -49,14 +45,15 @@
 ./tests/scenario_stock_location_move.rst
 ./tests/scenario_stock_location_move_empty.rst
 ./tests/scenario_stock_location_move_supply.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/location_form.xml
 ./view/shipment_internal_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

