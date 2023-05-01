# Comparing `tmp/trytond_stock_forecast-6.6.0.tar.gz` & `tmp/trytond_stock_forecast-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_forecast-6.6.0.tar", last modified: Mon Oct 31 15:57:12 2022, max compression
+gzip compressed data, was "trytond_stock_forecast-6.8.0.tar", last modified: Mon May  1 11:54:45 2023, max compression
```

## Comparing `trytond_stock_forecast-6.6.0.tar` & `trytond_stock_forecast-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:57:12.784723 trytond_stock_forecast-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_stock_forecast-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_forecast-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-31 15:57:11.000000 trytond_stock_forecast-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_forecast-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2560 2022-10-31 15:57:10.000000 trytond_stock_forecast-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:57:10.000000 trytond_stock_forecast-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:13.000000 trytond_stock_forecast-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_forecast-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3552 2022-10-31 15:57:12.784723 trytond_stock_forecast-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2020-06-04 11:08:36.000000 trytond_stock_forecast-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2021-12-11 16:59:34.000000 trytond_stock_forecast-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:57:12.781390 trytond_stock_forecast-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2020-06-04 11:08:36.000000 trytond_stock_forecast-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2019-06-04 16:49:45.000000 trytond_stock_forecast-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22041 2022-10-11 19:49:58.000000 trytond_stock_forecast-6.6.0/forecast.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7408 2021-04-27 07:34:41.000000 trytond_stock_forecast-6.6.0/forecast.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:57:12.778057 trytond_stock_forecast-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5576 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5419 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4756 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5555 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5414 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4592 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4980 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5769 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4756 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5457 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4991 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4659 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5006 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5414 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4768 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5352 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4951 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5247 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4508 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5773 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5133 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4756 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4486 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4811 2022-10-29 07:50:41.000000 trytond_stock_forecast-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      777 2019-08-09 14:52:50.000000 trytond_stock_forecast-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:57:12.784723 trytond_stock_forecast-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5064 2022-10-29 07:39:11.000000 trytond_stock_forecast-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:57:12.778057 trytond_stock_forecast-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_forecast-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13313 2022-04-16 16:30:57.000000 trytond_stock_forecast-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2022-10-31 15:10:09.000000 trytond_stock_forecast-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      119 2022-10-31 15:57:09.000000 trytond_stock_forecast-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:57:12.784723 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3552 2022-10-31 15:57:12.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-31 15:57:12.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:57:12.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 15:57:12.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:04.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2022-10-31 15:57:12.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:57:12.000000 trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:57:12.781390 trytond_stock_forecast-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2018-08-18 09:55:13.000000 trytond_stock_forecast-6.6.0/view/forecast_complete_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2018-08-18 09:55:13.000000 trytond_stock_forecast-6.6.0/view/forecast_complete_choose_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      915 2019-10-11 21:50:16.000000 trytond_stock_forecast-6.6.0/view/forecast_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      617 2021-10-07 13:08:07.000000 trytond_stock_forecast-6.6.0/view/forecast_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2019-12-28 17:16:43.000000 trytond_stock_forecast-6.6.0/view/forecast_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2022-04-08 16:23:27.000000 trytond_stock_forecast-6.6.0/view/forecast_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:45.912214 trytond_stock_forecast-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2750 2023-05-01 11:09:58.000000 trytond_stock_forecast-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:09:58.000000 trytond_stock_forecast-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_forecast-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3545 2023-05-01 11:54:45.908880 trytond_stock_forecast-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:45.908880 trytond_stock_forecast-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21470 2023-04-21 08:36:08.000000 trytond_stock_forecast-6.8.0/forecast.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7130 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/forecast.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:45.905547 trytond_stock_forecast-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5327 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5156 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4508 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5299 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5147 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4753 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5504 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4508 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5196 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4787 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4481 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4762 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5167 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4541 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4719 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5000 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4333 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5514 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4900 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4508 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4279 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4563 2023-04-30 10:46:36.000000 trytond_stock_forecast-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      777 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:54:45.912214 trytond_stock_forecast-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4253 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:45.905547 trytond_stock_forecast-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14556 2023-04-21 08:36:08.000000 trytond_stock_forecast-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2023-05-01 11:09:53.000000 trytond_stock_forecast-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:45.908880 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3545 2023-05-01 11:54:45.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-05-01 11:54:45.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:54:45.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:54:45.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      126 2023-05-01 11:54:45.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:54:45.000000 trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:45.908880 trytond_stock_forecast-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/view/forecast_complete_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      915 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/view/forecast_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      617 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/view/forecast_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/view/forecast_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/view/forecast_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_stock_forecast-6.8.0/view/product_list_forecast.xml
```

### Comparing `trytond_stock_forecast-6.6.0/CHANGELOG` & `trytond_stock_forecast-6.8.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Simplify complete wizard
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

### Comparing `trytond_stock_forecast-6.6.0/COPYRIGHT` & `trytond_stock_forecast-6.8.0/COPYRIGHT`

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

### Comparing `trytond_stock_forecast-6.6.0/LICENSE` & `trytond_stock_forecast-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-6.6.0/PKG-INFO` & `trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_forecast
-Version: 6.6.0
+Name: trytond-stock-forecast
+Version: 6.8.0
 Summary: Tryton module with stock forecasts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_forecast
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock forecast
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
 License-File: LICENSE
 
 Stock Forecast Module
 #####################
 
 The stock forecast module provide a simple way to create stock moves
 toward customers with a date in the future. This allow other stock
```

### Comparing `trytond_stock_forecast-6.6.0/README.rst` & `trytond_stock_forecast-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-6.6.0/__init__.py` & `trytond_stock_forecast-6.8.0/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
 def register():
     Pool.register(
         forecast.Forecast,
         forecast.ForecastLine,
         forecast.ForecastLineMove,
         forecast.ForecastCompleteAsk,
-        forecast.ForecastCompleteChoose,
         module='stock_forecast', type_='model')
     Pool.register(
         forecast.ForecastComplete,
         module='stock_forecast', type_='wizard')
```

### Comparing `trytond_stock_forecast-6.6.0/doc/index.rst` & `trytond_stock_forecast-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-6.6.0/forecast.py` & `trytond_stock_forecast-6.8.0/forecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,19 +157,35 @@
                 return [('to_date', operators[clause[1]], today)]
             else:
                 return [('to_date', operators[reverse[clause[1]]], today)]
         else:
             return []
 
     def get_rec_name(self, name):
-        return self.warehouse.rec_name
+        pool = Pool()
+        Lang = pool.get('ir.lang')
+
+        lang = Lang.get()
+        from_date = lang.strftime(self.from_date)
+        to_date = lang.strftime(self.to_date)
+        return (
+            f'{self.warehouse.rec_name} → {self.destination.rec_name} @ '
+            f'[{from_date} - {to_date}]')
 
     @classmethod
     def search_rec_name(cls, name, clause):
-        return [('warehouse.rec_name',) + tuple(clause[1:])]
+        operator = clause[1]
+        if operator.startswith('!') or operator.startswith('not '):
+            bool_op = 'AND'
+        else:
+            bool_op = 'OR'
+        return [bool_op,
+            ('warehouse.rec_name', *clause[1:]),
+            ('destination.rec_name', *clause[1:]),
+            ]
 
     @classmethod
     def validate_fields(cls, forecasts, field_names):
         super().validate_fields(forecasts, field_names)
         cls.check_date_overlap(forecasts, field_names)
 
     @classmethod
@@ -335,16 +351,15 @@
     @fields.depends('product')
     def on_change_product(self):
         if self.product:
             self.uom = self.product.default_uom
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @classmethod
     def get_forecast_states(cls):
         pool = Pool()
         Forecast = pool.get('stock.forecast')
         return Forecast.fields_get(['state'])['state']['selection']
 
