# Comparing `tmp/trytond_sale_advance_payment-6.6.0.tar.gz` & `tmp/trytond_sale_advance_payment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_advance_payment-6.6.0.tar", last modified: Mon Oct 31 16:20:01 2022, max compression
+gzip compressed data, was "trytond_sale_advance_payment-6.8.0.tar", last modified: Mon May  1 11:55:06 2023, max compression
```

## Comparing `trytond_sale_advance_payment-6.6.0.tar` & `trytond_sale_advance_payment-6.8.0.tar`

### file list

```diff
@@ -1,84 +1,81 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:01.517958 trytond_sale_advance_payment-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_advance_payment-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_advance_payment-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2022-10-31 16:20:00.000000 trytond_sale_advance_payment-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_advance_payment-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2022-10-31 16:19:59.000000 trytond_sale_advance_payment-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 16:19:58.000000 trytond_sale_advance_payment-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:00.000000 trytond_sale_advance_payment-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_advance_payment-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4024 2022-10-31 16:20:01.517958 trytond_sale_advance_payment-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2018-08-18 09:55:00.000000 trytond_sale_advance_payment-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2021-12-11 16:59:34.000000 trytond_sale_advance_payment-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2651 2022-04-12 08:31:36.000000 trytond_sale_advance_payment-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2019-06-04 16:49:45.000000 trytond_sale_advance_payment-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:01.514624 trytond_sale_advance_payment-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2018-08-18 09:55:00.000000 trytond_sale_advance_payment-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2021-12-11 16:59:34.000000 trytond_sale_advance_payment-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:01.514624 trytond_sale_advance_payment-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6244 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6144 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6189 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4752 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5189 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6656 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6189 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4838 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4995 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5200 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6199 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5063 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5905 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4841 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5597 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4752 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4960 2022-10-29 07:50:41.000000 trytond_sale_advance_payment-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2019-10-11 23:09:48.000000 trytond_sale_advance_payment-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2242 2019-06-04 16:49:45.000000 trytond_sale_advance_payment-6.6.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2020-09-19 09:15:22.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1213 2020-09-19 09:15:27.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2020-09-19 09:15:33.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1205 2020-09-19 09:15:40.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2020-09-19 09:15:44.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2020-09-19 09:15:50.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1210 2020-09-19 09:15:56.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1214 2020-09-19 09:16:04.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2020-09-19 09:16:12.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1211 2020-09-19 09:16:20.000000 trytond_sale_advance_payment-6.6.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    17434 2022-10-11 19:49:58.000000 trytond_sale_advance_payment-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5721 2021-03-24 12:34:22.000000 trytond_sale_advance_payment-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:20:01.517958 trytond_sale_advance_payment-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5387 2022-10-29 07:39:11.000000 trytond_sale_advance_payment-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2020-03-01 11:49:48.000000 trytond_sale_advance_payment-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:01.514624 trytond_sale_advance_payment-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_advance_payment-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12385 2021-12-16 21:33:22.000000 trytond_sale_advance_payment-6.6.0/tests/scenario_advance_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2022-04-16 16:30:57.000000 trytond_sale_advance_payment-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_advance_payment-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1291 2021-07-12 20:56:37.000000 trytond_sale_advance_payment-6.6.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2022-10-31 15:10:09.000000 trytond_sale_advance_payment-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2022-10-31 16:19:57.000000 trytond_sale_advance_payment-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:01.517958 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4024 2022-10-31 16:20:00.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2644 2022-10-31 16:20:01.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:20:00.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2022-10-31 16:20:00.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:04.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      168 2022-10-31 16:20:00.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:20:00.000000 trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:01.514624 trytond_sale_advance_payment-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2019-06-04 16:49:45.000000 trytond_sale_advance_payment-6.6.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      735 2018-08-18 09:55:00.000000 trytond_sale_advance_payment-6.6.0/view/advance_payment_condition_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2019-10-11 23:09:48.000000 trytond_sale_advance_payment-6.6.0/view/advance_payment_condition_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2018-08-18 09:55:00.000000 trytond_sale_advance_payment-6.6.0/view/advance_payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2018-08-18 09:55:00.000000 trytond_sale_advance_payment-6.6.0/view/advance_payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2019-10-11 23:09:48.000000 trytond_sale_advance_payment-6.6.0/view/advance_payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-10-11 23:09:48.000000 trytond_sale_advance_payment-6.6.0/view/advance_payment_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2020-04-26 13:06:29.000000 trytond_sale_advance_payment-6.6.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:06.202466 trytond_sale_advance_payment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-05-01 11:10:11.000000 trytond_sale_advance_payment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:10:11.000000 trytond_sale_advance_payment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4011 2023-05-01 11:55:06.202466 trytond_sale_advance_payment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2651 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:06.199132 trytond_sale_advance_payment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:06.195799 trytond_sale_advance_payment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6244 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6144 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6189 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4752 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5189 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6656 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6189 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4838 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4995 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5200 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6199 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5063 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5905 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4841 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5597 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4752 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4960 2023-04-29 08:02:47.000000 trytond_sale_advance_payment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1213 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1210 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1211 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16918 2023-04-21 08:36:08.000000 trytond_sale_advance_payment-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5721 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:55:06.202466 trytond_sale_advance_payment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4571 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:06.195799 trytond_sale_advance_payment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12047 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/tests/scenario_advance_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-05-01 11:10:06.000000 trytond_sale_advance_payment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:06.202466 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4011 2023-05-01 11:55:05.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2618 2023-05-01 11:55:06.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:55:05.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:55:05.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      168 2023-05-01 11:55:05.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:55:05.000000 trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:06.199132 trytond_sale_advance_payment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      735 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-6.8.0/view/advance_payment_condition_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/view/advance_payment_condition_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-6.8.0/view/advance_payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-6.8.0/view/advance_payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/view/advance_payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/view/advance_payment_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-6.8.0/view/sale_form.xml
```

### Comparing `trytond_sale_advance_payment-6.6.0/CHANGELOG` & `trytond_sale_advance_payment-6.8.0/CHANGELOG`

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
 * Fill origin name of invoice line from condition
```

