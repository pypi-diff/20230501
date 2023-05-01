# Comparing `tmp/trytond_sale_payment-6.6.0.tar.gz` & `tmp/trytond_sale_payment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_payment-6.6.0.tar", last modified: Mon Oct 31 16:17:32 2022, max compression
+gzip compressed data, was "trytond_sale_payment-6.8.0.tar", last modified: Mon May  1 11:58:40 2023, max compression
```

## Comparing `trytond_sale_payment-6.6.0.tar` & `trytond_sale_payment-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:17:32.595792 trytond_sale_payment-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_payment-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_payment-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-31 16:17:31.000000 trytond_sale_payment-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_payment-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      958 2022-10-31 16:17:30.000000 trytond_sale_payment-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      765 2022-10-31 16:17:30.000000 trytond_sale_payment-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35146 2019-06-04 16:49:46.000000 trytond_sale_payment-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_payment-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2729 2022-10-31 16:17:32.595792 trytond_sale_payment-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2019-06-04 16:49:46.000000 trytond_sale_payment-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2021-12-11 16:59:34.000000 trytond_sale_payment-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6141 2022-10-13 16:48:55.000000 trytond_sale_payment-6.6.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:17:32.592459 trytond_sale_payment-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2019-06-04 16:49:46.000000 trytond_sale_payment-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:17:32.592459 trytond_sale_payment-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      628 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      673 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      661 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2022-10-29 07:50:42.000000 trytond_sale_payment-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      594 2022-04-08 16:25:27.000000 trytond_sale_payment-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2927 2022-04-10 15:40:35.000000 trytond_sale_payment-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2020-04-26 13:06:29.000000 trytond_sale_payment-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:17:32.595792 trytond_sale_payment-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5284 2022-10-29 07:39:11.000000 trytond_sale_payment-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:17:32.592459 trytond_sale_payment-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_payment-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5698 2022-04-11 18:44:51.000000 trytond_sale_payment-6.6.0/tests/scenario_sale_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2967 2022-10-13 16:48:55.000000 trytond_sale_payment-6.6.0/tests/scenario_sale_payment_no_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2022-04-16 16:30:57.000000 trytond_sale_payment-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_payment-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2022-10-31 15:10:09.000000 trytond_sale_payment-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2022-10-31 16:17:29.000000 trytond_sale_payment-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:17:32.595792 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2729 2022-10-31 16:17:32.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1578 2022-10-31 16:17:32.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:17:32.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2022-10-31 16:17:32.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:08.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      194 2022-10-31 16:17:32.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:17:32.000000 trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:17:32.592459 trytond_sale_payment-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2020-04-26 13:06:29.000000 trytond_sale_payment-6.6.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:40.785128 trytond_sale_payment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1121 2023-05-01 11:12:43.000000 trytond_sale_payment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      765 2023-05-01 11:12:43.000000 trytond_sale_payment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-01-16 14:00:21.000000 trytond_sale_payment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2724 2023-05-01 11:58:40.785128 trytond_sale_payment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-01-16 14:00:21.000000 trytond_sale_payment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6408 2023-04-21 08:36:08.000000 trytond_sale_payment-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:40.781795 trytond_sale_payment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-01-16 14:00:21.000000 trytond_sale_payment-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:40.778462 trytond_sale_payment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      628 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      673 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      661 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-29 08:02:48.000000 trytond_sale_payment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      594 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2927 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:40.785128 trytond_sale_payment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4476 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:40.781795 trytond_sale_payment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5698 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/tests/scenario_sale_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2967 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/tests/scenario_sale_payment_no_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-05-01 11:12:38.000000 trytond_sale_payment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:40.785128 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2724 2023-05-01 11:58:39.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2023-05-01 11:58:40.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:39.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-05-01 11:58:39.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2023-05-01 11:58:39.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:39.000000 trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:40.781795 trytond_sale_payment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_sale_payment-6.8.0/view/sale_form.xml
```

### Comparing `trytond_sale_payment-6.6.0/CHANGELOG` & `trytond_sale_payment-6.8.0/CHANGELOG`

 * *Files 11% similar despite different names*

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

### Comparing `trytond_sale_payment-6.6.0/COPYRIGHT` & `trytond_sale_payment-6.8.0/COPYRIGHT`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Copyright (c) 2017 Mark S Hayden.
 Copyright (c) 2017 Coalesco Digital Systemc Inc.
-Copyright (c) 2017-2022 Cédric Krier.
-Copyright (c) 2017-2022 B2CK.
+Copyright (c) 2017-2023 Cédric Krier.
+Copyright (c) 2017-2023 B2CK.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_payment-6.6.0/LICENSE` & `trytond_sale_payment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/PKG-INFO` & `trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_sale_payment
-Version: 6.6.0
+Name: trytond-sale-payment
+Version: 6.8.0
 Summary: Tryton module that manage payments on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_payment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale payment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,22 +37,22 @@
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
 
 Sale Payment Module
 ###################
 
 The sale_payment module extends *Sale* to allow payments prior to the creation
```