@@ -420,52 +435,49 @@
         default.setdefault('moves', None)
         return super(ForecastLine, cls).copy(lines, default=default)
 
     def get_moves(self):
         'Get stock moves for the forecast line'
         pool = Pool()
         Move = pool.get('stock.move')
-        Uom = pool.get('product.uom')
         Date = pool.get('ir.date')
 
         assert not self.moves
 
         today = Date.today()
         from_date = self.forecast.from_date
         if from_date < today:
             from_date = today
         to_date = self.forecast.to_date
         if to_date < today:
             return []
+        if self.quantity_executed >= self.quantity:
+            return []
 
         delta = to_date - from_date
         delta = delta.days + 1
         nb_packet = ((self.quantity - self.quantity_executed)
             // self.minimal_quantity)
         distribution = self.distribute(delta, nb_packet)
-        unit_price = None
-        if self.forecast.destination.type == 'customer':
-            unit_price = self.product.list_price or 0
-            unit_price = Uom.compute_price(self.product.default_uom,
-                unit_price, self.uom)
 
         moves = []
         for day, qty in distribution.items():
             if qty == 0.0:
                 continue
             move = Move()
             move.from_location = self.forecast.warehouse.storage_location
             move.to_location = self.forecast.destination
             move.product = self.product
             move.uom = self.uom
             move.quantity = qty * self.minimal_quantity
             move.planned_date = from_date + datetime.timedelta(day)
             move.company = self.forecast.company
             move.currency = self.forecast.company.currency
-            move.unit_price = unit_price
+            move.unit_price = (
+                0 if self.forecast.destination.type == 'customer' else None)
             moves.append(move)
         return moves
 
     @classmethod
     def delete_moves(cls, lines):
         'Delete stock moves of the forecast line'
         Move = Pool().get('stock.move')
@@ -509,120 +521,90 @@
     move = fields.Many2One(
         'stock.move', "Move", ondelete='CASCADE', required=True)
 
 
 class ForecastCompleteAsk(ModelView):
     'Complete Forecast'
     __name__ = 'stock.forecast.complete.ask'
+    company = fields.Many2One('company.company', "Company", readonly=True)
+    warehouse = fields.Many2One('stock.location', "Warehouse", readonly=True)
+    destination = fields.Many2One(
+        'stock.location', "Destination", readonly=True)
     from_date = fields.Date(
         "From Date", required=True,
-        domain=[('from_date', '<', Eval('to_date'))])
+        domain=[('from_date', '<', Eval('to_date'))],
+        states={
+            'readonly': Bool(Eval('products')),
+            })
     to_date = fields.Date(
         "To Date", required=True,
-        domain=[('to_date', '>', Eval('from_date'))])
-
-
-class ForecastCompleteChoose(ModelView):
-    'Complete Forecast'
-    __name__ = 'stock.forecast.complete.choose'
+        domain=[('to_date', '>', Eval('from_date'))],
+        states={
+            'readonly': Bool(Eval('products')),
+            })
     products = fields.Many2Many(
         'product.product', None, None, "Products",
         domain=[
             ('type', '=', 'goods'),
             ('consumable', '=', False),
-            ])
+            ],
+        context={
+            'company': Eval('company', -1),
+            'locations': [Eval('warehouse', -1)],
+            'stock_destinations': [Eval('destination', -1)],
+            'stock_date_start': Eval('from_date', None),
+            'stock_date_end': Eval('to_date', None),
+            'with_childs': True,
+            'stock_invert': True,
+            },
+        depends=[
+            'company', 'warehouse', 'destination', 'from_date', 'to_date'])
 
 
 class ForecastComplete(Wizard):
     'Complete Forecast'
     __name__ = 'stock.forecast.complete'
     start_state = 'ask'
     ask = StateView('stock.forecast.complete.ask',
         'stock_forecast.forecast_complete_ask_view_form', [
-            Button('Cancel', 'end', 'tryton-cancel'),
-            Button('Choose Products', 'choose', 'tryton-forward'),
-            Button('Complete', 'complete', 'tryton-ok', default=True),
-            ])
-    choose = StateView('stock.forecast.complete.choose',
-        'stock_forecast.forecast_complete_choose_view_form', [
-            Button('Cancel', 'end', 'tryton-cancel'),
-            Button('Choose Dates', 'ask', 'tryton-back'),
-            Button('Complete', 'complete', 'tryton-ok', default=True),
+            Button("Cancel", 'end', 'tryton-cancel'),
+            Button("Complete", 'complete', 'tryton-ok', default=True),
             ])
     complete = StateTransition()
 
     def default_ask(self, fields):
         """
         Forecast dates shifted by one year.
         """
         default = {}
-        for field in ("to_date", "from_date"):
-            default[field] = (
-                getattr(self.record, field) - relativedelta(years=1))
+        for field in ['company', 'warehouse', 'destination']:
+            if field in fields:
+                record = getattr(self.record, field)
+                default[field] = record.id
+        for field in ["to_date", "from_date"]:
+            if field in fields:
+                default[field] = (
+                    getattr(self.record, field) - relativedelta(years=1))
         return default
 
-    def _get_product_quantity(self):
-        pool = Pool()
-        Product = pool.get('product.product')
-
-        with Transaction().set_context(
-                stock_destinations=[self.record.destination.id],
-                stock_date_start=self.ask.from_date,
-                stock_date_end=self.ask.to_date):
-            return Product.products_by_location([self.record.warehouse.id],
-                with_childs=True)
-
-    def default_choose(self, fields):
-        """
-        Collect products for which there is an outgoing stream between
-        the given location and the destination.
-        """
-        if getattr(self.choose, 'products', None):
-            return {'products': [x.id for x in self.choose.products]}
-        pbl = self._get_product_quantity()
-        products = []
-        for (_, product), qty in pbl.items():
-            if qty < 0:
-                products.append(product)
-        return {'products': products}
-
     def transition_complete(self):
         pool = Pool()
         ForecastLine = pool.get('stock.forecast.line')
-        Product = pool.get('product.product')
-
-        forecast = self.record
-        prod2line = {}
-        forecast_lines = ForecastLine.search([
-                ('forecast', '=', forecast.id),
-                ])
-        for forecast_line in forecast_lines:
-            prod2line[forecast_line.product.id] = forecast_line
-
-        pbl = self._get_product_quantity()
-        id2product = {p.id: p for p in Product.browse([x[1] for x in pbl])}
-
-        products = set(getattr(self.choose, 'products', {}))
 
+        product2line = {l.product: l for l in self.record.lines}
         to_save = []
-        for key, qty in pbl.items():
-            _, product_id = key
-            product = id2product[product_id]
-            if products and product not in products:
-                continue
-            if product.type != 'goods' or product.consumable:
-                continue
-            if -qty <= 0:
-                continue
-            if product in prod2line:
-                line = prod2line[product]
-            else:
-                line = ForecastLine()
-            line.product = product
-            line.quantity = -qty
-            line.uom = product.default_uom.id
-            line.forecast = forecast
-            line.minimal_quantity = min(1, -qty)
+        # Ensure context is set
+        self.ask.products = map(int, self.ask.products)
+        for product in self.ask.products:
+            line = product2line.get(product, ForecastLine())
+            self._fill_line(line, product)
             to_save.append(line)
-
         ForecastLine.save(to_save)
         return 'end'
+
+    def _fill_line(self, line, product):
+        quantity = max(product.quantity, 0)
+        line.product = product
+        line.quantity = quantity
+        line.uom = product.default_uom.id
+        line.forecast = self.record
+        line.minimal_quantity = min(1, quantity)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/forecast.xml` & `trytond_stock_forecast-6.8.0/forecast.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_stock_forecast-6.6.0/forecast.xml` & `trytond_stock_forecast-6.8.0/forecast.xml`

```diff
@@ -70,19 +70,14 @@
       <field name="name">forecast_line_tree</field>
     </record>
     <record model="ir.ui.view" id="forecast_complete_ask_view_form">
       <field name="model">stock.forecast.complete.ask</field>
       <field name="type">form</field>
       <field name="name">forecast_complete_ask_form</field>
     </record>