### Comparing `trytond_sale_advance_payment-6.6.0/COPYRIGHT` & `trytond_sale_advance_payment-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2015-2022 Nicolas Évrard.
-Copyright (C) 2017-2022 Cédric Krier.
-Copyright (C) 2015-2022 B2CK SPRL.
+Copyright (C) 2015-2023 Nicolas Évrard.
+Copyright (C) 2017-2023 Cédric Krier.
+Copyright (C) 2015-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_advance_payment-6.6.0/LICENSE` & `trytond_sale_advance_payment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/PKG-INFO` & `trytond_sale_advance_payment-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_advance_payment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale advance payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_advance_payment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale advance payment
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
 
 Sale Advance Payment Module
 ###########################
 
 The sale_advance_payment module adds support for advance payment management on
```

### Comparing `trytond_sale_advance_payment-6.6.0/README.rst` & `trytond_sale_advance_payment-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/__init__.py` & `trytond_sale_advance_payment-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/account.py` & `trytond_sale_advance_payment-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/account.xml` & `trytond_sale_advance_payment-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/doc/index.rst` & `trytond_sale_advance_payment-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/bg.po` & `trytond_sale_advance_payment-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/ca.po` & `trytond_sale_advance_payment-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/cs.po` & `trytond_sale_advance_payment-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/de.po` & `trytond_sale_advance_payment-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/es.po` & `trytond_sale_advance_payment-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/es_419.po` & `trytond_sale_advance_payment-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/et.po` & `trytond_sale_advance_payment-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/fa.po` & `trytond_sale_advance_payment-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/fi.po` & `trytond_sale_advance_payment-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/fr.po` & `trytond_sale_advance_payment-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/hu.po` & `trytond_sale_advance_payment-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/id.po` & `trytond_sale_advance_payment-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/it.po` & `trytond_sale_advance_payment-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/lo.po` & `trytond_sale_advance_payment-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/lt.po` & `trytond_sale_advance_payment-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/nl.po` & `trytond_sale_advance_payment-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/pl.po` & `trytond_sale_advance_payment-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/pt.po` & `trytond_sale_advance_payment-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/ro.po` & `trytond_sale_advance_payment-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/ru.po` & `trytond_sale_advance_payment-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/sl.po` & `trytond_sale_advance_payment-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/tr.po` & `trytond_sale_advance_payment-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/uk.po` & `trytond_sale_advance_payment-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/locale/zh_CN.po` & `trytond_sale_advance_payment-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/message.xml` & `trytond_sale_advance_payment-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_bg.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_ca.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_de.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_en.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_es.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_fr.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_nl.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_pt.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_ru.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/minimal_chart_sl.xml` & `trytond_sale_advance_payment-6.8.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/sale.py` & `trytond_sale_advance_payment-6.8.0/sale.py`

 * *Files 10% similar despite different names*

```diff
@@ -196,21 +196,19 @@
     @fields.depends('sale', '_parent_sale.state')
     def on_change_with_sale_state(self, name=None):
         if self.sale:
             return self.sale.state
 
     @fields.depends('sale', '_parent_sale.company')
     def on_change_with_sale_company(self, name=None):
