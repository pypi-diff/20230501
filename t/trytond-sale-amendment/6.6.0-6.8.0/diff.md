# Comparing `tmp/trytond_sale_amendment-6.6.0.tar.gz` & `tmp/trytond_sale_amendment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_amendment-6.6.0.tar", last modified: Mon Oct 31 16:20:16 2022, max compression
+gzip compressed data, was "trytond_sale_amendment-6.8.0.tar", last modified: Mon May  1 11:49:06 2023, max compression
```

## Comparing `trytond_sale_amendment-6.6.0.tar` & `trytond_sale_amendment-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:16.518175 trytond_sale_amendment-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_amendment-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_amendment-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-10-31 16:20:15.000000 trytond_sale_amendment-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_amendment-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      641 2022-10-31 16:20:14.000000 trytond_sale_amendment-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:20:14.000000 trytond_sale_amendment-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_amendment-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2022-10-31 16:20:16.518175 trytond_sale_amendment-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2021-12-11 16:59:34.000000 trytond_sale_amendment-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:16.518175 trytond_sale_amendment-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:16.514842 trytond_sale_amendment-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4218 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4229 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4251 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4259 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3762 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4270 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4228 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3645 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3589 2022-10-29 07:50:38.000000 trytond_sale_amendment-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16537 2022-10-11 19:49:58.000000 trytond_sale_amendment-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5282 2021-03-24 12:34:22.000000 trytond_sale_amendment-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:20:16.518175 trytond_sale_amendment-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5142 2022-10-29 07:39:11.000000 trytond_sale_amendment-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:16.514842 trytond_sale_amendment-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_amendment-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4510 2021-02-02 12:22:17.000000 trytond_sale_amendment-6.6.0/tests/scenario_sale_amendment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-04-16 16:30:57.000000 trytond_sale_amendment-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_amendment-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2022-10-31 15:10:09.000000 trytond_sale_amendment-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      129 2022-10-31 16:20:13.000000 trytond_sale_amendment-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:16.518175 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2022-10-31 16:20:15.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1772 2022-10-31 16:20:16.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:20:15.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 16:20:15.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-11-04 12:07:07.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2022-10-31 16:20:15.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:20:15.000000 trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:20:16.518175 trytond_sale_amendment-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      647 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/view/sale_amendment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1305 2022-10-11 19:45:05.000000 trytond_sale_amendment-6.6.0/view/sale_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/view/sale_amendment_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-04-08 16:23:26.000000 trytond_sale_amendment-6.6.0/view/sale_amendment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2019-10-11 23:19:18.000000 trytond_sale_amendment-6.6.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:06.281332 trytond_sale_amendment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      837 2023-05-01 11:06:04.000000 trytond_sale_amendment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:06:03.000000 trytond_sale_amendment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-05-01 11:49:06.281332 trytond_sale_amendment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:06.277999 trytond_sale_amendment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:06.274666 trytond_sale_amendment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4347 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4360 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4382 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4398 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3870 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4378 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4358 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3753 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3697 2023-04-30 10:46:36.000000 trytond_sale_amendment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16622 2023-04-21 08:36:08.000000 trytond_sale_amendment-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5880 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:49:06.281332 trytond_sale_amendment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4332 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:06.274666 trytond_sale_amendment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4510 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/tests/scenario_sale_amendment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      129 2023-05-01 11:05:58.000000 trytond_sale_amendment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:06.281332 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-05-01 11:49:05.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-05-01 11:49:06.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:49:05.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:49:05.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-05-01 11:49:05.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:49:05.000000 trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:06.277999 trytond_sale_amendment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      621 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/view/sale_amendment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1305 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/view/sale_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/view/sale_amendment_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/view/sale_amendment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_sale_amendment-6.8.0/view/sale_form.xml
```

### Comparing `trytond_sale_amendment-6.6.0/CHANGELOG` & `trytond_sale_amendment-6.8.0/CHANGELOG`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Add company rule for amendment
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

### Comparing `trytond_sale_amendment-6.6.0/COPYRIGHT` & `trytond_sale_amendment-6.8.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2019-2022 B2CK
-Copyright (C) 2019-2022 Cédric Krier
+Copyright (C) 2019-2023 B2CK
+Copyright (C) 2019-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_amendment-6.6.0/LICENSE` & `trytond_sale_amendment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-6.6.0/PKG-INFO` & `trytond_sale_amendment-6.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_amendment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to amend sales
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_amendment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale amendment
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
 
 Sale Amendment Module
 #####################
 
 The sale amendment module allows you to change sales that are being processed
