# Comparing `tmp/trytond_product_cost_fifo-6.6.0.tar.gz` & `tmp/trytond_product_cost_fifo-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_fifo-6.6.0.tar", last modified: Mon Oct 31 15:56:01 2022, max compression
+gzip compressed data, was "trytond_product_cost_fifo-6.8.0.tar", last modified: Mon May  1 11:51:30 2023, max compression
```

## Comparing `trytond_product_cost_fifo-6.6.0.tar` & `trytond_product_cost_fifo-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_product_cost_fifo-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_product_cost_fifo-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-31 15:55:59.000000 trytond_product_cost_fifo-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_product_cost_fifo-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2316 2022-10-31 15:55:59.000000 trytond_product_cost_fifo-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:55:58.000000 trytond_product_cost_fifo-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:45.000000 trytond_product_cost_fifo-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_product_cost_fifo-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2774 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2018-08-18 09:54:45.000000 trytond_product_cost_fifo-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2021-12-11 16:59:33.000000 trytond_product_cost_fifo-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2018-08-18 09:54:45.000000 trytond_product_cost_fifo-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1125 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1427 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1480 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1492 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1214 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1513 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1478 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1184 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2022-10-29 07:50:39.000000 trytond_product_cost_fifo-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      827 2022-09-14 17:10:44.000000 trytond_product_cost_fifo-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6063 2022-09-14 17:10:44.000000 trytond_product_cost_fifo-6.6.0/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9599 2022-04-08 16:24:28.000000 trytond_product_cost_fifo-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5236 2022-10-29 07:39:11.000000 trytond_product_cost_fifo-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_product_cost_fifo-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4744 2020-07-09 09:37:09.000000 trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3178 2020-07-09 09:37:09.000000 trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_no_in.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4604 2022-10-11 19:45:04.000000 trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3145 2022-10-11 19:45:04.000000 trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4682 2020-07-09 09:37:09.000000 trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_uom.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2022-04-16 16:30:56.000000 trytond_product_cost_fifo-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_product_cost_fifo-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      712 2022-10-31 15:10:09.000000 trytond_product_cost_fifo-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 15:55:57.000000 trytond_product_cost_fifo-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:01.040347 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2774 2022-10-31 15:56:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1903 2022-10-31 15:56:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:56:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 15:56:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      105 2022-10-31 15:56:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:56:00.000000 trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:30.373120 trytond_product_cost_fifo-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2023-05-01 11:07:40.000000 trytond_product_cost_fifo-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:07:40.000000 trytond_product_cost_fifo-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2764 2023-05-01 11:51:30.373120 trytond_product_cost_fifo-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:30.369787 trytond_product_cost_fifo-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:30.366454 trytond_product_cost_fifo-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1125 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1427 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1480 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1538 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1492 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1513 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1478 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1184 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-04-29 08:02:45.000000 trytond_product_cost_fifo-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6429 2023-04-30 10:46:36.000000 trytond_product_cost_fifo-6.8.0/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9599 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:51:30.373120 trytond_product_cost_fifo-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4423 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:30.369787 trytond_product_cost_fifo-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4687 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3178 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_no_in.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4547 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3145 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4682 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_uom.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:07:35.000000 trytond_product_cost_fifo-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:30.373120 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2764 2023-05-01 11:51:29.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1877 2023-05-01 11:51:30.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:51:29.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:51:29.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      105 2023-05-01 11:51:29.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:51:29.000000 trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/top_level.txt
```

### Comparing `trytond_product_cost_fifo-6.6.0/CHANGELOG` & `trytond_product_cost_fifo-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

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

### Comparing `trytond_product_cost_fifo-6.6.0/COPYRIGHT` & `trytond_product_cost_fifo-6.8.0/COPYRIGHT`

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

### Comparing `trytond_product_cost_fifo-6.6.0/LICENSE` & `trytond_product_cost_fifo-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/PKG-INFO` & `trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_product_cost_fifo
-Version: 6.6.0
+Name: trytond-product-cost-fifo
+Version: 6.8.0
 Summary: Tryton module to add FIFO cost method
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_cost_fifo
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost fifo
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
 
 Product Cost FIFO Module
 ########################
 
 The Product Cost FIFO Module add a *FIFO* option in the Cost Method
