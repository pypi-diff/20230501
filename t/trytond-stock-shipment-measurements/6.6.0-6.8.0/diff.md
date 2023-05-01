# Comparing `tmp/trytond_stock_shipment_measurements-6.6.0.tar.gz` & `tmp/trytond_stock_shipment_measurements-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_shipment_measurements-6.6.0.tar", last modified: Mon Oct 31 16:29:58 2022, max compression
+gzip compressed data, was "trytond_stock_shipment_measurements-6.8.0.tar", last modified: Mon May  1 12:06:44 2023, max compression
```

## Comparing `trytond_stock_shipment_measurements-6.6.0.tar` & `trytond_stock_shipment_measurements-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:58.343777 trytond_stock_shipment_measurements-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_stock_shipment_measurements-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_shipment_measurements-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2022-10-31 16:29:57.000000 trytond_stock_shipment_measurements-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_shipment_measurements-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1115 2022-10-31 16:29:56.000000 trytond_stock_shipment_measurements-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:29:55.000000 trytond_stock_shipment_measurements-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:20.000000 trytond_stock_shipment_measurements-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_shipment_measurements-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2410 2022-10-31 16:29:58.343777 trytond_stock_shipment_measurements-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2018-08-18 09:55:20.000000 trytond_stock_shipment_measurements-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:58.340444 trytond_stock_shipment_measurements-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2018-08-18 09:55:20.000000 trytond_stock_shipment_measurements-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:58.337110 trytond_stock_shipment_measurements-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6683 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6899 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6883 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6508 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7157 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6834 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6954 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6828 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6741 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5503 2022-10-29 07:50:48.000000 trytond_stock_shipment_measurements-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:29:58.343777 trytond_stock_shipment_measurements-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5226 2022-10-29 07:39:12.000000 trytond_stock_shipment_measurements-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16978 2022-04-10 15:40:36.000000 trytond_stock_shipment_measurements-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5104 2022-10-11 19:49:59.000000 trytond_stock_shipment_measurements-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:58.337110 trytond_stock_shipment_measurements-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_shipment_measurements-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8075 2022-04-16 16:30:57.000000 trytond_stock_shipment_measurements-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2022-10-31 15:10:09.000000 trytond_stock_shipment_measurements-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2022-10-31 16:29:54.000000 trytond_stock_shipment_measurements-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:58.343777 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2410 2022-10-31 16:29:57.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1865 2022-10-31 16:29:58.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:29:57.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2022-10-31 16:29:57.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:16.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      173 2022-10-31 16:29:57.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:29:57.000000 trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:58.340444 trytond_stock_shipment_measurements-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/view/package_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/view/package_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/view/package_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/view/shipment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2022-04-08 16:24:28.000000 trytond_stock_shipment_measurements-6.6.0/view/shipment_form_package.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2022-04-08 16:23:27.000000 trytond_stock_shipment_measurements-6.6.0/view/shipment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-04-08 16:24:28.000000 trytond_stock_shipment_measurements-6.6.0/view/shipment_list_package.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2022-10-11 19:49:59.000000 trytond_stock_shipment_measurements-6.6.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:44.711134 trytond_stock_shipment_measurements-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1278 2023-05-01 11:18:25.000000 trytond_stock_shipment_measurements-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:18:24.000000 trytond_stock_shipment_measurements-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_shipment_measurements-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2390 2023-05-01 12:06:44.711134 trytond_stock_shipment_measurements-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-01-16 14:00:21.000000 trytond_stock_shipment_measurements-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:44.707800 trytond_stock_shipment_measurements-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-01-16 14:00:21.000000 trytond_stock_shipment_measurements-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:44.704467 trytond_stock_shipment_measurements-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6683 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6899 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6883 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6508 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7157 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6834 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6954 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6828 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6741 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5503 2023-04-29 08:02:54.000000 trytond_stock_shipment_measurements-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:06:44.711134 trytond_stock_shipment_measurements-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4388 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16978 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5104 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:44.704467 trytond_stock_shipment_measurements-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8180 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-05-01 11:18:19.000000 trytond_stock_shipment_measurements-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:44.711134 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2390 2023-05-01 12:06:43.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1839 2023-05-01 12:06:44.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:06:43.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-05-01 12:06:43.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      173 2023-05-01 12:06:43.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:06:43.000000 trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:44.707800 trytond_stock_shipment_measurements-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/package_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/package_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/package_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/shipment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/shipment_form_package.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/shipment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/shipment_list_package.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_stock_shipment_measurements-6.8.0/view/stock_move_form.xml
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/CHANGELOG` & `trytond_stock_shipment_measurements-6.8.0/CHANGELOG`

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
 * Use configured unit for measurements
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/COPYRIGHT` & `trytond_stock_shipment_measurements-6.8.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2022 Cédric Krier
-Copyright (C) 2017-2022 B2CK
+Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/LICENSE` & `trytond_stock_shipment_measurements-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/PKG-INFO` & `trytond_stock_shipment_measurements-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_shipment_measurements
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add measurements to shipment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_shipment_measurements
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock shipment measurement
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Stock Shipment Measurements Module
 ##################################
 
 The Stock Shipment Measurements module adds weight and volume on shipments and
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/__init__.py` & `trytond_stock_shipment_measurements-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/bg.po` & `trytond_stock_shipment_measurements-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/ca.po` & `trytond_stock_shipment_measurements-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/cs.po` & `trytond_stock_shipment_measurements-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/de.po` & `trytond_stock_shipment_measurements-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/es.po` & `trytond_stock_shipment_measurements-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/es_419.po` & `trytond_stock_shipment_measurements-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/et.po` & `trytond_stock_shipment_measurements-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/fa.po` & `trytond_stock_shipment_measurements-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/fi.po` & `trytond_stock_shipment_measurements-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/fr.po` & `trytond_stock_shipment_measurements-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/hu.po` & `trytond_stock_shipment_measurements-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/id.po` & `trytond_stock_shipment_measurements-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/it.po` & `trytond_stock_shipment_measurements-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/lo.po` & `trytond_stock_shipment_measurements-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/lt.po` & `trytond_stock_shipment_measurements-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/nl.po` & `trytond_stock_shipment_measurements-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/pl.po` & `trytond_stock_shipment_measurements-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/pt.po` & `trytond_stock_shipment_measurements-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/ro.po` & `trytond_stock_shipment_measurements-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/ru.po` & `trytond_stock_shipment_measurements-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/sl.po` & `trytond_stock_shipment_measurements-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/tr.po` & `trytond_stock_shipment_measurements-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/uk.po` & `trytond_stock_shipment_measurements-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/locale/zh_CN.po` & `trytond_stock_shipment_measurements-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/setup.py` & `trytond_stock_shipment_measurements-6.8.0/setup.py`

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
@@ -34,61 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_shipment_measurements'
 
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
 
 tests_require = [get_require_version('trytond_stock_package')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add measurements to shipment',
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
-            'https://hg.tryton.org/modules/stock_shipment_measurements'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock shipment measurement',
     package_dir={'trytond.modules.stock_shipment_measurements': '.'},
     packages=(
         ['trytond.modules.stock_shipment_measurements']
         + ['trytond.modules.stock_shipment_measurements.%s' % p
             for p in find_packages()]
@@ -124,27 +101,26 @@
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
     stock_shipment_measurements = trytond.modules.stock_shipment_measurements
     """,
     )
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/stock.py` & `trytond_stock_shipment_measurements-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/stock.xml` & `trytond_stock_shipment_measurements-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_measurements-6.6.0/tests/test_module.py` & `trytond_stock_shipment_measurements-6.8.0/tests/test_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
                     'template': template.id,
                     }])
 
         with set_company(company):
             shipment = Shipment()
             shipment.customer = party
             shipment.delivery_address, = party.addresses
+            shipment.warehouse = Shipment.default_warehouse()
+            shipment.on_change_warehouse()
             shipment.save()
 
             # without moves
             self.assertEqual(shipment.weight, None)
             self.assertEqual(shipment.volume, None)
 
             shipment.moves = [Move(
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/PKG-INFO` & `trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-shipment-measurements
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add measurements to shipment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_shipment_measurements
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock shipment measurement
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Stock Shipment Measurements Module
 ##################################
 
 The Stock Shipment Measurements module adds weight and volume on shipments and
```

### Comparing `trytond_stock_shipment_measurements-6.6.0/trytond_stock_shipment_measurements.egg-info/SOURCES.txt` & `trytond_stock_shipment_measurements-6.8.0/trytond_stock_shipment_measurements.egg-info/SOURCES.txt`

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
 setup.py
@@ -48,14 +44,15 @@
 ./view/package_list.xml
 ./view/package_tree.xml
 ./view/shipment_form.xml
 ./view/shipment_form_package.xml
 ./view/shipment_list.xml
 ./view/shipment_list_package.xml
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

### Comparing `trytond_stock_shipment_measurements-6.6.0/view/configuration_form.xml` & `trytond_stock_shipment_measurements-6.8.0/view/configuration_form.xml`

 * *Files identical despite different names*

