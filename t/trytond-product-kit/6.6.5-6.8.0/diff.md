# Comparing `tmp/trytond_product_kit-6.6.5.tar.gz` & `tmp/trytond_product_kit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_kit-6.6.5.tar", last modified: Sat Apr  1 22:13:32 2023, max compression
+gzip compressed data, was "trytond_product_kit-6.8.0.tar", last modified: Mon May  1 11:43:26 2023, max compression
```

## Comparing `trytond_product_kit-6.6.5.tar` & `trytond_product_kit-6.8.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:13:32.721857 trytond_product_kit-6.6.5/
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-04-01 22:13:28.000000 trytond_product_kit-6.6.5/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-04-01 22:13:27.000000 trytond_product_kit-6.6.5/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-04-01 22:13:32.721857 trytond_product_kit-6.6.5/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1825 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1880 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16888 2023-03-18 11:00:44.000000 trytond_product_kit-6.6.5/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:13:32.715190 trytond_product_kit-6.6.5/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3587 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:13:32.701857 trytond_product_kit-6.6.5/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6947 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7124 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7028 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6963 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5715 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5736 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7014 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5709 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10067 2023-02-27 17:46:08.000000 trytond_product_kit-6.6.5/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5342 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5924 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      996 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:13:32.721857 trytond_product_kit-6.6.5/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4822 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8669 2023-02-27 17:48:09.000000 trytond_product_kit-6.6.5/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:13:32.705190 trytond_product_kit-6.6.5/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4448 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/scenario_product_kit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2043 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/scenario_product_kit_copy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8091 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/scenario_product_kit_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7818 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/scenario_product_kit_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      249 2023-03-04 11:48:18.000000 trytond_product_kit-6.6.5/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:13:32.718524 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-04-01 22:13:31.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2395 2023-04-01 22:13:32.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:13:31.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-04-01 22:13:31.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-15 18:01:32.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-04-01 22:13:31.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:13:31.000000 trytond_product_kit-6.6.5/trytond_product_kit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:13:32.711857 trytond_product_kit-6.6.5/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/product_component_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/product_component_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/purchase_line_component_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/purchase_line_component_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/sale_line_component_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/sale_line_component_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2022-12-19 12:02:50.000000 trytond_product_kit-6.6.5/view/sale_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:26.523783 trytond_product_kit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-05-01 11:02:24.000000 trytond_product_kit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-05-01 11:02:24.000000 trytond_product_kit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2429 2023-05-01 11:43:26.523783 trytond_product_kit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1825 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1880 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17175 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:26.520449 trytond_product_kit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3587 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:26.513783 trytond_product_kit-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6969 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7128 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7056 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6993 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5735 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5756 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7040 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5729 2023-04-30 10:46:36.000000 trytond_product_kit-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10061 2023-04-21 08:36:08.000000 trytond_product_kit-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5342 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5924 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      996 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:43:26.523783 trytond_product_kit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4790 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8663 2023-04-21 08:36:08.000000 trytond_product_kit-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:26.517116 trytond_product_kit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4448 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/scenario_product_kit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2043 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/scenario_product_kit_copy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2406 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/scenario_product_kit_duplicate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8085 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/scenario_product_kit_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7809 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/scenario_product_kit_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      249 2023-05-01 11:02:18.000000 trytond_product_kit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:26.523783 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2429 2023-05-01 11:43:25.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2023-05-01 11:43:26.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:43:25.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-01 11:43:25.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-05-01 11:43:25.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:43:25.000000 trytond_product_kit-6.8.0/trytond_product_kit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:26.520449 trytond_product_kit-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/product_component_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/product_component_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/purchase_line_component_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/purchase_line_component_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/sale_line_component_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/sale_line_component_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_product_kit-6.8.0/view/sale_line_form.xml
```

### Comparing `trytond_product_kit-6.6.5/COPYRIGHT` & `trytond_product_kit-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/LICENSE` & `trytond_product_kit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/PKG-INFO` & `trytond_product_kit-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_product_kit
-Version: 6.6.5
+Version: 6.8.0
 Summary: Tryton module to manage product kits and components
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-kit
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/product_kit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
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
 
 ##################
 Product Kit Module
 ##################