-    <record model="ir.ui.view" id="forecast_complete_choose_view_form">
-      <field name="model">stock.forecast.complete.choose</field>
-      <field name="type">form</field>
-      <field name="name">forecast_complete_choose_form</field>
-    </record>
     <record model="ir.rule.group" id="rule_group_forecast_companies">
       <field name="name">User in companies</field>
       <field name="model" search="[('model', '=', 'stock.forecast')]"/>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_forecast_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
```

### Comparing `trytond_stock_forecast-6.6.0/locale/bg.po` & `trytond_stock_forecast-6.8.0/locale/bg.po`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,40 @@
 msgid "To Date"
 msgstr "До дата"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "Местоположение"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Фирма"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Местонахождение-цел"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "От дата"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Продукти"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "До дата"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Продукти"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Прогноза"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
@@ -160,18 +175,14 @@
 msgid "Stock Forecast"
 msgstr "Прогноза за наличност"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Изготвяне на прогноза"
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Изготвяне на прогноза"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr "Ред от прогноза за наличност"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr "Ред от прогноза - Движение"
@@ -193,30 +204,14 @@
 msgid "Add forecast line based on past data."
 msgstr "Добавяне на ред от прогноза въз основа на минали данни"
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Изготвяне на прогноза"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Избот на продукти"
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr "Изпълнен"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "Отказ"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Избор на дати"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Пълен"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Отказ"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/ca.po` & `trytond_stock_forecast-6.8.0/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,37 @@
 msgid "To Date"
 msgstr "Fins a la data"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "Ubicació"
 
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Empresa"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Destí"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "Des de la data"
 
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Productes"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "Fins a la data"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Productes"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr "Magatzem"
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Previsió"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
@@ -155,18 +167,14 @@
 msgid "Stock Forecast"
 msgstr "Previsió d'existències"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Demanar previsió completa"
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Triar previsió completa"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr "Línia de previsió d'existències"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr "Línia de previsió - Moviment"
@@ -187,30 +195,14 @@
 msgid "Add forecast line based on past data."
 msgstr "Afegir línia de previsió sobre la base de dades anteriors."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Previsió completa"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Selecciona productes"
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr "Completa"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "Cancel·la"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Selecciona dates"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Complet"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancel·la"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/cs.po` & `trytond_stock_forecast-6.8.0/locale/it.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr ""
+msgstr "Attivo"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr ""
+msgstr "Azienda"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "Data Inizio"
 
+#, fuzzy
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Righe"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr ""
+msgstr "Stato"
 
+#, fuzzy
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "a data"
 
+#, fuzzy
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
+msgstr "Luogo"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Azienda"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "Data Inizio"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Prodotto"
 
+#, fuzzy
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "a data"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Forecasts"
 
@@ -55,66 +76,71 @@
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr ""
+msgstr "Movimenti"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Prodotto"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr ""
+msgstr "Categotia UdM prodotto"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Quantità"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr ""
+msgstr "UdM"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr ""
+msgstr "Movimento"
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "Tutti"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Done"
+msgstr "Fatto"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Bozza"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
@@ -124,15 +150,15 @@
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Annulla"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
 msgstr "Confirm"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
@@ -156,69 +182,45 @@
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "Annullato"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Done"
+msgstr "Fatto"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Bozza"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancel"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancel"
+msgstr "Annulla"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/locale/de.po` & `trytond_stock_forecast-6.8.0/locale/es.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,220 +1,208 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Aktiv"
+msgstr "Activo"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Unternehmen"
+msgstr "Empresa"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Bestimmungsort"
+msgstr "Destino"
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Von Datum"
+msgstr "Desde la fecha"
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Positionen"
+msgstr "Líneas"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "Status"
+msgstr "Estado"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Bis Datum"
+msgstr "Hasta la fecha"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Ort"
+msgstr "Ubicación"
+
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Empresa"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Destino"
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Von Datum"
+msgstr "Desde la fecha"
+
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Productos"
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Bis Datum"
+msgstr "Hasta la fecha"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Artikel"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr "Almacén"
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Bedarfsprognose"
+msgstr "Previsión"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr "Prognosestatus"
+msgstr "Estado de la previsión"
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Minimale Anzahl"
+msgstr "Cantidad mínima"
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Warenbewegungen"
+msgstr "Movimientos"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Artikel"
+msgstr "Producto"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Maßeinheitenkategorie"
+msgstr "Categoría UdM del producto"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Menge"
+msgstr "Cantidad"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Menge ausgeführt"
+msgstr "Cantidades ejecutadas"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "Maßeinheit"
+msgstr "UdM"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr "Bedarfsprognoseposition"
+msgstr "Línea de previsión"
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Warenbewegung"
+msgstr "Movimiento"
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "Bedarfsprognosen"
+msgstr "Previsiones"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Bedarfsprognose durchführen"
+msgstr "Previsión completa"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "Alle"
+msgstr "Todo"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Erledigt"
+msgstr "Finalizado"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Entwurf"
+msgstr "Borrador"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
-"Die Bedarfsprognosen \"%(first)s\" und \"%(second)s\" überschneiden sich. Es"
-" müssen unterschiedliche Daten verwendet werden."
+"Las previsiones \"%(first)s\" y \"%(second)s\" se solapan, debe usar fechas "
+"diferentes."
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
-msgstr ""
-"Damit die Bedarfsprognose \"%(forecast)s\" gelöscht werden kann, muss sie "
-"zuerst annulliert werden."
+msgstr "Para eliminar la previsión \"%(forecast)s\" debe cancelarla."
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr "Ein Artikel kann nur einmal pro Bedarfsprognose eingetragen werden."
+msgstr "El producto debe ser único en la previsión de existencias."
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Annullieren"
+msgstr "Cancelar"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Bestätigen"
+msgstr "Confirmar"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Entwurf"
+msgstr "Borrador"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "Bedarfsprognosen"
+msgstr "Previsiones"
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Lager Bedarfsprognose"
+msgstr "Previsión de existencias"
 
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Lager Bedarfsprognose"
+msgstr "Previsión de existencias"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Bedarfsprognose durchführen"
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Bedarfsprognose durchführen (Auswahl)"
+msgstr "Previsión completa"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr "Bedarfsprognoseposition"
+msgstr "Línea de previsión de existencias"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr "Bedarfsprognoseposition - Warenbewegung"
+msgstr "Línea de previsión - Movimiento"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Annulliert"
+msgstr "Cancelada"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Erledigt"
+msgstr "Finalizada"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Entwurf"
+msgstr "Borrador"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr ""
-"Erstelle Bedarfsprognosepositionen basierend auf den Werten aus der "
-"Vergangenheit."
+msgstr "Añadir línea de previsión en base a datos anteriores."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Bedarfsprognose durchführen"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Artikel auswählen"
+msgstr "Previsión completa"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr "Durchführen"
+msgstr "Completar"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Abbrechen"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Auswahl Datum"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Durchführen"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Abbrechen"
+msgstr "Cancelar"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/es.po` & `trytond_stock_forecast-6.8.0/locale/fr.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,216 +1,208 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Activo"
+msgstr "Actif"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Destino"
+msgstr "Destination"
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Desde la fecha"
+msgstr "Date de début"
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Líneas"
+msgstr "Lignes"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "État"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Hasta la fecha"
+msgstr "Date de fin"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Ubicación"
+msgstr "Emplacement"
+
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Société"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Destination"
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Desde la fecha"
+msgstr "Date de début"
+
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Produits"
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Hasta la fecha"
+msgstr "Date de fin"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Productos"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr "Entrepôt"
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Previsión"
+msgstr "Prévision"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr "Estado de la previsión"
+msgstr "État de la prévision"
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Cantidad mínima"
+msgstr "Qté minimale"
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Movimientos"
+msgstr "Mouvements"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Producto"
+msgstr "Produit"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Categoría UdM del producto"
+msgstr "Catégorie d'unité de mesure"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Cantidad"
+msgstr "Quantité"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Cantidades ejecutadas"
+msgstr "Quantité exécutée"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "UdM"
+msgstr "UDM"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr "Línea de previsión"
+msgstr "Ligne de prévision"
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Movimiento"
+msgstr "Mouvement"
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "Previsiones"
+msgstr "Prévisions"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Previsión completa"
+msgstr "Compléter la prévision"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Toutes"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Finalizado"
+msgstr "Effectuée"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
-"Las previsiones \"%(first)s\" y \"%(second)s\" se solapan, debe usar fechas "
-"diferentes."
+"Les prévisions « %(first)s » et « %(second)s » se chevauchent, vous devez "
+"utiliser des dates différentes."
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
-msgstr "Para eliminar la previsión \"%(forecast)s\" debe cancelarla."
+msgstr "Pour supprimer la prévision « %(forecast)s », vous devez l'annuler."
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr "El producto debe ser único en la previsión de existencias."
+msgstr "Le produit doit être unique par prévision."
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuler"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Confirmar"
+msgstr "Confirmer"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "Previsiones"
+msgstr "Prévisions"
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Previsión de existencias"
+msgstr "Stock prévisionnel"
 
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Previsión de existencias"
+msgstr "Stock prévisionnel"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Previsión completa"
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Elegir previsión completa"
+msgstr "Completer la prévision - Demander"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr "Línea de previsión de existencias"
+msgstr "Ligne de prévision de stock"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr "Línea de previsión - Movimiento"
+msgstr "Ligne de prévision - Mouvement"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancelada"
+msgstr "Annulée"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Finalizada"
+msgstr "Terminée"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Brouillon"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr "Añadir línea de previsión en base a datos anteriores."
+msgstr "Ajouter la ligne des prévisions fondées sur des données historiques."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Previsión completa"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Seleccionar productos"
+msgstr "Completer la prévision"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr "Completar"
+msgstr "Compléter"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancelar"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Seleccionar fechas"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Completar"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuler"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/es_419.po` & `trytond_stock_forecast-6.8.0/locale/lt.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
 msgstr ""
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
 msgstr ""
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
@@ -30,29 +30,43 @@
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Organizacija"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr ""
+msgstr "Forecasts"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
@@ -64,23 +78,23 @@
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Categoría de UdM de producto"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Cantidad ejecutada"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
 msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
@@ -88,32 +102,32 @@
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr ""
+msgstr "Forecasts"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr ""
+msgstr "Complete Forecast"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr ""
+msgstr "Done"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
@@ -121,97 +135,81 @@
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr ""
+msgstr "Confirm"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr ""
+msgstr "Forecasts"
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr ""
+msgstr "Stock Forecast"
 
+#, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr ""
+msgstr "Stock Forecast"
 
+#, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr ""
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr ""
+msgstr "Complete Forecast"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancelar"
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr ""
+msgstr "Done"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
 msgstr ""
 
+#, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
+msgstr "Complete Forecast"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancelar"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Cancel"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_forecast-6.6.0/locale/et.po` & `trytond_stock_forecast-6.8.0/locale/et.po`

 * *Files 3% similar despite different names*

