# Comparing `tmp/trytond_product-6.6.1.tar.gz` & `tmp/trytond_product-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product-6.6.1.tar", last modified: Sat Apr  1 22:15:51 2023, max compression
+gzip compressed data, was "trytond_product-6.8.0.tar", last modified: Mon May  1 11:57:31 2023, max compression
```

## Comparing `trytond_product-6.6.1.tar` & `trytond_product-6.8.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.586811 trytond_product-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     4938 2023-04-01 22:15:46.000000 trytond_product-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-04-01 22:15:46.000000 trytond_product-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_product-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:50.000000 trytond_product-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2542 2023-04-01 22:15:51.586811 trytond_product-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-12-19 12:02:49.000000 trytond_product-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2022-12-19 12:02:49.000000 trytond_product-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-03-26 09:50:14.000000 trytond_product-6.6.1/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4839 2022-12-19 12:02:49.000000 trytond_product-6.6.1/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2747 2022-12-19 12:02:49.000000 trytond_product-6.6.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2558 2022-12-19 12:02:49.000000 trytond_product-6.6.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.576811 trytond_product-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:50.000000 trytond_product-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-12-19 12:02:50.000000 trytond_product-6.6.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5540 2022-12-19 12:02:49.000000 trytond_product-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-12-19 12:02:49.000000 trytond_product-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:49.000000 trytond_product-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2539 2022-12-19 12:02:49.000000 trytond_product-6.6.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2022-12-19 12:02:49.000000 trytond_product-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.576811 trytond_product-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:49.000000 trytond_product-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2022-12-19 12:02:50.000000 trytond_product-6.6.1/icons/tryton-product.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2022-12-19 12:02:50.000000 trytond_product-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.556810 trytond_product-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    24191 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25528 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21626 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26040 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25767 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21685 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22233 2022-12-19 12:02:50.000000 trytond_product-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23573 2022-12-19 12:02:50.000000 trytond_product-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21561 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25716 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24311 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21350 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22384 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24649 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23328 2022-12-19 12:02:50.000000 trytond_product-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25655 2022-12-19 12:02:50.000000 trytond_product-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25421 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22785 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25194 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24435 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22972 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22893 2022-12-19 12:02:49.000000 trytond_product-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20611 2022-12-19 12:02:50.000000 trytond_product-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24271 2022-12-19 12:02:50.000000 trytond_product-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2022-12-19 12:02:49.000000 trytond_product-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    31952 2022-12-19 12:03:07.000000 trytond_product-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10515 2022-12-19 12:02:49.000000 trytond_product-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:15:51.586811 trytond_product-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4506 2022-12-19 12:02:49.000000 trytond_product-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.560144 trytond_product-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_product-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1262 2022-12-19 12:02:49.000000 trytond_product-6.6.1/tests/scenario_product_identifier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2022-12-19 12:02:50.000000 trytond_product-6.6.1/tests/scenario_product_variant.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    18141 2022-12-19 12:03:07.000000 trytond_product-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_product-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2022-12-19 12:02:49.000000 trytond_product-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2022-12-19 12:03:07.000000 trytond_product-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.583477 trytond_product-6.6.1/trytond_product.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2542 2023-04-01 22:15:50.000000 trytond_product-6.6.1/trytond_product.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2735 2023-04-01 22:15:51.000000 trytond_product-6.6.1/trytond_product.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:15:50.000000 trytond_product-6.6.1/trytond_product.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-04-01 22:15:50.000000 trytond_product-6.6.1/trytond_product.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:15:50.000000 trytond_product-6.6.1/trytond_product.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       95 2023-04-01 22:15:50.000000 trytond_product-6.6.1/trytond_product.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:15:50.000000 trytond_product-6.6.1/trytond_product.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    10737 2022-12-19 12:02:49.000000 trytond_product-6.6.1/uom.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15840 2022-12-19 12:02:49.000000 trytond_product-6.6.1/uom.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:15:51.573477 trytond_product-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2022-12-19 12:02:50.000000 trytond_product-6.6.1/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2022-12-19 12:02:50.000000 trytond_product-6.6.1/view/category_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1133 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2022-12-19 12:02:50.000000 trytond_product-6.6.1/view/product_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2022-12-19 12:02:50.000000 trytond_product-6.6.1/view/product_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/product_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1309 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/uom_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/uom_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      626 2022-12-19 12:02:49.000000 trytond_product-6.6.1/view/uom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2022-12-19 12:02:50.000000 trytond_product-6.6.1/view/uom_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.334267 trytond_product-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5145 2023-05-01 11:11:56.000000 trytond_product-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:11:56.000000 trytond_product-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2542 2023-05-01 11:57:31.334267 trytond_product-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_product-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-04-15 07:12:15.000000 trytond_product-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-04-15 07:12:15.000000 trytond_product-6.8.0/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-04-15 07:12:15.000000 trytond_product-6.8.0/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2747 2023-04-15 07:12:15.000000 trytond_product-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2558 2023-04-15 07:12:15.000000 trytond_product-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.330933 trytond_product-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-15 07:12:15.000000 trytond_product-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5486 2023-04-21 08:36:08.000000 trytond_product-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_product-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-04-15 07:12:15.000000 trytond_product-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_product-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.330933 trytond_product-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_product-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_product-6.8.0/icons/tryton-product.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_product-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.320933 trytond_product-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    24734 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26136 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22178 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26646 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26375 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22245 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22756 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24118 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22113 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26328 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24854 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21912 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22936 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25183 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23877 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26266 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25967 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23330 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25784 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24969 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23506 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23427 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21173 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24822 2023-04-30 10:46:36.000000 trytond_product-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-04-15 07:12:15.000000 trytond_product-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32802 2023-04-21 08:36:08.000000 trytond_product-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10515 2023-04-15 07:12:15.000000 trytond_product-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:57:31.334267 trytond_product-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2023-04-15 07:12:15.000000 trytond_product-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.324267 trytond_product-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1262 2023-04-15 07:12:15.000000 trytond_product-6.8.0/tests/scenario_product_identifier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-15 07:12:15.000000 trytond_product-6.8.0/tests/scenario_product_variant.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    22022 2023-04-15 07:12:15.000000 trytond_product-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_product-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-05-01 11:11:49.000000 trytond_product-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.334267 trytond_product-6.8.0/trytond_product.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2542 2023-05-01 11:57:30.000000 trytond_product-6.8.0/trytond_product.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2735 2023-05-01 11:57:31.000000 trytond_product-6.8.0/trytond_product.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:57:30.000000 trytond_product-6.8.0/trytond_product.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 11:57:30.000000 trytond_product-6.8.0/trytond_product.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_product-6.8.0/trytond_product.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      122 2023-05-01 11:57:30.000000 trytond_product-6.8.0/trytond_product.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:57:30.000000 trytond_product-6.8.0/trytond_product.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    10730 2023-04-15 07:12:15.000000 trytond_product-6.8.0/uom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17035 2023-04-15 07:12:15.000000 trytond_product-6.8.0/uom.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:31.327600 trytond_product-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/category_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1133 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/product_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/product_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/product_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_product-6.8.0/view/uom_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/uom_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-01-16 14:00:20.000000 trytond_product-6.8.0/view/uom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product-6.8.0/view/uom_tree.xml
```

### Comparing `trytond_product-6.6.1/CHANGELOG` & `trytond_product-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 
-Version 6.6.1 - 2023-04-01
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Remove non-standard work day unit
+* Add energy units and category
+* Add barcode function on product identifier
+* Add identifier_get to product
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 --------------------------
```

### Comparing `trytond_product-6.6.1/COPYRIGHT` & `trytond_product-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 Copyright (C) 2004-2008 Tiny SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_product-6.6.1/LICENSE` & `trytond_product-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/PKG-INFO` & `trytond_product-6.8.0/trytond_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_product
-Version: 6.6.1
+Name: trytond-product
+Version: 6.8.0
 Summary: Tryton module with products
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-product/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/product
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product
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
 
 ##############
 Product Module
 ##############
