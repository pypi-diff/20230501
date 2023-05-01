# Comparing `tmp/trytond_stock_package_shipping_ups-6.6.0.tar.gz` & `tmp/trytond_stock_package_shipping_ups-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_ups-6.6.0.tar", last modified: Mon Oct 31 16:32:25 2022, max compression
+gzip compressed data, was "trytond_stock_package_shipping_ups-6.8.0.tar", last modified: Mon May  1 12:00:39 2023, max compression
```

## Comparing `trytond_stock_package_shipping_ups-6.6.0.tar` & `trytond_stock_package_shipping_ups-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:25.479317 trytond_stock_package_shipping_ups-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2061 2022-04-08 16:28:17.000000 trytond_stock_package_shipping_ups-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_package_shipping_ups-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      611 2022-10-31 16:32:24.000000 trytond_stock_package_shipping_ups-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_package_shipping_ups-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1198 2022-10-31 16:32:23.000000 trytond_stock_package_shipping_ups-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2022-10-31 16:32:23.000000 trytond_stock_package_shipping_ups-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:19.000000 trytond_stock_package_shipping_ups-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_package_shipping_ups-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3675 2022-10-31 16:32:25.479317 trytond_stock_package_shipping_ups-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1457 2018-08-18 09:55:19.000000 trytond_stock_package_shipping_ups-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      610 2021-12-11 16:59:34.000000 trytond_stock_package_shipping_ups-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4698 2022-06-21 08:21:56.000000 trytond_stock_package_shipping_ups-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2021-10-07 13:09:31.000000 trytond_stock_package_shipping_ups-6.6.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:25.475984 trytond_stock_package_shipping_ups-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1457 2018-08-18 09:55:19.000000 trytond_stock_package_shipping_ups-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2019-06-04 16:49:46.000000 trytond_stock_package_shipping_ups-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:25.475984 trytond_stock_package_shipping_ups-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3479 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4212 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3359 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4311 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4252 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3297 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3438 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4404 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3359 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4353 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3412 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3321 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3408 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3453 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3383 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4236 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3464 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3678 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3496 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3459 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3634 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3359 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3273 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3374 2022-10-29 07:50:43.000000 trytond_stock_package_shipping_ups-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1284 2022-10-11 19:45:05.000000 trytond_stock_package_shipping_ups-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:32:25.479317 trytond_stock_package_shipping_ups-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5363 2022-10-29 07:39:12.000000 trytond_stock_package_shipping_ups-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16286 2022-10-21 11:17:03.000000 trytond_stock_package_shipping_ups-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2018-08-18 09:55:19.000000 trytond_stock_package_shipping_ups-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:25.475984 trytond_stock_package_shipping_ups-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_package_shipping_ups-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8075 2022-09-25 18:27:36.000000 trytond_stock_package_shipping_ups-6.6.0/tests/scenario_shipping_ups.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2022-04-16 16:30:57.000000 trytond_stock_package_shipping_ups-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2022-04-25 16:11:54.000000 trytond_stock_package_shipping_ups-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2022-10-31 15:10:09.000000 trytond_stock_package_shipping_ups-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2022-10-31 16:32:22.000000 trytond_stock_package_shipping_ups-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:25.479317 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3675 2022-10-31 16:32:24.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1828 2022-10-31 16:32:25.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:32:24.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-31 16:32:24.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:10.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-10-31 16:32:24.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:32:24.000000 trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:32:25.475984 trytond_stock_package_shipping_ups-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2022-04-08 16:25:28.000000 trytond_stock_package_shipping_ups-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2018-08-18 09:55:19.000000 trytond_stock_package_shipping_ups-6.6.0/view/package_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      711 2020-12-17 23:30:26.000000 trytond_stock_package_shipping_ups-6.6.0/view/ups_credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2020-12-17 23:30:26.000000 trytond_stock_package_shipping_ups-6.6.0/view/ups_credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:39.036596 trytond_stock_package_shipping_ups-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1361 2023-05-01 11:14:03.000000 trytond_stock_package_shipping_ups-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-05-01 11:14:02.000000 trytond_stock_package_shipping_ups-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3656 2023-05-01 12:00:39.036596 trytond_stock_package_shipping_ups-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1457 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      610 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4698 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:39.029929 trytond_stock_package_shipping_ups-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1457 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:39.026596 trytond_stock_package_shipping_ups-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3479 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4212 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3359 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4311 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4252 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3297 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3438 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4404 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3359 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4353 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3412 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3321 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3408 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3453 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3383 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3464 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3678 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3496 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3459 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3634 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3359 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3273 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3374 2023-04-29 08:02:49.000000 trytond_stock_package_shipping_ups-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1284 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:00:39.036596 trytond_stock_package_shipping_ups-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4526 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16286 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:39.029929 trytond_stock_package_shipping_ups-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7928 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/tests/scenario_shipping_ups.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-05-01 11:13:57.000000 trytond_stock_package_shipping_ups-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:39.036596 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3656 2023-05-01 12:00:38.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1802 2023-05-01 12:00:38.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:00:38.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:00:38.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:00:38.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:00:38.000000 trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:39.029929 trytond_stock_package_shipping_ups-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_ups-6.8.0/view/package_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      711 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/view/ups_credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_ups-6.8.0/view/ups_credential_list.xml
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/CHANGELOG` & `trytond_stock_package_shipping_ups-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

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
 * Use contact mechanism from address
 * Update service types
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/COPYRIGHT` & `trytond_stock_package_shipping_ups-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2016-2022 B2CK.
-Copyright (C) 2016-2022 Nicolas Évrard.
+Copyright (C) 2016-2023 B2CK.
+Copyright (C) 2016-2023 Nicolas Évrard.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/LICENSE` & `trytond_stock_package_shipping_ups-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/PKG-INFO` & `trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_package_shipping_ups
-Version: 6.6.0
+Name: trytond-stock-package-shipping-ups
+Version: 6.8.0
 Summary: UPS connector for the Tryton application platform
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_ups
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping ups
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 
 Stock Package Shipping UPS Module
 #################################
 
 The Stock Package Shipping UPS module allows you to generate the UPS labels per
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/README.rst` & `trytond_stock_package_shipping_ups-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/__init__.py` & `trytond_stock_package_shipping_ups-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/carrier.py` & `trytond_stock_package_shipping_ups-6.8.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/carrier.xml` & `trytond_stock_package_shipping_ups-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/doc/index.rst` & `trytond_stock_package_shipping_ups-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/bg.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/ca.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/cs.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/de.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/es.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/es_419.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/et.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/fa.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/fi.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/fr.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/hu.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/id.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/it.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/lo.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/lt.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/nl.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/pl.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/pt.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/ro.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/ru.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/sl.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/tr.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/uk.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/locale/zh_CN.po` & `trytond_stock_package_shipping_ups-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/message.xml` & `trytond_stock_package_shipping_ups-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/setup.py` & `trytond_stock_package_shipping_ups-6.8.0/setup.py`

 * *Files 10% similar despite different names*

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
@@ -34,65 +31,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_package_shipping_ups'
 
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
 
 requires = ['requests']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_sale_shipment_cost'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='UPS connector for the Tryton application platform',
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
-            'https://hg.tryton.org/modules/stock_package_shipping_ups'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock package shipping ups',
     package_dir={'trytond.modules.stock_package_shipping_ups': '.'},
     packages=(
         ['trytond.modules.stock_package_shipping_ups']
         + ['trytond.modules.stock_package_shipping_ups.%s' % p
             for p in find_packages()]
@@ -129,27 +106,26 @@
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
     stock_package_shipping_ups = trytond.modules.stock_package_shipping_ups
     """,
     )
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/stock.py` & `trytond_stock_package_shipping_ups-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/stock.xml` & `trytond_stock_package_shipping_ups-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/tests/scenario_shipping_ups.rst` & `trytond_stock_package_shipping_ups-6.8.0/tests/scenario_shipping_ups.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 ========================================
 Stock Package Shipping with UPS scenario
 ========================================
 
 Imports::
 
-    >>> import datetime
     >>> import os
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['stock_package_shipping_ups', 'sale', 'sale_shipment_cost'])
 
 Create company::
@@ -209,23 +206,22 @@
 
 Create the packs and ship the shipment::
 
     >>> Package = Model.get('stock.package')
     >>> shipment, = sale.shipments
     >>> shipment.shipping_description = 'Football Players'
     >>> shipment.click('assign_try')
-    True
     >>> shipment.click('pick')
     >>> pack = shipment.packages.new()
     >>> pack.type = ups_box
     >>> pack_move, = pack.moves.find([])
     >>> pack.moves.append(pack_move)
     >>> shipment.click('pack')
 
-    >>> create_shipping = Wizard('stock.shipment.create_shipping', [shipment])
+    >>> create_shipping = shipment.click('create_shipping')
     >>> shipment.reload()
     >>> shipment.reference != ''
     True
     >>> pack, = shipment.root_packages
     >>> pack.shipping_label is not None
     True
     >>> pack.shipping_label_mimetype
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/PKG-INFO` & `trytond_stock_package_shipping_ups-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-package-shipping-ups
-Version: 6.6.0
+Name: trytond_stock_package_shipping_ups
+Version: 6.8.0
 Summary: UPS connector for the Tryton application platform
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package_shipping_ups
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock package shipping ups
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 
 Stock Package Shipping UPS Module
 #################################
 
 The Stock Package Shipping UPS module allows you to generate the UPS labels per
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_ups-6.8.0/trytond_stock_package_shipping_ups.egg-info/SOURCES.txt`

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
 carrier.py
@@ -53,14 +49,15 @@
 ./tests/scenario_shipping_ups.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/carrier_form.xml
 ./view/package_type_form.xml
 ./view/ups_credential_form.xml
 ./view/ups_credential_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_stock_package_shipping_ups-6.6.0/view/carrier_form.xml` & `trytond_stock_package_shipping_ups-6.8.0/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_ups-6.6.0/view/ups_credential_form.xml` & `trytond_stock_package_shipping_ups-6.8.0/view/ups_credential_form.xml`

 * *Files identical despite different names*

