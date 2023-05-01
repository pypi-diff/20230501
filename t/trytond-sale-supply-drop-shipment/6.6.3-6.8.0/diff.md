# Comparing `tmp/trytond_sale_supply_drop_shipment-6.6.3.tar.gz` & `tmp/trytond_sale_supply_drop_shipment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply_drop_shipment-6.6.3.tar", last modified: Sat Mar  4 11:23:18 2023, max compression
+gzip compressed data, was "trytond_sale_supply_drop_shipment-6.8.0.tar", last modified: Mon May  1 11:35:17 2023, max compression
```

## Comparing `trytond_sale_supply_drop_shipment-6.6.3.tar` & `trytond_sale_supply_drop_shipment-6.8.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.588049 trytond_sale_supply_drop_shipment-6.6.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     2369 2023-03-04 11:23:12.000000 trytond_sale_supply_drop_shipment-6.6.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-03-04 11:23:11.000000 trytond_sale_supply_drop_shipment-6.6.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3311 2023-03-04 11:23:18.588049 trytond_sale_supply_drop_shipment-6.6.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      985 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      972 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.514715 trytond_sale_supply_drop_shipment-6.6.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      985 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.518048 trytond_sale_supply_drop_shipment-6.6.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/icons/tryton-shipment-drop.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.434714 trytond_sale_supply_drop_shipment-6.6.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7295 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7950 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6792 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8001 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7921 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6729 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6665 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8095 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6792 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8080 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6955 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6650 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7352 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7184 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6888 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7951 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7107 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7470 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6455 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7327 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7240 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6792 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6438 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6818 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      850 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1156 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9272 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5453 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:23:18.591382 trytond_sale_supply_drop_shipment-6.6.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4561 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26279 2023-02-27 17:47:03.000000 trytond_sale_supply_drop_shipment-6.6.3/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14339 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.441380 trytond_sale_supply_drop_shipment-6.6.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10961 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/tests/scenario_sale_supply_drop_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4502 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/tests/scenario_sale_supply_drop_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4144 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-02-17 18:38:34.000000 trytond_sale_supply_drop_shipment-6.6.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.588049 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3311 2023-03-04 11:23:16.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2693 2023-03-04 11:23:17.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:23:16.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-03-04 11:23:16.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:25:23.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-03-04 11:23:16.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:23:16.000000 trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:23:18.468047 trytond_sale_supply_drop_shipment-6.6.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/purchase_request_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/sale_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1447 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/view/shipment_drop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/shipment_drop_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2022-12-19 12:02:57.000000 trytond_sale_supply_drop_shipment-6.6.3/view/stock_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2022-12-19 12:02:58.000000 trytond_sale_supply_drop_shipment-6.6.3/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.874385 trytond_sale_supply_drop_shipment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2231 2023-05-01 10:56:59.000000 trytond_sale_supply_drop_shipment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 10:56:59.000000 trytond_sale_supply_drop_shipment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3295 2023-05-01 11:35:17.874385 trytond_sale_supply_drop_shipment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      987 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.871052 trytond_sale_supply_drop_shipment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      987 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.871052 trytond_sale_supply_drop_shipment-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/icons/tryton-shipment-drop.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.861052 trytond_sale_supply_drop_shipment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7295 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7950 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6792 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8001 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7921 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6729 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6665 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8095 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6792 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8080 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6955 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6650 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7352 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7184 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6888 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7951 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7107 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7470 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6455 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7327 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7240 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6792 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6438 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6818 2023-04-29 08:02:38.000000 trytond_sale_supply_drop_shipment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      850 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1156 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9278 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5342 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:17.874385 trytond_sale_supply_drop_shipment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4500 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26279 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14339 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.861052 trytond_sale_supply_drop_shipment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10896 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tests/scenario_sale_supply_drop_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4466 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tests/scenario_sale_supply_drop_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4053 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 10:56:54.000000 trytond_sale_supply_drop_shipment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.874385 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3295 2023-05-01 11:35:16.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2693 2023-05-01 11:35:17.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:16.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 11:35:16.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-05-01 11:35:16.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:16.000000 trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:17.867719 trytond_sale_supply_drop_shipment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/purchase_request_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-6.8.0/view/sale_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/shipment_drop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/shipment_drop_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/stock_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-6.8.0/view/stock_move_form.xml
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/CHANGELOG` & `trytond_sale_supply_drop_shipment-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 
-Version 6.6.3 - 2023-03-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.2 - 2023-02-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-01-02
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Improve moves synchronisation on drop shipment
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/COPYRIGHT` & `trytond_sale_supply_drop_shipment-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/LICENSE` & `trytond_sale_supply_drop_shipment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/PKG-INFO` & `trytond_sale_supply_drop_shipment-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply_drop_shipment
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for sale supply drop shipment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_supply_drop_shipment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale supply drop shipment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,33 +38,33 @@
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
 
 Sale Supply Drop Shipment Model
 ###############################
 
 The Sale Supply Drop Shipment module adds a drop shipment option on product
