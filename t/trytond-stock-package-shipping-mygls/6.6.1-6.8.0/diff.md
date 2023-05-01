# Comparing `tmp/trytond_stock_package_shipping_mygls-6.6.1.tar.gz` & `tmp/trytond_stock_package_shipping_mygls-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_mygls-6.6.1.tar", last modified: Mon Jan  2 22:19:41 2023, max compression
+gzip compressed data, was "trytond_stock_package_shipping_mygls-6.8.0.tar", last modified: Mon May  1 11:56:23 2023, max compression
```

## Comparing `trytond_stock_package_shipping_mygls-6.6.1.tar` & `trytond_stock_package_shipping_mygls-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:19:41.733750 trytond_stock_package_shipping_mygls-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-01-02 22:19:38.000000 trytond_stock_package_shipping_mygls-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-01-02 22:19:38.000000 trytond_stock_package_shipping_mygls-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2584 2023-01-02 22:19:41.733750 trytond_stock_package_shipping_mygls-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      994 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/api.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4021 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2734 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:19:41.730417 trytond_stock_package_shipping_mygls-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      931 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_mygls-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:19:41.727084 trytond_stock_package_shipping_mygls-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6786 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6925 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6871 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6957 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5146 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5246 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6760 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6834 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5121 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1992 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-01-02 22:19:41.733750 trytond_stock_package_shipping_mygls-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4872 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11221 2023-01-02 20:25:44.000000 trytond_stock_package_shipping_mygls-6.6.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:19:41.730417 trytond_stock_package_shipping_mygls-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6628 2023-01-02 20:25:44.000000 trytond_stock_package_shipping_mygls-6.6.1/tests/scenario_stock_package_shipping_mygls.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:59.000000 trytond_stock_package_shipping_mygls-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2022-12-19 12:03:07.000000 trytond_stock_package_shipping_mygls-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:19:41.733750 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2584 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1824 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-01-02 22:19:41.000000 trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:19:41.730417 trytond_stock_package_shipping_mygls-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/view/credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2022-12-19 12:02:58.000000 trytond_stock_package_shipping_mygls-6.6.1/view/credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:23.636760 trytond_stock_package_shipping_mygls-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-05-01 11:11:02.000000 trytond_stock_package_shipping_mygls-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:11:02.000000 trytond_stock_package_shipping_mygls-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2563 2023-05-01 11:56:23.636760 trytond_stock_package_shipping_mygls-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      994 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/api.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4021 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2734 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:23.633427 trytond_stock_package_shipping_mygls-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:23.626760 trytond_stock_package_shipping_mygls-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6786 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6925 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6871 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6957 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5146 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5246 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6760 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6799 2023-04-30 10:46:36.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5121 2023-04-29 08:02:48.000000 trytond_stock_package_shipping_mygls-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1992 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:56:23.636760 trytond_stock_package_shipping_mygls-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4808 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11221 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:23.630093 trytond_stock_package_shipping_mygls-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6609 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/tests/scenario_stock_package_shipping_mygls.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-05-01 11:10:57.000000 trytond_stock_package_shipping_mygls-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:23.636760 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2563 2023-05-01 11:56:22.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1824 2023-05-01 11:56:23.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:56:22.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2023-05-01 11:56:22.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-01 11:56:22.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:56:22.000000 trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:23.630093 trytond_stock_package_shipping_mygls-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/view/credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_mygls-6.8.0/view/credential_list.xml
```

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/COPYRIGHT` & `trytond_stock_package_shipping_mygls-6.8.0/COPYRIGHT`

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

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/LICENSE` & `trytond_stock_package_shipping_mygls-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/PKG-INFO` & `trytond_stock_package_shipping_mygls-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_mygls
-Version: 6.6.1
+Version: 6.8.0
 Summary: MyGLS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-mygls
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_mygls
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping gls mygls
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 ###################################
 Stock Package Shipping MyGLS Module
 ###################################
```

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/__init__.py` & `trytond_stock_package_shipping_mygls-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/api.py` & `trytond_stock_package_shipping_mygls-6.8.0/api.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/carrier.py` & `trytond_stock_package_shipping_mygls-6.8.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/carrier.xml` & `trytond_stock_package_shipping_mygls-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/doc/conf.py` & `trytond_stock_package_shipping_mygls-6.8.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/doc/design.rst` & `trytond_stock_package_shipping_mygls-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/bg.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/ca.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/cs.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/de.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/es.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/es_419.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/et.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/fa.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/fi.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/fr.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/hu.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/id.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/it.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/lo.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/lt.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/nl.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/pl.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/pt.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/ro.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/ro.po`

 * *Files 3% similar despite different names*

