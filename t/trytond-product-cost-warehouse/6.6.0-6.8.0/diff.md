# Comparing `tmp/trytond_product_cost_warehouse-6.6.0.tar.gz` & `tmp/trytond_product_cost_warehouse-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_warehouse-6.6.0.tar", last modified: Mon Oct 31 16:06:48 2022, max compression
+gzip compressed data, was "trytond_product_cost_warehouse-6.8.0.tar", last modified: Mon May  1 12:00:11 2023, max compression
```

## Comparing `trytond_product_cost_warehouse-6.6.0.tar` & `trytond_product_cost_warehouse-6.8.0.tar`

### file list

```diff
@@ -1,75 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_product_cost_warehouse-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 16:06:47.000000 trytond_product_cost_warehouse-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_product_cost_warehouse-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2022-10-31 16:06:46.000000 trytond_product_cost_warehouse-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:06:45.000000 trytond_product_cost_warehouse-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_product_cost_warehouse-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2510 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2022-10-27 11:24:44.000000 trytond_product_cost_warehouse-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2021-12-11 16:59:33.000000 trytond_product_cost_warehouse-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2022-04-10 15:40:35.000000 trytond_product_cost_warehouse-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2021-12-11 16:59:33.000000 trytond_product_cost_warehouse-6.6.0/company.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2022-10-27 11:24:44.000000 trytond_product_cost_warehouse-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_product_cost_warehouse-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2022-04-08 16:27:20.000000 trytond_product_cost_warehouse-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1326 2021-12-11 16:59:33.000000 trytond_product_cost_warehouse-6.6.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:48.363092 trytond_product_cost_warehouse-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2769 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2683 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2720 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2366 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2069 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2022-10-29 07:50:43.000000 trytond_product_cost_warehouse-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    10042 2022-04-10 15:40:35.000000 trytond_product_cost_warehouse-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2021-10-30 15:16:00.000000 trytond_product_cost_warehouse-6.6.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5672 2022-10-29 07:39:11.000000 trytond_product_cost_warehouse-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8952 2022-08-26 15:50:06.000000 trytond_product_cost_warehouse-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_product_cost_warehouse-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4445 2022-09-29 07:07:37.000000 trytond_product_cost_warehouse-6.6.0/tests/scenario_account_stock_continental.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4447 2022-09-29 07:07:37.000000 trytond_product_cost_warehouse-6.6.0/tests/scenario_product_cost_fifo_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6371 2022-09-29 07:07:37.000000 trytond_product_cost_warehouse-6.6.0/tests/scenario_product_cost_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2022-04-16 16:30:56.000000 trytond_product_cost_warehouse-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_product_cost_warehouse-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_product_cost_warehouse-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2022-10-31 16:06:45.000000 trytond_product_cost_warehouse-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2510 2022-10-31 16:06:47.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2057 2022-10-31 16:06:48.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:06:47.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 16:06:47.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-05-03 13:47:43.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      279 2022-10-31 16:06:47.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:06:47.000000 trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:48.366425 trytond_product_cost_warehouse-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2021-11-30 09:56:07.000000 trytond_product_cost_warehouse-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/view/ir_cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2021-04-03 16:10:55.000000 trytond_product_cost_warehouse-6.6.0/view/stock_location_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:11.702923 trytond_product_cost_warehouse-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-05-01 11:13:42.000000 trytond_product_cost_warehouse-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:13:42.000000 trytond_product_cost_warehouse-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2495 2023-05-01 12:00:11.702923 trytond_product_cost_warehouse-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/company.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:11.699590 trytond_product_cost_warehouse-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1530 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1326 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:11.692923 trytond_product_cost_warehouse-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2769 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2683 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2720 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2366 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2069 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-04-29 08:02:49.000000 trytond_product_cost_warehouse-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10188 2023-04-21 08:36:08.000000 trytond_product_cost_warehouse-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:00:11.702923 trytond_product_cost_warehouse-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4854 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8888 2023-04-21 08:36:08.000000 trytond_product_cost_warehouse-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:11.696256 trytond_product_cost_warehouse-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4445 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tests/scenario_account_stock_continental.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4447 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tests/scenario_product_cost_fifo_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6371 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tests/scenario_product_cost_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-05-01 11:13:36.000000 trytond_product_cost_warehouse-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:11.702923 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2495 2023-05-01 12:00:10.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2019 2023-05-01 12:00:11.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:00:10.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 12:00:10.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      279 2023-05-01 12:00:10.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:00:10.000000 trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:11.696256 trytond_product_cost_warehouse-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/view/ir_cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-6.8.0/view/stock_location_form.xml
```

### Comparing `trytond_product_cost_warehouse-6.6.0/CHANGELOG` & `trytond_product_cost_warehouse-6.8.0/CHANGELOG`

 * *Files 7% similar despite different names*

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
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_product_cost_warehouse-6.6.0/COPYRIGHT` & `trytond_product_cost_warehouse-6.8.0/COPYRIGHT`

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

