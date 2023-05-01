# Comparing `tmp/trytond_purchase_amendment-6.6.0.tar.gz` & `tmp/trytond_purchase_amendment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_amendment-6.6.0.tar", last modified: Mon Oct 31 16:15:51 2022, max compression
+gzip compressed data, was "trytond_purchase_amendment-6.8.0.tar", last modified: Mon May  1 11:51:40 2023, max compression
```

## Comparing `trytond_purchase_amendment-6.6.0.tar` & `trytond_purchase_amendment-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:51.677658 trytond_purchase_amendment-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_purchase_amendment-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_purchase_amendment-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-10-31 16:15:50.000000 trytond_purchase_amendment-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_purchase_amendment-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      641 2022-10-31 16:15:49.000000 trytond_purchase_amendment-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:15:49.000000 trytond_purchase_amendment-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_purchase_amendment-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2997 2022-10-31 16:15:51.677658 trytond_purchase_amendment-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      767 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2021-12-11 16:59:33.000000 trytond_purchase_amendment-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:51.674325 trytond_purchase_amendment-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      767 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:51.674325 trytond_purchase_amendment-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4324 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4358 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4351 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4364 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3850 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4058 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4334 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3759 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3710 2022-10-29 07:50:39.000000 trytond_purchase_amendment-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14793 2022-10-11 19:49:58.000000 trytond_purchase_amendment-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5495 2021-03-24 12:34:22.000000 trytond_purchase_amendment-6.6.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:15:51.677658 trytond_purchase_amendment-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5194 2022-10-29 07:39:11.000000 trytond_purchase_amendment-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:51.674325 trytond_purchase_amendment-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_purchase_amendment-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4620 2021-02-02 12:22:17.000000 trytond_purchase_amendment-6.6.0/tests/scenario_purchase_amendment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2022-04-16 16:30:57.000000 trytond_purchase_amendment-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_purchase_amendment-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-10-31 15:10:09.000000 trytond_purchase_amendment-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 16:15:48.000000 trytond_purchase_amendment-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:51.677658 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2997 2022-10-31 16:15:51.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1864 2022-10-31 16:15:51.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:15:51.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 16:15:51.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-11-04 12:05:11.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2022-10-31 16:15:51.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:15:51.000000 trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:51.674325 trytond_purchase_amendment-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/view/purchase_amendment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1228 2022-10-11 19:45:05.000000 trytond_purchase_amendment-6.6.0/view/purchase_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/view/purchase_amendment_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2022-04-08 16:23:26.000000 trytond_purchase_amendment-6.6.0/view/purchase_amendment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2019-10-11 23:19:17.000000 trytond_purchase_amendment-6.6.0/view/purchase_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:40.059907 trytond_purchase_amendment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      837 2023-05-01 11:07:47.000000 trytond_purchase_amendment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:07:47.000000 trytond_purchase_amendment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2986 2023-05-01 11:51:40.059907 trytond_purchase_amendment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:40.056574 trytond_purchase_amendment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:40.053241 trytond_purchase_amendment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4457 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4493 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4486 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4507 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3962 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4468 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3871 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-30 10:46:36.000000 trytond_purchase_amendment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14878 2023-04-21 08:36:08.000000 trytond_purchase_amendment-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6113 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:51:40.059907 trytond_purchase_amendment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4380 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:40.053241 trytond_purchase_amendment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4620 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/tests/scenario_purchase_amendment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 11:07:41.000000 trytond_purchase_amendment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:40.059907 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2986 2023-05-01 11:51:39.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1838 2023-05-01 11:51:39.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:51:39.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:51:39.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 11:51:39.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:51:39.000000 trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:40.056574 trytond_purchase_amendment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/view/purchase_amendment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1228 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/view/purchase_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/view/purchase_amendment_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/view/purchase_amendment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_purchase_amendment-6.8.0/view/purchase_form.xml
```

### Comparing `trytond_purchase_amendment-6.6.0/CHANGELOG` & `trytond_purchase_amendment-6.8.0/CHANGELOG`

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

### Comparing `trytond_purchase_amendment-6.6.0/COPYRIGHT` & `trytond_purchase_amendment-6.8.0/COPYRIGHT`

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

### Comparing `trytond_purchase_amendment-6.6.0/LICENSE` & `trytond_purchase_amendment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-6.6.0/PKG-INFO` & `trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_purchase_amendment
-Version: 6.6.0
+Name: trytond-purchase-amendment
+Version: 6.8.0
 Summary: Tryton module to amend purchases
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_amendment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase amendment
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
 
 Purchase Amendment Module
 #########################
 
 The purchase amendment module allows you to change purchases that are being
