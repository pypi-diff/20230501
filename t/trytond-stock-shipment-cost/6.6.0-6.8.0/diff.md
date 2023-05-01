# Comparing `tmp/trytond_stock_shipment_cost-6.6.0.tar.gz` & `tmp/trytond_stock_shipment_cost-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_shipment_cost-6.6.0.tar", last modified: Mon Oct 31 15:58:11 2022, max compression
+gzip compressed data, was "trytond_stock_shipment_cost-6.8.0.tar", last modified: Mon May  1 11:34:48 2023, max compression
```

## Comparing `trytond_stock_shipment_cost-6.6.0.tar` & `trytond_stock_shipment_cost-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:11.358908 trytond_stock_shipment_cost-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_stock_shipment_cost-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-02-27 13:40:01.000000 trytond_stock_shipment_cost-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 15:58:10.000000 trytond_stock_shipment_cost-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_shipment_cost-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2022-10-31 15:58:09.000000 trytond_stock_shipment_cost-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 15:58:08.000000 trytond_stock_shipment_cost-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-02-27 13:40:01.000000 trytond_stock_shipment_cost-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_shipment_cost-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2536 2022-10-31 15:58:11.358908 trytond_stock_shipment_cost-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2021-05-19 10:44:55.000000 trytond_stock_shipment_cost-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      892 2022-09-01 20:26:56.000000 trytond_stock_shipment_cost-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2022-04-11 22:36:02.000000 trytond_stock_shipment_cost-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2022-04-11 22:36:02.000000 trytond_stock_shipment_cost-6.6.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:11.355575 trytond_stock_shipment_cost-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2021-05-19 10:44:55.000000 trytond_stock_shipment_cost-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:11.355575 trytond_stock_shipment_cost-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2374 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2478 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2439 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2418 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2386 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2022-10-29 07:50:31.000000 trytond_stock_shipment_cost-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:58:11.358908 trytond_stock_shipment_cost-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5399 2022-10-29 07:39:12.000000 trytond_stock_shipment_cost-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8472 2022-09-14 17:15:59.000000 trytond_stock_shipment_cost-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1023 2022-10-11 19:49:59.000000 trytond_stock_shipment_cost-6.6.0/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1057 2022-10-11 19:49:59.000000 trytond_stock_shipment_cost-6.6.0/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2021-02-27 13:40:01.000000 trytond_stock_shipment_cost-6.6.0/stock_reporting_margin.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:11.355575 trytond_stock_shipment_cost-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_shipment_cost-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4005 2022-09-01 20:26:56.000000 trytond_stock_shipment_cost-6.6.0/tests/scenario_stock_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2022-04-16 16:30:57.000000 trytond_stock_shipment_cost-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_shipment_cost-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-31 15:10:09.000000 trytond_stock_shipment_cost-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2022-10-31 15:58:08.000000 trytond_stock_shipment_cost-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:11.358908 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2536 2022-10-31 15:58:10.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1859 2022-10-31 15:58:11.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:58:10.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2022-10-31 15:58:10.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-02-27 13:40:01.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2022-10-31 15:58:10.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:58:10.000000 trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:11.355575 trytond_stock_shipment_cost-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-04-11 22:36:02.000000 trytond_stock_shipment_cost-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2021-02-27 13:40:01.000000 trytond_stock_shipment_cost-6.6.0/view/reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2022-09-01 20:26:56.000000 trytond_stock_shipment_cost-6.6.0/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2022-10-11 19:49:59.000000 trytond_stock_shipment_cost-6.6.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:34:48.970693 trytond_stock_shipment_cost-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-05-01 10:56:41.000000 trytond_stock_shipment_cost-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:56:40.000000 trytond_stock_shipment_cost-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2524 2023-05-01 11:34:48.970693 trytond_stock_shipment_cost-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:34:48.967360 trytond_stock_shipment_cost-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:34:48.964027 trytond_stock_shipment_cost-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2374 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2478 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2439 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2418 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2386 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-29 08:02:38.000000 trytond_stock_shipment_cost-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:34:48.970693 trytond_stock_shipment_cost-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4584 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8592 2023-04-21 08:36:08.000000 trytond_stock_shipment_cost-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1023 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1057 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/stock_reporting_margin.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:34:48.964027 trytond_stock_shipment_cost-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4006 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/tests/scenario_stock_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      139 2023-05-01 10:56:35.000000 trytond_stock_shipment_cost-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:34:48.970693 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2524 2023-05-01 11:34:48.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1833 2023-05-01 11:34:48.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:34:48.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 11:34:48.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2023-05-01 11:34:48.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:34:48.000000 trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:34:48.967360 trytond_stock_shipment_cost-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/view/reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost-6.8.0/view/stock_move_form.xml
```

### Comparing `trytond_stock_shipment_cost-6.6.0/COPYRIGHT` & `trytond_stock_shipment_cost-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2022 B2CK
-Copyright (C) 2020-2022 Cédric Krier
+Copyright (C) 2020-2023 B2CK
+Copyright (C) 2020-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_shipment_cost-6.6.0/LICENSE` & `trytond_stock_shipment_cost-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/PKG-INFO` & `trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_shipment_cost
-Version: 6.6.0
+Name: trytond-stock-shipment-cost
+Version: 6.8.0
 Summary: Tryton module for stock shipment cost
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-shipment-cost/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 ##########################
 Stock Shipment Cost Module
 ##########################