```

### Comparing `trytond_product_kit-6.6.5/__init__.py` & `trytond_product_kit-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/account.py` & `trytond_product_kit-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/common.py` & `trytond_product_kit-6.8.0/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -225,25 +225,28 @@
 
         def get_move(self, type_):
             move = super().get_move(type_)
             if self.components:
                 move = None
             return move
 
-        def get_move_done(self, name):
-            done = super().get_move_done(name)
+        def get_moves_exception(self, name):
+            exception = super().get_moves_exception(name)
             if self.components:
-                done = all(c.move_done for c in self.components)
-            return done
+                exception = any(c.moves_exception for c in self.components)
+            return exception
 
-        def get_move_exception(self, name):
-            exception = super().get_move_exception(name)
+        def get_moves_progress(self, name):
+            progress = super().get_moves_progress(name)
             if self.components:
-                exception = any(c.move_exception for c in self.components)
-            return exception
+                progress = 0
+                for component in self.components:
+                    progress += component.moves_progress
+                progress = round(progress / len(self.components))
+            return progress
 
         def _get_invoice_line_quantity(self):
             quantity = super()._get_invoice_line_quantity()
             if (getattr(self, prefix).invoice_method == 'shipment'
                     and self.components):
                 ratio = min(c.get_moved_ratio() for c in self.components)
                 quantity = self.unit.round(self.quantity * ratio)
@@ -262,18 +265,19 @@
         moves = fields.One2Many('stock.move', 'origin', 'Moves', readonly=True)
         moves_ignored = fields.Many2Many(
             prefix + '.line.component-ignored-stock.move',
             'component', 'move', "Ignored Moves", readonly=True)
         moves_recreated = fields.Many2Many(
             prefix + '.line.component-recreated-stock.move',
             'component', 'move', "Recreated Moves", readonly=True)
-        move_done = fields.Function(
-            fields.Boolean('Moves Done'), 'get_move_done')
-        move_exception = fields.Function(
-            fields.Boolean('Moves Exception'), 'get_move_exception')
+        moves_exception = fields.Function(
+            fields.Boolean('Moves Exception'), 'get_moves_exception')
+        moves_progress = fields.Function(
+            fields.Float("Moves Progress", digits=(1, 4)),
+            'get_moves_progress')
         quantity_ratio = fields.Float(
             "Quantity Ratio", readonly=True,
             states={
                 'required': ~Eval('fixed', False),
                 })
         price_ratio = fields.Numeric(
             "Price Ratio", readonly=True, required=True)
@@ -343,28 +347,28 @@
             quantity = abs(self.quantity)
             for move in self.moves:
                 if move.state == 'done' or move in ignored:
                     quantity -= Uom.compute_qty(
                         move.uom, move.quantity, self.unit)
             return quantity
 
-        def get_move_done(self, name):
-            quantity = self._move_remaining_quantity
-            if quantity is None:
-                return True
-            else:
-                return self.unit.round(quantity) <= 0
-
-        def get_move_exception(self, name):
+        def get_moves_exception(self, name):
             skips = set(self.moves_ignored)
             skips.update(self.moves_recreated)
-            for move in self.moves:
-                if move.state == 'cancelled' and move not in skips:
-                    return True
-            return False
+            return any(
+                m.state == 'cancelled' for m in self.moves if m not in skips)
+
+        def get_moves_progress(self, name):
+            progress = None
+            quantity = self._move_remaining_quantity
+            if quantity is not None and self.quantity:
+                progress = round(
+                    (abs(self.quantity) - quantity) / abs(self.quantity), 4)
+                progress = max(0, min(1, progress))
+            return progress
 
         def get_moved_ratio(self):
             pool = Pool()
             Uom = pool.get('product.uom')
 
             quantity = 0
             for move in self.moves:
```

### Comparing `trytond_product_kit-6.6.5/doc/conf.py` & `trytond_product_kit-6.8.0/doc/conf.py`

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

### Comparing `trytond_product_kit-6.6.5/doc/design.rst` & `trytond_product_kit-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/locale/bg.po` & `trytond_product_kit-6.8.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/ca.po` & `trytond_product_kit-6.8.0/locale/ca.po`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr "Fix"
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr "Línia"
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Moviments finalitzats"
-
-msgctxt "field:purchase.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Moviments en excepció"
-
 msgctxt "field:purchase.line.component,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
+msgctxt "field:purchase.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Moviments en excepció"
+
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Moviments ignorats"
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progres dels moviments"
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Moviments recreats"
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Tipus pare"
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr "Fix"
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr "Línia"
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Moviments finalitzats"
-
-msgctxt "field:sale.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Moviments en excepció"
-
 msgctxt "field:sale.line.component,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
+msgctxt "field:sale.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Moviments en excepció"
+
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Moviments ignorats"
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progres dels moviments"
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Moviments recreats"
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Tipus pare"
```

