# Comparing `tmp/trytond_purchase_secondary_unit-6.6.0.tar.gz` & `tmp/trytond_purchase_secondary_unit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_secondary_unit-6.6.0.tar", last modified: Mon Oct 31 16:19:46 2022, max compression
+gzip compressed data, was "trytond_purchase_secondary_unit-6.8.0.tar", last modified: Mon May  1 12:06:35 2023, max compression
```

## Comparing `trytond_purchase_secondary_unit-6.6.0.tar` & `trytond_purchase_secondary_unit-6.8.0.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:19:46.544407 trytond_purchase_secondary_unit-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_purchase_secondary_unit-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_purchase_secondary_unit-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-10-31 16:19:44.000000 trytond_purchase_secondary_unit-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_purchase_secondary_unit-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      604 2022-10-31 16:19:43.000000 trytond_purchase_secondary_unit-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:19:43.000000 trytond_purchase_secondary_unit-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_purchase_secondary_unit-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2586 2022-10-31 16:19:46.544407 trytond_purchase_secondary_unit-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      852 2022-10-11 19:49:58.000000 trytond_purchase_secondary_unit-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1225 2021-12-11 16:59:33.000000 trytond_purchase_secondary_unit-6.6.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:19:46.544407 trytond_purchase_secondary_unit-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:19:46.541073 trytond_purchase_secondary_unit-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5190 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5276 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5198 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5377 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3946 2022-10-29 07:50:48.000000 trytond_purchase_secondary_unit-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6569 2022-04-11 21:24:34.000000 trytond_purchase_secondary_unit-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14889 2022-10-11 19:49:58.000000 trytond_purchase_secondary_unit-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:19:46.544407 trytond_purchase_secondary_unit-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5519 2022-10-29 07:39:11.000000 trytond_purchase_secondary_unit-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2021-12-11 16:59:33.000000 trytond_purchase_secondary_unit-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:19:46.541073 trytond_purchase_secondary_unit-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_purchase_secondary_unit-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3934 2022-10-11 19:49:58.000000 trytond_purchase_secondary_unit-6.6.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3229 2021-12-10 21:27:02.000000 trytond_purchase_secondary_unit-6.6.0/tests/scenario_purchase_requisition_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4007 2020-11-02 09:23:33.000000 trytond_purchase_secondary_unit-6.6.0/tests/scenario_purchase_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2022-10-11 19:49:58.000000 trytond_purchase_secondary_unit-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_purchase_secondary_unit-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2022-10-31 15:10:09.000000 trytond_purchase_secondary_unit-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2022-10-31 16:19:42.000000 trytond_purchase_secondary_unit-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:19:46.544407 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2586 2022-10-31 16:19:45.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2187 2022-10-31 16:19:46.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:19:45.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2022-10-31 16:19:45.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-11-04 12:06:19.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2022-10-31 16:19:45.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:19:45.000000 trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:19:46.541073 trytond_purchase_secondary_unit-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      723 2019-10-11 23:19:18.000000 trytond_purchase_secondary_unit-6.6.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2021-10-07 13:08:07.000000 trytond_purchase_secondary_unit-6.6.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2022-04-08 16:23:26.000000 trytond_purchase_secondary_unit-6.6.0/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2020-10-14 08:00:14.000000 trytond_purchase_secondary_unit-6.6.0/view/stock_move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:35.911024 trytond_purchase_secondary_unit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-05-01 11:18:18.000000 trytond_purchase_secondary_unit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:18:17.000000 trytond_purchase_secondary_unit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2570 2023-05-01 12:06:35.911024 trytond_purchase_secondary_unit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      852 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1225 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:35.907691 trytond_purchase_secondary_unit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:35.904358 trytond_purchase_secondary_unit-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5190 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5276 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5198 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5377 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3946 2023-04-29 08:02:54.000000 trytond_purchase_secondary_unit-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6555 2023-04-21 08:36:08.000000 trytond_purchase_secondary_unit-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14880 2023-04-21 08:36:08.000000 trytond_purchase_secondary_unit-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:06:35.911024 trytond_purchase_secondary_unit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4700 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:35.904358 trytond_purchase_secondary_unit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3876 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3229 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tests/scenario_purchase_requisition_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4007 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tests/scenario_purchase_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 11:18:12.000000 trytond_purchase_secondary_unit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:35.911024 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2570 2023-05-01 12:06:35.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-05-01 12:06:35.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:06:35.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-05-01 12:06:35.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-05-01 12:06:35.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:06:35.000000 trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:35.907691 trytond_purchase_secondary_unit-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      723 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-6.8.0/view/stock_move_list.xml
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/CHANGELOG` & `trytond_purchase_secondary_unit-6.8.0/CHANGELOG`

 * *Files 17% similar despite different names*

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

### Comparing `trytond_purchase_secondary_unit-6.6.0/COPYRIGHT` & `trytond_purchase_secondary_unit-6.8.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2019-2022 Cédric Krier
-Copyright (C) 2019-2022 B2CK
+Copyright (C) 2019-2023 Cédric Krier
+Copyright (C) 2019-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/LICENSE` & `trytond_purchase_secondary_unit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/PKG-INFO` & `trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_purchase_secondary_unit
-Version: 6.6.0
+Name: trytond-purchase-secondary-unit
+Version: 6.8.0
 Summary: Tryton module to add a secondary unit on purchase line
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_secondary_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase secondary unit
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
 
 Purchase Secondary Unit Module
 ##############################
 
 The purchase secondary unit module adds a secondary unit of measure on purchase
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/__init__.py` & `trytond_purchase_secondary_unit-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/account.py` & `trytond_purchase_secondary_unit-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/bg.po` & `trytond_purchase_secondary_unit-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/ca.po` & `trytond_purchase_secondary_unit-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/cs.po` & `trytond_purchase_secondary_unit-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/de.po` & `trytond_purchase_secondary_unit-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/es.po` & `trytond_purchase_secondary_unit-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/es_419.po` & `trytond_purchase_secondary_unit-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/et.po` & `trytond_purchase_secondary_unit-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/fa.po` & `trytond_purchase_secondary_unit-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/fi.po` & `trytond_purchase_secondary_unit-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/fr.po` & `trytond_purchase_secondary_unit-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/hu.po` & `trytond_purchase_secondary_unit-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/id.po` & `trytond_purchase_secondary_unit-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/it.po` & `trytond_purchase_secondary_unit-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/lo.po` & `trytond_purchase_secondary_unit-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/lt.po` & `trytond_purchase_secondary_unit-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/nl.po` & `trytond_purchase_secondary_unit-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/pl.po` & `trytond_purchase_secondary_unit-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/pt.po` & `trytond_purchase_secondary_unit-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/ro.po` & `trytond_purchase_secondary_unit-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/ru.po` & `trytond_purchase_secondary_unit-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/sl.po` & `trytond_purchase_secondary_unit-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/tr.po` & `trytond_purchase_secondary_unit-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/uk.po` & `trytond_purchase_secondary_unit-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/locale/zh_CN.po` & `trytond_purchase_secondary_unit-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/product.py` & `trytond_purchase_secondary_unit-6.8.0/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,20 +55,20 @@
             self.purchase_secondary_uom_factor = round(
                 1. / self.purchase_secondary_uom_rate,
                 uom_conversion_digits[1])
 
     @fields.depends('purchase_secondary_uom')
     def on_change_with_purchase_secondary_uom_category(self, name=None):
         if self.purchase_secondary_uom:
-            return self.purchase_secondary_uom.category.id
+            return self.purchase_secondary_uom.category
 
     @classmethod
     def search_purchase_secondary_uom_category(cls, name, clause):
-        return [('purchase_secondary_uom.category' + clause[0].lstrip(name),)
-            + tuple(clause[1:])]
+        return [('purchase_secondary_uom.category' + clause[0][len(name):],
+                *clause[1:])]
 
     @property
     def purchase_secondary_uom_normal_rate(self):
         uom = self.purchase_secondary_uom
         rate = self.purchase_secondary_uom_rate
         if self.purchase_uom and rate and uom:
             if self.purchase_uom.accurate_field == 'factor':
@@ -151,17 +151,17 @@
         fields.Many2One('product.uom.category', "Default UOM Category"),
         'on_change_with_default_uom_category')
 
     @fields.depends('template', '_parent_template.purchase_uom',
         'product', '_parent_product.purchase_uom')
     def on_change_with_default_uom_category(self, name=None):
         if self.product and self.product.purchase_uom:
-            return self.product.purchase_uom.category.id
+            return self.product.purchase_uom.category
         elif self.template and self.template.purchase_uom:
-            return self.template.purchase_uom.category.id
+            return self.template.purchase_uom.category
 
     @property
     def purchase_uom(self):
         if self.product and self.product.purchase_uom:
             return self.product.purchase_uom
         elif self.template and self.template.purchase_uom:
             return self.template.purchase_uom
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/product.xml` & `trytond_purchase_secondary_unit-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/purchase.py` & `trytond_purchase_secondary_unit-6.8.0/purchase.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self.on_change_secondary_quantity()
         self.on_change_secondary_unit_price()
 
     @fields.depends(methods=['_secondary_record'])
     def on_change_with_product_secondary_uom_category(self, name=None):
         secondary_record = self._secondary_record()
         if secondary_record:
-            return secondary_record.purchase_secondary_uom.category.id
+            return secondary_record.purchase_secondary_uom.category
 
     @classmethod
     def set_secondary(cls, lines, name, value):
         pass
 
     @fields.depends('secondary_unit',
         methods=['on_change_with_secondary_quantity', '_secondary_record'])
@@ -182,15 +182,15 @@
     @classmethod
     def _unit_categories(cls):
         return super()._unit_categories() + ['product_secondary_uom_category']
 
     @fields.depends('product')
     def on_change_with_product_secondary_uom_category(self, name=None):
         if self.product and self.product.purchase_secondary_uom:
-            return self.product.purchase_secondary_uom.category.id
+            return self.product.purchase_secondary_uom.category
 
     @property
     def request_unit(self):
         unit = super().request_unit
         product = self.product
         if (product
                 and self.unit
@@ -271,15 +271,15 @@
                 rate=line.secondary_uom_factor,
                 round=round)
         return remaining_quantity
 
     @fields.depends('product')
     def on_change_with_product_secondary_uom_category(self, name=None):
         if self.product and self.product.purchase_secondary_uom:
-            return self.product.purchase_secondary_uom.category.id
+            return self.product.purchase_secondary_uom.category
 
     def _set_purchase_line_quantity(self, purchase_line):
         super()._set_purchase_line_quantity(purchase_line)
         secondary_uom = self.product.purchase_secondary_uom
         if (secondary_uom
                 and self.unit.category == secondary_uom.category):
             purchase_line.unit = self.product.purchase_uom
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/purchase.xml` & `trytond_purchase_secondary_unit-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/setup.py` & `trytond_purchase_secondary_unit-6.8.0/setup.py`

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
@@ -34,65 +31,46 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_secondary_unit'
 
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
     get_require_version('trytond_account_invoice_secondary_unit'),
     get_require_version('trytond_purchase_blanket_agreement'),
     get_require_version('trytond_purchase_request'),
     get_require_version('trytond_purchase_requisition'),
     get_require_version('trytond_stock_secondary_unit')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add a secondary unit on purchase line',
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
-        "Source Code": 'https://hg.tryton.org/modules/purchase_secondary_unit',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase secondary unit',
     package_dir={'trytond.modules.purchase_secondary_unit': '.'},
     packages=(
         ['trytond.modules.purchase_secondary_unit']
         + ['trytond.modules.purchase_secondary_unit.%s' % p
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
     purchase_secondary_unit = trytond.modules.purchase_secondary_unit
     """,
     )
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/stock.py` & `trytond_purchase_secondary_unit-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst` & `trytond_purchase_secondary_unit-6.8.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 ==================================================
 Purchase Blanket Agreement Secondary Unit Scenario
 ==================================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts)
 
-    >>> today = datetime.date.today()
-    >>> later = today + relativedelta(days=30)
+    >>> today = dt.date.today()
+    >>> later = today + dt.timedelta(days=30)
 
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_secondary_unit', 'purchase_blanket_agreement'])
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/tests/scenario_purchase_requisition_secondary_unit.rst` & `trytond_purchase_secondary_unit-6.8.0/tests/scenario_purchase_requisition_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/tests/scenario_purchase_secondary_unit.rst` & `trytond_purchase_secondary_unit-6.8.0/tests/scenario_purchase_secondary_unit.rst`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 Confirm purchase::
 
     >>> line.secondary_unit = kg
     >>> line.quantity = 10
     >>> purchase.click('quote')
     >>> purchase.click('confirm')
     >>> purchase.invoice_state
-    'waiting'
+    'pending'
     >>> purchase.shipment_state
     'waiting'
 
 Check secondary unit on invoice::
 
     >>> invoice, = purchase.invoices
     >>> _, line = invoice.lines
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO` & `trytond_purchase_secondary_unit-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-secondary-unit
-Version: 6.6.0
+Name: trytond_purchase_secondary_unit
+Version: 6.8.0
 Summary: Tryton module to add a secondary unit on purchase line
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
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_secondary_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase secondary unit
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
 
 Purchase Secondary Unit Module
 ##############################
 
 The purchase secondary unit module adds a secondary unit of measure on purchase
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt` & `trytond_purchase_secondary_unit-6.8.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt`

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
 account.py
@@ -60,14 +56,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/product_supplier_form.xml
 ./view/product_template_form.xml
 ./view/purchase_line_form.xml
 ./view/purchase_line_tree.xml
 ./view/stock_move_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_purchase_secondary_unit-6.6.0/view/product_supplier_form.xml` & `trytond_purchase_secondary_unit-6.8.0/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/view/product_template_form.xml` & `trytond_purchase_secondary_unit-6.8.0/view/product_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-6.6.0/view/purchase_line_form.xml` & `trytond_purchase_secondary_unit-6.8.0/view/purchase_line_form.xml`

 * *Files identical despite different names*

