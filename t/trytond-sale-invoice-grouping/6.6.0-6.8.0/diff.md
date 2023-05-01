# Comparing `tmp/trytond_sale_invoice_grouping-6.6.0.tar.gz` & `tmp/trytond_sale_invoice_grouping-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_invoice_grouping-6.6.0.tar", last modified: Mon Oct 31 16:11:40 2022, max compression
+gzip compressed data, was "trytond_sale_invoice_grouping-6.8.0.tar", last modified: Mon May  1 11:36:19 2023, max compression
```

## Comparing `trytond_sale_invoice_grouping-6.6.0.tar` & `trytond_sale_invoice_grouping-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:40.400672 trytond_sale_invoice_grouping-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_invoice_grouping-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_invoice_grouping-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2022-10-31 16:11:39.000000 trytond_sale_invoice_grouping-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_invoice_grouping-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1594 2022-10-31 16:11:38.000000 trytond_sale_invoice_grouping-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      689 2022-10-31 16:11:37.000000 trytond_sale_invoice_grouping-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:40.000000 trytond_sale_invoice_grouping-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_invoice_grouping-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2903 2022-10-31 16:11:40.400672 trytond_sale_invoice_grouping-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2019-02-13 10:09:40.000000 trytond_sale_invoice_grouping-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      479 2021-12-11 16:59:34.000000 trytond_sale_invoice_grouping-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1378 2021-03-24 12:34:22.000000 trytond_sale_invoice_grouping-6.6.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2019-06-04 16:49:45.000000 trytond_sale_invoice_grouping-6.6.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:40.400672 trytond_sale_invoice_grouping-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2019-02-13 10:09:40.000000 trytond_sale_invoice_grouping-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:40.397338 trytond_sale_invoice_grouping-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1425 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1830 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1792 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1723 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1950 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1862 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1393 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1892 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1840 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1792 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1384 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1441 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1663 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1379 2022-10-29 07:50:32.000000 trytond_sale_invoice_grouping-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2022-10-11 19:49:58.000000 trytond_sale_invoice_grouping-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2019-02-13 10:09:40.000000 trytond_sale_invoice_grouping-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2420 2022-10-27 22:32:49.000000 trytond_sale_invoice_grouping-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:11:40.400672 trytond_sale_invoice_grouping-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5244 2022-10-29 07:39:11.000000 trytond_sale_invoice_grouping-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:40.397338 trytond_sale_invoice_grouping-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_invoice_grouping-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6001 2021-03-24 12:36:50.000000 trytond_sale_invoice_grouping-6.6.0/tests/scenario_sale_invoice_grouping.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2022-10-27 22:32:49.000000 trytond_sale_invoice_grouping-6.6.0/tests/scenario_sale_invoice_grouping_multiple.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2022-04-16 16:30:57.000000 trytond_sale_invoice_grouping-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_invoice_grouping-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 15:10:09.000000 trytond_sale_invoice_grouping-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2022-10-31 16:11:36.000000 trytond_sale_invoice_grouping-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:40.400672 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2903 2022-10-31 16:11:39.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1777 2022-10-31 16:11:40.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:11:39.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:11:39.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:48.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      125 2022-10-31 16:11:39.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:11:39.000000 trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:40.400672 trytond_sale_invoice_grouping-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2019-06-04 16:49:45.000000 trytond_sale_invoice_grouping-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2019-02-13 10:09:40.000000 trytond_sale_invoice_grouping-6.6.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:19.425149 trytond_sale_invoice_grouping-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1757 2023-05-01 10:57:37.000000 trytond_sale_invoice_grouping-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      689 2023-05-01 10:57:36.000000 trytond_sale_invoice_grouping-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2889 2023-05-01 11:36:19.425149 trytond_sale_invoice_grouping-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      479 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1378 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:19.421816 trytond_sale_invoice_grouping-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:19.418483 trytond_sale_invoice_grouping-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1425 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1830 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1792 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1723 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1950 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1862 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1892 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1840 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1792 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1384 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1441 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1663 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-04-29 08:02:39.000000 trytond_sale_invoice_grouping-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:36:19.425149 trytond_sale_invoice_grouping-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4427 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:19.421816 trytond_sale_invoice_grouping-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5882 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/tests/scenario_sale_invoice_grouping.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/tests/scenario_sale_invoice_grouping_multiple.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_invoice_grouping-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-05-01 10:57:31.000000 trytond_sale_invoice_grouping-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:19.425149 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2889 2023-05-01 11:36:18.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1751 2023-05-01 11:36:19.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:36:18.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:36:18.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      125 2023-05-01 11:36:18.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:36:18.000000 trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:19.421816 trytond_sale_invoice_grouping-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2023-01-16 14:00:21.000000 trytond_sale_invoice_grouping-6.8.0/view/party_form.xml
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/CHANGELOG` & `trytond_sale_invoice_grouping-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

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

