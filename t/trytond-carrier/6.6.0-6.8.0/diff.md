# Comparing `tmp/trytond_carrier-6.6.0.tar.gz` & `tmp/trytond_carrier-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier-6.6.0.tar", last modified: Mon Oct 31 15:52:08 2022, max compression
+gzip compressed data, was "trytond_carrier-6.8.0.tar", last modified: Mon May  1 11:57:50 2023, max compression
```

## Comparing `trytond_carrier-6.6.0.tar` & `trytond_carrier-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.623634 trytond_carrier-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_carrier-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_carrier-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1128 2022-10-31 15:52:07.000000 trytond_carrier-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_carrier-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2077 2022-10-31 15:52:06.000000 trytond_carrier-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2022-10-31 15:52:06.000000 trytond_carrier-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:28.000000 trytond_carrier-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_carrier-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3134 2022-10-31 15:52:08.623634 trytond_carrier-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      916 2018-08-18 09:54:28.000000 trytond_carrier-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2021-12-11 16:59:33.000000 trytond_carrier-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5136 2021-12-11 16:59:33.000000 trytond_carrier-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6323 2021-10-07 13:09:31.000000 trytond_carrier-6.6.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.620301 trytond_carrier-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      916 2018-08-18 09:54:28.000000 trytond_carrier-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.620301 trytond_carrier-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:32.000000 trytond_carrier-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2019-06-04 16:49:44.000000 trytond_carrier-6.6.0/icons/tryton-carrier.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.620301 trytond_carrier-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2621 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2704 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2717 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2175 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2563 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2959 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2718 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2780 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2334 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2398 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2949 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2664 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2332 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2506 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2575 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2296 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2416 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2108 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2265 2022-10-29 07:50:42.000000 trytond_carrier-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2020-03-01 11:49:44.000000 trytond_carrier-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:52:08.623634 trytond_carrier-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4971 2022-10-29 07:39:10.000000 trytond_carrier-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.620301 trytond_carrier-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_carrier-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2022-04-16 16:30:56.000000 trytond_carrier-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2022-10-31 15:10:09.000000 trytond_carrier-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2022-10-31 15:52:05.000000 trytond_carrier-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.623634 trytond_carrier-6.6.0/trytond_carrier.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3134 2022-10-31 15:52:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1607 2022-10-31 15:52:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:52:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2022-10-31 15:52:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2022-10-31 15:52:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:52:08.000000 trytond_carrier-6.6.0/trytond_carrier.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:08.620301 trytond_carrier-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2020-04-11 13:03:15.000000 trytond_carrier-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2022-04-08 16:23:26.000000 trytond_carrier-6.6.0/view/carrier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2018-08-18 09:54:28.000000 trytond_carrier-6.6.0/view/selection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2022-04-08 16:23:26.000000 trytond_carrier-6.6.0/view/selection_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2022-04-08 16:23:26.000000 trytond_carrier-6.6.0/view/selection_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.187834 trytond_carrier-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2240 2023-05-01 11:12:11.000000 trytond_carrier-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-01 11:12:11.000000 trytond_carrier-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3134 2023-05-01 11:57:50.187834 trytond_carrier-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-01-16 14:00:20.000000 trytond_carrier-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5115 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6323 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.184501 trytond_carrier-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-01-16 14:00:20.000000 trytond_carrier-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.184501 trytond_carrier-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-01-16 14:00:20.000000 trytond_carrier-6.8.0/icons/tryton-carrier.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.181167 trytond_carrier-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2704 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2717 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2175 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2563 2023-04-30 10:46:36.000000 trytond_carrier-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2959 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2718 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2780 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2334 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2398 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2949 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2332 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2506 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2575 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2296 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2108 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-04-29 08:02:48.000000 trytond_carrier-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:57:50.187834 trytond_carrier-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4167 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.181167 trytond_carrier-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-05-01 11:12:04.000000 trytond_carrier-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.184501 trytond_carrier-6.8.0/trytond_carrier.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3134 2023-05-01 11:57:49.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2023-05-01 11:57:50.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:57:49.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 11:57:49.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       94 2023-05-01 11:57:49.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:57:49.000000 trytond_carrier-6.8.0/trytond_carrier.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:50.184501 trytond_carrier-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/view/carrier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-01-16 14:00:20.000000 trytond_carrier-6.8.0/view/selection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/view/selection_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_carrier-6.8.0/view/selection_list_sequence.xml
```

### Comparing `trytond_carrier-6.6.0/CHANGELOG` & `trytond_carrier-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_carrier-6.6.0/COPYRIGHT` & `trytond_carrier-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2022 Cédric Krier.
+Copyright (C) 2011-2023 Cédric Krier.
 Copyright (C) 2011-2013 Bertrand Chenal.
-Copyright (C) 2011-2017 Nicolas Évrard.
-Copyright (C) 2011-2022 B2CK SPRL.
+Copyright (C) 2011-2023 Nicolas Évrard.
+Copyright (C) 2011-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_carrier-6.6.0/LICENSE` & `trytond_carrier-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/PKG-INFO` & `trytond_carrier-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_carrier
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with carriers
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
-Project-URL: Source Code, https://hg.tryton.org/modules/carrier
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 License-File: LICENSE
 
 Carrier Module
 ##############
 
 The carrier module defines the concept of carrier.
