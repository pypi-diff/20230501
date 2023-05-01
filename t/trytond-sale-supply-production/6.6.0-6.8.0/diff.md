# Comparing `tmp/trytond_sale_supply_production-6.6.0.tar.gz` & `tmp/trytond_sale_supply_production-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply_production-6.6.0.tar", last modified: Mon Oct 31 16:27:17 2022, max compression
+gzip compressed data, was "trytond_sale_supply_production-6.8.0.tar", last modified: Mon May  1 11:49:33 2023, max compression
```

## Comparing `trytond_sale_supply_production-6.6.0.tar` & `trytond_sale_supply_production-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:17.578033 trytond_sale_supply_production-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_supply_production-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_supply_production-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2022-10-31 16:27:16.000000 trytond_sale_supply_production-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_supply_production-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2022-10-31 16:27:15.000000 trytond_sale_supply_production-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:27:15.000000 trytond_sale_supply_production-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_supply_production-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2837 2022-10-31 16:27:17.574699 trytond_sale_supply_production-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2021-12-11 16:59:34.000000 trytond_sale_supply_production-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:17.574699 trytond_sale_supply_production-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:17.574699 trytond_sale_supply_production-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      527 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-10-29 07:50:38.000000 trytond_sale_supply_production-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2022-04-10 15:40:36.000000 trytond_sale_supply_production-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3820 2022-04-08 16:24:28.000000 trytond_sale_supply_production-6.6.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3660 2022-04-08 16:24:28.000000 trytond_sale_supply_production-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      939 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:27:17.578033 trytond_sale_supply_production-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5362 2022-10-29 07:39:11.000000 trytond_sale_supply_production-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:17.574699 trytond_sale_supply_production-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_supply_production-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4140 2020-07-09 09:37:28.000000 trytond_sale_supply_production-6.6.0/tests/scenario_sale_supply_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-04-16 16:30:57.000000 trytond_sale_supply_production-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_supply_production-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_sale_supply_production-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2022-10-31 16:27:14.000000 trytond_sale_supply_production-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:17.574699 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2837 2022-10-31 16:27:17.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1642 2022-10-31 16:27:17.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:27:17.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 16:27:17.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-05-04 10:30:04.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-31 16:27:17.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:27:17.000000 trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:27:17.574699 trytond_sale_supply_production-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2020-04-13 12:49:29.000000 trytond_sale_supply_production-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:33.791674 trytond_sale_supply_production-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2023-05-01 11:06:23.000000 trytond_sale_supply_production-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:06:22.000000 trytond_sale_supply_production-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2837 2023-05-01 11:49:33.791674 trytond_sale_supply_production-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:33.791674 trytond_sale_supply_production-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:33.788340 trytond_sale_supply_production-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      528 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-29 08:02:45.000000 trytond_sale_supply_production-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3820 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3790 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      939 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:49:33.791674 trytond_sale_supply_production-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4544 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:33.788340 trytond_sale_supply_production-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4144 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/tests/scenario_sale_supply_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2987 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/tests/scenario_sale_supply_production_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-05-01 11:06:17.000000 trytond_sale_supply_production-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:33.791674 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2837 2023-05-01 11:49:32.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-01 11:49:33.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:49:32.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:49:32.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 11:49:32.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:49:32.000000 trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:33.788340 trytond_sale_supply_production-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_supply_production-6.8.0/view/template_form.xml
```

### Comparing `trytond_sale_supply_production-6.6.0/COPYRIGHT` & `trytond_sale_supply_production-6.8.0/COPYRIGHT`

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

### Comparing `trytond_sale_supply_production-6.6.0/LICENSE` & `trytond_sale_supply_production-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/PKG-INFO` & `trytond_sale_supply_production-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply_production
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to supply sales from production
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_supply_production
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale supply production
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,32 +38,32 @@
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
 
 Sale Supply Production Module
 #############################
 
 The Sale Supply Production module adds a "supply on sale" option to producible
 products.
-If checked, it will generate a production request for each sale line of this
-product regardless of the stock levels. Once the products are produced they are
-assigned to the customer shipments.
+If selected, it will generate a production request for each sale line of this
+product depending of the option and the stock levels.
+Once the products are produced they are assigned to the customer shipments.
 If the production request is cancelled, the sale goes back to the default
 supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the production request will be
     created only when all the invoice lines are paid.
 ..
