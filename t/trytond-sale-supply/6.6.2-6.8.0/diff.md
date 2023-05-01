# Comparing `tmp/trytond_sale_supply-6.6.2.tar.gz` & `tmp/trytond_sale_supply-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply-6.6.2.tar", last modified: Sun Feb  5 21:07:38 2023, max compression
+gzip compressed data, was "trytond_sale_supply-6.8.0.tar", last modified: Mon May  1 11:47:47 2023, max compression
```

## Comparing `trytond_sale_supply-6.6.2.tar` & `trytond_sale_supply-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:07:38.979506 trytond_sale_supply-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     1987 2023-02-05 21:07:35.000000 trytond_sale_supply-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-02-05 21:07:35.000000 trytond_sale_supply-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-02-05 21:07:38.979506 trytond_sale_supply-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      590 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:07:38.976173 trytond_sale_supply-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:07:38.976173 trytond_sale_supply-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      875 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      809 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      916 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      785 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      966 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      809 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      809 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      851 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      766 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      875 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      951 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      766 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3516 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9859 2023-02-05 20:48:28.000000 trytond_sale_supply-6.6.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:07:38.979506 trytond_sale_supply-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4363 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2135 2023-02-05 20:48:28.000000 trytond_sale_supply-6.6.2/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:07:38.976173 trytond_sale_supply-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7966 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/tests/scenario_sale_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/tests/scenario_sale_supply_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2023-01-15 17:47:37.000000 trytond_sale_supply-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:07:38.979506 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-02-05 21:07:38.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1661 2023-02-05 21:07:38.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:07:38.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-02-05 21:07:38.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-15 17:47:29.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-02-05 21:07:38.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:07:38.000000 trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:07:38.976173 trytond_sale_supply-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2022-12-19 12:02:58.000000 trytond_sale_supply-6.6.2/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2022-12-19 12:02:57.000000 trytond_sale_supply-6.6.2/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2103 2023-05-01 11:05:13.000000 trytond_sale_supply-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:05:13.000000 trytond_sale_supply-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.190351 trytond_sale_supply-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.187018 trytond_sale_supply-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1885 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1898 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1809 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1852 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1628 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1728 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-04-30 10:46:36.000000 trytond_sale_supply-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2629 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3494 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11814 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4391 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.190351 trytond_sale_supply-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7845 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3849 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3356 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/scenario_sale_supply_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-05-01 11:05:07.000000 trytond_sale_supply-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.193684 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-05-01 11:47:47.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:46.000000 trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:47.190351 trytond_sale_supply-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_sale_supply-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-01-16 14:00:21.000000 trytond_sale_supply-6.8.0/view/template_form.xml
```

### Comparing `trytond_sale_supply-6.6.2/CHANGELOG` & `trytond_sale_supply-6.8.0/CHANGELOG`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-Version 6.6.2 - 2023-02-05
---------------------------
-* Bug fixes (see mercurial logs for details)
 
-Version 6.6.1 - 2023-01-15
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Add stock_first option to supply_on_sale
+* Change supply_on_sale into selection
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Notify when product is supplied on sale and has purchase order point
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_supply-6.6.2/COPYRIGHT` & `trytond_sale_supply-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.6.2/LICENSE` & `trytond_sale_supply-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.6.2/PKG-INFO` & `trytond_sale_supply-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for sale supply
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_supply
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale supply
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,31 +38,32 @@
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
 
 Sale Supply Module
 ##################
 
 The Sale Supply module adds a "supply on sale option" to purchasable products.
-If checked, it will generate a purchase request for each sale line of this
-product regardless of the stock levels. Once the purchased products are
-received they are assigned on the customer shipments.
+If selected, it will generate a purchase request for each sale line of this
+product depending of the option and the stock levels.
+Once the purchased products are received they are assigned on the customer
+shipments.
 If the purchase is cancelled the sale goes back to the default supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the purchase request will be
     created only when all the invoice lines are paid
 ..
```

### Comparing `trytond_sale_supply-6.6.2/README.rst` & `trytond_sale_supply-6.8.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Sale Supply Module
 ##################
 
 The Sale Supply module adds a "supply on sale option" to purchasable products.
