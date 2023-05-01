# Comparing `tmp/trytond_account_stock_shipment_cost-6.6.0.tar.gz` & `tmp/trytond_account_stock_shipment_cost-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_shipment_cost-6.6.0.tar", last modified: Mon Oct 31 16:03:31 2022, max compression
+gzip compressed data, was "trytond_account_stock_shipment_cost-6.8.0.tar", last modified: Mon May  1 12:05:06 2023, max compression
```

## Comparing `trytond_account_stock_shipment_cost-6.6.0.tar` & `trytond_account_stock_shipment_cost-6.8.0.tar`

### file list

```diff
@@ -1,74 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:31.580231 trytond_account_stock_shipment_cost-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_account_stock_shipment_cost-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 16:03:29.000000 trytond_account_stock_shipment_cost-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_stock_shipment_cost-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2022-10-31 16:03:28.000000 trytond_account_stock_shipment_cost-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:03:28.000000 trytond_account_stock_shipment_cost-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_stock_shipment_cost-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2595 2022-10-31 16:03:31.580231 trytond_account_stock_shipment_cost-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2022-10-27 11:24:44.000000 trytond_account_stock_shipment_cost-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2022-07-17 22:16:37.000000 trytond_account_stock_shipment_cost-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15600 2022-10-11 19:49:57.000000 trytond_account_stock_shipment_cost-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9525 2022-07-17 22:16:37.000000 trytond_account_stock_shipment_cost-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:31.573564 trytond_account_stock_shipment_cost-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2022-10-27 11:24:44.000000 trytond_account_stock_shipment_cost-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_account_stock_shipment_cost-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:31.570231 trytond_account_stock_shipment_cost-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7039 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6981 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7135 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5888 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5878 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6858 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2022-10-29 07:50:45.000000 trytond_account_stock_shipment_cost-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      671 2022-04-08 16:26:26.000000 trytond_account_stock_shipment_cost-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2022-04-10 15:40:35.000000 trytond_account_stock_shipment_cost-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:03:31.580231 trytond_account_stock_shipment_cost-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5615 2022-10-29 07:39:10.000000 trytond_account_stock_shipment_cost-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      709 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:31.570231 trytond_account_stock_shipment_cost-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_stock_shipment_cost-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7314 2022-09-29 07:07:37.000000 trytond_account_stock_shipment_cost-6.6.0/tests/scenario_account_stock_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2022-04-16 16:30:56.000000 trytond_account_stock_shipment_cost-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_account_stock_shipment_cost-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2022-10-31 15:10:09.000000 trytond_account_stock_shipment_cost-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2022-10-31 16:03:26.000000 trytond_account_stock_shipment_cost-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:31.576897 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2595 2022-10-31 16:03:30.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2147 2022-10-31 16:03:31.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:03:30.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2022-10-31 16:03:30.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-07-24 21:15:11.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2022-10-31 16:03:30.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:03:30.000000 trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:31.573564 trytond_account_stock_shipment_cost-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2022-07-17 22:16:37.000000 trytond_account_stock_shipment_cost-6.6.0/view/shipment_cost_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/view/shipment_cost_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2022-07-17 22:16:37.000000 trytond_account_stock_shipment_cost-6.6.0/view/shipment_cost_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2022-07-17 22:16:37.000000 trytond_account_stock_shipment_cost-6.6.0/view/shipment_cost_show_shipment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2021-10-07 13:08:07.000000 trytond_account_stock_shipment_cost-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:06.856586 trytond_account_stock_shipment_cost-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-05-01 11:17:15.000000 trytond_account_stock_shipment_cost-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:17:15.000000 trytond_account_stock_shipment_cost-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2575 2023-05-01 12:05:06.853253 trytond_account_stock_shipment_cost-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15600 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9525 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:06.849919 trytond_account_stock_shipment_cost-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:06.846586 trytond_account_stock_shipment_cost-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7039 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6981 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7186 2023-04-30 10:46:36.000000 trytond_account_stock_shipment_cost-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5878 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6858 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2023-04-30 10:46:36.000000 trytond_account_stock_shipment_cost-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-04-29 08:02:51.000000 trytond_account_stock_shipment_cost-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:05:06.856586 trytond_account_stock_shipment_cost-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4768 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      709 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:06.846586 trytond_account_stock_shipment_cost-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7257 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/tests/scenario_account_stock_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-05-01 11:17:09.000000 trytond_account_stock_shipment_cost-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:06.853253 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2575 2023-05-01 12:05:05.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-05-01 12:05:06.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:05:05.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-05-01 12:05:05.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-05-01 12:05:05.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:05:05.000000 trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:05:06.849919 trytond_account_stock_shipment_cost-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/shipment_cost_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/shipment_cost_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/shipment_cost_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/shipment_cost_show_shipment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-6.8.0/view/template_form.xml
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/COPYRIGHT` & `trytond_account_stock_shipment_cost-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2022 B2CK
-Copyright (C) 2021-2022 Cédric Krier
+Copyright (C) 2021-2023 B2CK
+Copyright (C) 2021-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/LICENSE` & `trytond_account_stock_shipment_cost-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/PKG-INFO` & `trytond_account_stock_shipment_cost-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_shipment_cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to allocate shipment cost based on invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-shipment-cost
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock shipment cost carrier invoice
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
 
 ##################################
 Account Stock Shipment Cost Module
 ##################################
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/__init__.py` & `trytond_account_stock_shipment_cost-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/account.py` & `trytond_account_stock_shipment_cost-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/account.xml` & `trytond_account_stock_shipment_cost-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/doc/conf.py` & `trytond_account_stock_shipment_cost-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_stock_shipment_cost-6.6.0/doc/design.rst` & `trytond_account_stock_shipment_cost-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/bg.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/ca.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/cs.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/de.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/es.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/es_419.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/et.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/fa.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/fi.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/fr.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 msgctxt "field:account.shipment_cost,number:"
 msgid "Number"
 msgstr "Numéro"
 
 msgctxt "field:account.shipment_cost,posted_date:"
 msgid "Posted Date"