```

### Comparing `trytond_stock_shipment_cost-6.6.0/__init__.py` & `trytond_stock_shipment_cost-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/carrier.py` & `trytond_stock_shipment_cost-6.8.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/bg.po` & `trytond_stock_shipment_cost-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/ca.po` & `trytond_stock_shipment_cost-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/cs.po` & `trytond_stock_shipment_cost-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/de.po` & `trytond_stock_shipment_cost-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/es.po` & `trytond_stock_shipment_cost-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/es_419.po` & `trytond_stock_shipment_cost-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/et.po` & `trytond_stock_shipment_cost-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/fa.po` & `trytond_stock_shipment_cost-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/fi.po` & `trytond_stock_shipment_cost-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/fr.po` & `trytond_stock_shipment_cost-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/hu.po` & `trytond_stock_shipment_cost-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/id.po` & `trytond_stock_shipment_cost-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/it.po` & `trytond_stock_shipment_cost-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/lo.po` & `trytond_stock_shipment_cost-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/lt.po` & `trytond_stock_shipment_cost-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/nl.po` & `trytond_stock_shipment_cost-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/pl.po` & `trytond_stock_shipment_cost-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/pt.po` & `trytond_stock_shipment_cost-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/ro.po` & `trytond_stock_shipment_cost-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/ru.po` & `trytond_stock_shipment_cost-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/sl.po` & `trytond_stock_shipment_cost-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/tr.po` & `trytond_stock_shipment_cost-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/uk.po` & `trytond_stock_shipment_cost-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/locale/zh_CN.po` & `trytond_stock_shipment_cost-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/setup.py` & `trytond_stock_shipment_cost-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
 name = 'trytond_stock_shipment_cost'
 
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
     description='Tryton module for stock shipment cost',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-stock-shipment-cost/'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/stock_shipment_cost',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock shipment cost',
     package_dir={'trytond.modules.stock_shipment_cost': '.'},
     packages=(
         ['trytond.modules.stock_shipment_cost']
         + ['trytond.modules.stock_shipment_cost.%s' % p
             for p in find_packages()]
@@ -129,27 +107,26 @@
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
     stock_shipment_cost = trytond.modules.stock_shipment_cost
     """,  # noqa: E501
     )
```

### Comparing `trytond_stock_shipment_cost-6.6.0/stock.py` & `trytond_stock_shipment_cost-6.8.0/stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from decimal import Decimal
 
 from sql import Null
 
 from trytond.model import ModelView, Workflow, fields
 from trytond.modules.product import price_digits, round_price
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Eval, Bool
+from trytond.pyson import Bool, Eval
 from trytond.transaction import Transaction
 
 
 class Move(metaclass=PoolMeta):
     __name__ = 'stock.move'
 
     shipment_out_cost_price = fields.Numeric(
@@ -26,17 +26,23 @@
         super().__setup__()
         cls._allow_modify_closed_period.add('shipment_out_cost_price')
 
 
 class ShipmentCostMixin:
     __slots__ = ()
 
-    carrier = fields.Many2One('carrier', 'Carrier', states={
+    carrier = fields.Many2One(
+        'carrier', "Carrier",
+        states={
             'readonly': Eval('shipment_cost_readonly', True),
-            })
+            },
+        context={
+            'company': Eval('company', -1),
+            },
+        depends=['company'])
 
     cost_currency_used = fields.Function(fields.Many2One(
             'currency.currency', "Cost Currency",
             states={
                 'readonly': (
                     Eval('shipment_cost_readonly', True)
                     | ~Eval('cost_edit', False)),
@@ -94,15 +100,15 @@
         'cost_currency', 'cost_edit',
         methods=['_compute_costs', 'on_change_with_shipment_cost_readonly'])
     def on_change_with_cost_currency_used(self, name=None):
         readonly = self.on_change_with_shipment_cost_readonly()
         if not self.cost_edit and not readonly:
             return self._compute_costs()['cost_currency']
         elif self.cost_currency:
-            return self.cost_currency.id
+            return self.cost_currency
 
     @fields.depends(
         'cost', 'cost_edit',
         methods=['_compute_costs', 'on_change_with_shipment_cost_readonly'])
     def on_change_with_cost_used(self, name=None):
         cost = self.cost
         readonly = self.on_change_with_shipment_cost_readonly()
```

### Comparing `trytond_stock_shipment_cost-6.6.0/stock.xml` & `trytond_stock_shipment_cost-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/stock_reporting_margin.py` & `trytond_stock_shipment_cost-6.8.0/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/stock_reporting_margin.xml` & `trytond_stock_shipment_cost-6.8.0/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost-6.6.0/tests/scenario_stock_shipment_cost.rst` & `trytond_stock_shipment_cost-6.8.0/tests/scenario_stock_shipment_cost.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
     >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
+
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_shipment_cost')
```

### Comparing `trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/PKG-INFO` & `trytond_stock_shipment_cost-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-shipment-cost
-Version: 6.6.0
+Name: trytond_stock_shipment_cost
+Version: 6.8.0
 Summary: Tryton module for stock shipment cost
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-shipment-cost/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock shipment cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 ##########################
 Stock Shipment Cost Module
 ##########################
```

### Comparing `trytond_stock_shipment_cost-6.6.0/trytond_stock_shipment_cost.egg-info/SOURCES.txt` & `trytond_stock_shipment_cost-6.8.0/trytond_stock_shipment_cost.egg-info/SOURCES.txt`

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
 carrier.py
@@ -53,14 +49,15 @@
 ./tests/scenario_stock_shipment_cost.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/carrier_form.xml
 ./view/reporting_margin_context_form.xml
 ./view/shipment_out_form.xml
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

### Comparing `trytond_stock_shipment_cost-6.6.0/view/shipment_out_form.xml` & `trytond_stock_shipment_cost-6.8.0/view/shipment_out_form.xml`

 * *Files identical despite different names*

