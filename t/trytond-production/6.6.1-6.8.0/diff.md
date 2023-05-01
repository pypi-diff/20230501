# Comparing `tmp/trytond_production-6.6.1.tar.gz` & `tmp/trytond_production-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production-6.6.1.tar", last modified: Sat Mar  4 11:51:10 2023, max compression
+gzip compressed data, was "trytond_production-6.8.0.tar", last modified: Mon May  1 11:42:56 2023, max compression
```

## Comparing `trytond_production-6.6.1.tar` & `trytond_production-6.8.0.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:10.036120 trytond_production-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2963 2023-03-04 11:51:03.000000 trytond_production-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-03-04 11:51:03.000000 trytond_production-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_production-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:50.000000 trytond_production-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4030 2023-03-04 11:51:10.036120 trytond_production-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2022-12-19 12:02:50.000000 trytond_production-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1010 2022-12-19 12:02:50.000000 trytond_production-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9153 2022-12-19 12:02:50.000000 trytond_production-6.6.1/bom.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6296 2022-12-19 12:02:50.000000 trytond_production-6.6.1/bom.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2516 2022-12-19 12:02:50.000000 trytond_production-6.6.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2122 2022-12-19 12:02:50.000000 trytond_production-6.6.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:10.016120 trytond_production-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:50.000000 trytond_production-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2022-12-19 12:02:50.000000 trytond_production-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2022-12-19 12:02:50.000000 trytond_production-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:10.019453 trytond_production-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:50.000000 trytond_production-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2022-12-19 12:02:50.000000 trytond_production-6.6.1/icons/tryton-production.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      574 2022-12-19 12:02:50.000000 trytond_production-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:09.959452 trytond_production-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14462 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14089 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12520 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14097 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13965 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11672 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13075 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14305 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12507 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14091 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13183 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12117 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13679 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14182 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12593 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13850 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13055 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13607 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11941 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14485 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13471 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13409 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11655 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12575 2022-12-19 12:02:50.000000 trytond_production-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      811 2022-12-19 12:02:50.000000 trytond_production-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4134 2023-02-23 20:43:10.000000 trytond_production-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4276 2022-12-19 12:02:50.000000 trytond_production-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    30939 2023-02-27 17:40:00.000000 trytond_production-6.6.1/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14686 2022-12-19 12:02:50.000000 trytond_production-6.6.1/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:51:10.036120 trytond_production-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4386 2022-12-19 12:02:50.000000 trytond_production-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5958 2022-12-19 12:02:50.000000 trytond_production-6.6.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1940 2022-12-19 12:02:50.000000 trytond_production-6.6.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:09.976119 trytond_production-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7188 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/scenario_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/scenario_production_by_product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2179 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/scenario_production_no_list_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2475 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/scenario_production_rounding.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3160 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/scenario_production_set_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2947 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/scenario_production_waste.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1401 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2022-12-19 12:02:50.000000 trytond_production-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2022-12-19 12:03:07.000000 trytond_production-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:10.032786 trytond_production-6.6.1/trytond_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4030 2023-03-04 11:51:08.000000 trytond_production-6.6.1/trytond_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3472 2023-03-04 11:51:09.000000 trytond_production-6.6.1/trytond_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:51:08.000000 trytond_production-6.6.1/trytond_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-03-04 11:51:08.000000 trytond_production-6.6.1/trytond_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:51:08.000000 trytond_production-6.6.1/trytond_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      136 2023-03-04 11:51:08.000000 trytond_production-6.6.1/trytond_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:51:08.000000 trytond_production-6.6.1/trytond_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:51:10.012786 trytond_production-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_input_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_input_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_output_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_output_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_tree_open_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_tree_open_tree_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/bom_tree_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/product_bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/product_bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/product_bom_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/production_calendar.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/production_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/production_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/production_lead_time_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2022-12-19 12:02:50.000000 trytond_production-6.6.1/view/template_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.570078 trytond_production-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3168 2023-05-01 11:02:05.000000 trytond_production-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:02:04.000000 trytond_production-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4027 2023-05-01 11:42:56.570078 trytond_production-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-04-15 07:12:15.000000 trytond_production-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-04-15 07:12:15.000000 trytond_production-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9147 2023-04-21 08:36:08.000000 trytond_production-6.8.0/bom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6296 2023-04-15 07:12:15.000000 trytond_production-6.8.0/bom.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2516 2023-04-15 07:12:15.000000 trytond_production-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2122 2023-04-15 07:12:15.000000 trytond_production-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.566744 trytond_production-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_production-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-04-15 07:12:15.000000 trytond_production-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-04-15 07:12:15.000000 trytond_production-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.566744 trytond_production-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_production-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-01-16 14:00:20.000000 trytond_production-6.8.0/icons/tryton-production.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-04-15 07:12:15.000000 trytond_production-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.556744 trytond_production-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14473 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14100 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12531 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14108 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13977 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11683 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13095 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14325 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12518 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14099 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13194 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12128 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13699 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14193 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12604 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13863 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13066 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13627 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11952 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14496 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13491 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13429 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11666 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12586 2023-04-30 10:46:36.000000 trytond_production-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-04-15 07:12:15.000000 trytond_production-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4297 2023-04-15 07:12:15.000000 trytond_production-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4276 2023-01-16 14:00:21.000000 trytond_production-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    31523 2023-04-21 08:36:08.000000 trytond_production-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14686 2023-04-15 07:12:15.000000 trytond_production-6.8.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:56.570078 trytond_production-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4412 2023-04-15 07:12:15.000000 trytond_production-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5952 2023-04-21 08:36:08.000000 trytond_production-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1940 2023-04-15 07:12:15.000000 trytond_production-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.563411 trytond_production-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7217 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2745 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production_by_product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2030 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2179 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production_no_list_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2475 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production_rounding.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3160 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production_set_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2947 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/scenario_production_waste.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1423 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_production-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-05-01 11:01:59.000000 trytond_production-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.570078 trytond_production-6.8.0/trytond_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4027 2023-05-01 11:42:55.000000 trytond_production-6.8.0/trytond_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3556 2023-05-01 11:42:56.000000 trytond_production-6.8.0/trytond_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:55.000000 trytond_production-6.8.0/trytond_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:42:55.000000 trytond_production-6.8.0/trytond_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_production-6.8.0/trytond_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 11:42:55.000000 trytond_production-6.8.0/trytond_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:55.000000 trytond_production-6.8.0/trytond_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:56.566744 trytond_production-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/bom_input_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/bom_input_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-01-16 14:00:20.000000 trytond_production-6.8.0/view/bom_output_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/bom_output_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-01-16 14:00:20.000000 trytond_production-6.8.0/view/bom_tree_open_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/bom_tree_open_tree_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/bom_tree_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/product_bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_production-6.8.0/view/product_bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_production-6.8.0/view/product_bom_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/production_calendar.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/production_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-01-16 14:00:21.000000 trytond_production-6.8.0/view/production_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/production_lead_time_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_production-6.8.0/view/template_list.xml
```

### Comparing `trytond_production-6.6.1/CHANGELOG` & `trytond_production-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Rename product lead times to production lead times
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Create lot for output product when needed
+* Assign all possible productions when trying
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_production-6.6.1/COPYRIGHT` & `trytond_production-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2012-2022 Cédric Krier.
-Copyright (C) 2012-2022 B2CK SPRL.
+Copyright (C) 2012-2023 Cédric Krier.
+Copyright (C) 2012-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_production-6.6.1/LICENSE` & `trytond_production-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/PKG-INFO` & `trytond_production-6.8.0/trytond_production.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_production
-Version: 6.6.1
+Name: trytond-production
+Version: 6.8.0
 Summary: Tryton module for production
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production
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
 
 Production Module
 #################
 
 The production module defines basics for production management: Bill of
