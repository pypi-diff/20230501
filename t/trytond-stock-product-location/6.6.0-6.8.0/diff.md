# Comparing `tmp/trytond_stock_product_location-6.6.0.tar.gz` & `tmp/trytond_stock_product_location-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_product_location-6.6.0.tar", last modified: Mon Oct 31 16:28:00 2022, max compression
+gzip compressed data, was "trytond_stock_product_location-6.8.0.tar", last modified: Mon May  1 11:55:45 2023, max compression
```

## Comparing `trytond_stock_product_location-6.6.0.tar` & `trytond_stock_product_location-6.8.0.tar`

### file list

```diff
@@ -1,68 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:00.512010 trytond_stock_product_location-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_stock_product_location-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_product_location-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-31 16:27:59.000000 trytond_stock_product_location-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_product_location-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2341 2022-10-31 16:27:58.000000 trytond_stock_product_location-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 16:27:58.000000 trytond_stock_product_location-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:20.000000 trytond_stock_product_location-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_product_location-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2586 2022-10-31 16:28:00.512010 trytond_stock_product_location-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2018-08-18 09:55:20.000000 trytond_stock_product_location-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      624 2021-12-11 16:59:34.000000 trytond_stock_product_location-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:00.508676 trytond_stock_product_location-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2018-08-18 09:55:20.000000 trytond_stock_product_location-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:00.508676 trytond_stock_product_location-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      729 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      690 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      712 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      676 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      704 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      713 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      713 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      837 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      713 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2022-10-29 07:50:41.000000 trytond_stock_product_location-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3195 2022-10-11 19:49:59.000000 trytond_stock_product_location-6.6.0/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2018-08-18 09:55:20.000000 trytond_stock_product_location-6.6.0/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2902 2022-04-10 15:40:36.000000 trytond_stock_product_location-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2020-05-26 07:40:44.000000 trytond_stock_product_location-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      876 2020-03-01 11:49:50.000000 trytond_stock_product_location-6.6.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:28:00.512010 trytond_stock_product_location-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5327 2022-10-29 07:39:12.000000 trytond_stock_product_location-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:00.508676 trytond_stock_product_location-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_product_location-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1966 2020-07-09 09:37:33.000000 trytond_stock_product_location-6.6.0/tests/scenario_product_copy_locations.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3722 2020-07-09 09:37:33.000000 trytond_stock_product_location-6.6.0/tests/scenario_stock_product_location.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4496 2021-11-23 13:40:57.000000 trytond_stock_product_location-6.6.0/tests/scenario_stock_product_location_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3730 2020-07-09 09:37:33.000000 trytond_stock_product_location-6.6.0/tests/scenario_stock_product_location_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-04-16 16:30:57.000000 trytond_stock_product_location-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_product_location-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_stock_product_location-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      129 2022-10-31 16:27:57.000000 trytond_stock_product_location-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:00.512010 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2586 2022-10-31 16:27:59.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2056 2022-10-31 16:28:00.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:27:59.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 16:27:59.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2022-10-31 16:27:59.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:27:59.000000 trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:00.508676 trytond_stock_product_location-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2018-08-18 09:55:20.000000 trytond_stock_product_location-6.6.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2020-05-26 07:40:44.000000 trytond_stock_product_location-6.6.0/view/product_location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2020-05-26 07:40:44.000000 trytond_stock_product_location-6.6.0/view/product_location_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:45.569621 trytond_stock_product_location-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2504 2023-05-01 11:10:36.000000 trytond_stock_product_location-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:10:36.000000 trytond_stock_product_location-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_product_location-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2571 2023-05-01 11:55:45.569621 trytond_stock_product_location-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-01-16 14:00:21.000000 trytond_stock_product_location-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      624 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:45.569621 trytond_stock_product_location-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-01-16 14:00:21.000000 trytond_stock_product_location-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:45.562954 trytond_stock_product_location-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      690 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      712 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      704 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      713 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      713 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      837 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      713 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2023-04-29 08:02:47.000000 trytond_stock_product_location-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3195 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-01-16 14:00:21.000000 trytond_stock_product_location-6.8.0/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2902 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:55:45.569621 trytond_stock_product_location-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4509 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:45.566287 trytond_stock_product_location-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1966 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/scenario_product_copy_locations.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3723 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/scenario_stock_product_location.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4519 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/scenario_stock_product_location_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3731 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/scenario_stock_product_location_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      129 2023-05-01 11:10:30.000000 trytond_stock_product_location-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:45.569621 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2571 2023-05-01 11:55:44.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2030 2023-05-01 11:55:45.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:55:44.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:55:44.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      139 2023-05-01 11:55:44.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:55:44.000000 trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:55:45.566287 trytond_stock_product_location-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-01-16 14:00:21.000000 trytond_stock_product_location-6.8.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/view/product_location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_product_location-6.8.0/view/product_location_tree.xml
```

### Comparing `trytond_stock_product_location-6.6.0/CHANGELOG` & `trytond_stock_product_location-6.8.0/CHANGELOG`

 * *Files 16% similar despite different names*

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

### Comparing `trytond_stock_product_location-6.6.0/COPYRIGHT` & `trytond_stock_product_location-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2012 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_product_location-6.6.0/LICENSE` & `trytond_stock_product_location-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/PKG-INFO` & `trytond_stock_product_location-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_product_location
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add default location on product
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_product_location
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock product location
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
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
 
 Stock Product Location Module
 #############################
 
 The Stock Product Location Module adds on the product form a list of