```diff
@@ -30,25 +30,40 @@
 msgid "To Date"
 msgstr "Kuupäevani"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "Asukoht"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Ettevõte"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Sihtkoht"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "Kuupäevast"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Tooted"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "Luupäevani"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Tooted"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Prognoos"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
@@ -154,18 +169,14 @@
 msgid "Stock Forecast"
 msgstr "Laoprognoos"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Täielik prognoos"
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Täielik prognoos"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr "Lao prognoosi rida"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr "Prognoosirida - kanne"
@@ -187,30 +198,14 @@
 msgid "Add forecast line based on past data."
 msgstr ""
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Täielik prognoos"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Vali tooted"
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr "Lõpetatud"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "Tühista"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Määra kuupäevad"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Lõpetatud"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Tühista"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/fa.po` & `trytond_stock_forecast-6.8.0/locale/fa.po`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,40 @@
 msgid "To Date"
 msgstr "تا تاریخ"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "مکان"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "شرکت"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "مقصد"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "از تاریخ"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "محصولات"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "تا تاریخ"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "محصولات"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "پیش بینی"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
@@ -155,18 +170,14 @@
 msgid "Stock Forecast"
 msgstr "پیش بینی موجودی"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "پیش بینی کامل"
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "پیش بینی کامل"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr "سطر پیش بینی موجودی"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr "سطر پیش بینی - جابجایی"
@@ -188,30 +199,14 @@
 msgid "Add forecast line based on past data."
 msgstr "بر اساس داده های گذشته سطر پیش بینی را اضافه کنید."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "پیش بینی کامل"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "انتخاب محصولات"
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr "تکمیل"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "انصراف"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "انتخاب تاریخ ها"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "تکمیل"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "انصراف"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/fi.po` & `trytond_stock_forecast-6.8.0/locale/pl.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,116 +1,135 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr ""
+msgstr "Aktywna"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr ""
+msgstr "Cel"
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "Od dnia"
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Wiersze"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr ""
+msgstr "Stan"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Do dnia"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr ""
+msgstr "Lokalizacja"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Firma"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Cel"
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "Od dnia"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Produkty"
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Do dnia"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Forecasts"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr ""
+msgstr "Minimalna ilość"
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr ""
+msgstr "Ruchy"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produkt"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr ""
+msgstr "Kategoria jm produktu"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Ilość"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr ""
+msgstr "Jm"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
 msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr ""
+msgstr "Ruch"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
 msgstr "All"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
 msgstr "Done"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
@@ -138,54 +157,50 @@
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "Anuluj"
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Done"
+msgstr "Wykonano"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "view:stock.forecast:"
@@ -193,32 +208,14 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancel"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anuluj"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/locale/fr.po` & `trytond_stock_forecast-6.8.0/locale/pt.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,216 +1,218 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Actif"
+msgstr "Ativo"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Empresa"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Destination"
+msgstr "Destino"
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Date de début"
+msgstr "Data de Início"
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Lignes"
+msgstr "Linhas"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "État"
+msgstr "Estado"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Date de fin"
+msgstr "Até a Data"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Emplacement"
+msgstr "Localização"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Empresa"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Destino"
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Date de début"
+msgstr "Desde a Data"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Produtos"
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Date de fin"
+msgstr "Até a Data"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Produits"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Prévision"
+msgstr "Previsão"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr "État de la prévision"
+msgstr "Estado da Previsão"
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Qté minimale"
+msgstr "Qtd Mínima"
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Mouvements"
+msgstr "Movimentações"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Produit"
+msgstr "Produto"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Catégorie d'unité de mesure"
+msgstr "Categoria da UDM do Produto"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Quantité"
+msgstr "Quantidade"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Quantité exécutée"
+msgstr "Quantidade Executada"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "UDM"
+msgstr "UM"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr "Ligne de prévision"
+msgstr "Linha de Previsão"
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Mouvement"
+msgstr "Movimentação"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "Prévisions"
+msgstr "Forecasts"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Compléter la prévision"
+msgstr "Complete Forecast"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "Toutes"
+msgstr "All"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Effectuée"
+msgstr "Done"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
-"Les prévisions « %(first)s » et « %(second)s » se chevauchent, vous devez "
-"utiliser des dates différentes."
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
-msgstr "Pour supprimer la prévision « %(forecast)s », vous devez l'annuler."
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr "Le produit doit être unique par prévision."
+msgstr "O produto deve ser único por previsão"
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Confirmer"
+msgstr "Confirm"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
-msgstr "Utilisateur dans les sociétés"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "Prévisions"
+msgstr "Forecasts"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Stock prévisionnel"
+msgstr "Stock Forecast"
 
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Stock prévisionnel"
+msgstr "Previsão do Estoque"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Completer la prévision - Demander"
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Completer la prévision - Choisir"
+msgstr "Pedir a Previsão Completa"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr "Ligne de prévision de stock"
+msgstr "Linha da Previsão de Estoque"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr "Ligne de prévision - Mouvement"
+msgstr "Linha de Previsão - Movimentação"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Annulée"
+msgstr "Cancelar"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Terminée"
+msgstr "Feito"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Brouillon"
+msgstr "Rascunho"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr "Ajouter la ligne des prévisions fondées sur des données historiques."
+msgstr "Adicionar linha de previsão com base em dados históricos."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Completer la prévision"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Choix des produits"
+msgstr "Completar a Previsão"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr "Compléter"
+msgstr "Completar"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Annuler"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Choix des dates"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Compléter"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Annuler"
+msgstr "Cancelar"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/hu.po` & `trytond_stock_forecast-6.8.0/locale/hu.po`

 * *Files 4% similar despite different names*

```diff
@@ -30,25 +30,40 @@
 msgid "To Date"
 msgstr "Eddig"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "Tárhely"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Cég"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Cél"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "Ettől"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Termékek"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "Eddig"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Termékek"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Előrejelzés"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