```

### Comparing `trytond_purchase_amendment-6.6.0/README.rst` & `trytond_purchase_amendment-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-6.6.0/doc/index.rst` & `trytond_purchase_amendment-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-6.6.0/locale/bg.po` & `trytond_purchase_amendment-6.8.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/ca.po` & `trytond_purchase_amendment-6.8.0/locale/es.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,176 +1,180 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:purchase.amendment,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "Fecha"
 
 msgctxt "field:purchase.amendment,description:"
 msgid "Description"
-msgstr "Descripció"
+msgstr "Descripción"
 
 msgctxt "field:purchase.amendment,lines:"
 msgid "Lines"
-msgstr "Línies"
+msgstr "Líneas"
 
 msgctxt "field:purchase.amendment,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
 msgctxt "field:purchase.amendment,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Estado"
 
 msgctxt "field:purchase.amendment.line,action:"
 msgid "Action"
-msgstr "Acció"
+msgstr "Acción"
 
 msgctxt "field:purchase.amendment.line,amendment:"
 msgid "Amendment"
-msgstr "Correcció"
+msgstr "Corrección"
 
 msgctxt "field:purchase.amendment.line,description:"
 msgid "Description"
-msgstr "Descripció"
+msgstr "Descripción"
 
 msgctxt "field:purchase.amendment.line,invoice_address:"
 msgid "Invoice Address"
-msgstr "Adreça de facturació"
+msgstr "Dirección de facturación"
 
 msgctxt "field:purchase.amendment.line,invoice_party:"
 msgid "Invoice Party"
-msgstr "Tercer de la factura"
+msgstr "Tercero de la factura"
 
 msgctxt "field:purchase.amendment.line,line:"
 msgid "Line"
-msgstr "Línia"
+msgstr "Línea"
 
 msgctxt "field:purchase.amendment.line,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Tercero"
 
 msgctxt "field:purchase.amendment.line,payment_term:"
 msgid "Payment Term"
-msgstr "Termini de pagament"
+msgstr "Plazo de pago"
 
 msgctxt "field:purchase.amendment.line,product:"
 msgid "Product"
-msgstr "Producte"
+msgstr "Producto"
 
 msgctxt "field:purchase.amendment.line,product_supplier:"
 msgid "Supplier's Product"
-msgstr "Producte proveïdor"
+msgstr "Producto proveedor"
 
 msgctxt "field:purchase.amendment.line,product_uom_category:"
 msgid "Product UoM Category"
-msgstr "Categoria UdM del producte"
+msgstr "Categoría UdM del producto"
 
 msgctxt "field:purchase.amendment.line,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
 msgctxt "field:purchase.amendment.line,quantity:"
 msgid "Quantity"
-msgstr "Quantitat"
+msgstr "Cantidad"
 
 msgctxt "field:purchase.amendment.line,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "Estado"
 
 msgctxt "field:purchase.amendment.line,unit:"
 msgid "Unit"
-msgstr "Unitat"
+msgstr "Unidad"
 
 msgctxt "field:purchase.amendment.line,unit_price:"
 msgid "Unit Price"
-msgstr "Preu unitari"
+msgstr "Precio unitario"
 
 msgctxt "field:purchase.amendment.line,warehouse:"
 msgid "Warehouse"
-msgstr "Magatzem"
+msgstr "Almacén"
 
 msgctxt "field:purchase.purchase,amendments:"
 msgid "Amendments"
-msgstr "Correccions"
+msgstr "Correcciones"
 
 msgctxt "model:ir.action,name:act_purchase_amendment_form"
 msgid "Amendments"
-msgstr "Correccions"
+msgstr "Correcciones"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_amendment_form_domain_all"
 msgid "All"