-msgstr "Date de postage"
+msgstr "Date de comptabilisation"
 
 msgctxt "field:account.shipment_cost,shipment_returns:"
 msgid "Shipment Returns"
 msgstr "Retours d'expédition"
 
 msgctxt "field:account.shipment_cost,shipments:"
 msgid "Shipments"
@@ -129,27 +129,27 @@
 
 msgctxt "model:account.shipment_cost.show,name:"
 msgid "Shipment Cost Show"
 msgstr "Montrer les coûts d'expédition"
 
 msgctxt "model:account.shipment_cost.show.shipment,name:"
 msgid "Post Shipment Cost"
-msgstr "Poster les coûts d'expédition"
+msgstr "Comptabiliser les coûts d'expédition"
 
 msgctxt "model:ir.action,name:act_shipment_cost_form"
 msgid "Shipment Costs"
 msgstr "Coûts d'expédition"
 
 msgctxt "model:ir.action,name:act_shipment_cost_form_shipment"
 msgid "Shipment Costs"
 msgstr "Coûts d'expédition"
 
 msgctxt "model:ir.action,name:wizard_shipment_cost_post"
 msgid "Post Shipment Cost"
-msgstr "Poster les coûts d'expédition"
+msgstr "Comptabiliser les coûts d'expédition"
 
 msgctxt "model:ir.action,name:wizard_shipment_cost_show"
 msgid "Show Shipment Cost"
 msgstr "Afficher le coût d'expédition"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_shipment_cost_form_domain_all"
@@ -160,15 +160,15 @@
 "model:ir.action.act_window.domain,name:act_shipment_cost_form_domain_draft"
 msgid "Draft"
 msgstr "Brouillons"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_shipment_cost_form_domain_posted"
 msgid "Posted"
-msgstr "Postés"
+msgstr "Comptabilisés"
 
 msgctxt "model:ir.message,text:msg_shipment_cost_post_no_shipment"
 msgid "The shipment cost \"%(shipment_cost)s\" has no shipment."
 msgstr "Le coût d'expédition « %(shipment_cost)s » n'a pas d'expédition."
 
 msgctxt "model:ir.message,text:msg_shipment_cost_post_same_parties"
 msgid ""
@@ -184,15 +184,15 @@
 
 msgctxt "model:ir.model.button,string:shipment_cost_draft_button"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "model:ir.model.button,string:shipment_cost_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:shipment_cost_show_button"
 msgid "Show"
 msgstr "Afficher"
 
 msgctxt "model:ir.rule.group,name:rule_group_shipment_cost_companies"
 msgid "User in companies"
@@ -220,15 +220,15 @@
 
 msgctxt "selection:account.shipment_cost,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:account.shipment_cost,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "selection:account.shipment_cost.show.shipment,shipment:"
 msgid "Shipment"
 msgstr "Expédition"
 
 msgctxt "selection:account.shipment_cost.show.shipment,shipment:"
 msgid "Shipment Return"
@@ -244,12 +244,12 @@
 
 msgctxt "wizard_button:account.shipment_cost.post,show,end:"
 msgid "Cancel"
 msgstr "Annuler"
 
 msgctxt "wizard_button:account.shipment_cost.post,show,post:"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "wizard_button:account.shipment_cost.show,show,end:"
 msgid "Close"
 msgstr "Fermer"
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/hu.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/id.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/it.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/lo.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/lt.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/nl.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/pl.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/pt.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/ro.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/ru.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/sl.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/tr.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/uk.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/locale/zh_CN.po` & `trytond_account_stock_shipment_cost-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #
+#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,shipment_cost_sequence:"
 msgid "Shipment Cost Sequence"
 msgstr ""
 
