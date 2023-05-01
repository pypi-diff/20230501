# Comparing `tmp/trytond_stock_lot-6.6.0.tar.gz` & `tmp/trytond_stock_lot-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot-6.6.0.tar", last modified: Mon Oct 31 16:24:06 2022, max compression
+gzip compressed data, was "trytond_stock_lot-6.8.0.tar", last modified: Mon May  1 11:42:36 2023, max compression
```

## Comparing `trytond_stock_lot-6.6.0.tar` & `trytond_stock_lot-6.8.0.tar`

### file list

```diff
@@ -1,82 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:24:06.795171 trytond_stock_lot-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_stock_lot-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_lot-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-31 16:24:05.000000 trytond_stock_lot-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_lot-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2407 2022-10-31 16:24:04.000000 trytond_stock_lot-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:24:04.000000 trytond_stock_lot-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_lot-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2508 2022-10-31 16:24:06.795171 trytond_stock_lot-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1255 2022-09-26 22:29:36.000000 trytond_stock_lot-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:24:06.791838 trytond_stock_lot-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      849 2021-03-24 12:34:22.000000 trytond_stock_lot-6.6.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:24:06.788504 trytond_stock_lot-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    11224 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11709 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10003 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12091 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11777 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9755 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10374 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12162 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9993 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11822 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10784 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9798 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10201 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10790 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10058 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11851 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10226 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11081 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9650 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11111 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10922 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9993 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9518 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10281 2022-10-29 07:50:34.000000 trytond_stock_lot-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2021-02-03 20:19:16.000000 trytond_stock_lot-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4379 2022-04-10 15:40:36.000000 trytond_stock_lot-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2021-02-03 20:19:16.000000 trytond_stock_lot-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:24:06.795171 trytond_stock_lot-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5138 2022-10-29 07:39:12.000000 trytond_stock_lot-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26825 2022-10-21 22:53:54.000000 trytond_stock_lot-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17895 2022-04-08 16:25:28.000000 trytond_stock_lot-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:24:06.791838 trytond_stock_lot-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_lot-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3556 2022-04-10 15:43:39.000000 trytond_stock_lot-6.6.0/tests/scenario_stock_lot_assign_try.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2641 2022-09-29 07:07:38.000000 trytond_stock_lot-6.6.0/tests/scenario_stock_lot_move_add.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2021-10-30 15:32:32.000000 trytond_stock_lot-6.6.0/tests/scenario_stock_lot_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3818 2020-10-12 20:56:13.000000 trytond_stock_lot-6.6.0/tests/scenario_stock_lot_shipment_out.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12527 2022-04-16 16:30:57.000000 trytond_stock_lot-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_lot-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      696 2022-10-31 15:10:09.000000 trytond_stock_lot-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      168 2022-10-31 16:24:03.000000 trytond_stock_lot-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:24:06.795171 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2508 2022-10-31 16:24:06.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2699 2022-10-31 16:24:06.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:24:06.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2022-10-31 16:24:06.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:52.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      121 2022-10-31 16:24:06.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:24:06.000000 trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:24:06.791838 trytond_stock_lot-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/view/inventory_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2019-10-11 21:50:16.000000 trytond_stock_lot-6.6.0/view/inventory_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/view/lot_by_location_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2020-10-11 14:05:26.000000 trytond_stock_lot-6.6.0/view/lot_by_warehouse_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-04-08 16:25:28.000000 trytond_stock_lot-6.6.0/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2022-04-08 16:25:28.000000 trytond_stock_lot-6.6.0/view/lot_trace_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2019-10-11 21:50:16.000000 trytond_stock_lot-6.6.0/view/lot_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2020-12-23 20:55:21.000000 trytond_stock_lot-6.6.0/view/lots_by_locations_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2022-10-11 19:49:58.000000 trytond_stock_lot-6.6.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2022-04-08 16:23:27.000000 trytond_stock_lot-6.6.0/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/view/period_cache_lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2019-02-13 10:05:00.000000 trytond_stock_lot-6.6.0/view/period_cache_lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2021-02-03 20:19:16.000000 trytond_stock_lot-6.6.0/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2021-02-03 20:19:16.000000 trytond_stock_lot-6.6.0/view/stock_move_add_lots_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2021-02-03 20:19:16.000000 trytond_stock_lot-6.6.0/view/stock_move_add_lots_start_lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2021-02-03 20:19:16.000000 trytond_stock_lot-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:36.959834 trytond_stock_lot-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2648 2023-05-01 11:01:52.000000 trytond_stock_lot-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:01:52.000000 trytond_stock_lot-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2506 2023-05-01 11:42:36.959834 trytond_stock_lot-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:36.953168 trytond_stock_lot-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      849 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:36.943168 trytond_stock_lot-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11320 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11796 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10098 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12181 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11865 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9838 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10473 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12269 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10089 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11909 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10880 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9881 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10298 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10886 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10152 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11923 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10322 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11177 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9733 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11207 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11018 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10089 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9601 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10379 2023-04-30 10:46:36.000000 trytond_stock_lot-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4666 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:36.959834 trytond_stock_lot-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4314 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27309 2023-04-21 08:36:08.000000 trytond_stock_lot-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19596 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:36.946501 trytond_stock_lot-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3491 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/scenario_stock_lot_assign_try.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/scenario_stock_lot_move_add.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1631 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/scenario_stock_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3762 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/scenario_stock_lot_shipment_out.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12470 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      168 2023-05-01 11:01:46.000000 trytond_stock_lot-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:36.956501 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2506 2023-05-01 11:42:36.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2673 2023-05-01 11:42:36.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:36.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-05-01 11:42:36.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      105 2023-05-01 11:42:36.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:36.000000 trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:36.953168 trytond_stock_lot-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/view/inventory_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/inventory_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/view/lot_by_location_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/lot_by_warehouse_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/lot_trace_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/lot_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/lots_by_locations_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/view/period_cache_lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:21.000000 trytond_stock_lot-6.8.0/view/period_cache_lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      718 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/stock_move_add_lots_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/stock_move_add_lots_start_lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-04-15 07:12:15.000000 trytond_stock_lot-6.8.0/view/template_form.xml
```

### Comparing `trytond_stock_lot-6.6.0/CHANGELOG` & `trytond_stock_lot-6.8.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Allow stock lot to be deactivated
+* Do not copy number of lot with sequence
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Synchronize lot on drop shipment
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_lot-6.6.0/COPYRIGHT` & `trytond_stock_lot-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2012-2022 Cédric Krier.
-Copyright (C) 2012-2022 B2CK SPRL.
+Copyright (C) 2012-2023 Cédric Krier.
+Copyright (C) 2012-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_lot-6.6.0/LICENSE` & `trytond_stock_lot-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-6.6.0/PKG-INFO` & `trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_lot
-Version: 6.6.0
+Name: trytond-stock-lot
+Version: 6.8.0
 Summary: Tryton module for lot of products
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_lot
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock lot
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
 
 Stock Lot Module
 ################
 
 The stock lot module defines lot of products.