```

### Comparing `trytond_product-6.6.1/__init__.py` & `trytond_product-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/category.py` & `trytond_product-6.8.0/category.py`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/category.xml` & `trytond_product-6.8.0/category.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/configuration.py` & `trytond_product-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/configuration.xml` & `trytond_product-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/doc/conf.py` & `trytond_product-6.8.0/doc/conf.py`

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

### Comparing `trytond_product-6.6.1/doc/configuration.rst` & `trytond_product-6.8.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/doc/design.rst` & `trytond_product-6.8.0/doc/design.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 context.
 
 Each product template can have many different product variants, but each
 product variant is based exclusively on one product template.
 
 A product's full code is made up from a prefix code which is defined on the
 product template and a suffix code which is specified on the product variant.
-The full product code can then be used as the product's |SKU|_.
+The full product code can then be used as the product's SKU_.
 
-.. |SKU| replace:: :abbr:`SKU (Stock Keeping Unit)`
 .. _SKU: https://en.wikipedia.org/wiki/Stock_keeping_unit
 
 .. _model-product.template:
 
 Product Template
 ----------------
```

### Comparing `trytond_product-6.6.1/doc/usage.rst` & `trytond_product-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/icons/LICENSE` & `trytond_product-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/ir.py` & `trytond_product-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/locale/bg.po` & `trytond_product-6.8.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -716,14 +716,30 @@
 msgstr "Cubic meter"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_gallon"