### Comparing `trytond_product_kit-6.6.5/locale/cs.po` & `trytond_product_kit-6.8.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/de.po` & `trytond_product_kit-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr "Fix"
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr "Position"
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Erledigte Warenbewegungen"
-
-msgctxt "field:purchase.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Warenbewegungen mit Vorbehalt"
-
 msgctxt "field:purchase.line.component,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
+msgctxt "field:purchase.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Warenbewegungen mit Vorbehalt"
+
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignorierte Warenbewegungen"
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Lieferfortschritt"
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Neu erstellte Warenbewegungen"
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Übergeordneter Typ"
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr "Fix"
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr "Position"
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Erledigte Warenbewegungen"
-
-msgctxt "field:sale.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Warenbewegungen mit Vorbehalt"
-
 msgctxt "field:sale.line.component,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
+msgctxt "field:sale.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Warenbewegungen mit Vorbehalt"
+
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Ignorierte Warenbewegungen"
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Lieferfortschritt"
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Neu erstellte Warenbewegungen"
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Übergeordneter Typ"
```

### Comparing `trytond_product_kit-6.6.5/locale/es.po` & `trytond_product_kit-6.8.0/locale/es.po`

 * *Files 8% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr "Fijo"
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr "Línea"
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Movimientos finalizados"
-
-msgctxt "field:purchase.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Movimientos en excepción"
-
 msgctxt "field:purchase.line.component,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
+msgctxt "field:purchase.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Movimientos en excepción"
+
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimientos ignorados"
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progreso de los movimientos"
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Movimientos recreados"
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Tipo padre"
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr "Fijo"
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr "Línea"
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Movimientos finalizados"
-
-msgctxt "field:sale.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Movimientos en excepción"
-
 msgctxt "field:sale.line.component,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
+msgctxt "field:sale.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Movimientos en excepción"
+
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Movimientos ignorados"
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progreso de los movimientos"
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Movimientos recreados"
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Tipo padre"
```

### Comparing `trytond_product_kit-6.6.5/locale/es_419.po` & `trytond_product_kit-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/et.po` & `trytond_product_kit-6.8.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/fa.po` & `trytond_product_kit-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/fi.po` & `trytond_product_kit-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/fr.po` & `trytond_product_kit-6.8.0/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr "Fixe"
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr "Ligne"
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Mouvements effectués"
-
-msgctxt "field:purchase.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Mouvements en exception"
-
 msgctxt "field:purchase.line.component,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
+msgctxt "field:purchase.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mouvements en exception"
+
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Mouvements ignorés"
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progression des mouvements"
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Mouvements recréés"
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Type de parent"
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr "Fixe"
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr "Ligne"
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Mouvements effectués"
-
-msgctxt "field:sale.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Mouvements en exception"
-
 msgctxt "field:sale.line.component,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
+msgctxt "field:sale.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mouvements en exception"
+
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Mouvements ignorés"
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Progression des mouvements"
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Mouvements recréés"
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Type de parent"
```

### Comparing `trytond_product_kit-6.6.5/locale/hu.po` & `trytond_product_kit-6.8.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/id.po` & `trytond_product_kit-6.8.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/it.po` & `trytond_product_kit-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
-msgstr ""
-
-msgctxt "field:sale.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves:"
 msgid "Moves"
 msgstr "Movimenti"
 
+msgctxt "field:sale.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/lo.po` & `trytond_product_kit-6.8.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/lt.po` & `trytond_product_kit-6.8.0/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/nl.po` & `trytond_product_kit-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 msgid "Fixed"
 msgstr "Vast"
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr "Regel"
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Mutaties gereed"
-
-msgctxt "field:purchase.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Mutaties uitzondering"
-
 msgctxt "field:purchase.line.component,moves:"
 msgid "Moves"
