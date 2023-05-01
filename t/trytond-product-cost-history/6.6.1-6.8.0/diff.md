# Comparing `tmp/trytond_product_cost_history-6.6.1.tar.gz` & `tmp/trytond_product_cost_history-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_history-6.6.1.tar", last modified: Sat Mar  4 11:56:26 2023, max compression
+gzip compressed data, was "trytond_product_cost_history-6.8.0.tar", last modified: Mon May  1 11:47:15 2023, max compression
```

## Comparing `trytond_product_cost_history-6.6.1.tar` & `trytond_product_cost_history-6.8.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:56:26.749544 trytond_product_cost_history-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2412 2023-03-04 11:56:22.000000 trytond_product_cost_history-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-03-04 11:56:21.000000 trytond_product_cost_history-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_product_cost_history-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2712 2023-03-04 11:56:26.749544 trytond_product_cost_history-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:56:26.746211 trytond_product_cost_history-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:56:26.739544 trytond_product_cost_history-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      633 2022-12-19 12:02:49.000000 trytond_product_cost_history-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:49.000000 trytond_product_cost_history-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      591 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      546 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2022-12-19 12:02:49.000000 trytond_product_cost_history-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      592 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2022-12-19 12:02:49.000000 trytond_product_cost_history-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2022-12-19 12:02:49.000000 trytond_product_cost_history-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      574 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      588 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      574 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6990 2023-02-23 20:30:05.000000 trytond_product_cost_history-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2100 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:56:26.749544 trytond_product_cost_history-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4461 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:56:26.742877 trytond_product_cost_history-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5074 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/tests/scenario_product_cost_history.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-12-19 12:03:07.000000 trytond_product_cost_history-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:56:26.749544 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2712 2023-03-04 11:56:25.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1602 2023-03-04 11:56:26.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:56:25.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-03-04 11:56:25.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:56:25.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      105 2023-03-04 11:56:25.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:56:25.000000 trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:56:26.742877 trytond_product_cost_history-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/view/product_cost_history_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2022-12-19 12:02:50.000000 trytond_product_cost_history-6.6.1/view/product_cost_history_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:15.819962 trytond_product_cost_history-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-05-01 11:04:54.000000 trytond_product_cost_history-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:04:54.000000 trytond_product_cost_history-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_history-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2699 2023-05-01 11:47:15.819962 trytond_product_cost_history-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:15.819962 trytond_product_cost_history-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:15.816628 trytond_product_cost_history-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      633 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      591 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      546 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      592 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-04-29 08:02:44.000000 trytond_product_cost_history-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6698 2023-04-21 08:36:08.000000 trytond_product_cost_history-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2100 2023-01-16 14:00:20.000000 trytond_product_cost_history-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:15.819962 trytond_product_cost_history-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4420 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:15.816628 trytond_product_cost_history-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5152 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/tests/scenario_product_cost_history.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:04:48.000000 trytond_product_cost_history-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:15.819962 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2699 2023-05-01 11:47:14.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1602 2023-05-01 11:47:15.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:14.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:47:14.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      105 2023-05-01 11:47:14.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:14.000000 trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:15.816628 trytond_product_cost_history-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-01-16 14:00:20.000000 trytond_product_cost_history-6.8.0/view/product_cost_history_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-04-15 07:12:15.000000 trytond_product_cost_history-6.8.0/view/product_cost_history_tree.xml
```

### Comparing `trytond_product_cost_history-6.6.1/CHANGELOG` & `trytond_product_cost_history-6.8.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_product_cost_history-6.6.1/COPYRIGHT` & `trytond_product_cost_history-6.8.0/COPYRIGHT`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2022 Cédric Krier.
+Copyright (C) 2009-2023 Cédric Krier.
 Copyright (C) 2009-2012 Bertrand Chenal.
-Copyright (C) 2009-2022 B2CK SPRL.
+Copyright (C) 2009-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_cost_history-6.6.1/LICENSE` & `trytond_product_cost_history-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/PKG-INFO` & `trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_product_cost_history
-Version: 6.6.1
+Name: trytond-product-cost-history
+Version: 6.8.0
 Summary: Tryton module to historize product cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_cost_history
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost history
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
 
 Product Cost History Module
 ###########################
 
 The Product Cost History Module adds a *Cost History* relate on the product
```

