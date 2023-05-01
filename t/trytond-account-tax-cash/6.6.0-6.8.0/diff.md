# Comparing `tmp/trytond_account_tax_cash-6.6.0.tar.gz` & `tmp/trytond_account_tax_cash-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_tax_cash-6.6.0.tar", last modified: Mon Oct 31 16:03:50 2022, max compression
+gzip compressed data, was "trytond_account_tax_cash-6.8.0.tar", last modified: Mon May  1 12:04:28 2023, max compression
```

## Comparing `trytond_account_tax_cash-6.6.0.tar` & `trytond_account_tax_cash-6.8.0.tar`

### file list

```diff
@@ -1,71 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:50.143834 trytond_account_tax_cash-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_tax_cash-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_tax_cash-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2022-10-31 16:03:48.000000 trytond_account_tax_cash-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_tax_cash-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      855 2022-10-31 16:03:47.000000 trytond_account_tax_cash-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:03:47.000000 trytond_account_tax_cash-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_tax_cash-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3015 2022-10-31 16:03:50.143834 trytond_account_tax_cash-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2021-12-11 16:59:32.000000 trytond_account_tax_cash-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12058 2022-04-10 15:40:35.000000 trytond_account_tax_cash-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:50.140501 trytond_account_tax_cash-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:50.140501 trytond_account_tax_cash-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2782 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2869 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3145 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2099 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2156 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2678 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2094 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2022-10-29 07:50:45.000000 trytond_account_tax_cash-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2019-10-11 23:09:47.000000 trytond_account_tax_cash-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2021-10-30 15:32:31.000000 trytond_account_tax_cash-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2021-10-30 15:32:31.000000 trytond_account_tax_cash-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:03:50.143834 trytond_account_tax_cash-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5091 2022-10-29 07:39:10.000000 trytond_account_tax_cash-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:50.140501 trytond_account_tax_cash-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_tax_cash-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5046 2020-07-09 09:37:01.000000 trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3282 2020-07-09 09:37:01.000000 trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash_period_close.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4412 2021-04-03 16:10:54.000000 trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2490 2020-07-09 09:37:01.000000 trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-04-16 16:30:56.000000 trytond_account_tax_cash-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_account_tax_cash-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2022-10-31 15:10:09.000000 trytond_account_tax_cash-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2022-10-31 16:03:45.000000 trytond_account_tax_cash-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:50.143834 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3015 2022-10-31 16:03:49.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2072 2022-10-31 16:03:50.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:03:49.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 16:03:49.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:14.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2022-10-31 16:03:49.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:03:49.000000 trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:03:50.140501 trytond_account_tax_cash-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2019-06-04 16:49:46.000000 trytond_account_tax_cash-6.6.0/view/tax_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:28.266107 trytond_account_tax_cash-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1018 2023-05-01 11:16:47.000000 trytond_account_tax_cash-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:16:47.000000 trytond_account_tax_cash-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3006 2023-05-01 12:04:28.266107 trytond_account_tax_cash-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12012 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:28.262774 trytond_account_tax_cash-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:28.256107 trytond_account_tax_cash-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2782 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2869 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3145 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2099 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2156 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2678 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2094 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-04-29 08:02:51.000000 trytond_account_tax_cash-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:04:28.266107 trytond_account_tax_cash-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4279 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:28.259441 trytond_account_tax_cash-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5046 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3282 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash_period_close.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4412 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2490 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_tax_cash-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2023-05-01 11:16:41.000000 trytond_account_tax_cash-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:28.262774 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3006 2023-05-01 12:04:27.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2046 2023-05-01 12:04:28.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:04:27.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 12:04:27.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-05-01 12:04:27.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:04:27.000000 trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:28.262774 trytond_account_tax_cash-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-01-16 14:00:20.000000 trytond_account_tax_cash-6.8.0/view/tax_line_form.xml
```

### Comparing `trytond_account_tax_cash-6.6.0/CHANGELOG` & `trytond_account_tax_cash-6.8.0/CHANGELOG`

 * *Files 13% similar despite different names*

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

### Comparing `trytond_account_tax_cash-6.6.0/COPYRIGHT` & `trytond_account_tax_cash-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2018-2022 Cédric Krier
-Copyright (C) 2018-2022 B2CK
+Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_tax_cash-6.6.0/LICENSE` & `trytond_account_tax_cash-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/PKG-INFO` & `trytond_account_tax_cash-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_cash
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to support tax report on cash basis
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_tax_cash
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account tax cash
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Account Tax Cash Module
 #######################
 
 The account_tax_cash module allows to make tax report on cash basis.