```

### Comparing `trytond_production-6.6.1/README.rst` & `trytond_production-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/__init__.py` & `trytond_production-6.8.0/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,11 +24,12 @@
         stock.Location,
         stock.Move,
         stock.ProductQuantitiesByWarehouseMove,
         ir.Cron,
         module='production', type_='model')
     Pool.register(
         stock.LotTrace,
+        production.Production_Lot,
         module='production', type_='model', depends=['stock_lot'])
     Pool.register(
         bom.OpenBOMTree,
         module='production', type_='wizard')
```

### Comparing `trytond_production-6.6.1/bom.py` & `trytond_production-6.8.0/bom.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,15 @@
             if not self.uom or self.uom.category != category:
                 self.uom = self.product.default_uom
         else:
             self.uom = None
 
     @fields.depends('product')
     def on_change_with_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom.category.id
+        return self.product.default_uom.category if self.product else None
 
     def get_rec_name(self, name):
         return self.product.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('product.rec_name',) + tuple(clause[1:])]
```

### Comparing `trytond_production-6.6.1/bom.xml` & `trytond_production-6.8.0/bom.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/configuration.py` & `trytond_production-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/configuration.xml` & `trytond_production-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/doc/conf.py` & `trytond_production-6.8.0/doc/conf.py`

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

### Comparing `trytond_production-6.6.1/doc/index.rst` & `trytond_production-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/icons/LICENSE` & `trytond_production-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/ir.py` & `trytond_production-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/locale/bg.po` & `trytond_production-6.8.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Спецификации"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Спецификация"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Продукт"
```

### Comparing `trytond_production-6.6.1/locale/ca.po` & `trytond_production-6.8.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Llistes de materials"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Temps d'espera"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Produïble"
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Temps d'espera"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Llista de materials"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Producte"
```

### Comparing `trytond_production-6.6.1/locale/cs.po` & `trytond_production-6.8.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
```

### Comparing `trytond_production-6.6.1/locale/de.po` & `trytond_production-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Stücklisten"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Beschaffungszeiten"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Produzierbar"
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Beschaffungszeiten"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Stückliste"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Artikel"
```

### Comparing `trytond_production-6.6.1/locale/es.po` & `trytond_production-6.8.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "LdM"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Tiempo de espera"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Producible"
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Tiempos de espera"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "LdM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Producto"
```

### Comparing `trytond_production-6.6.1/locale/es_419.po` & `trytond_production-6.8.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr ""
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr ""
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr ""
```

### Comparing `trytond_production-6.6.1/locale/et.po` & `trytond_production-6.8.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Retseptid"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Viiteaeg"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Toodetav"
 
