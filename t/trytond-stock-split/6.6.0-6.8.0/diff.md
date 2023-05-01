# Comparing `tmp/trytond_stock_split-6.6.0.tar.gz` & `tmp/trytond_stock_split-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_split-6.6.0.tar", last modified: Mon Oct 31 15:58:25 2022, max compression
+gzip compressed data, was "trytond_stock_split-6.8.0.tar", last modified: Mon May  1 11:46:28 2023, max compression
```

## Comparing `trytond_stock_split-6.6.0.tar` & `trytond_stock_split-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_stock_split-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_split-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-31 15:58:24.000000 trytond_stock_split-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_split-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2022-10-31 15:58:23.000000 trytond_stock_split-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:58:23.000000 trytond_stock_split-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:44.000000 trytond_stock_split-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_split-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2733 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2019-06-04 16:49:46.000000 trytond_stock_split-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      572 2021-12-11 16:59:34.000000 trytond_stock_split-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2019-06-04 16:49:46.000000 trytond_stock_split-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:44.000000 trytond_stock_split-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2019-10-11 21:49:57.000000 trytond_stock_split-6.6.0/icons/tryton-stock-split.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.539115 trytond_stock_split-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2213 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2275 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2282 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1944 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2083 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2514 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2339 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2176 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1948 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2132 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2303 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2293 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2102 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2306 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1927 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2142 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1927 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2085 2022-10-29 07:50:37.000000 trytond_stock_split-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5156 2022-10-29 07:39:12.000000 trytond_stock_split-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6493 2022-04-10 15:40:36.000000 trytond_stock_split-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4342 2020-08-14 21:16:39.000000 trytond_stock_split-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.539115 trytond_stock_split-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_split-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2603 2022-09-29 07:07:38.000000 trytond_stock_split-6.6.0/tests/scenario_stock_split_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3282 2022-04-16 16:30:57.000000 trytond_stock_split-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_split-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2022-10-31 15:10:09.000000 trytond_stock_split-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 15:58:22.000000 trytond_stock_split-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2733 2022-10-31 15:58:24.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1751 2022-10-31 15:58:25.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:58:24.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2022-10-31 15:58:24.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:56.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 15:58:24.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:58:24.000000 trytond_stock_split-6.6.0/trytond_stock_split.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:25.542448 trytond_stock_split-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2019-10-11 21:49:57.000000 trytond_stock_split-6.6.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2019-02-13 10:09:44.000000 trytond_stock_split-6.6.0/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2019-06-04 16:49:46.000000 trytond_stock_split-6.6.0/view/shipment_split_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2020-07-08 22:22:01.000000 trytond_stock_split-6.6.0/view/shipment_split_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2019-02-13 10:09:44.000000 trytond_stock_split-6.6.0/view/split_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.912713 trytond_stock_split-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-05-01 11:04:22.000000 trytond_stock_split-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:04:22.000000 trytond_stock_split-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_split-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2729 2023-05-01 11:46:28.912713 trytond_stock_split-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-01-16 14:00:21.000000 trytond_stock_split-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.909379 trytond_stock_split-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-01-16 14:00:21.000000 trytond_stock_split-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.909379 trytond_stock_split-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/icons/tryton-stock-split.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.906046 trytond_stock_split-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2213 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1944 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2083 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2514 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2339 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2176 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1948 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2132 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2303 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2293 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2102 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2306 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1927 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2142 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1927 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2085 2023-04-29 08:02:44.000000 trytond_stock_split-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:46:28.912713 trytond_stock_split-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4349 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6493 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4342 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.909379 trytond_stock_split-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2591 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/tests/scenario_stock_split_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3282 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:04:16.000000 trytond_stock_split-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.912713 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2729 2023-05-01 11:46:28.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1725 2023-05-01 11:46:28.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:46:28.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-01 11:46:28.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:46:28.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:46:28.000000 trytond_stock_split-6.8.0/trytond_stock_split.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:28.909379 trytond_stock_split-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 trytond_stock_split-6.8.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-01-16 14:00:21.000000 trytond_stock_split-6.8.0/view/shipment_split_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_stock_split-6.8.0/view/shipment_split_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 trytond_stock_split-6.8.0/view/split_start_form.xml
```

### Comparing `trytond_stock_split-6.6.0/CHANGELOG` & `trytond_stock_split-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_stock_split-6.6.0/COPYRIGHT` & `trytond_stock_split-6.8.0/COPYRIGHT`

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

### Comparing `trytond_stock_split-6.6.0/LICENSE` & `trytond_stock_split-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/PKG-INFO` & `trytond_stock_split-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_split
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to split stock move
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_split
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock split
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
 
 Stock Split Module
 ##################
 
 The Stock Split module adds on the stock move a wizard that allows to split them.
```

### Comparing `trytond_stock_split-6.6.0/__init__.py` & `trytond_stock_split-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/icons/LICENSE` & `trytond_stock_split-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/bg.po` & `trytond_stock_split-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/ca.po` & `trytond_stock_split-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/cs.po` & `trytond_stock_split-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/de.po` & `trytond_stock_split-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/es.po` & `trytond_stock_split-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/es_419.po` & `trytond_stock_split-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/et.po` & `trytond_stock_split-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/fa.po` & `trytond_stock_split-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/fi.po` & `trytond_stock_split-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/fr.po` & `trytond_stock_split-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/hu.po` & `trytond_stock_split-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/id.po` & `trytond_stock_split-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/it.po` & `trytond_stock_split-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/lo.po` & `trytond_stock_split-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/lt.po` & `trytond_stock_split-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/nl.po` & `trytond_stock_split-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/pl.po` & `trytond_stock_split-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/pt.po` & `trytond_stock_split-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/ro.po` & `trytond_stock_split-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/ru.po` & `trytond_stock_split-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/sl.po` & `trytond_stock_split-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/tr.po` & `trytond_stock_split-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/uk.po` & `trytond_stock_split-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/locale/zh_CN.po` & `trytond_stock_split-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/stock.py` & `trytond_stock_split-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/stock.xml` & `trytond_stock_split-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/tests/scenario_stock_split_shipment.rst` & `trytond_stock_split-6.8.0/tests/scenario_stock_split_shipment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     >>> shipment1.click('wait')
     >>> shipment1.click('draft')
     >>> len(shipment1.inventory_moves)
     2
 
 Split shipment::
 
-    >>> split_shipment = Wizard('stock.shipment.split', [shipment1])
+    >>> split_shipment = shipment1.click('split_wizard')
     >>> len(split_shipment.form.domain_moves)
     2
     >>> split_shipment.form.moves.append(Move(move2.id))
     >>> split_shipment.execute('split')
 
     >>> shipment2, = Shipment.find([('id', '!=', shipment1.id)])
```

### Comparing `trytond_stock_split-6.6.0/tests/test_module.py` & `trytond_stock_split-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-6.6.0/trytond_stock_split.egg-info/PKG-INFO` & `trytond_stock_split-6.8.0/trytond_stock_split.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-split
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to split stock move
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_split
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock split
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
 
 Stock Split Module
 ##################
 
 The Stock Split module adds on the stock move a wizard that allows to split them.
```

### Comparing `trytond_stock_split-6.6.0/trytond_stock_split.egg-info/SOURCES.txt` & `trytond_stock_split-6.8.0/trytond_stock_split.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
@@ -47,14 +43,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/move_form.xml
 ./view/move_tree.xml
 ./view/shipment_split_form.xml
 ./view/shipment_split_start_form.xml
 ./view/split_start_form.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-stock-split.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

