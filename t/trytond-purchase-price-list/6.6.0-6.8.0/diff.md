# Comparing `tmp/trytond_purchase_price_list-6.6.0.tar.gz` & `tmp/trytond_purchase_price_list-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_price_list-6.6.0.tar", last modified: Mon Oct 31 16:10:14 2022, max compression
+gzip compressed data, was "trytond_purchase_price_list-6.8.0.tar", last modified: Mon May  1 11:56:04 2023, max compression
```

## Comparing `trytond_purchase_price_list-6.6.0.tar` & `trytond_purchase_price_list-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:14.286086 trytond_purchase_price_list-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:02.000000 trytond_purchase_price_list-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-02-27 09:26:42.000000 trytond_purchase_price_list-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 16:10:12.000000 trytond_purchase_price_list-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_purchase_price_list-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2022-10-31 16:10:12.000000 trytond_purchase_price_list-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:10:11.000000 trytond_purchase_price_list-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-02-27 09:26:42.000000 trytond_purchase_price_list-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_purchase_price_list-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2444 2022-10-31 16:10:14.286086 trytond_purchase_price_list-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2022-10-27 11:24:44.000000 trytond_purchase_price_list-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2021-12-11 16:59:33.000000 trytond_purchase_price_list-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:14.282753 trytond_purchase_price_list-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-02-27 09:26:42.000000 trytond_purchase_price_list-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2022-04-08 16:27:20.000000 trytond_purchase_price_list-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2022-10-27 11:24:44.000000 trytond_purchase_price_list-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_purchase_price_list-6.6.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:14.282753 trytond_purchase_price_list-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      937 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_purchase_price_list-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2022-10-11 19:49:58.000000 trytond_purchase_price_list-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2021-02-27 09:26:42.000000 trytond_purchase_price_list-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1937 2022-04-08 16:23:26.000000 trytond_purchase_price_list-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2022-04-10 15:40:35.000000 trytond_purchase_price_list-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:10:14.286086 trytond_purchase_price_list-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5401 2022-10-29 07:39:11.000000 trytond_purchase_price_list-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:14.282753 trytond_purchase_price_list-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_purchase_price_list-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2571 2021-02-27 09:26:42.000000 trytond_purchase_price_list-6.6.0/tests/scenario_purchase_price_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2022-04-16 16:30:57.000000 trytond_purchase_price_list-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_purchase_price_list-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-31 15:10:09.000000 trytond_purchase_price_list-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2022-10-31 16:10:10.000000 trytond_purchase_price_list-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:14.286086 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2444 2022-10-31 16:10:13.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2022-10-31 16:10:14.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:10:13.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2022-10-31 16:10:13.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-02-27 09:17:55.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2022-10-31 16:10:13.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:10:13.000000 trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:14.282753 trytond_purchase_price_list-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2021-02-27 09:26:42.000000 trytond_purchase_price_list-6.6.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:04.149851 trytond_purchase_price_list-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-05-01 11:10:49.000000 trytond_purchase_price_list-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 11:10:49.000000 trytond_purchase_price_list-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2432 2023-05-01 11:56:04.149851 trytond_purchase_price_list-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:04.146518 trytond_purchase_price_list-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:04.143185 trytond_purchase_price_list-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      937 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_purchase_price_list-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1937 2023-04-22 08:56:15.000000 trytond_purchase_price_list-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:56:04.149851 trytond_purchase_price_list-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:04.143185 trytond_purchase_price_list-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2571 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/tests/scenario_purchase_price_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-05-01 11:10:44.000000 trytond_purchase_price_list-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:04.149851 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2432 2023-05-01 11:56:03.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-05-01 11:56:04.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:56:03.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 11:56:03.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2023-05-01 11:56:03.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:56:03.000000 trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:04.146518 trytond_purchase_price_list-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_purchase_price_list-6.8.0/view/party_form.xml
```

### Comparing `trytond_purchase_price_list-6.6.0/COPYRIGHT` & `trytond_purchase_price_list-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020-2022 Cédric Krier
+Copyright (C) 2020-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_price_list-6.6.0/LICENSE` & `trytond_purchase_price_list-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/PKG-INFO` & `trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_purchase_price_list
-Version: 6.6.0
+Name: trytond-purchase-price-list
+Version: 6.8.0
 Summary: Tryton module to add price list on purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase-price-list
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_price_list
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase price list
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
 
 ##########################
 Purchase Price List Module
 ##########################
```

### Comparing `trytond_purchase_price_list-6.6.0/doc/conf.py` & `trytond_purchase_price_list-6.8.0/doc/conf.py`

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

### Comparing `trytond_purchase_price_list-6.6.0/doc/design.rst` & `trytond_purchase_price_list-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/bg.po` & `trytond_purchase_price_list-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/ca.po` & `trytond_purchase_price_list-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/cs.po` & `trytond_purchase_price_list-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/de.po` & `trytond_purchase_price_list-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/es.po` & `trytond_purchase_price_list-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/es_419.po` & `trytond_purchase_price_list-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/et.po` & `trytond_purchase_price_list-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/fa.po` & `trytond_purchase_price_list-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/fi.po` & `trytond_purchase_price_list-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/fr.po` & `trytond_purchase_price_list-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/hu.po` & `trytond_purchase_price_list-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/id.po` & `trytond_purchase_price_list-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/it.po` & `trytond_purchase_price_list-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/lo.po` & `trytond_purchase_price_list-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/lt.po` & `trytond_purchase_price_list-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/nl.po` & `trytond_purchase_price_list-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/pl.po` & `trytond_purchase_price_list-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/pt.po` & `trytond_purchase_price_list-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/ro.po` & `trytond_purchase_price_list-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/ru.po` & `trytond_purchase_price_list-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/sl.po` & `trytond_purchase_price_list-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/tr.po` & `trytond_purchase_price_list-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/uk.po` & `trytond_purchase_price_list-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/locale/zh_CN.po` & `trytond_purchase_price_list-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/party.py` & `trytond_purchase_price_list-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/product.py` & `trytond_purchase_price_list-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/purchase.py` & `trytond_purchase_price_list-6.8.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/setup.py` & `trytond_purchase_price_list-6.8.0/setup.py`

 * *Files 11% similar despite different names*

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
@@ -37,62 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_price_list'
 
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
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module to add price list on purchase',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-purchase-price-list'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/purchase_price_list',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase price list',
     package_dir={'trytond.modules.purchase_price_list': '.'},
     packages=(
         ['trytond.modules.purchase_price_list']
         + ['trytond.modules.purchase_price_list.%s' % p
             for p in find_packages()]
@@ -130,27 +107,26 @@
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
     purchase_price_list = trytond.modules.purchase_price_list
     """,  # noqa: E501
     )
```

### Comparing `trytond_purchase_price_list-6.6.0/tests/scenario_purchase_price_list.rst` & `trytond_purchase_price_list-6.8.0/tests/scenario_purchase_price_list.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/PKG-INFO` & `trytond_purchase_price_list-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-price-list
-Version: 6.6.0
+Name: trytond_purchase_price_list
+Version: 6.8.0
 Summary: Tryton module to add price list on purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-purchase-price-list
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_price_list
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase price list
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
 
 ##########################
 Purchase Price List Module
 ##########################
```

### Comparing `trytond_purchase_price_list-6.6.0/trytond_purchase_price_list.egg-info/SOURCES.txt` & `trytond_purchase_price_list-6.8.0/trytond_purchase_price_list.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

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
 party.py
```

