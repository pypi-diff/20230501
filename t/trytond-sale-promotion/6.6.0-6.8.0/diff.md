# Comparing `tmp/trytond_sale_promotion-6.6.0.tar.gz` & `tmp/trytond_sale_promotion-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_promotion-6.6.0.tar", last modified: Mon Oct 31 16:18:02 2022, max compression
+gzip compressed data, was "trytond_sale_promotion-6.8.0.tar", last modified: Mon May  1 11:40:23 2023, max compression
```

## Comparing `trytond_sale_promotion-6.6.0.tar` & `trytond_sale_promotion-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:02.749564 trytond_sale_promotion-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_promotion-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_promotion-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2022-10-31 16:18:01.000000 trytond_sale_promotion-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_promotion-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1512 2022-10-31 16:18:00.000000 trytond_sale_promotion-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:18:00.000000 trytond_sale_promotion-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:40.000000 trytond_sale_promotion-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_promotion-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3222 2022-10-31 16:18:02.749564 trytond_sale_promotion-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2020-12-21 23:25:10.000000 trytond_sale_promotion-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2021-12-11 16:59:34.000000 trytond_sale_promotion-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:02.746231 trytond_sale_promotion-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2020-12-21 23:25:10.000000 trytond_sale_promotion-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2019-06-04 16:49:45.000000 trytond_sale_promotion-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:02.746231 trytond_sale_promotion-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2970 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2916 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2525 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2929 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2953 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2680 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3168 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2960 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2486 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2928 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2831 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2627 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2868 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2779 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2798 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2512 2022-10-29 07:50:33.000000 trytond_sale_promotion-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2396 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2527 2022-10-29 07:50:34.000000 trytond_sale_promotion-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2019-10-11 23:09:48.000000 trytond_sale_promotion-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11540 2022-10-11 19:49:58.000000 trytond_sale_promotion-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3940 2021-04-27 07:34:41.000000 trytond_sale_promotion-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:18:02.749564 trytond_sale_promotion-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5180 2022-10-29 07:39:11.000000 trytond_sale_promotion-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:02.746231 trytond_sale_promotion-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_promotion-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4595 2021-10-11 15:16:54.000000 trytond_sale_promotion-6.6.0/tests/scenario_sale_promotion.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2487 2020-12-21 23:25:10.000000 trytond_sale_promotion-6.6.0/tests/scenario_sale_promotion_amount.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2022-04-16 16:30:57.000000 trytond_sale_promotion-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_promotion-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2022-10-31 15:10:09.000000 trytond_sale_promotion-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2022-10-31 16:17:59.000000 trytond_sale_promotion-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:02.749564 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3222 2022-10-31 16:18:02.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1656 2022-10-31 16:18:02.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:18:02.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 16:18:02.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:51.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      228 2022-10-31 16:18:02.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:18:02.000000 trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:02.746231 trytond_sale_promotion-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2021-10-07 13:08:07.000000 trytond_sale_promotion-6.6.0/view/promotion_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-04-08 16:23:26.000000 trytond_sale_promotion-6.6.0/view/promotion_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:23.161507 trytond_sale_promotion-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1675 2023-05-01 11:00:23.000000 trytond_sale_promotion-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:00:23.000000 trytond_sale_promotion-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_promotion-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3215 2023-05-01 11:40:23.161507 trytond_sale_promotion-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:23.158174 trytond_sale_promotion-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      940 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:23.154841 trytond_sale_promotion-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2970 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2916 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2525 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2929 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2953 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2643 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2680 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3168 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2960 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2486 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2928 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2831 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2627 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2868 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2428 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2779 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2798 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2396 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2527 2023-04-29 08:02:40.000000 trytond_sale_promotion-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11540 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3940 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:40:23.161507 trytond_sale_promotion-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4370 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:23.154841 trytond_sale_promotion-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4595 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/tests/scenario_sale_promotion.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2487 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/tests/scenario_sale_promotion_amount.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-05-01 11:00:17.000000 trytond_sale_promotion-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:23.161507 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3215 2023-05-01 11:40:22.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1630 2023-05-01 11:40:23.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:40:22.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:40:22.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      228 2023-05-01 11:40:22.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:40:22.000000 trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:23.158174 trytond_sale_promotion-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/view/promotion_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_sale_promotion-6.8.0/view/promotion_list.xml
```

### Comparing `trytond_sale_promotion-6.6.0/CHANGELOG` & `trytond_sale_promotion-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_sale_promotion-6.6.0/COPYRIGHT` & `trytond_sale_promotion-6.8.0/COPYRIGHT`

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

### Comparing `trytond_sale_promotion-6.6.0/LICENSE` & `trytond_sale_promotion-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/PKG-INFO` & `trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_sale_promotion
-Version: 6.6.0
+Name: trytond-sale-promotion
+Version: 6.8.0
 Summary: Tryton module for sale promotion
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_promotion
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale promotion
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
 
 Sale Promotion
 ##############
 
 The sale_promotion module allows to apply promotions on sale based on criteria.
