# Comparing `tmp/trytond_carrier_weight-6.6.0.tar.gz` & `tmp/trytond_carrier_weight-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_weight-6.6.0.tar", last modified: Mon Oct 31 16:26:47 2022, max compression
+gzip compressed data, was "trytond_carrier_weight-6.8.0.tar", last modified: Mon May  1 11:41:49 2023, max compression
```

## Comparing `trytond_carrier_weight-6.6.0.tar` & `trytond_carrier_weight-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:47.614250 trytond_carrier_weight-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_carrier_weight-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_carrier_weight-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-31 16:26:46.000000 trytond_carrier_weight-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_carrier_weight-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1844 2022-10-31 16:26:45.000000 trytond_carrier_weight-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2022-10-31 16:26:44.000000 trytond_carrier_weight-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_carrier_weight-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2510 2022-10-31 16:26:47.614250 trytond_carrier_weight-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2021-12-11 16:59:33.000000 trytond_carrier_weight-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4305 2022-10-11 19:49:57.000000 trytond_carrier_weight-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      993 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:47.614250 trytond_carrier_weight-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:47.610916 trytond_carrier_weight-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1654 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1746 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1801 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1478 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1632 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1921 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1767 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1741 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1453 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1799 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1603 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1756 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1460 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1569 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1462 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1505 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1514 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2022-10-29 07:50:34.000000 trytond_carrier_weight-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2022-09-12 22:47:25.000000 trytond_carrier_weight-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:26:47.614250 trytond_carrier_weight-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5350 2022-10-29 07:39:10.000000 trytond_carrier_weight-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2768 2021-12-11 16:59:33.000000 trytond_carrier_weight-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:47.610916 trytond_carrier_weight-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_carrier_weight-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7692 2022-09-29 07:07:37.000000 trytond_carrier_weight-6.6.0/tests/scenario_carrier_weight.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2650 2022-04-16 16:30:56.000000 trytond_carrier_weight-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_carrier_weight-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2022-10-31 15:10:09.000000 trytond_carrier_weight-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2022-10-31 16:26:43.000000 trytond_carrier_weight-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:47.614250 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2510 2022-10-31 16:26:47.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1666 2022-10-31 16:26:47.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:26:47.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 16:26:47.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:52.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2022-10-31 16:26:47.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:26:47.000000 trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:47.614250 trytond_carrier_weight-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/view/weight_price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2019-02-13 10:09:31.000000 trytond_carrier_weight-6.6.0/view/weight_price_list_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:49.799249 trytond_carrier_weight-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2047 2023-05-01 11:01:20.000000 trytond_carrier_weight-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-01 11:01:20.000000 trytond_carrier_weight-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_weight-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2469 2023-05-01 11:41:49.799249 trytond_carrier_weight-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4558 2023-04-21 08:36:08.000000 trytond_carrier_weight-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-01-16 14:00:20.000000 trytond_carrier_weight-6.8.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      993 2023-01-16 14:00:20.000000 trytond_carrier_weight-6.8.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:49.795916 trytond_carrier_weight-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:49.792582 trytond_carrier_weight-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1784 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2010 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2087 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1739 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1990 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1822 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1583 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1826 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1929 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1733 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2028 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1590 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1635 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1644 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2023-04-30 10:46:36.000000 trytond_carrier_weight-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:41:49.799249 trytond_carrier_weight-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4540 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:49.792582 trytond_carrier_weight-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7573 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/tests/scenario_carrier_weight.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3683 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_carrier_weight-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-05-01 11:01:15.000000 trytond_carrier_weight-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:49.799249 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2469 2023-05-01 11:41:48.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1640 2023-05-01 11:41:49.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:41:48.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:41:48.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 11:41:48.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:41:48.000000 trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:49.795916 trytond_carrier_weight-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_carrier_weight-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:20.000000 trytond_carrier_weight-6.8.0/view/weight_price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-01-16 14:00:20.000000 trytond_carrier_weight-6.8.0/view/weight_price_list_tree.xml
```

### Comparing `trytond_carrier_weight-6.6.0/CHANGELOG` & `trytond_carrier_weight-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Support having a price without weight
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
```

### Comparing `trytond_carrier_weight-6.6.0/COPYRIGHT` & `trytond_carrier_weight-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2022 Cédric Krier.
+Copyright (C) 2011-2023 Cédric Krier.
 Copyright (C) 2011-2013 Bertrand Chenal.
