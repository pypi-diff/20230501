# Comparing `tmp/trytond_sale_blanket_agreement-6.6.0.tar.gz` & `tmp/trytond_sale_blanket_agreement-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_blanket_agreement-6.6.0.tar", last modified: Mon Oct 31 16:10:44 2022, max compression
+gzip compressed data, was "trytond_sale_blanket_agreement-6.8.0.tar", last modified: Mon May  1 11:49:24 2023, max compression
```

## Comparing `trytond_sale_blanket_agreement-6.6.0.tar` & `trytond_sale_blanket_agreement-6.8.0.tar`

### file list

```diff
@@ -1,74 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:44.306522 trytond_sale_blanket_agreement-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)       47 2022-10-31 16:10:42.000000 trytond_sale_blanket_agreement-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 16:10:42.000000 trytond_sale_blanket_agreement-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      794 2022-10-31 16:10:41.000000 trytond_sale_blanket_agreement-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_blanket_agreement-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2022-10-31 16:10:44.306522 trytond_sale_blanket_agreement-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:44.303189 trytond_sale_blanket_agreement-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1592 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2022-10-27 11:24:44.000000 trytond_sale_blanket_agreement-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_sale_blanket_agreement-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:44.303189 trytond_sale_blanket_agreement-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7069 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7164 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7145 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7108 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6047 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7216 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6015 2022-10-29 07:50:38.000000 trytond_sale_blanket_agreement-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      929 2022-10-21 22:41:05.000000 trytond_sale_blanket_agreement-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28598 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11626 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:10:44.306522 trytond_sale_blanket_agreement-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5506 2022-10-29 07:39:11.000000 trytond_sale_blanket_agreement-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:44.303189 trytond_sale_blanket_agreement-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5428 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/tests/scenario_sale_blanket_agreement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_sale_blanket_agreement-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2022-10-31 16:10:40.000000 trytond_sale_blanket_agreement-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:44.306522 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2022-10-31 16:10:43.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2294 2022-10-31 16:10:44.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:10:43.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 16:10:43.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:10:43.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2022-10-31 16:10:43.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:10:43.000000 trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:10:44.303189 trytond_sale_blanket_agreement-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/product_list_agreement_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_create_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1592 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2022-10-11 19:49:59.000000 trytond_sale_blanket_agreement-6.6.0/view/sale_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:24.134887 trytond_sale_blanket_agreement-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-05-01 11:06:16.000000 trytond_sale_blanket_agreement-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-05-01 11:06:16.000000 trytond_sale_blanket_agreement-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2023-05-01 11:49:24.134887 trytond_sale_blanket_agreement-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:24.131554 trytond_sale_blanket_agreement-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:24.124887 trytond_sale_blanket_agreement-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7069 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7164 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7145 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7108 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6047 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7216 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6015 2023-04-29 08:02:45.000000 trytond_sale_blanket_agreement-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      929 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    28587 2023-04-21 08:36:08.000000 trytond_sale_blanket_agreement-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11626 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:49:24.134887 trytond_sale_blanket_agreement-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4679 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:24.128220 trytond_sale_blanket_agreement-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5317 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/tests/scenario_sale_blanket_agreement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      705 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-05-01 11:06:11.000000 trytond_sale_blanket_agreement-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:24.134887 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2357 2023-05-01 11:49:23.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2023-05-01 11:49:24.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:49:23.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:49:23.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-05-01 11:49:23.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:49:23.000000 trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:49:24.131554 trytond_sale_blanket_agreement-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/product_list_agreement_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_create_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1592 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_blanket_agreement-6.8.0/view/sale_line_list.xml
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/COPYRIGHT` & `trytond_sale_blanket_agreement-6.8.0/COPYRIGHT`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Copyright (C) 2021 Hashbang
 Copyright (C) 2021 Maxime Richez
 Copyright (C) 2021 SALUC SA
 Copyright (C) 2021 Thierry Bruyere
-Copyright (C) 2022 B2CK
-Copyright (C) 2022 Cédric Krier
+Copyright (C) 2022-2023 B2CK
+Copyright (C) 2022-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/LICENSE` & `trytond_sale_blanket_agreement-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/PKG-INFO` & `trytond_sale_blanket_agreement-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_blanket_agreement
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale blanket agreement
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-blanket-agreement
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_blanket_agreement
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton,blanket agreement,sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,19 +38,19 @@
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
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 doc/index.rst
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/__init__.py` & `trytond_sale_blanket_agreement-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/doc/conf.py` & `trytond_sale_blanket_agreement-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_blanket_agreement-6.6.0/doc/design.rst` & `trytond_sale_blanket_agreement-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/bg.po` & `trytond_sale_blanket_agreement-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/ca.po` & `trytond_sale_blanket_agreement-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/cs.po` & `trytond_sale_blanket_agreement-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/de.po` & `trytond_sale_blanket_agreement-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/es.po` & `trytond_sale_blanket_agreement-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/es_419.po` & `trytond_sale_blanket_agreement-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/et.po` & `trytond_sale_blanket_agreement-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/fa.po` & `trytond_sale_blanket_agreement-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/fi.po` & `trytond_sale_blanket_agreement-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/fr.po` & `trytond_sale_blanket_agreement-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/hu.po` & `trytond_sale_blanket_agreement-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/id.po` & `trytond_sale_blanket_agreement-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/it.po` & `trytond_sale_blanket_agreement-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/lo.po` & `trytond_sale_blanket_agreement-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/lt.po` & `trytond_sale_blanket_agreement-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/nl.po` & `trytond_sale_blanket_agreement-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/pl.po` & `trytond_sale_blanket_agreement-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/pt.po` & `trytond_sale_blanket_agreement-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/ro.po` & `trytond_sale_blanket_agreement-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/ru.po` & `trytond_sale_blanket_agreement-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/sl.po` & `trytond_sale_blanket_agreement-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/tr.po` & `trytond_sale_blanket_agreement-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/uk.po` & `trytond_sale_blanket_agreement-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/locale/zh_CN.po` & `trytond_sale_blanket_agreement-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/message.xml` & `trytond_sale_blanket_agreement-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/product.xml` & `trytond_sale_blanket_agreement-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/sale.py` & `trytond_sale_blanket_agreement-6.8.0/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,16 +501,15 @@
 
     @classmethod
     def _unit_categories(cls):
         return ['product_uom_category']
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @fields.depends(
         'quantity', 'unit_price', 'blanket_agreement',
         '_parent_blanket_agreement.currency')
     def on_change_with_amount(self, name=None):
         amount = (
             Decimal(str(self.quantity or '0.0'))
@@ -518,16 +517,16 @@
 
         if self.blanket_agreement and self.blanket_agreement.currency:
             return self.blanket_agreement.currency.round(amount)
         return amount
 
     @fields.depends('blanket_agreement', '_parent_blanket_agreement.currency')
     def on_change_with_currency(self, name=None):
-        if self.blanket_agreement and self.blanket_agreement.currency:
-            return self.blanket_agreement.currency.id
+        if self.blanket_agreement:
+            return self.blanket_agreement.currency
 
     def get_processed_quantity(self, name=None):
         processed_quantity = 0.
         for line in self.sale_lines:
             if line.sale.state in {'confirmed', 'processing', 'done'}:
                 processed_quantity += line.quantity_for_blanket_agreement(
                     self, round=False)
@@ -547,16 +546,16 @@
     @fields.depends('blanket_agreement', '_parent_blanket_agreement.state')
     def on_change_with_agreement_state(self, name=None):
         if self.blanket_agreement:
             return self.blanket_agreement.state
 
     @fields.depends('blanket_agreement', '_parent_blanket_agreement.company')
     def on_change_with_company(self, name=None):
-        if self.blanket_agreement and self.blanket_agreement.company:
-            return self.blanket_agreement.company.id
+        if self.blanket_agreement:
+            return self.blanket_agreement.company
 
     def get_sale_line(self, sale):
         pool = Pool()
         SaleLine = pool.get('sale.line')
         sale_line = SaleLine(
             sale=sale,
             product=self.product,
@@ -728,22 +727,23 @@
                     remaining_quantity = Uom.compute_qty(
                         line.unit, line.remaining_quantity, self.unit)
                     if (self.quantity is None
                             or remaining_quantity < self.quantity):
                         self.quantity = remaining_quantity
                         self.on_change_quantity()
 
-    @fields.depends(
-        'blanket_agreement_line', 'product',
-        '_parent_blanket_agreement_line.product')
+    @fields.depends(methods=['is_valid_product_for_blanket_agreement'])
     def on_change_product(self):
         super().on_change_product()
         if not self.is_valid_product_for_blanket_agreement():
             self.blanket_agreement_line = None
 
+    @fields.depends(
+        'blanket_agreement_line', 'product',
+        '_parent_blanket_agreement_line.product')
     def is_valid_product_for_blanket_agreement(self):
         if self.blanket_agreement_line:
             return self.product == self.blanket_agreement_line.product
 
     def quantity_for_blanket_agreement(self, line, round=True):
         pool = Pool()
         Uom = pool.get('product.uom')
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/sale.xml` & `trytond_sale_blanket_agreement-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/setup.py` & `trytond_sale_blanket_agreement-6.8.0/setup.py`

 * *Files 4% similar despite different names*

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
@@ -37,64 +34,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_blanket_agreement'
 
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
 
 tests_require = [
     get_require_version('proteus'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module for sale blanket agreement',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
             'https://docs.tryton.org/projects/modules-sale-blanket-agreement',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/sale_blanket_agreement',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton, blanket agreement, sale',
     package_dir={'trytond.modules.sale_blanket_agreement': '.'},
     packages=(
         ['trytond.modules.sale_blanket_agreement']
         + ['trytond.modules.sale_blanket_agreement.%s' % p
             for p in find_packages()]
@@ -132,28 +109,27 @@
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
         'Programming Language :: Python :: Implementation :: PyPy',
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
     sale_blanket_agreement = trytond.modules.sale_blanket_agreement
     """,  # noqa: E501
     )
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/tests/scenario_sale_blanket_agreement.rst` & `trytond_sale_blanket_agreement-6.8.0/tests/scenario_sale_blanket_agreement.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 ===============================
 Sale Blanket Agreement Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts)
 
-    >>> today = datetime.date.today()
-    >>> later = today + relativedelta(days=30)
-
+    >>> today = dt.date.today()
+    >>> later = today + dt.timedelta(days=30)
 
 Activate modules::
 
     >>> config = activate_modules('sale_blanket_agreement')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
@@ -94,17 +92,15 @@
     >>> blanket_agreement_line.unit_price = Decimal('9.0000')
     >>> blanket_agreement.click('run')
     >>> blanket_agreement.state
     'running'
 
 Create sale from blanket agreement::
 
-    >>> create_sale = Wizard(
-    ...     'sale.blanket_agreement.create_sale',
-    ...     [blanket_agreement])
+    >>> create_sale = blanket_agreement.click('create_sale')
     >>> len(create_sale.form.lines)
     1
     >>> create_sale.form.lines[0].remaining_quantity
     20.0
     >>> create_sale.execute('create_sale')
     >>> sale, = create_sale.actions[0]
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/tests/test_scenario.py` & `trytond_sale_blanket_agreement-6.8.0/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/tox.ini` & `trytond_sale_blanket_agreement-6.8.0/tox.ini`

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
-    coverage run --include=./**/sale_blanket_agreement/* -m unittest discover -s tests
-    coverage report --include=./**/sale_blanket_agreement/* --omit=*/tests/*
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

### Comparing `trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO` & `trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-blanket-agreement
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale blanket agreement
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-blanket-agreement
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_blanket_agreement
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton,blanket agreement,sale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,19 +38,19 @@
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
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 doc/index.rst
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt` & `trytond_sale_blanket_agreement-6.8.0/trytond_sale_blanket_agreement.egg-info/SOURCES.txt`

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
```

### Comparing `trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_form.xml` & `trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_blanket_agreement-6.6.0/view/sale_blanket_agreement_line_form.xml` & `trytond_sale_blanket_agreement-6.8.0/view/sale_blanket_agreement_line_form.xml`

 * *Files identical despite different names*