@@ -827,19 +843,14 @@
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
 #, fuzzy
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
-#, fuzzy
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -868,14 +879,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -957,27 +984,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Мерни единици"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_surface"
```

### Comparing `trytond_product-6.6.1/locale/ca.po` & `trytond_product-6.8.0/locale/ca.po`

 * *Files 4% similar despite different names*

```diff
@@ -664,14 +664,30 @@
 msgid "Cubic meter"
 msgstr "Metre cúbic"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Dia"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr "Joule"
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr "Kilowatt hora"
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr "Megajoule"
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr "Megawatt hora"
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Peu"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galó"
@@ -752,18 +768,14 @@
 msgid "Square yard"
 msgstr "Iarda quadrada"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unitat"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Dia de treball"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Iarda"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -792,14 +804,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr "J"
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr "kW⋅h"
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr "MJ"
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr "MW⋅h"
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "peu"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -880,26 +908,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Categoria d'unitat de mesura"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr "Energia"
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Longitud"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Superfície"
```

### Comparing `trytond_product-6.6.1/locale/cs.po` & `trytond_product-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 msgid "Product Price Decimal"
 msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
@@ -163,18 +162,17 @@
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
@@ -238,18 +236,17 @@
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
 msgstr "Variants"
 
 msgctxt "field:product.template,type:"
@@ -280,35 +277,33 @@
 msgid "Display Digits"
 msgstr ""
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
 msgstr ""
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
 msgstr ""
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
@@ -670,14 +665,30 @@
 msgid "Cubic meter"
 msgstr "Cubic meter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -758,18 +769,14 @@
 msgid "Square yard"
 msgstr "Square yard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -798,14 +805,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -886,27 +909,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Units of Measure"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Surface"
```

### Comparing `trytond_product-6.6.1/locale/de.po` & `trytond_product-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -594,15 +594,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_uom_form"
 msgid "Units of Measure"
 msgstr "Maßeinheiten"
 
 msgctxt "model:product.category,name:"
 msgid "Product Category"
-msgstr "Artikel Kategorie"
+msgstr "Artikelkategorie"
 
 msgctxt "model:product.configuration,name:"
 msgid "Product Configuration"
 msgstr "Einstellungen Artikel"
 
 msgctxt "model:product.configuration.default_cost_price_method,name:"
 msgid "Product Configuration Default Cost Price Method"
@@ -672,14 +672,30 @@
 msgid "Cubic meter"
 msgstr "Kubikmeter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Tag"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr "Joule"
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr "Kilowattstunde"
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr "Megajoule"
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr "Megawattstunde"
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Fuß"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallone"
@@ -760,18 +776,14 @@
 msgid "Square yard"
 msgstr "Quadratyard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Stück"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Arbeitstag"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -800,14 +812,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr "J"
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr "kWh"
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr "MJ"
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr "MWh"
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -888,26 +916,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "Stk."
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "At."
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Größenart"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr "Energie"
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Länge"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Fläche"
```

### Comparing `trytond_product-6.6.1/locale/es.po` & `trytond_product-6.8.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -664,14 +664,30 @@
 msgid "Cubic meter"
 msgstr "Metro cúbico"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Día"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr "Joule"
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr "Kilowatt hora"
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr "Megajoule"
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr "Megawatt hora"
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Pie"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galón"
@@ -752,18 +768,14 @@
 msgid "Square yard"
 msgstr "Yarda cuadrada"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unidad"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Día de trabajo"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yarda"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -792,14 +804,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr "J"
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr "kW⋅h"
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr "MJ"
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr "MW⋅h"
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "pie"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -880,26 +908,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Categoría de la Unidad de medida"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr "Energía"
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Longitud"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Superficie"
```

### Comparing `trytond_product-6.6.1/locale/es_419.po` & `trytond_product-6.8.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -676,14 +676,30 @@
 msgid "Cubic meter"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr ""
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr ""
@@ -764,18 +780,14 @@
 msgid "Square yard"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr ""
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr ""
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -805,14 +817,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -893,26 +921,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr ""
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr ""
```

### Comparing `trytond_product-6.6.1/locale/et.po` & `trytond_product-6.8.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr "Ülem"
 
-#, fuzzy
 msgctxt "field:product.category,templates:"
 msgid "Products"
 msgstr "Tooted"
 
 msgctxt "field:product.configuration,default_cost_price_method:"
 msgid "Default Cost Method"
 msgstr "Vaikimisi kulumeetod"
@@ -444,15 +443,14 @@
 msgid "The symbol that represents the unit of measure."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_category_list"
 msgid "Categories"
 msgstr "Kategooriad"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_category_product"
 msgid "Add products"
 msgstr "Tooted"
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
 msgstr "Kategooriad"
@@ -548,15 +546,14 @@
 msgid "Categories"
 msgstr "Kategooriad"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Seadistus"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
 msgstr "Tooted"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
 msgstr "Variandid"
@@ -661,14 +658,30 @@
 msgid "Cubic meter"
 msgstr "Kuupmeeter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Päev"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Jalg"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -749,18 +762,14 @@
 msgid "Square yard"
 msgstr "Ruutjard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Ühik"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Tööpäev"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Jard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -789,14 +798,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -877,27 +902,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Mõõtühik"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Pikkus"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Pindala"
