# Comparing `tmp/trytond_account_stock_continental-6.6.0.tar.gz` & `tmp/trytond_account_stock_continental-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_continental-6.6.0.tar", last modified: Mon Oct 31 15:59:43 2022, max compression
+gzip compressed data, was "trytond_account_stock_continental-6.8.0.tar", last modified: Mon May  1 11:58:30 2023, max compression
```

## Comparing `trytond_account_stock_continental-6.6.0.tar` & `trytond_account_stock_continental-6.8.0.tar`

### file list

```diff
@@ -1,77 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:59:43.016908 trytond_account_stock_continental-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_stock_continental-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_stock_continental-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1128 2022-10-31 15:59:41.000000 trytond_account_stock_continental-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_stock_continental-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2418 2022-10-31 15:59:40.000000 trytond_account_stock_continental-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:59:40.000000 trytond_account_stock_continental-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:21.000000 trytond_account_stock_continental-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_stock_continental-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3453 2022-10-31 15:59:43.013574 trytond_account_stock_continental-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1105 2020-12-07 15:56:32.000000 trytond_account_stock_continental-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2021-12-11 16:59:32.000000 trytond_account_stock_continental-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2021-12-11 16:59:32.000000 trytond_account_stock_continental-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1254 2018-08-18 09:54:21.000000 trytond_account_stock_continental-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:59:43.010241 trytond_account_stock_continental-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1105 2020-12-07 15:56:32.000000 trytond_account_stock_continental-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:59:43.010241 trytond_account_stock_continental-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1321 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1654 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1626 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1653 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1462 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1659 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1571 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1550 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1572 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1328 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1351 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1556 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1308 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1335 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1525 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-29 07:50:42.000000 trytond_account_stock_continental-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4058 2020-01-08 13:36:55.000000 trytond_account_stock_continental-6.6.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2188 2020-09-19 09:14:11.000000 trytond_account_stock_continental-6.6.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2142 2020-09-19 09:14:16.000000 trytond_account_stock_continental-6.6.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2132 2020-09-19 09:14:21.000000 trytond_account_stock_continental-6.6.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2128 2020-09-19 09:14:26.000000 trytond_account_stock_continental-6.6.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2144 2020-09-19 09:14:31.000000 trytond_account_stock_continental-6.6.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2142 2020-09-19 09:14:36.000000 trytond_account_stock_continental-6.6.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2121 2020-09-19 09:14:42.000000 trytond_account_stock_continental-6.6.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2141 2020-09-19 09:14:48.000000 trytond_account_stock_continental-6.6.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2192 2020-09-19 09:14:55.000000 trytond_account_stock_continental-6.6.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2126 2020-09-19 09:15:02.000000 trytond_account_stock_continental-6.6.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9179 2022-09-01 20:04:04.000000 trytond_account_stock_continental-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2020-01-26 20:10:51.000000 trytond_account_stock_continental-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:59:43.016908 trytond_account_stock_continental-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5482 2022-10-29 07:39:10.000000 trytond_account_stock_continental-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6297 2022-04-27 15:54:20.000000 trytond_account_stock_continental-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:59:43.010241 trytond_account_stock_continental-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_stock_continental-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11993 2022-04-08 16:23:26.000000 trytond_account_stock_continental-6.6.0/tests/scenario_account_stock_continental.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-04-16 16:30:56.000000 trytond_account_stock_continental-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_account_stock_continental-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      748 2021-07-12 20:56:37.000000 trytond_account_stock_continental-6.6.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:10:09.000000 trytond_account_stock_continental-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2022-10-31 15:59:38.000000 trytond_account_stock_continental-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:59:43.013574 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3453 2022-10-31 15:59:42.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2245 2022-10-31 15:59:42.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:59:42.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2022-10-31 15:59:42.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:08.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2022-10-31 15:59:42.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:59:42.000000 trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:59:43.010241 trytond_account_stock_continental-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      581 2020-01-08 13:36:55.000000 trytond_account_stock_continental-6.6.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2020-01-08 13:36:55.000000 trytond_account_stock_continental-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2018-08-18 09:54:21.000000 trytond_account_stock_continental-6.6.0/view/fiscalyear_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:30.628336 trytond_account_stock_continental-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2581 2023-05-01 11:12:37.000000 trytond_account_stock_continental-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:12:37.000000 trytond_account_stock_continental-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_continental-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3434 2023-05-01 11:58:30.628336 trytond_account_stock_continental-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-30 10:46:36.000000 trytond_account_stock_continental-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1254 2023-01-16 14:00:20.000000 trytond_account_stock_continental-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:30.625002 trytond_account_stock_continental-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-30 10:46:36.000000 trytond_account_stock_continental-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:30.621669 trytond_account_stock_continental-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1321 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1654 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1626 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1653 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1462 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1659 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1571 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1572 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1328 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1351 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1556 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1308 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1335 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1525 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2023-04-29 08:02:48.000000 trytond_account_stock_continental-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4058 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2188 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2142 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2132 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2128 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2144 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2142 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2121 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2141 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2192 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2126 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9168 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:30.628336 trytond_account_stock_continental-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4646 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6424 2023-04-21 08:36:08.000000 trytond_account_stock_continental-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:30.625002 trytond_account_stock_continental-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11982 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/tests/scenario_account_stock_continental.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-05-01 11:12:31.000000 trytond_account_stock_continental-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:30.628336 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3434 2023-05-01 11:58:29.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2219 2023-05-01 11:58:30.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:29.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 11:58:29.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-05-01 11:58:29.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:29.000000 trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:30.625002 trytond_account_stock_continental-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_account_stock_continental-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:20.000000 trytond_account_stock_continental-6.8.0/view/fiscalyear_form.xml
```

### Comparing `trytond_account_stock_continental-6.6.0/CHANGELOG` & `trytond_account_stock_continental-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_account_stock_continental-6.6.0/COPYRIGHT` & `trytond_account_stock_continental-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2010-2022 Cédric Krier.
-Copyright (C) 2010-2022 B2CK SPRL.
+Copyright (C) 2010-2023 Cédric Krier.
+Copyright (C) 2010-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_stock_continental-6.6.0/LICENSE` & `trytond_account_stock_continental-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/PKG-INFO` & `trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_stock_continental
-Version: 6.6.0
+Name: trytond-account-stock-continental
+Version: 6.8.0
 Summary: Tryton module for continental real-time stock valuation
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_continental
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock valuation continental
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
 
 Account Stock Continental Module
 ################################
 
 The account_stock_continental module adds continental accounting model for
