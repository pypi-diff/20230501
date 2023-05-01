# Comparing `tmp/trytond_purchase_shipment_cost-6.6.0.tar.gz` & `tmp/trytond_purchase_shipment_cost-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_shipment_cost-6.6.0.tar", last modified: Mon Oct 31 16:25:05 2022, max compression
+gzip compressed data, was "trytond_purchase_shipment_cost-6.8.0.tar", last modified: Mon May  1 11:58:11 2023, max compression
```

## Comparing `trytond_purchase_shipment_cost-6.6.0.tar` & `trytond_purchase_shipment_cost-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_purchase_shipment_cost-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_purchase_shipment_cost-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-31 16:25:03.000000 trytond_purchase_shipment_cost-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_purchase_shipment_cost-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2022-10-31 16:25:03.000000 trytond_purchase_shipment_cost-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2022-10-31 16:25:02.000000 trytond_purchase_shipment_cost-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:59.000000 trytond_purchase_shipment_cost-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_purchase_shipment_cost-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3201 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2018-08-18 09:54:59.000000 trytond_purchase_shipment_cost-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2021-12-11 16:59:33.000000 trytond_purchase_shipment_cost-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2020-03-01 11:49:48.000000 trytond_purchase_shipment_cost-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2018-08-18 09:54:59.000000 trytond_purchase_shipment_cost-6.6.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2018-08-18 09:54:59.000000 trytond_purchase_shipment_cost-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:05.242714 trytond_purchase_shipment_cost-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1462 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1223 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1226 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1190 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1259 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1263 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1079 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1126 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1142 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:42.000000 trytond_purchase_shipment_cost-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5659 2022-10-29 07:39:11.000000 trytond_purchase_shipment_cost-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7108 2022-10-11 19:49:58.000000 trytond_purchase_shipment_cost-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      773 2022-10-11 19:49:58.000000 trytond_purchase_shipment_cost-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_purchase_shipment_cost-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4623 2022-09-29 07:07:38.000000 trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4110 2021-04-27 22:35:16.000000 trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6817 2022-09-29 07:07:38.000000 trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6414 2021-03-24 12:34:59.000000 trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2022-04-16 16:30:57.000000 trytond_purchase_shipment_cost-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_purchase_shipment_cost-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_purchase_shipment_cost-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2022-10-31 16:25:01.000000 trytond_purchase_shipment_cost-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3201 2022-10-31 16:25:04.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2080 2022-10-31 16:25:05.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:25:04.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 16:25:04.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:08.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2022-10-31 16:25:04.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:25:04.000000 trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:05.246048 trytond_purchase_shipment_cost-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2018-08-18 09:54:59.000000 trytond_purchase_shipment_cost-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2022-09-12 22:47:25.000000 trytond_purchase_shipment_cost-6.6.0/view/shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2022-10-11 19:49:58.000000 trytond_purchase_shipment_cost-6.6.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:11.508098 trytond_purchase_shipment_cost-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2023-05-01 11:12:24.000000 trytond_purchase_shipment_cost-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-01 11:12:24.000000 trytond_purchase_shipment_cost-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2023-05-01 11:58:11.508098 trytond_purchase_shipment_cost-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:11.504765 trytond_purchase_shipment_cost-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:11.501432 trytond_purchase_shipment_cost-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1462 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1223 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1226 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1190 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1259 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1263 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1079 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1126 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1142 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:48.000000 trytond_purchase_shipment_cost-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:11.508098 trytond_purchase_shipment_cost-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4652 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7108 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      773 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:11.504765 trytond_purchase_shipment_cost-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4504 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4117 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6698 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6365 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-05-01 11:12:18.000000 trytond_purchase_shipment_cost-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:11.508098 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2023-05-01 11:58:10.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-05-01 11:58:11.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:10.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:58:10.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-05-01 11:58:10.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:10.000000 trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:11.504765 trytond_purchase_shipment_cost-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/view/shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-6.8.0/view/stock_move_form.xml
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/CHANGELOG` & `trytond_purchase_shipment_cost-6.8.0/CHANGELOG`

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
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/COPYRIGHT` & `trytond_purchase_shipment_cost-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2022 Cédric Krier.
+Copyright (C) 2011-2023 Cédric Krier.
 Copyright (C) 2011-2020 Bertrand Chenal.
-Copyright (C) 2011-2022 Nicolas Évrard.
-Copyright (C) 2011-2022 B2CK SPRL.
+Copyright (C) 2011-2023 Nicolas Évrard.
+Copyright (C) 2011-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/LICENSE` & `trytond_purchase_shipment_cost-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/PKG-INFO` & `trytond_purchase_shipment_cost-6.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_shipment_cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for purchase shipment cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,26 +39,21 @@
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
-Provides-Extra: account_invoice_stock
-Provides-Extra: account_product
-Provides-Extra: account_stock_continental
-Provides-Extra: account_stock_anglo_saxon
-Provides-Extra: product_kit
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Purchase Shipment Cost Module
 #############################
 
 The purchase_shipment_cost module adds shipment cost to *Supplier Shipment*.
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/README.rst` & `trytond_purchase_shipment_cost-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/carrier.py` & `trytond_purchase_shipment_cost-6.8.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/doc/index.rst` & `trytond_purchase_shipment_cost-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/bg.po` & `trytond_purchase_shipment_cost-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/ca.po` & `trytond_purchase_shipment_cost-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/cs.po` & `trytond_purchase_shipment_cost-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/de.po` & `trytond_purchase_shipment_cost-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/es.po` & `trytond_purchase_shipment_cost-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/es_419.po` & `trytond_purchase_shipment_cost-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/et.po` & `trytond_purchase_shipment_cost-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/fa.po` & `trytond_purchase_shipment_cost-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/fi.po` & `trytond_purchase_shipment_cost-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/fr.po` & `trytond_purchase_shipment_cost-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/hu.po` & `trytond_purchase_shipment_cost-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/id.po` & `trytond_purchase_shipment_cost-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/it.po` & `trytond_purchase_shipment_cost-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/lo.po` & `trytond_purchase_shipment_cost-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/lt.po` & `trytond_purchase_shipment_cost-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/nl.po` & `trytond_purchase_shipment_cost-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/pl.po` & `trytond_purchase_shipment_cost-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/pt.po` & `trytond_purchase_shipment_cost-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/ro.po` & `trytond_purchase_shipment_cost-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/ru.po` & `trytond_purchase_shipment_cost-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/sl.po` & `trytond_purchase_shipment_cost-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/tr.po` & `trytond_purchase_shipment_cost-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/uk.po` & `trytond_purchase_shipment_cost-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/locale/zh_CN.po` & `trytond_purchase_shipment_cost-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/setup.py` & `trytond_purchase_shipment_cost-6.8.0/setup.py`

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
@@ -34,70 +31,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_shipment_cost'
 
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
 