@@ -156,19 +171,14 @@
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
@@ -190,30 +200,14 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "Mégse"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Mégse"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/id.po` & `trytond_stock_forecast-6.8.0/locale/id.po`

 * *Files 6% similar despite different names*

```diff
@@ -30,24 +30,38 @@
 msgid "To Date"
 msgstr "Ke Tanggal"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "Lokasi"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Perusahaan"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "Dari Tanggal"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Produk"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "Ke Tanggal"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast_state:"
@@ -153,18 +167,14 @@
 msgid "Stock Forecast"
 msgstr ""
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr ""
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr ""
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
@@ -186,30 +196,14 @@
 msgid "Add forecast line based on past data."
 msgstr ""
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr ""
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "Batal"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Batal"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/it.po` & `trytond_stock_forecast-6.8.0/locale/lo.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Attivo"
+msgstr "ໃຊ້ຢູ່"
 
+#, fuzzy
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "ຫ້ອງການ/ສຳນັກງານ"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Data Inizio"
+msgstr "ແຕ່ວັນທີ"
 
 #, fuzzy
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Righe"
+msgstr "ຮ່ວງ"
 
+#, fuzzy
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "Stato"
+msgstr "ສະຖານະ"
 
 #, fuzzy
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "a data"
+msgstr "ເຖິງວັນທີ"
 
 #, fuzzy
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Luogo"
+msgstr "ບ່ອນຢູ່"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "ຫ້ອງການ/ສຳນັກງານ"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Data Inizio"
+msgstr "ແຕ່ວັນທີ"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "ຜະລິດຕະພັນ"
 
 #, fuzzy
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "a data"
+msgstr "ເຖິງວັນທີ"
 
-#, fuzzy
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Prodotto"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Forecasts"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
@@ -66,68 +81,70 @@
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Movimenti"
+msgstr "ຕັດບັນຊີສາງ"
 
+#, fuzzy
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Prodotto"
+msgstr "ຜະລິດຕະພັນ"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Categotia UdM prodotto"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Quantità"
+msgstr "ຈຳນວນ"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "UdM"
+msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Movimento"
+msgstr "ເຄື່ອນໄຫວ"
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "Tutti"
+msgstr "ທັງໝົດ"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Fatto"
+msgstr "ແລ້ວໆ"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Bozza"
+msgstr "ຮ່າງກຽມ"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
@@ -137,15 +154,15 @@
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
 msgstr "Confirm"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
@@ -169,67 +186,47 @@
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr "ຍົກເລີກ"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Fatto"
+msgstr "ແລ້ວໆ"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Bozza"
+msgstr "ຮ່າງກຽມ"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
-msgctxt "wizard_button:stock.forecast.complete,ask,end:"
-msgid "Cancel"
-msgstr "Annulla"
-
 #, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Scelta date"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
+msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "ຍົກເລີກ"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/lo.po` & `trytond_stock_forecast-6.8.0/locale/sl.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,151 +1,154 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "ໃຊ້ຢູ່"
+msgstr "Aktivno"
 
-#, fuzzy
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "ຫ້ອງການ/ສຳນັກງານ"
+msgstr "Družba"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr ""
+msgstr "Cilj"
 
-#, fuzzy
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "ແຕ່ວັນທີ"
+msgstr "Od"
 
-#, fuzzy
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "ຮ່ວງ"
+msgstr "Postavke"
 
-#, fuzzy
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "ສະຖານະ"
+msgstr "Stanje"
 
-#, fuzzy
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "ເຖິງວັນທີ"
+msgstr "Do"
 
-#, fuzzy
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "ບ່ອນຢູ່"
+msgstr "Lokacija"
 
 #, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Družba"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Cilj"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "ແຕ່ວັນທີ"
+msgstr "Od"
 
 #, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Izdelki"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "ເຖິງວັນທີ"
+msgstr "Do"
 
-#, fuzzy
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "ຜະລິດຕະພັນ"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Forecasts"
+msgstr "Napoved"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr ""
+msgstr "Stanje napovedi"
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr ""
+msgstr "Minimalna količina"
 
-#, fuzzy
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "ຕັດບັນຊີສາງ"
+msgstr "Promet"
 
-#, fuzzy
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "ຜະລິດຕະພັນ"
+msgstr "Izdelek"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr ""
+msgstr "Katerogija ME izdelka"
 
-#, fuzzy
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "ຈຳນວນ"
+msgstr "Količina"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr ""
+msgstr "Izvedena količina"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr ""
+msgstr "ME"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr ""
+msgstr "Postavka napovedi"
 
-#, fuzzy
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "ເຄື່ອນໄຫວ"
+msgstr "Promet"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "ທັງໝົດ"
+msgstr "All"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "ແລ້ວໆ"
+msgstr "Done"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "ຮ່າງກຽມ"
+msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr ""
+msgstr "Izdelek mora biti edinstven po napovedih"
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
@@ -155,88 +158,61 @@
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
 msgstr "Stock Forecast"
 
-#, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Stock Forecast"
+msgstr "Napoved zaloge"
 
-#, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
+msgstr "Izpolnitev napovedi"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr ""
+msgstr "Postavka napovedi zaloge"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr ""
+msgstr "Postavka napovedi - Promet"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "ຍົກເລີກ"
+msgstr "Preklic"
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "ແລ້ວໆ"
+msgstr "Zaključeno"
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "ຮ່າງກຽມ"
+msgstr "V pripravi"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr ""
+msgstr "Dodaj postavko napovedi na osnovi preteklih podatkov."
 
-#, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
+msgstr "Izpolnitev napovedi"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr ""
+msgstr "Zaključi"
 
-#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "ຍົກເລີກ"
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "ເລືອກວັນທີ"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "ຍົກເລີກ"
+msgstr "Prekliči"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/lt.po` & `trytond_stock_forecast-6.8.0/locale/zh_CN.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr ""
+msgstr "启用"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
 msgstr ""
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Forecasts"
 
@@ -95,21 +109,23 @@
 msgid "Forecasts"
 msgstr "Forecasts"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Done"
+msgstr "完成"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
@@ -156,36 +172,31 @@
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "取消"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Done"
+msgstr "完成"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "view:stock.forecast:"
@@ -193,32 +204,15 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancel"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancel"
+msgstr "取消"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/locale/nl.po` & `trytond_stock_forecast-6.8.0/locale/de.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,216 +1,212 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Actief"
+msgstr "Aktiv"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Unternehmen"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Bestemming"
+msgstr "Bestimmungsort"
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Vanaf datum"
+msgstr "Von Datum"
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Regels"
+msgstr "Positionen"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Tot datum"
+msgstr "Bis Datum"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Plaats"
+msgstr "Ort"
+
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Unternehmen"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Bestimmungsort"
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Vanaf datum"
+msgstr "Von Datum"
+
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Artikel"
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Tot datum"
+msgstr "Bis Datum"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Producten"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr "Logistikstandort"
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "prognose"
+msgstr "Bedarfsprognose"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr "prognose status"
+msgstr "Prognosestatus"
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Minimale hoeveelheid"
+msgstr "Minimale Anzahl"
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Mutaties"
+msgstr "Warenbewegungen"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Product"
+msgstr "Artikel"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Poduct maateenheid categorie"
+msgstr "Maßeinheitenkategorie"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Hoeveelheid"
+msgstr "Menge"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Uitgevoerde hoeveelheid (verbruikt?)"
+msgstr "Menge ausgeführt"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "maateenheid"
+msgstr "Maßeinheit"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr "prognose lijn"
+msgstr "Bedarfsprognoseposition"
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Mutatie"
+msgstr "Warenbewegung"
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "voorspellingen"
+msgstr "Bedarfsprognosen"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Prognose voltooien"
+msgstr "Bedarfsprognose durchführen"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
 msgstr "Alle"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Erledigt"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Entwurf"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
-"De prognoses\"%(first)s\" en \"%(second)s\" overlappen elkaar. Verschillende"
-" gegevens moeten worden gebruikt."
+"Die Bedarfsprognosen \"%(first)s\" und \"%(second)s\" überschneiden sich. Es"
+" müssen unterschiedliche Daten verwendet werden."
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
-msgstr "Om voorspelling \"%(forecast)s\"\" te verwijderen, moet u deze annuleren."
+msgstr ""
+"Damit die Bedarfsprognose \"%(forecast)s\" gelöscht werden kann, muss sie "
+"zuerst annulliert werden."
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr "Product moet uniek zijn op basis van prognose."
+msgstr "Ein Artikel kann nur einmal pro Bedarfsprognose eingetragen werden."
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Annuleren"
+msgstr "Annullieren"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Bevestigen"
+msgstr "Bestätigen"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Entwurf"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
-msgstr "Gebruiker in het bedrijf"
+msgstr "Benutzer im Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "prognose"
+msgstr "Bedarfsprognosen"
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Stock prognose"
+msgstr "Lager Bedarfsprognose"
 
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Stock prognose"
+msgstr "Lager Bedarfsprognose"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Prognose voltooien"
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Prognose voltooien"
+msgstr "Bedarfsprognose durchführen"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr "Stock prognose lijn"
+msgstr "Bedarfsprognoseposition"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr "Prognose lijn - Mutatie"
+msgstr "Bedarfsprognoseposition - Warenbewegung"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Geannuleerd"
+msgstr "Annulliert"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Klaar"
+msgstr "Erledigt"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Concept"
+msgstr "Entwurf"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr "prognosesregel toevoegen op basis van gegevens uit het verleden."
+msgstr ""
+"Erstelle Bedarfsprognosepositionen basierend auf den Werten aus der "
+"Vergangenheit."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Prognose voltooien"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Kies producten"
+msgstr "Bedarfsprognose durchführen"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr "Voltooien"
+msgstr "Durchführen"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Annuleren"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Kies datums"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Voltooien"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Annuleren"
+msgstr "Abbrechen"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/locale/pl.po` & `trytond_stock_forecast-6.8.0/locale/cs.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,128 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Aktywna"
+msgstr ""
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr ""
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Cel"
+msgstr ""
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Od dnia"
+msgstr ""
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Wiersze"
+msgstr ""
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "Stan"
+msgstr ""
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Do dnia"
+msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Lokalizacja"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Od dnia"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Do dnia"
+msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Produkty"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Forecasts"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Minimalna ilość"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Ruchy"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Produkt"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Kategoria jm produktu"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Ilość"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "Jm"
+msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
 msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Ruch"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
 msgstr "All"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
 msgstr "Done"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
@@ -142,55 +150,49 @@
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
 msgstr "Stock Forecast"
 
 #, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Anuluj"
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Wykonano"
+msgstr "Done"
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "view:stock.forecast:"
@@ -198,30 +200,15 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Wybierz produkty"
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Anuluj"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Wybierz daty"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Anuluj"
+msgstr "Cancel"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_forecast-6.6.0/locale/pt.po` & `trytond_stock_forecast-6.8.0/locale/nl.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,223 +1,208 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Ativo"
+msgstr "Actief"
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Bedrijf"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Destino"
+msgstr "Bestemming"
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Data de Início"
+msgstr "Vanaf datum"
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Linhas"
+msgstr "Regels"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Status"
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Até a Data"
+msgstr "Tot datum"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Localização"
+msgstr "Plaats"
+
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Bedrijf"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Bestemming"
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Desde a Data"
+msgstr "Vanaf datum"
+
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Producten"
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Até a Data"
+msgstr "Tot datum"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Produtos"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr "Magazijn"
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Previsão"
+msgstr "prognose"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr "Estado da Previsão"
+msgstr "prognose status"
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Qtd Mínima"
+msgstr "Minimale hoeveelheid"
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Movimentações"
+msgstr "Mutaties"
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Produto"
+msgstr "Product"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Categoria da UDM do Produto"
+msgstr "Poduct maateenheid categorie"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Quantidade"
+msgstr "Hoeveelheid"
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Quantidade Executada"
+msgstr "Uitgevoerde hoeveelheid (verbruikt?)"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "UM"
+msgstr "maateenheid"
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr "Linha de Previsão"
+msgstr "prognose lijn"
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Movimentação"
+msgstr "Mutatie"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "Forecasts"
+msgstr "voorspellingen"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
+msgstr "Prognose voltooien"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "Alle"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Done"
+msgstr "Klaar"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Concept"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
+"De prognoses\"%(first)s\" en \"%(second)s\" overlappen elkaar. Verschillende"
+" gegevens moeten worden gebruikt."
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
-msgstr ""
+msgstr "Om voorspelling \"%(forecast)s\"\" te verwijderen, moet u deze annuleren."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr "O produto deve ser único por previsão"
+msgstr "Product moet uniek zijn op basis van prognose."
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Annuleren"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Confirm"
+msgstr "Bevestigen"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Concept"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Gebruiker in het bedrijf"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "Forecasts"
+msgstr "prognose"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Stock Forecast"
+msgstr "Stock prognose"
 
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Previsão do Estoque"
+msgstr "Stock prognose"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Pedir a Previsão Completa"
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Escolher a Previsão Completa"
+msgstr "Prognose voltooien"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr "Linha da Previsão de Estoque"
+msgstr "Stock prognose lijn"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr "Linha de Previsão - Movimentação"
+msgstr "Prognose lijn - Mutatie"
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancelar"
+msgstr "Geannuleerd"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Feito"
+msgstr "Klaar"
 
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Rascunho"
+msgstr "Concept"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr "Adicionar linha de previsão com base em dados históricos."
+msgstr "prognosesregel toevoegen op basis van gegevens uit het verleden."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Completar a Previsão"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Escolher os Produtos"
+msgstr "Prognose voltooien"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr "Completar"
+msgstr "Voltooien"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancelar"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Escolher Datas"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Concluída"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Annuleren"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_forecast-6.6.0/locale/ro.po` & `trytond_stock_forecast-6.8.0/locale/fi.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,55 +4,68 @@
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
 msgstr ""
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
 msgstr ""
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr ""
+msgstr "Forecasts"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
@@ -60,15 +73,15 @@
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
@@ -88,32 +101,32 @@
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr ""
+msgstr "Forecasts"
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr ""
+msgstr "Complete Forecast"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr ""
+msgstr "Done"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
@@ -123,92 +136,79 @@
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr ""
+msgstr "Confirm"
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr ""
+msgstr "Forecasts"
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr ""
+msgstr "Stock Forecast"
 
+#, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr ""
+msgstr "Stock Forecast"
 
+#, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr ""
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr ""
+msgstr "Complete Forecast"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr ""
+msgstr "Done"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
 msgstr ""
 
+#, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
+msgstr "Complete Forecast"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_forecast-6.6.0/locale/ru.po` & `trytond_stock_forecast-6.8.0/locale/ru.po`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,40 @@
 msgid "To Date"
 msgstr "Конечная дата"
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr "Местоположение"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Организация"
+
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr "Назначение"
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr "Начальная дата"
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Продукция"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr "Конечная дата"
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Продукция"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr "Прогноз"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
@@ -162,18 +177,14 @@
 msgid "Stock Forecast"
 msgstr "Прогноз по складу"
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr "Завершить прогноз"
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Завершить прогноз"
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr "Строка прогноза по складу"
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr "Строка прогноза - Перемещение"
@@ -195,30 +206,14 @@
 msgid "Add forecast line based on past data."
 msgstr "Добавить строчку прогноза основанного на предыдущих данных."
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr "Завершить прогноз"
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Выбрать продукты"
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr "Завершить"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr "Отменить"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Выбрать даты"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Завершить"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Отменить"
```

### Comparing `trytond_stock_forecast-6.6.0/locale/sl.po` & `trytond_stock_forecast-6.8.0/locale/tr.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,128 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "Aktivno"
+msgstr ""
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
-msgstr "Cilj"
+msgstr ""
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
-msgstr "Od"
+msgstr ""
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr "Postavke"
+msgstr ""
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr ""
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
-msgstr "Do"
+msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
-msgstr "Lokacija"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
 
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
-msgstr "Od"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
 
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
-msgstr "Do"
+msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
-msgstr "Izdelki"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Napoved"
+msgstr "Forecasts"
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
-msgstr "Stanje napovedi"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
-msgstr "Minimalna količina"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
-msgstr "Promet"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr "Izdelek"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr "Katerogija ME izdelka"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
-msgstr "Količina"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr "Izvedena količina"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
-msgstr "ME"
+msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
-msgstr "Postavka napovedi"
+msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
-msgstr "Promet"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
 msgstr "Complete Forecast"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
 msgstr "All"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
 msgstr "Done"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