```

### Comparing `trytond_sale_supply_production-6.6.0/README.rst` & `trytond_sale_supply_production-6.8.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Sale Supply Production Module
 #############################
 
 The Sale Supply Production module adds a "supply on sale" option to producible
 products.
-If checked, it will generate a production request for each sale line of this
-product regardless of the stock levels. Once the products are produced they are
-assigned to the customer shipments.
+If selected, it will generate a production request for each sale line of this
+product depending of the option and the stock levels.
+Once the products are produced they are assigned to the customer shipments.
 If the production request is cancelled, the sale goes back to the default
 supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the production request will be
     created only when all the invoice lines are paid.
 ..
```

### Comparing `trytond_sale_supply_production-6.6.0/__init__.py` & `trytond_sale_supply_production-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/doc/index.rst` & `trytond_sale_supply_production-6.8.0/doc/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Sale Supply Production Module
 #############################
 
 The Sale Supply Production module adds a "supply on sale" option to producible
 products.
-If checked, it will generate a production request for each sale line of this
-product regardless of the stock levels. Once the products are produced they are
-assigned to the customer shipments.
+If selected, it will generate a production request for each sale line of this
+product depending of the option and the stock levels.
+Once the products are produced they are assigned to the customer shipments.
 If the production request is cancelled, the sale goes back to the default
 supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the production request will be
     created only when all the invoice lines are paid.
 ..
```

### Comparing `trytond_sale_supply_production-6.6.0/locale/ca.po` & `trytond_sale_supply_production-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/locale/de.po` & `trytond_sale_supply_production-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/locale/es.po` & `trytond_sale_supply_production-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/locale/fr.po` & `trytond_sale_supply_production-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/locale/it.po` & `trytond_sale_supply_production-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/locale/nl.po` & `trytond_sale_supply_production-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/product.py` & `trytond_sale_supply_production-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/production.py` & `trytond_sale_supply_production-6.8.0/production.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import Model, ModelView, Workflow
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 
 def process_sale_supply(func):
     @wraps(func)
     def wrapper(cls, productions):
         pool = Pool()
         Sale = pool.get('sale.sale')
         transaction = Transaction()
         context = transaction.context
 
         sales = set()
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             for sub_productions in grouped_slice(productions):
                 ids = [p.id for p in sub_productions]
                 sales.update([s.id for s in Sale.search([
                                 ('lines.productions', 'in', ids),
                                 ])])
         func(cls, productions)
         if sales:
```

### Comparing `trytond_sale_supply_production-6.6.0/sale.py` & `trytond_sale_supply_production-6.8.0/sale.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 from trytond.transaction import Transaction
 
 
 class Sale(metaclass=PoolMeta):
     __name__ = 'sale.sale'
 
     @classmethod
-    def _process_shipment(cls, sales):
+    def _process_supply(cls, sales, product_quantities):
         pool = Pool()
         Production = pool.get('production')
 
         productions = []
         for sale in sales:
-            productions.extend(sale.create_productions())
+            productions.extend(sale.create_productions(product_quantities))
         Production.save(productions)
         Production.set_moves(productions)
-        super()._process_shipment(sales)
+        super()._process_supply(sales, product_quantities)
 
-    def create_productions(self):
+    def create_productions(self, product_quantities):
         productions = []
         for line in self.lines:
-            production = line.get_production()
+            production = line.get_production(product_quantities)
             if not production:
                 continue
             production.planned_start_date = (
                 production.on_change_with_planned_start_date())
             productions.append(production)
             assert not line.productions
         return productions
@@ -63,45 +63,47 @@
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('productions', None)
         return super().copy(lines, default=default)
 
-    def get_production(self):
+    def get_production(self, product_quantities):
         "Return production for the sale line"
         pool = Pool()
         Production = pool.get('production')
         Date = pool.get('ir.date')
+        Uom = pool.get('product.uom')
+
         with Transaction().set_context(company=self.sale.company.id):
             today = Date.today()
 
         if (not self.supply_on_sale
                 or self.productions
+                or not self.ready_for_supply
                 or not self.product.producible):
             return
 