```

### Comparing `trytond_stock_lot-6.6.0/__init__.py` & `trytond_stock_lot-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-6.6.0/ir.xml` & `trytond_stock_lot-6.8.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-6.6.0/locale/bg.po` & `trytond_stock_lot-6.8.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,19 @@
 msgstr "Планирано количество"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/ca.po` & `trytond_stock_lot-6.8.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "Locations Tree Quantity"
 msgstr "Quantitat per ubicacions"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr "Traçabilitat descendent"
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr "Traçabilitat ascendent"
```

### Comparing `trytond_stock_lot-6.6.0/locale/cs.po` & `trytond_stock_lot-6.8.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lot"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lot"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/de.po` & `trytond_stock_lot-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,18 @@
 msgid "Locations Tree Quantity"
 msgstr "Lagerbestand (Strukturansicht)"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Chargen"
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Chargen"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr "Retrograde Rückverfolgung"
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr "Progressive Rückverfolgung"
```

### Comparing `trytond_stock_lot-6.6.0/locale/es.po` & `trytond_stock_lot-6.8.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "Locations Tree Quantity"
 msgstr "Cantidad por ubicaciones"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lotes"
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lotes"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr "Trazabilidad descendente"
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr "Trazabilidad ascendente"
```

### Comparing `trytond_stock_lot-6.6.0/locale/es_419.po` & `trytond_stock_lot-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,18 @@
 msgid "Locations Tree Quantity"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/et.po` & `trytond_stock_lot-6.8.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,19 @@
 msgid "Locations Tree Quantity"
 msgstr "Prognoositav kogus"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Partiid"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Partiid"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/fa.po` & `trytond_stock_lot-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,19 @@
 msgid "Locations Tree Quantity"
 msgstr "مقدار پیش بینی شده"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "قطعه‌ها"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "قطعه‌ها"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/fi.po` & `trytond_stock_lot-6.8.0/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,19 @@
 msgid "Locations Tree Quantity"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/fr.po` & `trytond_stock_lot-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 msgid "Locations Tree Quantity"
 msgstr "Arbre des quantité par emplacements"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr "Traces descendantes"
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr "Traces ascendantes"
```

### Comparing `trytond_stock_lot-6.6.0/locale/hu.po` & `trytond_stock_lot-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,19 @@
 msgstr "Előrelátható mennyiség"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/id.po` & `trytond_stock_lot-6.8.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,18 @@
 msgid "Locations Tree Quantity"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/it.po` & `trytond_stock_lot-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,19 @@
 msgid "Locations Tree Quantity"
 msgstr "Quantità prevista"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lotti"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lotti"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/lo.po` & `trytond_stock_lot-6.8.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,19 @@
 msgid "Locations Tree Quantity"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/lt.po` & `trytond_stock_lot-6.8.0/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lo"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lo"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/nl.po` & `trytond_stock_lot-6.8.0/locale/nl.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.configuration,default_lot_sequence:"
 msgid "Default Lot Sequence"