```

### Comparing `trytond_account_tax_cash-6.6.0/README.rst` & `trytond_account_tax_cash-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/__init__.py` & `trytond_account_tax_cash-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/account.py` & `trytond_account_tax_cash-6.8.0/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             if not invoice.move:
                 continue
             if invoice.company not in periods:
                 with Transaction().set_context(company=invoice.company.id):
                     date = Transaction().context.get(
                         'payment_date', Date.today())
                 periods[invoice.company] = Period.find(
-                    invoice.company.id, date=date)
+                    invoice.company, date=date)
             period = periods[invoice.company]
             ratio = invoice.cash_paid_ratio
             for line in invoice.move.lines:
                 to_update[(period, ratio)].extend(line.tax_lines)
         for (period, ratio), tax_lines in to_update.items():
             TaxLine.update_cash_basis(tax_lines, ratio, period)
 
@@ -327,16 +327,15 @@
                 return True
             if self.invoice.move:
                 period = self.invoice.move.period
             else:
                 accounting_date = (
                     self.invoice.accounting_date or self.invoice.invoice_date)
                 period = Period.find(
-                    self.invoice.company.id, date=accounting_date)
-                period = Period(period)
+                    self.invoice.company, date=accounting_date)
             return period.is_on_cash_basis(self.tax)
 
 
 class InvoiceTaxGroupCash(ModelSQL):
     "Tax Group on Cash Basis per Invoice"
     __name__ = 'account.invoice.tax.group.cash'
```

### Comparing `trytond_account_tax_cash-6.6.0/account.xml` & `trytond_account_tax_cash-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/doc/index.rst` & `trytond_account_tax_cash-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/bg.po` & `trytond_account_tax_cash-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/ca.po` & `trytond_account_tax_cash-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/cs.po` & `trytond_account_tax_cash-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/de.po` & `trytond_account_tax_cash-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/es.po` & `trytond_account_tax_cash-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/es_419.po` & `trytond_account_tax_cash-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/et.po` & `trytond_account_tax_cash-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/fa.po` & `trytond_account_tax_cash-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/fi.po` & `trytond_account_tax_cash-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/fr.po` & `trytond_account_tax_cash-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/hu.po` & `trytond_account_tax_cash-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/id.po` & `trytond_account_tax_cash-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/it.po` & `trytond_account_tax_cash-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/lo.po` & `trytond_account_tax_cash-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/lt.po` & `trytond_account_tax_cash-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/nl.po` & `trytond_account_tax_cash-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/pl.po` & `trytond_account_tax_cash-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/pt.po` & `trytond_account_tax_cash-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/ro.po` & `trytond_account_tax_cash-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/ru.po` & `trytond_account_tax_cash-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/sl.po` & `trytond_account_tax_cash-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/tr.po` & `trytond_account_tax_cash-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/uk.po` & `trytond_account_tax_cash-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/locale/zh_CN.po` & `trytond_account_tax_cash-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/party.py` & `trytond_account_tax_cash-6.8.0/party.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,16 @@
     supplier_tax_group_on_cash_basis = fields.Many2Many(
         'account.tax.group.cash', 'party', 'tax_group',
         "Supplier Tax Group On Cash Basis",
         help="The tax group reported on cash basis for this supplier.")
 
     @classmethod
     def copy(cls, parties, default=None):
-        context = Transaction().context
         default = default.copy() if default else {}
-        if context.get('_check_access'):
+        if Transaction().check_access:
             default.setdefault(
                 'supplier_tax_group_on_cash_basis',
                 cls.default_get(
                     ['supplier_tax_group_on_cash_basis'],
                     with_rec_name=False).get(
                     'supplier_tax_group_on_cash_basis'))
         return super().copy(parties, default=default)
```

### Comparing `trytond_account_tax_cash-6.6.0/party.xml` & `trytond_account_tax_cash-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/setup.py` & `trytond_account_tax_cash-6.8.0/setup.py`

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_tax_cash'
 
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
     description='Tryton module to support tax report on cash basis',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_tax_cash',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account tax cash',
     package_dir={'trytond.modules.account_tax_cash': '.'},
     packages=(
         ['trytond.modules.account_tax_cash']
         + ['trytond.modules.account_tax_cash.%s' % p for p in find_packages()]
         ),
@@ -122,27 +100,26 @@
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
     account_tax_cash = trytond.modules.account_tax_cash
     """,
     )
```

### Comparing `trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash.rst` & `trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash_period_close.rst` & `trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash_period_close.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash_reconciliation.rst` & `trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash_reconciliation.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/tests/scenario_account_tax_cash_supplier.rst` & `trytond_account_tax_cash-6.8.0/tests/scenario_account_tax_cash_supplier.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/PKG-INFO` & `trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-tax-cash
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to support tax report on cash basis
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_tax_cash
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account tax cash
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Account Tax Cash Module
 #######################
 
 The account_tax_cash module allows to make tax report on cash basis.
```

### Comparing `trytond_account_tax_cash-6.6.0/trytond_account_tax_cash.egg-info/SOURCES.txt` & `trytond_account_tax_cash-6.8.0/trytond_account_tax_cash.egg-info/SOURCES.txt`

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
@@ -57,14 +53,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/fiscalyear_form.xml
 ./view/invoice_form.xml
 ./view/party_form.xml
 ./view/period_form.xml
 ./view/tax_line_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

