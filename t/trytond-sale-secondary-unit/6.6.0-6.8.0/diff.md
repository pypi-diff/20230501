# Comparing `tmp/trytond_sale_secondary_unit-6.6.0.tar.gz` & `tmp/trytond_sale_secondary_unit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_secondary_unit-6.6.0.tar", last modified: Mon Oct 31 16:25:19 2022, max compression
+gzip compressed data, was "trytond_sale_secondary_unit-6.8.0.tar", last modified: Mon May  1 12:05:16 2023, max compression
```

## Comparing `trytond_sale_secondary_unit-6.6.0.tar` & `trytond_sale_secondary_unit-6.8.0.tar`

### file list

```diff
@@ -1,71 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:19.732932 trytond_sale_secondary_unit-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_secondary_unit-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_secondary_unit-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-10-31 16:25:18.000000 trytond_sale_secondary_unit-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_secondary_unit-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      604 2022-10-31 16:25:17.000000 trytond_sale_secondary_unit-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:25:17.000000 trytond_sale_secondary_unit-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_secondary_unit-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2688 2022-10-31 16:25:19.732932 trytond_sale_secondary_unit-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2022-10-11 19:49:58.000000 trytond_sale_secondary_unit-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1189 2021-12-11 16:59:34.000000 trytond_sale_secondary_unit-6.6.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:19.729598 trytond_sale_secondary_unit-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:19.729598 trytond_sale_secondary_unit-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4831 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4909 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4866 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4963 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4987 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3612 2022-10-29 07:50:45.000000 trytond_sale_secondary_unit-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6211 2022-04-11 21:24:34.000000 trytond_sale_secondary_unit-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      834 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12898 2022-10-11 19:49:58.000000 trytond_sale_secondary_unit-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:25:19.732932 trytond_sale_secondary_unit-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5423 2022-10-29 07:39:11.000000 trytond_sale_secondary_unit-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1172 2021-12-11 16:59:34.000000 trytond_sale_secondary_unit-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:19.729598 trytond_sale_secondary_unit-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_secondary_unit-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3826 2022-10-11 19:49:58.000000 trytond_sale_secondary_unit-6.6.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3534 2020-11-02 09:23:33.000000 trytond_sale_secondary_unit-6.6.0/tests/scenario_sale_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2022-10-11 19:49:58.000000 trytond_sale_secondary_unit-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_secondary_unit-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-31 15:10:09.000000 trytond_sale_secondary_unit-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2022-10-31 16:25:16.000000 trytond_sale_secondary_unit-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:19.732932 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2688 2022-10-31 16:25:19.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1999 2022-10-31 16:25:19.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:25:19.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2022-10-31 16:25:19.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-11-04 12:09:20.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2022-10-31 16:25:19.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:25:19.000000 trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:25:19.729598 trytond_sale_secondary_unit-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/view/product_customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      711 2019-10-11 23:19:18.000000 trytond_sale_secondary_unit-6.6.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2021-10-07 13:08:07.000000 trytond_sale_secondary_unit-6.6.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2022-04-08 16:23:27.000000 trytond_sale_secondary_unit-6.6.0/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2020-10-09 17:09:19.000000 trytond_sale_secondary_unit-6.6.0/view/stock_move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:16.023367 trytond_sale_secondary_unit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-05-01 11:17:22.000000 trytond_sale_secondary_unit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:17:22.000000 trytond_sale_secondary_unit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-05-01 12:05:16.023367 trytond_sale_secondary_unit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1189 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:16.020033 trytond_sale_secondary_unit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:16.016700 trytond_sale_secondary_unit-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4831 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4909 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4866 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4963 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4987 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3612 2023-04-29 08:02:51.000000 trytond_sale_secondary_unit-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6197 2023-04-21 08:36:08.000000 trytond_sale_secondary_unit-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      834 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12892 2023-04-21 08:36:08.000000 trytond_sale_secondary_unit-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:05:16.023367 trytond_sale_secondary_unit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4608 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1172 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:16.016700 trytond_sale_secondary_unit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3534 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/tests/scenario_sale_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-05-01 11:17:16.000000 trytond_sale_secondary_unit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:16.023367 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-05-01 12:05:15.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1973 2023-05-01 12:05:15.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:05:15.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 12:05:15.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-05-01 12:05:15.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:05:15.000000 trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:16.020033 trytond_sale_secondary_unit-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/view/product_customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      711 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-6.8.0/view/stock_move_list.xml
```

### Comparing `trytond_sale_secondary_unit-6.6.0/CHANGELOG` & `trytond_sale_secondary_unit-6.8.0/CHANGELOG`

 * *Files 17% similar despite different names*

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

### Comparing `trytond_sale_secondary_unit-6.6.0/COPYRIGHT` & `trytond_sale_secondary_unit-6.8.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2019-2022 Cédric Krier
-Copyright (C) 2019-2022 B2CK
+Copyright (C) 2019-2023 Cédric Krier
+Copyright (C) 2019-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_secondary_unit-6.6.0/LICENSE` & `trytond_sale_secondary_unit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/PKG-INFO` & `trytond_sale_secondary_unit-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_secondary_unit
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add a secondary unit on sale line
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_secondary_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale secondary unit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 
 Sale Secondary Unit Module
 ##########################
 
 The sale secondary unit module adds a secondary unit of measure on sale lines.