-msgstr "beweging"
+msgstr "Mutaties"
+
+msgctxt "field:purchase.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mutaties Uitzondering"
 
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
-msgstr "Genegeerde mutaties"
+msgstr "Genegeerde Mutaties"
+
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Mutaties Voortgang"
 
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Opnieuw aangemaakte mutaties"
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr "Vast"
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr "Regels"
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
-msgstr "Mutaties gereed"
-
-msgctxt "field:sale.line.component,move_exception:"
-msgid "Moves Exception"
-msgstr "Mutaties uitzondering"
-
 msgctxt "field:sale.line.component,moves:"
 msgid "Moves"
 msgstr "Mutaties"
 
+msgctxt "field:sale.line.component,moves_exception:"
+msgid "Moves Exception"
+msgstr "Mutaties Uitzondering"
+
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Genegeerde mutaties"
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr "Mutaties Voortgang"
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Opnieuw aangemaakte mutaties"
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr "Oudertype"
```

### Comparing `trytond_product_kit-6.6.5/locale/pl.po` & `trytond_product_kit-6.8.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/pt.po` & `trytond_product_kit-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/ro.po` & `trytond_product_kit-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/ru.po` & `trytond_product_kit-6.8.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/sl.po` & `trytond_product_kit-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/tr.po` & `trytond_product_kit-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/uk.po` & `trytond_product_kit-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/locale/zh_CN.po` & `trytond_product_kit-6.8.0/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:purchase.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:purchase.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:purchase.line.component,move_exception:"
+msgctxt "field:purchase.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:purchase.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:purchase.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:purchase.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:purchase.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:purchase.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
@@ -142,30 +142,30 @@
 msgid "Fixed"
 msgstr ""
 
 msgctxt "field:sale.line.component,line:"
 msgid "Line"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_done:"
-msgid "Moves Done"
+msgctxt "field:sale.line.component,moves:"
+msgid "Moves"
 msgstr ""
 
-msgctxt "field:sale.line.component,move_exception:"
+msgctxt "field:sale.line.component,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
 
-msgctxt "field:sale.line.component,moves:"
-msgid "Moves"
-msgstr ""
-
 msgctxt "field:sale.line.component,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
+msgctxt "field:sale.line.component,moves_progress:"
+msgid "Moves Progress"
+msgstr ""
+
 msgctxt "field:sale.line.component,moves_recreated:"
 msgid "Recreated Moves"
 msgstr ""
 
 msgctxt "field:sale.line.component,parent_type:"
 msgid "Parent Type"
 msgstr ""
```

### Comparing `trytond_product_kit-6.6.5/product.py` & `trytond_product_kit-6.8.0/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,16 +184,15 @@
                 self.on_change_with_product_unit_category())
             if (not self.unit
                     or self.unit.category != self.product_unit_category):
                 self.unit = self.product.default_uom
 
     @fields.depends('product')
     def on_change_with_product_unit_category(self, name=None):
-        if self.product:
-            return self.product.default_uom.category.id
+        return self.product.default_uom.category if self.product else None
 
     def get_line(self, Line, quantity, unit, **values):
         pool = Pool()
         Uom = pool.get('product.uom')
         line = Line(product=self.product, **values)
         line.unit = self.unit
         if self.fixed:
```

### Comparing `trytond_product_kit-6.6.5/product.xml` & `trytond_product_kit-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/purchase.py` & `trytond_product_kit-6.8.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/purchase.xml` & `trytond_product_kit-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/sale.py` & `trytond_product_kit-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/sale.xml` & `trytond_product_kit-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/setup.py` & `trytond_product_kit-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
 name = 'trytond_product_kit'
 
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
 
