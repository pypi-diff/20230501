# Comparing `tmp/trytond_sale_shipment_grouping-6.6.1.tar.gz` & `tmp/trytond_sale_shipment_grouping-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_shipment_grouping-6.6.1.tar", last modified: Sun Feb  5 21:10:50 2023, max compression
+gzip compressed data, was "trytond_sale_shipment_grouping-6.8.0.tar", last modified: Mon May  1 11:40:52 2023, max compression
```

## Comparing `trytond_sale_shipment_grouping-6.6.1.tar` & `trytond_sale_shipment_grouping-6.8.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:10:50.859371 trytond_sale_shipment_grouping-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1622 2023-02-05 21:10:47.000000 trytond_sale_shipment_grouping-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      689 2023-02-05 21:10:47.000000 trytond_sale_shipment_grouping-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_sale_shipment_grouping-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-02-05 21:10:50.859371 trytond_sale_shipment_grouping-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1393 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:10:50.856037 trytond_sale_shipment_grouping-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:10:50.856037 trytond_sale_shipment_grouping-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1474 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2022-12-19 12:02:58.000000 trytond_sale_shipment_grouping-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1795 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1742 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1733 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1959 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1912 2022-12-19 12:02:58.000000 trytond_sale_shipment_grouping-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1802 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1420 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1873 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1411 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1771 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2022-12-19 12:02:58.000000 trytond_sale_shipment_grouping-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1404 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1486 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1625 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2247 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2022-12-19 12:02:58.000000 trytond_sale_shipment_grouping-6.6.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2787 2023-02-05 20:48:28.000000 trytond_sale_shipment_grouping-6.6.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:10:50.859371 trytond_sale_shipment_grouping-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4483 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:10:50.856037 trytond_sale_shipment_grouping-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5786 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/tests/scenario_sale_shipment_grouping.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2885 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/tests/scenario_sale_shipment_grouping_multiple.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2022-12-19 12:02:58.000000 trytond_sale_shipment_grouping-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      117 2022-12-19 12:03:07.000000 trytond_sale_shipment_grouping-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:10:50.859371 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1762 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      115 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:10:50.000000 trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:10:50.856037 trytond_sale_shipment_grouping-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2022-12-19 12:02:57.000000 trytond_sale_shipment_grouping-6.6.1/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:52.765208 trytond_sale_shipment_grouping-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1685 2023-05-01 11:00:42.000000 trytond_sale_shipment_grouping-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      689 2023-05-01 11:00:42.000000 trytond_sale_shipment_grouping-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2766 2023-05-01 11:40:52.765208 trytond_sale_shipment_grouping-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:52.761875 trytond_sale_shipment_grouping-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:52.758541 trytond_sale_shipment_grouping-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1474 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1795 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1742 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1733 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1959 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1912 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1802 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1873 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1411 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1771 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1413 2023-04-30 10:46:36.000000 trytond_sale_shipment_grouping-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1486 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1625 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-29 08:02:40.000000 trytond_sale_shipment_grouping-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2247 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2888 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:40:52.765208 trytond_sale_shipment_grouping-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4382 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:52.761875 trytond_sale_shipment_grouping-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5666 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tests/scenario_sale_shipment_grouping.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2888 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tests/scenario_sale_shipment_grouping_multiple.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2170 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tests/scenario_sale_shipment_grouping_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      117 2023-05-01 11:00:36.000000 trytond_sale_shipment_grouping-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:52.765208 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2766 2023-05-01 11:40:51.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1862 2023-05-01 11:40:52.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:40:51.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:40:51.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      115 2023-05-01 11:40:51.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:40:51.000000 trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:52.761875 trytond_sale_shipment_grouping-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-6.8.0/view/party_form.xml
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/CHANGELOG` & `trytond_sale_shipment_grouping-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_sale_shipment_grouping-6.6.1/COPYRIGHT` & `trytond_sale_shipment_grouping-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2014-2017 Nicolas Évrard.
+Copyright (C) 2014-2023 Nicolas Évrard.
 Copyright (C) 2014-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/LICENSE` & `trytond_sale_shipment_grouping-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/PKG-INFO` & `trytond_sale_shipment_grouping-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_grouping
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to group sale stock moves
 Home-page: http://www.tryton.org/
