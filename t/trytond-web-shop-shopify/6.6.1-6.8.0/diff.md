# Comparing `tmp/trytond_web_shop_shopify-6.6.1.tar.gz` & `tmp/trytond_web_shop_shopify-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_shopify-6.6.1.tar", last modified: Sat Mar  4 11:12:25 2023, max compression
+gzip compressed data, was "trytond_web_shop_shopify-6.8.0.tar", last modified: Mon May  1 11:35:59 2023, max compression
```

## Comparing `trytond_web_shop_shopify-6.6.1.tar` & `trytond_web_shop_shopify-6.8.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:12:25.817658 trytond_web_shop_shopify-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      621 2023-03-04 11:12:22.000000 trytond_web_shop_shopify-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-03-04 11:12:21.000000 trytond_web_shop_shopify-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2555 2023-03-04 11:12:25.814324 trytond_web_shop_shopify-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2282 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5112 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5597 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:12:25.810991 trytond_web_shop_shopify-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:12:25.804324 trytond_web_shop_shopify-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10064 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10405 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10110 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10355 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7363 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7351 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10006 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4138 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4339 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21438 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      790 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2137 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17299 2023-02-23 20:24:34.000000 trytond_web_shop_shopify-6.6.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:12:25.817658 trytond_web_shop_shopify-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5030 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1124 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/shopify_retry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6220 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2852 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:12:25.807658 trytond_web_shop_shopify-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20077 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/tests/scenario_web_shop_shopify.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7234 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/tests/scenario_web_shop_shopify_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2022-12-19 12:03:07.000000 trytond_web_shop_shopify-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:12:25.814324 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2555 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2742 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:12:25.000000 trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:12:25.810991 trytond_web_shop_shopify-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/product_attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_shopify_payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_shopify_payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_stock_location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/shop_stock_location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/stock_shipment_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/view/stock_shipment_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28233 2023-02-23 20:24:34.000000 trytond_web_shop_shopify-6.6.1/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2022-12-19 12:02:59.000000 trytond_web_shop_shopify-6.6.1/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-05-01 10:57:24.000000 trytond_web_shop_shopify-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:57:24.000000 trytond_web_shop_shopify-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2546 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5112 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5642 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.061563 trytond_web_shop_shopify-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.054896 trytond_web_shop_shopify-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10064 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10405 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10110 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10355 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7363 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7351 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10006 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4138 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4339 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21438 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17299 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4993 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/shopify_retry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2852 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.054896 trytond_web_shop_shopify-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20068 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7234 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-05-01 10:57:19.000000 trytond_web_shop_shopify-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2546 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2742 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.058230 trytond_web_shop_shopify-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/product_attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_stock_location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_stock_location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/stock_shipment_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/stock_shipment_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    28233 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/web.xml
```

### Comparing `trytond_web_shop_shopify-6.6.1/CHANGELOG` & `trytond_web_shop_shopify-6.8.0/CHANGELOG`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Replace deprecated fulfillment by fulfillment order
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_web_shop_shopify-6.6.1/COPYRIGHT` & `trytond_web_shop_shopify-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/LICENSE` & `trytond_web_shop_shopify-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/PKG-INFO` & `trytond_web_shop_shopify-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_shopify
-Version: 6.6.1
+Version: 6.8.0
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-web-shop-shopify
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/web_shop_shopify
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web shopify ecommerce
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
 
 #######################
 Web Shop Shopify Module
 #######################
```

### Comparing `trytond_web_shop_shopify-6.6.1/__init__.py` & `trytond_web_shop_shopify-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/account.py` & `trytond_web_shop_shopify-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/common.py` & `trytond_web_shop_shopify-6.8.0/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from trytond.model import fields
 from trytond.pool import Pool
 
 
 class IdentifierMixin:
     __slots__ = ()
 