```

### Comparing `trytond_product-6.6.1/locale/fa.po` & `trytond_product-6.8.0/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -666,14 +666,30 @@
 msgid "Cubic meter"
 msgstr "متر مکعب"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "روز"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "فوت"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "گالن"
@@ -754,18 +770,14 @@
 msgid "Square yard"
 msgstr "یارد مربع"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "واحد"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "روز کاری"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "یارد"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -794,14 +806,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -882,27 +910,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "واحد اندازه گیری"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "طول"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "سطح"
```

### Comparing `trytond_product-6.6.1/locale/fi.po` & `trytond_product-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 msgid "Product Price Decimal"
 msgstr ""
 
 msgctxt "field:product.category,childs:"
 msgid "Children"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.category,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:product.category,parent:"
 msgid "Parent"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.category,templates:"
@@ -162,17 +163,18 @@
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.product,list_prices:"
 msgid "List Prices"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:product.product,prefix_code:"
 msgid "Prefix Code"
 msgstr ""
 
 msgctxt "field:product.product,suffix_code:"
 msgid "Suffix Code"
@@ -236,17 +238,18 @@
 msgid "List Price"
 msgstr ""
 
 msgctxt "field:product.template,list_prices:"
 msgid "List Prices"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:product.template,products:"
 msgid "Variants"
 msgstr "Variants"
 
 msgctxt "field:product.template,type:"
@@ -277,33 +280,35 @@
 msgid "Display Digits"
 msgstr ""
 
 msgctxt "field:product.uom,factor:"
 msgid "Factor"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.uom,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:product.uom,rate:"
 msgid "Rate"
 msgstr ""
 
 msgctxt "field:product.uom,rounding:"
 msgid "Rounding Precision"
 msgstr ""
 
 msgctxt "field:product.uom,symbol:"
 msgid "Symbol"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.uom.category,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 #, fuzzy
 msgctxt "field:product.uom.category,uoms:"
 msgid "Units of Measure"
 msgstr "Units of Measure"
 
 msgctxt "help:product.category,childs:"
@@ -665,14 +670,30 @@
 msgid "Cubic meter"
 msgstr "Cubic meter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -753,18 +774,14 @@
 msgid "Square yard"
 msgstr "Square yard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -793,14 +810,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -881,27 +914,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Units of Measure"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Surface"
```

### Comparing `trytond_product-6.6.1/locale/fr.po` & `trytond_product-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -666,14 +666,30 @@
 msgid "Cubic meter"
 msgstr "Mètre cube"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Jour"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr "Joule"
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr "Kilowatt-heure"
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr "Mégajoule"
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr "Mégawatt-heure"
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Pied"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -754,18 +770,14 @@
 msgid "Square yard"
 msgstr "Yard carré"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unité"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Jour de travail"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -794,14 +806,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "j"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr "J"
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr "kW⋅h"
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr "MJ"
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr "MW⋅h"
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -882,26 +910,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "jt"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Catégorie d'unité de mesure"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr "Énergie"
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Longueur"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Surface"
```

### Comparing `trytond_product-6.6.1/locale/hu.po` & `trytond_product-6.8.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -670,14 +670,30 @@
 msgid "Cubic meter"
 msgstr "Köbméter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Nap"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Láb"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -758,18 +774,14 @@
 msgid "Square yard"
 msgstr "Négyzetyard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Darab"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Munkanap"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -798,14 +810,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "t"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -886,28 +914,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "db"
 
-#, fuzzy
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Mértékegység"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Hossz"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Terület"
```

### Comparing `trytond_product-6.6.1/locale/id.po` & `trytond_product-6.8.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -647,14 +647,30 @@
 msgid "Cubic meter"
 msgstr "Meter kubik"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Hari"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Kaki"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galon"
@@ -735,18 +751,14 @@
 msgid "Square yard"
 msgstr "Yard persegi"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr ""
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr ""
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr ""
@@ -775,14 +787,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr ""
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr ""
@@ -863,26 +891,26 @@
 msgid "yd²"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr ""
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr ""
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Kategori Satuan Ukuran"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Panjang"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr ""
```

### Comparing `trytond_product-6.6.1/locale/it.po` & `trytond_product-6.8.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -668,14 +668,30 @@
 msgid "Cubic meter"
 msgstr "Cubic meter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Giorno"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -756,18 +772,14 @@
 msgid "Square yard"
 msgstr "Square yard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unità"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -796,14 +808,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -884,27 +912,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Unità di misura"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Lunghezza"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Surface"
```

### Comparing `trytond_product-6.6.1/locale/lo.po` & `trytond_product-6.8.0/locale/lo.po`

 * *Files 7% similar despite different names*

```diff
@@ -701,14 +701,30 @@
 msgstr "Cubic meter"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_gallon"