-msgstr "Standaard batchvolgorde"
+msgstr "Standaard Batch Reeks"
 
 msgctxt ""
 "field:product.configuration.default_lot_sequence,default_lot_sequence:"
 msgid "Default Lot Sequence"
-msgstr "Standaard batchvolgorde"
+msgstr "Standaard Batch Reeks"
 
 msgctxt "field:product.product,lot_required:"
 msgid "Lot Required"
-msgstr "Batch vereist"
+msgstr "Batch Vereist"
 
 msgctxt "field:product.product,lot_sequence:"
 msgid "Lot Sequence"
-msgstr "Batch volgorde"
+msgstr "Batch Reeks"
 
 msgctxt "field:product.template,lot_required:"
 msgid "Lot Required"
-msgstr "Batch vereist"
+msgstr "Batch Vereist"
 
 msgctxt "field:product.template,lot_sequence:"
 msgid "Lot Sequence"
-msgstr "Batch volgorde"
+msgstr "Batch Reeks"
 
 msgctxt "field:stock.inventory.line,lot:"
 msgid "Lot"
 msgstr "Batch"
 
 msgctxt "field:stock.lot,default_uom:"
 msgid "Default UOM"
@@ -41,15 +41,15 @@
 
 msgctxt "field:stock.lot,forecast_quantity:"
 msgid "Forecast Quantity"
 msgstr "Verwachte hoeveelheid"
 
 msgctxt "field:stock.lot,has_sequence:"
 msgid "Has Sequence"
-msgstr "Heeft reeks"
+msgstr "Heeft Reeks"
 
 msgctxt "field:stock.lot,number:"
 msgid "Number"
 msgstr "Nummer"
 
 msgctxt "field:stock.lot,product:"
 msgid "Product"
@@ -225,23 +225,23 @@
 
 msgctxt "help:product.product,lot_required:"
 msgid "The type of location for which lot is required."
 msgstr "Het soort locatie waarvoor een batch vereist is."
 
 msgctxt "help:product.product,lot_sequence:"
 msgid "The sequence used to automatically number lots."
-msgstr "De volgorde die wordt gebruikt om batches automatisch te nummeren."
+msgstr "De reeks die wordt gebruikt om batches automatisch te nummeren."
 
 msgctxt "help:product.template,lot_required:"
 msgid "The type of location for which lot is required."
 msgstr "Het soort locatie waarvoor een batch vereist is."
 
 msgctxt "help:product.template,lot_sequence:"
 msgid "The sequence used to automatically number lots."
-msgstr "De volgorde die wordt gebruikt om batches automatisch te nummeren."
+msgstr "De reeks die wordt gebruikt om batches automatisch te nummeren."
 
 msgctxt "help:stock.lots_by_location.context,forecast_date:"
 msgid ""
 "Allow to compute expected stock quantities for this date.\n"
 "* An empty value is an infinite date in the future.\n"
 "* A date in the past will provide historical values."
 msgstr ""
