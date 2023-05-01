# Comparing `tmp/trytond_sale_complaint-6.6.0.tar.gz` & `tmp/trytond_sale_complaint-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_complaint-6.6.0.tar", last modified: Mon Oct 31 16:10:58 2022, max compression
+gzip compressed data, was "trytond_sale_complaint-6.8.0.tar", last modified: Mon May  1 11:55:24 2023, max compression
```

## Comparing `trytond_sale_complaint-6.6.0.tar` & `trytond_sale_complaint-6.8.0.tar`

### file list

```diff
@@ -1,78 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.310059 trytond_sale_complaint-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_complaint-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_complaint-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2022-10-31 16:10:56.000000 trytond_sale_complaint-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_complaint-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2022-10-31 16:10:56.000000 trytond_sale_complaint-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:10:55.000000 trytond_sale_complaint-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:01.000000 trytond_sale_complaint-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_complaint-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3930 2022-10-31 16:10:58.310059 trytond_sale_complaint-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2018-08-18 09:55:01.000000 trytond_sale_complaint-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2021-12-11 16:59:34.000000 trytond_sale_complaint-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2020-03-01 11:49:48.000000 trytond_sale_complaint-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29114 2022-10-11 19:49:58.000000 trytond_sale_complaint-6.6.0/complaint.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14106 2021-04-27 07:34:40.000000 trytond_sale_complaint-6.6.0/complaint.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.306726 trytond_sale_complaint-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2018-08-18 09:55:01.000000 trytond_sale_complaint-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.306726 trytond_sale_complaint-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:41.000000 trytond_sale_complaint-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2020-04-13 10:22:05.000000 trytond_sale_complaint-6.6.0/icons/tryton-sale-complaint.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.306726 trytond_sale_complaint-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     9562 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9624 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8685 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9529 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9641 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8224 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9356 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10051 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8672 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9560 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9535 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8875 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9449 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9756 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8754 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9421 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9063 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9573 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8178 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9567 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9409 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8672 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8113 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8846 2022-10-29 07:50:41.000000 trytond_sale_complaint-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2019-10-11 23:09:48.000000 trytond_sale_complaint-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2020-04-13 10:22:05.000000 trytond_sale_complaint-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2666 2022-04-10 15:40:35.000000 trytond_sale_complaint-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2021-03-24 12:34:22.000000 trytond_sale_complaint-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:10:58.310059 trytond_sale_complaint-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5220 2022-10-29 07:39:11.000000 trytond_sale_complaint-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.306726 trytond_sale_complaint-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_complaint-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8133 2021-02-02 12:17:57.000000 trytond_sale_complaint-6.6.0/tests/scenario_sale_complaint.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2022-04-16 16:30:57.000000 trytond_sale_complaint-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_complaint-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2022-10-31 15:10:09.000000 trytond_sale_complaint-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2022-10-31 16:10:54.000000 trytond_sale_complaint-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.310059 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3930 2022-10-31 16:10:57.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2142 2022-10-31 16:10:58.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:10:57.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 16:10:57.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2022-10-31 16:10:57.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:10:57.000000 trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:58.306726 trytond_sale_complaint-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2021-10-07 13:08:07.000000 trytond_sale_complaint-6.6.0/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2021-10-07 13:08:07.000000 trytond_sale_complaint-6.6.0/view/action_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2021-10-07 13:08:07.000000 trytond_sale_complaint-6.6.0/view/action_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2021-10-07 13:08:07.000000 trytond_sale_complaint-6.6.0/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2022-10-11 19:49:58.000000 trytond_sale_complaint-6.6.0/view/complaint_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2022-04-08 16:23:26.000000 trytond_sale_complaint-6.6.0/view/complaint_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2018-08-18 09:55:01.000000 trytond_sale_complaint-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2020-04-13 10:22:05.000000 trytond_sale_complaint-6.6.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2020-04-13 10:22:05.000000 trytond_sale_complaint-6.6.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2020-11-05 23:46:40.000000 trytond_sale_complaint-6.6.0/view/type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2019-10-11 23:09:48.000000 trytond_sale_complaint-6.6.0/view/type_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.186022 trytond_sale_complaint-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1859 2023-05-01 11:10:24.000000 trytond_sale_complaint-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:10:23.000000 trytond_sale_complaint-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_complaint-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3923 2023-05-01 11:55:24.186022 trytond_sale_complaint-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29027 2023-04-21 08:36:08.000000 trytond_sale_complaint-6.8.0/complaint.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14106 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/complaint.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.179355 trytond_sale_complaint-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-01-16 14:00:21.000000 trytond_sale_complaint-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.179355 trytond_sale_complaint-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/icons/tryton-sale-complaint.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.172689 trytond_sale_complaint-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9562 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9624 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8685 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9529 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9641 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8224 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9356 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10051 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8672 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9560 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9535 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8875 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9449 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9756 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8754 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9421 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9063 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9573 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8178 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9567 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9409 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8672 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8113 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8846 2023-04-29 08:02:47.000000 trytond_sale_complaint-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2666 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:55:24.186022 trytond_sale_complaint-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4410 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.176022 trytond_sale_complaint-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8133 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/tests/scenario_sale_complaint.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-05-01 11:10:18.000000 trytond_sale_complaint-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.182689 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3923 2023-05-01 11:55:23.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-05-01 11:55:24.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:55:23.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:55:23.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-05-01 11:55:23.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:55:23.000000 trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:24.179355 trytond_sale_complaint-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/action_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/action_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-28 07:46:16.000000 trytond_sale_complaint-6.8.0/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/complaint_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/complaint_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_sale_complaint-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_sale_complaint-6.8.0/view/type_list.xml
```

### Comparing `trytond_sale_complaint-6.6.0/CHANGELOG` & `trytond_sale_complaint-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

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
 * Add employee on complaint for some states
 * Remove address on complaint
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_sale_complaint-6.6.0/COPYRIGHT` & `trytond_sale_complaint-6.8.0/COPYRIGHT`

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

### Comparing `trytond_sale_complaint-6.6.0/LICENSE` & `trytond_sale_complaint-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/PKG-INFO` & `trytond_sale_complaint-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_complaint
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale complaint
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_complaint
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale customer complaint
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
 
 Sale Complaint Module
 #####################
 
 The sale_complaint module defines Complaint model.
