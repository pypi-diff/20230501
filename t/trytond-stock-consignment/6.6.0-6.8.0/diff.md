# Comparing `tmp/trytond_stock_consignment-6.6.0.tar.gz` & `tmp/trytond_stock_consignment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_consignment-6.6.0.tar", last modified: Mon Oct 31 16:21:41 2022, max compression
+gzip compressed data, was "trytond_stock_consignment-6.8.0.tar", last modified: Mon May  1 11:52:18 2023, max compression
```

## Comparing `trytond_stock_consignment-6.6.0.tar` & `trytond_stock_consignment-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:41.112739 trytond_stock_consignment-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_stock_consignment-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_consignment-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-31 16:21:39.000000 trytond_stock_consignment-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_consignment-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1024 2022-10-31 16:21:39.000000 trytond_stock_consignment-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:21:38.000000 trytond_stock_consignment-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_stock_consignment-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_consignment-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3492 2022-10-31 16:21:41.112739 trytond_stock_consignment-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2019-06-04 16:49:46.000000 trytond_stock_consignment-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2021-12-11 16:59:34.000000 trytond_stock_consignment-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2021-12-11 16:59:34.000000 trytond_stock_consignment-6.6.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:41.112739 trytond_stock_consignment-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2019-06-04 16:49:46.000000 trytond_stock_consignment-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:41.109405 trytond_stock_consignment-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-10-29 07:50:39.000000 trytond_stock_consignment-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:21:41.112739 trytond_stock_consignment-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5276 2022-10-29 07:39:11.000000 trytond_stock_consignment-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10799 2022-10-11 19:49:58.000000 trytond_stock_consignment-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-11 19:49:58.000000 trytond_stock_consignment-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:41.109405 trytond_stock_consignment-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_consignment-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8379 2022-09-29 07:07:38.000000 trytond_stock_consignment-6.6.0/tests/scenario_stock_consignment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5411 2020-07-09 09:37:29.000000 trytond_stock_consignment-6.6.0/tests/scenario_stock_consignment_supplier_customer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2022-04-16 16:30:57.000000 trytond_stock_consignment-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_consignment-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      712 2022-10-31 15:10:09.000000 trytond_stock_consignment-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2022-10-31 16:21:37.000000 trytond_stock_consignment-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:41.112739 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3492 2022-10-31 16:21:40.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1683 2022-10-31 16:21:41.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:21:40.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 16:21:40.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:02.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2022-10-31 16:21:40.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:21:40.000000 trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:21:41.109405 trytond_stock_consignment-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2022-09-12 22:47:25.000000 trytond_stock_consignment-6.6.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2022-10-11 19:49:58.000000 trytond_stock_consignment-6.6.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:18.677053 trytond_stock_consignment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-05-01 11:08:16.000000 trytond_stock_consignment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:08:16.000000 trytond_stock_consignment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_consignment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3482 2023-05-01 11:52:18.677053 trytond_stock_consignment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-01-16 14:00:21.000000 trytond_stock_consignment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:18.673720 trytond_stock_consignment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-01-16 14:00:21.000000 trytond_stock_consignment-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:18.670386 trytond_stock_consignment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-29 08:02:45.000000 trytond_stock_consignment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:52:18.677053 trytond_stock_consignment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4463 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10971 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:18.670386 trytond_stock_consignment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8367 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/tests/scenario_stock_consignment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5393 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/tests/scenario_stock_consignment_supplier_customer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-05-01 11:08:10.000000 trytond_stock_consignment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:18.677053 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3482 2023-05-01 11:52:17.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-05-01 11:52:18.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:52:17.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:52:17.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-05-01 11:52:17.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:52:17.000000 trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:18.673720 trytond_stock_consignment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_stock_consignment-6.8.0/view/stock_move_form.xml
```

### Comparing `trytond_stock_consignment-6.6.0/CHANGELOG` & `trytond_stock_consignment-6.8.0/CHANGELOG`

 * *Files 18% similar despite different names*

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

### Comparing `trytond_stock_consignment-6.6.0/COPYRIGHT` & `trytond_stock_consignment-6.8.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2022 Cédric Krier
-Copyright (C) 2017-2022 B2CK
+Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_consignment-6.6.0/LICENSE` & `trytond_stock_consignment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/PKG-INFO` & `trytond_stock_consignment-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_consignment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to manage consignment stock
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_consignment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock consignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 
 Stock Consignment Module
 ########################
 
 The stock consignment modules allow to manage consignment stock from supplier
```

### Comparing `trytond_stock_consignment-6.6.0/README.rst` & `trytond_stock_consignment-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/__init__.py` & `trytond_stock_consignment-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/account.py` & `trytond_stock_consignment-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/doc/index.rst` & `trytond_stock_consignment-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/locale/fa.po` & `trytond_stock_consignment-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/setup.py` & `trytond_stock_consignment-6.8.0/setup.py`

 * *Files 11% similar despite different names*

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
@@ -34,61 +31,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_consignment'
 
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
 
 tests_require = [get_require_version('proteus'),
     get_require_version('trytond_stock_supply')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to manage consignment stock',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_consignment',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock consignment',
     package_dir={'trytond.modules.stock_consignment': '.'},
     packages=(
         ['trytond.modules.stock_consignment']
         + ['trytond.modules.stock_consignment.%s' % p for p in find_packages()]
         ),
@@ -126,27 +104,26 @@
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
     stock_consignment = trytond.modules.stock_consignment
     """,
     )
```