@@ -45,15 +46,15 @@
 
 msgctxt "field:account.shipment_cost,shipment_returns:"
 msgid "Shipment Returns"
 msgstr ""
 
 msgctxt "field:account.shipment_cost,shipments:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:account.shipment_cost,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.shipment_cost-stock.shipment.out,shipment:"
 msgid "Shipment"
@@ -73,23 +74,23 @@
 
 msgctxt "field:account.shipment_cost.show,cost:"
 msgid "Cost"
 msgstr ""
 
 msgctxt "field:account.shipment_cost.show,shipments:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:account.shipment_cost.show.shipment,cost:"
 msgid "Cost"
 msgstr ""
 
 msgctxt "field:account.shipment_cost.show.shipment,shipment:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:product.product,shipment_cost:"
 msgid "Shipment Cost"
 msgstr ""
 
 msgctxt "field:product.template,shipment_cost:"
 msgid "Shipment Cost"
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/message.xml` & `trytond_account_stock_shipment_cost-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/product.py` & `trytond_account_stock_shipment_cost-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/setup.py` & `trytond_account_stock_shipment_cost-6.8.0/setup.py`

 * *Files 15% similar despite different names*

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
@@ -37,64 +34,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_stock_shipment_cost'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-
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
+
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module to allocate shipment cost based on invoice',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/'
             'modules-account-stock-shipment-cost'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_stock_shipment_cost'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock shipment cost carrier invoice',
     package_dir={'trytond.modules.account_stock_shipment_cost': '.'},
     packages=(
         ['trytond.modules.account_stock_shipment_cost']
         + ['trytond.modules.account_stock_shipment_cost.%s' % p
             for p in find_packages()]
@@ -132,28 +108,27 @@
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
     account_stock_shipment_cost = trytond.modules.account_stock_shipment_cost
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/stock.py` & `trytond_account_stock_shipment_cost-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-6.6.0/tests/scenario_account_stock_shipment_cost.rst` & `trytond_account_stock_shipment_cost-6.8.0/tests/scenario_account_stock_shipment_cost.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
@@ -147,28 +147,28 @@
     >>> shipment_cost1.shipments.extend(
     ...     shipment_cost1.shipments.find([]))
     >>> shipment_cost1.save()
     >>> shipment_cost1.state
     'draft'
     >>> bool(shipment_cost1.number)
     True
-    >>> post_shipment_cost = Wizard('account.shipment_cost.post', [shipment_cost1])
+    >>> post_shipment_cost = shipment_cost1.click('post_wizard')
     >>> post_shipment_cost.form.cost
     Decimal('10.0000')
     >>> sorted([s.cost for s in post_shipment_cost.form.shipments])
     [Decimal('5.0000'), Decimal('5.0000')]
     >>> post_shipment_cost.execute('post')
     >>> shipment_cost1.state
     'posted'
     >>> bool(shipment_cost1.posted_date)
     True
 
 Show shipment cost::
 
-    >>> show_shipment_cost = Wizard('account.shipment_cost.show', [shipment_cost1])
+    >>> show_shipment_cost = shipment_cost1.click('show')
     >>> show_shipment_cost.form.cost
     Decimal('10.0000')
     >>> sorted([s.cost for s in show_shipment_cost.form.shipments])
     [Decimal('5.0000'), Decimal('5.0000')]
 
 Check shipment cost::
 
@@ -190,15 +190,15 @@
     >>> invoice.state
     'posted'
 
     >>> shipment_cost2 = ShipmentCost()
     >>> shipment_cost2.invoice_lines.append(InvoiceLine(line.id))
     >>> shipment_cost2.shipments.append(ShipmentOut(shipment1.id))
     >>> shipment_cost2.save()
-    >>> post_shipment_cost = Wizard('account.shipment_cost.post', [shipment_cost2])
+    >>> post_shipment_cost = shipment_cost2.click('post_wizard')
     >>> post_shipment_cost.form.cost
     Decimal('2.0000')
     >>> sorted([s.cost for s in post_shipment_cost.form.shipments])
     [Decimal('2.0000')]
     >>> try:
     ...     post_shipment_cost.execute('post')
     ... except SamePartiesWarning as warning:
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO` & `trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-stock-shipment-cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to allocate shipment cost based on invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-shipment-cost
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_shipment_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock shipment cost carrier invoice
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
 
 ##################################
 Account Stock Shipment Cost Module
 ##################################
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt` & `trytond_account_stock_shipment_cost-6.8.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_account_stock_shipment_cost-6.6.0/view/shipment_cost_form.xml` & `trytond_account_stock_shipment_cost-6.8.0/view/shipment_cost_form.xml`

 * *Files identical despite different names*