```

### Comparing `trytond_sale_complaint-6.6.0/README.rst` & `trytond_sale_complaint-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/__init__.py` & `trytond_sale_complaint-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/complaint.py` & `trytond_sale_complaint-6.8.0/complaint.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 
     @fields.depends('complaint',
         '_parent_complaint.origin_model', '_parent_complaint.origin')
     def on_change_with_unit(self, name=None):
         if (self.complaint
                 and self.complaint.origin_model in {
                     'sale.line', 'account.invoice.line'}):
-            return self.complaint.origin.unit.id
+            return self.complaint.origin.unit
 
     @fields.depends(
         'quantity', 'unit_price', 'currency', 'sale_lines', 'invoice_lines',
         'complaint', '_parent_complaint.origin_model',
         '_parent_complaint.origin')
     def on_change_with_amount(self, name=None):
         if self.complaint:
@@ -502,15 +502,15 @@
         'complaint',
         '_parent_complaint.origin_model', '_parent_complaint.origin')
     def on_change_with_currency(self, name=None):
         if (self.complaint
                 and self.complaint.origin_model in {
                     'sale.sale', 'sale.line',
                     'account.invoice', 'account.invoice.line'}):
-            return self.complaint.origin.currency.id
+            return self.complaint.origin.currency
 
     @classmethod
     def get_complaint_states(cls):
         pool = Pool()
         Complaint = pool.get('sale.complaint')
         return Complaint.fields_get(['state'])['state']['selection']
 
@@ -702,16 +702,15 @@
         raise NotImplementedError
 
     def get_unit_price(self):
         raise NotImplementedError
 
     @fields.depends('action', '_parent_action.currency')
     def on_change_with_currency(self, name=None):
-        if self.action and self.action.currency:
-            return self.action.currency.id
+        return self.action.currency if self.action else None
 
     @classmethod
     def get_complaint_states(cls):
         pool = Pool()
         Complaint = pool.get('sale.complaint')
         return Complaint.fields_get(['state'])['state']['selection']
 
@@ -738,16 +737,15 @@
         domain=[
             ('type', '=', 'line'),
             ('sale', '=', Eval('complaint_origin_id', -1)),
             ])
 
     @fields.depends('line')
     def on_change_with_unit(self, name=None):
-        if self.line and self.line.unit:
-            return self.line.unit.id
+        return self.line.unit if self.line else None
 
     @fields.depends('quantity', 'line')
     def get_quantity(self):
         if self.quantity is not None:
             return self.quantity
         elif self.line:
             return self.line.quantity
@@ -770,16 +768,15 @@
         domain=[
             ('type', '=', 'line'),
             ('invoice', '=', Eval('complaint_origin_id', -1)),
             ])
 
     @fields.depends('line')
     def on_change_with_unit(self, name=None):
