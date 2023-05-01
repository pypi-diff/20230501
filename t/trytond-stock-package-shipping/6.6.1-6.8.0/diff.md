# Comparing `tmp/trytond_stock_package_shipping-6.6.1.tar.gz` & `tmp/trytond_stock_package_shipping-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping-6.6.1.tar", last modified: Sat Mar  4 11:16:26 2023, max compression
+gzip compressed data, was "trytond_stock_package_shipping-6.8.0.tar", last modified: Mon May  1 11:49:42 2023, max compression
```

## Comparing `trytond_stock_package_shipping-6.6.1.tar` & `trytond_stock_package_shipping-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:16:26.266924 trytond_stock_package_shipping-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-03-04 11:16:22.000000 trytond_stock_package_shipping-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-03-04 11:16:22.000000 trytond_stock_package_shipping-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4068 2023-03-04 11:16:26.266924 trytond_stock_package_shipping-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      677 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:16:26.260257 trytond_stock_package_shipping-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2022-12-19 12:02:59.000000 trytond_stock_package_shipping-6.6.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:16:26.253590 trytond_stock_package_shipping-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3768 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3891 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3838 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3873 2022-12-19 12:02:59.000000 trytond_stock_package_shipping-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3190 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3848 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4091 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3975 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3659 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3150 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3340 2022-12-19 12:02:59.000000 trytond_stock_package_shipping-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3519 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3760 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3642 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3932 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3114 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3502 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2022-12-19 12:02:59.000000 trytond_stock_package_shipping-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3114 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3315 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      604 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:16:26.266924 trytond_stock_package_shipping-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4579 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13338 2023-02-27 17:46:08.000000 trytond_stock_package_shipping-6.6.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4228 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:16:26.253590 trytond_stock_package_shipping-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 trytond_stock_package_shipping-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2022-12-19 12:03:07.000000 trytond_stock_package_shipping-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:16:26.263591 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4068 2023-03-04 11:16:25.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1841 2023-03-04 11:16:26.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:16:25.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-03-04 11:16:25.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:16:25.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-03-04 11:16:25.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:16:25.000000 trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:16:26.260257 trytond_stock_package_shipping-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/view/carrier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      925 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/view/package_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/view/package_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      553 2022-12-19 12:02:59.000000 trytond_stock_package_shipping-6.6.1/view/package_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2022-12-19 12:02:58.000000 trytond_stock_package_shipping-6.6.1/view/shipment_out_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:42.198445 trytond_stock_package_shipping-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1860 2023-05-01 11:06:29.000000 trytond_stock_package_shipping-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-05-01 11:06:29.000000 trytond_stock_package_shipping-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4053 2023-05-01 11:49:42.198445 trytond_stock_package_shipping-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      650 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-01-16 14:00:21.000000 trytond_stock_package_shipping-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:42.198445 trytond_stock_package_shipping-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:42.191778 trytond_stock_package_shipping-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2263 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2270 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2192 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2423 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2358 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1791 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1963 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2215 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2192 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1791 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2162 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1791 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1956 2023-04-30 10:46:36.000000 trytond_stock_package_shipping-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      604 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:49:42.198445 trytond_stock_package_shipping-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4536 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10622 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3950 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:42.191778 trytond_stock_package_shipping-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-05-01 11:06:23.000000 trytond_stock_package_shipping-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:42.198445 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4053 2023-05-01 11:49:41.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-05-01 11:49:42.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:49:41.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:49:41.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 11:49:41.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:49:41.000000 trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:42.195111 trytond_stock_package_shipping-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/view/carrier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/view/package_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/view/package_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_stock_package_shipping-6.8.0/view/shipment_out_form.xml
```

### Comparing `trytond_stock_package_shipping-6.6.1/CHANGELOG` & `trytond_stock_package_shipping-6.8.0/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Move dimensions definition to stock_package module
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 --------------------------
```

### Comparing `trytond_stock_package_shipping-6.6.1/COPYRIGHT` & `trytond_stock_package_shipping-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2016-2022 Nicolas Évrard.
+Copyright (C) 2016-2023 Nicolas Évrard.
 Copyright (C) 2016-2023 B2CK.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_stock_package_shipping-6.6.1/LICENSE` & `trytond_stock_package_shipping-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-6.6.1/PKG-INFO` & `trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_package_shipping