```

### Comparing `trytond_sale_amendment-6.6.0/README.rst` & `trytond_sale_amendment-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-6.6.0/doc/index.rst` & `trytond_sale_amendment-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-6.6.0/locale/bg.po` & `trytond_sale_amendment-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.amendment,date:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
 msgctxt "field:sale.amendment,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:sale.amendment,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:sale.amendment,sale:"
 msgid "Sale"
@@ -20,23 +20,23 @@
 
 msgctxt "field:sale.amendment,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,action:"
 msgid "Action"
-msgstr ""
+msgstr "Acțiune"
 
 msgctxt "field:sale.amendment.line,amendment:"
 msgid "Amendment"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:sale.amendment.line,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,invoice_party:"
 msgid "Invoice Party"
@@ -44,23 +44,23 @@
 
 msgctxt "field:sale.amendment.line,line:"
 msgid "Line"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:sale.amendment.line,payment_term:"
 msgid "Payment Term"
-msgstr ""
+msgstr "Termen de plata"
 
 msgctxt "field:sale.amendment.line,product:"
 msgid "Product"
-msgstr ""
+msgstr "Produs"
 
 msgctxt "field:sale.amendment.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,quantity:"
 msgid "Quantity"
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_amendment-6.6.0/locale/ca.po` & `trytond_sale_amendment-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 msgstr "Esteu segurs que voleu validar les correccions?"
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Valida"
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr "Usuari a les empreses"
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Correccions"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr "Correcció de venta"
```

### Comparing `trytond_sale_amendment-6.6.0/locale/cs.po` & `trytond_sale_amendment-6.8.0/locale/bg.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/de.po` & `trytond_sale_amendment-6.8.0/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 msgstr "Änderung tatsächlich bestätigen?"
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Bestätigen"
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr "Benutzer im Unternehmen"
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Änderungen"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr "Verkauf Änderung"
```

### Comparing `trytond_sale_amendment-6.6.0/locale/es.po` & `trytond_sale_amendment-6.8.0/locale/es.po`

 * *Files 8% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 msgstr "¿Estas seguro que quieres validar las correciones?"
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Validar"
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr "Usuario en las empresas"
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Correcciones"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr "Correción de venta"
```

### Comparing `trytond_sale_amendment-6.6.0/locale/es_419.po` & `trytond_sale_amendment-6.8.0/locale/cs.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/et.po` & `trytond_sale_amendment-6.8.0/locale/es_419.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/fa.po` & `trytond_sale_amendment-6.8.0/locale/et.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/fi.po` & `trytond_sale_amendment-6.8.0/locale/fa.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/fr.po` & `trytond_sale_amendment-6.8.0/locale/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 msgstr "Êtes-vous sûr de vouloir valider les amendements ?"
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Valider"
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr "Utilisateur dans les sociétés"
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Amendements"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr "Amendement de vente"
```

### Comparing `trytond_sale_amendment-6.6.0/locale/hu.po` & `trytond_sale_amendment-6.8.0/locale/fi.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/id.po` & `trytond_sale_amendment-6.8.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/it.po` & `trytond_sale_amendment-6.8.0/locale/it.po`

 * *Files 6% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 msgstr "Sei sicuro di voler verificare le correzioni?"
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Verifica"
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Correzioni"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr "Modifiche sulla vendita"
```