-msgstr "Tot"
+msgstr "Todo"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_amendment_form_domain_draft"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Borrador"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_amendment_form_domain_validated"
 msgid "Validated"
 msgstr "Validada"
 
 msgctxt "model:ir.message,text:msg_one_purchase_at_time"
 msgid ""
 "You cannot validate more than one amendment at the same time for purchase "
 "\"%(purchase)s\"."
 msgstr ""
-"No es pot validar a la vegada més d'una correcció de la mateixa compra "
+"No puedes validar a la vez mas de una corrección de la misma compra "
 "\"%(compra)s\"."
 
 msgctxt ""
 "model:ir.model.button,confirm:purchase_amendment_validation_amendment_button"
 msgid "Are you sure you want to validate the amendements?"
-msgstr "Esteu segurs que voleu validar les correccions?"
+msgstr "¿Estas seguro que quieres validar las correciones?"
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
-msgstr "Valida"
+msgstr "Validar"
+
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
-msgstr "Correccions"
+msgstr "Correcciones"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
-msgstr "Correcció de compra"
+msgstr "Correción de compra"
 
 msgctxt "model:purchase.amendment.line,name:"
 msgid "Purchase Amendment Line"
-msgstr "Línia de correcció de compra"
+msgstr "Línea de correción de compra"
 
 msgctxt "model:res.group,name:group_purchase_amendment"
 msgid "Purchase Amendment"
-msgstr "Correcció de compra"
+msgstr "Correción de compra"
 
 msgctxt "selection:purchase.amendment,state:"
 msgid "Draft"
-msgstr "Esborrany"
+msgstr "Borrador"
 
 msgctxt "selection:purchase.amendment,state:"
 msgid "Validated"
-msgstr "Validada"
+msgstr "Validado"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Line"
-msgstr "Canvia línia"
+msgstr "Modificar línea"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Parties and Addresses"
-msgstr "Canvia tercer i adreces"
+msgstr "Modificar terceros y direcciones"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Payment Term"
-msgstr "Canvia termini de pagament"
+msgstr "Modificar plazo de pago"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Warehouse"
-msgstr "Canvia magatzem"
+msgstr "Modificar almacén"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Recompute Taxes"
-msgstr "Recalcula impostos"
+msgstr "Recalcular impuestos"
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/cs.po` & `trytond_purchase_amendment-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/de.po` & `trytond_purchase_amendment-6.8.0/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,18 @@
 msgstr "Die Änderungen tatsächlich bestätigen?"
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Bestätigen"
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr "Benutzer im Unternehmen"
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr "Änderungen"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr "Einkauf Änderung"
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/es.po` & `trytond_purchase_amendment-6.8.0/locale/ca.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,176 +1,180 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:purchase.amendment,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Data"
 
 msgctxt "field:purchase.amendment,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Descripció"
 
 msgctxt "field:purchase.amendment,lines:"
 msgid "Lines"
-msgstr "Líneas"
+msgstr "Línies"
 
 msgctxt "field:purchase.amendment,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
 msgctxt "field:purchase.amendment,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Estat"
 
 msgctxt "field:purchase.amendment.line,action:"
 msgid "Action"
-msgstr "Acción"
+msgstr "Acció"
 
 msgctxt "field:purchase.amendment.line,amendment:"
 msgid "Amendment"
-msgstr "Corrección"
+msgstr "Correcció"
 
 msgctxt "field:purchase.amendment.line,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Descripció"
 
 msgctxt "field:purchase.amendment.line,invoice_address:"
 msgid "Invoice Address"
-msgstr "Dirección de facturación"
+msgstr "Adreça de facturació"
 
 msgctxt "field:purchase.amendment.line,invoice_party:"
 msgid "Invoice Party"
-msgstr "Tercero de la factura"
+msgstr "Tercer de la factura"
 
 msgctxt "field:purchase.amendment.line,line:"
 msgid "Line"
-msgstr "Línea"
+msgstr "Línia"
 
 msgctxt "field:purchase.amendment.line,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Tercer"
 
 msgctxt "field:purchase.amendment.line,payment_term:"
 msgid "Payment Term"
-msgstr "Plazo de pago"
+msgstr "Termini de pagament"
 
 msgctxt "field:purchase.amendment.line,product:"
 msgid "Product"