### Comparing `trytond_sale_invoice_grouping-6.6.0/COPYRIGHT` & `trytond_sale_invoice_grouping-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2013-2017 Nicolas Évrard.
-Copyright (C) 2013-2022 B2CK SPRL.
+Copyright (C) 2013-2023 Nicolas Évrard.
+Copyright (C) 2013-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/LICENSE` & `trytond_sale_invoice_grouping-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/PKG-INFO` & `trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_sale_invoice_grouping
-Version: 6.6.0
+Name: trytond-sale-invoice-grouping
+Version: 6.8.0
 Summary: Tryton module to group sale invoices
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_invoice_grouping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale group invoice
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
 
 Sale Invoice Grouping Module
 ############################
 
 The ``sale_invoice_grouping`` module adds an option to define how invoice lines
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/README.rst` & `trytond_sale_invoice_grouping-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/configuration.py` & `trytond_sale_invoice_grouping-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/doc/index.rst` & `trytond_sale_invoice_grouping-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/bg.po` & `trytond_sale_invoice_grouping-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/ca.po` & `trytond_sale_invoice_grouping-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/cs.po` & `trytond_sale_invoice_grouping-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/de.po` & `trytond_sale_invoice_grouping-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/es.po` & `trytond_sale_invoice_grouping-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/es_419.po` & `trytond_sale_invoice_grouping-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/et.po` & `trytond_sale_invoice_grouping-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/fa.po` & `trytond_sale_invoice_grouping-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/fi.po` & `trytond_sale_invoice_grouping-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/fr.po` & `trytond_sale_invoice_grouping-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/hu.po` & `trytond_sale_invoice_grouping-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/id.po` & `trytond_sale_invoice_grouping-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/it.po` & `trytond_sale_invoice_grouping-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/lo.po` & `trytond_sale_invoice_grouping-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/lt.po` & `trytond_sale_invoice_grouping-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/nl.po` & `trytond_sale_invoice_grouping-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/pl.po` & `trytond_sale_invoice_grouping-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/pt.po` & `trytond_sale_invoice_grouping-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/ro.po` & `trytond_sale_invoice_grouping-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/ru.po` & `trytond_sale_invoice_grouping-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/sl.po` & `trytond_sale_invoice_grouping-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/tr.po` & `trytond_sale_invoice_grouping-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/uk.po` & `trytond_sale_invoice_grouping-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/locale/zh_CN.po` & `trytond_sale_invoice_grouping-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/party.py` & `trytond_sale_invoice_grouping-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/sale.py` & `trytond_sale_invoice_grouping-6.8.0/sale.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,31 @@
     __name__ = 'sale.sale'
 
     @property
     def invoice_grouping_method(self):
         party = self.invoice_party or self.party
         return party.sale_invoice_grouping_method
 
-    @property
-    def _invoice_grouping_fields(self):
-        return ('state', 'company', 'type', 'journal', 'party',
-            'invoice_address', 'currency', 'account', 'payment_term')
+    def _get_invoice_grouping_fields(self, invoice):
+        return ['state', 'company', 'type', 'journal', 'party',
+            'invoice_address', 'currency', 'account', 'payment_term']
 
     def _get_grouped_invoice_order(self):
         "Returns the order clause used to find invoice that should be grouped"
         return None
 
     def _get_grouped_invoice_domain(self, invoice):
         "Returns a domain that will find invoices that should be grouped"
         Invoice = invoice.__class__
         invoice_domain = [
             ('lines.origin', 'like', 'sale.line,%'),
             ]
-        defaults = Invoice.default_get(self._invoice_grouping_fields,
-            with_rec_name=False)
-        for field in self._invoice_grouping_fields:
+        fields = self._get_invoice_grouping_fields(invoice)
+        defaults = Invoice.default_get(fields, with_rec_name=False)
+        for field in fields:
             invoice_domain.append(
                 (field, '=', getattr(invoice, field, defaults.get(field)))
                 )
         return invoice_domain
 
     def _get_invoice_sale(self):
         transaction = Transaction()
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/setup.py` & `trytond_sale_invoice_grouping-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_invoice_grouping'
 
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
     description='Tryton module to group sale invoices',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_invoice_grouping',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale group invoice',
     package_dir={'trytond.modules.sale_invoice_grouping': '.'},
     packages=(
         ['trytond.modules.sale_invoice_grouping']
         + ['trytond.modules.sale_invoice_grouping.%s' % p
             for p in find_packages()]
@@ -124,28 +102,27 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     sale_invoice_grouping = trytond.modules.sale_invoice_grouping
     """,
     )
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/tests/scenario_sale_invoice_grouping.rst` & `trytond_sale_invoice_grouping-6.8.0/tests/scenario_sale_invoice_grouping.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 ==============================
 Sale Invoice Grouping Scenario
 ==============================
 
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
 
     >>> config = activate_modules('sale_invoice_grouping')
 
 Create company::
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/tests/scenario_sale_invoice_grouping_multiple.rst` & `trytond_sale_invoice_grouping-6.8.0/tests/scenario_sale_invoice_grouping_multiple.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/PKG-INFO` & `trytond_sale_invoice_grouping-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-sale-invoice-grouping
-Version: 6.6.0
+Name: trytond_sale_invoice_grouping
+Version: 6.8.0
 Summary: Tryton module to group sale invoices
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_invoice_grouping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale group invoice
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
 
 Sale Invoice Grouping Module
 ############################
 
 The ``sale_invoice_grouping`` module adds an option to define how invoice lines
```

### Comparing `trytond_sale_invoice_grouping-6.6.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt` & `trytond_sale_invoice_grouping-6.8.0/trytond_sale_invoice_grouping.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
 configuration.py
@@ -50,14 +46,15 @@
 ./tests/__init__.py
 ./tests/scenario_sale_invoice_grouping.rst
 ./tests/scenario_sale_invoice_grouping_multiple.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/configuration_form.xml
 ./view/party_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