-        if self.line and self.line.unit:
-            return self.line.unit.id
+        return self.line.unit if self.line else None
 
     @fields.depends('quantity', 'line')
     def get_quantity(self):
         if self.quantity is not None:
             return self.quantity
         elif self.line:
             return self.line.quantity
```

### Comparing `trytond_sale_complaint-6.6.0/complaint.xml` & `trytond_sale_complaint-6.8.0/complaint.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/doc/index.rst` & `trytond_sale_complaint-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/icons/LICENSE` & `trytond_sale_complaint-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/bg.po` & `trytond_sale_complaint-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/ca.po` & `trytond_sale_complaint-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/cs.po` & `trytond_sale_complaint-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/de.po` & `trytond_sale_complaint-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/es.po` & `trytond_sale_complaint-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/es_419.po` & `trytond_sale_complaint-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/et.po` & `trytond_sale_complaint-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/fa.po` & `trytond_sale_complaint-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/fi.po` & `trytond_sale_complaint-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/fr.po` & `trytond_sale_complaint-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/hu.po` & `trytond_sale_complaint-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/id.po` & `trytond_sale_complaint-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/it.po` & `trytond_sale_complaint-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/lo.po` & `trytond_sale_complaint-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/lt.po` & `trytond_sale_complaint-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/nl.po` & `trytond_sale_complaint-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/pl.po` & `trytond_sale_complaint-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/pt.po` & `trytond_sale_complaint-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/ro.po` & `trytond_sale_complaint-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/ru.po` & `trytond_sale_complaint-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/sl.po` & `trytond_sale_complaint-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/tr.po` & `trytond_sale_complaint-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/uk.po` & `trytond_sale_complaint-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/locale/zh_CN.po` & `trytond_sale_complaint-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/message.xml` & `trytond_sale_complaint-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/sale.py` & `trytond_sale_complaint-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/sale.xml` & `trytond_sale_complaint-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/setup.py` & `trytond_sale_complaint-6.8.0/setup.py`

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
 name = 'trytond_sale_complaint'
 
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
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for sale complaint',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_complaint',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale customer complaint',
     package_dir={'trytond.modules.sale_complaint': '.'},
     packages=(
         ['trytond.modules.sale_complaint']
         + ['trytond.modules.sale_complaint.%s' % p for p in find_packages()]
         ),
@@ -124,28 +102,27 @@
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
     sale_complaint = trytond.modules.sale_complaint
     """,
     )
```

### Comparing `trytond_sale_complaint-6.6.0/tests/scenario_sale_complaint.rst` & `trytond_sale_complaint-6.8.0/tests/scenario_sale_complaint.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/tox.ini` & `trytond_sale_complaint-6.8.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/sale_complaint/* -m unittest discover -s tests
-    coverage report --include=./**/sale_complaint/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
+passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
-    sqlite: DB_NAME={env:SQLITE_NAME::memory:}
-    postgresql: DB_NAME={env:POSTGRESQL_NAME:test}
-install_command = pip install --pre --find-links https://trydevpi.tryton.org/?local_version={env:CI_JOB_ID:{env:CI_BUILD_NUMBER:}.{env:CI_JOB_NUMBER:}} {opts} {packages}
+    sqlite: DB_NAME={env:DB_NAME::memory:}
+    postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/PKG-INFO` & `trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-complaint
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale complaint
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_complaint
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale customer complaint
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
 
 Sale Complaint Module
 #####################
 
 The sale_complaint module defines Complaint model.
```

### Comparing `trytond_sale_complaint-6.6.0/trytond_sale_complaint.egg-info/SOURCES.txt` & `trytond_sale_complaint-6.8.0/trytond_sale_complaint.egg-info/SOURCES.txt`

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
@@ -63,14 +59,15 @@
 ./view/complaint_form.xml
 ./view/complaint_list.xml
 ./view/configuration_form.xml
 ./view/party_form.xml
 ./view/sale_form.xml
 ./view/type_form.xml
 ./view/type_list.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-sale-complaint.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

### Comparing `trytond_sale_complaint-6.6.0/view/action_form.xml` & `trytond_sale_complaint-6.8.0/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/view/complaint_form.xml` & `trytond_sale_complaint-6.8.0/view/complaint_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_complaint-6.6.0/view/complaint_list.xml` & `trytond_sale_complaint-6.8.0/view/complaint_list.xml`

 * *Files identical despite different names*