-msgstr "Producto"
+msgstr "Producte"
 
 msgctxt "field:purchase.amendment.line,product_supplier:"
 msgid "Supplier's Product"
-msgstr "Producto proveedor"
+msgstr "Producte proveïdor"
 
 msgctxt "field:purchase.amendment.line,product_uom_category:"
 msgid "Product UoM Category"
-msgstr "Categoría UdM del producto"
+msgstr "Categoria UdM del producte"
 
 msgctxt "field:purchase.amendment.line,purchase:"
 msgid "Purchase"
 msgstr "Compra"
 
 msgctxt "field:purchase.amendment.line,quantity:"
 msgid "Quantity"
-msgstr "Cantidad"
+msgstr "Quantitat"
 
 msgctxt "field:purchase.amendment.line,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Estat"
 
 msgctxt "field:purchase.amendment.line,unit:"
 msgid "Unit"
-msgstr "Unidad"
+msgstr "Unitat"
 
 msgctxt "field:purchase.amendment.line,unit_price:"
 msgid "Unit Price"
-msgstr "Precio unitario"
+msgstr "Preu unitari"
 
 msgctxt "field:purchase.amendment.line,warehouse:"
 msgid "Warehouse"
-msgstr "Almacén"
+msgstr "Magatzem"
 
 msgctxt "field:purchase.purchase,amendments:"
 msgid "Amendments"
-msgstr "Correcciones"
+msgstr "Correccions"
 
 msgctxt "model:ir.action,name:act_purchase_amendment_form"
 msgid "Amendments"
-msgstr "Correcciones"
+msgstr "Correccions"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_amendment_form_domain_all"
 msgid "All"
-msgstr "Todo"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_amendment_form_domain_draft"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Esborrany"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_amendment_form_domain_validated"
 msgid "Validated"
 msgstr "Validada"
 
 msgctxt "model:ir.message,text:msg_one_purchase_at_time"
 msgid ""
 "You cannot validate more than one amendment at the same time for purchase "
 "\"%(purchase)s\"."
 msgstr ""
-"No puedes validar a la vez mas de una corrección de la misma compra "
+"No es pot validar a la vegada més d'una correcció de la mateixa compra "
 "\"%(compra)s\"."
 
 msgctxt ""
 "model:ir.model.button,confirm:purchase_amendment_validation_amendment_button"
 msgid "Are you sure you want to validate the amendements?"
-msgstr "¿Estas seguro que quieres validar las correciones?"
+msgstr "Esteu segurs que voleu validar les correccions?"
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
-msgstr "Validar"
+msgstr "Valida"
+
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr "Usuari a les empreses"
 
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
-msgstr "Correcciones"
+msgstr "Correccions"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
-msgstr "Correción de compra"
+msgstr "Correcció de compra"
 
 msgctxt "model:purchase.amendment.line,name:"
 msgid "Purchase Amendment Line"
-msgstr "Línea de correción de compra"
+msgstr "Línia de correcció de compra"
 
 msgctxt "model:res.group,name:group_purchase_amendment"
 msgid "Purchase Amendment"
-msgstr "Correción de compra"
+msgstr "Correcció de compra"
 
 msgctxt "selection:purchase.amendment,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "Esborrany"
 
 msgctxt "selection:purchase.amendment,state:"
 msgid "Validated"
-msgstr "Validado"
+msgstr "Validada"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Line"
-msgstr "Modificar línea"
+msgstr "Canvia línia"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Parties and Addresses"
-msgstr "Modificar terceros y direcciones"
+msgstr "Canvia tercer i adreces"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Payment Term"
-msgstr "Modificar plazo de pago"
+msgstr "Canvia termini de pagament"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Change Warehouse"
-msgstr "Modificar almacén"
+msgstr "Canvia magatzem"
 
 msgctxt "selection:purchase.amendment.line,action:"
 msgid "Recompute Taxes"
