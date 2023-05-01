# Comparing `tmp/trytond_sale_product_customer-6.6.0.tar.gz` & `tmp/trytond_sale_product_customer-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_product_customer-6.6.0.tar", last modified: Mon Oct 31 16:23:39 2022, max compression
+gzip compressed data, was "trytond_sale_product_customer-6.8.0.tar", last modified: Mon May  1 11:56:33 2023, max compression
```

## Comparing `trytond_sale_product_customer-6.6.0.tar` & `trytond_sale_product_customer-6.8.0.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:39.461428 trytond_sale_product_customer-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_product_customer-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_product_customer-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2022-10-31 16:23:38.000000 trytond_sale_product_customer-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_product_customer-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 16:23:37.000000 trytond_sale_product_customer-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      719 2022-10-31 16:23:37.000000 trytond_sale_product_customer-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_sale_product_customer-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_product_customer-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2022-10-31 16:23:39.461428 trytond_sale_product_customer-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2019-06-04 16:49:46.000000 trytond_sale_product_customer-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      899 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:39.458094 trytond_sale_product_customer-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2019-06-04 16:49:46.000000 trytond_sale_product_customer-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:39.454761 trytond_sale_product_customer-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2022-10-29 07:50:42.000000 trytond_sale_product_customer-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1249 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1216 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1254 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1218 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1246 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:42.000000 trytond_sale_product_customer-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2022-10-29 07:50:41.000000 trytond_sale_product_customer-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5821 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2019-06-04 16:49:46.000000 trytond_sale_product_customer-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7544 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4759 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:23:39.461428 trytond_sale_product_customer-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5358 2022-10-29 07:39:11.000000 trytond_sale_product_customer-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:39.454761 trytond_sale_product_customer-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_product_customer-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1670 2020-07-09 09:37:22.000000 trytond_sale_product_customer-6.6.0/tests/scenario_sale_copy_product_customer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1923 2020-07-09 09:37:22.000000 trytond_sale_product_customer-6.6.0/tests/scenario_sale_product_customer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_product_customer-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 15:10:09.000000 trytond_sale_product_customer-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2022-10-31 16:23:36.000000 trytond_sale_product_customer-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:39.461428 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2022-10-31 16:23:38.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2291 2022-10-31 16:23:39.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:23:38.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:23:38.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2022-10-31 16:23:38.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:23:38.000000 trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:39.458094 trytond_sale_product_customer-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      671 2021-02-02 12:17:57.000000 trytond_sale_product_customer-6.6.0/view/product_customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2019-10-11 23:09:48.000000 trytond_sale_product_customer-6.6.0/view/product_customer_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2019-10-11 23:09:48.000000 trytond_sale_product_customer-6.6.0/view/product_customer_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2019-10-11 23:09:48.000000 trytond_sale_product_customer-6.6.0/view/sale_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/view/sale_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2022-10-11 19:49:58.000000 trytond_sale_product_customer-6.6.0/view/sale_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2019-06-04 16:49:46.000000 trytond_sale_product_customer-6.6.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2022-04-08 16:23:26.000000 trytond_sale_product_customer-6.6.0/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2022-04-08 16:23:26.000000 trytond_sale_product_customer-6.6.0/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2019-06-04 16:49:46.000000 trytond_sale_product_customer-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:33.180212 trytond_sale_product_customer-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      883 2023-05-01 11:11:10.000000 trytond_sale_product_customer-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      719 2023-05-01 11:11:10.000000 trytond_sale_product_customer-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2597 2023-05-01 11:56:33.180212 trytond_sale_product_customer-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      899 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:33.176878 trytond_sale_product_customer-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:33.170211 trytond_sale_product_customer-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1249 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1216 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1254 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1218 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1237 2023-04-30 10:46:36.000000 trytond_sale_product_customer-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-04-29 08:02:48.000000 trytond_sale_product_customer-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5821 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7527 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4759 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:56:33.180212 trytond_sale_product_customer-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4541 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:33.173545 trytond_sale_product_customer-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1670 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/tests/scenario_sale_copy_product_customer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1923 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/tests/scenario_sale_product_customer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-05-01 11:11:03.000000 trytond_sale_product_customer-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:33.180212 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2597 2023-05-01 11:56:32.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2265 2023-05-01 11:56:33.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:56:32.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:56:32.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-05-01 11:56:32.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:56:32.000000 trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:33.176878 trytond_sale_product_customer-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/product_customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/product_customer_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/product_customer_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/sale_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/sale_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/sale_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_sale_product_customer-6.8.0/view/template_form.xml
```

### Comparing `trytond_sale_product_customer-6.6.0/CHANGELOG` & `trytond_sale_product_customer-6.8.0/CHANGELOG`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_sale_product_customer-6.6.0/COPYRIGHT` & `trytond_sale_product_customer-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/LICENSE` & `trytond_sale_product_customer-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/PKG-INFO` & `trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_sale_product_customer
-Version: 6.6.0
+Name: trytond-sale-product-customer
+Version: 6.8.0
 Summary: Tryton module to manage customer product on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_product_customer
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale product customer
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
 
 Sale Product Customer Module
 ############################
 
 The sale_product_customer module defines customer's names and
```