@@ -271,14 +271,18 @@
 msgid "Locations Tree Quantity"
 msgstr "Boomstructuur met hoeveelheden per locatie"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Batches"
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Batches"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr "Neerwaartse tracering"
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr "Opwaartse tracering"
@@ -345,15 +349,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_lot_form"
 msgid "Lots"
 msgstr "Batches"
 
 msgctxt "model:product.configuration.default_lot_sequence,name:"
 msgid "Product Configuration Default Lot Sequence"
-msgstr "Productconfiguratie Standaard Batchvolgorde"
+msgstr "Productconfiguratie Standaard Batch Reeks"
 
 msgctxt "model:stock.lot,name:"
 msgid "Stock Lot"
 msgstr "Voorraad batch"
 
 msgctxt "model:stock.lot.trace,name:"
 msgid "Lot Trace"
```

### Comparing `trytond_stock_lot-6.6.0/locale/pl.po` & `trytond_stock_lot-6.8.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,19 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/pt.po` & `trytond_stock_lot-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,19 @@
 msgstr "Quantidade prevista"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/ro.po` & `trytond_stock_lot-6.8.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,18 @@
 msgid "Locations Tree Quantity"
 msgstr "Arbore Cantitate Locaţii"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/ru.po` & `trytond_stock_lot-6.8.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,19 @@
 msgid "Locations Tree Quantity"
 msgstr "Прогноз количества"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/sl.po` & `trytond_stock_lot-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,19 @@
 msgstr "Predvidena količina"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/tr.po` & `trytond_stock_lot-6.8.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,19 @@
 msgid "Locations Tree Quantity"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "Lots"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "Lots"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/uk.po` & `trytond_stock_lot-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,18 @@
 msgid "Locations Tree Quantity"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/locale/zh_CN.po` & `trytond_stock_lot-6.8.0/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,19 @@
 msgid "Locations Tree Quantity"
 msgstr "库位树数量"
 
 msgctxt "model:ir.action,name:act_lot_form"
 msgid "Lots"
 msgstr "批次"
 
+#, fuzzy
+msgctxt "model:ir.action,name:act_lot_form_product_relate"
+msgid "Lots"
+msgstr "批次"
+
 msgctxt "model:ir.action,name:act_lot_trace_downward_relate"
 msgid "Downward Traces"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_lot_trace_upward_relate"
 msgid "Upward Traces"
 msgstr ""
```

### Comparing `trytond_stock_lot-6.6.0/message.xml` & `trytond_stock_lot-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-6.6.0/product.py` & `trytond_stock_lot-6.8.0/product.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,7 +108,18 @@
 
 class Product(metaclass=PoolMeta):
     __name__ = 'product.product'
 
     def lot_is_required(self, from_, to):
         'Is product lot required for move with "from_" and "to" location ?'
         return any(l.type in (self.lot_required or []) for l in [from_, to])
+
+    def create_lot(self):
+        pool = Pool()
+        Lot = pool.get('stock.lot')
+        if self.lot_sequence:
+            lot = Lot(product=self)
+            try:
+                lot.on_change_product()
+            except AttributeError:
+                pass
+            return lot
```

### Comparing `trytond_stock_lot-6.6.0/product.xml` & `trytond_stock_lot-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-6.6.0/setup.py` & `trytond_stock_lot-6.8.0/setup.py`

 * *Files 15% similar despite different names*

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
 name = 'trytond_stock_lot'
 
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
 
-tests_require = [get_require_version('proteus'), 'python-dateutil']
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
+tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for lot of products',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_lot',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock lot',
     package_dir={'trytond.modules.stock_lot': '.'},
     packages=(
         ['trytond.modules.stock_lot']
         + ['trytond.modules.stock_lot.%s' % p for p in find_packages()]
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
     stock_lot = trytond.modules.stock_lot
     """,
     )
```

### Comparing `trytond_stock_lot-6.6.0/stock.py` & `trytond_stock_lot-6.8.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from copy import copy
 from functools import wraps
 
 from sql import Column
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
-from trytond.model import Index, Model, ModelSQL, ModelView, fields
+from trytond.model import (
+    DeactivableMixin, Index, Model, ModelSQL, ModelView, fields)
 from trytond.model.exceptions import (
     AccessError, RequiredValidationError, ValidationError)
 from trytond.modules.stock import StockMixin
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, Len
 from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