@@ -812,19 +828,14 @@
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
 #, fuzzy
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
-#, fuzzy
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -860,14 +871,30 @@
 msgstr "m³"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_gallon"
@@ -971,28 +998,27 @@
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
 #, fuzzy
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "ໜ່ວຍວັດແທກ"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_surface"
```

### Comparing `trytond_product-6.6.1/locale/lt.po` & `trytond_product-6.8.0/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -665,14 +665,30 @@
 msgid "Cubic meter"
 msgstr "Kubinis metras"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Diena"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Pėda"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galonas"
@@ -753,18 +769,14 @@
 msgid "Square yard"
 msgstr "Kvadratinis jardas"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Vienetas"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Darbo diena"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Jardas"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -793,14 +805,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -881,27 +909,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "vnt"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "dd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Mato vienetas"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Ilgis"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Paviršius"
```

### Comparing `trytond_product-6.6.1/locale/nl.po` & `trytond_product-6.8.0/locale/nl.po`

 * *Files 4% similar despite different names*

```diff
@@ -667,14 +667,30 @@
 msgid "Cubic meter"
 msgstr "Kubieke meter"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Dag"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr "Joule"
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr "Kilowattuur"
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr "Megajoule"
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr "Megawattuur"
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Voet"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Gallon"
@@ -755,18 +771,14 @@
 msgid "Square yard"
 msgstr "Vierkante yard"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Eenheid"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Werkdag"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -795,14 +807,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr "J"
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr "kW⋅u"
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr "MJ"
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr "MW⋅u"
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -883,26 +911,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "st"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Categorie maateenheid"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr "Energie"
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Lengte"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Oppervlakte"
```

### Comparing `trytond_product-6.6.1/locale/pl.po` & `trytond_product-6.8.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -673,14 +673,30 @@
 msgid "Cubic meter"
 msgstr "Metr sześcienny"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Dzień"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Stopa"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galon"
@@ -761,18 +777,14 @@
 msgid "Square yard"
 msgstr "Jard kwadratowy"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Jednostka"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Dzień roboczy"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Jard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -801,14 +813,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -889,26 +917,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "szt."
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Kategoria jednostek miary"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Długość"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Powierzchnia"
```

### Comparing `trytond_product-6.6.1/locale/pt.po` & `trytond_product-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -666,14 +666,30 @@
 msgid "Cubic meter"
 msgstr "Metro cúbico"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Dia"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Pé"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galão"
@@ -754,18 +770,14 @@
 msgid "Square yard"
 msgstr "Jarda quadrada"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unidade"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Dia de trabalho"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Jarda"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -794,14 +806,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -882,27 +910,27 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "dt"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Unidade de Medida"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Comprimento"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Superfície"
```

### Comparing `trytond_product-6.6.1/locale/ro.po` & `trytond_product-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -501,30 +501,29 @@
 msgid "The %(type)s \"%(code)s\" for product \"%(product)s\" is not valid."
 msgstr "%(type)s \"%(code)s\" nu este valabil pentru produsul \"%(product)s\"."
 
 msgctxt "model:ir.message,text:msg_product_code_unique"
 msgid "Code of active product must be unique."
 msgstr "Codul al unui produs activ trebuie să fie unic."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_uom_decrease_digits"
 msgid "You cannot decrease the digits of UOM \"%(uom)s\"."
-msgstr "Nu se poate modifică rate al UM \"%(uom)s\"."
+msgstr "Nu se pot reduce zecimalele al UM \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_incompatible_factor_rate"
 msgid "Incompatible factor and rate values on UOM \"%(uom)s\"."
 msgstr "Factor şi rata incompatibil pentru UM \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_modify_category"
 msgid "You cannot modify the category of UOM \"%(uom)s\"."
-msgstr "Nu se poate modifică categorie de UM \"%(uom)s\"."
+msgstr "Categoria de UM nu se poate modifica \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_modify_factor"
 msgid "You cannot modify the factor of UOM \"%(uom)s\"."
-msgstr "Nu se poate modifică factorul al Unitaţii de Masură \"%(uom)s\"."
+msgstr "Nu se poate modifica factorul Unităţii de Masură \"%(uom)s\"."
 
 msgctxt "model:ir.message,text:msg_uom_modify_options"
 msgid ""
 "If the UOM is still not used, you can delete it otherwise you can deactivate"
 " it and create a new one."
 msgstr ""
 "Dacă UM nu este utilizată se poate şterge, altfel se poate dezactiva în "
@@ -558,15 +557,14 @@
 msgid "Categories"
 msgstr "Categorii"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Configurare"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_main_product"
 msgid "Products"
 msgstr "Produse"
 
 msgctxt "model:ir.ui.menu,name:menu_product"
 msgid "Variants"
 msgstr "Variante"