+#, fuzzy
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Viiteaeg"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Retsept"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Toode"
```

### Comparing `trytond_production-6.6.1/locale/fa.po` & `trytond_production-6.8.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "زمان پیشبرد"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "قابل توليد"
 
+#, fuzzy
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "زمان پیشبرد"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "محصول"
```

### Comparing `trytond_production-6.6.1/locale/fi.po` & `trytond_production-6.8.0/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
```

### Comparing `trytond_production-6.6.1/locale/fr.po` & `trytond_production-6.8.0/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Nomenclatures"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Délais de production"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Productible"
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Délais de production"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Nomenclature"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Produit"
@@ -96,15 +96,15 @@
 
 msgctxt "field:production,reference:"
 msgid "Reference"
 msgstr "Référence"
 
 msgctxt "field:production,run_by:"
 msgid "Run By"
-msgstr "Exécutée par"
+msgstr "Lancée par"
 
 msgctxt "field:production,state:"
 msgid "State"
 msgstr "État"
 
 msgctxt "field:production,uom:"
 msgid "Uom"
```

### Comparing `trytond_production-6.6.1/locale/hu.po` & `trytond_production-6.8.0/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 #, fuzzy
 msgctxt "field:product.product-production.bom,product:"
```

### Comparing `trytond_production-6.6.1/locale/id.po` & `trytond_production-6.8.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr ""
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr ""
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Produk"
```

### Comparing `trytond_production-6.6.1/locale/it.po` & `trytond_production-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Distinte materiali"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Tempi di consegna"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Producible"
 
+#, fuzzy
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Tempi di consegna"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Distinta materiali"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Prodotto"
```

### Comparing `trytond_production-6.6.1/locale/lo.po` & `trytond_production-6.8.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
```

### Comparing `trytond_production-6.6.1/locale/lt.po` & `trytond_production-6.8.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
```

### Comparing `trytond_production-6.6.1/locale/nl.po` & `trytond_production-6.8.0/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "stuklijsten"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Doorlooptijd"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "produceerbaar"
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Doorlooptijden"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "stuklijst"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Product"
```

### Comparing `trytond_production-6.6.1/locale/pl.po` & `trytond_production-6.8.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMy"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Produkt"
```

### Comparing `trytond_production-6.6.1/locale/pt.po` & `trytond_production-6.8.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Listas de Materiais"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Tempo de Espera"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Produzível"
 