-msgstr "Recalcular impuestos"
+msgstr "Recalcula impostos"
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/es_419.po` & `trytond_purchase_amendment-6.8.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/et.po` & `trytond_purchase_amendment-6.8.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/fa.po` & `trytond_purchase_amendment-6.8.0/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/fi.po` & `trytond_purchase_amendment-6.8.0/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/fr.po` & `trytond_purchase_amendment-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,18 @@
 msgstr "Êtes-vous sûr de vouloir valider les amendements ?"
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "Valider"
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr "Utilisateur dans les sociétés"
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr "Amendements"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr "Amendement d'achat"
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/hu.po` & `trytond_purchase_amendment-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/id.po` & `trytond_purchase_amendment-6.8.0/locale/id.po`

 * *Files 7% similar despite different names*

```diff
@@ -126,14 +126,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/it.po` & `trytond_purchase_amendment-6.8.0/locale/it.po`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr "Correzioni"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/lo.po` & `trytond_purchase_amendment-6.8.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/lt.po` & `trytond_purchase_amendment-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/nl.po` & `trytond_purchase_amendment-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,18 @@
 msgstr "Weet u zeker dat u de wijzigingen wilt valideren?"
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr "bevestigen"
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr "Gebruiker in bedrijven"
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr "wijzigingen"
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr "Aankoopwijziging"
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/pl.po` & `trytond_purchase_amendment-6.8.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/pt.po` & `trytond_purchase_amendment-6.8.0/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/ro.po` & `trytond_purchase_amendment-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/ru.po` & `trytond_purchase_amendment-6.8.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/sl.po` & `trytond_purchase_amendment-6.8.0/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/tr.po` & `trytond_purchase_amendment-6.8.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/uk.po` & `trytond_purchase_amendment-6.8.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/locale/zh_CN.po` & `trytond_purchase_amendment-6.8.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,18 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_amendment_validation_amendment_button"
 msgid "Validate"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_purchase_amendment_companies"
+msgid "User in companies"
+msgstr ""
+
 msgctxt "model:ir.ui.menu,name:menu_purchase_amendment"
 msgid "Amendments"
 msgstr ""
 
 msgctxt "model:purchase.amendment,name:"
 msgid "Purchase Amendment"
 msgstr ""
```