@@ -667,14 +665,30 @@
 msgid "Cubic meter"
 msgstr "Metru cub"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Zi"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr "Joule"
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr "Kilowatt-oră"
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr "Megajoule"
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr "Megawatt-oră"
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Picior"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "Galon"
@@ -755,18 +769,14 @@
 msgid "Square yard"
 msgstr "Iard Pătrat"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unitate"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Zi de lucru"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Iard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -795,14 +805,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr "J"
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr "kW⋅h"
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr "MJ"
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr "MW⋅h"
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -883,26 +909,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "buc"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Categorie Unitate de Măsura"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr "Energie"
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Lungime"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "Suprafața"
```

### Comparing `trytond_product-6.6.1/locale/ru.po` & `trytond_product-6.8.0/locale/ru.po`

 * *Files 7% similar despite different names*

```diff
@@ -710,14 +710,30 @@
 msgstr "Cubic meter"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_gallon"
@@ -821,19 +837,14 @@
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
 #, fuzzy
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
-#, fuzzy
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
@@ -870,14 +881,30 @@
 msgstr "m³"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_gallon"
@@ -981,28 +1008,27 @@
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
 #, fuzzy
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Единица измерения"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_surface"
```

### Comparing `trytond_product-6.6.1/locale/sl.po` & `trytond_product-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -695,14 +695,30 @@
 msgstr "Cubic meter"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_gallon"
@@ -806,19 +822,14 @@
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
 #, fuzzy
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
-#, fuzzy
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -847,14 +858,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -936,28 +963,27 @@
 msgstr "yd²"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-#, fuzzy
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Merska enota"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_surface"
```

### Comparing `trytond_product-6.6.1/locale/tr.po` & `trytond_product-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -683,14 +683,30 @@
 msgstr "Cubic meter"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "Day"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "Foot"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
@@ -788,19 +804,14 @@
 msgstr "Square yard"
 
 #, fuzzy
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "Unit"
 
-#, fuzzy
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "Work Day"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "Yard"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -830,14 +841,30 @@
 msgstr "m³"
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -923,28 +950,27 @@
 
 #, fuzzy
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
 #, fuzzy
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
-#, fuzzy
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "Ölçü birimi"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "Length"
 
 #, fuzzy
 msgctxt "model:product.uom.category,name:uom_cat_surface"
```

### Comparing `trytond_product-6.6.1/locale/uk.po` & `trytond_product-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -641,14 +641,30 @@
 msgid "Cubic meter"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr ""
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr ""
@@ -729,18 +745,14 @@
 msgid "Square yard"
 msgstr ""
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr ""
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr ""
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr ""
@@ -769,14 +781,30 @@
 msgid "m³"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr ""
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr ""
@@ -857,26 +885,26 @@
 msgid "yd²"
 msgstr ""
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr ""
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr ""
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr ""
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr ""
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr ""
```

### Comparing `trytond_product-6.6.1/locale/zh_CN.po` & `trytond_product-6.8.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -661,14 +661,30 @@
 msgid "Cubic meter"
 msgstr "立方米"
 
 msgctxt "model:product.uom,name:uom_day"
 msgid "Day"
 msgstr "天"
 
+msgctxt "model:product.uom,name:uom_energy_joule"
+msgid "Joule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_kwh"
+msgid "Kilowatt-hour"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_megajoule"
+msgid "Megajoule"
+msgstr ""
+
+msgctxt "model:product.uom,name:uom_energy_mwh"
+msgid "Megawatt-hour"
+msgstr ""
+
 msgctxt "model:product.uom,name:uom_foot"
 msgid "Foot"
 msgstr "英尺"
 
 msgctxt "model:product.uom,name:uom_gallon"
 msgid "Gallon"
 msgstr "加仑"
@@ -749,18 +765,14 @@
 msgid "Square yard"
 msgstr "平方码"
 
 msgctxt "model:product.uom,name:uom_unit"
 msgid "Unit"
 msgstr "单位"
 
-msgctxt "model:product.uom,name:uom_work_day"
-msgid "Work Day"
-msgstr "工作日"
-
 msgctxt "model:product.uom,name:uom_yard"
 msgid "Yard"
 msgstr "码"
 
 msgctxt "model:product.uom,symbol:uom_are"
 msgid "a"
 msgstr "a"
@@ -789,14 +801,30 @@
 msgid "m³"
 msgstr "m³"
 
 msgctxt "model:product.uom,symbol:uom_day"
 msgid "d"
 msgstr "d"
 
+msgctxt "model:product.uom,symbol:uom_energy_joule"
+msgid "J"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_kwh"
+msgid "kW⋅h"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_megajoule"
+msgid "MJ"
+msgstr ""
+
+msgctxt "model:product.uom,symbol:uom_energy_mwh"
+msgid "MW⋅h"
+msgstr ""
+
 msgctxt "model:product.uom,symbol:uom_foot"
 msgid "ft"
 msgstr "ft"
 
 msgctxt "model:product.uom,symbol:uom_gallon"
 msgid "gal"
 msgstr "gal"