+#, fuzzy
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Tempo de Espera"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Lista de Materiais"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Produto"
```

### Comparing `trytond_production-6.6.1/locale/ro.po` & `trytond_production-6.8.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr ""
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr ""
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Produs"
```

### Comparing `trytond_production-6.6.1/locale/ru.po` & `trytond_production-6.8.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Спецификации"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Спецификация"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Продукт"
```

### Comparing `trytond_production-6.6.1/locale/sl.po` & `trytond_production-6.8.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "Kosovnice"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Dobavni roki"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Se proizvaja"
 
+#, fuzzy
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Dobavni roki"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "Kosovnica"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Izdelek"
```

### Comparing `trytond_production-6.6.1/locale/tr.po` & `trytond_production-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMlar"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr "Tedarik Süreleri"
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr "Üretilebilir"
 
+#, fuzzy
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr "Tedarik Süreleri"
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr "Ürün"
```

### Comparing `trytond_production-6.6.1/locale/uk.po` & `trytond_production-6.8.0/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr ""
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr ""
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
 msgstr ""
```

### Comparing `trytond_production-6.6.1/locale/zh_CN.po` & `trytond_production-6.8.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
 msgstr "BOMs"
 
-msgctxt "field:product.product,lead_times:"
-msgid "Lead Times"
-msgstr ""
-
 msgctxt "field:product.product,producible:"
 msgid "Producible"
 msgstr ""
 
+msgctxt "field:product.product,production_lead_times:"
+msgid "Lead Times"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
```

### Comparing `trytond_production-6.6.1/message.xml` & `trytond_production-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/product.py` & `trytond_production-6.8.0/product.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.i18n import gettext
 from trytond.model import (
     MatchMixin, ModelSQL, ModelView, fields, sequence_ordered)
 from trytond.model.exceptions import RecursionError
 from trytond.pool import PoolMeta
-from trytond.pyson import Bool, Eval, Get, If
+from trytond.pyson import Bool, Eval, Get, If, TimeDelta
 
 
 class Template(metaclass=PoolMeta):
     __name__ = 'product.template'
     producible = fields.Boolean("Producible")
 
     @classmethod
@@ -35,15 +35,15 @@
     __name__ = 'product.product'
 
     boms = fields.One2Many('product.product-production.bom', 'product',
         'BOMs', order=[('sequence', 'ASC'), ('id', 'ASC')],
         states={
             'invisible': ~Eval('producible')
             })
-    lead_times = fields.One2Many('production.lead_time',
+    production_lead_times = fields.One2Many('production.lead_time',
         'product', 'Lead Times', order=[('sequence', 'ASC'), ('id', 'ASC')],
         states={
             'invisible': ~Eval('producible'),
             })
 
     @classmethod
     def validate(cls, products):
@@ -69,15 +69,15 @@
     @classmethod
     def copy(cls, products, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('boms', None)
-        default.setdefault('lead_times', None)
+        default.setdefault('production_lead_times', None)
         return super(Product, cls).copy(products, default=default)
 
 
 class ProductBom(sequence_ordered(), ModelSQL, ModelView):
     'Product - BOM'
     __name__ = 'product.product-production.bom'
 
@@ -113,13 +113,18 @@
             ])
     bom = fields.Many2One('production.bom', 'BOM', ondelete='CASCADE',
         domain=[
             ('output_products', '=', If(Bool(Eval('product')),
                     Eval('product', -1),
                     Get(Eval('_parent_product', {}), 'id', 0))),
             ])
-    lead_time = fields.TimeDelta('Lead Time')
+    lead_time = fields.TimeDelta(
+        "Lead Time",
+        domain=['OR',
+            ('lead_time', '=', None),
+            ('lead_time', '>=', TimeDelta()),
+            ])
 
     @classmethod
     def __setup__(cls):
         super(ProductionLeadTime, cls).__setup__()
         cls._order.insert(0, ('product', 'ASC'))
```

### Comparing `trytond_production-6.6.1/product.xml` & `trytond_production-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/production.py` & `trytond_production-6.8.0/production.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 
 from trytond.i18n import gettext
 from trytond.model import (
     Index, ModelSQL, ModelView, Workflow, dualmethod, fields)
 from trytond.modules.company.model import employee_field, set_employee
 from trytond.modules.product import price_digits, round_price
 from trytond.modules.stock.shipment import ShipmentAssignMixin
