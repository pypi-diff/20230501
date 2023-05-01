# Comparing `tmp/trytond_stock_assign_manual-6.6.0.tar.gz` & `tmp/trytond_stock_assign_manual-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_assign_manual-6.6.0.tar", last modified: Mon Oct 31 16:27:32 2022, max compression
+gzip compressed data, was "trytond_stock_assign_manual-6.8.0.tar", last modified: Mon May  1 11:46:47 2023, max compression
```

## Comparing `trytond_stock_assign_manual-6.6.0.tar` & `trytond_stock_assign_manual-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:32.264920 trytond_stock_assign_manual-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_stock_assign_manual-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_assign_manual-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2022-10-31 16:27:30.000000 trytond_stock_assign_manual-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_assign_manual-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2022-10-31 16:27:30.000000 trytond_stock_assign_manual-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:27:29.000000 trytond_stock_assign_manual-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2020-09-12 14:25:19.000000 trytond_stock_assign_manual-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_assign_manual-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2540 2022-10-31 16:27:32.264920 trytond_stock_assign_manual-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      805 2021-12-11 16:59:34.000000 trytond_stock_assign_manual-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:32.264920 trytond_stock_assign_manual-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:32.261586 trytond_stock_assign_manual-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4822 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5004 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4846 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4869 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3876 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4886 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2022-10-29 07:50:37.000000 trytond_stock_assign_manual-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2020-09-12 14:25:19.000000 trytond_stock_assign_manual-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2020-09-12 14:25:19.000000 trytond_stock_assign_manual-6.6.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2020-09-12 14:25:19.000000 trytond_stock_assign_manual-6.6.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:27:32.268253 trytond_stock_assign_manual-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5384 2022-10-29 07:39:11.000000 trytond_stock_assign_manual-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15514 2022-04-10 15:40:36.000000 trytond_stock_assign_manual-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5993 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:32.261586 trytond_stock_assign_manual-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_assign_manual-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6298 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/tests/scenario_stock_assign_manual.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-04-16 16:30:57.000000 trytond_stock_assign_manual-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_stock_assign_manual-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-31 15:10:09.000000 trytond_stock_assign_manual-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      133 2022-10-31 16:27:28.000000 trytond_stock_assign_manual-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:32.264920 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2540 2022-10-31 16:27:31.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1929 2022-10-31 16:27:32.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:27:31.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2022-10-31 16:27:31.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-10-13 07:23:31.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2022-10-31 16:27:31.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:27:31.000000 trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:32.264920 trytond_stock_assign_manual-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2020-10-09 17:09:19.000000 trytond_stock_assign_manual-6.6.0/view/shipment_assign_manual_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/view/shipment_assigned_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/view/shipment_assigned_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2020-09-12 14:25:19.000000 trytond_stock_assign_manual-6.6.0/view/shipment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2021-04-27 07:34:41.000000 trytond_stock_assign_manual-6.6.0/view/shipment_unassign_manual_show_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:47.886282 trytond_stock_assign_manual-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-05-01 11:04:35.000000 trytond_stock_assign_manual-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 11:04:35.000000 trytond_stock_assign_manual-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2528 2023-05-01 11:46:47.886282 trytond_stock_assign_manual-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      805 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:47.882948 trytond_stock_assign_manual-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:47.876282 trytond_stock_assign_manual-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4822 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5004 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4846 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4869 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3876 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4886 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-04-29 08:02:44.000000 trytond_stock_assign_manual-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:46:47.886282 trytond_stock_assign_manual-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4569 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15508 2023-04-21 08:36:08.000000 trytond_stock_assign_manual-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5993 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:47.879615 trytond_stock_assign_manual-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/tests/scenario_stock_assign_manual.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      133 2023-05-01 11:04:29.000000 trytond_stock_assign_manual-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:47.886282 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2528 2023-05-01 11:46:47.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-05-01 11:46:47.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:46:47.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 11:46:47.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2023-05-01 11:46:47.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:46:47.000000 trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:47.882948 trytond_stock_assign_manual-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/view/shipment_assign_manual_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/view/shipment_assigned_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/view/shipment_assigned_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/view/shipment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-6.8.0/view/shipment_unassign_manual_show_form.xml
```

### Comparing `trytond_stock_assign_manual-6.6.0/COPYRIGHT` & `trytond_stock_assign_manual-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020-2022 Cédric Krier
+Copyright (C) 2020-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_assign_manual-6.6.0/LICENSE` & `trytond_stock_assign_manual-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/PKG-INFO` & `trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_assign_manual
-Version: 6.6.0
+Name: trytond-stock-assign-manual
+Version: 6.8.0
 Summary: Tryton module to assign manually stock move
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_assign_manual
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock assign
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
 
 Stock Assign Manual Module
 ##########################
 
 The Stock Assign Manual module adds a wizard on shipments and production that