### Comparing `trytond_sale_amendment-6.6.0/locale/lo.po` & `trytond_sale_amendment-6.8.0/locale/hu.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/lt.po` & `trytond_sale_amendment-6.8.0/locale/lo.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/nl.po` & `trytond_sale_amendment-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 msgstr "Weet u zeker dat u de wijzigingen wilt valideren?"
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "bevestigen"
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr "Gebruiker in bedrijven"
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr "Wijzigingen"
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr "Verkoop wijziging"
```

### Comparing `trytond_sale_amendment-6.6.0/locale/pl.po` & `trytond_sale_amendment-6.8.0/locale/lt.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/pt.po` & `trytond_sale_amendment-6.8.0/locale/pl.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/ro.po` & `trytond_sale_amendment-6.8.0/locale/pt.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:sale.amendment,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:sale.amendment,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.amendment,lines:"
 msgid "Lines"
 msgstr ""
 
 msgctxt "field:sale.amendment,sale:"
 msgid "Sale"
@@ -20,23 +20,23 @@
 
 msgctxt "field:sale.amendment,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,action:"
 msgid "Action"
-msgstr "Acțiune"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,amendment:"
 msgid "Amendment"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,invoice_party:"
 msgid "Invoice Party"
@@ -44,23 +44,23 @@
 
 msgctxt "field:sale.amendment.line,line:"
 msgid "Line"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,payment_term:"
 msgid "Payment Term"
-msgstr "Termen de plata"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:sale.amendment.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
 msgctxt "field:sale.amendment.line,quantity:"
 msgid "Quantity"
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_amendment-6.6.0/locale/ru.po` & `trytond_sale_amendment-6.8.0/locale/ru.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/sl.po` & `trytond_sale_amendment-6.8.0/locale/sl.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/tr.po` & `trytond_sale_amendment-6.8.0/locale/tr.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/uk.po` & `trytond_sale_amendment-6.8.0/locale/uk.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/locale/zh_CN.po` & `trytond_sale_amendment-6.8.0/locale/zh_CN.po`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:sale_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_sale_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_sale_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:res.group,name:group_sale_amendment"
 msgid "Sale Amendment"
 msgstr ""
```