-extras_require = {}
-for dep in info.get('extras_depend', []):
-    if not re.match(r'(ir|res)(\W|$)', dep):
-        extras_require[dep] = get_require_version('trytond_%s' % dep)
-
 tests_require = [get_require_version('proteus'),
     get_require_version('trytond_account_invoice_stock'),
     get_require_version('trytond_account_stock_continental'),
     get_require_version('trytond_account_stock_anglo_saxon'),
     get_require_version('trytond_purchase')]
-extras_require['test'] = tests_require
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for purchase shipment cost',
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
-        "Source Code": 'https://hg.tryton.org/modules/purchase_shipment_cost',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase shipment cost',
     package_dir={'trytond.modules.purchase_shipment_cost': '.'},
     packages=(
         ['trytond.modules.purchase_shipment_cost']
         + ['trytond.modules.purchase_shipment_cost.%s' % p
             for p in find_packages()]
@@ -135,25 +107,26 @@
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
-    extras_require=extras_require,
-    dependency_links=dependency_links,
+    extras_require={
+        'test': tests_require,
+        },
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     purchase_shipment_cost = trytond.modules.purchase_shipment_cost
     """,
     )
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/stock.py` & `trytond_purchase_shipment_cost-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/stock.xml` & `trytond_purchase_shipment_cost-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost.rst` & `trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 ===============================
 Purchase Shipment Cost Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('purchase_shipment_cost')
 
 Create company::
 
@@ -110,15 +107,15 @@
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> [move.unit_price for move in shipment.incoming_moves] == \
-    ...     [Decimal('8.3333'), Decimal('8.3333'), Decimal('8.3334')]
+    ...     [Decimal('8.3334'), Decimal('8.3333'), Decimal('8.3333')]
     True
 
 Receive a two lines with no cost::
 
     >>> shipment = ShipmentIn()
     >>> shipment.supplier = supplier
     >>> move = shipment.incoming_moves.new()
@@ -138,8 +135,8 @@
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> tuple(m.unit_price for m in shipment.incoming_moves)
-    (Decimal('0.0600'), Decimal('0.0200'))
+    (Decimal('0.0200'), Decimal('0.0600'))
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst` & `trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create account categories::
 
     >>> account_category = ProductCategory(name="Account Category")
     >>> account_category.accounting = True
     >>> account_category.account_expense = accounts['expense']
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst` & `trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 ==================================================
 Purchase Shipment Cost with Account Stock Scenario
 ==================================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
     >>> from trytond.modules.account_stock_continental.tests.tools import \
     ...     add_stock_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_shipment_cost',
     ...         'account_stock_continental',
     ...         ])
@@ -181,15 +178,15 @@
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> [move.unit_price for move in shipment.incoming_moves] == \
-    ...     [Decimal('8.3333'), Decimal('8.3333'), Decimal('8.3334')]
+    ...     [Decimal('8.3334'), Decimal('8.3333'), Decimal('8.3333')]
     True
     >>> stock_in.reload()
     >>> (stock_in.debit, stock_in.credit) == \
     ...     (Decimal('0.00'), Decimal('467.20'))
     True
     >>> expense.reload()
     >>> (expense.debit, expense.credit) == \
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst` & `trytond_purchase_shipment_cost-6.8.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ==============================================================
 Purchase Shipment Cost with Account Stock Anglo-Saxon Scenario
 ==============================================================
 
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
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.account_stock_continental.tests.tools import \
     ...     add_stock_accounts
     >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import \
     ...     add_cogs_accounts
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_shipment_cost',
     ...         'account_stock_anglo_saxon',
     ...         'purchase',
@@ -33,15 +33,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.account_stock_method = 'anglo_saxon'
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_cogs_accounts(add_stock_accounts(
```

### Comparing `trytond_purchase_shipment_cost-6.6.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt` & `trytond_purchase_shipment_cost-6.8.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt`

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
 carrier.py
@@ -51,14 +47,15 @@
 ./tests/scenario_purchase_shipment_cost_with_account_stock.rst
 ./tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/carrier_form.xml
 ./view/shipment_in_form.xml
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

### Comparing `trytond_purchase_shipment_cost-6.6.0/view/shipment_in_form.xml` & `trytond_purchase_shipment_cost-6.8.0/view/shipment_in_form.xml`

 * *Files identical despite different names*