-Version: 6.6.1
+Name: trytond-stock-package-shipping
+Version: 6.8.0
 Summary: The package shipping module of the Tryton application platform.
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping
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
 
 Stock Package Shipping Module
 #############################
 
 This module is the base module required to interact with shipping service
```

### Comparing `trytond_stock_package_shipping-6.6.1/README.rst` & `trytond_stock_package_shipping-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-6.6.1/__init__.py` & `trytond_stock_package_shipping-6.8.0/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from trytond.pool import Pool
 
 from . import carrier, stock
 
 
 def register():
     Pool.register(
-        stock.PackageType,
         stock.Package,
         stock.ShipmentOut,
         stock.ShipmentInReturn,
         carrier.Carrier,
         module='stock_package_shipping', type_='model')
     Pool.register(
         stock.CreateShipping,
```

### Comparing `trytond_stock_package_shipping-6.6.1/carrier.xml` & `trytond_stock_package_shipping-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-6.6.1/doc/conf.py` & `trytond_stock_package_shipping-6.8.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping-6.6.1/doc/configuration.rst` & `trytond_stock_package_shipping-6.8.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-6.6.1/doc/index.rst` & `trytond_stock_package_shipping-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-6.6.1/locale/id.po` & `trytond_stock_package_shipping-6.8.0/locale/fa.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,81 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,shipping_service:"
 msgid "Shipping Service"
-msgstr ""
-
-msgctxt "field:stock.package,height:"
-msgid "Height"
-msgstr "Tinggi"
-
-msgctxt "field:stock.package,height_digits:"
-msgid "Height Digits"
-msgstr ""
-
-msgctxt "field:stock.package,height_uom:"
-msgid "Height Unit"
-msgstr ""
-
-msgctxt "field:stock.package,length:"
-msgid "Length"
-msgstr "Panjang"
-
-msgctxt "field:stock.package,length_digits:"
-msgid "Length Digits"
-msgstr ""
-
-msgctxt "field:stock.package,length_uom:"
-msgid "Length Unit"
-msgstr ""
+msgstr "خدمات حمل ونقل"
 
 msgctxt "field:stock.package,shipping_label:"
 msgid "Shipping Label"
-msgstr ""
+msgstr "برچسب حمل ونقل"
 
+#, fuzzy
 msgctxt "field:stock.package,shipping_label_id:"
 msgid "Shipping Label ID"
-msgstr ""
+msgstr "برچسب حمل ونقل"
 
+#, fuzzy
 msgctxt "field:stock.package,shipping_label_mimetype:"
 msgid "Shipping Label MIME Type"
-msgstr ""
+msgstr "برچسب حمل ونقل"
 
 msgctxt "field:stock.package,shipping_reference:"
 msgid "Shipping Reference"
-msgstr ""
+msgstr "مرجع حمل ونقل"
 
 msgctxt "field:stock.package,shipping_tracking_url:"
 msgid "Shipping Tracking URL"
 msgstr ""
 
-msgctxt "field:stock.package,width:"
-msgid "Width"
-msgstr "Lebar"
-
-msgctxt "field:stock.package,width_digits:"
-msgid "Width Digits"
-msgstr ""
-
-msgctxt "field:stock.package,width_uom:"
-msgid "Width Unit"
-msgstr ""
-
-msgctxt "field:stock.package.type,height:"
-msgid "Height"
-msgstr "Tinggi"
-
-msgctxt "field:stock.package.type,height_digits:"
-msgid "Height Digits"
-msgstr ""
-
-msgctxt "field:stock.package.type,height_uom:"
-msgid "Height Unit"
-msgstr ""
-
-msgctxt "field:stock.package.type,length:"
-msgid "Length"
-msgstr "Panjang"
-
-msgctxt "field:stock.package.type,length_digits:"
-msgid "Length Digits"
-msgstr ""
-
-msgctxt "field:stock.package.type,length_uom:"
-msgid "Length Unit"
-msgstr ""
-
-msgctxt "field:stock.package.type,width:"
-msgid "Width"
-msgstr "Lebar"
-
-msgctxt "field:stock.package.type,width_digits:"
-msgid "Width Digits"
-msgstr ""
-
-msgctxt "field:stock.package.type,width_uom:"
-msgid "Width Unit"
-msgstr ""
-
 msgctxt "field:stock.shipment.in.return,carrier:"
 msgid "Carrier"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.shipment.in.return,shipping_description:"
 msgid "Shipping Description"
-msgstr ""
+msgstr "شرح حمل ونقل"
 
 msgctxt "field:stock.shipment.out,shipping_description:"
 msgid "Shipping Description"
-msgstr ""
+msgstr "شرح حمل ونقل"
 
 msgctxt "model:ir.action,name:act_create_shipping_wizard"
 msgid "Create Shipping"
-msgstr ""
+msgstr "ایجاد حمل ونقل"
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_shipping_label"
 msgid "Shipping Label"
-msgstr ""
+msgstr "برچسب حمل ونقل"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_print_shipping_label"
 msgid "Shipping Labels"
-msgstr ""
+msgstr "برچسب حمل ونقل"
 
 msgctxt "model:ir.message,text:msg_shipment_not_packed"
 msgid "To create shipping labels for shipment \"%(shipment)s\", you must pack it."
 msgstr ""
+"برای ایجاد برچسب های حمل و نقل محموله :\"%(shipment)s\"، شما باید آن را بسته"
+" بندی کنید."
 
 msgctxt "model:ir.message,text:msg_shipment_without_carrier"
 msgid "The shipment \"%(shipment)s\" does not have a carrier set."
-msgstr ""
+msgstr "هیچ حمل کننده ایی برای محموله : \"%s\" تنظیم نشده است."
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:package_print_shipping_label_button"
 msgid "Shipping Label"
-msgstr ""
+msgstr "برچسب حمل ونقل"
 
+#, fuzzy
 msgctxt ""
 "model:ir.model.button,string:shipment_in_return_create_shipping_button"
 msgid "Create Shipping for Packages"
-msgstr ""
+msgstr "Create Shipping for Packages"
 
 msgctxt "model:ir.model.button,string:shipment_out_create_shipping_button"
 msgid "Create Shipping for Packages"
-msgstr ""
+msgstr "Create Shipping for Packages"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_package_shipping-6.6.1/locale/lo.po` & `trytond_stock_package_shipping-6.8.0/locale/it.po`

 * *Files 22% similar despite different names*

```diff
@@ -2,44 +2,14 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,shipping_service:"
 msgid "Shipping Service"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,height:"
-msgid "Height"
-msgstr "ນໍ້າໜັກ"
-
-#, fuzzy
-msgctxt "field:stock.package,height_digits:"
-msgid "Height Digits"
-msgstr "ນໍ້າໜັກ"
-
-#, fuzzy
-msgctxt "field:stock.package,height_uom:"
-msgid "Height Unit"
-msgstr "ນໍ້າໜັກ"
-
-#, fuzzy
-msgctxt "field:stock.package,length:"
-msgid "Length"
-msgstr "ຄວາມຍາວ"
-
-#, fuzzy
-msgctxt "field:stock.package,length_digits:"
-msgid "Length Digits"
-msgstr "ຄວາມຍາວ"
-
-#, fuzzy
-msgctxt "field:stock.package,length_uom:"
-msgid "Length Unit"
-msgstr "ຄວາມຍາວ"
-
 msgctxt "field:stock.package,shipping_label:"
 msgid "Shipping Label"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,shipping_label_id:"
 msgid "Shipping Label ID"
@@ -54,67 +24,17 @@
 msgid "Shipping Reference"
 msgstr ""
 
 msgctxt "field:stock.package,shipping_tracking_url:"
 msgid "Shipping Tracking URL"
 msgstr ""
 
-msgctxt "field:stock.package,width:"
-msgid "Width"
-msgstr ""
-
-msgctxt "field:stock.package,width_digits:"
-msgid "Width Digits"
-msgstr ""
-
-msgctxt "field:stock.package,width_uom:"
-msgid "Width Unit"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:stock.package.type,height:"
-msgid "Height"
-msgstr "ນໍ້າໜັກ"
-
-msgctxt "field:stock.package.type,height_digits:"
-msgid "Height Digits"
-msgstr ""
-
-msgctxt "field:stock.package.type,height_uom:"
-msgid "Height Unit"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:stock.package.type,length:"
-msgid "Length"
-msgstr "ຄວາມຍາວ"
-
-msgctxt "field:stock.package.type,length_digits:"
-msgid "Length Digits"
-msgstr ""
-
-msgctxt "field:stock.package.type,length_uom:"
-msgid "Length Unit"
-msgstr ""
-
-msgctxt "field:stock.package.type,width:"
-msgid "Width"
-msgstr ""
-
-msgctxt "field:stock.package.type,width_digits:"
-msgid "Width Digits"
-msgstr ""
-
-msgctxt "field:stock.package.type,width_uom:"
-msgid "Width Unit"
-msgstr ""
-
 msgctxt "field:stock.shipment.in.return,carrier:"
 msgid "Carrier"
-msgstr ""
+msgstr "Vettore"
 
 msgctxt "field:stock.shipment.in.return,shipping_description:"
 msgid "Shipping Description"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,shipping_description:"
 msgid "Shipping Description"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_package_shipping-6.6.1/locale/pl.po` & `trytond_stock_package_shipping-6.8.0/locale/bg.po`

 * *Files 24% similar despite different names*

```diff
@@ -2,44 +2,14 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,shipping_service:"
 msgid "Shipping Service"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,height:"
-msgid "Height"
-msgstr "Wysokość"
-
-#, fuzzy
-msgctxt "field:stock.package,height_digits:"
-msgid "Height Digits"
-msgstr "Cyfry wysokości"
-
-#, fuzzy
-msgctxt "field:stock.package,height_uom:"
-msgid "Height Unit"
-msgstr "Jednostka wysokości"
-
-#, fuzzy
-msgctxt "field:stock.package,length:"
-msgid "Length"
-msgstr "Długość"
-
-#, fuzzy
-msgctxt "field:stock.package,length_digits:"
-msgid "Length Digits"
-msgstr "Cyfry długości"
-
-#, fuzzy
-msgctxt "field:stock.package,length_uom:"
-msgid "Length Unit"
-msgstr "Jednostka długości"
-
 msgctxt "field:stock.package,shipping_label:"
 msgid "Shipping Label"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,shipping_label_id:"
 msgid "Shipping Label ID"
@@ -54,65 +24,14 @@
 msgid "Shipping Reference"
 msgstr ""
 
 msgctxt "field:stock.package,shipping_tracking_url:"
 msgid "Shipping Tracking URL"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,width:"
-msgid "Width"
-msgstr "Szerokość"
-
-#, fuzzy
-msgctxt "field:stock.package,width_digits:"
-msgid "Width Digits"
-msgstr "Cyfry szerokości"
-
-#, fuzzy
-msgctxt "field:stock.package,width_uom:"
-msgid "Width Unit"
-msgstr "Jednostka szerokości"
-
-msgctxt "field:stock.package.type,height:"
-msgid "Height"
-msgstr "Wysokość"
-
-msgctxt "field:stock.package.type,height_digits:"
-msgid "Height Digits"
-msgstr "Cyfry wysokości"
-
-msgctxt "field:stock.package.type,height_uom:"
-msgid "Height Unit"
-msgstr "Jednostka wysokości"
-
-msgctxt "field:stock.package.type,length:"
-msgid "Length"
-msgstr "Długość"
-
-msgctxt "field:stock.package.type,length_digits:"
-msgid "Length Digits"
-msgstr "Cyfry długości"
-
-msgctxt "field:stock.package.type,length_uom:"
-msgid "Length Unit"
-msgstr "Jednostka długości"
-
-msgctxt "field:stock.package.type,width:"
-msgid "Width"
-msgstr "Szerokość"
-
-msgctxt "field:stock.package.type,width_digits:"
-msgid "Width Digits"
-msgstr "Cyfry szerokości"
-
-msgctxt "field:stock.package.type,width_uom:"
-msgid "Width Unit"
-msgstr "Jednostka szerokości"
-
 msgctxt "field:stock.shipment.in.return,carrier:"
 msgid "Carrier"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,shipping_description:"
 msgid "Shipping Description"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_package_shipping-6.6.1/locale/sl.po` & `trytond_stock_package_shipping-6.8.0/locale/sl.po`

 * *Files 23% similar despite different names*

```diff
@@ -2,44 +2,14 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:carrier,shipping_service:"
 msgid "Shipping Service"
 msgstr "Dostavna služba"
 
-#, fuzzy
-msgctxt "field:stock.package,height:"
-msgid "Height"
-msgstr "Višina"
-
-#, fuzzy
-msgctxt "field:stock.package,height_digits:"
-msgid "Height Digits"
-msgstr "Decimalke za višino"
-
-#, fuzzy
-msgctxt "field:stock.package,height_uom:"
-msgid "Height Unit"
-msgstr "Enota višine"
-
-#, fuzzy
-msgctxt "field:stock.package,length:"
-msgid "Length"
-msgstr "Dolžina"
-
-#, fuzzy
-msgctxt "field:stock.package,length_digits:"
-msgid "Length Digits"
-msgstr "Decimalke za dolžino"
-
-#, fuzzy
-msgctxt "field:stock.package,length_uom:"
-msgid "Length Unit"
-msgstr "Enota dolžine"
-
 msgctxt "field:stock.package,shipping_label:"
 msgid "Shipping Label"
 msgstr "Nalepka pošiljke"
 
 #, fuzzy
 msgctxt "field:stock.package,shipping_label_id:"
 msgid "Shipping Label ID"
@@ -54,65 +24,14 @@
 msgid "Shipping Reference"
 msgstr "Sklic paketne dostave"
 
 msgctxt "field:stock.package,shipping_tracking_url:"
 msgid "Shipping Tracking URL"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,width:"
-msgid "Width"
-msgstr "Širina"
-
-#, fuzzy
-msgctxt "field:stock.package,width_digits:"
-msgid "Width Digits"
-msgstr "Decimalke za širino"
-
-#, fuzzy
-msgctxt "field:stock.package,width_uom:"
-msgid "Width Unit"
-msgstr "Enota širine"
-
-msgctxt "field:stock.package.type,height:"
-msgid "Height"
-msgstr "Višina"
-
-msgctxt "field:stock.package.type,height_digits:"
-msgid "Height Digits"
-msgstr "Decimalke za višino"
-
-msgctxt "field:stock.package.type,height_uom:"
-msgid "Height Unit"
-msgstr "Enota višine"
-
-msgctxt "field:stock.package.type,length:"
-msgid "Length"
-msgstr "Dolžina"
-
-msgctxt "field:stock.package.type,length_digits:"
-msgid "Length Digits"
-msgstr "Decimalke za dolžino"
-
-msgctxt "field:stock.package.type,length_uom:"
-msgid "Length Unit"
-msgstr "Enota dolžine"
-
-msgctxt "field:stock.package.type,width:"
-msgid "Width"
-msgstr "Širina"
-
-msgctxt "field:stock.package.type,width_digits:"
-msgid "Width Digits"
-msgstr "Decimalke za širino"
-
-msgctxt "field:stock.package.type,width_uom:"
-msgid "Width Unit"
-msgstr "Enota širine"
-
 msgctxt "field:stock.shipment.in.return,carrier:"
 msgid "Carrier"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.shipment.in.return,shipping_description:"
 msgid "Shipping Description"
```

### Comparing `trytond_stock_package_shipping-6.6.1/message.xml` & `trytond_stock_package_shipping-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping-6.6.1/setup.py` & `trytond_stock_package_shipping-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -37,16 +34,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_package_shipping'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -54,22 +54,22 @@
 
 setup(name=name,
     version=version,
     description=('The package shipping module of the '
         'Tryton application platform.'),
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_package_shipping',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping',
     package_dir={'trytond.modules.stock_package_shipping': '.'},
     packages=(
         ['trytond.modules.stock_package_shipping']
         + ['trytond.modules.stock_package_shipping.%s' % p
             for p in find_packages()]
@@ -106,23 +106,23 @@
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

### Comparing `trytond_stock_package_shipping-6.6.1/stock.py` & `trytond_stock_package_shipping-6.8.0/stock.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,99 +5,30 @@
 from sql import Column
 
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Bool, Eval, Id
+from trytond.pyson import Eval
 from trytond.report import Report
 from trytond.transaction import Transaction
 from trytond.wizard import StateAction, StateTransition, Wizard
 
 from .exceptions import PackWarning
 
 if config.getboolean('stock_package_shipping', 'filestore', default=False):
     file_id = 'shipping_label_id'
     store_prefix = config.get(
         'stock_package_shipping', 'store_prefix', default=None)
 else:
     file_id = store_prefix = None
 
 
-class DimensionsMixin(object):
-    __slots__ = ()
-
-    length = fields.Float('Length', digits=(16, Eval('length_digits', 2)))
-    length_uom = fields.Many2One('product.uom', 'Length Unit',
-        domain=[
-            ('category', '=', Id('product', 'uom_cat_length')),
-            ],
-        states={
-            'required': Bool(Eval('length')),
-            },
-        depends={'length_digits'})
-    length_digits = fields.Function(fields.Integer('Length Digits'),
-        'on_change_with_length_digits')
-    height = fields.Float('Height', digits=(16, Eval('height_digits', 2)))
-    height_uom = fields.Many2One('product.uom', 'Height Unit',
-        domain=[
-            ('category', '=', Id('product', 'uom_cat_length')),
-            ],
-        states={
-            'required': Bool(Eval('height')),
-            },
-        depends={'height_digits'})
-    height_digits = fields.Function(fields.Integer('Height Digits'),
-        'on_change_with_height_digits')
-    width = fields.Float('Width', digits=(16, Eval('width_digits', 2)))
-    width_uom = fields.Many2One('product.uom', 'Width Unit',
-        domain=[
-            ('category', '=', Id('product', 'uom_cat_length')),
-            ],
-        states={
-            'required': Bool(Eval('width')),
-            },
-        depends={'width_digits'})
-    width_digits = fields.Function(fields.Integer('Width Digits'),
-        'on_change_with_width_digits')
-
-    @fields.depends('length_uom')
-    def on_change_with_length_digits(self, name=None):
-        return (self.length_uom.digits if self.length_uom
-            else self.default_length_digits())
-
-    @fields.depends('height_uom')
-    def on_change_with_height_digits(self, name=None):
-        return (self.height_uom.digits if self.height_uom
-            else self.default_height_digits())
-
-    @fields.depends('width_uom')
-    def on_change_with_width_digits(self, name=None):
-        return (self.width_uom.digits if self.width_uom
-            else self.default_width_digits())
-
-    @classmethod
-    def default_length_digits(cls):
-        return 2
-
-    @classmethod
-    def default_height_digits(cls):
-        return 2
-
-    @classmethod
-    def default_width_digits(cls):
-        return 2
-
-
-class PackageType(DimensionsMixin, metaclass=PoolMeta):
-    __name__ = 'stock.package.type'
-
-
-class Package(DimensionsMixin, metaclass=PoolMeta):
+class Package(metaclass=PoolMeta):
     __name__ = 'stock.package'
 
     shipping_reference = fields.Char('Shipping Reference',
         states={
             'readonly': Eval('_parent_shipment', {}).get('carrier', False),
             })
     shipping_label = fields.Binary(
@@ -166,25 +97,14 @@
             bool_op = 'OR'
         domain = super(Package, cls).search_rec_name(name, clause)
         return [bool_op,
             domain,
             ('shipping_reference', *clause[1:]),
             ]
 
-    @fields.depends('type')
-    def on_change_type(self):
-        super().on_change_type()
-        if self.type:
-            self.length = self.type.length
-            self.length_uom = self.type.length_uom
-            self.height = self.type.height
-            self.height_uom = self.type.height_uom
-            self.width = self.type.width
-            self.width_uom = self.type.width_uom
-
     @classmethod
     def copy(cls, packages, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('shipping_reference', None)
```

### Comparing `trytond_stock_package_shipping-6.6.1/stock.xml` & `trytond_stock_package_shipping-6.8.0/stock.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_stock_package_shipping-6.6.1/stock.xml` & `trytond_stock_package_shipping-6.8.0/stock.xml`

```diff
@@ -1,17 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data>
-    <record model="ir.ui.view" id="package_type_view_form">
-      <field name="model">stock.package.type</field>
-      <field name="inherit" ref="stock_package.package_type_view_form"/>
-      <field name="name">package_type_form</field>
-    </record>
     <record model="ir.ui.view" id="package_view_form">
       <field name="model">stock.package</field>
       <field name="inherit" ref="stock_package.package_view_form"/>
       <field name="name">package_form</field>
     </record>
     <record model="ir.ui.view" id="package_view_tree">
       <field name="model">stock.package</field>
```

### Comparing `trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/PKG-INFO` & `trytond_stock_package_shipping-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-package-shipping
-Version: 6.6.1
+Name: trytond_stock_package_shipping
+Version: 6.8.0
 Summary: The package shipping module of the Tryton application platform.
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping
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
 
 Stock Package Shipping Module
 #############################
 
 This module is the base module required to interact with shipping service
```

### Comparing `trytond_stock_package_shipping-6.6.1/trytond_stock_package_shipping.egg-info/SOURCES.txt` & `trytond_stock_package_shipping-6.8.0/trytond_stock_package_shipping.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/carrier_form.xml
 ./view/carrier_tree.xml
 ./view/package_form.xml
 ./view/package_list.xml
-./view/package_type_form.xml
 ./view/shipment_in_return_form.xml
 ./view/shipment_out_form.xml
 doc/conf.py
 doc/configuration.rst
 doc/index.rst
 doc/releases.rst
 locale/bg.po
@@ -91,10 +90,9 @@
 trytond_stock_package_shipping.egg-info/not-zip-safe
 trytond_stock_package_shipping.egg-info/requires.txt
 trytond_stock_package_shipping.egg-info/top_level.txt
 view/carrier_form.xml
 view/carrier_tree.xml
 view/package_form.xml
 view/package_list.xml
-view/package_type_form.xml
 view/shipment_in_return_form.xml
 view/shipment_out_form.xml
```

### Comparing `trytond_stock_package_shipping-6.6.1/view/shipment_in_return_form.xml` & `trytond_stock_package_shipping-6.8.0/view/shipment_in_return_form.xml`

 * *Files identical despite different names*