@@ -62,15 +62,15 @@
 A new configuration field for accounting is added:
 
 - Journal Stock: The journal used for stock move.
 
 Three new fields are added to Accounting categories:
 
 - Account Stock: The account which is used to record stock value.
-- Account Stock IN: The counter part account for incomming stock moves.
+- Account Stock IN: The counter part account for incoming stock moves.
 - Account Stock OUT: The counter part account for outgoing stock moves.
 
 An Account Move is created for each Stock Move done under a fiscal year with
 the account stock method set and for which one Stock Location has the type
 "Storage" and an the other has the type "Supplier", "Customer", "Production" or
 "Lost and Found".
```

### Comparing `trytond_account_stock_continental-6.6.0/README.rst` & `trytond_account_stock_continental-6.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 A new configuration field for accounting is added:
 
 - Journal Stock: The journal used for stock move.
 
 Three new fields are added to Accounting categories:
 
 - Account Stock: The account which is used to record stock value.
-- Account Stock IN: The counter part account for incomming stock moves.
+- Account Stock IN: The counter part account for incoming stock moves.
 - Account Stock OUT: The counter part account for outgoing stock moves.
 
 An Account Move is created for each Stock Move done under a fiscal year with
 the account stock method set and for which one Stock Location has the type
 "Storage" and an the other has the type "Supplier", "Customer", "Production" or
 "Lost and Found".
