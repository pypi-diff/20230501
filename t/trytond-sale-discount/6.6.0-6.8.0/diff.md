# Comparing `tmp/trytond_sale_discount-6.6.0.tar.gz` & `tmp/trytond_sale_discount-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_discount-6.6.0.tar", last modified: Mon Oct 31 16:11:26 2022, max compression
+gzip compressed data, was "trytond_sale_discount-6.8.0.tar", last modified: Mon May  1 11:48:56 2023, max compression
```

## Comparing `trytond_sale_discount-6.6.0.tar` & `trytond_sale_discount-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:26.113797 trytond_sale_discount-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_discount-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_discount-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2022-10-31 16:11:24.000000 trytond_sale_discount-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_discount-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-10-31 16:11:24.000000 trytond_sale_discount-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:11:23.000000 trytond_sale_discount-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2020-10-12 14:22:10.000000 trytond_sale_discount-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_discount-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2529 2022-10-31 16:11:26.113797 trytond_sale_discount-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2020-10-12 14:22:10.000000 trytond_sale_discount-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2020-10-12 14:22:10.000000 trytond_sale_discount-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:26.110464 trytond_sale_discount-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2020-10-12 14:22:10.000000 trytond_sale_discount-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:26.110464 trytond_sale_discount-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      509 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      509 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      501 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-10-29 07:50:38.000000 trytond_sale_discount-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5787 2022-05-07 06:21:31.000000 trytond_sale_discount-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2020-10-12 14:22:10.000000 trytond_sale_discount-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:11:26.113797 trytond_sale_discount-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5279 2022-10-29 07:39:11.000000 trytond_sale_discount-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:26.110464 trytond_sale_discount-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_discount-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1921 2020-10-12 14:22:10.000000 trytond_sale_discount-6.6.0/tests/scenario_sale_discount.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2022-04-16 16:30:57.000000 trytond_sale_discount-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_discount-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      704 2022-10-31 15:10:09.000000 trytond_sale_discount-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2022-10-31 16:11:22.000000 trytond_sale_discount-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:26.113797 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2529 2022-10-31 16:11:25.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1507 2022-10-31 16:11:26.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:11:25.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2022-10-31 16:11:25.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-10-13 07:23:31.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       93 2022-10-31 16:11:25.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:11:25.000000 trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:26.110464 trytond_sale_discount-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2021-10-07 13:08:07.000000 trytond_sale_discount-6.6.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2022-04-08 16:23:26.000000 trytond_sale_discount-6.6.0/view/sale_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:56.501211 trytond_sale_discount-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-05-01 11:05:57.000000 trytond_sale_discount-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:05:57.000000 trytond_sale_discount-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2523 2023-05-01 11:48:56.501211 trytond_sale_discount-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:56.501211 trytond_sale_discount-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:56.497878 trytond_sale_discount-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      509 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      509 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-29 08:02:45.000000 trytond_sale_discount-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5787 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:48:56.501211 trytond_sale_discount-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4470 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:56.497878 trytond_sale_discount-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1921 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/tests/scenario_sale_discount.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:05:52.000000 trytond_sale_discount-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:56.501211 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2523 2023-05-01 11:48:55.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1481 2023-05-01 11:48:56.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:48:55.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-05-01 11:48:55.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       93 2023-05-01 11:48:55.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:48:55.000000 trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:56.501211 trytond_sale_discount-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-04-15 07:12:15.000000 trytond_sale_discount-6.8.0/view/sale_line_list.xml
```

### Comparing `trytond_sale_discount-6.6.0/COPYRIGHT` & `trytond_sale_discount-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2022 B2CK
-Copyright (C) 2020-2022 Cédric Krier
+Copyright (C) 2020-2023 B2CK
+Copyright (C) 2020-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_discount-6.6.0/LICENSE` & `trytond_sale_discount-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_discount-6.6.0/PKG-INFO` & `trytond_sale_discount-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_discount
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module that manages discount on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_discount
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale discount
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
 
 Sale Discount Module
 ####################
 
 The sale_discount module adds discount on sale line.
```

### Comparing `trytond_sale_discount-6.6.0/sale.py` & `trytond_sale_discount-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_discount-6.6.0/sale.xml` & `trytond_sale_discount-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_discount-6.6.0/setup.py` & `trytond_sale_discount-6.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     if slice:
         content = '\n'.join(content.splitlines()[slice])
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
@@ -37,60 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_discount'
 
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
     description='Tryton module that manages discount on sale',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_discount',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale discount',
     package_dir={'trytond.modules.sale_discount': '.'},
     packages=(
         ['trytond.modules.sale_discount']
         + ['trytond.modules.sale_discount.%s' % p
             for p in find_packages()]
@@ -128,27 +106,26 @@
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
     sale_discount = trytond.modules.sale_discount
     """,  # noqa: E501
     )
```

### Comparing `trytond_sale_discount-6.6.0/tests/scenario_sale_discount.rst` & `trytond_sale_discount-6.8.0/tests/scenario_sale_discount.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/PKG-INFO` & `trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-discount
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module that manages discount on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_discount
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale discount
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
 
 Sale Discount Module
 ####################
 
 The sale_discount module adds discount on sale line.
```

### Comparing `trytond_sale_discount-6.6.0/trytond_sale_discount.egg-info/SOURCES.txt` & `trytond_sale_discount-6.8.0/trytond_sale_discount.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

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
 sale.py
@@ -43,14 +39,15 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_discount.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/sale_line_form.xml
 ./view/sale_line_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_sale_discount-6.6.0/view/sale_line_form.xml` & `trytond_sale_discount-6.8.0/view/sale_line_form.xml`

 * *Files identical despite different names*

