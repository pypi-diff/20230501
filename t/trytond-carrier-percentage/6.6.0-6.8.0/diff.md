# Comparing `tmp/trytond_carrier_percentage-6.6.0.tar.gz` & `tmp/trytond_carrier_percentage-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_carrier_percentage-6.6.0.tar", last modified: Mon Oct 31 16:26:31 2022, max compression
+gzip compressed data, was "trytond_carrier_percentage-6.8.0.tar", last modified: Mon May  1 11:47:06 2023, max compression
```

## Comparing `trytond_carrier_percentage-6.6.0.tar` & `trytond_carrier_percentage-6.8.0.tar`

### file list

```diff
@@ -1,62 +1,59 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:31.367339 trytond_carrier_percentage-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_carrier_percentage-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_carrier_percentage-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-31 16:26:30.000000 trytond_carrier_percentage-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_carrier_percentage-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1775 2022-10-31 16:26:29.000000 trytond_carrier_percentage-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2022-10-31 16:26:28.000000 trytond_carrier_percentage-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:30.000000 trytond_carrier_percentage-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_carrier_percentage-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2427 2022-10-31 16:26:31.367339 trytond_carrier_percentage-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2019-02-13 10:09:30.000000 trytond_carrier_percentage-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2021-12-11 16:59:33.000000 trytond_carrier_percentage-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2022-09-25 18:21:55.000000 trytond_carrier_percentage-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2019-02-13 10:09:30.000000 trytond_carrier_percentage-6.6.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:31.364006 trytond_carrier_percentage-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2019-02-13 10:09:30.000000 trytond_carrier_percentage-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:31.364006 trytond_carrier_percentage-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2022-10-29 07:50:38.000000 trytond_carrier_percentage-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      956 2022-09-12 22:47:25.000000 trytond_carrier_percentage-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:26:31.367339 trytond_carrier_percentage-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5402 2022-10-29 07:39:10.000000 trytond_carrier_percentage-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2155 2020-08-04 22:27:56.000000 trytond_carrier_percentage-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:31.364006 trytond_carrier_percentage-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_carrier_percentage-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6999 2022-09-29 07:07:37.000000 trytond_carrier_percentage-6.6.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2022-04-16 16:30:56.000000 trytond_carrier_percentage-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_carrier_percentage-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-10-31 15:10:09.000000 trytond_carrier_percentage-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2022-10-31 16:26:27.000000 trytond_carrier_percentage-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:31.367339 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2427 2022-10-31 16:26:30.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1604 2022-10-31 16:26:31.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:26:30.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 16:26:30.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:56.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2022-10-31 16:26:30.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:26:30.000000 trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:31.364006 trytond_carrier_percentage-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2019-02-13 10:09:30.000000 trytond_carrier_percentage-6.6.0/view/carrier_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:06.329844 trytond_carrier_percentage-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1938 2023-05-01 11:04:48.000000 trytond_carrier_percentage-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-01 11:04:47.000000 trytond_carrier_percentage-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_carrier_percentage-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-05-01 11:47:06.329844 trytond_carrier_percentage-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-01-16 14:00:20.000000 trytond_carrier_percentage-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:20.000000 trytond_carrier_percentage-6.8.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:06.326511 trytond_carrier_percentage-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-01-16 14:00:20.000000 trytond_carrier_percentage-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:06.323177 trytond_carrier_percentage-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-29 08:02:44.000000 trytond_carrier_percentage-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      956 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:06.329844 trytond_carrier_percentage-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4588 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2155 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:06.323177 trytond_carrier_percentage-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6880 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_carrier_percentage-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-05-01 11:04:42.000000 trytond_carrier_percentage-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:06.329844 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-05-01 11:47:05.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1578 2023-05-01 11:47:06.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:05.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:47:05.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-05-01 11:47:05.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:05.000000 trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:06.323177 trytond_carrier_percentage-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_carrier_percentage-6.8.0/view/carrier_form.xml
```

### Comparing `trytond_carrier_percentage-6.6.0/CHANGELOG` & `trytond_carrier_percentage-6.8.0/CHANGELOG`

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

### Comparing `trytond_carrier_percentage-6.6.0/COPYRIGHT` & `trytond_carrier_percentage-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2022 Cédric Krier.
+Copyright (C) 2011-2023 Cédric Krier.
 Copyright (C) 2011-2012 Bertrand Chenal.
-Copyright (C) 2011-2022 Nicolas Évrard.
-Copyright (C) 2011-2022 B2CK SPRL.
+Copyright (C) 2011-2023 Nicolas Évrard.
+Copyright (C) 2011-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_carrier_percentage-6.6.0/LICENSE` & `trytond_carrier_percentage-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/PKG-INFO` & `trytond_carrier_percentage-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_carrier_percentage
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add cost method "on percentage" on carrier
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
-Project-URL: Source Code, https://hg.tryton.org/modules/carrier_percentage
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier percentage
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
 Provides-Extra: test
 License-File: LICENSE
 
 Carrier Percentage Module
 #########################
 
 The carrier percentage module adds a cost method based on percentage.
```

### Comparing `trytond_carrier_percentage-6.6.0/__init__.py` & `trytond_carrier_percentage-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/carrier.py` & `trytond_carrier_percentage-6.8.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/locale/lo.po` & `trytond_carrier_percentage-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/sale.py` & `trytond_carrier_percentage-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/setup.py` & `trytond_carrier_percentage-6.8.0/setup.py`

 * *Files 14% similar despite different names*

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
@@ -34,64 +31,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_carrier_percentage'
 
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
 
 tests_require = [get_require_version('proteus'),
     get_require_version('trytond_purchase_shipment_cost'),
     get_require_version('trytond_sale_shipment_cost'),
     get_require_version('trytond_stock_shipment_cost'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add cost method "on percentage" on carrier',
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
-        "Source Code": 'https://hg.tryton.org/modules/carrier_percentage',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton carrier percentage',
     package_dir={'trytond.modules.carrier_percentage': '.'},
     packages=(
         ['trytond.modules.carrier_percentage']
         + ['trytond.modules.carrier_percentage.%s' % p
             for p in find_packages()]
@@ -129,27 +107,26 @@
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
     carrier_percentage = trytond.modules.carrier_percentage
     """,
     )
```

### Comparing `trytond_carrier_percentage-6.6.0/stock.py` & `trytond_carrier_percentage-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst` & `trytond_carrier_percentage-6.8.0/tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 =======================================================
 Carrier Percentage with Purchase Shipment Cost Scenario
 =======================================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'carrier_percentage',
     ...         'purchase_shipment_cost',
     ...         'sale_shipment_cost',
```

### Comparing `trytond_carrier_percentage-6.6.0/tests/test_module.py` & `trytond_carrier_percentage-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/PKG-INFO` & `trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-carrier-percentage
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add cost method "on percentage" on carrier
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
-Project-URL: Source Code, https://hg.tryton.org/modules/carrier_percentage
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton carrier percentage
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
 Provides-Extra: test
 License-File: LICENSE
 
 Carrier Percentage Module
 #########################
 
 The carrier percentage module adds a cost method based on percentage.
```

### Comparing `trytond_carrier_percentage-6.6.0/trytond_carrier_percentage.egg-info/SOURCES.txt` & `trytond_carrier_percentage-6.8.0/trytond_carrier_percentage.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

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
@@ -46,14 +42,15 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_carrier_percentage_with_purchase_shipment_cost.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/carrier_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