-supplier if "supply on request" is checked. When checked, the purchase request
-and the linked purchase have the address of customer as Delivery Address;
-at the confirmation of the purchase a drop shipment is created and linked to
-both the purchase and the sale.
+supplier if "supply on request" is selected.
+When selected, the purchase request and the linked purchase have the address of
+customer as Delivery Address; at the confirmation of the purchase a drop
+shipment is created and linked to both the purchase and the sale.
 
 Drop Shipment
 *************
 
 A drop shipment is used when products are sent directly from the supplier to
 the customer without going through the warehouse.
 It is mainly composed of a supplier, a customer and a list of moves.
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/README.rst` & `trytond_sale_supply_drop_shipment-6.8.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Sale Supply Drop Shipment Model
 ###############################
 
 The Sale Supply Drop Shipment module adds a drop shipment option on product
-supplier if "supply on request" is checked. When checked, the purchase request
-and the linked purchase have the address of customer as Delivery Address;
-at the confirmation of the purchase a drop shipment is created and linked to
-both the purchase and the sale.
+supplier if "supply on request" is selected.
+When selected, the purchase request and the linked purchase have the address of
+customer as Delivery Address; at the confirmation of the purchase a drop
+shipment is created and linked to both the purchase and the sale.
 
 Drop Shipment
 *************
 
 A drop shipment is used when products are sent directly from the supplier to
 the customer without going through the warehouse.
 It is mainly composed of a supplier, a customer and a list of moves.
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/__init__.py` & `trytond_sale_supply_drop_shipment-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/doc/conf.py` & `trytond_sale_supply_drop_shipment-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/doc/index.rst` & `trytond_sale_supply_drop_shipment-6.8.0/doc/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Sale Supply Drop Shipment Model
 ###############################
 
 The Sale Supply Drop Shipment module adds a drop shipment option on product