@@ -33,16 +34,15 @@
             if moves:
                 return True
         return False
 
     @wraps(func)
     def decorator(cls, *args):
         transaction = Transaction()
-        if (transaction.user != 0
-                and transaction.context.get('_check_access')):
+        if transaction.user and transaction.check_access:
             actions = iter(args)
             for records, values in zip(actions, actions):
                 for field, state, error in cls._modify_no_move:
                     if field in values:
                         if find_moves(cls, records, state):
                             raise AccessError(gettext(error))
                         # No moves for those records
@@ -69,15 +69,15 @@
 
     @fields.depends('product')
     def on_change_with_has_sequence(self, name=None):
         if self.product:
             return bool(self.product.lot_sequence)
 
 
-class Lot(ModelSQL, ModelView, LotMixin, StockMixin):
+class Lot(DeactivableMixin, ModelSQL, ModelView, LotMixin, StockMixin):
     "Stock Lot"
     __name__ = 'stock.lot'
     _rec_name = 'number'
 
     quantity = fields.Function(fields.Float('Quantity'), 'get_quantity',
         searcher='search_quantity')
     forecast_quantity = fields.Function(fields.Float('Forecast Quantity'),
@@ -119,23 +119,30 @@
     def search_quantity(cls, name, domain=None):
         location_ids = Transaction().context.get('locations')
         return cls._search_quantity(name, location_ids, domain,
             grouping=('product', 'lot'))
 
     @fields.depends('product')
     def on_change_with_default_uom(self, name=None):
-        if self.product:
-            return self.product.default_uom.id
+        return self.product.default_uom if self.product else None
 
     @fields.depends('product')
     def on_change_with_default_uom_digits(self, name=None):
         if self.product:
             return self.product.default_uom.digits
 
     @classmethod
+    def copy(cls, lots, default=None):
+        default = default.copy() if default else {}
+        has_sequence = {l.id: l.has_sequence for l in lots}
+        default.setdefault(
+            'number', lambda o: None if has_sequence[o['id']] else o['number'])
+        return super().copy(lots, default=default)
+
+    @classmethod
     def create(cls, vlist):
         vlist = [v.copy() for v in vlist]
         for values in vlist:
             if not values.get('number'):
                 values['number'] = cls._new_number(values)
         return super().create(vlist)
 
@@ -369,15 +376,15 @@
     def default_warehouse(cls):
         return Pool().get('stock.location').get_default_warehouse()
 
     @fields.depends('warehouse')
     def on_change_with_locations(self, name=None):
         locations = []
         if self.warehouse:
-            locations.append(self.warehouse.id)
+            locations.append(self.warehouse)
         return locations
 
 
 class Location(metaclass=PoolMeta):
     __name__ = 'stock.location'
 
     @classmethod
@@ -420,14 +427,20 @@
                 })
 
     @classmethod
     @ModelView.button_action('stock_lot.wizard_move_add_lots')
     def add_lots_wizard(cls, moves):
         pass
 
+    def add_lot(self):
+        if not self.lot and self.product:
+            lot = self.product.create_lot()
+            if lot:
+                self.lot = lot
+
     def check_lot(self):
         "Check if lot is required"
         if (self.state == 'done'
                 and self.internal_quantity
                 and not self.lot
                 and self.product.lot_is_required(
                     self.from_location, self.to_location)):
```

### Comparing `trytond_stock_lot-6.6.0/stock.xml` & `trytond_stock_lot-6.8.0/stock.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_stock_lot-6.6.0/stock.xml` & `trytond_stock_lot-6.8.0/stock.xml`

```diff
@@ -24,14 +24,39 @@
     </record>
     <record model="ir.action.act_window.view" id="act_lot_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="lot_view_form"/>
       <field name="act_window" ref="act_lot_form"/>
     </record>
     <menuitem parent="stock.menu_stock" action="act_lot_form" sequence="50" id="menu_lot_form"/>