```diff
@@ -62,48 +62,45 @@
 msgid "Create MyGLS Shipping for Packages"
 msgstr "Creare Expediere MyGLS pentru Colete"
 
 msgctxt "model:ir.action,name:act_credential_form"
 msgid "MyGLS Credentials"
 msgstr "Credenţiale MyGLS"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_email_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add an email for address "
 "\"%(address)s\"."
 msgstr ""
-"Pentru a valida expedierea \"%(shipment)s\" trebuie să adăugaţi o adresă de "
-"e-mail la parte \"%(party)s\"."
+"Pentru a valida expedierea \"%(shipment)s\" trebuie adăugat un e-mail pentru"
+" adresă \"%(address)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_mobile_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add a mobile number for "
 "address \"%(address)s\"."
 msgstr ""
-"Pentru a valida expedierea \"%(shipment)s\" trebuie adăugat un număr de "
-"telefon mobil la parte \"%(party)s\"."
+"Pentru a valida expedierea\"%(shipment)s\" trebuie adăugat un mobil pentru "
+"adresa \"%(address)s\"."
 
 msgctxt "model:ir.message,text:msg_mygls_api_error"
 msgid ""
 "MyGLS API call failed with the following error message:\n"
 "%(message)s"
 msgstr ""
 "Interogarea API MyGLS a eşuat cu următorul mesaj:\n"
 "%(message)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_phone_mobile_required"
 msgid ""
 "To validate shipment \"%(shipment)s\" you must add a phone or mobile number "
 "for address \"%(address)s\"."
 msgstr ""
-"Pentru a valida expedierea \"%(shipment)s\"trebuie adăugat un număr de "
-"telefon mobil la parte \"%(party)s\"."
+"Pentru a valida expedierea \"%(shipment)s\" trebuie adăugat un număr de "
+"telefon sau mobil pentru adresa \"%(address)s\"."
 
 msgctxt "model:ir.message,text:msg_shipment_has_reference_number"
 msgid ""
 "You cannot create a shipping label for shipment \"%(shipment)s\" because it "
 "already has a reference number."
 msgstr ""
 "Nu se poate crea o eticheta pentru expedierea \"%(shipment)s\" pentru că are"
```

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/ru.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/sl.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/tr.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/uk.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/locale/zh_CN.po` & `trytond_stock_package_shipping_mygls-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/message.xml` & `trytond_stock_package_shipping_mygls-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/setup.py` & `trytond_stock_package_shipping_mygls-6.8.0/setup.py`

 * *Files 5% similar despite different names*

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
 name = 'trytond_stock_package_shipping_mygls'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['zeep', 'PyPDF2']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -57,25 +57,24 @@
     ]
 
 setup(name=name,
     version=version,
     description='MyGLS connector for the Tryton application platform',
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
             'modules-stock-package-shipping-mygls'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": (
-            'https://hg.tryton.org/modules/stock_package_shipping_mygls'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping gls mygls',
     package_dir={'trytond.modules.stock_package_shipping_mygls': '.'},
     packages=(
         ['trytond.modules.stock_package_shipping_mygls']
         + ['trytond.modules.stock_package_shipping_mygls.%s' % p
             for p in find_packages()]
@@ -113,23 +112,23 @@
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

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/stock.py` & `trytond_stock_package_shipping_mygls-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/tests/scenario_stock_package_shipping_mygls.rst` & `trytond_stock_package_shipping_mygls-6.8.0/tests/scenario_stock_package_shipping_mygls.rst`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     >>> pack = shipment.packages.new(type=box)
     >>> pack_moves = pack.moves.find([])
     >>> pack.moves.append(pack_moves[0])
     >>> pack = shipment.packages.new(type=box)
     >>> pack.moves.append(pack_moves[1])
     >>> shipment.click('pack')
 
-    >>> create_shipping = Wizard('stock.shipment.create_shipping', [shipment])
+    >>> create_shipping = shipment.click('create_shipping')
     >>> shipment.reload()
     >>> bool(shipment.reference)
     True
     >>> pack, _ = shipment.root_packages
     >>> pack.shipping_label is not None
     True
     >>> pack.shipping_label_mimetype
```

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO` & `trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-package-shipping-mygls
-Version: 6.6.1
+Version: 6.8.0
 Summary: MyGLS connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-mygls
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_mygls
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping gls mygls
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 ###################################
 Stock Package Shipping MyGLS Module
 ###################################
```

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_mygls-6.8.0/trytond_stock_package_shipping_mygls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/view/carrier_form.xml` & `trytond_stock_package_shipping_mygls-6.8.0/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_mygls-6.6.1/view/credential_form.xml` & `trytond_stock_package_shipping_mygls-6.8.0/view/credential_form.xml`

 * *Files identical despite different names*

