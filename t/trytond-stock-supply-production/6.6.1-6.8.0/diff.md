# Comparing `tmp/trytond_stock_supply_production-6.6.1.tar.gz` & `tmp/trytond_stock_supply_production-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply_production-6.6.1.tar", last modified: Sun Feb  5 21:02:21 2023, max compression
+gzip compressed data, was "trytond_stock_supply_production-6.8.0.tar", last modified: Mon May  1 11:39:05 2023, max compression
```

## Comparing `trytond_stock_supply_production-6.6.1.tar` & `trytond_stock_supply_production-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:02:21.094739 trytond_stock_supply_production-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2023-02-05 21:02:18.000000 trytond_stock_supply_production-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-02-05 21:02:17.000000 trytond_stock_supply_production-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3049 2023-02-05 21:02:21.094739 trytond_stock_supply_production-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      745 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:02:21.091405 trytond_stock_supply_production-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      745 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:02:21.088072 trytond_stock_supply_production-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      912 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      965 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      954 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      960 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      873 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      968 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      864 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      900 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      981 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      822 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      937 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      906 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9199 2023-02-05 20:48:28.000000 trytond_stock_supply_production-6.6.1/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1458 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:02:21.094739 trytond_stock_supply_production-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4481 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3619 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      618 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:02:21.091405 trytond_stock_supply_production-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4285 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/tests/scenario_stock_supply_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      554 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2022-12-19 12:03:07.000000 trytond_stock_supply_production-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:02:21.091405 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3049 2023-02-05 21:02:20.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1667 2023-02-05 21:02:21.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:02:20.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-02-05 21:02:20.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:02:20.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-02-05 21:02:20.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:02:20.000000 trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:02:21.091405 trytond_stock_supply_production-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-12-19 12:02:59.000000 trytond_stock_supply_production-6.6.1/view/production_configuration_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:05.300541 trytond_stock_supply_production-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2164 2023-05-01 10:59:31.000000 trytond_stock_supply_production-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 10:59:31.000000 trytond_stock_supply_production-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply_production-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3033 2023-05-01 11:39:05.300541 trytond_stock_supply_production-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-01-16 14:00:21.000000 trytond_stock_supply_production-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:05.297208 trytond_stock_supply_production-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-01-16 14:00:21.000000 trytond_stock_supply_production-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:05.297208 trytond_stock_supply_production-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      912 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      965 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      954 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      960 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      873 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      968 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      864 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      900 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      981 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      822 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      937 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      906 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-04-29 08:02:40.000000 trytond_stock_supply_production-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9353 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-01-16 14:00:21.000000 trytond_stock_supply_production-6.8.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:39:05.300541 trytond_stock_supply_production-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4437 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3619 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      618 2023-01-16 14:00:21.000000 trytond_stock_supply_production-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:05.297208 trytond_stock_supply_production-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/tests/scenario_stock_supply_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_supply_production-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-05-01 10:59:26.000000 trytond_stock_supply_production-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:05.300541 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3033 2023-05-01 11:39:04.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1667 2023-05-01 11:39:05.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:39:04.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-05-01 11:39:04.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-05-01 11:39:04.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:39:04.000000 trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:05.297208 trytond_stock_supply_production-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 trytond_stock_supply_production-6.8.0/view/production_configuration_form.xml
```

### Comparing `trytond_stock_supply_production-6.6.1/CHANGELOG` & `trytond_stock_supply_production-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-Version 6.6.1 - 2023-02-05
+
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_supply_production-6.6.1/COPYRIGHT` & `trytond_stock_supply_production-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/LICENSE` & `trytond_stock_supply_production-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/PKG-INFO` & `trytond_stock_supply_production-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply_production
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for stock supply of production
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_supply_production
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock supply production
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
 
 Stock Supply Production Module
 ##############################
 
 The Stock Supply Production module adds automatic supply mechanisms via
```

### Comparing `trytond_stock_supply_production-6.6.1/README.rst` & `trytond_stock_supply_production-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/__init__.py` & `trytond_stock_supply_production-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/doc/conf.py` & `trytond_stock_supply_production-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
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
```

### Comparing `trytond_stock_supply_production-6.6.1/doc/index.rst` & `trytond_stock_supply_production-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/bg.po` & `trytond_stock_supply_production-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/ca.po` & `trytond_stock_supply_production-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/cs.po` & `trytond_stock_supply_production-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/de.po` & `trytond_stock_supply_production-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/es.po` & `trytond_stock_supply_production-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/es_419.po` & `trytond_stock_supply_production-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/et.po` & `trytond_stock_supply_production-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/fa.po` & `trytond_stock_supply_production-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/fi.po` & `trytond_stock_supply_production-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/fr.po` & `trytond_stock_supply_production-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/hu.po` & `trytond_stock_supply_production-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/id.po` & `trytond_stock_supply_production-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/it.po` & `trytond_stock_supply_production-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/lo.po` & `trytond_stock_supply_production-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/lt.po` & `trytond_stock_supply_production-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/nl.po` & `trytond_stock_supply_production-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/pl.po` & `trytond_stock_supply_production-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/pt.po` & `trytond_stock_supply_production-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/ro.po` & `trytond_stock_supply_production-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/ru.po` & `trytond_stock_supply_production-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/sl.po` & `trytond_stock_supply_production-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/tr.po` & `trytond_stock_supply_production-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/uk.po` & `trytond_stock_supply_production-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/locale/zh_CN.po` & `trytond_stock_supply_production-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/product.py` & `trytond_stock_supply_production-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/production.py` & `trytond_stock_supply_production-6.8.0/production.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 from collections import defaultdict
 
 from trytond.model import ModelSQL, ValueMixin, fields
 from trytond.pool import Pool, PoolMeta
+from trytond.pyson import TimeDelta
 from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 
-supply_period = fields.TimeDelta("Supply Period")
+supply_period = fields.TimeDelta(
+    "Supply Period",
+    domain=['OR',
+        ('supply_period', '=', None),
+        ('supply_period', '>=', TimeDelta()),
+        ])
 
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'production.configuration'
     supply_period = fields.MultiValue(supply_period)
```

### Comparing `trytond_stock_supply_production-6.6.1/production.xml` & `trytond_stock_supply_production-6.8.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/setup.py` & `trytond_stock_supply_production-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -34,38 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_supply_production'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for stock supply of production',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_supply_production',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock supply production',
     package_dir={'trytond.modules.stock_supply_production': '.'},
     packages=(
         ['trytond.modules.stock_supply_production']
         + ['trytond.modules.stock_supply_production.%s' % p
             for p in find_packages()]
@@ -103,23 +103,23 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_stock_supply_production-6.6.1/stock.py` & `trytond_stock_supply_production-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/stock.xml` & `trytond_stock_supply_production-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-6.6.1/tests/scenario_stock_supply_production.rst` & `trytond_stock_supply_production-6.8.0/tests/scenario_stock_supply_production.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.stock.exceptions import MoveFutureWarning
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply_production')
 
 Create company::
```

### Comparing `trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/PKG-INFO` & `trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-supply-production
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for stock supply of production
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_supply_production
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock supply production
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
 
 Stock Supply Production Module
 ##############################
 
 The Stock Supply Production module adds automatic supply mechanisms via
```

### Comparing `trytond_stock_supply_production-6.6.1/trytond_stock_supply_production.egg-info/SOURCES.txt` & `trytond_stock_supply_production-6.8.0/trytond_stock_supply_production.egg-info/SOURCES.txt`

 * *Files identical despite different names*