-from trytond.pool import Pool
+from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, If
 from trytond.transaction import Transaction
 
 from .exceptions import CostWarning
 
-BOM_CHANGES = ['bom', 'product', 'quantity', 'uom', 'warehouse', 'location',
-    'company', 'inputs', 'outputs']
-
 
 class Production(ShipmentAssignMixin, Workflow, ModelSQL, ModelView):
     "Production"
     __name__ = 'production'
     _rec_name = 'number'
     _assign_moves_field = 'inputs'
 
@@ -321,15 +318,15 @@
 
     @fields.depends('product', 'bom')
     def compute_lead_time(self, pattern=None):
         if pattern is None:
             pattern = {}
         if self.product:
             pattern.setdefault('bom', self.bom.id if self.bom else None)
-            for line in self.product.lead_times:
+            for line in self.product.production_lead_times:
                 if line.match(pattern):
                     return line.lead_time or timedelta()
         return timedelta()
 
     @fields.depends('planned_date', methods=['compute_lead_time'])
     def on_change_with_planned_start_date(self, pattern=None):
         if self.planned_date and self.product:
@@ -353,65 +350,67 @@
     @classmethod
     def get_origin(cls):
         Model = Pool().get('ir.model')
         get_name = Model.get_name
         models = cls._get_origin()
         return [(None, '')] + [(m, get_name(m)) for m in models]
 
-    def _move(self, from_location, to_location, company, product, uom,
-            quantity):
-        Move = Pool().get('stock.move')
+    @fields.depends(
+        'company', 'location', methods=['picking_location', 'output_location'])
+    def _move(self, type, product, uom, quantity):
+        pool = Pool()
+        Move = pool.get('stock.move')
+        assert type in {'input', 'output'}
         move = Move(
             product=product,
             uom=uom,
             quantity=quantity,
-            from_location=from_location,
-            to_location=to_location,
-            company=company,
-            currency=company.currency if company else None,
-            state='draft',
-            )
+            company=self.company,
+            currency=self.company.currency if self.company else None)
+        if type == 'input':
+            move.from_location = self.picking_location
+            move.to_location = self.location
+            move.production_input = self
+        else:
+            move.from_location = self.location
+            move.to_location = self.output_location
+            move.production_output = self
         return move
 
-    def _explode_move_values(self, from_location, to_location, company,
-            bom_io, quantity):
-        move = self._move(from_location, to_location, company,
-            bom_io.product, bom_io.uom, quantity)
-        move.from_location = from_location.id if from_location else None
-        move.to_location = to_location.id if to_location else None
+    @fields.depends(methods=['_move'])
+    def _explode_move_values(self, type, bom_io, quantity):
+        move = self._move(type, bom_io.product, bom_io.uom, quantity)
         move.unit_price_required = move.on_change_with_unit_price_required()
         return move
 
-    @fields.depends(*BOM_CHANGES)
+    @fields.depends(
+        'bom', 'product', 'uom', 'quantity', 'company', 'inputs', 'outputs',
+        methods=['_explode_move_values'])
     def explode_bom(self):
         pool = Pool()
         Uom = pool.get('product.uom')
         if not (self.bom and self.product and self.uom):
             return
 
         factor = self.bom.compute_factor(self.product, self.quantity or 0,
             self.uom)
         inputs = []
         for input_ in self.bom.inputs:
             quantity = input_.compute_quantity(factor)
-            move = self._explode_move_values(
-                self.picking_location, self.location, self.company,
-                input_, quantity)
+            move = self._explode_move_values('input', input_, quantity)
             if move:
                 inputs.append(move)
                 quantity = Uom.compute_qty(input_.uom, quantity,
                     input_.product.default_uom, round=False)
         self.inputs = inputs
 
         outputs = []
         for output in self.bom.outputs:
             quantity = output.compute_quantity(factor)
-            move = self._explode_move_values(
-                self.location, self.output_location, self.company, output,
-                quantity)
+            move = self._explode_move_values('output', output, quantity)
             if move:
                 move.unit_price = Decimal(0)
                 move.currency = self.company.currency
                 outputs.append(move)
         self.outputs = outputs
 
     @fields.depends('warehouse')