### Comparing `trytond_purchase_amendment-6.6.0/purchase.py` & `trytond_purchase_amendment-6.8.0/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     state = fields.Selection([
             ('draft', "Draft"),
             ('validated', "Validated"),
             ], "State", readonly=True, required=True, sort=False)
     lines = fields.One2Many(
         'purchase.amendment.line', 'amendment', "Lines",
         states={
-            'readonly': Eval('state') != 'draft',
+            'readonly': (
+                (Eval('state') != 'draft')
+                | ~Eval('purchase')),
             })
 
     @classmethod
     def __setup__(cls):
         super(Amendment, cls).__setup__()
         t = cls.__table__()
         cls._sql_indexes.add(
@@ -192,15 +194,15 @@
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
@@ -239,15 +241,16 @@
             'invisible': Eval('action') != 'warehouse',
             'required': Eval('action') == 'warehouse',
             })
 
     product = fields.Many2One(
         'product.product', "Product",
         domain=[
-            If(Eval('state') == 'draft',
+            If((Eval('state') == 'draft')
+                & ~(Eval('quantity', 0) < 0),
                 ('purchasable', '=', True),
                 ()),
             If(Eval('product_uom_category'),
                 ('default_uom_category', '=', Eval('product_uom_category')),
                 ()),
             ],
         states={
@@ -353,16 +356,15 @@
         self.on_change_line()
         self.on_change_amendment()
 
     @fields.depends(
         'amendment',
         '_parent_amendment.purchase')
     def on_change_with_purchase(self, name=None):
-        if self.amendment and self.amendment.purchase:
-            return self.amendment.purchase.id
+        return self.amendment.purchase if self.amendment else None
 
     @fields.depends('line')
     def on_change_line(self):
         if self.line:
             self.product = self.line.product
             self.product_supplier = self.line.product_supplier
             self.quantity = self.line.quantity
@@ -389,17 +391,17 @@
         elif self.party:
             self.invoice_address = self.party.address_get(type='invoice')
 
     @fields.depends('line')
     def on_change_with_product_uom_category(self, name=None):
         if self.line:
             if self.line.product_uom_category:
-                return self.line.product_uom_category.id
+                return self.line.product_uom_category
             elif self.line.unit:
-                return self.line.unit.category.id
+                return self.line.unit.category
 
     def apply(self, purchase):
         assert self.purchase == purchase
         purchase_line = None
         if self.line:
             for line in purchase.lines:
                 if self.line == line:
```

### Comparing `trytond_purchase_amendment-6.6.0/purchase.xml` & `trytond_purchase_amendment-6.8.0/purchase.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_purchase_amendment-6.6.0/purchase.xml` & `trytond_purchase_amendment-6.8.0/purchase.xml`

```diff
@@ -70,14 +70,23 @@
       <field name="model" search="[('model', '=', 'purchase.amendment')]"/>
       <field name="group" ref="purchase.group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
+    <record model="ir.rule.group" id="rule_group_purchase_amendment_companies">
+      <field name="name">User in companies</field>
+      <field name="model" search="[('model', '=', 'purchase.amendment')]"/>
+      <field name="global_p" eval="True"/>
+    </record>
+    <record model="ir.rule" id="rule_purchase_amendment_companies">
+      <field name="domain" eval="[('purchase.company', 'in', Eval('companies', []))]" pyson="1"/>
+      <field name="rule_group" ref="rule_group_purchase_amendment_companies"/>
+    </record>
     <record model="ir.model.button" id="purchase_amendment_validation_amendment_button">
       <field name="name">validate_amendment</field>
       <field name="string">Validate</field>
       <field name="confirm">Are you sure you want to validate the amendements?</field>
       <field name="model" search="[('model', '=', 'purchase.amendment')]"/>
     </record>
     <record model="ir.model.button-res.group" id="purchase_amendment_validation_amendment_button_group_purchase_amendment">
```

### Comparing `trytond_purchase_amendment-6.6.0/setup.py` & `trytond_purchase_amendment-6.8.0/setup.py`

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
 name = 'trytond_purchase_amendment'
 
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
     description='Tryton module to amend purchases',
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
-        "Source Code": 'https://hg.tryton.org/modules/purchase_amendment',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase amendment',
     package_dir={'trytond.modules.purchase_amendment': '.'},
     packages=(
         ['trytond.modules.purchase_amendment']
         + ['trytond.modules.purchase_amendment.%s' % p
             for p in find_packages()]
@@ -125,27 +103,26 @@
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
     purchase_amendment = trytond.modules.purchase_amendment
     """,
     )
```

### Comparing `trytond_purchase_amendment-6.6.0/tests/scenario_purchase_amendment.rst` & `trytond_purchase_amendment-6.8.0/tests/scenario_purchase_amendment.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/PKG-INFO` & `trytond_purchase_amendment-6.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-amendment
-Version: 6.6.0
+Name: trytond_purchase_amendment
+Version: 6.8.0
 Summary: Tryton module to amend purchases
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_amendment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase amendment
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
 
 Purchase Amendment Module
 #########################
 
 The purchase amendment module allows you to change purchases that are being
```

### Comparing `trytond_purchase_amendment-6.6.0/trytond_purchase_amendment.egg-info/SOURCES.txt` & `trytond_purchase_amendment-6.8.0/trytond_purchase_amendment.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
 ./view/purchase_amendment_form.xml
 ./view/purchase_amendment_line_form.xml
 ./view/purchase_amendment_line_list.xml
 ./view/purchase_amendment_list.xml
 ./view/purchase_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_purchase_amendment-6.6.0/view/purchase_amendment_form.xml` & `trytond_purchase_amendment-6.8.0/view/purchase_amendment_form.xml`

 * *Files 19% similar despite different names*

#### Comparing `trytond_purchase_amendment-6.6.0/view/purchase_amendment_form.xml` & `trytond_purchase_amendment-6.8.0/view/purchase_amendment_form.xml`

```diff
@@ -1,16 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
   <label name="purchase"/>
-  <field name="purchase" colspan="3"/>
+  <field name="purchase"/>
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

### Comparing `trytond_purchase_amendment-6.6.0/view/purchase_amendment_line_form.xml` & `trytond_purchase_amendment-6.8.0/view/purchase_amendment_line_form.xml`

 * *Files identical despite different names*