```

### Comparing `trytond_product_cost_fifo-6.6.0/locale/bg.po` & `trytond_product_cost_fifo-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/ca.po` & `trytond_product_cost_fifo-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/cs.po` & `trytond_product_cost_fifo-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/de.po` & `trytond_product_cost_fifo-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/es.po` & `trytond_product_cost_fifo-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/es_419.po` & `trytond_product_cost_fifo-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/et.po` & `trytond_product_cost_fifo-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/fa.po` & `trytond_product_cost_fifo-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/fi.po` & `trytond_product_cost_fifo-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/fr.po` & `trytond_product_cost_fifo-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/hu.po` & `trytond_product_cost_fifo-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/id.po` & `trytond_product_cost_fifo-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/it.po` & `trytond_product_cost_fifo-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/lo.po` & `trytond_product_cost_fifo-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/lt.po` & `trytond_product_cost_fifo-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/nl.po` & `trytond_product_cost_fifo-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/pl.po` & `trytond_product_cost_fifo-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/pt.po` & `trytond_product_cost_fifo-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/ro.po` & `trytond_product_cost_fifo-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/ru.po` & `trytond_product_cost_fifo-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/sl.po` & `trytond_product_cost_fifo-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/tr.po` & `trytond_product_cost_fifo-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/uk.po` & `trytond_product_cost_fifo-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/locale/zh_CN.po` & `trytond_product_cost_fifo-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/message.xml` & `trytond_product_cost_fifo-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/move.py` & `trytond_product_cost_fifo-6.8.0/move.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,19 +25,28 @@
     @classmethod
     def __setup__(cls):
         super(Move, cls).__setup__()
         cls._allow_modify_closed_period.add('fifo_quantity')
 
         t = cls.__table__()
         cls._sql_constraints += [
-            ('check_fifo_quantity_out',
+            ('check_fifo_quantity',
                 Check(t, t.quantity >= t.fifo_quantity),
                 'product_cost_fifo.msg_move_fifo_quantity_greater'),
             ]
 
+    @classmethod
+    def __register__(cls, module):
+        table_h = cls.__table_handler__(module)
+        super().__register__(module)
+
+        # Migration from 6.6: rename check_fifo_quantity_out to
+        # check_fifo_quantity
+        table_h.drop_constraint('check_fifo_quantity_out')
+
     @staticmethod
     def default_fifo_quantity():
         return 0.0
 
     def get_fifo_quantity_available(self, name):
         return self.quantity - (self.fifo_quantity or 0)
 
@@ -58,15 +67,15 @@
         expression = field._domain_add_null(
             column, operator, value, expression)
         return expression
 
     def _update_fifo_out_product_cost_price(self):
         '''
         Update the product cost price of the given product on the move. Update
-        fifo_quantity on the concerned incomming moves. Return the
+        fifo_quantity on the concerned incoming moves. Return the
         cost price for outputing the given product and quantity.
         '''
         pool = Pool()
         Uom = pool.get('product.uom')
 
         total_qty = Uom.compute_qty(self.uom, self.quantity,
             self.product.default_uom, round=False)
@@ -103,25 +112,27 @@
             cost_price = round_price(cost_price)
         else:
             cost_price = average_cost_price
         return cost_price, average_cost_price, to_save
 
     def _do(self):
         cost_price, to_save = super(Move, self)._do()
+        cost_price_method = self.product.get_multivalue(
+            'cost_price_method', **self._cost_price_pattern)
         if (self.from_location.type != 'storage'
                 and self.to_location.type == 'storage'
-                and self.product.cost_price_method == 'fifo'):
+                and cost_price_method == 'fifo'):
             cost_price = self._compute_product_cost_price('in')
         elif (self.to_location.type == 'supplier'
                 and self.from_location.type == 'storage'
-                and self.product.cost_price_method == 'fifo'):
+                and cost_price_method == 'fifo'):
             cost_price = self._compute_product_cost_price('out')
         elif (self.from_location.type == 'storage'
                 and self.to_location.type != 'storage'
-                and self.product.cost_price_method == 'fifo'):
+                and cost_price_method == 'fifo'):
             fifo_cost_price, cost_price, moves = (
                 self._update_fifo_out_product_cost_price())
             if self.cost_price_required and self.cost_price is None:
                 self.cost_price = fifo_cost_price
             to_save.extend(moves)
         return cost_price, to_save
```

### Comparing `trytond_product_cost_fifo-6.6.0/product.py` & `trytond_product_cost_fifo-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/setup.py` & `trytond_product_cost_fifo-6.8.0/setup.py`

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_product_cost_fifo'
 
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
     description='Tryton module to add FIFO cost method',
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
-        "Source Code": 'https://hg.tryton.org/modules/product_cost_fifo',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product cost fifo',
     package_dir={'trytond.modules.product_cost_fifo': '.'},
     packages=(
         ['trytond.modules.product_cost_fifo']
         + ['trytond.modules.product_cost_fifo.%s' % p for p in find_packages()]
         ),
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
     product_cost_fifo = trytond.modules.product_cost_fifo
     """,
     )
```

### Comparing `trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo.rst` & `trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 =====================
 Stock FIFO Cost Price
 =====================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_no_in.rst` & `trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_no_in.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ===================================
 Stock FIFO Cost Price with no Input
 ===================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst` & `trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 ======================================
 Product Cost FIFO Recompute Cost Price
 ======================================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> today = dt.date.today()
```

### Comparing `trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst` & `trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-6.6.0/tests/scenario_product_cost_fifo_uom.rst` & `trytond_product_cost_fifo-6.8.0/tests/scenario_product_cost_fifo_uom.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 =========================
 Stock FIFO Cost Price UoM
 =========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/PKG-INFO` & `trytond_product_cost_fifo-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-product-cost-fifo
-Version: 6.6.0
+Name: trytond_product_cost_fifo
+Version: 6.8.0
 Summary: Tryton module to add FIFO cost method
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_cost_fifo
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost fifo
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
 
 Product Cost FIFO Module
 ########################
 
 The Product Cost FIFO Module add a *FIFO* option in the Cost Method
```

### Comparing `trytond_product_cost_fifo-6.6.0/trytond_product_cost_fifo.egg-info/SOURCES.txt` & `trytond_product_cost_fifo-6.8.0/trytond_product_cost_fifo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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
@@ -47,14 +43,15 @@
 ./tests/scenario_product_cost_fifo.rst
 ./tests/scenario_product_cost_fifo_no_in.rst
 ./tests/scenario_product_cost_fifo_recompute_cost_price.rst
 ./tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
 ./tests/scenario_product_cost_fifo_uom.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