### Comparing `trytond_sale_product_customer-6.6.0/__init__.py` & `trytond_sale_product_customer-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/bg.po` & `trytond_sale_product_customer-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/ca.po` & `trytond_sale_product_customer-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/cs.po` & `trytond_sale_product_customer-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/de.po` & `trytond_sale_product_customer-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/es.po` & `trytond_sale_product_customer-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/es_419.po` & `trytond_sale_product_customer-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/et.po` & `trytond_sale_product_customer-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/fa.po` & `trytond_sale_product_customer-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/fi.po` & `trytond_sale_product_customer-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/fr.po` & `trytond_sale_product_customer-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/hu.po` & `trytond_sale_product_customer-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/id.po` & `trytond_sale_product_customer-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/it.po` & `trytond_sale_product_customer-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/lo.po` & `trytond_sale_product_customer-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/lt.po` & `trytond_sale_product_customer-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/nl.po` & `trytond_sale_product_customer-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/pl.po` & `trytond_sale_product_customer-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/pt.po` & `trytond_sale_product_customer-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/ro.po` & `trytond_sale_product_customer-6.8.0/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 msgid "Customers"
 msgstr "Clienți"
 
 msgctxt "field:sale.amendment.line,product_customer:"
 msgid "Customer's Product"
 msgstr "Produsul Clientului"
 
-#, fuzzy
 msgctxt "field:sale.blanket_agreement.line,product_customer:"
 msgid "Customer's Product"
 msgstr "Produsul Clientului"
 
 msgctxt "field:sale.line,product_customer:"
 msgid "Customer's Product"
 msgstr "Produsul Clientului"
```

### Comparing `trytond_sale_product_customer-6.6.0/locale/ru.po` & `trytond_sale_product_customer-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/sl.po` & `trytond_sale_product_customer-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/tr.po` & `trytond_sale_product_customer-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/uk.po` & `trytond_sale_product_customer-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/locale/zh_CN.po` & `trytond_sale_product_customer-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/product.py` & `trytond_sale_product_customer-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/sale.py` & `trytond_sale_product_customer-6.8.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                     [
                         ('template.products', '=', Eval('product')),
                         ('product', '=', None),
                         ],
                     ('product', '=', Eval('product')),
                     ],
                 []),
-            ('party', '=', Eval('_parent_sale', {}).get('party')),
+            ('party', '=', Eval('customer', -1)),
             ],
         states={
             'invisible': Eval('type') != 'line',
             'readonly': Eval('sale_state') != 'draft',
             },
         depends={'sale'})
```

### Comparing `trytond_sale_product_customer-6.6.0/sale.xml` & `trytond_sale_product_customer-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/setup.py` & `trytond_sale_product_customer-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
 name = 'trytond_sale_product_customer'
 
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
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_sale_amendment'),
     get_require_version('trytond_sale_blanket_agreement'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to manage customer product on sale',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_product_customer',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale product customer',
     package_dir={'trytond.modules.sale_product_customer': '.'},
     packages=(
         ['trytond.modules.sale_product_customer']
         + ['trytond.modules.sale_product_customer.%s' % p
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
     sale_product_customer = trytond.modules.sale_product_customer
     """,
     )
```

### Comparing `trytond_sale_product_customer-6.6.0/tests/scenario_sale_copy_product_customer.rst` & `trytond_sale_product_customer-6.8.0/tests/scenario_sale_copy_product_customer.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/tests/scenario_sale_product_customer.rst` & `trytond_sale_product_customer-6.8.0/tests/scenario_sale_product_customer.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/PKG-INFO` & `trytond_sale_product_customer-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-sale-product-customer
-Version: 6.6.0
+Name: trytond_sale_product_customer
+Version: 6.8.0
 Summary: Tryton module to manage customer product on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_product_customer
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale product customer
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
 
 Sale Product Customer Module
 ############################
 
 The sale_product_customer module defines customer's names and
```

### Comparing `trytond_sale_product_customer-6.6.0/trytond_sale_product_customer.egg-info/SOURCES.txt` & `trytond_sale_product_customer-6.8.0/trytond_sale_product_customer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
@@ -56,14 +52,15 @@
 ./view/sale_amendment_line_form.xml
 ./view/sale_blanket_agreement_line_form.xml
 ./view/sale_blanket_agreement_line_list.xml
 ./view/sale_line_form.xml
 ./view/sale_line_tree.xml
 ./view/sale_line_tree_sequence.xml
 ./view/template_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_sale_product_customer-6.6.0/view/product_customer_form.xml` & `trytond_sale_product_customer-6.8.0/view/product_customer_form.xml`

 * *Files identical despite different names*