```

### Comparing `trytond_sale_secondary_unit-6.6.0/__init__.py` & `trytond_sale_secondary_unit-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/account.py` & `trytond_sale_secondary_unit-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/bg.po` & `trytond_sale_secondary_unit-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/ca.po` & `trytond_sale_secondary_unit-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/cs.po` & `trytond_sale_secondary_unit-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/de.po` & `trytond_sale_secondary_unit-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/es.po` & `trytond_sale_secondary_unit-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/es_419.po` & `trytond_sale_secondary_unit-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/et.po` & `trytond_sale_secondary_unit-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/fa.po` & `trytond_sale_secondary_unit-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/fi.po` & `trytond_sale_secondary_unit-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/fr.po` & `trytond_sale_secondary_unit-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/hu.po` & `trytond_sale_secondary_unit-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/id.po` & `trytond_sale_secondary_unit-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/it.po` & `trytond_sale_secondary_unit-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/lo.po` & `trytond_sale_secondary_unit-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/lt.po` & `trytond_sale_secondary_unit-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/nl.po` & `trytond_sale_secondary_unit-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/pl.po` & `trytond_sale_secondary_unit-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/pt.po` & `trytond_sale_secondary_unit-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/ro.po` & `trytond_sale_secondary_unit-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/ru.po` & `trytond_sale_secondary_unit-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/sl.po` & `trytond_sale_secondary_unit-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/tr.po` & `trytond_sale_secondary_unit-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/uk.po` & `trytond_sale_secondary_unit-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/locale/zh_CN.po` & `trytond_sale_secondary_unit-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/product.py` & `trytond_sale_secondary_unit-6.8.0/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
         else:
             self.sale_secondary_uom_factor = round(
                 1. / self.sale_secondary_uom_rate, uom_conversion_digits[1])
 
     @fields.depends('sale_secondary_uom')
     def on_change_with_sale_secondary_uom_category(self, name=None):
         if self.sale_secondary_uom:
-            return self.sale_secondary_uom.category.id
+            return self.sale_secondary_uom.category
 
     @classmethod
     def search_sale_secondary_uom_category(cls, name, clause):
-        return [('sale_secondary_uom.category' + clause[0].lstrip(name),)
-            + tuple(clause[1:])]
+        return [('sale_secondary_uom.category' + clause[0][len(name):],
+                *clause[1:])]
 
     @property
     def sale_secondary_uom_normal_rate(self):
         uom = self.sale_secondary_uom
         rate = self.sale_secondary_uom_rate
         if self.sale_uom and rate and uom:
             if self.sale_uom.accurate_field == 'factor':
@@ -147,17 +147,17 @@
         fields.Many2One('product.uom.category', "Default UOM Category"),
         'on_change_with_default_uom_category')
 
     @fields.depends('template', '_parent_template.sale_uom',
         'product', '_parent_product.sale_uom')
     def on_change_with_default_uom_category(self, name=None):
         if self.product and self.product.sale_uom:
-            return self.product.sale_uom.category.id
+            return self.product.sale_uom.category
         elif self.template and self.template.sale_uom:
-            return self.template.sale_uom.category.id
+            return self.template.sale_uom.category
 
     @property
     def sale_uom(self):
         if self.product and self.product.sale_uom:
             return self.product.sale_uom
         elif self.template and self.template.sale_uom:
             return self.template.sale_uom
```

### Comparing `trytond_sale_secondary_unit-6.6.0/product.xml` & `trytond_sale_secondary_unit-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/sale.py` & `trytond_sale_secondary_unit-6.8.0/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         self.on_change_secondary_quantity()
         self.on_change_secondary_unit_price()
 
     @fields.depends(methods=['_secondary_record'])
     def on_change_with_product_secondary_uom_category(self, name=None):
         secondary_record = self._secondary_record()
         if secondary_record:
-            return secondary_record.sale_secondary_uom.category.id
+            return secondary_record.sale_secondary_uom.category
 
     @classmethod
     def set_secondary(cls, lines, name, value):
         pass
 
     @fields.depends('secondary_unit',
         methods=['on_change_with_secondary_quantity', '_secondary_record'])