-If checked, it will generate a purchase request for each sale line of this
-product regardless of the stock levels. Once the purchased products are
-received they are assigned on the customer shipments.
+If selected, it will generate a purchase request for each sale line of this
+product depending of the option and the stock levels.
+Once the purchased products are received they are assigned on the customer
+shipments.
 If the purchase is cancelled the sale goes back to the default supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the purchase request will be
     created only when all the invoice lines are paid
 ..
```

### Comparing `trytond_sale_supply-6.6.2/__init__.py` & `trytond_sale_supply-6.8.0/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,7 +15,10 @@
         stock.ShipmentIn,
         product.Template,
         product.Product,
         module='sale_supply', type_='model')
     Pool.register(
         purchase.HandlePurchaseCancellationException,
         module='sale_supply', type_='wizard')
+    Pool.register(
+        stock.OrderPoint,
+        module='sale_supply', type_='model', depends=['stock_supply'])
```

### Comparing `trytond_sale_supply-6.6.2/doc/conf.py` & `trytond_sale_supply-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_supply-6.6.2/doc/index.rst` & `trytond_sale_supply-6.8.0/doc/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Sale Supply Module
 ##################
 
 The Sale Supply module adds a "supply on sale option" to purchasable products.
-If checked, it will generate a purchase request for each sale line of this
-product regardless of the stock levels. Once the purchased products are
-received they are assigned on the customer shipments.
+If selected, it will generate a purchase request for each sale line of this
+product depending of the option and the stock levels.
+Once the purchased products are received they are assigned on the customer
+shipments.
 If the purchase is cancelled the sale goes back to the default supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the purchase request will be
     created only when all the invoice lines are paid
 ..
```

### Comparing `trytond_sale_supply-6.6.2/locale/ca.po` & `trytond_sale_supply-6.8.0/locale/ca.po`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,48 @@
 msgid "Supply State"
 msgstr "Estat subministrament"
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr "Sol·licituds de compra"
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr "El producte \"%(product)s\" es subministra a la venda."
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+"El producte te regles d'aprovisionament de compra \"%(order_point)s\" "
+"definits."
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr "Sempre"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr "Mai"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr "Primer existències"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr "Sempre"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr "Mai"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr "Primer existències"
+
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
 msgstr "Cancel·lat"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
 msgstr "Sol·licitat"
```

### Comparing `trytond_sale_supply-6.6.2/locale/cs.po` & `trytond_sale_supply-6.8.0/locale/et.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,74 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Müügitarne"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Müügitarne"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr ""
+msgstr "Müügirida"
 
-#, fuzzy
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Purchase Requests"
+msgstr "Ostupäring"
 
+#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr ""
+msgstr "Müügitarne"
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
-msgstr "Purchase Requests"
+msgstr "Ostupäringud"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
 
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Tühista"
 
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr ""
+msgstr "Päritud"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_supply-6.6.2/locale/es.po` & `trytond_sale_supply-6.8.0/locale/es.po`

 * *Files 26% similar despite different names*

```diff
@@ -22,18 +22,52 @@
 msgid "Supply State"
 msgstr "Estado suministro"
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr "Solicitudes de compra"
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr "El producto \"%(product)s\" se subministra en la venta."
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+"El producto tiene reglas de abastecimientod e compra \"%(order_point)s\" "
+"definidos."
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr "Siempre"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr "Nunca"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr "Primero existencias"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr "Siempre"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr "Nunca"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr "Primero existencias"
+
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
 msgstr "Cancelado"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
 msgstr "Solicitado"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
-msgstr "Subministrado"
+msgstr "Suministrado"
```

### Comparing `trytond_sale_supply-6.6.2/locale/es_419.po` & `trytond_sale_supply-6.8.0/locale/pt.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,73 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Abastecimento Na Venda"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Abastecimento Na Venda"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr ""
+msgstr "Linhas de Venda"
 
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr ""
+msgstr "Pedido de Compra"
 
+#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr ""
+msgstr "Abastecimento Na Venda"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
+msgstr "Purchase Requests"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
 msgstr ""
 
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancelar"
 
 #, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
 msgstr "Solicitado"
 
 msgctxt "selection:sale.line,supply_state:"
```

### Comparing `trytond_sale_supply-6.6.2/locale/et.po` & `trytond_sale_supply-6.8.0/locale/fa.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,74 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Müügitarne"
+msgstr "عرضه در فروش"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Müügitarne"
+msgstr "عرضه در فروش"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr "Müügirida"
+msgstr "سطرهای فروش"
 
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Ostupäring"
+msgstr "درخواست خرید"
 
 #, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr "Müügitarne"