-Download-URL: http://dowloads.tryton.org/6.6/
+Download-URL: http://dowloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_shipment_grouping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale shipment grouping
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
 
 Sale Shipment Grouping Module
 #############################
 
 The ``sale_shipment_grouping`` module adds an option to define how stock moves
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/configuration.py` & `trytond_sale_shipment_grouping-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/doc/conf.py` & `trytond_sale_shipment_grouping-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/bg.po` & `trytond_sale_shipment_grouping-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/ca.po` & `trytond_sale_shipment_grouping-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/cs.po` & `trytond_sale_shipment_grouping-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/de.po` & `trytond_sale_shipment_grouping-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/es.po` & `trytond_sale_shipment_grouping-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/es_419.po` & `trytond_sale_shipment_grouping-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/et.po` & `trytond_sale_shipment_grouping-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/fa.po` & `trytond_sale_shipment_grouping-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/fi.po` & `trytond_sale_shipment_grouping-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/fr.po` & `trytond_sale_shipment_grouping-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/hu.po` & `trytond_sale_shipment_grouping-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/id.po` & `trytond_sale_shipment_grouping-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/it.po` & `trytond_sale_shipment_grouping-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/lo.po` & `trytond_sale_shipment_grouping-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/lt.po` & `trytond_sale_shipment_grouping-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/nl.po` & `trytond_sale_shipment_grouping-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/pl.po` & `trytond_sale_shipment_grouping-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/pt.po` & `trytond_sale_shipment_grouping-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/ro.po` & `trytond_sale_shipment_grouping-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 
 msgctxt "selection:party.party,sale_shipment_grouping_method:"
 msgid "Standard"
 msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/ru.po` & `trytond_sale_shipment_grouping-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/sl.po` & `trytond_sale_shipment_grouping-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/tr.po` & `trytond_sale_shipment_grouping-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/uk.po` & `trytond_sale_shipment_grouping-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/locale/zh_CN.po` & `trytond_sale_shipment_grouping-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/party.py` & `trytond_sale_shipment_grouping-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-6.6.1/sale.py` & `trytond_sale_shipment_grouping-6.8.0/sale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from itertools import groupby
 
-from trytond.pool import PoolMeta
+from trytond.pool import Pool, PoolMeta
 from trytond.transaction import Transaction
 
 
 class Sale(metaclass=PoolMeta):
     __name__ = 'sale.sale'
 
     @property
     def shipment_grouping_method(self):
         return self.party.sale_shipment_grouping_method
 
     @property
     def _shipment_grouping_state(self):
         return ['draft', 'waiting']
 
-    @property
-    def _shipment_grouping_fields(self):
-        return ('customer', 'delivery_address', 'company', 'warehouse')
+    def _get_shipment_grouping_fields(self, shipment):
+        pool = Pool()
+        ShipmentOut = pool.get('stock.shipment.out')
+        fields = ['customer', 'company', 'warehouse']
+        if isinstance(shipment, ShipmentOut):
+            fields.append('delivery_address')
+        return fields
 
     def _get_grouped_shipment_planned_date(self, shipment):
         return [('planned_date', '=', shipment.planned_date)]
 
-    def _get_grouped_shipment_order(self):
+    def _get_grouped_shipment_order(self, Shipment):
         "Returns the order used to find shipments that should be grouped"
         return None
 
     def _get_grouped_shipment_domain(self, shipment):
         "Returns a domain that will find shipments that should be grouped"
         Shipment = shipment.__class__
         shipment_domain = [
             ('moves.origin', 'like', 'sale.line,%'),
             ('state', 'in', self._shipment_grouping_state),
             ]
         shipment_domain += self._get_grouped_shipment_planned_date(shipment)
-        fields = [
-            f for f in self._shipment_grouping_fields if f in Shipment._fields]
+        fields = self._get_shipment_grouping_fields(shipment)
         defaults = Shipment.default_get(fields, with_rec_name=False)
         for field in fields:
             shipment_domain.append((field, '=',
                     getattr(shipment, field, defaults.get(field))))
         return shipment_domain
 