@@ -877,26 +905,26 @@
 msgid "yd²"
 msgstr "yd²"
 
 msgctxt "model:product.uom,symbol:uom_unit"
 msgid "u"
 msgstr "u"
 
-msgctxt "model:product.uom,symbol:uom_work_day"
-msgid "wd"
-msgstr "wd"
-
 msgctxt "model:product.uom,symbol:uom_yard"
 msgid "yd"
 msgstr "yd"
 
 msgctxt "model:product.uom.category,name:"
 msgid "Unit of Measure Category"
 msgstr "计量单位类别"
 
+msgctxt "model:product.uom.category,name:uom_cat_energy"
+msgid "Energy"
+msgstr ""
+
 msgctxt "model:product.uom.category,name:uom_cat_length"
 msgid "Length"
 msgstr "长度"
 
 msgctxt "model:product.uom.category,name:uom_cat_surface"
 msgid "Surface"
 msgstr "面积"
```

### Comparing `trytond_product-6.6.1/message.xml` & `trytond_product-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/product.py` & `trytond_product-6.8.0/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.pool import Pool
 from trytond.pyson import Eval, Get, If
 from trytond.tools import is_full_text, lstrip_wildcard
 from trytond.tools.multivalue import migrate_property
 from trytond.transaction import Transaction
 
+try:
+    from trytond.tools import barcode
+except ImportError:
+    barcode = None
+
 from .exceptions import InvalidIdentifierCode
 from .ir import price_decimal
 
 __all__ = ['price_digits', 'round_price', 'TemplateFunction']
 logger = logging.getLogger(__name__)
 
 TYPES = [
@@ -232,21 +237,19 @@
     @fields.depends('type', 'cost_price_method')
     def on_change_type(self):
         if self.type == 'service':
             self.cost_price_method = 'fixed'
 
     @fields.depends('default_uom')
     def on_change_with_default_uom_category(self, name=None):
-        if self.default_uom:
-            return self.default_uom.category.id
+        return self.default_uom.category if self.default_uom else None
 
     @classmethod
     def search_default_uom_category(cls, name, clause):
-        return [('default_uom.category' + clause[0].lstrip(name),)
-            + tuple(clause[1:])]
+        return [('default_uom.category' + clause[0][len(name):], *clause[1:])]
 
     @fields.depends('default_uom')
     def on_change_with_default_uom_digits(self, name=None):
         if self.default_uom:
             return self.default_uom.digits
 
     @classmethod
@@ -517,14 +520,20 @@
     def set_multivalue(self, name, value, save=True, **pattern):
         context = Transaction().context
         if name in {'cost_price', 'list_price'} and not value:
             if not pattern.get('company', context.get('company')):
                 return []
         return super().set_multivalue(name, value, save=save, **pattern)
 
+    def get_multivalue(self, name, **pattern):
+        if isinstance(self._fields[name], TemplateFunction):
+            return self.template.get_multivalue(name, **pattern)
+        else:
+            return super().get_multivalue(name, **pattern)
+
     @classmethod
     def default_cost_price(cls, **pattern):
         context = Transaction().context
         if pattern.get('company', context.get('company')):
             return Decimal(0)
 
     @classmethod
@@ -599,14 +608,22 @@
         Configuration = pool.get('product.configuration')
         config = Configuration(1)
         return bool(config.product_sequence)
 
     def get_code_readonly(self, name):
         return self.default_code_readonly()
 
+    def identifier_get(self, types=None):
+        "Return the first identifier for the given types"
+        if isinstance(types, str) or types is None:
+            types = {types}
+        for identifier in self.identifiers:
+            if identifier.type in types:
+                return identifier
+
     @classmethod
     def _new_suffix_code(cls):
         pool = Pool()
         Configuration = pool.get('product.configuration')
         config = Configuration(1)
         sequence = config.product_sequence
         if sequence:
@@ -896,7 +913,12 @@
                 else:
                     product = ''
                 raise InvalidIdentifierCode(
                     gettext('product.msg_invalid_code',
                         type=self.type_string,
                         code=self.code,
                         product=product))
+
+    def barcode(self, format='svg', **options):
+        if barcode and self.type in barcode.BARCODES:
+            generator = getattr(barcode, 'generate_%s' % format)
+            return generator(self.type, self.on_change_with_code(), **options)
```

### Comparing `trytond_product-6.6.1/product.xml` & `trytond_product-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/setup.py` & `trytond_product-6.8.0/setup.py`

 * *Files 9% similar despite different names*

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
@@ -37,38 +34,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_product'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql', 'python-stdnum']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond[barcode]'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module with products',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-product/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/product',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product',
     package_dir={'trytond.modules.product': '.'},
     packages=(
         ['trytond.modules.product']
         + ['trytond.modules.product.%s' % p for p in find_packages()]
         ),
@@ -106,23 +109,23 @@
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

### Comparing `trytond_product-6.6.1/tests/scenario_product_identifier.rst` & `trytond_product-6.8.0/tests/scenario_product_identifier.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/tests/scenario_product_variant.rst` & `trytond_product-6.8.0/tests/scenario_product_variant.rst`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/trytond_product.egg-info/PKG-INFO` & `trytond_product-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-product
-Version: 6.6.1
+Name: trytond_product
+Version: 6.8.0
 Summary: Tryton module with products
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-product/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/product
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product
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
 
 ##############
 Product Module
 ##############
```

### Comparing `trytond_product-6.6.1/trytond_product.egg-info/SOURCES.txt` & `trytond_product-6.8.0/trytond_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/uom.py` & `trytond_product-6.8.0/uom.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             ('non_zero_rate_factor', Check(t, (t.rate != 0) | (t.factor != 0)),
                 'product.msg_uom_no_zero_factor_rate')
             ]
         cls._order.insert(0, ('name', 'ASC'))
 
     @classmethod
     def check_xml_record(cls, records, values):