+msgstr "عرضه در فروش"
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
-msgstr "Ostupäringud"
+msgstr "درخواست های خرید"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr "Tühista"
+msgstr "انصراف"
 
 #, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr "Päritud"
+msgstr "درخواست شده"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
 msgstr ""
```

### Comparing `trytond_sale_supply-6.6.2/locale/fa.po` & `trytond_sale_supply-6.8.0/locale/nl.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,72 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "عرضه در فروش"
+msgstr "Inkopen Bij Verkoop"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "عرضه در فروش"
+msgstr "Inkopen Bij Verkoop"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr "سطرهای فروش"
+msgstr "Verkoop Regels"
 
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "درخواست خرید"
+msgstr "Inkoop Aanvraag"
 
-#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr "عرضه در فروش"
+msgstr "Lever Status"
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
-msgstr "درخواست های خرید"
+msgstr "Inkoop Aanvragen"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr "Het product \"%(product)s\" is aangeleverd voor verkoop."
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+"Op het product zijn inkoop order niveaus \"%(order_points)s\" gedefinieerd."
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr "Altijd"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr "Nooit"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr "Voorraad eerst"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr "Altijd"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr "Nooit"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr "Voorraad eerst"
 
-#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr "انصراف"
+msgstr "Geannuleerd"
 
-#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr "درخواست شده"
+msgstr "Aangevraagd"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
-msgstr ""
+msgstr "Geleverd"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_supply-6.6.2/locale/fi.po` & `trytond_sale_supply-6.8.0/locale/tr.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,78 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Satış Tedariği"
 
+#, fuzzy
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Satış Tedariği"
 
+#, fuzzy
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr ""
+msgstr "Satış Kanalları"
 
-#, fuzzy
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Purchase Requests"
+msgstr "Satınalma Talebi"
 
+#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr ""
+msgstr "Satış Tedariği"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr "Purchase Requests"
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Vazgeç"
 
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr ""
+msgstr "Talep Edilen"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_supply-6.6.2/locale/id.po` & `trytond_sale_supply-6.8.0/locale/ru.po`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,64 @@
 msgid "Supply On Sale"
 msgstr ""
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr ""
+msgstr "Запрос на покупку"
 
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
+msgstr "Запросы на покупку"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr "Dibatalkan"
+msgstr "Отменить"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
 msgstr ""
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_supply-6.6.2/locale/lt.po` & `trytond_sale_supply-6.8.0/locale/sl.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,75 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Dobava ob prodaji"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr ""
+msgstr "Dobava ob prodaji"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr ""
+msgstr "Prodajne postavke"
 
-#, fuzzy
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Purchase Requests"
+msgstr "Nabavni zahtevek"
 
+#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr ""
+msgstr "Dobava ob prodaji"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr "Purchase Requests"
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Preklicano"
 
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr ""
+msgstr "Zahtevano"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
 msgstr ""
```

### Comparing `trytond_sale_supply-6.6.2/locale/pt.po` & `trytond_sale_supply-6.8.0/locale/de.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,72 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Abastecimento Na Venda"
+msgstr "Beschaffung bei Verkauf"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Abastecimento Na Venda"
+msgstr "Beschaffung bei Verkauf"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr "Linhas de Venda"
+msgstr "Verkaufspositionen"
 
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Pedido de Compra"
+msgstr "Bestellvorschlag"
 
-#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr "Abastecimento Na Venda"
+msgstr "Beschaffungsstatus"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
-msgstr "Purchase Requests"
+msgstr "Bestellvorschläge"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr "Der Artikel \"%(product)s\" wird bei Bestellung beschafft."
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+"Für den Artikel sind Einkaufsbestellpunkte \"%(order_points)s\" definiert."
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr "Immer"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr "Niemals"
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr "Lagerbestand Zuerst"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr "Immer"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr "Niemals"
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr "Lagerbestand Zuerst"
 
-#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr "Cancelar"
+msgstr "Annulliert"
 
-#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr "Solicitado"
+msgstr "Angefragt"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
-msgstr ""
+msgstr "Beschafft"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_supply-6.6.2/locale/ro.po` & `trytond_sale_supply-6.8.0/locale/es_419.po`

 * *Files 18% similar despite different names*

```diff
@@ -22,18 +22,51 @@
 msgid "Supply State"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr ""
