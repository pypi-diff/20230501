# Comparing `tmp/trytond_stock_package_shipping_dpd-6.6.2.tar.gz` & `tmp/trytond_stock_package_shipping_dpd-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_dpd-6.6.2.tar", last modified: Sat Apr  1 22:07:09 2023, max compression
+gzip compressed data, was "trytond_stock_package_shipping_dpd-6.8.0.tar", last modified: Mon May  1 11:53:38 2023, max compression
```

## Comparing `trytond_stock_package_shipping_dpd-6.6.2.tar` & `trytond_stock_package_shipping_dpd-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:07:09.057330 trytond_stock_package_shipping_dpd-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     1417 2023-04-01 22:07:04.000000 trytond_stock_package_shipping_dpd-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-04-01 22:07:03.000000 trytond_stock_package_shipping_dpd-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3312 2023-04-01 22:07:09.057330 trytond_stock_package_shipping_dpd-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_dpd-6.6.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4192 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1107 2023-03-12 09:16:43.000000 trytond_stock_package_shipping_dpd-6.6.2/configuration.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:07:09.053997 trytond_stock_package_shipping_dpd-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:07:09.047330 trytond_stock_package_shipping_dpd-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2728 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3188 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2549 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3204 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3220 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2472 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2605 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2549 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3249 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2620 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2525 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2573 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2682 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2573 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3120 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2646 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2796 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2682 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2775 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2549 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2463 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1043 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:07:09.057330 trytond_stock_package_shipping_dpd-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4610 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_dpd-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11801 2023-01-02 20:25:44.000000 trytond_stock_package_shipping_dpd-6.6.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:07:09.050663 trytond_stock_package_shipping_dpd-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7531 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/tests/scenario_shipping_dpd.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-01-02 22:21:01.000000 trytond_stock_package_shipping_dpd-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:07:09.057330 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3312 2023-04-01 22:07:07.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1782 2023-04-01 22:07:08.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:07:07.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-01 22:07:07.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:20:52.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-01 22:07:07.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:07:07.000000 trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:07:09.053997 trytond_stock_package_shipping_dpd-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/view/dpd_credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_dpd-6.6.2/view/dpd_credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:38.678046 trytond_stock_package_shipping_dpd-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1379 2023-05-01 11:09:12.000000 trytond_stock_package_shipping_dpd-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-05-01 11:09:12.000000 trytond_stock_package_shipping_dpd-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_dpd-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3293 2023-05-01 11:53:38.678046 trytond_stock_package_shipping_dpd-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4192 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1107 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/configuration.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:38.674713 trytond_stock_package_shipping_dpd-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:38.671379 trytond_stock_package_shipping_dpd-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2728 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3188 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2549 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3204 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3220 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2472 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2605 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3202 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2549 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3249 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2620 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2525 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2573 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2573 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3120 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2646 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2796 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2775 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2549 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2463 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_dpd-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1043 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:53:38.678046 trytond_stock_package_shipping_dpd-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4548 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11801 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_dpd-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:38.674713 trytond_stock_package_shipping_dpd-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7384 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/tests/scenario_shipping_dpd.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-05-01 11:09:06.000000 trytond_stock_package_shipping_dpd-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:38.678046 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3293 2023-05-01 11:53:37.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1782 2023-05-01 11:53:38.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:53:37.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 11:53:37.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-05-01 11:53:37.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:53:37.000000 trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:38.674713 trytond_stock_package_shipping_dpd-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/view/dpd_credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-6.8.0/view/dpd_credential_list.xml
```

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/CHANGELOG` & `trytond_stock_package_shipping_dpd-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 
-Version 6.6.2 - 2023-04-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-01-02
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add notification preference
 * Use contact mechanism from address
```

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/COPYRIGHT` & `trytond_stock_package_shipping_dpd-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Copyright (C) 2016-2023 B2CK.
-Copyright (C) 2016-2022 Nicolas Évrard.
+Copyright (C) 2016-2023 Nicolas Évrard.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/LICENSE` & `trytond_stock_package_shipping_dpd-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/PKG-INFO` & `trytond_stock_package_shipping_dpd-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_dpd
-Version: 6.6.2
+Version: 6.8.0
 Summary: DPD connector for the Tryton application platform
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_dpd
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping dpd
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
 
 Stock Package Shipping DPD Module
 #################################
 
 The Stock Package Shipping DPD module allows you to generate the DPD label
