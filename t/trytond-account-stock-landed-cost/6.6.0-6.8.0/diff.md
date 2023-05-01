# Comparing `tmp/trytond_account_stock_landed_cost-6.6.0.tar.gz` & `tmp/trytond_account_stock_landed_cost-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_landed_cost-6.6.0.tar", last modified: Mon Oct 31 16:03:13 2022, max compression
+gzip compressed data, was "trytond_account_stock_landed_cost-6.8.0.tar", last modified: Mon May  1 12:03:16 2023, max compression
```

## Comparing `trytond_account_stock_landed_cost-6.6.0.tar` & `trytond_account_stock_landed_cost-6.8.0.tar`

### file list

```diff
@@ -1,73 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:13.456634 trytond_account_stock_landed_cost-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_stock_landed_cost-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_stock_landed_cost-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2022-10-31 16:03:11.000000 trytond_account_stock_landed_cost-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_stock_landed_cost-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1590 2022-10-31 16:03:10.000000 trytond_account_stock_landed_cost-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:03:09.000000 trytond_account_stock_landed_cost-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:21.000000 trytond_account_stock_landed_cost-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_stock_landed_cost-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3182 2022-10-31 16:03:13.456634 trytond_account_stock_landed_cost-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2018-08-18 09:54:21.000000 trytond_account_stock_landed_cost-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2022-07-17 22:16:37.000000 trytond_account_stock_landed_cost-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20560 2022-10-11 19:49:57.000000 trytond_account_stock_landed_cost-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8970 2022-07-17 22:16:37.000000 trytond_account_stock_landed_cost-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:13.453301 trytond_account_stock_landed_cost-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2018-08-18 09:54:21.000000 trytond_account_stock_landed_cost-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2020-10-11 11:46:39.000000 trytond_account_stock_landed_cost-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:13.449967 trytond_account_stock_landed_cost-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6516 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7044 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7007 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7101 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6263 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6610 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6658 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7203 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6744 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5929 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6551 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6582 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6259 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6815 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6280 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6631 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5794 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6505 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6400 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6206 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5778 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6248 2022-10-29 07:50:44.000000 trytond_account_stock_landed_cost-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2020-10-11 11:46:39.000000 trytond_account_stock_landed_cost-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2022-04-10 15:40:35.000000 trytond_account_stock_landed_cost-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2018-08-18 09:54:21.000000 trytond_account_stock_landed_cost-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:03:13.456634 trytond_account_stock_landed_cost-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5301 2022-10-29 07:39:10.000000 trytond_account_stock_landed_cost-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1158 2022-10-11 19:49:57.000000 trytond_account_stock_landed_cost-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2022-10-11 19:49:57.000000 trytond_account_stock_landed_cost-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:13.453301 trytond_account_stock_landed_cost-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_stock_landed_cost-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7100 2022-09-29 07:07:37.000000 trytond_account_stock_landed_cost-6.6.0/tests/scenario_account_stock_landed_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2022-04-16 16:30:56.000000 trytond_account_stock_landed_cost-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_account_stock_landed_cost-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:10:09.000000 trytond_account_stock_landed_cost-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2022-10-31 16:03:08.000000 trytond_account_stock_landed_cost-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:13.456634 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3182 2022-10-31 16:03:12.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2135 2022-10-31 16:03:13.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:03:12.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2022-10-31 16:03:12.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:14.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2022-10-31 16:03:12.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:03:12.000000 trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:13.453301 trytond_account_stock_landed_cost-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2018-08-18 09:54:21.000000 trytond_account_stock_landed_cost-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2018-08-18 09:54:21.000000 trytond_account_stock_landed_cost-6.6.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2022-07-17 22:16:37.000000 trytond_account_stock_landed_cost-6.6.0/view/landed_cost_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2019-10-11 23:09:47.000000 trytond_account_stock_landed_cost-6.6.0/view/landed_cost_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2022-07-17 22:16:37.000000 trytond_account_stock_landed_cost-6.6.0/view/landed_cost_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2022-07-17 22:16:37.000000 trytond_account_stock_landed_cost-6.6.0/view/landed_cost_show_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2022-10-11 19:49:57.000000 trytond_account_stock_landed_cost-6.6.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2019-06-04 16:49:44.000000 trytond_account_stock_landed_cost-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:16.845221 trytond_account_stock_landed_cost-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1753 2023-05-01 11:15:59.000000 trytond_account_stock_landed_cost-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:15:58.000000 trytond_account_stock_landed_cost-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3164 2023-05-01 12:03:16.845221 trytond_account_stock_landed_cost-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      846 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20560 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8970 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:16.841888 trytond_account_stock_landed_cost-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:16.838554 trytond_account_stock_landed_cost-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6516 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7044 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7007 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7101 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6263 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6610 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6658 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7255 2023-04-30 10:46:36.000000 trytond_account_stock_landed_cost-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6744 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5929 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6551 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6582 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6259 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6815 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6280 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6631 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5803 2023-04-30 10:46:36.000000 trytond_account_stock_landed_cost-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6505 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6400 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5778 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6248 2023-04-29 08:02:50.000000 trytond_account_stock_landed_cost-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      824 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:03:16.845221 trytond_account_stock_landed_cost-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4465 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1158 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:16.838554 trytond_account_stock_landed_cost-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7010 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/tests/scenario_account_stock_landed_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-05-01 11:15:53.000000 trytond_account_stock_landed_cost-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:16.845221 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3164 2023-05-01 12:03:15.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-05-01 12:03:16.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:03:15.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 12:03:15.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-05-01 12:03:15.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:03:15.000000 trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:16.841888 trytond_account_stock_landed_cost-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/view/landed_cost_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/view/landed_cost_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/view/landed_cost_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/view/landed_cost_show_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_stock_landed_cost-6.8.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_account_stock_landed_cost-6.8.0/view/template_form.xml
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/CHANGELOG` & `trytond_account_stock_landed_cost-6.8.0/CHANGELOG`

 * *Files 5% similar despite different names*

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
 * Show cost allocation before and after posting
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/COPYRIGHT` & `trytond_account_stock_landed_cost-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2022 Cédric Krier.
-Copyright (C) 2015-2022 B2CK SPRL.
+Copyright (C) 2015-2023 Cédric Krier.
+Copyright (C) 2015-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/LICENSE` & `trytond_account_stock_landed_cost-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/PKG-INFO` & `trytond_account_stock_landed_cost-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_landed_cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for landed cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_landed_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock valuation landed cost
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
 
 Account Stock Landed Cost Module
 ################################
 
 The account_stock_landed_cost module allows to allocate landed cost on
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/README.rst` & `trytond_account_stock_landed_cost-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/__init__.py` & `trytond_account_stock_landed_cost-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/account.py` & `trytond_account_stock_landed_cost-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/account.xml` & `trytond_account_stock_landed_cost-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/doc/index.rst` & `trytond_account_stock_landed_cost-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/bg.po` & `trytond_account_stock_landed_cost-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/ca.po` & `trytond_account_stock_landed_cost-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/cs.po` & `trytond_account_stock_landed_cost-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/de.po` & `trytond_account_stock_landed_cost-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/es.po` & `trytond_account_stock_landed_cost-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/es_419.po` & `trytond_account_stock_landed_cost-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/et.po` & `trytond_account_stock_landed_cost-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/fa.po` & `trytond_account_stock_landed_cost-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/fi.po` & `trytond_account_stock_landed_cost-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/fr.po` & `trytond_account_stock_landed_cost-6.8.0/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 msgctxt "field:account.landed_cost,number:"
 msgid "Number"
 msgstr "Numéro"
 
 msgctxt "field:account.landed_cost,posted_date:"
 msgid "Posted Date"
-msgstr "Date de postage"
+msgstr "Date de comptabilisation"
 
 msgctxt "field:account.landed_cost,products:"
 msgid "Products"
 msgstr "Produits"
 
 msgctxt "field:account.landed_cost,shipments:"
 msgid "Shipments"
@@ -153,15 +153,15 @@
 
 msgctxt "model:ir.action,name:act_landed_cost_form_shipment"
 msgid "Landed Costs"
 msgstr "Coûts de débarquement"
 
 msgctxt "model:ir.action,name:wizard_landed_cost_post"
 msgid "Post Landed Cost"
-msgstr "Poster le coût de débarquement"
+msgstr "Comptabiliser le coût de débarquement"
 
 msgctxt "model:ir.action,name:wizard_landed_cost_show"
 msgid "Show Landed Cost"
 msgstr "Afficher le coût de débarquement"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_landed_cost_form_domain_all"
@@ -172,21 +172,21 @@
 "model:ir.action.act_window.domain,name:act_landed_cost_form_domain_draft"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_landed_cost_form_domain_posted"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisés"
 
 msgctxt "model:ir.message,text:msg_landed_cost_post_no_stock_move"
 msgid "The posted landed cost \"%(landed_cost)s\" has no stock move."
 msgstr ""
-"Le coût de débarquement posté « %(landed_cost)s » n'a pas de mouvement de "
-"stock."
+"Le coût de débarquement comptabilisé « %(landed_cost)s » n'a pas de "
+"mouvement de stock."
 
 msgctxt "model:ir.message,text:msg_landed_cost_unused_category"
 msgid "The category \"%(category)s\" on landed cost \"%(landed_cost)s\" is not used."
 msgstr ""
 "La catégorie « %(category)s » sur le coût de débarquement "
 "« %(landed_cost)s » n'est pas utilisée."
 
@@ -202,15 +202,15 @@
 
 msgctxt "model:ir.model.button,string:landed_cost_draft_button"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "model:ir.model.button,string:landed_cost_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:landed_cost_show_button"
 msgid "Show"
 msgstr "Afficher"
 
 msgctxt "model:ir.rule.group,name:rule_group_landed_cost_companies"
 msgid "User in companies"
@@ -238,15 +238,15 @@
 
 msgctxt "selection:account.landed_cost,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:account.landed_cost,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "view:account.configuration:"
 msgid "Landed Cost"
 msgstr "Coût de débarquement"
 
 msgctxt "view:account.configuration:"
 msgid "Sequence"
@@ -254,12 +254,12 @@
 
 msgctxt "wizard_button:account.landed_cost.post,show,end:"
 msgid "Cancel"
 msgstr "Annuler"
 
 msgctxt "wizard_button:account.landed_cost.post,show,post:"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "wizard_button:account.landed_cost.show,show,end:"
 msgid "Close"
 msgstr "Fermer"
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/hu.po` & `trytond_account_stock_landed_cost-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/id.po` & `trytond_account_stock_landed_cost-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/it.po` & `trytond_account_stock_landed_cost-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/lo.po` & `trytond_account_stock_landed_cost-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/lt.po` & `trytond_account_stock_landed_cost-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/nl.po` & `trytond_account_stock_landed_cost-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/pl.po` & `trytond_account_stock_landed_cost-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/pt.po` & `trytond_account_stock_landed_cost-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/ro.po` & `trytond_account_stock_landed_cost-6.8.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 msgctxt "field:account.landed_cost,products:"
 msgid "Products"
 msgstr ""
 
 msgctxt "field:account.landed_cost,shipments:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
 
 msgctxt "field:account.landed_cost,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.landed_cost-product.category,category:"
 msgid "Category"
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/ru.po` & `trytond_account_stock_landed_cost-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/sl.po` & `trytond_account_stock_landed_cost-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/tr.po` & `trytond_account_stock_landed_cost-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/uk.po` & `trytond_account_stock_landed_cost-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/locale/zh_CN.po` & `trytond_account_stock_landed_cost-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/message.xml` & `trytond_account_stock_landed_cost-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/product.py` & `trytond_account_stock_landed_cost-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/setup.py` & `trytond_account_stock_landed_cost-6.8.0/setup.py`

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
@@ -34,61 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_stock_landed_cost'
 
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
     description='Tryton module for landed cost',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_stock_landed_cost'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock valuation landed cost',
     package_dir={'trytond.modules.account_stock_landed_cost': '.'},
     packages=(
         ['trytond.modules.account_stock_landed_cost']
         + ['trytond.modules.account_stock_landed_cost.%s' % p
             for p in find_packages()]
@@ -125,28 +102,27 @@
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
     account_stock_landed_cost = trytond.modules.account_stock_landed_cost
     """,
     )
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/stock.py` & `trytond_account_stock_landed_cost-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_landed_cost-6.6.0/tests/scenario_account_stock_landed_cost.rst` & `trytond_account_stock_landed_cost-6.8.0/tests/scenario_account_stock_landed_cost.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 =========================
 Account Stock Landed Cost
 =========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_stock_landed_cost')
 
 Create company::
 
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
     >>> payable = accounts['payable']
@@ -166,30 +166,30 @@
     >>> landed_cost.allocation_method = 'value'
     >>> landed_cost.categories.append(ProductCategory(category.id))
     >>> landed_cost.products.append(Product(product.id))
     >>> landed_cost.save()
     >>> landed_cost.state
     'draft'
 
-    >>> post_landed_cost = Wizard('account.landed_cost.post', [landed_cost])
+    >>> post_landed_cost = landed_cost.click('post_wizard')
     >>> post_landed_cost.form.cost
     Decimal('10.0000')
     >>> sorted([m.cost for m in post_landed_cost.form.moves])
     [Decimal('1.0000')]
     >>> post_landed_cost.execute('post')
     >>> landed_cost.state
     'posted'
     >>> bool(landed_cost.posted_date)
     True
     >>> bool(landed_cost.factors)
     True
 
 Show landed cost::
 
-    >>> show_landed_cost = Wizard('account.landed_cost.show', [landed_cost])
+    >>> show_landed_cost = landed_cost.click('show')
     >>> show_landed_cost.form.cost
     Decimal('10.0000')
     >>> sorted([m.cost for m in show_landed_cost.form.moves])
     [Decimal('1.0000')]
 
 Check move unit price is 101::
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/PKG-INFO` & `trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-stock-landed-cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for landed cost
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_stock_landed_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock valuation landed cost
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
 
 Account Stock Landed Cost Module
 ################################
 
 The account_stock_landed_cost module allows to allocate landed cost on
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/trytond_account_stock_landed_cost.egg-info/SOURCES.txt` & `trytond_account_stock_landed_cost-6.8.0/trytond_account_stock_landed_cost.egg-info/SOURCES.txt`

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
@@ -61,14 +57,15 @@
 ./view/invoice_line_form.xml
 ./view/landed_cost_form.xml
 ./view/landed_cost_list.xml
 ./view/landed_cost_show_form.xml
 ./view/landed_cost_show_move_list.xml
 ./view/stock_move_form.xml
 ./view/template_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_stock_landed_cost-6.6.0/view/landed_cost_form.xml` & `trytond_account_stock_landed_cost-6.8.0/view/landed_cost_form.xml`

 * *Files identical despite different names*