```

### Comparing `trytond_stock_product_location-6.6.0/__init__.py` & `trytond_stock_product_location-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/bg.po` & `trytond_stock_product_location-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/ca.po` & `trytond_stock_product_location-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/cs.po` & `trytond_stock_product_location-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/de.po` & `trytond_stock_product_location-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/es.po` & `trytond_stock_product_location-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/es_419.po` & `trytond_stock_product_location-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/et.po` & `trytond_stock_product_location-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/fa.po` & `trytond_stock_product_location-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/fi.po` & `trytond_stock_product_location-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/fr.po` & `trytond_stock_product_location-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/hu.po` & `trytond_stock_product_location-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/id.po` & `trytond_stock_product_location-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/it.po` & `trytond_stock_product_location-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/lo.po` & `trytond_stock_product_location-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/lt.po` & `trytond_stock_product_location-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/nl.po` & `trytond_stock_product_location-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/pl.po` & `trytond_stock_product_location-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/pt.po` & `trytond_stock_product_location-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/ro.po` & `trytond_stock_product_location-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/ru.po` & `trytond_stock_product_location-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/sl.po` & `trytond_stock_product_location-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/tr.po` & `trytond_stock_product_location-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/uk.po` & `trytond_stock_product_location-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/locale/zh_CN.po` & `trytond_stock_product_location-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/location.py` & `trytond_stock_product_location-6.8.0/location.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/location.xml` & `trytond_stock_product_location-6.8.0/location.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/product.py` & `trytond_stock_product_location-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/setup.py` & `trytond_stock_product_location-6.8.0/setup.py`

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
@@ -34,62 +31,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_product_location'
 
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
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 for dep in ['production']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add default location on product',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_product_location',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock product location',
     package_dir={'trytond.modules.stock_product_location': '.'},
     packages=(
         ['trytond.modules.stock_product_location']
         + ['trytond.modules.stock_product_location.%s' % p
             for p in find_packages()]
@@ -127,27 +105,26 @@
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
     stock_product_location = trytond.modules.stock_product_location
     """,
     )
```

### Comparing `trytond_stock_product_location-6.6.0/tests/scenario_product_copy_locations.rst` & `trytond_stock_product_location-6.8.0/tests/scenario_product_copy_locations.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_product_location-6.6.0/tests/scenario_stock_product_location.rst` & `trytond_stock_product_location-6.8.0/tests/scenario_stock_product_location.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ================================
 Stock Product Locations Scenario
 ================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_product_location')
 
 Create company::
```

### Comparing `trytond_stock_product_location-6.6.0/tests/scenario_stock_product_location_production.rst` & `trytond_stock_product_location-6.8.0/tests/scenario_stock_product_location_production.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ===========================================
 Stock Product Locations Production Scenario
 ===========================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
 
+    >>> today = dt.date.today()
+
 Activate modules::
 
     >>> _ = activate_modules(['stock_product_location', 'production'])
 
 Create company::
 
     >>> _ = create_company()
@@ -116,15 +118,15 @@
     >>> inventory.state
     'done'
 
 Make a production::
 
     >>> Production = Model.get('production')
     >>> production = Production()
-    >>> production.planned_date = datetime.date.today()
+    >>> production.planned_date = today
     >>> production.product = product
     >>> production.bom = bom
     >>> production.quantity = 2
 
 Test storage location of the warehouse::
 
     >> warehouse_loc.storage_location == storage_loc
```

### Comparing `trytond_stock_product_location-6.6.0/tests/scenario_stock_product_location_template.rst` & `trytond_stock_product_location-6.8.0/tests/scenario_stock_product_location_template.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 =========================================
 Stock Product Locations Template Scenario
 =========================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_product_location')
 
 Create company::
```

### Comparing `trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/PKG-INFO` & `trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-product-location
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add default location on product
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_product_location
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock product location
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
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
 
 Stock Product Location Module
 #############################
 
 The Stock Product Location Module adds on the product form a list of
```

### Comparing `trytond_stock_product_location-6.6.0/trytond_stock_product_location.egg-info/SOURCES.txt` & `trytond_stock_product_location-6.8.0/trytond_stock_product_location.egg-info/SOURCES.txt`

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
 location.py
@@ -53,14 +49,15 @@
 ./tests/scenario_stock_product_location_production.rst
 ./tests/scenario_stock_product_location_template.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/product_form.xml
 ./view/product_location_form.xml
 ./view/product_location_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

