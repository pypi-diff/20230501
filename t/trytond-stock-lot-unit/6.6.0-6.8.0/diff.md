# Comparing `tmp/trytond_stock_lot_unit-6.6.0.tar.gz` & `tmp/trytond_stock_lot_unit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot_unit-6.6.0.tar", last modified: Mon Oct 31 16:27:46 2022, max compression
+gzip compressed data, was "trytond_stock_lot_unit-6.8.0.tar", last modified: Mon May  1 12:01:08 2023, max compression
```

## Comparing `trytond_stock_lot_unit-6.6.0.tar` & `trytond_stock_lot_unit-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:46.908472 trytond_stock_lot_unit-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_stock_lot_unit-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_lot_unit-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2022-10-31 16:27:45.000000 trytond_stock_lot_unit-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_lot_unit-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2022-10-31 16:27:44.000000 trytond_stock_lot_unit-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 16:27:44.000000 trytond_stock_lot_unit-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_lot_unit-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2639 2022-10-31 16:27:46.908472 trytond_stock_lot_unit-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2021-12-11 16:59:34.000000 trytond_stock_lot_unit-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:46.905139 trytond_stock_lot_unit-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:46.905139 trytond_stock_lot_unit-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2267 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2378 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2278 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2620 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2363 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2370 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:43.000000 trytond_stock_lot_unit-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2019-08-09 14:52:51.000000 trytond_stock_lot_unit-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2022-04-10 15:40:36.000000 trytond_stock_lot_unit-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:27:46.908472 trytond_stock_lot_unit-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5143 2022-10-29 07:39:12.000000 trytond_stock_lot_unit-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7375 2022-04-10 15:40:36.000000 trytond_stock_lot_unit-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2021-02-03 20:19:16.000000 trytond_stock_lot_unit-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:46.905139 trytond_stock_lot_unit-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_lot_unit-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5827 2022-09-29 07:07:38.000000 trytond_stock_lot_unit-6.6.0/tests/scenario_stock_lot_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1938 2022-09-29 07:07:38.000000 trytond_stock_lot_unit-6.6.0/tests/scenario_stock_lot_unit_move_add.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-04-16 16:30:57.000000 trytond_stock_lot_unit-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_lot_unit-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2022-10-31 15:10:09.000000 trytond_stock_lot_unit-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2022-10-31 16:27:43.000000 trytond_stock_lot_unit-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:46.908472 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2639 2022-10-31 16:27:46.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1738 2022-10-31 16:27:46.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:27:46.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 16:27:46.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:12.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-31 16:27:46.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:27:46.000000 trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:46.905139 trytond_stock_lot_unit-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/view/lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2019-06-04 16:49:46.000000 trytond_stock_lot_unit-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:08.000289 trytond_stock_lot_unit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      913 2023-05-01 11:14:27.000000 trytond_stock_lot_unit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 11:14:27.000000 trytond_stock_lot_unit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2634 2023-05-01 12:01:08.000289 trytond_stock_lot_unit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:08.000289 trytond_stock_lot_unit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:07.996955 trytond_stock_lot_unit-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2267 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2378 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2278 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2620 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2363 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2370 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:49.000000 trytond_stock_lot_unit-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:01:08.000289 trytond_stock_lot_unit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4333 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7318 2023-04-21 08:36:08.000000 trytond_stock_lot_unit-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:07.996955 trytond_stock_lot_unit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5681 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/tests/scenario_stock_lot_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1930 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/tests/scenario_stock_lot_unit_move_add.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 11:14:21.000000 trytond_stock_lot_unit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:08.000289 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2634 2023-05-01 12:01:07.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2023-05-01 12:01:07.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:07.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 12:01:07.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-05-01 12:01:07.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:01:07.000000 trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:07.996955 trytond_stock_lot_unit-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-6.8.0/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-6.8.0/view/lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-6.8.0/view/template_form.xml
```

### Comparing `trytond_stock_lot_unit-6.6.0/CHANGELOG` & `trytond_stock_lot_unit-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_stock_lot_unit-6.6.0/COPYRIGHT` & `trytond_stock_lot_unit-6.8.0/COPYRIGHT`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2018-2022 Cédric Krier
-Copyright (C) 2017-2022 Nicolas Évrard
-Copyright (C) 2017-2022 B2CK
+Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2017-2023 Nicolas Évrard
+Copyright (C) 2017-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_lot_unit-6.6.0/LICENSE` & `trytond_stock_lot_unit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/PKG-INFO` & `trytond_stock_lot_unit-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot_unit
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to define unit on stock lot
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_lot_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock lot unit serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,28 +37,29 @@
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
 
 Stock Lot Unit Module
 #####################
 
-The `stock_lot_unit` module allows to define a unit and quantity on stock lot.
+The ``stock_lot_unit`` module allows to define a unit and quantity on stock
+lot.
 
 Lots with unit have the following properties:
 
     - no shipment may contain a summed quantity for a lot greater than the
       quantity of the lot.
     - no move related to a lot with a unit may concern a quantity greater than
       the quantity of the lot.
```