+msgstr "Solicitado"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
 msgstr ""
```

### Comparing `trytond_sale_supply-6.6.2/locale/sl.po` & `trytond_sale_supply-6.8.0/locale/it.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Dobava ob prodaji"
+msgstr "forniture in vendita"
 
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Dobava ob prodaji"
+msgstr "forniture in vendita"
 
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr "Prodajne postavke"
+msgstr "Righe di vendita"
 
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Nabavni zahtevek"
+msgstr "Richiesta di acquisto"
 
-#, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr "Dobava ob prodaji"
+msgstr "Stato della fornitura"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
-msgstr "Purchase Requests"
+msgstr "Richiesta acquisti"
+
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr "Preklicano"
+msgstr "Annullato"
 
-#, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr "Zahtevano"
+msgstr "Richiesto"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
-msgstr ""
+msgstr "Fornito"
```

### Comparing `trytond_sale_supply-6.6.2/locale/tr.po` & `trytond_sale_supply-6.8.0/locale/lo.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,75 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:product.product,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Satış Tedariği"
+msgstr "ສະໜອງການຂາຍ"
 
-#, fuzzy
 msgctxt "field:product.template,supply_on_sale:"
 msgid "Supply On Sale"
-msgstr "Satış Tedariği"
+msgstr "ສະໜອງການຂາຍ"
 
-#, fuzzy
 msgctxt "field:purchase.request,sale_lines:"
 msgid "Sale Lines"
-msgstr "Satış Kanalları"
+msgstr "ລາຍການຂາຍ"
 
 msgctxt "field:sale.line,purchase_request:"
 msgid "Purchase Request"
-msgstr "Satınalma Talebi"
+msgstr "ຕ້ອງການສັ່ງຊື້"
 
 #, fuzzy
 msgctxt "field:sale.line,supply_state:"
 msgid "Supply State"
-msgstr "Satış Tedariği"
+msgstr "ສະໜອງການຂາຍ"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr "Purchase Requests"
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
 #, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr "Vazgeç"
+msgstr "ຍົກເລີກ"
 
 #, fuzzy
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
-msgstr "Talep Edilen"
+msgstr "ສັ່ງແລ້ວ"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
 msgstr ""
```

### Comparing `trytond_sale_supply-6.6.2/locale/uk.po` & `trytond_sale_supply-6.8.0/locale/id.po`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,49 @@
 msgid "Supply State"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_request_form"
 msgid "Purchase Requests"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_order_point_product_supply_on_sale"
+msgid "The product \"%(product)s\" is supplied on sale."
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_template_supply_on_sale_order_point"
+msgid "The product has purchase order points \"%(order_points)s\" defined."
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.product,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Always"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Never"
+msgstr ""
+
+msgctxt "selection:product.template,supply_on_sale:"
+msgid "Stock First"
+msgstr ""
+
 msgctxt "selection:sale.line,supply_state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Dibatalkan"
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Requested"
 msgstr ""
 
 msgctxt "selection:sale.line,supply_state:"
 msgid "Supplied"
```

### Comparing `trytond_sale_supply-6.6.2/purchase.py` & `trytond_sale_supply-6.8.0/purchase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from functools import wraps
 
 from trytond.model import ModelView, Workflow, fields
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 
 class Request(metaclass=PoolMeta):
     __name__ = 'purchase.request'
 
     sale_lines = fields.One2Many(
         'sale.line', 'purchase_request', "Sale Lines", readonly=True)
@@ -22,15 +22,15 @@
     def delete(cls, requests):
         pool = Pool()
         Sale = pool.get('sale.sale')
         SaleLine = pool.get('sale.line')
         transaction = Transaction()
         context = transaction.context
 
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             reqs = cls.browse(requests)
             sales = set(r.origin for r in reqs if isinstance(r.origin, Sale))
             sale_lines = [l for r in reqs for l in r.sale_lines]
             if sale_lines:
                 SaleLine.write(sale_lines, {
                         'purchase_request': None,
                         })
@@ -49,15 +49,15 @@
         pool = Pool()
         Request = pool.get('purchase.request')
         Sale = pool.get('sale.sale')
         transaction = Transaction()
         context = transaction.context
 
         sales = set()