+    <record model="ir.action.act_window" id="act_lot_form_product_relate">
+      <field name="name">Lots</field>
+      <field name="res_model">stock.lot</field>
+      <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], (If(Eval('active_model') == 'product.template', 'product.template', 'product'), '=', Eval('active_id', -1)), (If(Eval('active_model') == 'product.template', 'product.template', 'product'), 'in', Eval('active_ids', [])))]" pyson="1"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_lot_form_product_relate_view1">
+      <field name="sequence" eval="10"/>
+      <field name="view" ref="lot_view_tree"/>
+      <field name="act_window" ref="act_lot_form_product_relate"/>
+    </record>
+    <record model="ir.action.act_window.view" id="act_lot_form_product_relate_view2">
+      <field name="sequence" eval="20"/>
+      <field name="view" ref="lot_view_form"/>
+      <field name="act_window" ref="act_lot_form_product_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_lot_form_product_relate_keyword1">
+      <field name="keyword">form_relate</field>
+      <field name="model">product.product,-1</field>
+      <field name="action" ref="act_lot_form_product_relate"/>
+    </record>
+    <record model="ir.action.keyword" id="act_lot_form_product_relate_keyword2">
+      <field name="keyword">form_relate</field>
+      <field name="model">product.template,-1</field>
+      <field name="action" ref="act_lot_form_product_relate"/>
+    </record>
     <record model="ir.model.access" id="access_lot">
       <field name="model" search="[('model', '=', 'stock.lot')]"/>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
```

### Comparing `trytond_stock_lot-6.6.0/tests/scenario_stock_lot_assign_try.rst` & `trytond_stock_lot-6.8.0/tests/scenario_stock_lot_assign_try.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =================================
 Stock Lot Assign Request Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import config, Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot')
     >>> Inventory = Model.get('stock.inventory')
     >>> Location = Model.get('stock.location')
     >>> Lot = Model.get('stock.lot')
@@ -111,13 +111,12 @@
     >>> move, = shipment.inventory_moves
     >>> move.lot = lot
     >>> move.save()
 
 Assign the shipment::
 
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> move, = shipment.inventory_moves
     >>> move.from_location.name
     'Zone2'
```

### Comparing `trytond_stock_lot-6.6.0/tests/scenario_stock_lot_move_add.rst` & `trytond_stock_lot-6.8.0/tests/scenario_stock_lot_move_add.rst`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     >>> Lot = Model.get('stock.lot')
     >>> lot2 = Lot(number='02', product=product)
     >>> lot2.save()
 
 Add few lots::
 
-    >>> add_lots = Wizard('stock.move.add.lots', [move])
+    >>> add_lots = move.click('add_lots_wizard')
     >>> add_lots.form.product== product
     True
     >>> add_lots.form.quantity
     10.0
     >>> add_lots.form.unit == unit
     True
     >>> add_lots.form.quantity_remaining
@@ -94,15 +94,15 @@
     True
     >>> move, = Move.find([('lot', '=', None)])
     >>> move.quantity
     7.0
 
 Add lot to remaining::
 
-    >>> add_lots = Wizard('stock.move.add.lots', [move])
+    >>> add_lots = move.click('add_lots_wizard')
     >>> lot = add_lots.form.lots.new()
     >>> lot.number = '03'
     >>> add_lots.execute('add')
 
     >>> len(Move.find([]))
     3
     >>> move.lot.number
```

### Comparing `trytond_stock_lot-6.6.0/tests/scenario_stock_lot_number.rst` & `trytond_stock_lot-6.8.0/tests/scenario_stock_lot_number.rst`

 * *Files 9% similar despite different names*

```diff
@@ -47,7 +47,21 @@
 
     >>> Lot = Model.get('stock.lot')
     >>> lot = Lot(product=product)
     >>> lot.save()
 
     >>> lot.number
     '1'
+
+Copy set a new number::
+
+    >>> lot2, = lot.duplicate()
+    >>> lot2.number
+    '2'
+
+Copy without sequence keep same number::
+
+    >>> template.lot_sequence = None
+    >>> template.save()
+    >>> lot3, = lot.duplicate()
+    >>> lot3.number
+    '1'
```

### Comparing `trytond_stock_lot-6.6.0/tests/scenario_stock_lot_shipment_out.rst` & `trytond_stock_lot-6.8.0/tests/scenario_stock_lot_shipment_out.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ===============================
 Stock Lot Shipment Out Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import config, Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot')
 
 Create company::
 