@@ -122,18 +130,17 @@
 "different dates."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_forecast_delete_cancel"
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
-msgstr "Izdelek mora biti edinstven po napovedih"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
 msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
@@ -143,81 +150,65 @@
 msgid "Draft"
 msgstr "Draft"
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
 msgstr "Forecasts"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
 msgstr "Stock Forecast"
 
+#, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Napoved zaloge"
+msgstr "Stock Forecast"
 
+#, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Izpolnitev napovedi"
-
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Izpolnitev napovedi"
+msgstr "Complete Forecast"
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
-msgstr "Postavka napovedi zaloge"
+msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
-msgstr "Postavka napovedi - Promet"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Preklic"
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Zaključeno"
+msgstr "Done"
 
+#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "V pripravi"
+msgstr "Draft"
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
-msgstr "Dodaj postavko napovedi na osnovi preteklih podatkov."
+msgstr ""
 
+#, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Izpolnitev napovedi"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr "Izberi izdelke"
+msgstr "Complete Forecast"
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
-msgstr "Zaključi"
+msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Prekliči"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr "Izberi datume"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr "Zaključi"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Cancel"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_forecast-6.6.0/locale/tr.po` & `trytond_stock_forecast-6.8.0/locale/es_419.po`

 * *Files 13% similar despite different names*

```diff
@@ -30,30 +30,41 @@
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Forecasts"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
@@ -65,23 +76,23 @@
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
-msgstr ""
+msgstr "Categoría de UdM de producto"
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity_executed:"
 msgid "Quantity Executed"