### Comparing `trytond_product_cost_history-6.6.1/doc/conf.py` & `trytond_product_cost_history-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
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
```

### Comparing `trytond_product_cost_history-6.6.1/locale/bg.po` & `trytond_product_cost_history-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/ca.po` & `trytond_product_cost_history-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/cs.po` & `trytond_product_cost_history-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/de.po` & `trytond_product_cost_history-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/es.po` & `trytond_product_cost_history-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/es_419.po` & `trytond_product_cost_history-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/et.po` & `trytond_product_cost_history-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/fa.po` & `trytond_product_cost_history-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/fi.po` & `trytond_product_cost_history-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/fr.po` & `trytond_product_cost_history-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/hu.po` & `trytond_product_cost_history-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/id.po` & `trytond_product_cost_history-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/it.po` & `trytond_product_cost_history-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/lo.po` & `trytond_product_cost_history-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/lt.po` & `trytond_product_cost_history-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/nl.po` & `trytond_product_cost_history-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/pl.po` & `trytond_product_cost_history-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/pt.po` & `trytond_product_cost_history-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/ro.po` & `trytond_product_cost_history-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/ru.po` & `trytond_product_cost_history-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/sl.po` & `trytond_product_cost_history-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/tr.po` & `trytond_product_cost_history-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/locale/zh_CN.po` & `trytond_product_cost_history-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/product.py` & `trytond_product_cost_history-6.8.0/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,21 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from sql import Column, Literal, Window
 from sql.aggregate import Max
 from sql.conditionals import Coalesce
 from sql.functions import CurrentTimestamp, LastValue
 
-from trytond.model import ModelSQL, ModelView, fields
+from trytond.model import ModelSQL, ModelView, convert_from, fields
 from trytond.modules.product import round_price
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import timezone as tz
 from trytond.transaction import Transaction
 
 
-def convert_from(table, tables):
-    right, condition = tables[None]
-    if table:
-        table = table.join(right, condition=condition)
-    else:
-        table = right
-    for k, sub_tables in tables.items():
-        if k is None:
-            continue
-        table = convert_from(table, sub_tables)
-    return table
-
-
 class Product(metaclass=PoolMeta):
     __name__ = 'product.product'
 
     def get_multivalue(self, name, **pattern):
         pool = Pool()
         Company = pool.get('company.company')
         context = Transaction().context
@@ -117,15 +104,15 @@
                 [move.effective_date, move.product],
                 frame='ROWS', start=None, end=None,
                 order_by=[move.write_date.asc, move.id.asc])
             cost_price = LastValue(move.cost_price, window=window)
         else:
             cost_price = cls.cost_price.sql_cast(move.cost_price)
 
-        move_history = convert_from(None, tables).select(
+        move_history = convert_from(None, tables, type_='INNER').select(
             (move.id * 2).as_('id'),
             move.effective_date.as_('date'),
             move.product.as_('product'),
             cost_price.as_('cost_price'),
             where=clause)
         query = move_history.select(
             Max(move_history.id).as_('id'),
```

### Comparing `trytond_product_cost_history-6.6.1/product.xml` & `trytond_product_cost_history-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-6.6.1/setup.py` & `trytond_product_cost_history-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -34,38 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_product_cost_history'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module to historize product cost',
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
-        "Source Code": 'https://hg.tryton.org/modules/product_cost_history',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product cost history',
     package_dir={'trytond.modules.product_cost_history': '.'},
     packages=(
         ['trytond.modules.product_cost_history']
         + ['trytond.modules.product_cost_history.%s' % p
             for p in find_packages()]
@@ -103,23 +103,23 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_product_cost_history-6.6.1/tests/scenario_product_cost_history.rst` & `trytond_product_cost_history-6.8.0/tests/scenario_product_cost_history.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 Product Cost History
 ====================
 
 Imports::
 
     >>> import datetime as dt
     >>> import time
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = dt.date.today()
-    >>> now = dt.datetime.now()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_history')
 
+    >>> Date = Model.get('ir.date')
+
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
+    >>> company.timezone = 'Europe/Madrid'
+    >>> company.save()
+
+    >>> today = Date.today(config.context)
+    >>> now = dt.datetime.combine(today, dt.time())
 
 Create product::
 
     >>> ProductUom = Model.get('product.uom')
     >>> ProductTemplate = Model.get('product.template')
     >>> Product = Model.get('product.product')
     >>> unit, = ProductUom.find([('name', '=', 'Unit')])
```

### Comparing `trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/PKG-INFO` & `trytond_product_cost_history-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-product-cost-history
-Version: 6.6.1
+Name: trytond_product_cost_history
+Version: 6.8.0
 Summary: Tryton module to historize product cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_cost_history
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost history
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
 
 Product Cost History Module
 ###########################
 
 The Product Cost History Module adds a *Cost History* relate on the product
```

### Comparing `trytond_product_cost_history-6.6.1/trytond_product_cost_history.egg-info/SOURCES.txt` & `trytond_product_cost_history-6.8.0/trytond_product_cost_history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