### Comparing `trytond_stock_consignment-6.6.0/stock.py` & `trytond_stock_consignment-6.8.0/stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,24 +140,32 @@
             name=name)
         if self.from_location:
             if (self.from_location.type == 'supplier'
                     and self.from_location.warehouse):
                 required = True
         return required
 
+    @property
+    def is_supplier_consignment(self):
+        return (self.from_location.type == 'supplier'
+            and self.to_location.type in {'storage', 'production', 'customer'}
+            and self.from_location.consignment_party)
+
+    @property
+    def is_customer_consignment(self):
+        return (
+            self.from_location.type in {'storage', 'production', 'supplier'}
+            and self.to_location.type == 'customer'
+            and self.from_location.consignment_party)
+
     def get_invoice_lines_consignment(self):
         lines = []
-        if (self.from_location.type == 'supplier'
-                and self.to_location.type in {
-                    'storage', 'production', 'customer'}
-                and self.from_location.consignment_party):
+        if self.is_supplier_consignment:
             lines.append(self._get_supplier_invoice_line_consignment())
-        if (self.from_location.type in {'storage', 'production', 'supplier'}
-                and self.to_location.type == 'customer'
-                and self.from_location.consignment_party):
+        if self.is_customer_consignment:
             lines.append(self._get_customer_invoice_line_consignment())
         return lines
 
     def _get_supplier_invoice_line_consignment(self):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
         Product = pool.get('product.product')
```

### Comparing `trytond_stock_consignment-6.6.0/stock.xml` & `trytond_stock_consignment-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-6.6.0/tests/scenario_stock_consignment.rst` & `trytond_stock_consignment-6.8.0/tests/scenario_stock_consignment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,14 @@
     >>> move.quantity = 10
     >>> move.from_location = supplier_loc
     >>> move.to_location = supplier_consignment_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('done')
     >>> shipment.state
     'done'
 
 Use supplier consignment stock::
@@ -138,15 +137,14 @@
     >>> move.quantity = 4
     >>> move.from_location = supplier_consignment_loc
     >>> move.to_location = storage_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('done')
     >>> shipment.state
     'done'
 
 Check supplier invoice line::
@@ -180,15 +178,16 @@
     >>> move.currency = company.currency
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment_out.click('wait')
     >>> move, = shipment_out.inventory_moves
     >>> move.from_location = supplier_consignment_loc
     >>> shipment_out.click('assign_try')
-    True
+    >>> shipment_out.state
+    'assigned'
     >>> move, = shipment_out.inventory_moves
     >>> len(move.invoice_lines)
     1
 
 Fill customer consignment location::
 
     >>> shipment = Shipment()
@@ -199,15 +198,14 @@
     >>> move.quantity = 3
     >>> move.from_location = storage_loc
     >>> move.to_location = customer_consignment_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('done')
     >>> shipment.state
     'done'
 
 Use customer consignment stock::
@@ -220,15 +218,14 @@
     >>> move.quantity = 1
     >>> move.from_location = customer_consignment_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('done')
     >>> shipment.state
     'done'
 
 Check customer invoice line::
@@ -264,15 +261,14 @@
     >>> move.quantity = 1
     >>> move.from_location = supplier_consignment_loc
     >>> move.to_location = storage_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> move, = shipment.moves
     >>> bool(move.origin)
     True
     >>> shipment.click('cancel')
     >>> shipment.state
```

### Comparing `trytond_stock_consignment-6.6.0/tests/scenario_stock_consignment_supplier_customer.rst` & `trytond_stock_consignment-6.8.0/tests/scenario_stock_consignment_supplier_customer.rst`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
     >>> move.quantity = 10
     >>> move.from_location = supplier_loc
     >>> move.to_location = supplier_consignment_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('done')
     >>> shipment.state
     'done'
 
 Use supplier consignment stock by customer::
@@ -129,15 +128,14 @@
     >>> move.quantity = 4
     >>> move.from_location = supplier_consignment_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('done')
     >>> shipment.state
     'done'
     >>> move, = shipment.moves
     >>> len(move.invoice_lines)
```

### Comparing `trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/PKG-INFO` & `trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-consignment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to manage consignment stock
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_consignment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock consignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 
 Stock Consignment Module
 ########################
 
 The stock consignment modules allow to manage consignment stock from supplier
```

### Comparing `trytond_stock_consignment-6.6.0/trytond_stock_consignment.egg-info/SOURCES.txt` & `trytond_stock_consignment-6.8.0/trytond_stock_consignment.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
@@ -46,14 +42,15 @@
 ./tests/__init__.py
 ./tests/scenario_stock_consignment.rst
 ./tests/scenario_stock_consignment_supplier_customer.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/location_form.xml
 ./view/stock_move_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