@@ -429,16 +428,15 @@
         else:
             self.bom = None
             self.uom = None
         self.explode_bom()
 
     @fields.depends('product')
     def on_change_with_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom.category.id
+        return self.product.default_uom.category if self.product else None
 
     @fields.depends(methods=['explode_bom'])
     def on_change_bom(self):
         self.explode_bom()
 
     @fields.depends(methods=['explode_bom'])
     def on_change_uom(self):
@@ -453,18 +451,15 @@
         self.explode_bom()
 
     def get_cost(self, name):
         cost = Decimal(0)
         for input_ in self.inputs:
             if input_.state == 'cancelled':
                 continue
-            if input_.cost_price is not None:
-                cost_price = input_.cost_price
-            else:
-                cost_price = input_.product.cost_price
+            cost_price = input_.get_cost_price()
             cost += (Decimal(str(input_.internal_quantity)) * cost_price)
         return round_price(cost)
 
     @fields.depends('inputs')
     def on_change_with_cost(self):
         Uom = Pool().get('product.uom')
 
@@ -486,49 +481,41 @@
 
     @dualmethod
     def set_moves(cls, productions):
         pool = Pool()
         Move = pool.get('stock.move')
         to_save = []
         for production in productions:
-            location = production.location
-            company = production.company
-
             if not production.bom:
                 if production.product:
                     move = production._move(
-                        location, production.output_location, company,
-                        production.product, production.uom,
+                        'output', production.product, production.uom,
                         production.quantity)
                     if move:
-                        move.production_output = production
                         move.unit_price = Decimal(0)
                         move.currency = production.company.currency
                         to_save.append(move)
                 continue
 
             factor = production.bom.compute_factor(
                 production.product, production.quantity, production.uom)
             for input_ in production.bom.inputs:
                 quantity = input_.compute_quantity(factor)
                 product = input_.product
                 move = production._move(
-                    production.picking_location, location, company, product,
-                    input_.uom, quantity)
+                    'input', product, input_.uom, quantity)
                 if move:
-                    move.production_input = production
                     to_save.append(move)
 
             for output in production.bom.outputs:
                 quantity = output.compute_quantity(factor)
                 product = output.product
-                move = production._move(location, production.output_location,
-                    company, product, output.uom, quantity)
+                move = production._move(
+                    'output', product, output.uom, quantity)
                 if move:
-                    move.production_output = production
                     move.unit_price = Decimal(0)
                     move.currency = production.company.currency
                     to_save.append(move)
         Move.save(to_save)
         cls._set_move_planned_date(productions)
 
     @classmethod
@@ -561,18 +548,15 @@
             cost = production.cost
 
             input_quantities = defaultdict(Decimal)
             input_costs = defaultdict(Decimal)
             for input_ in production.inputs:
                 if input_.state == 'cancelled':
                     continue