-        if self.sale and self.sale.company:
-            return self.sale.company.id
+        return self.sale.company if self.sale else None
 
     @fields.depends('sale', '_parent_sale.currency')
     def on_change_with_currency(self, name=None):
-        if self.sale and self.sale.currency:
-            return self.sale.currency.id
+        return self.sale.currency if self.sale else None
 
     @classmethod
     def copy(cls, conditions, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
@@ -339,31 +337,19 @@
                 if invoice_line.invoice:
                     invoices.add(invoice_line.invoice.id)
         return list(invoices)
 
     @classmethod
     def search_advance_payment_invoices(cls, name, clause):
         return [('advance_payment_conditions.invoice_lines.invoice'
-                + clause[0].lstrip(name),)
-            + tuple(clause[1:])]
+                + clause[0][len(name):], *clause[1:])]
 
-    def get_invoice_state(self):
-        state = super(Sale, self).get_invoice_state()
-        skip_ids = set(x.id for x in self.invoices_ignored)
-        skip_ids.update(x.id for x in self.invoices_recreated)
-        invoices = [i
-            for i in self.advance_payment_invoices if i.id not in skip_ids]
-        if invoices:
-            if any(i.state == 'cancelled' for i in invoices):
-                return 'exception'
-            elif all(i.state == 'paid' for i in invoices):
-                return state
-            else:
-                return 'waiting'
-        return state
+    @property
+    def _invoices_for_state(self):
+        return super()._invoices_for_state + self.advance_payment_invoices
 
     def get_recall_lines(self, invoice):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
 
         recall_lines = []
         advance_lines = InvoiceLine.search([
@@ -448,16 +434,16 @@
     def get_move(self, shipment_type):
         move = super(SaleLine, self).get_move(shipment_type)
         if (self.sale.advance_payment_eligible(shipment_type)
                 and self.sale.supply_blocked):
             return None
         return move
 
-    def get_purchase_request(self):
-        request = super(SaleLine, self).get_purchase_request()
+    def get_purchase_request(self, product_quantities):
+        request = super().get_purchase_request(product_quantities)
         if (self.sale.advance_payment_eligible()
                 and self.sale.supply_blocked):
             return None
         return request
 
     def get_invoice_line(self):
         lines = super(SaleLine, self).get_invoice_line()
```

### Comparing `trytond_sale_advance_payment-6.6.0/sale.xml` & `trytond_sale_advance_payment-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/setup.py` & `trytond_sale_advance_payment-6.8.0/setup.py`

 * *Files 20% similar despite different names*

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
 name = 'trytond_sale_advance_payment'
 
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
 
 requires = ['simpleeval']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 for dep in ['sale_supply']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for sale advance payment',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_advance_payment',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale advance payment',
     package_dir={'trytond.modules.sale_advance_payment': '.'},
     packages=(
         ['trytond.modules.sale_advance_payment']
         + ['trytond.modules.sale_advance_payment.%s' % p
             for p in find_packages()]
@@ -127,28 +105,27 @@
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
     sale_advance_payment = trytond.modules.sale_advance_payment
     """,
     )
```

### Comparing `trytond_sale_advance_payment-6.6.0/stock.py` & `trytond_sale_advance_payment-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/tests/scenario_advance_payment.rst` & `trytond_sale_advance_payment-6.8.0/tests/scenario_advance_payment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 ==============================
 Sale Advance Payment Scenario
 ==============================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from dateutil.relativedelta import relativedelta
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.sale_advance_payment.tests.tools import \
     ...     create_advance_payment_term, add_advance_payment_accounts
-    >>> today = datetime.date.today()
-    >>> next_week = today + relativedelta(days=7)
+
+    >>> today = dt.date.today()
+    >>> next_week = today + dt.timedelta(days=7)
 
 Activate sale_advance_payment::
 
     >>> config = activate_modules(['sale_advance_payment', 'sale_supply'])
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal years::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, today=today))
+    ...     create_fiscalyear(company, (today, next_week)))
     >>> fiscalyear.click('create_period')
-    >>> next_fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, today=today + relativedelta(years=1)))
-    >>> next_fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_advance_payment_accounts(get_accounts(company))
     >>> revenue = accounts['revenue']
     >>> payable = accounts['payable']
@@ -179,15 +176,15 @@
     >>> len(sale.invoices)
     0
     >>> len(sale.shipments)
     0
 
 Let's pay the advance payment invoice::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
 
     >>> sale.reload()
     >>> sale.state
     'processing'
     >>> len(sale.invoices)