```

### Comparing `trytond_sale_promotion-6.6.0/README.rst` & `trytond_sale_promotion-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/doc/index.rst` & `trytond_sale_promotion-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/bg.po` & `trytond_sale_promotion-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/ca.po` & `trytond_sale_promotion-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/cs.po` & `trytond_sale_promotion-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/de.po` & `trytond_sale_promotion-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/es.po` & `trytond_sale_promotion-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/es_419.po` & `trytond_sale_promotion-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/et.po` & `trytond_sale_promotion-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/fa.po` & `trytond_sale_promotion-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/fi.po` & `trytond_sale_promotion-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/fr.po` & `trytond_sale_promotion-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/hu.po` & `trytond_sale_promotion-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/id.po` & `trytond_sale_promotion-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/it.po` & `trytond_sale_promotion-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/lo.po` & `trytond_sale_promotion-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/lt.po` & `trytond_sale_promotion-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/nl.po` & `trytond_sale_promotion-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/pl.po` & `trytond_sale_promotion-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/pt.po` & `trytond_sale_promotion-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/ro.po` & `trytond_sale_promotion-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/ru.po` & `trytond_sale_promotion-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/sl.po` & `trytond_sale_promotion-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/tr.po` & `trytond_sale_promotion-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/uk.po` & `trytond_sale_promotion-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/locale/zh_CN.po` & `trytond_sale_promotion-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/sale.py` & `trytond_sale_promotion-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/sale.xml` & `trytond_sale_promotion-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/setup.py` & `trytond_sale_promotion-6.8.0/setup.py`

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_promotion'
 
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
 
 requires = ['simpleeval']
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
     description='Tryton module for sale promotion',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_promotion',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale promotion',
     package_dir={'trytond.modules.sale_promotion': '.'},
     packages=(
         ['trytond.modules.sale_promotion']
         + ['trytond.modules.sale_promotion.%s' % p for p in find_packages()]
         ),
@@ -123,28 +101,27 @@
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
     sale_promotion = trytond.modules.sale_promotion
     """,
     )
```

### Comparing `trytond_sale_promotion-6.6.0/tests/scenario_sale_promotion.rst` & `trytond_sale_promotion-6.8.0/tests/scenario_sale_promotion.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/tests/scenario_sale_promotion_amount.rst` & `trytond_sale_promotion-6.8.0/tests/scenario_sale_promotion_amount.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/PKG-INFO` & `trytond_sale_promotion-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-sale-promotion
-Version: 6.6.0
+Name: trytond_sale_promotion
+Version: 6.8.0
 Summary: Tryton module for sale promotion
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_promotion
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale promotion
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
 
 Sale Promotion
 ##############
 
 The sale_promotion module allows to apply promotions on sale based on criteria.
```

### Comparing `trytond_sale_promotion-6.6.0/trytond_sale_promotion.egg-info/SOURCES.txt` & `trytond_sale_promotion-6.8.0/trytond_sale_promotion.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

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
@@ -48,14 +44,15 @@
 ./tests/__init__.py
 ./tests/scenario_sale_promotion.rst
 ./tests/scenario_sale_promotion_amount.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/promotion_form.xml
 ./view/promotion_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_sale_promotion-6.6.0/view/promotion_form.xml` & `trytond_sale_promotion-6.8.0/view/promotion_form.xml`

 * *Files identical despite different names*