```

### Comparing `trytond_carrier-6.6.0/README.rst` & `trytond_carrier-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/carrier.py` & `trytond_carrier-6.8.0/carrier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.cache import Cache
 from trytond.model import (
     DeactivableMixin, MatchMixin, ModelSQL, ModelView, fields,
     sequence_ordered)
 from trytond.pool import Pool
-from trytond.transaction import Transaction
+from trytond.transaction import inactive_records
 
 
 class Carrier(DeactivableMixin, ModelSQL, ModelView):
     'Carrier'
     __name__ = 'carrier'
     party = fields.Many2One('party.party', 'Party', required=True,
             ondelete='CASCADE', help="The party which represents the carrier.")
@@ -123,15 +123,15 @@
         carriers = cls._get_carriers_cache.get(key)
         if carriers is not None:
             return Carrier.browse(carriers)
 
         carriers = []
         selections = cls.search([])
         if not selections:
-            with Transaction().set_context(active_test=False):
+            with inactive_records():
                 carriers = Carrier.search([])
         else:
             for selection in selections:
                 if (selection.match(pattern)
                         and selection.carrier not in carriers):
                     carriers.append(selection.carrier)
```

### Comparing `trytond_carrier-6.6.0/carrier.xml` & `trytond_carrier-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/doc/index.rst` & `trytond_carrier-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/icons/LICENSE` & `trytond_carrier-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/bg.po` & `trytond_carrier-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/ca.po` & `trytond_carrier-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/cs.po` & `trytond_carrier-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/de.po` & `trytond_carrier-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/es.po` & `trytond_carrier-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/es_419.po` & `trytond_carrier-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/et.po` & `trytond_carrier-6.8.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 msgctxt "field:carrier,carrier_product:"
 msgid "Carrier Product"
 msgstr "Vedaja toode"
 
 msgctxt "field:carrier,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 #, fuzzy
 msgctxt "field:carrier,selections:"
 msgid "Selections"
 msgstr "Vedaja valik"
 
 msgctxt "field:carrier.selection,carrier:"
@@ -38,15 +38,15 @@
 
 msgctxt "help:carrier,carrier_product:"
 msgid "The product to invoice the carrier service."
 msgstr "Toose veoteenuse arveldamiseks."
 
 msgctxt "help:carrier,party:"
 msgid "The party which represents the carrier."
-msgstr "Osapool kes esindab vedajat."
+msgstr "Partner kes esindab vedajat."
 
 msgctxt "help:carrier.selection,carrier:"
 msgid "The selected carrier."
 msgstr "Valitud vedaja."
 
 msgctxt "help:carrier.selection,from_country:"
 msgid ""
```

### Comparing `trytond_carrier-6.6.0/locale/fa.po` & `trytond_carrier-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/fi.po` & `trytond_carrier-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/fr.po` & `trytond_carrier-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/hu.po` & `trytond_carrier-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/id.po` & `trytond_carrier-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/it.po` & `trytond_carrier-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/lo.po` & `trytond_carrier-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/lt.po` & `trytond_carrier-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/nl.po` & `trytond_carrier-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/pl.po` & `trytond_carrier-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/pt.po` & `trytond_carrier-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/ro.po` & `trytond_carrier-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/ru.po` & `trytond_carrier-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/sl.po` & `trytond_carrier-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/tr.po` & `trytond_carrier-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/uk.po` & `trytond_carrier-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/locale/zh_CN.po` & `trytond_carrier-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier-6.6.0/setup.py` & `trytond_carrier-6.8.0/setup.py`

 * *Files 16% similar despite different names*

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
@@ -34,59 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_carrier'
 
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
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module with carriers',
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
-        "Source Code": 'https://hg.tryton.org/modules/carrier',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton carrier',
     package_dir={'trytond.modules.carrier': '.'},
     packages=(
         ['trytond.modules.carrier']
         + ['trytond.modules.carrier.%s' % p for p in find_packages()]
         ),
@@ -123,24 +100,23 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     carrier = trytond.modules.carrier
     """,
     )
```

### Comparing `trytond_carrier-6.6.0/trytond_carrier.egg-info/PKG-INFO` & `trytond_carrier-6.8.0/trytond_carrier.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-carrier
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with carriers
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
-Project-URL: Source Code, https://hg.tryton.org/modules/carrier
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 License-File: LICENSE
 
 Carrier Module
 ##############
 
 The carrier module defines the concept of carrier.
```

### Comparing `trytond_carrier-6.6.0/trytond_carrier.egg-info/SOURCES.txt` & `trytond_carrier-6.8.0/trytond_carrier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
@@ -47,14 +43,15 @@
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/carrier_form.xml
 ./view/carrier_tree.xml
 ./view/selection_form.xml
 ./view/selection_list.xml
 ./view/selection_list_sequence.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-carrier.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