-Copyright (C) 2011-2022 Nicolas Évrard.
-Copyright (C) 2011-2022 B2CK SPRL.
+Copyright (C) 2011-2023 Nicolas Évrard.
+Copyright (C) 2011-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_carrier_weight-6.6.0/LICENSE` & `trytond_carrier_weight-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-6.6.0/PKG-INFO` & `trytond_carrier_weight-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_weight
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add cost method "on weight" on carrier
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
-Project-URL: Source Code, https://hg.tryton.org/modules/carrier_weight
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier weight
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,23 +39,23 @@
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
 
 Carrier Weight Module
 #####################
 
 The carrier weight module adds a cost method based on weight.
-The price is computed by finding the line for which the weight is greater or
-equal but smaller than the next line.
+The price is computed by finding the first line for which the weight is
+greater.
```

### Comparing `trytond_carrier_weight-6.6.0/__init__.py` & `trytond_carrier_weight-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-6.6.0/carrier.py` & `trytond_carrier_weight-6.8.0/carrier.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         help="The currency of the price.")
     weight_price_list = fields.One2Many('carrier.weight_price_list', 'carrier',
         'Price List',
         states={
             'invisible': Eval('carrier_cost_method') != 'weight',
             'readonly': ~(Eval('weight_uom', 0) & Eval('weight_currency', 0)),
             },
-        help="Add price to the carrier service.")
+        help="Add price per weight to the carrier service.\n"
+        "The first line for which the weight is greater is used.\n"
+        "The line with weight of 0 is used as default price.")
 
     @classmethod
     def __setup__(cls):
         super(Carrier, cls).__setup__()
         selection = ('weight', 'Weight')
         if selection not in cls.carrier_cost_method.selection:
             cls.carrier_cost_method.selection.append(selection)
@@ -54,43 +56,52 @@
         return 2
 
     def compute_weight_price(self, weight):
         "Compute price based on weight"
         for line in reversed(self.weight_price_list):
             if line.weight < weight:
                 return line.price
+        else:
+            if not line.weight and not weight:
+                return line.price
         return Decimal(0)
 
+    def _get_weight_price(self):
+        weights = Transaction().context.get('weights', [])
+        if weights:
+            weight_price = sum(
+                self.compute_weight_price(w) for w in weights)
+        else:
+            weight_price = self.compute_weight_price(0)
+        return weight_price, self.weight_currency.id
+
     def get_sale_price(self):
         price, currency_id = super(Carrier, self).get_sale_price()
         if self.carrier_cost_method == 'weight':
-            weight_price = Decimal(0)
-            for weight in Transaction().context.get('weights', []):
-                weight_price += self.compute_weight_price(weight)
-            return weight_price, self.weight_currency.id
+            price, currency_id = self._get_weight_price()
         return price, currency_id
 
     def get_purchase_price(self):
         price, currency_id = super(Carrier, self).get_purchase_price()
         if self.carrier_cost_method == 'weight':