@@ -61,23 +61,23 @@
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module to manage product kits and components',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": ('https://docs.tryton.org/projects/'
             'modules-product-kit'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/product_kit',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='',
     package_dir={'trytond.modules.product_kit': '.'},
     packages=(
         ['trytond.modules.product_kit']
         + ['trytond.modules.product_kit.%s' % p
             for p in find_packages()]
@@ -115,23 +115,23 @@
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

### Comparing `trytond_product_kit-6.6.5/stock.py` & `trytond_product_kit-6.8.0/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         SaleLineComponent = pool.get('sale.line.component')
         category = super().on_change_with_product_uom_category(name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to ship and the quantity to invoice.
         # Use getattr as reference field can have negative id
         if (isinstance(self.origin, SaleLineComponent)
                 and getattr(self.origin, 'unit', None)):
-            category = self.origin.unit.category.id
+            category = self.origin.unit.category
         return category
 
     def get_cost_price(self, product_cost_price=None):
         pool = Pool()
         SaleLineComponent = pool.get('sale.line.component')
         Sale = pool.get('sale.sale')
         # For return sale's move use the cost price of the original sale
@@ -195,15 +195,15 @@
         PurchaseLineComponent = pool.get('purchase.line.component')
         category = super().on_change_with_product_uom_category(name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to ship and the quantity to invoice.
         # Use getattr as reference field can have negative id
         if (isinstance(self.origin, PurchaseLineComponent)
                 and getattr(self.origin, 'unit', None)):
-            category = self.origin.unit.category.id
+            category = self.origin.unit.category
         return category
 
     @property
     def origin_name(self):
         pool = Pool()
         PurchaseLineComponent = pool.get('purchase.line.component')
         name = super().origin_name
```

### Comparing `trytond_product_kit-6.6.5/tests/scenario_product_kit.rst` & `trytond_product_kit-6.8.0/tests/scenario_product_kit.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/tests/scenario_product_kit_copy.rst` & `trytond_product_kit-6.8.0/tests/scenario_product_kit_copy.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_kit-6.6.5/tests/scenario_product_kit_purchase.rst` & `trytond_product_kit-6.8.0/tests/scenario_product_kit_purchase.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
@@ -268,15 +268,15 @@
     'cancelled'
     >>> purchase.reload()
     >>> purchase.shipment_state
     'exception'
 
 Handle shipment exception::
 
-    >>> shipment_exception = Wizard('purchase.handle.shipment.exception', [purchase])
+    >>> shipment_exception = purchase.click('handle_shipment_exception')
     >>> shipment_exception.execute('handle')
 
     >>> len(purchase.moves)
     6
     >>> backorder.reload()
     >>> backorder.purchase_exception_state
     'recreated'
```

### Comparing `trytond_product_kit-6.6.5/tests/scenario_product_kit_sale.rst` & `trytond_product_kit-6.8.0/tests/scenario_product_kit_sale.rst`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
     'cancelled'
     >>> sale.reload()
     >>> sale.shipment_state
     'exception'
 
 Handle shipment exception::
 
-    >>> shipment_exception = Wizard('sale.handle.shipment.exception', [sale])
+    >>> shipment_exception = sale.click('handle_shipment_exception')
     >>> move, = [
     ...     m for m in shipment_exception.form.recreate_moves
     ...     if m.product == product1]
     >>> shipment_exception.form.recreate_moves.remove(move)
     >>> shipment_exception.execute('handle')
 
     >>> _, _, shipment = sale.shipments
```

### Comparing `trytond_product_kit-6.6.5/trytond_product_kit.egg-info/PKG-INFO` & `trytond_product_kit-6.8.0/trytond_product_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-product-kit
-Version: 6.6.5
+Version: 6.8.0
 Summary: Tryton module to manage product kits and components
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-kit
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/product_kit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
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
 
 ##################
 Product Kit Module
 ##################
```

### Comparing `trytond_product_kit-6.6.5/trytond_product_kit.egg-info/SOURCES.txt` & `trytond_product_kit-6.8.0/trytond_product_kit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_product_kit.rst
 ./tests/scenario_product_kit_copy.rst
+./tests/scenario_product_kit_duplicate.rst
 ./tests/scenario_product_kit_purchase.rst
 ./tests/scenario_product_kit_sale.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/product_component_form.xml
 ./view/product_component_list.xml
 ./view/product_template_form.xml
@@ -94,14 +95,15 @@
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_product_kit.rst
 tests/scenario_product_kit_copy.rst
+tests/scenario_product_kit_duplicate.rst
 tests/scenario_product_kit_purchase.rst
 tests/scenario_product_kit_sale.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_product_kit.egg-info/PKG-INFO
 trytond_product_kit.egg-info/SOURCES.txt
 trytond_product_kit.egg-info/dependency_links.txt
```

### Comparing `trytond_product_kit-6.6.5/view/product_component_form.xml` & `trytond_product_kit-6.8.0/view/product_component_form.xml`

 * *Files identical despite different names*