-msgstr ""
+msgstr "Cantidad ejecutada"
 
 msgctxt "field:stock.forecast.line,uom:"
 msgid "UOM"
 msgstr ""
 
 msgctxt "field:stock.forecast.line-stock.move,line:"
 msgid "Forecast Line"
@@ -89,32 +100,32 @@
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "Forecasts"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "Done"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
@@ -122,103 +133,77 @@
 msgid "To delete forecast \"%(forecast)s\" you must cancel it."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Cancelar"
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Confirm"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "Forecasts"
+msgstr ""
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Stock Forecast"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Stock Forecast"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
+msgstr ""
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr "Cancelar"
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "Done"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
 msgstr ""
 
-#, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
 msgstr ""
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
 #, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "Cancel"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "Cancel"
+msgstr "Cancelar"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/locale/uk.po` & `trytond_stock_forecast-6.8.0/locale/ro.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,50 +4,64 @@
 
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
 msgstr ""
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
 msgstr ""
 
 msgctxt "field:stock.forecast,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Rânduri"
 
 msgctxt "field:stock.forecast,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr "Companie"
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr "Produs"
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast_state:"
@@ -60,15 +74,15 @@
 
 msgctxt "field:stock.forecast.line,moves:"
 msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:stock.forecast.line,product_uom_category:"
 msgid "Product Uom Category"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,quantity:"
 msgid "Quantity"
@@ -153,18 +167,14 @@
 msgid "Stock Forecast"
 msgstr ""
 
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
 msgstr ""
 
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr ""
-
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
@@ -185,30 +195,14 @@
 msgid "Add forecast line based on past data."
 msgstr ""
 
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
 msgstr ""
 
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
-msgstr ""
-
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
 msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/locale/zh_CN.po` & `trytond_stock_forecast-6.8.0/locale/uk.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:stock.forecast,active:"
 msgid "Active"
-msgstr "启用"
+msgstr ""
 
 msgctxt "field:stock.forecast,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:stock.forecast,destination:"
 msgid "Destination"
@@ -19,43 +18,53 @@
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.forecast,state:"
 msgid "State"
-msgstr "状态"
+msgstr ""
 
 msgctxt "field:stock.forecast,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:stock.forecast,warehouse:"
 msgid "Location"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,company:"
+msgid "Company"
+msgstr ""
+
+msgctxt "field:stock.forecast.complete.ask,destination:"
+msgid "Destination"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,from_date:"
 msgid "From Date"
 msgstr ""
 
+msgctxt "field:stock.forecast.complete.ask,products:"
+msgid "Products"
+msgstr ""
+
 msgctxt "field:stock.forecast.complete.ask,to_date:"
 msgid "To Date"
 msgstr ""
 
-msgctxt "field:stock.forecast.complete.choose,products:"
-msgid "Products"
+msgctxt "field:stock.forecast.complete.ask,warehouse:"
+msgid "Warehouse"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.forecast.line,forecast:"
 msgid "Forecast"
-msgstr "Forecasts"
+msgstr ""
 
 msgctxt "field:stock.forecast.line,forecast_state:"
 msgid "Forecast State"
 msgstr ""
 
 msgctxt "field:stock.forecast.line,minimal_quantity:"
 msgid "Minimal Qty"
@@ -91,34 +100,32 @@
 
 msgctxt "field:stock.forecast.line-stock.move,move:"
 msgid "Move"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_forecast_form"
 msgid "Forecasts"
-msgstr "Forecasts"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_forecast_complete"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_forecast_form_domain_done"
 msgid "Done"
-msgstr "完成"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_forecast_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_forecast_date_overlap"
 msgid ""
 "The forecasts \"%(first)s\" and \"%(second)s\" overlap, you must use "
 "different dates."
 msgstr ""
 