-        with transaction.set_context(_check_access=False):
+        with without_check_access():
             for sub_purchases in grouped_slice(purchases):
                 ids = [x.id for x in sub_purchases]
                 requests = Request.search([
                         ('purchase_line.purchase.id', 'in', ids),
                         ('origin', 'like', 'sale.sale,%'),
                         ])
                 sales.update(r.origin.id for r in requests)
```

### Comparing `trytond_sale_supply-6.6.2/sale.py` & `trytond_sale_supply-6.8.0/sale.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+
+from collections import defaultdict
+from itertools import groupby
+from operator import attrgetter
+
 from trytond.model import Model, fields
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 from trytond.transaction import Transaction
 
 
 class Sale(metaclass=PoolMeta):
@@ -16,42 +21,63 @@
                     for l in self.lines if l.supply_on_sale):
                 return False
         return done
 
     @classmethod
     def _process_shipment(cls, sales):
         pool = Pool()
+        Product = pool.get('product.product')
+
+        product_quantities = defaultdict(float)
+        get_warehouse = attrgetter('warehouse')
+        for warehouse, sub_sales in groupby(
+                filter(get_warehouse, sales), key=get_warehouse):
+            products = {
+                l.product for s in sub_sales for l in s.lines
+                if l.product and l.product.supply_on_sale == 'stock_first'}
+            locations = [warehouse.id]
+            with Transaction().set_context(
+                    locations=locations, stock_date_end=None):
+                products = Product.browse(products)
+                product_quantities.update(
+                    (p, min(p.quantity, p.forecast_quantity))
+                    for p in Product.browse(products))
+
+        # purchase requests must be created before shipments to get information
+        # about requests during the shipments creation like the supplier
+        cls._process_supply(sales, product_quantities)
+        super()._process_shipment(sales)
+
+    @classmethod
+    def _process_supply(cls, sales, product_quantities):
+        pool = Pool()
         Line = pool.get('sale.line')
         Move = pool.get('stock.move')
         PurchaseRequest = pool.get('purchase.request')
         ShipmentOut = pool.get('stock.shipment.out')
 
         requests, lines = [], []
         moves_to_draft, shipments_to_wait = [], []
         for sale in sales:
-            # purchase requests must be created before shipments to get
-            # information about requests during the shipments creation
-            # like the supplier
-            reqs, lns = sale.create_purchase_requests()
+            reqs, lns = sale.create_purchase_requests(product_quantities)
             requests.extend(reqs)
             lines.extend(lns)
 
             moves, shipments = sale.create_move_from_supply()
             moves_to_draft.extend(moves)
             shipments_to_wait.extend(shipments)
         PurchaseRequest.save(requests)
         Line.save(lines)
         Move.draft(moves_to_draft)
         ShipmentOut.wait(shipments_to_wait)
-        super()._process_shipment(sales)
 
-    def create_purchase_requests(self):
+    def create_purchase_requests(self, product_quantities):
         requests, lines = [], []
         for line in self.lines:
-            request = line.get_purchase_request()
+            request = line.get_purchase_request(product_quantities)
             if not request:
                 continue
             requests.append(request)
             assert not line.purchase_request
             line.purchase_request = request
             lines.append(line)
         return requests, lines
@@ -117,58 +143,82 @@
         if (self.type != 'line'
                 or self.sale.shipment_method == 'manual'
                 or not self.product
                 or self.quantity <= 0
                 or any(m.state not in ['staging', 'cancelled']
                     for m in self.moves)):
             return False
-        return self.product.supply_on_sale
+        return bool(self.product.supply_on_sale)
+
+    @property
+    def ready_for_supply(self):
+        if self.sale.shipment_method == 'invoice':
+            # Ensure to create the request for the maximum paid
+            invoice_skips = (
+                set(self.sale.invoices_ignored)
+                | set(self.sale.invoices_recreated))
+            invoice_lines = [
+                l for l in self.invoice_lines
+                if l.invoice not in invoice_skips]
+            if (not invoice_lines
+                    or any(
+                        (not l.invoice) or l.invoice.state != 'paid'
+                        for l in invoice_lines)):
+                return False
+        return True
 
     def get_move(self, shipment_type):
         move = super().get_move(shipment_type)
         if (move
                 and shipment_type == 'out'
-                and (self.supply_on_sale or self.has_supply)):
+                and self.has_supply):
             if self.supply_state in {'', 'requested'}:
                 move.state = 'staging'
         return move
 