```

### Comparing `trytond_account_stock_continental-6.6.0/__init__.py` & `trytond_account_stock_continental-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/account.py` & `trytond_account_stock_continental-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/account.xml` & `trytond_account_stock_continental-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/doc/index.rst` & `trytond_account_stock_continental-6.8.0/doc/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 A new configuration field for accounting is added:
 
 - Journal Stock: The journal used for stock move.
 
 Three new fields are added to Accounting categories:
 
 - Account Stock: The account which is used to record stock value.
-- Account Stock IN: The counter part account for incomming stock moves.
+- Account Stock IN: The counter part account for incoming stock moves.
 - Account Stock OUT: The counter part account for outgoing stock moves.
 
 An Account Move is created for each Stock Move done under a fiscal year with
 the account stock method set and for which one Stock Location has the type
 "Storage" and an the other has the type "Supplier", "Customer", "Production" or
 "Lost and Found".
```

### Comparing `trytond_account_stock_continental-6.6.0/locale/bg.po` & `trytond_account_stock_continental-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/ca.po` & `trytond_account_stock_continental-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/cs.po` & `trytond_account_stock_continental-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/de.po` & `trytond_account_stock_continental-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/es.po` & `trytond_account_stock_continental-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/es_419.po` & `trytond_account_stock_continental-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/et.po` & `trytond_account_stock_continental-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/fa.po` & `trytond_account_stock_continental-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/fi.po` & `trytond_account_stock_continental-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/fr.po` & `trytond_account_stock_continental-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/hu.po` & `trytond_account_stock_continental-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/id.po` & `trytond_account_stock_continental-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/it.po` & `trytond_account_stock_continental-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/lo.po` & `trytond_account_stock_continental-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/lt.po` & `trytond_account_stock_continental-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/nl.po` & `trytond_account_stock_continental-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/pl.po` & `trytond_account_stock_continental-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/pt.po` & `trytond_account_stock_continental-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/ro.po` & `trytond_account_stock_continental-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/ru.po` & `trytond_account_stock_continental-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/sl.po` & `trytond_account_stock_continental-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/tr.po` & `trytond_account_stock_continental-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/uk.po` & `trytond_account_stock_continental-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/locale/zh_CN.po` & `trytond_account_stock_continental-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_bg.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_ca.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_de.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_en.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_es.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_fr.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_nl.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_pt.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_ru.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/minimal_chart_sl.xml` & `trytond_account_stock_continental-6.8.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-6.6.0/product.py` & `trytond_account_stock_continental-6.8.0/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         Period = pool.get('account.period')
 
         context = Transaction().context
         locations = Stock.search([('type', '=', 'storage')])
         company = Company(context['company'])
         with Transaction().set_context(company=company.id):
             stock_date_end = Date.today()
-        period = Period(Period.find(company.id, date=stock_date_end))
+        period = Period.find(company, date=stock_date_end)
         if period.fiscalyear.account_stock_method:
             moves = []
             with Transaction().set_context(locations=[l.id for l in locations],
                     stock_date_end=stock_date_end):
                 for cost, products in costs.items():
                     products = cls.browse(products)
                     for product in products:
```

### Comparing `trytond_account_stock_continental-6.6.0/setup.py` & `trytond_account_stock_continental-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
@@ -34,64 +31,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_stock_continental'
 
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
 for dep in ['sale', 'purchase', 'account_invoice',
         'sale_supply_drop_shipment']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for continental real-time stock valuation',
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
-            'https://hg.tryton.org/modules/account_stock_continental'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock valuation continental',
     package_dir={'trytond.modules.account_stock_continental': '.'},
     packages=(
         ['trytond.modules.account_stock_continental']
         + ['trytond.modules.account_stock_continental.%s' % p
             for p in find_packages()]
@@ -128,28 +105,27 @@
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
     account_stock_continental = trytond.modules.account_stock_continental
     """,
     )
```

### Comparing `trytond_account_stock_continental-6.6.0/stock.py` & `trytond_account_stock_continental-6.8.0/stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from decimal import Decimal
 
 from trytond.model import ModelView, Workflow
+from trytond.modules.account.exceptions import PeriodNotFoundError
 from trytond.pool import Pool, PoolMeta
 from trytond.transaction import Transaction
 
 
 class Move(metaclass=PoolMeta):
     __name__ = 'stock.move'
 
@@ -17,18 +18,20 @@
         pool = Pool()
         Uom = pool.get('product.uom')
         AccountMoveLine = pool.get('account.move.line')
         assert type_.startswith('in_') or type_.startswith('out_'), \
             'wrong type'
 
         move_line = AccountMoveLine()
+        cost_price_method = self.product.get_multivalue(
+            'cost_price_method', **self._cost_price_pattern)
         if ((
                     type_.endswith('supplier')
                     or type_ in {'in_production', 'in_warehouse'})
-                and self.product.cost_price_method != 'fixed'):
+                and cost_price_method != 'fixed'):
             unit_price = self.unit_price_company
         else:
             unit_price = self.cost_price
         unit_price = Uom.compute_price(self.product.default_uom,
             unit_price, self.uom)
         amount = self.company.currency.round(
                 Decimal(str(self.quantity)) * unit_price)
@@ -101,28 +104,28 @@
 
         if self.product.type != 'goods':
             return
 
         with Transaction().set_context(company=self.company.id):
             today = Date.today()
         for date in [self.effective_date, today]:
-            period_id = Period.find(
-                self.company.id, date=date, exception=False, test_state=False)
-            if not period_id and date < today:
-                return
-            elif period_id:
-                break
+            try:
+                period = Period.find(self.company, date=date, test_state=False)
+            except PeriodNotFoundError:
+                if date < today:
+                    return
+                continue
+            break
         else:
             return
-        period = Period(period_id)
         if not period.fiscalyear.account_stock_method:
             return
         if period.state != 'open':
             date = today
-            period = Period(Period.find(self.company.id, date=date))
+            period = Period.find(self.company, date=date)
 
         type_ = self._get_account_stock_move_type()
         if not type_:
             return
         with Transaction().set_context(
                 company=self.company.id, date=date):
             if type_ == 'supplier_customer':
@@ -149,15 +152,15 @@
             account_move_lines.append(move_line)
 
         account_configuration = AccountConfiguration(1)
         journal = account_configuration.get_multivalue(
             'stock_journal', company=self.company.id)
         return AccountMove(
             journal=journal,
-            period=period_id,
+            period=period,
             date=date,
             origin=self,
             lines=account_move_lines,
             )
 
     @classmethod
     @ModelView.button
```

### Comparing `trytond_account_stock_continental-6.6.0/tests/scenario_account_stock_continental.rst` & `trytond_account_stock_continental-6.8.0/tests/scenario_account_stock_continental.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 ==================================
 Account Stock Continental Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
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
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'account_stock_continental',
     ...         'sale',
     ...         'purchase',
@@ -32,15 +33,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.account_stock_method = 'continental'
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_stock_accounts(get_accounts(company), company)
@@ -82,15 +83,15 @@
     >>> template.name = 'product'
     >>> template.default_uom = cm
     >>> template.type = 'goods'
     >>> template.purchasable = True
     >>> template.salable = True
     >>> template.list_price = Decimal('10')
     >>> template.cost_price_method = 'fixed'
-    >>> template.lead_time = datetime.timedelta(0)
+    >>> template.lead_time = dt.timedelta(0)
     >>> template.account_category = account_category
     >>> product, = template.products
     >>> product.cost_price = Decimal('5')
     >>> template.save()
     >>> product, = template.products
     >>> template_average, = template.duplicate({
     ...         'cost_price_method': 'average',
@@ -201,15 +202,14 @@
     >>> sale.state
     'processing'
 
 Send 5 products::
 
     >>> shipment, = sale.shipments
     >>> shipment.click('assign_try')
-    True
     >>> shipment.state
     'assigned'
     >>> shipment.click('pick')
     >>> shipment.state
     'picked'
     >>> shipment.click('pack')
     >>> shipment.state
@@ -278,17 +278,17 @@
 Create Drop Shipment Move::
 
     >>> ProductSupplier = Model.get('purchase.product_supplier')
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = product.template
     >>> product_supplier.party = supplier
     >>> product_supplier.drop_shipment = True
-    >>> product_supplier.lead_time = datetime.timedelta(0)
+    >>> product_supplier.lead_time = dt.timedelta(0)
     >>> product_supplier.save()
-    >>> product.template.supply_on_sale = True
+    >>> product.template.supply_on_sale = 'always'
     >>> product.template.save()
 
     >>> sale = Sale()
     >>> sale.party = customer
     >>> sale.payment_term = payment_term
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
@@ -331,17 +331,17 @@
     >>> stock_out.credit
     Decimal('0.00')
 
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = product_average.template
     >>> product_supplier.party = supplier
     >>> product_supplier.drop_shipment = True
-    >>> product_supplier.lead_time = datetime.timedelta(0)
+    >>> product_supplier.lead_time = dt.timedelta(0)
     >>> product_supplier.save()
-    >>> product_average.template.supply_on_sale = True
+    >>> product_average.template.supply_on_sale = 'always'
     >>> product_average.template.save()
 
     >>> sale = Sale()
     >>> sale.party = customer
     >>> sale.payment_term = payment_term
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product_average
```

### Comparing `trytond_account_stock_continental-6.6.0/tests/tools.py` & `trytond_account_stock_continental-6.8.0/tests/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model
-
 from trytond.modules.company.tests.tools import get_company
 
 
 def add_stock_accounts(accounts, company=None, config=None):
     "Add stock kind to accounts"
     Account = Model.get('account.account', config=config)
```

### Comparing `trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/PKG-INFO` & `trytond_account_stock_continental-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-stock-continental
-Version: 6.6.0
+Name: trytond_account_stock_continental
+Version: 6.8.0
 Summary: Tryton module for continental real-time stock valuation
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_continental
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock valuation continental
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
 
 Account Stock Continental Module
 ################################
 
 The account_stock_continental module adds continental accounting model for
@@ -62,15 +62,15 @@
 A new configuration field for accounting is added:
 
 - Journal Stock: The journal used for stock move.
 
 Three new fields are added to Accounting categories:
 
 - Account Stock: The account which is used to record stock value.
-- Account Stock IN: The counter part account for incomming stock moves.
+- Account Stock IN: The counter part account for incoming stock moves.
 - Account Stock OUT: The counter part account for outgoing stock moves.
 
 An Account Move is created for each Stock Move done under a fiscal year with
 the account stock method set and for which one Stock Location has the type
 "Storage" and an the other has the type "Supplier", "Customer", "Production" or
 "Lost and Found".
```

### Comparing `trytond_account_stock_continental-6.6.0/trytond_account_stock_continental.egg-info/SOURCES.txt` & `trytond_account_stock_continental-6.8.0/trytond_account_stock_continental.egg-info/SOURCES.txt`

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
 account.py
@@ -72,14 +68,15 @@
 ./tests/scenario_account_stock_continental.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./tests/tools.py
 ./view/category_form.xml
 ./view/configuration_form.xml
 ./view/fiscalyear_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_stock_continental-6.6.0/view/category_form.xml` & `trytond_account_stock_continental-6.8.0/view/category_form.xml`

 * *Files identical despite different names*