### Comparing `trytond_product_cost_warehouse-6.6.0/LICENSE` & `trytond_product_cost_warehouse-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/PKG-INFO` & `trytond_product_cost_warehouse-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_product_cost_warehouse
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to compute product cost per warehouse
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-cost-warehouse
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/product_cost_warehouse
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost warehouse
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
 
 #############################
 Product Cost Warehouse Module
 #############################
```

### Comparing `trytond_product_cost_warehouse-6.6.0/__init__.py` & `trytond_product_cost_warehouse-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/company.py` & `trytond_product_cost_warehouse-6.8.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/doc/conf.py` & `trytond_product_cost_warehouse-6.8.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-modules_url = 'https://docs.tryton.org/projects/modules-{module}/en/{series}/'
-trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+import os
+
+base_url = os.environ.get('DOC_BASE_URL')
+if base_url:
+    modules_url = base_url + '/modules-{module}/'
+    trytond_url = base_url + '/server/'
+else:
+    modules_url = (
+        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
+    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
 
 
 def get_info():
     import configparser
-    import os
     import subprocess
     import sys
 
     module_dir = os.path.dirname(os.path.dirname(__file__))
 
     config = configparser.ConfigParser()
     config.read_file(open(os.path.join(module_dir, 'tryton.cfg')))
@@ -22,15 +29,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     for key in {'depends', 'extras_depend'}:
         info[key] = info.get(key, '').strip().splitlines()
     info['modules'] = set(info['depends'] + info['extras_depend'])
@@ -53,9 +63,10 @@
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
+linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
-del get_info, info, modules_url, trytond_url
+del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_product_cost_warehouse-6.6.0/doc/usage.rst` & `trytond_product_cost_warehouse-6.8.0/doc/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    Once you have activated the cost prices per warehouse if you then want
    to deactivate it you may need to manually run a recalculation of all the
    products' cost prices.
 
 .. _Viewing product cost prices:
 
 Viewing product cost prices
-===========================  
+===========================
 
 With this module activated each `Product's <product:concept-product>` cost
 price is shown based on your current `Company <company:model-company.company>`
 and `Warehouse <stock:concept-stock.location.warehouse>`.
 These can be updated in your user preferences.
 
 .. _Moving stock between warehouses:
```

### Comparing `trytond_product_cost_warehouse-6.6.0/ir.py` & `trytond_product_cost_warehouse-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/bg.po` & `trytond_product_cost_warehouse-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/ca.po` & `trytond_product_cost_warehouse-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/cs.po` & `trytond_product_cost_warehouse-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/de.po` & `trytond_product_cost_warehouse-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/es.po` & `trytond_product_cost_warehouse-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/es_419.po` & `trytond_product_cost_warehouse-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/et.po` & `trytond_product_cost_warehouse-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/fa.po` & `trytond_product_cost_warehouse-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/fi.po` & `trytond_product_cost_warehouse-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/fr.po` & `trytond_product_cost_warehouse-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/hu.po` & `trytond_product_cost_warehouse-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/id.po` & `trytond_product_cost_warehouse-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/it.po` & `trytond_product_cost_warehouse-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/lo.po` & `trytond_product_cost_warehouse-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/lt.po` & `trytond_product_cost_warehouse-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/nl.po` & `trytond_product_cost_warehouse-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/pl.po` & `trytond_product_cost_warehouse-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/pt.po` & `trytond_product_cost_warehouse-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/ro.po` & `trytond_product_cost_warehouse-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/ru.po` & `trytond_product_cost_warehouse-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/sl.po` & `trytond_product_cost_warehouse-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/tr.po` & `trytond_product_cost_warehouse-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/uk.po` & `trytond_product_cost_warehouse-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/locale/zh_CN.po` & `trytond_product_cost_warehouse-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/product.py` & `trytond_product_cost_warehouse-6.8.0/product.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.model import ModelSQL, fields
 from trytond.modules.company.model import CompanyValueMixin
+from trytond.modules.product.product import TemplateFunction
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 from trytond.transaction import Transaction
 
 cost_price_warehouse = fields.Boolean(
     "Cost Price per Warehouse",
     help="Compute product cost price for each warehouse.")
@@ -53,19 +54,20 @@
             records = sorted(records, key=lambda r: r.warehouse is None)
         return records
 
     def get_multivalue(self, name, **pattern):
         pool = Pool()
         Company = pool.get('company.company')
         context = Transaction().context
-        Value = self.multivalue_model(name)
-        if issubclass(Value, CostPrice) and context.get('company'):
-            company = Company(context['company'])
-            if company.cost_price_warehouse:
-                pattern.setdefault('warehouse', context.get('warehouse'))
+        if not isinstance(self._fields[name], TemplateFunction):
+            Value = self.multivalue_model(name)
+            if issubclass(Value, CostPrice) and context.get('company'):
+                company = Company(context['company'])
+                if company.cost_price_warehouse:
+                    pattern.setdefault('warehouse', context.get('warehouse'))
         return super().get_multivalue(name, **pattern)
 
     def set_multivalue(self, name, value, save=True, **pattern):
         pool = Pool()
         Company = pool.get('company.company')
         context = Transaction().context
         Value = self.multivalue_model(name)
```

### Comparing `trytond_product_cost_warehouse-6.6.0/res.py` & `trytond_product_cost_warehouse-6.8.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/setup.py` & `trytond_product_cost_warehouse-6.8.0/setup.py`

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
@@ -37,67 +34,48 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_product_cost_warehouse'
 
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
     get_require_version('trytond_account_invoice_stock'),
     get_require_version('trytond_product_cost_fifo'),
     get_require_version('trytond_product_cost_history'),
     get_require_version('trytond_account_stock_continental'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to compute product cost per warehouse',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-product-cost-warehouse'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/product_cost_warehouse',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product cost warehouse',
     package_dir={'trytond.modules.product_cost_warehouse': '.'},
     packages=(
         ['trytond.modules.product_cost_warehouse']
         + ['trytond.modules.product_cost_warehouse.%s' % p
             for p in find_packages()]
@@ -135,27 +113,26 @@
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
     product_cost_warehouse = trytond.modules.product_cost_warehouse
     """,  # noqa: E501
     )
```

### Comparing `trytond_product_cost_warehouse-6.6.0/stock.py` & `trytond_product_cost_warehouse-6.8.0/stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,10 +219,8 @@
     def on_change_with_transit_location(self, name=None):
         pool = Pool()
         Config = pool.get('stock.configuration')
         location = super().on_change_with_transit_location(name=name)
         if not location and self.company and self.company.cost_price_warehouse:
             location = Config(1).get_multivalue(
                 'shipment_internal_transit', company=self.company)
-            if location:
-                location = location.id
         return location
```

### Comparing `trytond_product_cost_warehouse-6.6.0/tests/scenario_account_stock_continental.rst` & `trytond_product_cost_warehouse-6.8.0/tests/scenario_account_stock_continental.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/tests/scenario_product_cost_fifo_warehouse.rst` & `trytond_product_cost_warehouse-6.8.0/tests/scenario_product_cost_fifo_warehouse.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/tests/scenario_product_cost_warehouse.rst` & `trytond_product_cost_warehouse-6.8.0/tests/scenario_product_cost_warehouse.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/PKG-INFO` & `trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-product-cost-warehouse
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to compute product cost per warehouse
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-cost-warehouse
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/product_cost_warehouse
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost warehouse
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
 
 #############################
 Product Cost Warehouse Module
 #############################
```

### Comparing `trytond_product_cost_warehouse-6.6.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt` & `trytond_product_cost_warehouse-6.8.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt`

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
```