```

### Comparing `trytond_stock_assign_manual-6.6.0/__init__.py` & `trytond_stock_assign_manual-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/bg.po` & `trytond_stock_assign_manual-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/ca.po` & `trytond_stock_assign_manual-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/cs.po` & `trytond_stock_assign_manual-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/de.po` & `trytond_stock_assign_manual-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/es.po` & `trytond_stock_assign_manual-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/es_419.po` & `trytond_stock_assign_manual-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/et.po` & `trytond_stock_assign_manual-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/fa.po` & `trytond_stock_assign_manual-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/fi.po` & `trytond_stock_assign_manual-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/fr.po` & `trytond_stock_assign_manual-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/hu.po` & `trytond_stock_assign_manual-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/id.po` & `trytond_stock_assign_manual-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/it.po` & `trytond_stock_assign_manual-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/lo.po` & `trytond_stock_assign_manual-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/lt.po` & `trytond_stock_assign_manual-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/nl.po` & `trytond_stock_assign_manual-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/pl.po` & `trytond_stock_assign_manual-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/pt.po` & `trytond_stock_assign_manual-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/ro.po` & `trytond_stock_assign_manual-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/ru.po` & `trytond_stock_assign_manual-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/sl.po` & `trytond_stock_assign_manual-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/tr.po` & `trytond_stock_assign_manual-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/uk.po` & `trytond_stock_assign_manual-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/locale/zh_CN.po` & `trytond_stock_assign_manual-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/message.xml` & `trytond_stock_assign_manual-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/production.py` & `trytond_stock_assign_manual-6.8.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/production.xml` & `trytond_stock_assign_manual-6.8.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/setup.py` & `trytond_stock_assign_manual-6.8.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     if slice:
         content = '\n'.join(content.splitlines()[slice])
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
@@ -37,63 +34,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_assign_manual'
 
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
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_production'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to assign manually stock move',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_assign_manual',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock assign',
     package_dir={'trytond.modules.stock_assign_manual': '.'},
     packages=(
         ['trytond.modules.stock_assign_manual']
         + ['trytond.modules.stock_assign_manual.%s' % p
             for p in find_packages()]
@@ -131,27 +109,26 @@
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
     stock_assign_manual = trytond.modules.stock_assign_manual
     """,  # noqa: E501
     )
```

### Comparing `trytond_stock_assign_manual-6.6.0/stock.py` & `trytond_stock_assign_manual-6.8.0/stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,16 +404,15 @@
     def on_change_assigned_quantity(self, name=None):
         if self.move and self.assigned_quantity:
             self.unassigned_quantity = self.unit.round(
                 self.move.quantity - self.assigned_quantity)
 
     @fields.depends('move')
     def on_change_with_unit(self, name=None):
-        if self.move:
-            return self.move.uom.id
+        return self.move.uom if self.move else None
 
     @fields.depends('move')
     def on_change_with_move_quantity(self, name=None):
         if self.move:
             return self.move.quantity
```

### Comparing `trytond_stock_assign_manual-6.6.0/stock.xml` & `trytond_stock_assign_manual-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-6.6.0/tests/scenario_stock_assign_manual.rst` & `trytond_stock_assign_manual-6.8.0/tests/scenario_stock_assign_manual.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ============================
 Stock Assign Manual Scenario
 ============================
 
 Imports::
 
-    >>> import datetime as dt
     >>> import json
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
-    >>> today = dt.date.today()
 
 Activate stock_assign_manual::
 
     >>> config = activate_modules('stock_assign_manual')
 
 Create company::
 
@@ -96,15 +94,15 @@
     >>> move.currency = company.currency
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
 
 Assign manually the first move::
 
-    >>> assign_manual = Wizard('stock.shipment.assign.manual', [shipment])
+    >>> assign_manual = shipment.click('assign_manual_wizard')
     >>> assign_manual.form.move == shipment.inventory_moves[0]
     True
     >>> assign_manual.form.move_quantity
     2.0
     >>> assign_manual.form.place = json.dumps([storage_loc.id, product.id])
     >>> assign_manual.execute('assign')
     >>> assign_manual.form.move_quantity
@@ -121,21 +119,21 @@
 
     >>> shipment.state
     'waiting'
     >>> sorted([m.state for m in shipment.inventory_moves])
     ['assigned', 'assigned', 'draft']
     >>> [m.quantity for m in shipment.inventory_moves if m.state == 'assigned']
     [1.0, 1.0]
-    >>> [m.from_location for m in shipment.inventory_moves
-    ...     if m.state == 'assigned'] == [storage_loc, storage_loc2]
+    >>> {m.from_location for m in shipment.inventory_moves
+    ...     if m.state == 'assigned'} == {storage_loc, storage_loc2}
     True
 
 Assign manually remaining move::
 
-    >>> assign_manual = Wizard('stock.shipment.assign.manual', [shipment])
+    >>> assign_manual = shipment.click('assign_manual_wizard')
     >>> assign_manual.form.place = json.dumps([storage_loc2.id, product.id])
     >>> assign_manual.execute('assign')
 
     >>> shipment.state
     'assigned'
 
 Unassign move::
```

### Comparing `trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/PKG-INFO` & `trytond_stock_assign_manual-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-assign-manual
-Version: 6.6.0
+Name: trytond_stock_assign_manual
+Version: 6.8.0
 Summary: Tryton module to assign manually stock move
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_assign_manual
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock assign
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
 
 Stock Assign Manual Module
 ##########################
 
 The Stock Assign Manual module adds a wizard on shipments and production that
```

### Comparing `trytond_stock_assign_manual-6.6.0/trytond_stock_assign_manual.egg-info/SOURCES.txt` & `trytond_stock_assign_manual-6.8.0/trytond_stock_assign_manual.egg-info/SOURCES.txt`

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
@@ -52,14 +48,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/shipment_assign_manual_show_form.xml
 ./view/shipment_assigned_move_form.xml
 ./view/shipment_assigned_move_list.xml
 ./view/shipment_form.xml
 ./view/shipment_unassign_manual_show_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