-                if input_.cost_price is not None:
-                    cost_price = input_.cost_price
-                else:
-                    cost_price = input_.product.cost_price
+                cost_price = input_.get_cost_price()
                 input_quantities[input_.product] += (
                     Decimal(str(input_.internal_quantity)))
                 input_costs[input_.product] += (
                     Decimal(str(input_.internal_quantity)) * cost_price)
             outputs = []
             for output in production.outputs:
                 if (output.to_location.type == 'lost_found'
@@ -790,20 +774,30 @@
         pass
 
     @dualmethod
     @ModelView.button
     def assign_try(cls, productions):
         pool = Pool()
         Move = pool.get('stock.move')
-        if Move.assign_try(
-                [m for p in productions for m in p.assign_moves]):
+        to_assign = [
+            m for p in productions for m in p.assign_moves
+            if m.assignation_required]
+        if Move.assign_try(to_assign):
             cls.assign(productions)
-            return True
         else:
-            return False
+            to_assign = []
+            for production in productions:
+                if any(
+                        m.state in {'staging', 'draft'}
+                        for m in production.assign_moves
+                        if m.assignation_required):
+                    continue
+                to_assign.append(production)
+            if to_assign:
+                cls.assign(to_assign)
 
     @classmethod
     def _get_reschedule_domain(cls, date):
         context = Transaction().context
         return [
             ('company', '=', context.get('company')),
             ('state', '=', 'waiting'),
@@ -819,17 +813,43 @@
         productions = cls.search(cls._get_reschedule_domain(date))
         for production in productions:
             production.planned_start_date = date
             production.on_change_planned_start_date()
         cls.save(productions)
 
     @property
+    @fields.depends('warehouse')
     def picking_location(self):
         if self.warehouse:
             return (self.warehouse.production_picking_location
                 or self.warehouse.storage_location)
 
     @property
+    @fields.depends('warehouse')
     def output_location(self):
         if self.warehouse:
             return (self.warehouse.production_output_location
                 or self.warehouse.storage_location)
+
+
+class Production_Lot(metaclass=PoolMeta):
+    __name__ = 'production'
+
+    @classmethod
+    @ModelView.button
+    @Workflow.transition('done')
+    def done(cls, productions):
+        pool = Pool()
+        Lot = pool.get('stock.lot')
+        Move = pool.get('stock.move')
+        lots, moves = [], []
+        for production in productions:
+            for move in production.outputs:
+                if not move.lot and move.product.lot_is_required(
+                        move.from_location, move.to_location):
+                    move.add_lot()
+                    if move.lot:
+                        lots.append(move.lot)
+                        moves.append(move)
+        Lot.save(lots)
+        Move.save(moves)
+        super().done(productions)
```

### Comparing `trytond_production-6.6.1/production.xml` & `trytond_production-6.8.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/setup.py` & `trytond_production-6.8.0/setup.py`

 * *Files 5% similar despite different names*

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
@@ -34,38 +31,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_production'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond_stock_lot'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module for production',
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
-        "Source Code": 'https://hg.tryton.org/modules/production',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton production',
     package_dir={'trytond.modules.production': '.'},
     packages=(
         ['trytond.modules.production']
         + ['trytond.modules.production.%s' % p for p in find_packages()]
         ),
@@ -103,23 +106,23 @@
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

### Comparing `trytond_production-6.6.1/stock.py` & `trytond_production-6.8.0/stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,17 @@
             ]
 
     @fields.depends(
         'production_input', '_parent_production_input.id',
         'production_output', '_parent_production_output.id')
     def on_change_with_production(self, name=None):
         if self.production_input:
-            return self.production_input.id
+            return self.production_input
         elif self.production_output:
-            return self.production_output.id
+            return self.production_output
 
     def set_effective_date(self):
         if not self.effective_date and self.production_input:
             self.effective_date = self.production_input.effective_start_date
         if not self.effective_date and self.production_output:
             self.effective_date = self.production_output.effective_date
         super(Move, self).set_effective_date()
```

### Comparing `trytond_production-6.6.1/stock.xml` & `trytond_production-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/tests/scenario_production.rst` & `trytond_production-6.8.0/tests/scenario_production.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ===================
 Production Scenario
 ===================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> from trytond.modules.production.production import BOM_CHANGES
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
-    >>> before_yesterday = yesterday - relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
+    >>> before_yesterday = yesterday - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('production')
 
 Create company::
 
@@ -93,15 +92,15 @@
     >>> product.boms.append(ProductBom(bom=bom))
     >>> product.save()
 
     >>> ProductionLeadTime = Model.get('production.lead_time')
     >>> production_lead_time = ProductionLeadTime()
     >>> production_lead_time.product = product
     >>> production_lead_time.bom = bom
-    >>> production_lead_time.lead_time = datetime.timedelta(1)
+    >>> production_lead_time.lead_time = dt.timedelta(1)
     >>> production_lead_time.save()
 
 Create an Inventory::
 
     >>> Inventory = Model.get('stock.inventory')
     >>> InventoryLine = Model.get('stock.inventory.line')
     >>> Location = Model.get('stock.location')
@@ -144,25 +143,30 @@
     >>> production.state
     'waiting'
 
 Test reset bom button::
 
     >>> for input in production.inputs:
     ...     input.quantity += 1
-    >>> production.click('reset_bom', change=BOM_CHANGES)
+    >>> production.click(
+    ...     'reset_bom',
+    ...     change=[
+    ...         'bom', 'product', 'uom', 'quantity',
+    ...         'inputs', 'outputs', 'company', 'warehouse', 'location'])
     >>> sorted([i.quantity for i in production.inputs]) == [10, 300]
     True
     >>> output, = production.outputs
     >>> output.quantity == 2
     True
 
 Do the production::
 
     >>> production.click('assign_try')
-    True
+    >>> production.state
+    'assigned'
     >>> all(i.state == 'assigned' for i in production.inputs)
     True
     >>> production.click('run')
     >>> all(i.state == 'done' for i in production.inputs)
     True
     >>> len(set(i.effective_date == today for i in production.inputs))
     1
@@ -185,15 +189,14 @@
     >>> production.effective_date = yesterday
     >>> production.effective_start_date = before_yesterday
     >>> production.product = product
     >>> production.bom = bom
     >>> production.quantity = 2
     >>> production.click('wait')
     >>> production.click('assign_try')
-    True
     >>> production.click('run')
     >>> production.reload()
     >>> all(i.effective_date == before_yesterday for i in production.inputs)
     True
     >>> production.click('done')
     >>> production.reload()
     >>> output, = production.outputs
```

### Comparing `trytond_production-6.6.1/tests/scenario_production_by_product.rst` & `trytond_production-6.8.0/tests/scenario_production_by_product.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/tests/scenario_production_no_list_price.rst` & `trytond_production-6.8.0/tests/scenario_production_no_list_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/tests/scenario_production_rounding.rst` & `trytond_production-6.8.0/tests/scenario_production_rounding.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/tests/scenario_production_set_cost.rst` & `trytond_production-6.8.0/tests/scenario_production_set_cost.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/tests/scenario_production_waste.rst` & `trytond_production-6.8.0/tests/scenario_production_waste.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/tests/test_module.py` & `trytond_production-6.8.0/tests/test_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,23 +17,23 @@
         pool = Pool()
         Production = pool.get('production')
         Product = pool.get('product.product')
         LeadTime = pool.get('production.lead_time')
 
         date = datetime.date(2016, 11, 26)
         product = Product()
-        product.lead_times = []
+        product.production_lead_times = []
         production = Production()
         production.planned_date = date
         production.product = product
 
         self.assertEqual(production.on_change_with_planned_start_date(), date)
 
         lead_time = LeadTime(bom=None, lead_time=None)
-        product.lead_times = [lead_time]
+        product.production_lead_times = [lead_time]
         self.assertEqual(production.on_change_with_planned_start_date(), date)
 
         lead_time.lead_time = datetime.timedelta(1)
         self.assertEqual(
             production.on_change_with_planned_start_date(),
             datetime.date(2016, 11, 25))
```

### Comparing `trytond_production-6.6.1/tox.ini` & `trytond_production-6.8.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/production/* -m unittest discover -s tests
-    coverage report --include=./**/production/* --omit=*/tests/*
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

### Comparing `trytond_production-6.6.1/trytond_production.egg-info/PKG-INFO` & `trytond_production-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-production
-Version: 6.6.1
+Name: trytond_production
+Version: 6.8.0
 Summary: Tryton module for production
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production
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
 
 Production Module
 #################
 
 The production module defines basics for production management: Bill of
```

### Comparing `trytond_production-6.6.1/trytond_production.egg-info/SOURCES.txt` & `trytond_production-6.8.0/trytond_production.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_production.rst
 ./tests/scenario_production_by_product.rst
+./tests/scenario_production_lot_number.rst
 ./tests/scenario_production_no_list_price.rst
 ./tests/scenario_production_rounding.rst
 ./tests/scenario_production_set_cost.rst
 ./tests/scenario_production_waste.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/bom_form.xml
@@ -120,14 +121,15 @@
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_production.rst
 tests/scenario_production_by_product.rst
+tests/scenario_production_lot_number.rst
 tests/scenario_production_no_list_price.rst
 tests/scenario_production_rounding.rst
 tests/scenario_production_set_cost.rst
 tests/scenario_production_waste.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_production.egg-info/PKG-INFO
```

### Comparing `trytond_production-6.6.1/view/location_form.xml` & `trytond_production-6.8.0/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/view/production_form.xml` & `trytond_production-6.8.0/view/production_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/view/production_list.xml` & `trytond_production-6.8.0/view/production_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-6.6.1/view/template_form.xml` & `trytond_production-6.8.0/view/template_form.xml`

 * *Files identical despite different names*