-    def _get_shipment_sale(self, shipment_type, values):
+    def _get_shipment_sale(self, Shipment, values):
         transaction = Transaction()
         context = transaction.context
-        shipment = super(Sale, self)._get_shipment_sale(shipment_type, values)
+        shipment = super(Sale, self)._get_shipment_sale(Shipment, values)
         if (not context.get('skip_grouping', False)
                 and self.shipment_grouping_method):
             with transaction.set_context(skip_grouping=True):
-                shipment = self._get_shipment_sale(shipment_type, values)
-            Shipment = shipment.__class__
+                shipment = self._get_shipment_sale(Shipment, values)
             domain = self._get_grouped_shipment_domain(shipment)
-            order = self._get_grouped_shipment_order()
+            order = self._get_grouped_shipment_order(Shipment)
             grouped_shipments = Shipment.search(domain, order=order, limit=1)
             if grouped_shipments:
                 shipment, = grouped_shipments
         return shipment
 
     @classmethod
     def _process_shipment(cls, sales):
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/setup.py` & `trytond_sale_shipment_grouping-6.8.0/setup.py`

 * *Files 3% similar despite different names*

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
@@ -50,22 +47,22 @@
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module to group sale stock moves',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_shipment_grouping',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale shipment grouping',
     package_dir={'trytond.modules.sale_shipment_grouping': '.'},
     packages=(
         ['trytond.modules.sale_shipment_grouping']
         + ['trytond.modules.sale_shipment_grouping.%s' % p
             for p in find_packages()]
@@ -102,24 +99,24 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/tests/scenario_sale_shipment_grouping.rst` & `trytond_sale_shipment_grouping-6.8.0/tests/scenario_sale_shipment_grouping.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-==============================
-Sale Invoice Grouping Scenario
-==============================
+===============================
+Sale Shipment Grouping Scenario
+===============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_grouping')
 
 Create company::
 
@@ -146,15 +143,15 @@
 
     >>> set_user(stock_user)
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> shipments = ShipmentOut.find([('customer', '=', customer.id)])
     >>> len(shipments)
     2
     >>> for shipment in shipments:
-    ...     _ = shipment.click('assign_try')
+    ...     shipment.click('assign_try')
     ...     shipment.click('pick')
     ...     shipment.click('pack')
     ...     shipment.click('done')
 
 Now we'll use the same scenario with the grouped customer::
 
     >>> set_user(sale_user)
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/tests/scenario_sale_shipment_grouping_multiple.rst` & `trytond_sale_shipment_grouping-6.8.0/tests/scenario_sale_shipment_grouping_multiple.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-=======================================
-Sale Invoice Grouping Multiple Scenario
-=======================================
+========================================
+Sale Shipment Grouping Multiple Scenario
+========================================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/PKG-INFO` & `trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-shipment-grouping
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to group sale stock moves
 Home-page: http://www.tryton.org/
-Download-URL: http://dowloads.tryton.org/6.6/
+Download-URL: http://dowloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_shipment_grouping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale shipment grouping
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
 
 Sale Shipment Grouping Module
 #############################
 
 The ``sale_shipment_grouping`` module adds an option to define how stock moves
```

### Comparing `trytond_sale_shipment_grouping-6.6.1/trytond_sale_shipment_grouping.egg-info/SOURCES.txt` & `trytond_sale_shipment_grouping-6.8.0/trytond_sale_shipment_grouping.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_shipment_grouping.rst
 ./tests/scenario_sale_shipment_grouping_multiple.rst
+./tests/scenario_sale_shipment_grouping_return.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/configuration_form.xml
 ./view/party_form.xml
 doc/conf.py
 doc/index.rst
 locale/bg.po
@@ -75,14 +76,15 @@
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_sale_shipment_grouping.rst
 tests/scenario_sale_shipment_grouping_multiple.rst
+tests/scenario_sale_shipment_grouping_return.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_sale_shipment_grouping.egg-info/PKG-INFO
 trytond_sale_shipment_grouping.egg-info/SOURCES.txt
 trytond_sale_shipment_grouping.egg-info/dependency_links.txt
 trytond_sale_shipment_grouping.egg-info/entry_points.txt
 trytond_sale_shipment_grouping.egg-info/not-zip-safe
```