@@ -123,8 +123,8 @@
     [0.0, 3.0, 7.0]
     >>> lot_quantities = {}
     >>> for move in shipment_out.outgoing_moves:
     ...     number = move.lot.number if move.lot else ''
     ...     quantity = lot_quantities.setdefault(number, 0)
     ...     lot_quantities[number] += move.quantity
     >>> sorted(lot_quantities.items())
-    [('', 0.0), ('00001', 3.0), ('00002', 7.0)]
+    [('', 0.0), ('00001', 7.0), ('00002', 3.0)]
```

### Comparing `trytond_stock_lot-6.6.0/tests/test_module.py` & `trytond_stock_lot-6.8.0/tests/test_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-import datetime
+import datetime as dt
 from decimal import Decimal
 
-from dateutil.relativedelta import relativedelta
-
 from trytond.modules.company.tests import (
     CompanyTestMixin, create_company, set_company)
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 from trytond.transaction import Transaction
 
 
@@ -141,57 +139,57 @@
                         'number': '1',
                         'product': product.id,
                         }, {
                         'number': '2',
                         'product': product.id,
                         }])
 
-            today = datetime.date.today()
+            today = dt.date.today()
 
             moves = Move.create([{
                         'product': product.id,
                         'lot': lot1.id,
                         'uom': unit.id,
                         'quantity': 5,
                         'from_location': supplier.id,
                         'to_location': storage.id,
-                        'planned_date': today - relativedelta(days=1),
-                        'effective_date': today - relativedelta(days=1),
+                        'planned_date': today - dt.timedelta(days=1),
+                        'effective_date': today - dt.timedelta(days=1),
                         'company': company.id,
                         'unit_price': Decimal('1'),
                         'currency': currency.id,
                         }, {
                         'product': product.id,
                         'lot': lot2.id,
                         'uom': unit.id,
                         'quantity': 10,
                         'from_location': supplier.id,
                         'to_location': storage.id,
-                        'planned_date': today - relativedelta(days=1),
-                        'effective_date': today - relativedelta(days=1),
+                        'planned_date': today - dt.timedelta(days=1),
+                        'effective_date': today - dt.timedelta(days=1),
                         'company': company.id,
                         'unit_price': Decimal('1'),
                         'currency': currency.id,
                         }, {
                         'product': product.id,
                         'lot': None,
                         'uom': unit.id,
                         'quantity': 3,
                         'from_location': supplier.id,
                         'to_location': storage.id,
-                        'planned_date': today - relativedelta(days=1),
-                        'effective_date': today - relativedelta(days=1),
+                        'planned_date': today - dt.timedelta(days=1),
+                        'effective_date': today - dt.timedelta(days=1),
                         'company': company.id,
                         'unit_price': Decimal('1'),
                         'currency': currency.id,
                         }])
             Move.do(moves)
 
             period, = Period.create([{
-                        'date': today - relativedelta(days=1),
+                        'date': today - dt.timedelta(days=1),
                         'company': company.id,
                         }])
             Period.close([period])
             self.assertEqual(period.state, 'closed')
 
             quantities = {
                 supplier: -18,
```

### Comparing `trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/PKG-INFO` & `trytond_stock_lot-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-lot
-Version: 6.6.0
+Name: trytond_stock_lot
+Version: 6.8.0
 Summary: Tryton module for lot of products
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_lot
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock lot
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
 
 Stock Lot Module
 ################
 
 The stock lot module defines lot of products.
```

### Comparing `trytond_stock_lot-6.6.0/trytond_stock_lot.egg-info/SOURCES.txt` & `trytond_stock_lot-6.8.0/trytond_stock_lot.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

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
 ir.xml
@@ -68,14 +64,15 @@
 ./view/move_tree.xml
 ./view/period_cache_lot_form.xml
 ./view/period_cache_lot_list.xml
 ./view/product_configuration_form.xml
 ./view/stock_move_add_lots_start_form.xml
 ./view/stock_move_add_lots_start_lot_list.xml
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

### Comparing `trytond_stock_lot-6.6.0/view/stock_move_add_lots_start_form.xml` & `trytond_stock_lot-6.8.0/view/stock_move_add_lots_start_form.xml`

 * *Files identical despite different names*