### Comparing `trytond_sale_amendment-6.6.0/sale.py` & `trytond_sale_amendment-6.8.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     state = fields.Selection([
             ('draft', "Draft"),
             ('validated', "Validated"),
             ], "State", readonly=True, required=True, sort=False)
     lines = fields.One2Many(
         'sale.amendment.line', 'amendment', "Lines",
         states={
-            'readonly': Eval('state') != 'draft',
+            'readonly': (
+                (Eval('state') != 'draft')
+                | ~Eval('sale')),
             })
 
     @classmethod
     def __setup__(cls):
         super(Amendment, cls).__setup__()
         t = cls.__table__()
         cls._sql_indexes.add(
@@ -208,15 +210,15 @@
         states={
             'readonly': Eval('state') != 'draft',
             'invisible': Eval('action') != 'line',
             'required': Eval('action') == 'line',
             })
 
     payment_term = fields.Many2One(
-        'account.invoice.payment_term', "Payment Term",
+        'account.invoice.payment_term', "Payment Term", ondelete='RESTRICT',
         states={
             'invisible': Eval('action') != 'payment_term',
             })
 
     party = fields.Many2One(
         'party.party', "Party",
         states={
@@ -276,15 +278,16 @@
             'invisible': Eval('action') != 'warehouse',
             'required': Eval('action') == 'warehouse',
             })
 
     product = fields.Many2One(
         'product.product', "Product",
         domain=[
-            If(Eval('state') == 'draft',
+            If((Eval('state') == 'draft')
+                & ~(Eval('quantity', 0) < 0),
                 ('salable', '=', True),
                 ()),
             If(Eval('product_uom_category'),
                 ('default_uom_category', '=', Eval('product_uom_category')),
                 ()),
             ],
         states={
@@ -378,16 +381,15 @@
         self.on_change_line()
         self.on_change_amendment()
 
     @fields.depends(
         'amendment',
         '_parent_amendment.sale')
     def on_change_with_sale(self, name=None):
-        if self.amendment and self.amendment.sale:
-            return self.amendment.sale.id
+        return self.amendment.sale if self.amendment else None
 
     @fields.depends('line')
     def on_change_line(self):
         if self.line:
             self.product = self.line.product
             self.quantity = self.line.quantity
             self.unit = self.line.unit
@@ -431,17 +433,17 @@
             elif self.party:
                 self.shipment_address = self.party.address_get(type='delivery')
 
     @fields.depends('line')
     def on_change_with_product_uom_category(self, name=None):
         if self.line:
             if self.line.product_uom_category:
-                return self.line.product_uom_category.id
+                return self.line.product_uom_category
             elif self.line.unit:
-                return self.line.unit.category.id
+                return self.line.unit.category
 
     def apply(self, sale):
         assert self.sale == sale
         sale_line = None
         if self.line:
             for line in sale.lines:
                 if self.line == line:
```

### Comparing `trytond_sale_amendment-6.6.0/sale.xml` & `trytond_sale_amendment-6.8.0/sale.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_sale_amendment-6.6.0/sale.xml` & `trytond_sale_amendment-6.8.0/sale.xml`

```diff
@@ -70,14 +70,23 @@
       <field name="model" search="[('model', '=', 'sale.amendment')]"/>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
+    <record model="ir.rule.group" id="rule_group_sale_amendment_companies">
+      <field name="name">User in companies</field>
+      <field name="model" search="[('model', '=', 'sale.amendment')]"/>
+      <field name="global_p" eval="True"/>
+    </record>
+    <record model="ir.rule" id="rule_sale_amendment_companies">
+      <field name="domain" eval="[('sale.company', 'in', Eval('companies', []))]" pyson="1"/>
+      <field name="rule_group" ref="rule_group_sale_amendment_companies"/>
+    </record>
     <record model="ir.model.button" id="sale_amendment_validation_amendment_button">
       <field name="name">validate_amendment</field>
       <field name="string">Validate</field>
       <field name="confirm">Are you sure you want to validate the amendments?</field>
       <field name="model" search="[('model', '=', 'sale.amendment')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_amendment_validation_amendment_button_group_sale_amendment">
```

### Comparing `trytond_sale_amendment-6.6.0/setup.py` & `trytond_sale_amendment-6.8.0/setup.py`

 * *Files 15% similar despite different names*

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
 name = 'trytond_sale_amendment'
 
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
     description='Tryton module to amend sales',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_amendment',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale amendment',
     package_dir={'trytond.modules.sale_amendment': '.'},
     packages=(
         ['trytond.modules.sale_amendment']
         + ['trytond.modules.sale_amendment.%s' % p for p in find_packages()]
         ),
@@ -124,27 +102,26 @@
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
     sale_amendment = trytond.modules.sale_amendment
     """,
     )
```

### Comparing `trytond_sale_amendment-6.6.0/tests/scenario_sale_amendment.rst` & `trytond_sale_amendment-6.8.0/tests/scenario_sale_amendment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/PKG-INFO` & `trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-amendment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to amend sales
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_amendment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale amendment
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
 
 Sale Amendment Module
 #####################
 
 The sale amendment module allows you to change sales that are being processed
```

### Comparing `trytond_sale_amendment-6.6.0/trytond_sale_amendment.egg-info/SOURCES.txt` & `trytond_sale_amendment-6.8.0/trytond_sale_amendment.egg-info/SOURCES.txt`

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
 exceptions.py
@@ -50,14 +46,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/sale_amendment_form.xml
 ./view/sale_amendment_line_form.xml
 ./view/sale_amendment_line_list.xml
 ./view/sale_amendment_list.xml
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

### Comparing `trytond_sale_amendment-6.6.0/view/sale_amendment_form.xml` & `trytond_sale_amendment-6.8.0/view/sale_amendment_form.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond_sale_amendment-6.6.0/view/sale_amendment_form.xml` & `trytond_sale_amendment-6.8.0/view/sale_amendment_form.xml`

```diff
@@ -1,16 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
   <label name="sale"/>
-  <field name="sale" colspan="3"/>
+  <field name="sale"/>
   <label name="date"/>
   <field name="date"/>
-  <newline/>
   <label name="description"/>
   <field name="description" colspan="3"/>
   <field name="lines" colspan="4"/>
   <group col="2" colspan="2" id="states">
     <label name="state"/>
     <field name="state"/>
   </group>
```

### Comparing `trytond_sale_amendment-6.6.0/view/sale_amendment_line_form.xml` & `trytond_sale_amendment-6.8.0/view/sale_amendment_line_form.xml`

 * *Files identical despite different names*