### Comparing `trytond_stock_lot_unit-6.6.0/__init__.py` & `trytond_stock_lot_unit-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/bg.po` & `trytond_stock_lot_unit-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/ca.po` & `trytond_stock_lot_unit-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/cs.po` & `trytond_stock_lot_unit-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/de.po` & `trytond_stock_lot_unit-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/es.po` & `trytond_stock_lot_unit-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/es_419.po` & `trytond_stock_lot_unit-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/et.po` & `trytond_stock_lot_unit-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/fa.po` & `trytond_stock_lot_unit-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/fi.po` & `trytond_stock_lot_unit-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/fr.po` & `trytond_stock_lot_unit-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/hu.po` & `trytond_stock_lot_unit-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/id.po` & `trytond_stock_lot_unit-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/it.po` & `trytond_stock_lot_unit-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/lo.po` & `trytond_stock_lot_unit-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/lt.po` & `trytond_stock_lot_unit-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/nl.po` & `trytond_stock_lot_unit-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/pl.po` & `trytond_stock_lot_unit-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/pt.po` & `trytond_stock_lot_unit-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/ro.po` & `trytond_stock_lot_unit-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/ru.po` & `trytond_stock_lot_unit-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/sl.po` & `trytond_stock_lot_unit-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/tr.po` & `trytond_stock_lot_unit-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/uk.po` & `trytond_stock_lot_unit-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/locale/zh_CN.po` & `trytond_stock_lot_unit-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/message.xml` & `trytond_stock_lot_unit-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/product.py` & `trytond_stock_lot_unit-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/setup.py` & `trytond_stock_lot_unit-6.8.0/setup.py`

 * *Files 23% similar despite different names*

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
 name = 'trytond_stock_lot_unit'
 
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
     get_require_version('trytond_production')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to define unit on stock lot',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_lot_unit',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock lot unit serial',
     package_dir={'trytond.modules.stock_lot_unit': '.'},
     packages=(
         ['trytond.modules.stock_lot_unit']
         + ['trytond.modules.stock_lot_unit.%s' % p for p in find_packages()]
         ),
@@ -124,27 +102,26 @@
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
     stock_lot_unit = trytond.modules.stock_lot_unit
     """,
     )
```

### Comparing `trytond_stock_lot_unit-6.6.0/stock.py` & `trytond_stock_lot_unit-6.8.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     def on_change_unit(self):
         if self.unit:
             self.unit_quantity = self.unit.rounding
 
     @fields.depends('product')
     def on_change_with_product_default_uom_category(self, name=None):
         if self.product:
-            category = self.product.default_uom_category
-            return category.id if category else None
+            return self.product.default_uom_category
 
 
 class Lot(LotUnitMixin, metaclass=PoolMeta):
     __name__ = 'stock.lot'
 
     @classmethod
     def __setup__(cls):
```

### Comparing `trytond_stock_lot_unit-6.6.0/stock.xml` & `trytond_stock_lot_unit-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-6.6.0/tests/scenario_stock_lot_unit.rst` & `trytond_stock_lot_unit-6.8.0/tests/scenario_stock_lot_unit.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 =======================
 Stock Lot Unit Scenario
 =======================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import config, Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot_unit')
 
 Create company::
 
@@ -99,15 +96,14 @@
     >>> move.quantity = 1
     >>> move.unit_price = Decimal('20')
     >>> move.currency = company.currency
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
-    True
     >>> move.lot = lot
     >>> shipment.click('pick')
     >>> shipment.click('pack')
     >>> shipment.click('done')
 
 Let's ship now two times the same lot::
 
@@ -128,15 +124,14 @@
     >>> move2.quantity = 1
     >>> move2.unit_price = Decimal('20')
     >>> move2.currency = company.currency
     >>> move2.from_location = output_loc
     >>> move2.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
-    True
     >>> move1, move2 = shipment.inventory_moves
     >>> move1.lot = lot
     >>> move2.lot = lot
     >>> shipment.save()
     >>> shipment.click('pick')  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
@@ -155,15 +150,14 @@
     >>> move.quantity = 4
     >>> move.unit_price = Decimal('20')
     >>> move.currency = company.currency
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
-    True
     >>> move, = shipment.inventory_moves
     >>> move.lot = lot
     >>> shipment.click('pick')  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     LotUnitQuantityError: ...
```

### Comparing `trytond_stock_lot_unit-6.6.0/tests/scenario_stock_lot_unit_move_add.rst` & `trytond_stock_lot_unit-6.8.0/tests/scenario_stock_lot_unit_move_add.rst`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     >>> lot = Lot(number='01', product=product)
     >>> lot.unit = unit
     >>> lot.unit_quantity = 1
     >>> lot.save()
 
 Add a lot::
 
-    >>> add_lots = Wizard('stock.move.add.lots', [move])
+    >>> add_lots = move.click('add_lots_wizard')
     >>> lot = add_lots.form.lots.new()
     >>> lot.quantity
     5.0
     >>> lot.product = product  # proteus does not set reverse domain
     >>> lot.number = '01'
     >>> lot.unit == unit
     True
```

### Comparing `trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/PKG-INFO` & `trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-lot-unit
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to define unit on stock lot
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_lot_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock lot unit serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,28 +37,29 @@
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
 
 Stock Lot Unit Module
 #####################
 
-The `stock_lot_unit` module allows to define a unit and quantity on stock lot.
+The ``stock_lot_unit`` module allows to define a unit and quantity on stock
+lot.
 
 Lots with unit have the following properties:
 
     - no shipment may contain a summed quantity for a lot greater than the
       quantity of the lot.
     - no move related to a lot with a unit may concern a quantity greater than
       the quantity of the lot.
```

### Comparing `trytond_stock_lot_unit-6.6.0/trytond_stock_lot_unit.egg-info/SOURCES.txt` & `trytond_stock_lot_unit-6.8.0/trytond_stock_lot_unit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
 exceptions.py
@@ -53,14 +49,15 @@
 ./tests/scenario_stock_lot_unit.rst
 ./tests/scenario_stock_lot_unit_move_add.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/lot_form.xml
 ./view/lot_list.xml
 ./view/template_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