-        return True
+        pass
 
     @staticmethod
     def default_rate():
         return 1.0
 
     @staticmethod
     def default_factor():
```

### Comparing `trytond_product-6.6.1/uom.xml` & `trytond_product-6.8.0/uom.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_product-6.6.1/uom.xml` & `trytond_product-6.8.0/uom.xml`

```diff
@@ -125,21 +125,14 @@
     <record model="product.uom" id="uom_hour">
       <field name="name">Hour</field>
       <field name="symbol">h</field>
       <field name="category" ref="uom_cat_time"/>
       <field name="factor" eval="1."/>
       <field name="rate" eval="1."/>
     </record>
-    <record model="product.uom" id="uom_work_day">
-      <field name="name">Work Day</field>
-      <field name="symbol">wd</field>
-      <field name="category" ref="uom_cat_time"/>
-      <field name="factor" eval="8."/>
-      <field name="rate" eval="0.125"/>
-    </record>
     <record model="product.uom" id="uom_day">
       <field name="name">Day</field>
       <field name="symbol">d</field>
       <field name="category" ref="uom_cat_time"/>
       <field name="factor" eval="24."/>
       <field name="rate" eval="round(1.0 / 24, 12)"/>
     </record>
@@ -295,14 +288,45 @@
     <record model="product.uom" id="uom_square_yard">
       <field name="name">Square yard</field>
       <field name="symbol">yd²</field>
       <field name="category" ref="uom_cat_surface"/>
       <field name="factor" eval="0.83612736"/>
       <field name="rate" eval="round(1.0 / 0.83612736, 12)"/>
     </record>
+    <record model="product.uom.category" id="uom_cat_energy">
+      <field name="name">Energy</field>
+    </record>
+    <record model="product.uom" id="uom_energy_joule">
+      <field name="name">Joule</field>
+      <field name="symbol">J</field>
+      <field name="category" ref="uom_cat_energy"/>
+      <field name="factor" eval="1."/>
+      <field name="rate" eval="1."/>
+    </record>
+    <record model="product.uom" id="uom_energy_megajoule">
+      <field name="name">Megajoule</field>
+      <field name="symbol">MJ</field>
+      <field name="category" ref="uom_cat_energy"/>
+      <field name="factor" eval="1_000_000."/>
+      <field name="rate" eval="round(1.0 / 1_000_000, 12)"/>
+    </record>
+    <record model="product.uom" id="uom_energy_kwh">
+      <field name="name">Kilowatt-hour</field>
+      <field name="symbol">kW⋅h</field>
+      <field name="category" ref="uom_cat_energy"/>
+      <field name="factor" eval="3_600_000"/>
+      <field name="rate" eval="round(1.0 / 3_600_000, 12)"/>
+    </record>
+    <record model="product.uom" id="uom_energy_mwh">
+      <field name="name">Megawatt-hour</field>
+      <field name="symbol">MW⋅h</field>
+      <field name="category" ref="uom_cat_energy"/>
+      <field name="factor" eval="3_600_000_000"/>
+      <field name="rate" eval="round(1.0 / 3_600_000_000, 12)"/>
+    </record>
     <record model="ir.model.access" id="access_uom">
       <field name="model" search="[('model', '=', 'product.uom')]"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
```

### Comparing `trytond_product-6.6.1/view/category_form.xml` & `trytond_product-6.8.0/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/view/product_form.xml` & `trytond_product-6.8.0/view/product_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/view/product_form_simple.xml` & `trytond_product-6.8.0/view/product_form_simple.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/view/template_form.xml` & `trytond_product-6.8.0/view/template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product-6.6.1/view/uom_form.xml` & `trytond_product-6.8.0/view/uom_form.xml`

 * *Files identical despite different names*