-            weight_price = Decimal(0)
-            for weight in Transaction().context.get('weights', []):
-                weight_price += self.compute_weight_price(weight)
-            return weight_price, self.weight_currency.id
+            price, currency_id = self._get_weight_price()
         return price, currency_id
 
 
 class WeightPriceList(ModelSQL, ModelView):
     'Carrier Weight Price List'
     __name__ = 'carrier.weight_price_list'
     carrier = fields.Many2One(
         'carrier', "Carrier", required=True,
         help="The carrier that the price list belongs to.")
     weight = fields.Float('Weight',
         digits=(16, Eval('_parent_carrier', {}).get('weight_uom_digits', 2)),
+        domain=[
+            ('weight', '>=', 0),
+            ],
         depends={'carrier'},
         help="The lower limit for the price.")
     price = Monetary(
         "Price", currency='currency', digits='currency',
         help="The price of the carrier service.")
 
     currency = fields.Function(fields.Many2One(
@@ -100,9 +111,8 @@
     @classmethod
     def __setup__(cls):
         super(WeightPriceList, cls).__setup__()
         cls._order.insert(0, ('weight', 'ASC'))
 
     @fields.depends('carrier', '_parent_carrier.weight_currency')
     def on_change_with_currency(self, name=None):
-        if self.carrier and self.carrier.weight_currency:
-            return self.carrier.weight_currency.id
+        return self.carrier.weight_currency if self.carrier else None
```

### Comparing `trytond_carrier_weight-6.6.0/carrier.xml` & `trytond_carrier_weight-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-6.6.0/common.py` & `trytond_carrier_weight-6.8.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-6.6.0/locale/bg.po` & `trytond_carrier_weight-6.8.0/locale/et.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Valuuta"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Ценова листа"
+msgstr "Hinnakiri"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "Мер. ед. за тегло"
+msgstr "Kaalu mõõtühik"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Цифри на мер. ед, за тегло"
+msgstr "Kaalu mõõtühiku numbriväärtus"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Превозвач"
+msgstr "Vedaja"
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Валута"
+msgstr "Valuuta"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Цена"
+msgstr "Hind"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Тегло"
+msgstr "Kaal"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr ""
+msgstr "Hinna valuuta."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr ""
+msgstr "Vedaja teenuse hind."
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr ""
+msgstr "Hinnale kehtim madalaim piirang"
 
-#, fuzzy
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Ценови лист на карго тегло"
+msgstr "Vedaja kaalu hinnakiri"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Тегло"
+msgstr "Kaal"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/ca.po` & `trytond_carrier_weight-6.8.0/locale/hu.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Pénznem"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Tarifa"
+msgstr "Fuvarozási árlista"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "UdM del pes"
+msgstr "Súly mértékegysége"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Decimals de la UdM del pes"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Transportista"
+msgstr "Fuvarozó"
 
+#, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Pénznem"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Preu"
+msgstr "Ár"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Pes"
+msgstr "Súly"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr "La moneda del preu."
+msgstr "Az árlista ebben a pénznemben van megadva."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Afegeix preus al servei del transportista."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
-msgstr "La unitat de pes utilitzada per la tarifa."
+msgstr ""
+"A fuvarozási árlistában a súlyok ebben a mértékegységben vannak megadva."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
-msgstr "El transportista al que pertany la tarifa."
+msgstr ""
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr "El preu del servei del transportista."
+msgstr "A fuvarozás díja."
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr "El límit inferior al que aplica el preu."
+msgstr "Az ár ettől a súlytól érvényes."
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Tarifa pes transportista"
+msgstr ""
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Pes"
+msgstr "súly"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/cs.po` & `trytond_carrier_weight-6.8.0/locale/es_419.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr ""
+msgstr "Lista de precios"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
 msgstr ""
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
@@ -35,15 +35,18 @@
 msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -56,12 +59,12 @@
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr ""
+msgstr "Lista de precio por peso de transportista"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
 msgstr ""
```

### Comparing `trytond_carrier_weight-6.6.0/locale/de.po` & `trytond_carrier_weight-6.8.0/locale/es.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Währung"
+msgstr "Moneda"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Preisliste"
+msgstr "Tarifa"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "Gewichtseinheit"
+msgstr "UdM del peso"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Nachkommastellen Gewichtseinheit"
+msgstr "Decimales de la UdM del peso"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Versanddienstleister"
+msgstr "Transportista"
 
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Währung"
+msgstr "Moneda"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Preis"
+msgstr "Precio"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Gewicht"
+msgstr "Peso"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr "Die Währung des Preises."
+msgstr "La moneda del precio."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Einen Preis zur Versanddienstleistung hinzufügen."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
+"Añade un precio por peso al servicio del transportista.\n"
+"Se utiliza la primera lína que el peso es superior.\n"
+"Una línea con peso 0 se utilizara como precio por defecto."
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
-msgstr "Die Gewichtseinheit für die Preisliste."
+msgstr "La unidad de peso utilizada por la tarifa."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
-msgstr "Der Versanddienstleister dem diese Preisliste zugeordnet ist."
+msgstr "El transportista al que pertenece la tarifa."
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr "Der Preis der Versanddienstleistung."
+msgstr "El precio del servicio del transportista."
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr "Die Untergrenze für den Preis."
+msgstr "El límite inferior al que aplica el precio."
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Preisliste Versandgewicht"
+msgstr "Tarifa peso transportista"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Gewicht"
+msgstr "Peso"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/es.po` & `trytond_carrier_weight-6.8.0/locale/fr.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Tarifa"
+msgstr "Liste de prix"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "UdM del peso"
+msgstr "UDM de poids"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Decimales de la UdM del peso"
+msgstr "Décimales de l'UDM de poids"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Transportista"
+msgstr "Transporteur"
 
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Precio"
+msgstr "Prix"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Peso"
+msgstr "Poids"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr "La moneda del precio."
+msgstr "La devise du prix."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Añade precios al servicio del transportista."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
+"Ajoutez le prix au poids au service de transport.\n"
+"La première ligne pour laquelle le poids est plus élevé est utilisée.\n"
+"La ligne avec un poids de 0 est utilisée comme prix par défaut."
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
-msgstr "La unidad de peso utilizada por la tarifa."
+msgstr "L'unit de poids des critères de la liste de prix."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
-msgstr "El transportista al que pertenece la tarifa."
+msgstr "Le transporteur à qui la liste de prix appartient."
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr "El precio del servicio del transportista."
+msgstr "Le prix du service du transporteur."
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr "El límite inferior al que aplica el precio."
+msgstr "La limite inférieure pour le prix."
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Tarifa peso transportista"
+msgstr "Liste de prix par poids"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Peso"
+msgstr "Poids"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/es_419.po` & `trytond_carrier_weight-6.8.0/locale/cs.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Lista de precios"
+msgstr ""
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
 msgstr ""
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
@@ -35,15 +35,18 @@
 msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -56,12 +59,12 @@
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Lista de precio por peso de transportista"
+msgstr ""
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
 msgstr ""
```

### Comparing `trytond_carrier_weight-6.6.0/locale/et.po` & `trytond_carrier_weight-6.8.0/locale/pt.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr "Moeda"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Hinnakiri"
+msgstr "Lista de preços"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "Kaalu mõõtühik"
+msgstr "UDM do peso"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Kaalu mõõtühiku numbriväärtus"
+msgstr "Dígitos decimais da UDM do peso"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Vedaja"
+msgstr "Transportadora"
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr "Moeda"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Hind"
+msgstr "Preço"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Kaal"
+msgstr "Peso"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr "Hinna valuuta."
+msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Lisa veoteenusele hind."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr "Vedaja teenuse hind."
+msgstr ""
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr "Hinnale kehtim madalaim piirang"
+msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Vedaja kaalu hinnakiri"
+msgstr "Lista de preço por peso da transportadora"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Kaal"
+msgstr "Peso"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/fa.po` & `trytond_carrier_weight-6.8.0/locale/fa.po`

 * *Files 9% similar despite different names*

```diff
@@ -36,16 +36,19 @@
 msgstr "وزن"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr "واحد ارز قیمت."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "اضافه کردن قیمت به خدمات حمل ونقل."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr "شاخص واحد اندازه گیری وزن لیست قیمت."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
```

### Comparing `trytond_carrier_weight-6.6.0/locale/fi.po` & `trytond_carrier_weight-6.8.0/locale/fi.po`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,18 @@
 msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/fr.po` & `trytond_carrier_weight-6.8.0/locale/lo.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "ສະກຸນເງິນ"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Liste de prix"
+msgstr "ລາຍການລາຄາ"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "UDM de poids"
+msgstr "ຫົວໜ່ວຍນໍ້າໜັກ"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Décimales de l'UDM de poids"
+msgstr "ເສດຫົວໜ່ວຍນໍ້າໜັກ"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Transporteur"
+msgstr "ຜູ້ໃຫ້ບໍລິການ"
 
+#, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "ສະກຸນເງິນ"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Prix"
+msgstr "ລາຄາ"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Poids"
+msgstr "ນໍ້າໜັກ"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr "La devise du prix."
+msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Ajouter un prix au service du transporteur."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
-msgstr "L'unit de poids des critères de la liste de prix."
+msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
-msgstr "Le transporteur à qui la liste de prix appartient."
+msgstr ""
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr "Le prix du service du transporteur."
+msgstr ""
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr "La limite inférieure pour le prix."
+msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Liste de prix par poids"
+msgstr "ລາຍການລາຄາຂອງຜູ້ໃຫ້ບໍລິການນໍ້າໜັກ"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Poids"
+msgstr "ນໍ້າໜັກ"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/hu.po` & `trytond_carrier_weight-6.8.0/locale/bg.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Валута"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Fuvarozási árlista"
+msgstr "Ценова листа"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "Súly mértékegysége"
+msgstr "Мер. ед. за тегло"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr ""
+msgstr "Цифри на мер. ед, за тегло"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Fuvarozó"
+msgstr "Превозвач"
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Валута"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Ár"
+msgstr "Цена"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Súly"
+msgstr "Тегло"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
-msgstr "Az árlista ebben a pénznemben van megadva."
+msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Itt lehet a fuvarozás díjtáblázatát megadni."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
-"A fuvarozási árlistában a súlyok ebben a mértékegységben vannak megadva."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,price:"
 msgid "The price of the carrier service."
-msgstr "A fuvarozás díja."
+msgstr ""
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
-msgstr "Az ár ettől a súlytól érvényes."
+msgstr ""
 
+#, fuzzy
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr ""
+msgstr "Ценови лист на карго тегло"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "súly"
+msgstr "Тегло"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/id.po` & `trytond_carrier_weight-6.8.0/locale/tr.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Mata uang"
+msgstr ""
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
 msgstr ""
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
@@ -18,33 +18,35 @@
 msgid "Weight Uom Digits"
 msgstr ""
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Mata uang"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Harga"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
 msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/it.po` & `trytond_carrier_weight-6.8.0/locale/it.po`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,19 @@
 msgstr "Peso"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr "La valuta del prezzo."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Aggiungi prezzo al servizio di corriere."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr "L'unità di peso utilizzata nel listino prezzi."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
```

### Comparing `trytond_carrier_weight-6.6.0/locale/lo.po` & `trytond_carrier_weight-6.8.0/locale/id.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "ສະກຸນເງິນ"
+msgstr "Mata uang"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "ລາຍການລາຄາ"
+msgstr ""
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "ຫົວໜ່ວຍນໍ້າໜັກ"
+msgstr ""
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "ເສດຫົວໜ່ວຍນໍ້າໜັກ"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "ຜູ້ໃຫ້ບໍລິການ"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "ສະກຸນເງິນ"
+msgstr "Mata uang"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "ລາຄາ"
+msgstr "Harga"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "ນໍ້າໜັກ"
+msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -57,12 +60,12 @@
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "ລາຍການລາຄາຂອງຜູ້ໃຫ້ບໍລິການນໍ້າໜັກ"
+msgstr ""
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "ນໍ້າໜັກ"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_carrier_weight-6.6.0/locale/lt.po` & `trytond_carrier_weight-6.8.0/locale/lt.po`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 msgstr "Svoris"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr "Kainos valiuta."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/nl.po` & `trytond_carrier_weight-6.8.0/locale/nl.po`

 * *Files 22% similar despite different names*

```diff
@@ -35,16 +35,22 @@
 msgstr "Gewicht"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr "De valuta van de prijs."
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
-msgstr "Voeg prijs toe aan de transport service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
+msgstr ""
+"Voeg prijs per gewicht toe aan de koerier service.\n"
+"De eerste regel waarvan het gewicht groter is wordt gebruikt.\n"
+"De regel met gewicht 0 wordt gebruikt als standaard prijs."
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr "De gewichtseenheid criteria van de prijslijst."
 
 msgctxt "help:carrier.weight_price_list,carrier:"
 msgid "The carrier that the price list belongs to."
```

### Comparing `trytond_carrier_weight-6.6.0/locale/pl.po` & `trytond_carrier_weight-6.8.0/locale/pl.po`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 msgstr "Waga"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/pt.po` & `trytond_carrier_weight-6.8.0/locale/sl.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr "Valuta"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Lista de preços"
+msgstr "Cenik"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "UDM do peso"
+msgstr "ME za težo"
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Dígitos decimais da UDM do peso"
+msgstr "Decimalke za težo"
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Transportadora"
+msgstr "Špediter"
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr "Valuta"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Preço"
+msgstr "Cena"
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Peso"
+msgstr "Teža"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -57,12 +60,12 @@
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Lista de preço por peso da transportadora"
+msgstr "Ceniki po teži"
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Peso"
+msgstr "Teža"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/ro.po` & `trytond_carrier_weight-6.8.0/locale/ru.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Listă de prețuri"
+msgstr ""
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
 msgstr ""
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
@@ -21,30 +22,34 @@
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr "Валюты"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr ""
+msgstr "Ширина"
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -59,10 +64,11 @@
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr ""
+msgstr "Ширина"
```

### Comparing `trytond_carrier_weight-6.6.0/locale/ru.po` & `trytond_carrier_weight-6.8.0/locale/uk.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr ""
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
 msgstr ""
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
@@ -19,34 +18,35 @@
 msgid "Weight Uom Digits"
 msgstr ""
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Валюты"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Ширина"
+msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -61,11 +61,10 @@
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Ширина"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_carrier_weight-6.6.0/locale/sl.po` & `trytond_carrier_weight-6.8.0/locale/ro.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,weight_currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Valută"
 
 msgctxt "field:carrier,weight_price_list:"
 msgid "Price List"
-msgstr "Cenik"
+msgstr "Listă de prețuri"
 
 msgctxt "field:carrier,weight_uom:"
 msgid "Weight Uom"
-msgstr "ME za težo"
+msgstr ""
 
 msgctxt "field:carrier,weight_uom_digits:"
 msgid "Weight Uom Digits"
-msgstr "Decimalke za težo"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,carrier:"
 msgid "Carrier"
-msgstr "Špediter"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:carrier.weight_price_list,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Valută"
 
 msgctxt "field:carrier.weight_price_list,price:"
 msgid "Price"
-msgstr "Cena"
+msgstr ""
 
 msgctxt "field:carrier.weight_price_list,weight:"
 msgid "Weight"
-msgstr "Teža"
+msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
@@ -57,12 +60,12 @@
 
 msgctxt "help:carrier.weight_price_list,weight:"
 msgid "The lower limit for the price."
 msgstr ""
 
 msgctxt "model:carrier.weight_price_list,name:"
 msgid "Carrier Weight Price List"
-msgstr "Ceniki po teži"
+msgstr ""
 
 msgctxt "selection:carrier,carrier_cost_method:"
 msgid "Weight"
-msgstr "Teža"
+msgstr ""
```

### Comparing `trytond_carrier_weight-6.6.0/locale/tr.po` & `trytond_carrier_weight-6.8.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,18 @@
 msgstr ""
 
 msgctxt "help:carrier,weight_currency:"
 msgid "The currency of the price."
 msgstr ""
 
 msgctxt "help:carrier,weight_price_list:"
-msgid "Add price to the carrier service."
+msgid ""
+"Add price per weight to the carrier service.\n"
+"The first line for which the weight is greater is used.\n"
+"The line with weight of 0 is used as default price."
 msgstr ""
 
 msgctxt "help:carrier,weight_uom:"
 msgid "The unit of weight criteria of the price list."
 msgstr ""
 
 msgctxt "help:carrier.weight_price_list,carrier:"
```

### Comparing `trytond_carrier_weight-6.6.0/sale.py` & `trytond_carrier_weight-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-6.6.0/setup.py` & `trytond_carrier_weight-6.8.0/setup.py`

 * *Files 14% similar despite different names*

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
@@ -34,64 +31,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_carrier_weight'
 
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
 
 tests_require = [get_require_version('proteus'),
     get_require_version('trytond_purchase_shipment_cost'),
     get_require_version('trytond_sale_shipment_cost'),
     get_require_version('trytond_stock_shipment_cost'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add cost method "on weight" on carrier',
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
-        "Source Code": 'https://hg.tryton.org/modules/carrier_weight',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton carrier weight',
     package_dir={'trytond.modules.carrier_weight': '.'},
     packages=(
         ['trytond.modules.carrier_weight']
         + ['trytond.modules.carrier_weight.%s' % p for p in find_packages()]
         ),
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
     carrier_weight = trytond.modules.carrier_weight
     """,
     )
```

### Comparing `trytond_carrier_weight-6.6.0/stock.py` & `trytond_carrier_weight-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_weight-6.6.0/tests/scenario_carrier_weight.rst` & `trytond_carrier_weight-6.8.0/tests/scenario_carrier_weight.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 =======================
 Carrier Weight Scenario
 =======================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'carrier_weight',
     ...         'purchase_shipment_cost',
     ...         'sale_shipment_cost',
```

### Comparing `trytond_carrier_weight-6.6.0/tox.ini` & `trytond_carrier_weight-6.8.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/carrier_weight/* -m unittest discover -s tests
-    coverage report --include=./**/carrier_weight/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
+passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
-    sqlite: DB_NAME={env:SQLITE_NAME::memory:}
-    postgresql: DB_NAME={env:POSTGRESQL_NAME:test}
-install_command = pip install --pre --find-links https://trydevpi.tryton.org/?local_version={env:CI_JOB_ID:{env:CI_BUILD_NUMBER:}.{env:CI_JOB_NUMBER:}} {opts} {packages}
+    sqlite: DB_NAME={env:DB_NAME::memory:}
+    postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/PKG-INFO` & `trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-carrier-weight
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add cost method "on weight" on carrier
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
-Project-URL: Source Code, https://hg.tryton.org/modules/carrier_weight
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier weight
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,23 +39,23 @@
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
 
 Carrier Weight Module
 #####################
 
 The carrier weight module adds a cost method based on weight.
-The price is computed by finding the line for which the weight is greater or
-equal but smaller than the next line.
+The price is computed by finding the first line for which the weight is
+greater.
```

### Comparing `trytond_carrier_weight-6.6.0/trytond_carrier_weight.egg-info/SOURCES.txt` & `trytond_carrier_weight-6.8.0/trytond_carrier_weight.egg-info/SOURCES.txt`

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
 carrier.py
@@ -50,14 +46,15 @@
 ./tests/__init__.py
 ./tests/scenario_carrier_weight.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/carrier_form.xml
 ./view/weight_price_list_form.xml
 ./view/weight_price_list_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