+    def _get_move_quantity(self, shipment_type):
+        quantity = super()._get_move_quantity(shipment_type)
+        if self.supply_on_sale and not self.ready_for_supply:
+            quantity = 0
+        return quantity
+
     def _get_purchase_request_product_supplier_pattern(self):
         return {
             'company': self.sale.company.id,
             }
 
-    def get_purchase_request(self):
-        'Return purchase request for the sale line'
+    def get_purchase_request(self, product_quantities):
+        """Return purchase request for the sale line
+        depending on the product quantities"""
         pool = Pool()
         Uom = pool.get('product.uom')
         Request = pool.get('purchase.request')
 
         if (not self.supply_on_sale
                 or self.purchase_request
+                or not self.ready_for_supply
                 or not self.product.purchasable):
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
+            if available_qty > 0:
+                product_quantities[product] -= Uom.compute_qty(
+                    self.unit, quantity, product.default_uom, round=False)
                 return
 
-        product = self.product
         supplier, purchase_date = Request.find_best_supplier(product,
             self.shipping_date,
             **self._get_purchase_request_product_supplier_pattern())
         uom = product.purchase_uom or product.default_uom
-        quantity = self._get_move_quantity('out')
         quantity = Uom.compute_qty(self.unit, quantity, uom)
         return Request(
             product=product,
             party=supplier,
             quantity=quantity,
             uom=uom,
             computed_quantity=quantity,
```

### Comparing `trytond_sale_supply-6.6.2/sale.xml` & `trytond_sale_supply-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.6.2/setup.py` & `trytond_sale_supply-6.8.0/setup.py`

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
@@ -34,38 +31,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_supply'
 
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
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond_stock_supply'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module for sale supply',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_supply',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale supply',
     package_dir={'trytond.modules.sale_supply': '.'},
     packages=(
         ['trytond.modules.sale_supply']
         + ['trytond.modules.sale_supply.%s' % p for p in find_packages()]
         ),
@@ -101,24 +104,24 @@
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

### Comparing `trytond_sale_supply-6.6.2/stock.py` & `trytond_sale_supply-6.8.0/stock.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from collections import defaultdict
 
-from trytond.model import Model, ModelView, Workflow
+from trytond.i18n import gettext
+from trytond.model import Model, ModelView, Workflow, fields
 from trytond.pool import Pool, PoolMeta
 
 
 class ShipmentIn(metaclass=PoolMeta):
     __name__ = 'stock.shipment.in'
 
     @classmethod
@@ -52,7 +53,26 @@
         else:
             inventory_moves = self.inventory_moves
         for move in filter(filter_func, inventory_moves):
             pbl[move.product][get_key(move)] += move.internal_quantity
         for sale_line in sale_lines:
             sale_line.assign_supplied(
                 pbl[sale_line.product], grouping=grouping)
+
+
+class OrderPoint(metaclass=PoolMeta):
+    __name__ = 'stock.order_point'
+
+    @fields.depends(methods=['_notify_product_supply_on_sale'])
+    def on_change_notify(self):
+        notifications = super().on_change_notify()
+        notifications.extend(self._notify_product_supply_on_sale())
+        return notifications
+
+    @fields.depends('type', 'product')
+    def _notify_product_supply_on_sale(self):
+        if (self.type == 'purchase'
+                and self.product and self.product.supply_on_sale):
+            yield ('warning', gettext(
+                    'sale_supply'
+                    '.msg_order_point_product_supply_on_sale',
+                    product=self.product.rec_name))
```

### Comparing `trytond_sale_supply-6.6.2/tests/scenario_sale_supply.rst` & `trytond_sale_supply-6.8.0/tests/scenario_sale_supply.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 ====================
 Sale Supply Scenario
 ====================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
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
 
     >>> config = activate_modules(['sale_supply', 'sale', 'purchase'])
 
 Create company::
 
@@ -98,15 +95,15 @@
     >>> template = ProductTemplate()
     >>> template.name = 'product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.purchasable = True
     >>> template.salable = True
     >>> template.list_price = Decimal('10')
-    >>> template.supply_on_sale = True
+    >>> template.supply_on_sale = 'always'
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
 
 Create payment term::
 
     >>> payment_term = create_payment_term()
@@ -207,15 +204,15 @@
     >>> changing_template.name = 'product'
     >>> changing_template.default_uom = unit
     >>> changing_template.type = 'goods'
     >>> changing_template.purchasable = True
     >>> changing_template.salable = True
     >>> changing_template.list_price = Decimal('10')
     >>> changing_template.account_category = account_category
-    >>> changing_template.supply_on_sale = False
+    >>> changing_template.supply_on_sale = None
     >>> changing_template.save()
     >>> changing_product, = changing_template.products
 
     >>> set_user(sale_user)
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
     >>> sale.party = customer
@@ -242,20 +239,19 @@
     >>> inventory_line.quantity = 100.0
     >>> inventory_line.expected_quantity = 0.0
     >>> inventory.save()
     >>> inventory.click('confirm')
     >>> inventory.state
     'done'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> shipment.click('pack')
 
     >>> set_user(admin_user)
-    >>> changing_template.supply_on_sale = True
+    >>> changing_template.supply_on_sale = 'always'
     >>> changing_template.save()
 
     >>> set_user(stock_user)
     >>> shipment.click('done')
     >>> set_user(purchase_user)
     >>> len(PurchaseRequest.find([('product', '=', changing_product.id)]))
     0
```

### Comparing `trytond_sale_supply-6.6.2/tests/scenario_sale_supply_shipment_on_invoice.rst` & `trytond_sale_supply-6.8.0/tests/scenario_sale_supply_shipment_on_invoice.rst`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     >>> template = ProductTemplate()
     >>> template.name = 'product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.salable = True
     >>> template.purchasable = True
     >>> template.list_price = Decimal('10')
-    >>> template.supply_on_sale = True
+    >>> template.supply_on_sale = 'always'
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
 
 Sale 5 products with shipment method on invoice::
 
     >>> Sale = Model.get('sale.sale')
@@ -99,29 +99,29 @@
     >>> sale_line.purchase_request
 
 Pay for 4 products::
 
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity = 4
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
 
 Not yet a purchase request::
 
     >>> sale_line.reload()
     >>> sale_line.purchase_request
 
 Pay for remaining products::
 
     >>> sale.reload()
     >>> _, invoice = sale.invoices
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
 
 Check purchase request::
 
     >>> sale_line.reload()
     >>> bool(sale_line.purchase_request)
```

### Comparing `trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/PKG-INFO` & `trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-supply
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for sale supply
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_supply
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale supply
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,31 +38,32 @@
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
 
 Sale Supply Module
 ##################
 
 The Sale Supply module adds a "supply on sale option" to purchasable products.
-If checked, it will generate a purchase request for each sale line of this
-product regardless of the stock levels. Once the purchased products are
-received they are assigned on the customer shipments.
+If selected, it will generate a purchase request for each sale line of this
+product depending of the option and the stock levels.
+Once the purchased products are received they are assigned on the customer
+shipments.
 If the purchase is cancelled the sale goes back to the default supply method.
 
 .. warning::
     If the shiment method is *On Invoice Paid*, the purchase request will be
     created only when all the invoice lines are paid
 ..
```

### Comparing `trytond_sale_supply-6.6.2/trytond_sale_supply.egg-info/SOURCES.txt` & `trytond_sale_supply-6.8.0/trytond_sale_supply.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
+message.xml
 product.py
 product.xml
 purchase.py
 sale.py
 sale.xml
 setup.py
 stock.py
 tox.ini
 tryton.cfg
 ./__init__.py
+./message.xml
 ./product.py
 ./product.xml
 ./purchase.py
 ./sale.py
 ./sale.xml
 ./stock.py
 ./tryton.cfg
@@ -43,15 +45,17 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_supply.rst
+./tests/scenario_sale_supply_notifications.rst
 ./tests/scenario_sale_supply_shipment_on_invoice.rst
+./tests/scenario_sale_supply_stock_first.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/sale_line_form.xml
 ./view/template_form.xml
 doc/conf.py
 doc/index.rst
 locale/bg.po
@@ -76,15 +80,17 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_sale_supply.rst
+tests/scenario_sale_supply_notifications.rst
 tests/scenario_sale_supply_shipment_on_invoice.rst
+tests/scenario_sale_supply_stock_first.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_sale_supply.egg-info/PKG-INFO
 trytond_sale_supply.egg-info/SOURCES.txt
 trytond_sale_supply.egg-info/dependency_links.txt
 trytond_sale_supply.egg-info/entry_points.txt
 trytond_sale_supply.egg-info/not-zip-safe
```