-        # Ensure to create the request for the maximum paid
-        if self.sale.shipment_method == 'invoice':
-            invoice_skips = (set(self.sale.invoices_ignored)
-                | set(self.sale.invoices_recreated))
-            invoice_lines = [l for l in self.invoice_lines
-                if l.invoice not in invoice_skips]
-            if (not invoice_lines
-                    or any((not l.invoice) or l.invoice.state != 'paid'
-                        for l in invoice_lines)):
+        product = self.product
+        quantity = self._get_move_quantity('out')
+        if product.supply_on_sale == 'stock_first':
+            available_qty = product_quantities[product]
+            available_qty = Uom.compute_qty(
+                product.default_uom, available_qty, self.unit,
+                round=False)
+            if quantity < available_qty:
+                product_quantities[product] -= Uom.compute_qty(
+                    self.unit, quantity, product.default_uom, round=False)
                 return
 
         date = self.shipping_date or today
         if date <= today:
             date = today
         else:
             date -= dt.timedelta(1)
-        product = self.product
-        quantity = self._get_move_quantity('out')
         return Production(
             planned_date=date,
             company=self.sale.company,
             warehouse=self.warehouse,
             location=self.warehouse.production_location,
             product=product,
             bom=product.boms[0].bom if product.boms else None,
```

### Comparing `trytond_sale_supply_production-6.6.0/sale.xml` & `trytond_sale_supply_production-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-6.6.0/setup.py` & `trytond_sale_supply_production-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
@@ -37,60 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_supply_production'
 
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
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to supply sales from production',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_supply_production',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale supply production',
     package_dir={'trytond.modules.sale_supply_production': '.'},
     packages=(
         ['trytond.modules.sale_supply_production']
         + ['trytond.modules.sale_supply_production.%s' % p
             for p in find_packages()]
@@ -128,27 +106,26 @@
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
     sale_supply_production = trytond.modules.sale_supply_production
     """,  # noqa: E501
     )
```

### Comparing `trytond_sale_supply_production-6.6.0/tests/scenario_sale_supply_production.rst` & `trytond_sale_supply_production-6.8.0/tests/scenario_sale_supply_production.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     >>> template = ProductTemplate()
     >>> template.name = "Product"
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.producible = True
     >>> template.salable = True
-    >>> template.supply_on_sale = True
+    >>> template.supply_on_sale = 'always'
     >>> template.list_price = Decimal(30)
     >>> template.account_category = account_category
     >>> product, = template.products
     >>> product.cost_price = Decimal(20)
     >>> template.save()
     >>> product, = template.products
```

### Comparing `trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/PKG-INFO` & `trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-supply-production
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to supply sales from production
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_supply_production
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale supply production
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,32 +38,32 @@
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
 
 Sale Supply Production Module
 #############################
 
 The Sale Supply Production module adds a "supply on sale" option to producible
 products.
-If checked, it will generate a production request for each sale line of this
-product regardless of the stock levels. Once the products are produced they are
-assigned to the customer shipments.
+If selected, it will generate a production request for each sale line of this
+product depending of the option and the stock levels.
+Once the products are produced they are assigned to the customer shipments.
 If the production request is cancelled, the sale goes back to the default
 supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the production request will be
     created only when all the invoice lines are paid.
 ..
```

### Comparing `trytond_sale_supply_production-6.6.0/trytond_sale_supply_production.egg-info/SOURCES.txt` & `trytond_sale_supply_production-6.8.0/trytond_sale_supply_production.egg-info/SOURCES.txt`

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
 message.xml
@@ -47,17 +43,19 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_supply_production.rst
+./tests/scenario_sale_supply_production_stock_first.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/template_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -77,14 +75,15 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_sale_supply_production.rst
+tests/scenario_sale_supply_production_stock_first.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_sale_supply_production.egg-info/PKG-INFO
 trytond_sale_supply_production.egg-info/SOURCES.txt
 trytond_sale_supply_production.egg-info/dependency_links.txt
 trytond_sale_supply_production.egg-info/entry_points.txt
 trytond_sale_supply_production.egg-info/not-zip-safe
```