@@ -244,29 +241,28 @@
 
     >>> shipment, = sale.shipments
 
 Let's try to pack it::
 
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> shipment.click('pack')  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     ShippingBlocked: ...
 
 Let's pay the advance payment invoice::
 
     >>> invoice, = sale.advance_payment_invoices
     >>> invoice.invoice_date == next_week
     True
     >>> invoice.invoice_date = None
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> sale.reload()
     >>> sale.state
     'processing'
 
 Packing the shipment is now allowed::
@@ -285,15 +281,15 @@
     >>> sos_template.name = 'Supply On Sale product'
     >>> sos_template.default_uom = unit
     >>> sos_template.type = 'goods'
     >>> sos_template.purchasable = True
     >>> sos_template.salable = True
     >>> sos_template.list_price = Decimal('10')
     >>> sos_template.account_category = account_category
-    >>> sos_template.supply_on_sale = True
+    >>> sos_template.supply_on_sale = 'always'
     >>> sos_template.save()
     >>> sos_product, = sos_template.products
 
 Sell 10 of those products::
 
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
@@ -318,15 +314,15 @@
 The advance payment invoice has been created, now pay it::
 
     >>> invoice, = sale.advance_payment_invoices
     >>> invoice.invoice_date == next_week
     True
     >>> invoice.invoice_date = None
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> sale.reload()
     >>> sale.state
     'processing'
 
 There is now a purchase request of the desired quantity::
@@ -363,15 +359,15 @@
     >>> sale.reload()
     >>> sale.invoice_state
     'exception'
 
 Handle the exception on the sale level, not recreating the invoice will create
 the final invoice with the remaining total::
 
-    >>> handle_exception = Wizard('sale.handle.invoice.exception', [sale])
+    >>> handle_exception = sale.click('handle_invoice_exception')
     >>> _ = handle_exception.form.recreate_invoices.pop()
     >>> handle_exception.execute('handle')
 
     >>> sale.reload()
     >>> len(sale.advance_payment_invoices)
     1
     >>> last_invoice, = sale.invoices
@@ -396,24 +392,24 @@
     'processing'
     >>> inv, = sale.advance_payment_invoices
     >>> inv.click('cancel')
     >>> sale.reload()
     >>> sale.invoice_state
     'exception'
 
-    >>> handle_exception = Wizard('sale.handle.invoice.exception', [sale])
+    >>> handle_exception = sale.click('handle_invoice_exception')
     >>> handle_exception.execute('handle')
     >>> sale.reload()
     >>> _, inv_recreated = sale.advance_payment_invoices
     >>> inv_recreated.total_amount
     Decimal('10.00')
     >>> inv_recreated.invoice_date == next_week
     True
     >>> inv_recreated.invoice_date = None
     >>> inv_recreated.click('post')
-    >>> pay = Wizard('account.invoice.pay', [inv_recreated])
+    >>> pay = inv_recreated.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> sale.reload()
     >>> last_invoice, = sale.invoices
     >>> last_invoice.total_amount
     Decimal('90.00')
```

### Comparing `trytond_sale_advance_payment-6.6.0/tests/tools.py` & `trytond_sale_advance_payment-6.8.0/tests/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from datetime import timedelta
 
 from proteus import Model
-
 from trytond.modules.company.tests.tools import get_company
 
 
 def create_advance_payment_term(
         name, formula, account, block_supply=False, block_shipping=False,
         delay=7, config=None):
     "Create an advance payment term"
```

### Comparing `trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/PKG-INFO` & `trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-advance-payment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale advance payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_advance_payment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale advance payment
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
 
 Sale Advance Payment Module
 ###########################
 
 The sale_advance_payment module adds support for advance payment management on
```

### Comparing `trytond_sale_advance_payment-6.6.0/trytond_sale_advance_payment.egg-info/SOURCES.txt` & `trytond_sale_advance_payment-6.8.0/trytond_sale_advance_payment.egg-info/SOURCES.txt`

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
@@ -81,14 +77,15 @@
 ./view/advance_payment_condition_form.xml
 ./view/advance_payment_condition_list.xml
 ./view/advance_payment_term_form.xml
 ./view/advance_payment_term_line_form.xml
 ./view/advance_payment_term_line_list.xml
 ./view/advance_payment_term_list.xml
 ./view/sale_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_sale_advance_payment-6.6.0/view/advance_payment_condition_form.xml` & `trytond_sale_advance_payment-6.8.0/view/advance_payment_condition_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/view/advance_payment_term_line_form.xml` & `trytond_sale_advance_payment-6.8.0/view/advance_payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-6.6.0/view/sale_form.xml` & `trytond_sale_advance_payment-6.8.0/view/sale_form.xml`

 * *Files identical despite different names*

