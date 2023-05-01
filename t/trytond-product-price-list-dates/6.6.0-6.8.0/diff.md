# Comparing `tmp/trytond_product_price_list_dates-6.6.0.tar.gz` & `tmp/trytond_product_price_list_dates-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_price_list_dates-6.6.0.tar", last modified: Mon Oct 31 16:15:23 2022, max compression
+gzip compressed data, was "trytond_product_price_list_dates-6.8.0.tar", last modified: Mon May  1 11:48:18 2023, max compression
```

## Comparing `trytond_product_price_list_dates-6.6.0.tar` & `trytond_product_price_list_dates-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:23.283912 trytond_product_price_list_dates-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_product_price_list_dates-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_product_price_list_dates-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2022-10-31 16:15:21.000000 trytond_product_price_list_dates-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_product_price_list_dates-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1001 2022-10-31 16:15:21.000000 trytond_product_price_list_dates-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:15:20.000000 trytond_product_price_list_dates-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:47.000000 trytond_product_price_list_dates-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_product_price_list_dates-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2414 2022-10-31 16:15:23.283912 trytond_product_price_list_dates-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      172 2018-08-18 09:54:47.000000 trytond_product_price_list_dates-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      581 2021-12-11 16:59:33.000000 trytond_product_price_list_dates-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:23.280579 trytond_product_price_list_dates-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      172 2018-08-18 09:54:47.000000 trytond_product_price_list_dates-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:23.280579 trytond_product_price_list_dates-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      696 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      838 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      746 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      748 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      643 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:38.000000 trytond_product_price_list_dates-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2530 2022-06-21 08:14:03.000000 trytond_product_price_list_dates-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3729 2020-02-23 12:55:09.000000 trytond_product_price_list_dates-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      743 2022-04-08 16:23:26.000000 trytond_product_price_list_dates-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:15:23.283912 trytond_product_price_list_dates-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5273 2022-10-29 07:39:11.000000 trytond_product_price_list_dates-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:23.280579 trytond_product_price_list_dates-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_product_price_list_dates-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3275 2022-06-21 08:14:03.000000 trytond_product_price_list_dates-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2022-10-31 15:10:09.000000 trytond_product_price_list_dates-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      118 2022-10-31 16:15:19.000000 trytond_product_price_list_dates-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:23.283912 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2414 2022-10-31 16:15:22.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1804 2022-10-31 16:15:23.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:15:22.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2022-10-31 16:15:22.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:58.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2022-10-31 16:15:22.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:15:22.000000 trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:23.280579 trytond_product_price_list_dates-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2019-06-04 16:49:45.000000 trytond_product_price_list_dates-6.6.0/view/price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2018-08-18 09:54:47.000000 trytond_product_price_list_dates-6.6.0/view/price_list_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2019-10-11 23:09:48.000000 trytond_product_price_list_dates-6.6.0/view/price_list_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2018-08-18 09:54:47.000000 trytond_product_price_list_dates-6.6.0/view/price_list_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2018-08-18 09:54:47.000000 trytond_product_price_list_dates-6.6.0/view/price_list_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2020-02-23 12:55:09.000000 trytond_product_price_list_dates-6.6.0/view/product_sale_context_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:18.037400 trytond_product_price_list_dates-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1164 2023-05-01 11:05:32.000000 trytond_product_price_list_dates-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:05:32.000000 trytond_product_price_list_dates-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2397 2023-05-01 11:48:18.037400 trytond_product_price_list_dates-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2023-04-22 08:56:15.000000 trytond_product_price_list_dates-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-22 08:56:15.000000 trytond_product_price_list_dates-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:18.034067 trytond_product_price_list_dates-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      172 2023-04-22 08:56:15.000000 trytond_product_price_list_dates-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:18.030734 trytond_product_price_list_dates-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      696 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      838 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      746 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      748 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      643 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:45.000000 trytond_product_price_list_dates-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2530 2023-04-22 08:56:15.000000 trytond_product_price_list_dates-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3729 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      743 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:48:18.037400 trytond_product_price_list_dates-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4438 2023-04-22 08:56:15.000000 trytond_product_price_list_dates-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:18.030734 trytond_product_price_list_dates-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3275 2023-04-22 08:56:15.000000 trytond_product_price_list_dates-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      118 2023-05-01 11:05:27.000000 trytond_product_price_list_dates-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:18.037400 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2397 2023-05-01 11:48:17.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1778 2023-05-01 11:48:17.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:48:17.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2023-05-01 11:48:17.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2023-05-01 11:48:17.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:48:17.000000 trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:18.030734 trytond_product_price_list_dates-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:21.000000 trytond_product_price_list_dates-6.8.0/view/price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-6.8.0/view/price_list_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/view/price_list_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-6.8.0/view/price_list_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:20.000000 trytond_product_price_list_dates-6.8.0/view/price_list_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_product_price_list_dates-6.8.0/view/product_sale_context_form.xml
```

### Comparing `trytond_product_price_list_dates-6.6.0/CHANGELOG` & `trytond_product_price_list_dates-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_product_price_list_dates-6.6.0/COPYRIGHT` & `trytond_product_price_list_dates-6.8.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2022 Cédric Krier
-Copyright (C) 2017-2022 B2CK
+Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_price_list_dates-6.6.0/LICENSE` & `trytond_product_price_list_dates-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/PKG-INFO` & `trytond_product_price_list_dates-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list_dates
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add dates on price list
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_price_list_dates
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton price list
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
 
 Product Price List Dates Module
 ###############################
 
 The product_price_list_dates module adds *Start Date* and *End Date* conditions