@@ -128,101 +135,72 @@
 
 msgctxt "model:ir.message,text:msg_forecast_line_product_unique"
 msgid "Product must be unique by forecast."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_confirm_button"
 msgid "Confirm"
-msgstr "Confirm"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:forecast_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_forecast_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_forecast_form"
 msgid "Forecasts"
-msgstr "Forecasts"
+msgstr ""
 
 msgctxt "model:res.group,name:group_stock_forecast"
 msgid "Stock Forecast"
-msgstr "Stock Forecast"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.forecast,name:"
 msgid "Stock Forecast"
-msgstr "Stock Forecast"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.forecast.complete.ask,name:"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
-#, fuzzy
-msgctxt "model:stock.forecast.complete.choose,name:"
-msgid "Complete Forecast"
-msgstr "Complete Forecast"
+msgstr ""
 
 msgctxt "model:stock.forecast.line,name:"
 msgid "Stock Forecast Line"
 msgstr ""
 
 msgctxt "model:stock.forecast.line-stock.move,name:"
 msgid "ForecastLine - Move"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Cancelled"
-msgstr "取消"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Done"
-msgstr "完成"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:stock.forecast,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "view:stock.forecast:"
 msgid "Add forecast line based on past data."
 msgstr ""
 
-#, fuzzy
 msgctxt "view:stock.forecast:"
 msgid "Complete Forecast"
-msgstr "Complete Forecast"
-
-msgctxt "wizard_button:stock.forecast.complete,ask,choose:"
-msgid "Choose Products"
 msgstr ""
 
 msgctxt "wizard_button:stock.forecast.complete,ask,complete:"
 msgid "Complete"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:stock.forecast.complete,ask,end:"
 msgid "Cancel"
-msgstr "取消"
-
-msgctxt "wizard_button:stock.forecast.complete,choose,ask:"
-msgid "Choose Dates"
 msgstr ""
-
-msgctxt "wizard_button:stock.forecast.complete,choose,complete:"
-msgid "Complete"
-msgstr ""
-
-#, fuzzy
-msgctxt "wizard_button:stock.forecast.complete,choose,end:"
-msgid "Cancel"
-msgstr "取消"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_forecast-6.6.0/message.xml` & `trytond_stock_forecast-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-6.6.0/setup.py` & `trytond_stock_forecast-6.8.0/setup.py`

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
@@ -34,59 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_forecast'
 
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
 
 requires = ['python-dateutil', 'python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module with stock forecasts',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_forecast',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock forecast',
     package_dir={'trytond.modules.stock_forecast': '.'},
     packages=(
         ['trytond.modules.stock_forecast']
         + ['trytond.modules.stock_forecast.%s' % p for p in find_packages()]
         ),
@@ -123,24 +100,23 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     stock_forecast = trytond.modules.stock_forecast
     """,
     )
```

### Comparing `trytond_stock_forecast-6.6.0/tests/test_module.py` & `trytond_stock_forecast-6.8.0/tests/test_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,48 @@
 
 from dateutil.relativedelta import relativedelta
 
 from trytond.modules.company.tests import (
     CompanyTestMixin, create_company, set_company)
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 
 class StockForecastTestCase(CompanyTestMixin, ModuleTestCase):
     'Test StockForecast module'
     module = 'stock_forecast'
 
     @with_transaction()
+    def test_forecast_rec_name(self):
+        pool = Pool()
+        Forecast = pool.get('stock.forecast')
+        Location = pool.get('stock.location')
+
+        customer, = Location.search([('code', '=', 'CUS')])
+        warehouse, = Location.search([('code', '=', 'WH')])
+        storage, = Location.search([('code', '=', 'STO')])
+        company = create_company()
+        with set_company(company):
+            forecast = Forecast(
+                warehouse=warehouse,
+                destination=customer,
+                from_date=datetime.date(2023, 1, 1),
+                to_date=datetime.date(2023, 3, 31),
+                )
+            forecast.save()
+            with inactive_records():
+                forecasts = Forecast.search([('rec_name', '=', "Warehouse")])
+
+            self.assertEqual(
+                forecast.rec_name,
+                "Warehouse → Customer @ [01/01/2023 - 03/31/2023]")
+            self.assertEqual(forecasts, [forecast])
+
+    @with_transaction()
     def test_distribute(self):
         'Test distribute'
         pool = Pool()
         Line = pool.get('stock.forecast.line')
         line = Line()
         for values, result in (
                 ((1, 5), {0: 5}),
@@ -300,18 +326,22 @@
                         'company': company.id,
                         }])
 
             with Transaction().set_context(
                     active_model=Forecast.__name__, active_id=forecast.id):
                 session_id, _, _ = ForecastComplete.create()
                 forecast_complete = ForecastComplete(session_id)
+                forecast_complete.ask.company = company
+                forecast_complete.ask.warehouse = warehouse
+                forecast_complete.ask.destination = customer
                 forecast_complete.ask.from_date = (
                     today + relativedelta(months=-1, day=1))
                 forecast_complete.ask.to_date = (
                     today + relativedelta(months=-1, day=20))
+                forecast_complete.ask.products = [product]
                 forecast_complete.transition_complete()
 
             self.assertEqual(len(forecast.lines), 1)
             forecast_line, = forecast.lines
             self.assertEqual(forecast_line.product, product)
             self.assertEqual(forecast_line.uom, unit)
             self.assertEqual(forecast_line.quantity, 5)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/PKG-INFO` & `trytond_stock_forecast-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-forecast
-Version: 6.6.0
+Name: trytond_stock_forecast
+Version: 6.8.0
 Summary: Tryton module with stock forecasts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_forecast
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock forecast
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
 License-File: LICENSE
 
 Stock Forecast Module
 #####################
 
 The stock forecast module provide a simple way to create stock moves
 toward customers with a date in the future. This allow other stock
```

### Comparing `trytond_stock_forecast-6.6.0/trytond_stock_forecast.egg-info/SOURCES.txt` & `trytond_stock_forecast-6.8.0/trytond_stock_forecast.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
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
 forecast.py
 forecast.xml
 message.xml
+product.xml
 setup.py
 tox.ini
 tryton.cfg
 ./__init__.py
 ./exceptions.py
 ./forecast.py
 ./forecast.xml
 ./message.xml
+./product.xml
 ./tryton.cfg
 ./locale/bg.po
 ./locale/ca.po
 ./locale/cs.po
 ./locale/de.po
 ./locale/es.po
 ./locale/es_419.po
@@ -44,19 +42,20 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/forecast_complete_ask_form.xml
-./view/forecast_complete_choose_form.xml
 ./view/forecast_form.xml
 ./view/forecast_line_form.xml
 ./view/forecast_line_tree.xml
 ./view/forecast_tree.xml
+./view/product_list_forecast.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -84,12 +83,12 @@
 trytond_stock_forecast.egg-info/SOURCES.txt
 trytond_stock_forecast.egg-info/dependency_links.txt
 trytond_stock_forecast.egg-info/entry_points.txt
 trytond_stock_forecast.egg-info/not-zip-safe
 trytond_stock_forecast.egg-info/requires.txt
 trytond_stock_forecast.egg-info/top_level.txt
 view/forecast_complete_ask_form.xml
-view/forecast_complete_choose_form.xml
 view/forecast_form.xml
 view/forecast_line_form.xml
 view/forecast_line_tree.xml
-view/forecast_tree.xml
+view/forecast_tree.xml
+view/product_list_forecast.xml
```

### Comparing `trytond_stock_forecast-6.6.0/view/forecast_form.xml` & `trytond_stock_forecast-6.8.0/view/forecast_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_forecast-6.6.0/view/forecast_line_form.xml` & `trytond_stock_forecast-6.8.0/view/forecast_line_form.xml`

 * *Files identical despite different names*