-    shopify_identifier_signed = fields.BigInteger(
+    shopify_identifier_signed = fields.Integer(
         lazy_gettext('web_shop_shopify.msg_shopify_identifier'))
-    shopify_identifier = fields.Function(fields.BigInteger(
+    shopify_identifier_signed._sql_type = 'BIGINT'
+    shopify_identifier = fields.Function(fields.Integer(
             lazy_gettext('web_shop_shopify.msg_shopify_identifier')),
         'get_shopify_identifier', setter='set_shopify_identifier',
         searcher='search_shopify_identifier')
     shopify_identifier_char = fields.Function(fields.Char(
             lazy_gettext('web_shop_shopify.msg_shopify_identifier')),
         'get_shopify_identifier', setter='set_shopify_identifier',
         searcher='search_shopify_identifier')
```

### Comparing `trytond_web_shop_shopify-6.6.1/doc/conf.py` & `trytond_web_shop_shopify-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
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
```

### Comparing `trytond_web_shop_shopify-6.6.1/doc/design.rst` & `trytond_web_shop_shopify-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/doc/usage.rst` & `trytond_web_shop_shopify-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/ir.py` & `trytond_web_shop_shopify-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/ir.xml` & `trytond_web_shop_shopify-6.8.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/bg.po` & `trytond_web_shop_shopify-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/ca.po` & `trytond_web_shop_shopify-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/cs.po` & `trytond_web_shop_shopify-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/de.po` & `trytond_web_shop_shopify-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/es.po` & `trytond_web_shop_shopify-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/es_419.po` & `trytond_web_shop_shopify-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/et.po` & `trytond_web_shop_shopify-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/fa.po` & `trytond_web_shop_shopify-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/fi.po` & `trytond_web_shop_shopify-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/fr.po` & `trytond_web_shop_shopify-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/hu.po` & `trytond_web_shop_shopify-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/id.po` & `trytond_web_shop_shopify-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/it.po` & `trytond_web_shop_shopify-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/lo.po` & `trytond_web_shop_shopify-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/lt.po` & `trytond_web_shop_shopify-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/nl.po` & `trytond_web_shop_shopify-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/pl.po` & `trytond_web_shop_shopify-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/pt.po` & `trytond_web_shop_shopify-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/ro.po` & `trytond_web_shop_shopify-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/ru.po` & `trytond_web_shop_shopify-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/sl.po` & `trytond_web_shop_shopify-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/tr.po` & `trytond_web_shop_shopify-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/uk.po` & `trytond_web_shop_shopify-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/locale/zh_CN.po` & `trytond_web_shop_shopify-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/message.xml` & `trytond_web_shop_shopify-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/party.py` & `trytond_web_shop_shopify-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/product.py` & `trytond_web_shop_shopify-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/product.xml` & `trytond_web_shop_shopify-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/routes.py` & `trytond_web_shop_shopify-6.8.0/routes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import base64
 import hashlib
 import hmac
 import logging
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
-from werkzeug.exceptions import abort
-from werkzeug.wrappers import Response
-
-from trytond.protocols.wrappers import with_pool, with_transaction
+from trytond.protocols.wrappers import (
+    HTTPStatus, Response, abort, with_pool, with_transaction)
 from trytond.wsgi import app
 
 logger = logging.getLogger(__name__)
 
 
 def verify_webhook(data, hmac_header, secret):
     digest = hmac.new(secret, data, hashlib.sha256).digest()
```

### Comparing `trytond_web_shop_shopify-6.6.1/sale.py` & `trytond_web_shop_shopify-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/setup.py` & `trytond_web_shop_shopify-6.8.0/setup.py`

 * *Files 1% similar despite different names*

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
@@ -37,16 +34,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_web_shop_shopify'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['ShopifyAPI', 'pyactiveresource', 'python-sql', 'python-dateutil']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -62,23 +62,23 @@
     ]
 
 setup(name=name,
     version=version,
     description='Module to integrate Tryton with Shopify',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-web-shop-shopify'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/web_shop_shopify',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='web shopify ecommerce',
     package_dir={'trytond.modules.web_shop_shopify': '.'},
     packages=(
         ['trytond.modules.web_shop_shopify']
         + ['trytond.modules.web_shop_shopify.%s' % p
             for p in find_packages()]
@@ -116,23 +116,23 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_web_shop_shopify-6.6.1/shopify_retry.py` & `trytond_web_shop_shopify-6.8.0/shopify_retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import time
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
 from pyactiveresource.connection import ClientError
 from shopify import Limits
 from shopify.base import ShopifyConnection
 
+from trytond.protocols.wrappers import HTTPStatus
+
 
 def patch():
     def _open(*args, **kwargs):
         while True:
             try:
                 return func(*args, **kwargs)
             except ClientError as e:
```

### Comparing `trytond_web_shop_shopify-6.6.1/stock.py` & `trytond_web_shop_shopify-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/stock.xml` & `trytond_web_shop_shopify-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/tests/scenario_web_shop_shopify.rst` & `trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify.rst`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
     >>> len(order.fulfillments)
     1
     >>> order.financial_status
     'paid'
 
 Ignore shipment exception::
 
-    >>> shipment_exception = Wizard('sale.handle.shipment.exception', [sale])
+    >>> shipment_exception = sale.click('handle_shipment_exception')
     >>> move = shipment_exception.form.recreate_moves.pop()
     >>> shipment_exception.execute('handle')
 
     >>> order.reload()
     >>> order.fulfillment_status
     'partial'
     >>> len(order.fulfillments)
```

### Comparing `trytond_web_shop_shopify-6.6.1/tests/scenario_web_shop_shopify_secondary_unit.rst` & `trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/tox.ini` & `trytond_web_shop_shopify-6.8.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/web_shop_shopify/* -m unittest discover -s tests
-    coverage report --include=./**/web_shop_shopify/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/PKG-INFO` & `trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-web-shop-shopify
-Version: 6.6.1
+Version: 6.8.0
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-web-shop-shopify
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/web_shop_shopify
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web shopify ecommerce
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
 
 #######################
 Web Shop Shopify Module
 #######################
```

### Comparing `trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/SOURCES.txt` & `trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/trytond_web_shop_shopify.egg-info/requires.txt` & `trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ShopifyAPI
 pyactiveresource
 python-sql
 python-dateutil
-trytond_account_payment<6.7,>=6.6
-trytond_currency<6.7,>=6.6
-trytond_party<6.7,>=6.6
-trytond_product<6.7,>=6.6
-trytond_product_attribute<6.7,>=6.6
-trytond_sale<6.7,>=6.6
-trytond_sale_amendment<6.7,>=6.6
-trytond_sale_payment<6.7,>=6.6
-trytond_stock<6.7,>=6.6
-trytond_web_shop<6.7,>=6.6
-trytond<6.7,>=6.6
+trytond_account_payment<6.9,>=6.8
+trytond_currency<6.9,>=6.8
+trytond_party<6.9,>=6.8
+trytond_product<6.9,>=6.8
+trytond_product_attribute<6.9,>=6.8
+trytond_sale<6.9,>=6.8
+trytond_sale_amendment<6.9,>=6.8
+trytond_sale_payment<6.9,>=6.8
+trytond_stock<6.9,>=6.8
+trytond_web_shop<6.9,>=6.8
+trytond<6.9,>=6.8
 
 [test]
-proteus<6.7,>=6.6
-trytond_account_payment_clearing<6.7,>=6.6
-trytond_customs<6.7,>=6.6
-trytond_product_measurements<6.7,>=6.6
-trytond_product_image<6.7,>=6.6
-trytond_sale_discount<6.7,>=6.6
-trytond_sale_shipment_cost<6.7,>=6.6
-trytond_sale_secondary_unit<6.7,>=6.6
+proteus<6.9,>=6.8
+trytond_account_payment_clearing<6.9,>=6.8
+trytond_customs<6.9,>=6.8
+trytond_product_measurements<6.9,>=6.8
+trytond_product_image<6.9,>=6.8
+trytond_sale_discount<6.9,>=6.8
+trytond_sale_shipment_cost<6.9,>=6.8
+trytond_sale_secondary_unit<6.9,>=6.8
```

### Comparing `trytond_web_shop_shopify-6.6.1/view/shop_form.xml` & `trytond_web_shop_shopify-6.8.0/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/web.py` & `trytond_web_shop_shopify-6.8.0/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.6.1/web.xml` & `trytond_web_shop_shopify-6.8.0/web.xml`

 * *Files identical despite different names*