```

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/README.rst` & `trytond_stock_package_shipping_dpd-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/__init__.py` & `trytond_stock_package_shipping_dpd-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/carrier.py` & `trytond_stock_package_shipping_dpd-6.8.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/carrier.xml` & `trytond_stock_package_shipping_dpd-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/configuration.py` & `trytond_stock_package_shipping_dpd-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/doc/conf.py` & `trytond_stock_package_shipping_dpd-6.8.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/doc/index.rst` & `trytond_stock_package_shipping_dpd-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/bg.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/ca.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/cs.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/de.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/es.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/es_419.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/et.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/fa.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/fi.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/fr.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/hu.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/id.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/it.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/lo.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/lt.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/nl.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/pl.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/pt.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/ro.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/ru.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/sl.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/tr.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/uk.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/locale/zh_CN.po` & `trytond_stock_package_shipping_dpd-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/message.xml` & `trytond_stock_package_shipping_dpd-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/setup.py` & `trytond_stock_package_shipping_dpd-6.8.0/setup.py`

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
@@ -34,16 +31,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_package_shipping_dpd'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['zeep >= 0.12', 'PyPDF2', 'lxml']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -54,23 +54,22 @@
     ]
 
 setup(name=name,
     version=version,
     description='DPD connector for the Tryton application platform',
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
-            'https://hg.tryton.org/modules/stock_package_shipping_dpd'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping dpd',
     package_dir={'trytond.modules.stock_package_shipping_dpd': '.'},
     packages=(
         ['trytond.modules.stock_package_shipping_dpd']
         + ['trytond.modules.stock_package_shipping_dpd.%s' % p
             for p in find_packages()]
@@ -107,23 +106,23 @@
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

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/stock.py` & `trytond_stock_package_shipping_dpd-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/tests/scenario_shipping_dpd.rst` & `trytond_stock_package_shipping_dpd-6.8.0/tests/scenario_shipping_dpd.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 ========================================
 Stock Package Shipping with DPD scenario
 ========================================
 
 Imports::
 
-    >>> import datetime
     >>> import os
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['stock_package_shipping_dpd', 'sale', 'sale_shipment_cost'])
 
 Create company::
@@ -202,23 +199,22 @@
     >>> sale.click('process')
 
 Create the packs and ship the shipment::
 
     >>> Package = Model.get('stock.package')
     >>> shipment, = sale.shipments
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> pack = shipment.packages.new()
     >>> pack.type = box
     >>> pack_move, = pack.moves.find([])
     >>> pack.moves.append(pack_move)
     >>> shipment.click('pack')
 
-    >>> create_shipping = Wizard('stock.shipment.create_shipping', [shipment])
+    >>> create_shipping = shipment.click('create_shipping')
     >>> shipment.reload()
     >>> shipment.reference != ''
     True
     >>> pack, = shipment.root_packages
     >>> pack.shipping_label is not None
     True
     >>> pack.shipping_label_mimetype
```

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO` & `trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-package-shipping-dpd
-Version: 6.6.2
+Version: 6.8.0
 Summary: DPD connector for the Tryton application platform
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_dpd
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping dpd
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
 
 Stock Package Shipping DPD Module
 #################################
 
 The Stock Package Shipping DPD module allows you to generate the DPD label
```

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_dpd-6.8.0/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/view/carrier_form.xml` & `trytond_stock_package_shipping_dpd-6.8.0/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-6.6.2/view/dpd_credential_form.xml` & `trytond_stock_package_shipping_dpd-6.8.0/view/dpd_credential_form.xml`

 * *Files identical despite different names*