```

### Comparing `trytond_product_price_list_dates-6.6.0/__init__.py` & `trytond_product_price_list_dates-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/bg.po` & `trytond_product_price_list_dates-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/ca.po` & `trytond_product_price_list_dates-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/cs.po` & `trytond_product_price_list_dates-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/de.po` & `trytond_product_price_list_dates-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/es.po` & `trytond_product_price_list_dates-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/es_419.po` & `trytond_product_price_list_dates-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/et.po` & `trytond_product_price_list_dates-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/fa.po` & `trytond_product_price_list_dates-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/fi.po` & `trytond_product_price_list_dates-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/fr.po` & `trytond_product_price_list_dates-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/hu.po` & `trytond_product_price_list_dates-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/id.po` & `trytond_product_price_list_dates-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/it.po` & `trytond_product_price_list_dates-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/lo.po` & `trytond_product_price_list_dates-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/lt.po` & `trytond_product_price_list_dates-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/nl.po` & `trytond_product_price_list_dates-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/pl.po` & `trytond_product_price_list_dates-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/pt.po` & `trytond_product_price_list_dates-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/ro.po` & `trytond_product_price_list_dates-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/ru.po` & `trytond_product_price_list_dates-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/sl.po` & `trytond_product_price_list_dates-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/tr.po` & `trytond_product_price_list_dates-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/uk.po` & `trytond_product_price_list_dates-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/locale/zh_CN.po` & `trytond_product_price_list_dates-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/product.py` & `trytond_product_price_list_dates-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/product.xml` & `trytond_product_price_list_dates-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/sale.py` & `trytond_product_price_list_dates-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/setup.py` & `trytond_product_price_list_dates-6.8.0/setup.py`

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
@@ -34,61 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_product_price_list_dates'
 
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
 
 tests_require = [get_require_version('trytond_sale_price_list')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add dates on price list',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/product_price_list_dates'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton price list',
     package_dir={'trytond.modules.product_price_list_dates': '.'},
     packages=(
         ['trytond.modules.product_price_list_dates']
         + ['trytond.modules.product_price_list_dates.%s' % p
             for p in find_packages()]
@@ -126,27 +103,26 @@
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
     product_price_list_dates = trytond.modules.product_price_list_dates
     """,
     )
```

### Comparing `trytond_product_price_list_dates-6.6.0/tests/test_module.py` & `trytond_product_price_list_dates-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/PKG-INFO` & `trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-product-price-list-dates
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add dates on price list
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_price_list_dates
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton price list
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
 
 Product Price List Dates Module
 ###############################
 
 The product_price_list_dates module adds *Start Date* and *End Date* conditions
```

### Comparing `trytond_product_price_list_dates-6.6.0/trytond_product_price_list_dates.egg-info/SOURCES.txt` & `trytond_product_price_list_dates-6.8.0/trytond_product_price_list_dates.egg-info/SOURCES.txt`

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
 product.py
@@ -47,14 +43,15 @@
 ./tests/test_module.py
 ./view/price_list_form.xml
 ./view/price_list_line_context_form.xml
 ./view/price_list_line_form.xml
 ./view/price_list_line_tree.xml
 ./view/price_list_line_tree_sequence.xml
 ./view/product_sale_context_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

