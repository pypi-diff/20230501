# Comparing `tmp/trytond_account_stock_anglo_saxon-6.6.0.tar.gz` & `tmp/trytond_account_stock_anglo_saxon-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_anglo_saxon-6.6.0.tar", last modified: Mon Oct 31 16:06:33 2022, max compression
+gzip compressed data, was "trytond_account_stock_anglo_saxon-6.8.0.tar", last modified: Mon May  1 11:50:12 2023, max compression
```

## Comparing `trytond_account_stock_anglo_saxon-6.6.0.tar` & `trytond_account_stock_anglo_saxon-6.8.0.tar`

### file list

```diff
@@ -1,78 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:33.119537 trytond_account_stock_anglo_saxon-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_stock_anglo_saxon-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_stock_anglo_saxon-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2022-10-31 16:06:31.000000 trytond_account_stock_anglo_saxon-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_stock_anglo_saxon-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2259 2022-10-31 16:06:30.000000 trytond_account_stock_anglo_saxon-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:06:30.000000 trytond_account_stock_anglo_saxon-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:20.000000 trytond_account_stock_anglo_saxon-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_stock_anglo_saxon-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3253 2022-10-31 16:06:33.119537 trytond_account_stock_anglo_saxon-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2020-12-07 15:56:31.000000 trytond_account_stock_anglo_saxon-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2021-12-11 16:59:32.000000 trytond_account_stock_anglo_saxon-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2020-03-01 11:49:44.000000 trytond_account_stock_anglo_saxon-6.6.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:33.116204 trytond_account_stock_anglo_saxon-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2020-12-07 15:56:31.000000 trytond_account_stock_anglo_saxon-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2019-06-04 16:49:44.000000 trytond_account_stock_anglo_saxon-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4294 2021-12-11 16:59:32.000000 trytond_account_stock_anglo_saxon-6.6.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:33.116204 trytond_account_stock_anglo_saxon-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1337 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1275 2022-10-29 07:50:38.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      985 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1176 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1338 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1301 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:39.000000 trytond_account_stock_anglo_saxon-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      669 2019-10-11 23:09:47.000000 trytond_account_stock_anglo_saxon-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1124 2019-06-04 16:49:44.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2020-09-19 09:13:05.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2020-09-19 09:13:10.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2020-09-19 09:13:16.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2020-09-19 09:13:22.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      691 2020-09-19 09:13:26.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2020-09-19 09:13:32.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2020-09-19 09:13:37.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2020-09-19 09:13:43.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2020-09-19 09:13:50.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2020-09-19 09:13:57.000000 trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2942 2022-04-10 15:40:35.000000 trytond_account_stock_anglo_saxon-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2019-06-04 16:49:44.000000 trytond_account_stock_anglo_saxon-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:06:33.119537 trytond_account_stock_anglo_saxon-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5471 2022-10-29 07:39:10.000000 trytond_account_stock_anglo_saxon-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2021-12-11 16:59:32.000000 trytond_account_stock_anglo_saxon-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:33.116204 trytond_account_stock_anglo_saxon-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_stock_anglo_saxon-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12345 2021-10-30 15:32:31.000000 trytond_account_stock_anglo_saxon-6.6.0/tests/scenario_account_stock_anglo_saxon.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8065 2022-06-03 05:54:34.000000 trytond_account_stock_anglo_saxon-6.6.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1829 2022-04-16 16:30:56.000000 trytond_account_stock_anglo_saxon-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_account_stock_anglo_saxon-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2021-07-12 20:56:37.000000 trytond_account_stock_anglo_saxon-6.6.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:10:09.000000 trytond_account_stock_anglo_saxon-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2022-10-31 16:06:29.000000 trytond_account_stock_anglo_saxon-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:33.116204 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3253 2022-10-31 16:06:32.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2319 2022-10-31 16:06:33.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:06:32.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2022-10-31 16:06:32.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:00.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2022-10-31 16:06:32.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:06:32.000000 trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:33.116204 trytond_account_stock_anglo_saxon-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2018-08-18 09:54:20.000000 trytond_account_stock_anglo_saxon-6.6.0/view/category_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:12.705490 trytond_account_stock_anglo_saxon-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2422 2023-05-01 11:06:48.000000 trytond_account_stock_anglo_saxon-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:06:48.000000 trytond_account_stock_anglo_saxon-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3235 2023-05-01 11:50:12.705490 trytond_account_stock_anglo_saxon-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:12.705490 trytond_account_stock_anglo_saxon-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4253 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:12.702157 trytond_account_stock_anglo_saxon-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1337 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1275 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      985 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1176 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1338 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:45.000000 trytond_account_stock_anglo_saxon-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      669 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1124 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      691 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2942 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:50:12.708823 trytond_account_stock_anglo_saxon-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6714 2023-04-21 08:36:08.000000 trytond_account_stock_anglo_saxon-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:12.702157 trytond_account_stock_anglo_saxon-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12275 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tests/scenario_account_stock_anglo_saxon.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8008 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1829 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-05-01 11:06:42.000000 trytond_account_stock_anglo_saxon-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:12.705490 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3235 2023-05-01 11:50:11.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2293 2023-05-01 11:50:12.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:50:11.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 11:50:11.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 11:50:11.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:50:11.000000 trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:12.702157 trytond_account_stock_anglo_saxon-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-6.8.0/view/category_form.xml
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/CHANGELOG` & `trytond_account_stock_anglo_saxon-6.8.0/CHANGELOG`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/COPYRIGHT` & `trytond_account_stock_anglo_saxon-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/LICENSE` & `trytond_account_stock_anglo_saxon-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/PKG-INFO` & `trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_stock_anglo_saxon
-Version: 6.6.0
+Name: trytond-account-stock-anglo-saxon
+Version: 6.8.0
 Summary: Tryton module for anglo-saxon real-time stock valuation
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_anglo_saxon
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock valuation anglo-saxon
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
 
 Account Stock Anglo-Saxon Module
 ################################
 
 The account_stock_anglo_saxon module adds anglo-saxon accounting model for
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/README.rst` & `trytond_account_stock_anglo_saxon-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/doc/index.rst` & `trytond_account_stock_anglo_saxon-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/invoice.py` & `trytond_account_stock_anglo_saxon-6.8.0/invoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         if not self.product:
             return result
         if self.product.type != 'goods':
             return result
 
         accounting_date = (self.invoice.accounting_date
             or self.invoice.invoice_date)
-        period_id = Period.find(self.invoice.company.id, date=accounting_date)
-        period = Period(period_id)
+        period = Period.find(self.invoice.company, date=accounting_date)
         if period.fiscalyear.account_stock_method != 'anglo_saxon':
             return result
 
         # an empty list means we'll use the current cost price
         moves = []
         for move in self.stock_moves:
             if move.state != 'done':
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/bg.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/ca.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/cs.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/de.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/es.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/es_419.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/et.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/fa.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/fi.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/fr.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/hu.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/id.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/it.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/lo.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/lt.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/nl.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/pl.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/pt.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/ro.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/ru.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/sl.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/tr.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/uk.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/locale/zh_CN.po` & `trytond_account_stock_anglo_saxon-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/message.xml` & `trytond_account_stock_anglo_saxon-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_bg.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_ca.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_de.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_en.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_es.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_fr.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_nl.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_pt.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_ru.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/minimal_chart_sl.xml` & `trytond_account_stock_anglo_saxon-6.8.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/product.py` & `trytond_account_stock_anglo_saxon-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/setup.py` & `trytond_account_stock_anglo_saxon-6.8.0/setup.py`

 * *Files 10% similar despite different names*

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
 name = 'trytond_account_stock_anglo_saxon'
 
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
     get_require_version('trytond_sale_supply_drop_shipment'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_purchase')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for anglo-saxon real-time stock valuation',
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
-            'https://hg.tryton.org/modules/account_stock_anglo_saxon'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock valuation anglo-saxon',
     package_dir={'trytond.modules.account_stock_anglo_saxon': '.'},
     packages=(
         ['trytond.modules.account_stock_anglo_saxon']
         + ['trytond.modules.account_stock_anglo_saxon.%s' % p
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
     account_stock_anglo_saxon = trytond.modules.account_stock_anglo_saxon
     """,
     )
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/stock.py` & `trytond_account_stock_anglo_saxon-6.8.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,17 @@
 
     def _get_account_stock_move_lines(self, type_):
         pool = Pool()
         Uom = pool.get('product.uom')
         AccountMoveLine = pool.get('account.move.line')
         Currency = pool.get('currency.currency')
         lines = super(Move, self)._get_account_stock_move_lines(type_)
-        if (type_.endswith('supplier')
-                and self.product.cost_price_method == 'fixed'):
+        cost_price_method = self.product.get_multivalue(
+            'cost_price_method', **self._cost_price_pattern)
+        if type_.endswith('supplier') and cost_price_method == 'fixed':
             cost_price = Uom.compute_price(self.product.default_uom,
                 self.cost_price, self.uom)
             with Transaction().set_context(date=self.effective_date):
                 unit_price = Currency.compute(self.currency, self.unit_price,
                     self.company.currency, round=False)
             amount = self.company.currency.round(
                 Decimal(str(self.quantity)) * (unit_price - cost_price))
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/tests/scenario_account_stock_anglo_saxon.rst` & `trytond_account_stock_anglo_saxon-6.8.0/tests/scenario_account_stock_anglo_saxon.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ==================================
 Account Stock Anglo-Saxon Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
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
     ...         'account_stock_anglo_saxon',
     ...         'sale',
     ...         'purchase',
@@ -65,15 +65,15 @@
     >>> stock_group, = Group.find([('name', '=', 'Stock')])
     >>> stock_user.groups.append(stock_group)
     >>> stock_user.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.account_stock_method = 'anglo_saxon'
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_cogs_accounts(add_stock_accounts(
@@ -117,15 +117,15 @@
     >>> template.name = 'product'
     >>> template.default_uom = unit
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
     >>> template_average, = template.duplicate({'cost_price_method': 'average'})
     >>> template_average.account_category = account_category
@@ -240,15 +240,14 @@
     'processing'
 
 Send 5 products::
 
     >>> ShipmentOut = Model.get('stock.shipment.out')
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
@@ -351,15 +350,15 @@
     >>> template_by5.type = 'goods'
     >>> template_by5.purchasable = True
     >>> template_by5.purchase_uom = unit_5
     >>> template_by5.salable = True
     >>> template_by5.sale_uom = unit_5
     >>> template_by5.list_price = Decimal('10')
     >>> template_by5.cost_price_method = 'fixed'
-    >>> template_by5.lead_time = datetime.timedelta(0)
+    >>> template_by5.lead_time = dt.timedelta(0)
     >>> template_by5.account_category = account_category
     >>> product_by5, = template_by5.products
     >>> product_by5.cost_price = Decimal('5')
     >>> template_by5.save()
     >>> product_by5, = template_by5.products
 
     >>> set_user(purchase_user)
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst` & `trytond_account_stock_anglo_saxon-6.8.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 =====================================================
 Account Stock Anglo-Saxon with Drop Shipment Scenario
 =====================================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
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
     ...         'account_stock_anglo_saxon',
     ...         'sale_supply_drop_shipment',
     ...         'sale',
@@ -75,15 +75,15 @@
     >>> account_group, = Group.find([('name', '=', 'Account')])
     >>> account_user.groups.append(account_group)
     >>> account_user.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.account_stock_method = 'anglo_saxon'
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_cogs_accounts(add_stock_accounts(
@@ -128,26 +128,26 @@
     >>> template.name = 'product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.purchasable = True
     >>> template.salable = True
     >>> template.list_price = Decimal('10')
     >>> template.cost_price_method = 'fixed'
-    >>> template.lead_time = datetime.timedelta(0)
-    >>> template.supply_on_sale = True
+    >>> template.lead_time = dt.timedelta(0)
+    >>> template.supply_on_sale = 'always'
     >>> template.account_category = account_category
     >>> product, = template.products
     >>> product.cost_price = Decimal('5')
     >>> template.save()
     >>> product, = template.products
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = template
     >>> product_supplier.party = supplier
     >>> product_supplier.drop_shipment = True
-    >>> product_supplier.lead_time = datetime.timedelta(0)
+    >>> product_supplier.lead_time = dt.timedelta(0)
     >>> product_supplier.save()
 
 Create payment term::
 
     >>> payment_term = create_payment_term()
     >>> payment_term.save()
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/tests/test_module.py` & `trytond_account_stock_anglo_saxon-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/tests/tools.py` & `trytond_account_stock_anglo_saxon-6.8.0/tests/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model
-
 from trytond.modules.company.tests.tools import get_company
 
 
 def add_cogs_accounts(accounts, company=None, config=None):
     "Add COGS to accounts"
     Account = Model.get('account.account', config=config)
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO` & `trytond_account_stock_anglo_saxon-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-stock-anglo-saxon
-Version: 6.6.0
+Name: trytond_account_stock_anglo_saxon
+Version: 6.8.0
 Summary: Tryton module for anglo-saxon real-time stock valuation
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_anglo_saxon
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock valuation anglo-saxon
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
 
 Account Stock Anglo-Saxon Module
 ################################
 
 The account_stock_anglo_saxon module adds anglo-saxon accounting model for
```

### Comparing `trytond_account_stock_anglo_saxon-6.6.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt` & `trytond_account_stock_anglo_saxon-6.8.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt`

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
 account.py
@@ -75,14 +71,15 @@
 ./tests/__init__.py
 ./tests/scenario_account_stock_anglo_saxon.rst
 ./tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./tests/tools.py
 ./view/category_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