-supplier if "supply on request" is checked. When checked, the purchase request
-and the linked purchase have the address of customer as Delivery Address;
-at the confirmation of the purchase a drop shipment is created and linked to
-both the purchase and the sale.
+supplier if "supply on request" is selected.
+When selected, the purchase request and the linked purchase have the address of
+customer as Delivery Address; at the confirmation of the purchase a drop
+shipment is created and linked to both the purchase and the sale.
 
 Drop Shipment
 *************
 
 A drop shipment is used when products are sent directly from the supplier to
 the customer without going through the warehouse.
 It is mainly composed of a supplier, a customer and a list of moves.
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/icons/LICENSE` & `trytond_sale_supply_drop_shipment-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/icons/tryton-shipment-drop.svg` & `trytond_sale_supply_drop_shipment-6.8.0/icons/tryton-shipment-drop.svg`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/bg.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/ca.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/cs.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/de.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/es.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/es_419.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/et.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/fa.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/fi.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/fr.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/hu.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/id.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/it.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/lo.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/lt.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/nl.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/pl.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/pt.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/ro.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/ru.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/sl.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/tr.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/uk.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/locale/zh_CN.po` & `trytond_sale_supply_drop_shipment-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/message.xml` & `trytond_sale_supply_drop_shipment-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/party.py` & `trytond_sale_supply_drop_shipment-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/product.py` & `trytond_sale_supply_drop_shipment-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/purchase.py` & `trytond_sale_supply_drop_shipment-6.8.0/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
     @fields.depends('product', 'template',
         '_parent_product.type', '_parent_product.supply_on_sale',
         '_parent_template.type', '_parent_template.supply_on_sale')
     def on_change_with_drop_shipment_available(self, name=None):
         product = self.product or self.template
         if product and product.type in {'goods', 'assets'}:
-            return product.supply_on_sale
+            return bool(product.supply_on_sale)
 
 
 class RequestCreatePurchase(metaclass=PoolMeta):
     __name__ = 'purchase.request.create_purchase'
 
     @classmethod
     def _group_purchase_key(cls, requests, request):
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/purchase.xml` & `trytond_sale_supply_drop_shipment-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/sale.py` & `trytond_sale_supply_drop_shipment-6.8.0/sale.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from trytond import backend
 from trytond.model import ModelSQL, ValueMixin, fields
 from trytond.modules.sale.sale import (
     get_shipments_returns, search_shipments_returns)
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 from trytond.tools.multivalue import migrate_property
-from trytond.transaction import Transaction
 
 sale_drop_location = fields.Many2One(
     'stock.location', "Sale Drop Location", domain=[('type', '=', 'drop')])
 
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'sale.configuration'
@@ -78,22 +77,21 @@
         if config.sale_drop_location:
             return config.sale_drop_location.id
 
     get_drop_shipments = get_shipments_returns('stock.shipment.drop')
     search_drop_shipments = search_shipments_returns('stock.shipment.drop')
 
     @classmethod
-    def _process_shipment(cls, sales):
+    def _process_supply(cls, sales, product_quantities):
         pool = Pool()
         Move = pool.get('stock.move')
-        super()._process_shipment(sales)
+        super()._process_supply(sales, product_quantities)
         moves = []
-        with Transaction().set_context(_drop_shipment=True):
-            for sale in sales:
-                moves.extend(sale.create_drop_shipment_moves())
+        for sale in sales:
+            moves.extend(sale.create_drop_shipment_moves())
         Move.save(moves)
 
     def create_drop_shipment_moves(self):
         moves = []
         for line in self.lines:
             moves += line.get_drop_moves()
         return moves
@@ -116,28 +114,26 @@
             return False
         if self.purchase_request and not self.purchase_request.customer:
             return False
         if self.supply_state == 'cancelled':
             return False
         if self.purchase_request:
             purchase_line = self.purchase_request.purchase_line
-            if purchase_line and purchase_line.move_done:
+            if purchase_line and purchase_line.moves_progress >= 1:
                 return False
         return True
 
     def get_move(self, shipment_type):
-        result = super().get_move(shipment_type)
-        if (shipment_type == 'out'
-                and not Transaction().context.get('_drop_shipment')):
-            if self.supply_on_sale_drop_move:
-                return
-        return result
+        move = super().get_move(shipment_type)
+        if self.supply_on_sale_drop_move and not self.purchase_request:
+            move = None
+        return move
 
-    def get_purchase_request(self):
-        request = super().get_purchase_request()
+    def get_purchase_request(self, product_quantities):
+        request = super().get_purchase_request(product_quantities)
         if request and request.party:
             if self.product and self.product.type in ('goods', 'assets'):
                 product_supplier = request.find_best_product_supplier(
                     self.product, self.shipping_date,
                     **self._get_purchase_request_product_supplier_pattern())
                 if product_supplier.drop_shipment:
                     request.customer = (
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/sale.xml` & `trytond_sale_supply_drop_shipment-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/setup.py` & `trytond_sale_supply_drop_shipment-6.8.0/setup.py`

 * *Files 6% similar despite different names*

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
@@ -34,39 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_supply_drop_shipment'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for sale supply drop shipment',
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
-            'https://hg.tryton.org/modules/sale_supply_drop_shipment'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale supply drop shipment',
     package_dir={'trytond.modules.sale_supply_drop_shipment': '.'},
     packages=(
         ['trytond.modules.sale_supply_drop_shipment']
         + ['trytond.modules.sale_supply_drop_shipment.%s' % p
             for p in find_packages()]
@@ -104,24 +103,24 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/stock.py` & `trytond_sale_supply_drop_shipment-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/stock.xml` & `trytond_sale_supply_drop_shipment-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/tests/scenario_sale_supply_drop_shipment.rst` & `trytond_sale_supply_drop_shipment-6.8.0/tests/scenario_sale_supply_drop_shipment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ==================================
 Sale Supply Drop Shipment Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_supply_drop_shipment',
     ...         'sale',
     ...         'purchase',
@@ -78,15 +78,15 @@
     >>> account_group, = Group.find([('name', '=', "Account")])
     >>> account_user.groups.append(account_group)
     >>> account_user.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> revenue = accounts['revenue']
@@ -119,25 +119,25 @@
     >>> template = ProductTemplate()
     >>> template.name = 'product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.purchasable = True
     >>> template.salable = True
     >>> template.list_price = Decimal('10')
-    >>> template.supply_on_sale = True
+    >>> template.supply_on_sale = 'always'
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
     >>> product.cost_price = Decimal('4')
     >>> product.save()
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = template
     >>> product_supplier.party = supplier
     >>> product_supplier.drop_shipment = True
-    >>> product_supplier.lead_time = datetime.timedelta(0)
+    >>> product_supplier.lead_time = dt.timedelta(0)
     >>> product_supplier.save()
 
 Create payment term::
 
     >>> payment_term = create_payment_term()
     >>> payment_term.save()
 
@@ -227,15 +227,15 @@
     2
 
 The purchase is now waiting for his new drop shipment::
 
     >>> set_user(purchase_user)
     >>> purchase.reload()
     >>> purchase.shipment_state
-    'waiting'
+    'partially shipped'
     >>> len(purchase.drop_shipments)
     2
     >>> shipment, = [s for s in purchase.drop_shipments
     ...     if s.state == 'waiting']
     >>> move, = shipment.customer_moves
     >>> move.quantity
     150.0
@@ -249,16 +249,15 @@
     >>> set_user(stock_user)
     >>> shipment.click('cancel')
 
     >>> set_user(purchase_user)
     >>> purchase.reload()
     >>> purchase.shipment_state
     'exception'
-    >>> handle_exception = Wizard('purchase.handle.shipment.exception',
-    ...     [purchase])
+    >>> handle_exception = purchase.click('handle_shipment_exception')
     >>> _ = handle_exception.form.recreate_moves.pop()
     >>> handle_exception.execute('handle')
     >>> purchase.reload()
     >>> purchase.shipment_state
     'received'
 
     >>> set_user(sale_user)
@@ -317,17 +316,16 @@
     >>> purchase, = Purchase.find([('state', '=', 'draft')])
     >>> purchase.click('cancel')
     >>> purchase_request.state
     'exception'
 
 Let's reset the purchase request and create a new purchase::
 
-    >>> handle_exception = Wizard(
-    ...     'purchase.request.handle.purchase.cancellation',
-    ...     [purchase_request])
+    >>> handle_exception = purchase_request.click(
+    ...     'handle_purchase_cancellation_exception')
     >>> handle_exception.execute('reset')
     >>> purchase_request.state
     'draft'
 
     >>> create_purchase = Wizard('purchase.request.create_purchase',
     ...     [purchase_request])
     >>> purchase, = Purchase.find([('state', '=', 'draft')])
@@ -337,28 +335,27 @@
 Let's cancel it again and cancel the request in order to manage the process on
 the sale::
 
     >>> purchase.click('cancel')
     >>> purchase_request.reload()
     >>> purchase_request.state
     'exception'
-    >>> handle_exception = Wizard(
-    ...     'purchase.request.handle.purchase.cancellation',
-    ...     [purchase_request])
+    >>> handle_exception = purchase_request.click(
+    ...     'handle_purchase_cancellation_exception')
     >>> handle_exception.execute('cancel_request')
     >>> purchase_request.state
     'cancelled'
 
 The sale is then in exception::
 
     >>> set_user(sale_user)
     >>> sale.reload()
     >>> sale.shipment_state
     'exception'
-    >>> handle_exception = Wizard('sale.handle.shipment.exception', [sale])
+    >>> handle_exception = sale.click('handle_shipment_exception')
     >>> handle_exception.execute('handle')
     >>> sale.reload()
     >>> sale.shipment_state
     'waiting'
 
 The sale just created a new outgoing shipment for the sale and we can deliver
 from stock::
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/tests/scenario_sale_supply_drop_shipment_on_invoice.rst` & `trytond_sale_supply_drop_shipment-6.8.0/tests/scenario_sale_supply_drop_shipment_on_invoice.rst`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     >>> template = ProductTemplate()
     >>> template.name = 'product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.purchasable = True
     >>> template.salable = True
     >>> template.list_price = Decimal('10')
-    >>> template.supply_on_sale = True
+    >>> template.supply_on_sale = 'always'
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = template
     >>> product_supplier.party = supplier
     >>> product_supplier.drop_shipment = True
@@ -111,15 +111,15 @@
     >>> sale_line.purchase_request
 
 Pay for 3 products::
 
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity = 3
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
 
 Not yet a purchase request::
 
     >>> sale.reload()
     >>> len(sale.shipments)
@@ -130,15 +130,15 @@
     >>> sale_line.purchase_request
 
 Pay for remaining products::
 
     >>> sale.reload()
     >>> _, invoice = sale.invoices
     >>> invoice.click('post')
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
 
 Check drop shipment::
 
     >>> sale.reload()
     >>> sale_line, = sale.lines
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst` & `trytond_sale_supply_drop_shipment-6.8.0/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ==================================
 Sale Supply Drop Shipment Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
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
     ...         'sale_supply_drop_shipment',
     ...         'sale',
     ...         'purchase',
@@ -70,23 +68,23 @@
     >>> template = ProductTemplate()
     >>> template.name = 'product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.purchasable = True
     >>> template.salable = True
     >>> template.list_price = Decimal('10')
-    >>> template.supply_on_sale = True
+    >>> template.supply_on_sale = 'always'
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = template
     >>> product_supplier.party = supplier
     >>> product_supplier.drop_shipment = True
-    >>> product_supplier.lead_time = datetime.timedelta(0)
+    >>> product_supplier.lead_time = dt.timedelta(0)
     >>> product_supplier.save()
 
 Create payment term::
 
     >>> payment_term = create_payment_term()
     >>> payment_term.save()
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO` & `trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-supply-drop-shipment
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for sale supply drop shipment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_supply_drop_shipment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale supply drop shipment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,33 +38,33 @@
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
 
 Sale Supply Drop Shipment Model
 ###############################
 
 The Sale Supply Drop Shipment module adds a drop shipment option on product
-supplier if "supply on request" is checked. When checked, the purchase request
-and the linked purchase have the address of customer as Delivery Address;
-at the confirmation of the purchase a drop shipment is created and linked to
-both the purchase and the sale.
+supplier if "supply on request" is selected.
+When selected, the purchase request and the linked purchase have the address of
+customer as Delivery Address; at the confirmation of the purchase a drop
+shipment is created and linked to both the purchase and the sale.
 
 Drop Shipment
 *************
 
 A drop shipment is used when products are sent directly from the supplier to
 the customer without going through the warehouse.
 It is mainly composed of a supplier, a customer and a list of moves.
```

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt` & `trytond_sale_supply_drop_shipment-6.8.0/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/view/purchase_form.xml` & `trytond_sale_supply_drop_shipment-6.8.0/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/view/sale_form.xml` & `trytond_sale_supply_drop_shipment-6.8.0/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/view/shipment_drop_form.xml` & `trytond_sale_supply_drop_shipment-6.8.0/view/shipment_drop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-6.6.3/view/shipment_drop_tree.xml` & `trytond_sale_supply_drop_shipment-6.8.0/view/shipment_drop_tree.xml`

 * *Files identical despite different names*