@@ -222,15 +222,15 @@
                 rate=line.secondary_uom_factor,
                 round=round)
         return remaining_quantity
 
     @fields.depends('product')
     def on_change_with_product_secondary_uom_category(self, name=None):
         if self.product and self.product.sale_secondary_uom:
-            return self.product.sale_secondary_uom.category.id
+            return self.product.sale_secondary_uom.category
 
     def _set_sale_line_quantity(self, sale_line):
         super()._set_sale_line_quantity(sale_line)
         secondary_uom = self.product.sale_secondary_uom
         if (secondary_uom
                 and self.unit.category == secondary_uom.category):
             sale_line.unit = self.product.sale_uom
```

### Comparing `trytond_sale_secondary_unit-6.6.0/sale.xml` & `trytond_sale_secondary_unit-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/setup.py` & `trytond_sale_secondary_unit-6.8.0/setup.py`

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
@@ -34,64 +31,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_secondary_unit'
 
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
     get_require_version('trytond_account_invoice_secondary_unit'),
     get_require_version('trytond_sale_blanket_agreement'),
     get_require_version('trytond_stock_secondary_unit'),
     get_require_version('trytond_sale_product_customer')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add a secondary unit on sale line',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_secondary_unit',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale secondary unit',
     package_dir={'trytond.modules.sale_secondary_unit': '.'},
     packages=(
         ['trytond.modules.sale_secondary_unit']
         + ['trytond.modules.sale_secondary_unit.%s' % p
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
     sale_secondary_unit = trytond.modules.sale_secondary_unit
     """,
     )
```

### Comparing `trytond_sale_secondary_unit-6.6.0/stock.py` & `trytond_sale_secondary_unit-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst` & `trytond_sale_secondary_unit-6.8.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 ==============================================
 Sale Blanket Agreement Secondary Unit Scenario
 ==============================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts)
 
-    >>> today = datetime.date.today()
-    >>> later = today + relativedelta(days=30)
-
+    >>> today = dt.date.today()
+    >>> later = today + dt.timedelta(days=30)
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_secondary_unit', 'sale_blanket_agreement'])
 
     >>> Party = Model.get('party.party')
@@ -84,16 +82,15 @@
     >>> blanket_agreement_line.unit_price = Decimal('9.000')
     >>> blanket_agreement.click('run')
     >>> blanket_agreement.state
     'running'
 
 Create sale from blanket agreement::
 
-    >>> create_sale = Wizard(
-    ...     'sale.blanket_agreement.create_sale', [blanket_agreement])
+    >>> create_sale = blanket_agreement.click('create_sale')
     >>> create_sale.form.lines[0].unit == gr
     True
     >>> create_sale.execute('create_sale')
 
     >>> sale, = create_sale.actions[0]
     >>> line, = sale.lines
     >>> line.product == product
```

### Comparing `trytond_sale_secondary_unit-6.6.0/tests/scenario_sale_secondary_unit.rst` & `trytond_sale_secondary_unit-6.8.0/tests/scenario_sale_secondary_unit.rst`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 Confirm sale::
 
     >>> line.secondary_unit = kg
     >>> line.quantity = 10
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> sale.invoice_state
-    'waiting'
+    'pending'
     >>> sale.shipment_state
     'waiting'
 
 Check secondary unit on invoice::
 
     >>> invoice, = sale.invoices
     >>> _, line = invoice.lines
```

### Comparing `trytond_sale_secondary_unit-6.6.0/tox.ini` & `trytond_sale_secondary_unit-6.8.0/tox.ini`

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
-    coverage run --include=./**/sale_secondary_unit/* -m unittest discover -s tests
-    coverage report --include=./**/sale_secondary_unit/* --omit=*/tests/*
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

### Comparing `trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/PKG-INFO` & `trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-secondary-unit
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add a secondary unit on sale line
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_secondary_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale secondary unit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 
 Sale Secondary Unit Module
 ##########################
 
 The sale secondary unit module adds a secondary unit of measure on sale lines.
```

### Comparing `trytond_sale_secondary_unit-6.6.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt` & `trytond_sale_secondary_unit-6.8.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt`

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
 account.py
@@ -59,14 +55,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/product_customer_form.xml
 ./view/product_template_form.xml
 ./view/sale_line_form.xml
 ./view/sale_line_tree.xml
 ./view/stock_move_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_sale_secondary_unit-6.6.0/view/product_customer_form.xml` & `trytond_sale_secondary_unit-6.8.0/view/product_customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/view/product_template_form.xml` & `trytond_sale_secondary_unit-6.8.0/view/product_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-6.6.0/view/sale_line_form.xml` & `trytond_sale_secondary_unit-6.8.0/view/sale_line_form.xml`

 * *Files identical despite different names*