### Comparing `trytond_sale_payment-6.6.0/account.py` & `trytond_sale_payment-6.8.0/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,26 +135,34 @@
 
     def reconcile_payments(self):
         pool = Pool()
         Payment = pool.get('account.payment')
         Line = pool.get('account.move.line')
         if not hasattr(Payment, 'clearing_move'):
             return
+
+        def balance(line):
+            if self.currency == line.second_currency:
+                return line.amount_second_currency
+            elif self.currency == self.company.currency:
+                return line.debit - line.credit
+            else:
+                return 0
         to_reconcile = []
         for line in self.lines_to_pay:
             if line.reconciliation:
                 continue
             lines = [line]
             for payment in line.payments:
                 if payment.state == 'succeeded' and payment.clearing_move:
                     for pline in payment.clearing_move.lines:
                         if (pline.account == line.account
                                 and not pline.reconciliation):
                             lines.append(pline)
-            if not sum(l.debit - l.credit for l in lines):
+            if not sum(map(balance, lines)):
                 to_reconcile.append(lines)
         for lines in to_reconcile:
             Line.reconcile(lines)
 
     @classmethod
     def _post(cls, invoices):
         pool = Pool()
```

### Comparing `trytond_sale_payment-6.6.0/locale/ca.po` & `trytond_sale_payment-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/de.po` & `trytond_sale_payment-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/es.po` & `trytond_sale_payment-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/et.po` & `trytond_sale_payment-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/fa.po` & `trytond_sale_payment-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/fr.po` & `trytond_sale_payment-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/id.po` & `trytond_sale_payment-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/it.po` & `trytond_sale_payment-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/nl.po` & `trytond_sale_payment-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/pl.po` & `trytond_sale_payment-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/pt.po` & `trytond_sale_payment-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/locale/ro.po` & `trytond_sale_payment-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/message.xml` & `trytond_sale_payment-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/sale.py` & `trytond_sale_payment-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/sale.xml` & `trytond_sale_payment-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/setup.py` & `trytond_sale_payment-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
@@ -34,62 +31,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_payment'
 
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
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 for dep in ['account_payment_clearing']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module that manage payments on sale',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_payment',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale payment',
     package_dir={'trytond.modules.sale_payment': '.'},
     packages=(
         ['trytond.modules.sale_payment']
         + ['trytond.modules.sale_payment.%s' % p for p in find_packages()]
         ),
@@ -125,28 +103,27 @@
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
     sale_payment = trytond.modules.sale_payment
     """,
     )
```

### Comparing `trytond_sale_payment-6.6.0/tests/scenario_sale_payment.rst` & `trytond_sale_payment-6.8.0/tests/scenario_sale_payment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/tests/scenario_sale_payment_no_clearing.rst` & `trytond_sale_payment-6.8.0/tests/scenario_sale_payment_no_clearing.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/PKG-INFO` & `trytond_sale_payment-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-sale-payment
-Version: 6.6.0
+Name: trytond_sale_payment
+Version: 6.8.0
 Summary: Tryton module that manage payments on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_payment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale payment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,22 +37,22 @@
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
 
 Sale Payment Module
 ###################
 
 The sale_payment module extends *Sale* to allow payments prior to the creation
```

### Comparing `trytond_sale_payment-6.6.0/trytond_sale_payment.egg-info/SOURCES.txt` & `trytond_sale_payment-6.8.0/trytond_sale_payment.egg-info/SOURCES.txt`

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
@@ -47,14 +43,15 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_payment.rst
 ./tests/scenario_sale_payment_no_clearing.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/sale_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

