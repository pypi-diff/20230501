# Comparing `tmp/trytond_stock_package_shipping_sendcloud-6.6.0.tar.gz` & `tmp/trytond_stock_package_shipping_sendcloud-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_sendcloud-6.6.0.tar", last modified: Mon Oct 31 16:32:10 2022, max compression
+gzip compressed data, was "trytond_stock_package_shipping_sendcloud-6.8.0.tar", last modified: Mon May  1 11:53:59 2023, max compression
```

## Comparing `trytond_stock_package_shipping_sendcloud-6.6.0.tar` & `trytond_stock_package_shipping_sendcloud-6.8.0.tar`

### file list

```diff
@@ -1,74 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:10.909099 trytond_stock_package_shipping_sendcloud-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2305 2022-04-25 16:35:02.000000 trytond_stock_package_shipping_sendcloud-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 16:32:09.000000 trytond_stock_package_shipping_sendcloud-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_package_shipping_sendcloud-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-10-31 16:32:08.000000 trytond_stock_package_shipping_sendcloud-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:32:08.000000 trytond_stock_package_shipping_sendcloud-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_package_shipping_sendcloud-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2022-10-31 16:32:10.909099 trytond_stock_package_shipping_sendcloud-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2022-10-27 11:24:45.000000 trytond_stock_package_shipping_sendcloud-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      792 2021-12-11 16:59:34.000000 trytond_stock_package_shipping_sendcloud-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9518 2022-09-19 19:26:12.000000 trytond_stock_package_shipping_sendcloud-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5549 2021-10-07 13:09:31.000000 trytond_stock_package_shipping_sendcloud-6.6.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:10.905765 trytond_stock_package_shipping_sendcloud-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      998 2022-09-14 06:59:12.000000 trytond_stock_package_shipping_sendcloud-6.6.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2022-04-08 16:27:20.000000 trytond_stock_package_shipping_sendcloud-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2022-10-27 11:24:45.000000 trytond_stock_package_shipping_sendcloud-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:45.000000 trytond_stock_package_shipping_sendcloud-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:10.905765 trytond_stock_package_shipping_sendcloud-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3514 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3502 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3553 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2851 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3543 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3450 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:40.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2022-10-29 07:50:41.000000 trytond_stock_package_shipping_sendcloud-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:32:10.909099 trytond_stock_package_shipping_sendcloud-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5703 2022-10-29 07:39:12.000000 trytond_stock_package_shipping_sendcloud-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6802 2022-10-11 19:45:05.000000 trytond_stock_package_shipping_sendcloud-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:10.905765 trytond_stock_package_shipping_sendcloud-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_package_shipping_sendcloud-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7880 2022-09-25 18:27:36.000000 trytond_stock_package_shipping_sendcloud-6.6.0/tests/scenario_stock_package_shipping_sendcloud.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-04-16 16:30:57.000000 trytond_stock_package_shipping_sendcloud-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2022-04-25 16:11:54.000000 trytond_stock_package_shipping_sendcloud-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2022-10-31 15:10:09.000000 trytond_stock_package_shipping_sendcloud-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2022-10-31 16:32:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:10.909099 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2022-10-31 16:32:10.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2184 2022-10-31 16:32:10.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:32:10.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2022-10-31 16:32:10.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-08-21 17:38:21.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-10-31 16:32:10.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:32:10.000000 trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:10.905765 trytond_stock_package_shipping_sendcloud-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/carrier_address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/carrier_address_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2021-10-30 15:16:01.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/carrier_shipping_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/carrier_shipping_method_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2021-10-07 13:08:07.000000 trytond_stock_package_shipping_sendcloud-6.6.0/view/credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:59.108300 trytond_stock_package_shipping_sendcloud-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-05-01 11:09:26.000000 trytond_stock_package_shipping_sendcloud-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:09:26.000000 trytond_stock_package_shipping_sendcloud-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2618 2023-05-01 11:53:59.108300 trytond_stock_package_shipping_sendcloud-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      792 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9468 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5549 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:59.104966 trytond_stock_package_shipping_sendcloud-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:59.101633 trytond_stock_package_shipping_sendcloud-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3514 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3502 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3553 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2851 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3543 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3450 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2948 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-29 08:02:47.000000 trytond_stock_package_shipping_sendcloud-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:53:59.108300 trytond_stock_package_shipping_sendcloud-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4851 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6802 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:59.101633 trytond_stock_package_shipping_sendcloud-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7861 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/tests/scenario_stock_package_shipping_sendcloud.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-05-01 11:09:20.000000 trytond_stock_package_shipping_sendcloud-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:59.108300 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2618 2023-05-01 11:53:58.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2146 2023-05-01 11:53:59.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:53:58.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-05-01 11:53:58.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-05-01 11:53:58.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:53:58.000000 trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:59.104966 trytond_stock_package_shipping_sendcloud-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/carrier_address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/carrier_address_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/carrier_shipping_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/carrier_shipping_method_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_sendcloud-6.8.0/view/credential_list.xml
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/COPYRIGHT` & `trytond_stock_package_shipping_sendcloud-6.8.0/COPYRIGHT`

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

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/LICENSE` & `trytond_stock_package_shipping_sendcloud-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/PKG-INFO` & `trytond_stock_package_shipping_sendcloud-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_sendcloud
-Version: 6.6.0
+Version: 6.8.0
 Summary: Sendcloud connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-sendcloud
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_sendcloud
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping sendcloud
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
 
 #######################################
 Stock Package Shipping Sendcloud Module
 #######################################
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/__init__.py` & `trytond_stock_package_shipping_sendcloud-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/carrier.py` & `trytond_stock_package_shipping_sendcloud-6.8.0/carrier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import time
 from functools import wraps
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
 import requests
 
 from trytond.cache import Cache
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
     MatchMixin, ModelSQL, ModelView, fields, sequence_ordered)
 from trytond.pool import PoolMeta
+from trytond.protocols.wrappers import HTTPStatus
 from trytond.pyson import Eval
 
 from .exceptions import SendcloudError
 
 SENDCLOUD_API_URL = 'https://panel.sendcloud.sc/api/v2/'
 TIMEOUT = config.getfloat(
     'stock_package_shipping_sendcloud', 'requests_timeout', default=300)
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/carrier.xml` & `trytond_stock_package_shipping_sendcloud-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/doc/conf.py` & `trytond_stock_package_shipping_sendcloud-6.8.0/doc/conf.py`

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

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/doc/configuration.rst` & `trytond_stock_package_shipping_sendcloud-6.8.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/doc/design.rst` & `trytond_stock_package_shipping_sendcloud-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/bg.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/ca.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/cs.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/de.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/es.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/es_419.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/et.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/fa.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/fi.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/fr.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/hu.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/id.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/it.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/lo.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/lt.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/nl.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/pl.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/pt.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/ro.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/ru.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/sl.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/tr.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/uk.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/locale/zh_CN.po` & `trytond_stock_package_shipping_sendcloud-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/message.xml` & `trytond_stock_package_shipping_sendcloud-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/setup.py` & `trytond_stock_package_shipping_sendcloud-6.8.0/setup.py`

 * *Files 17% similar despite different names*

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
@@ -37,68 +34,47 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_package_shipping_sendcloud'
 
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
 requires = ['requests']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_sale_shipment_cost'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Sendcloud connector for the Tryton application platform',
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
             'modules-stock-package-shipping-sendcloud'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": (
-            'https://hg.tryton.org/modules/stock_package_shipping_sendcloud'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping sendcloud',
     package_dir={'trytond.modules.stock_package_shipping_sendcloud': '.'},
     packages=(
         ['trytond.modules.stock_package_shipping_sendcloud']
         + ['trytond.modules.stock_package_shipping_sendcloud.%s' % p
             for p in find_packages()]
@@ -137,27 +113,26 @@
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
     stock_package_shipping_sendcloud = trytond.modules.stock_package_shipping_sendcloud
     """,  # noqa: E501
     )
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/stock.py` & `trytond_stock_package_shipping_sendcloud-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/tests/scenario_stock_package_shipping_sendcloud.rst` & `trytond_stock_package_shipping_sendcloud-6.8.0/tests/scenario_stock_package_shipping_sendcloud.rst`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     >>> shipment.click('pick')
     >>> pack = shipment.packages.new()
     >>> pack.type = box
     >>> pack_move, = pack.moves.find([])
     >>> pack.moves.append(pack_move)
     >>> shipment.click('pack')
 
-    >>> create_shipping = Wizard('stock.shipment.create_shipping', [shipment])
+    >>> create_shipping = shipment.click('create_shipping')
     >>> shipment.reload()
     >>> bool(shipment.reference)
     True
     >>> pack, = shipment.root_packages
     >>> bool(pack.sendcloud_shipping_id)
     True
     >>> pack.shipping_label is not None
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/PKG-INFO` & `trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-package-shipping-sendcloud
-Version: 6.6.0
+Version: 6.8.0
 Summary: Sendcloud connector for the Tryton application platform
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-package-shipping-sendcloud
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_sendcloud
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping sendcloud
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
 
 #######################################
 Stock Package Shipping Sendcloud Module
 #######################################
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_sendcloud-6.8.0/trytond_stock_package_shipping_sendcloud.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

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
```

### Comparing `trytond_stock_package_shipping_sendcloud-6.6.0/view/credential_form.xml` & `trytond_stock_package_shipping_sendcloud-6.8.0/view/credential_form.xml`

 * *Files identical despite different names*

