# Comparing `tmp/trytond_account_asset-6.6.1.tar.gz` & `tmp/trytond_account_asset-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_asset-6.6.1.tar", last modified: Sun Feb  5 21:29:12 2023, max compression
+gzip compressed data, was "trytond_account_asset-6.8.0.tar", last modified: Mon May  1 11:47:37 2023, max compression
```

## Comparing `trytond_account_asset-6.6.1.tar` & `trytond_account_asset-6.8.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:29:12.454159 trytond_account_asset-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2235 2023-02-05 21:29:08.000000 trytond_account_asset-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-02-05 21:29:08.000000 trytond_account_asset-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3187 2023-02-05 21:29:12.454159 trytond_account_asset-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1351 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7892 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1065 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    43517 2023-02-05 20:48:28.000000 trytond_account_asset-6.6.1/asset.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11622 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/asset.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    61964 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/asset_table.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:29:12.450825 trytond_account_asset-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3090 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:29:12.444159 trytond_account_asset-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    19721 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20940 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18189 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21368 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21049 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19616 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20298 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22250 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18189 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21098 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18853 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18548 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19852 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23118 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18567 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20824 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18955 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20787 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17768 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19780 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19843 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19753 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17526 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18533 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1552 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3101 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1746 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1749 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1749 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1750 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1766 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1751 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4345 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1111 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:29:12.454159 trytond_account_asset-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4489 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:29:12.444159 trytond_account_asset-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8615 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/scenario_account_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4678 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/scenario_account_asset_depreciated.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3746 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/scenario_purchase_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1645 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      861 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      534 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2022-12-19 12:03:07.000000 trytond_account_asset-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:29:12.454159 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3187 2023-02-05 21:29:11.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3177 2023-02-05 21:29:12.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:29:11.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-02-05 21:29:11.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:29:11.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-02-05 21:29:11.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:29:11.000000 trytond_account_asset-6.6.1/trytond_account_asset.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:29:12.450825 trytond_account_asset-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_create_moves_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2323 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      532 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      617 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_update_show_depreciation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      561 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/asset_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/print_depreciation_table_start.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/revision_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2022-12-19 12:02:48.000000 trytond_account_asset-6.6.1/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:37.506897 trytond_account_asset-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2298 2023-05-01 11:05:07.000000 trytond_account_asset-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-05-01 11:05:06.000000 trytond_account_asset-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3181 2023-05-01 11:47:37.506897 trytond_account_asset-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1351 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7892 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    43401 2023-04-21 08:36:08.000000 trytond_account_asset-6.8.0/asset.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11622 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/asset.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    61964 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/asset_table.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:37.503564 trytond_account_asset-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:37.496897 trytond_account_asset-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19721 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20940 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18189 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21368 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21049 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19616 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20298 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22250 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18189 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21098 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18853 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18548 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19852 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23118 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18567 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20824 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18955 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20787 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17768 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19780 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19843 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19753 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17526 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18533 2023-04-29 08:02:44.000000 trytond_account_asset-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3101 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1746 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1749 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1766 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1751 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4345 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1111 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:37.506897 trytond_account_asset-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4455 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:37.500231 trytond_account_asset-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8537 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/scenario_account_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4600 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/scenario_account_asset_depreciated.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3627 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/scenario_purchase_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1645 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-05-01 11:05:01.000000 trytond_account_asset-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:37.506897 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3181 2023-05-01 11:47:36.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3177 2023-05-01 11:47:37.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:36.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-05-01 11:47:36.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-05-01 11:47:36.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:36.000000 trytond_account_asset-6.8.0/trytond_account_asset.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:37.503564 trytond_account_asset-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/asset_create_moves_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2323 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/asset_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/asset_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/asset_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      532 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/asset_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      617 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/view/asset_update_show_depreciation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/asset_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/view/print_depreciation_table_start.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:14.000000 trytond_account_asset-6.8.0/view/revision_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:20.000000 trytond_account_asset-6.8.0/view/template_form.xml
```

### Comparing `trytond_account_asset-6.6.1/CHANGELOG` & `trytond_account_asset-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-Version 6.6.1 - 2023-02-05
+
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_asset-6.6.1/COPYRIGHT` & `trytond_account_asset-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2012-2022 Nicolas Évrard.
+Copyright (C) 2012-2023 Nicolas Évrard.
 Copyright (C) 2012-2023 Cédric Krier.
 Copyright (C) 2012-2013 Bertrand Chenal.
 Copyright (C) 2012-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `trytond_account_asset-6.6.1/LICENSE` & `trytond_account_asset-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/PKG-INFO` & `trytond_account_asset-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_asset
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for assets management
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_asset
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account asset
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
 
 Account Asset Module
 ####################
 
 The account_asset module adds the depreciation of fixed assets.
```

### Comparing `trytond_account_asset-6.6.1/README.rst` & `trytond_account_asset-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/__init__.py` & `trytond_account_asset-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/account.py` & `trytond_account_asset-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/account.xml` & `trytond_account_asset-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/asset.py` & `trytond_account_asset-6.8.0/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from trytond.model import Index, ModelSQL, ModelView, Unique, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.modules.company import CompanyReport
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
 from trytond.tools import cached_property, grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access, without_check_access
 from trytond.wizard import (
     Button, StateReport, StateTransition, StateView, Wizard)
 
 from .exceptions import PrintDepreciationTableError
 
 
 def date2datetime(date):
@@ -305,16 +305,15 @@
         if self.value is not None and self.depreciated_amount is not None:
             return self.value - self.depreciated_amount
         else:
             return Decimal(0)
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @fields.depends('supplier_invoice_line', 'unit')
     def on_change_supplier_invoice_line(self):
         pool = Pool()
         Currency = pool.get('currency.currency')
         Unit = Pool().get('product.uom')
 
@@ -346,17 +345,15 @@
             self.quantity = invoice_line.quantity
         else:
             self.quantity = Unit.compute_qty(invoice_line.unit,
                 invoice_line.quantity, self.unit)
 
     @fields.depends('product')
     def on_change_with_unit(self):
-        if not self.product:
-            return None
-        return self.product.default_uom.id
+        return self.product.default_uom if self.product else None
 
     @fields.depends('end_date', 'product', 'start_date')
     def on_change_with_end_date(self):
         if (all(getattr(self, k, None) for k in ('product', 'start_date'))
                 and not self.end_date):
             if self.product.depreciation_duration:
                 duration = relativedelta.relativedelta(
@@ -530,15 +527,15 @@
         Return the account.move generated by an asset line.
         """
         pool = Pool()
         Period = pool.get('account.period')
         Move = pool.get('account.move')
         MoveLine = pool.get('account.move.line')
 
-        period_id = Period.find(self.company.id, line.date)
+        period = Period.find(self.company, line.date)
         with Transaction().set_context(date=line.date):
             expense_line = MoveLine(
                 credit=0,
                 debit=line.depreciation,
                 account=self.product.account_expense_used,
                 )
             depreciation_line = MoveLine(
@@ -546,15 +543,15 @@
                 credit=line.depreciation,
                 account=self.product.account_depreciation_used,
                 )
 
         return Move(
             company=self.company,
             origin=line,
-            period=period_id,
+            period=period,
             journal=self.account_journal,
             date=line.date,
             lines=[expense_line, depreciation_line],
             )
 
     @classmethod
     def create_moves(cls, assets, date):
@@ -592,15 +589,15 @@
         Date = pool.get('ir.date')
         Move = pool.get('account.move')
         MoveLine = pool.get('account.move.line')
 
         if date is None:
             with Transaction().set_context(company=self.company.id):
                 date = Date.today()
-        period_id = Period.find(self.company.id, date)
+        period = Period.find(self.company, date)
         if self.supplier_invoice_line:
             account_asset = self.supplier_invoice_line.account.current()
         else:
             account_asset = self.product.account_asset_used
 
         asset_line = MoveLine(
             debit=0,
@@ -622,15 +619,15 @@
                 credit=-square_amount if square_amount < 0 else 0,
                 account=account,
                 )
             lines.append(counter_part_line)
         return Move(
             company=self.company,
             origin=self,
-            period=period_id,
+            period=period,
             journal=self.account_journal,
             date=date,
             lines=lines,
             )
 
     @classmethod
     def set_number(cls, assets):
@@ -755,16 +752,15 @@
     def __setup__(cls):
         super(AssetLine, cls).__setup__()
         cls.__access__.add('asset')
         cls._order.insert(0, ('date', 'ASC'))
 
     @fields.depends('asset', '_parent_asset.currency')
     def on_change_with_currency(self, name=None):
-        if self.asset:
-            return self.asset.currency.id
+        return self.asset.currency if self.asset else None
 
 
 class AssetUpdateMove(ModelSQL):
     'Asset - Update - Move'
     __name__ = 'account.asset-update-account.move'
     asset = fields.Many2One(
         'account.asset', "Asset", ondelete='CASCADE', required=True)
@@ -788,17 +784,19 @@
     start = StateView('account.asset.create_moves.start',
         'account_asset.asset_create_moves_start_view_form', [
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('OK', 'create_moves', 'tryton-ok', True),
             ])
     create_moves = StateTransition()
 
+    @without_check_access
     def transition_create_moves(self):
-        Asset = Pool().get('account.asset')
-        with Transaction().set_context(_check_access=True):
+        pool = Pool()
+        with check_access():
+            Asset = pool.get('account.asset')
             assets = Asset.search([
                     ('state', '=', 'running'),
                     ])
         assets = Asset.browse(assets)
         Asset.create_moves(assets, self.start.date)
         return 'end'
 
@@ -880,22 +878,24 @@
                 self.record),
             }
 
     def get_move(self, asset):
         pool = Pool()
         Period = pool.get('account.period')
         Move = pool.get('account.move')
-        period_id = Period.find(asset.company.id, self.show_move.date)
-        return Move(
+        period = Period.find(asset.company, self.show_move.date)
+        move = Move(
             company=asset.company,
             origin=asset,
             journal=asset.account_journal.id,
-            period=period_id,
+            period=period,
             date=self.show_move.date,
             )
+        move.lines = self.get_move_lines(asset)
+        return move
 
     def get_move_lines(self, asset):
         MoveLine = Pool().get('account.move.line')
         expense_line = MoveLine(
             account=self.show_move.counterpart_account,
             credit=self.show_move.amount if self.show_move.amount > 0 else 0,
             debit=-self.show_move.amount if self.show_move.amount < 0 else 0,
@@ -912,15 +912,14 @@
         Move = pool.get('account.move')
 
         latest_move_date = self.show_move.latest_move_date
         next_date = self.show_move.next_depreciation_date
         if not (latest_move_date <= self.show_move.date <= next_date):
             raise ValueError('The update move date is invalid')
         move = self.get_move(self.record)
-        move.lines = self.get_move_lines(self.record)
         move.save()
         self.model.write([self.record], {
                 'update_moves': [('add', [move.id])],
                 })
         Move.post([move])
         return 'create_lines'
 
@@ -957,16 +956,15 @@
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('asset')
 
     @fields.depends('asset', '_parent_asset.currency')
     def on_change_with_currency(self, name=None):
-        if self.asset and self.asset.currency:
-            return self.asset.currency.id
+        return self.asset.currency if self.asset else None
 
     @fields.depends('origin', 'value', 'asset', '_parent_asset.value')
     def on_change_origin(self, name=None):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
         if isinstance(self.origin, InvoiceLine) and self.origin.id >= 0:
             self.value = self.asset.value + self.origin.amount
@@ -1174,29 +1172,29 @@
     start = StateView('account.asset.print_depreciation_table.start',
         'account_asset.print_depreciation_table_start_view_form', [
             Button('Cancel', 'end', 'tryton-cancel'),
             Button('Print', 'print_', 'tryton-print', default=True),
             ])
     print_ = StateReport('account.asset.depreciation_table')
 
+    @check_access
     def do_print_(self, action):
         pool = Pool()
         Asset = pool.get('account.asset')
-        with Transaction().set_context(_check_access=True):
-            assets = Asset.search([
-                    ['OR',
-                        ('purchase_date', '<=', self.start.end_date),
-                        ('start_date', '<=', self.start.end_date),
-                        ],
-                    ['OR',
-                        ('move', '=', None),
-                        ('move.date', '>=', self.start.start_date),
-                        ],
-                    ('state', '!=', 'draft'),
-                    ])
+        assets = Asset.search([
+                ['OR',
+                    ('purchase_date', '<=', self.start.end_date),
+                    ('start_date', '<=', self.start.end_date),
+                    ],
+                ['OR',
+                    ('move', '=', None),
+                    ('move.date', '>=', self.start.start_date),
+                    ],
+                ('state', '!=', 'draft'),
+                ])
         if not assets:
             raise PrintDepreciationTableError(
                 gettext('account_asset.msg_no_assets'))
         return action, {
             'ids': [a.id for a in assets],
             'start_date': self.start.start_date,
             'end_date': self.start.end_date,
```

### Comparing `trytond_account_asset-6.6.1/asset.xml` & `trytond_account_asset-6.8.0/asset.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/asset_table.fodt` & `trytond_account_asset-6.8.0/asset_table.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/doc/conf.py` & `trytond_account_asset-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_asset-6.6.1/doc/index.rst` & `trytond_account_asset-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/invoice.py` & `trytond_account_asset-6.8.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/bg.po` & `trytond_account_asset-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/ca.po` & `trytond_account_asset-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/cs.po` & `trytond_account_asset-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/de.po` & `trytond_account_asset-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/es.po` & `trytond_account_asset-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/es_419.po` & `trytond_account_asset-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/et.po` & `trytond_account_asset-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/fa.po` & `trytond_account_asset-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/fi.po` & `trytond_account_asset-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/fr.po` & `trytond_account_asset-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/hu.po` & `trytond_account_asset-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/id.po` & `trytond_account_asset-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/it.po` & `trytond_account_asset-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/lo.po` & `trytond_account_asset-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/lt.po` & `trytond_account_asset-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/nl.po` & `trytond_account_asset-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/pl.po` & `trytond_account_asset-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/pt.po` & `trytond_account_asset-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/ro.po` & `trytond_account_asset-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/ru.po` & `trytond_account_asset-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/sl.po` & `trytond_account_asset-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/tr.po` & `trytond_account_asset-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/uk.po` & `trytond_account_asset-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/locale/zh_CN.po` & `trytond_account_asset-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/message.xml` & `trytond_account_asset-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart.xml` & `trytond_account_asset-6.8.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_bg.xml` & `trytond_account_asset-6.8.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_ca.xml` & `trytond_account_asset-6.8.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_de.xml` & `trytond_account_asset-6.8.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_en.xml` & `trytond_account_asset-6.8.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_es.xml` & `trytond_account_asset-6.8.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_fr.xml` & `trytond_account_asset-6.8.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_nl.xml` & `trytond_account_asset-6.8.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_pt.xml` & `trytond_account_asset-6.8.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_ru.xml` & `trytond_account_asset-6.8.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/minimal_chart_sl.xml` & `trytond_account_asset-6.8.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/product.py` & `trytond_account_asset-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/product.xml` & `trytond_account_asset-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/purchase.py` & `trytond_account_asset-6.8.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/setup.py` & `trytond_account_asset-6.8.0/setup.py`

 * *Files 4% similar despite different names*

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
@@ -34,16 +31,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_asset'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-dateutil', 'python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -51,22 +51,22 @@
     get_require_version('trytond_purchase')]
 
 setup(name=name,
     version=version,
     description='Tryton module for assets management',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_asset',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account asset',
     package_dir={'trytond.modules.account_asset': '.'},
     packages=(
         ['trytond.modules.account_asset']
         + ['trytond.modules.account_asset.%s' % p for p in find_packages()]
         ),
@@ -103,24 +103,24 @@
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

### Comparing `trytond_account_asset-6.6.1/tests/scenario_account_asset.rst` & `trytond_account_asset-6.8.0/tests/scenario_account_asset.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 ======================
 Account Asset Scenario
 ======================
 
 Imports::
 
-    >>> import datetime
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.account_asset.tests.tools \
     ...     import add_asset_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_asset')
 
 Create company::
 
@@ -94,15 +92,15 @@
     >>> invoice_line = InvoiceLine()
     >>> supplier_invoice.lines.append(invoice_line)
     >>> invoice_line.product = asset_product
     >>> invoice_line.quantity = 1
     >>> invoice_line.unit_price = Decimal('1000')
     >>> invoice_line.account == asset_account
     True
-    >>> supplier_invoice.invoice_date = today + relativedelta(day=1, month=1)
+    >>> supplier_invoice.invoice_date = fiscalyear.start_date
     >>> supplier_invoice.click('post')
     >>> supplier_invoice.state
     'posted'
     >>> invoice_line, = supplier_invoice.lines
     >>> (asset_account.debit, asset_account.credit) == \
     ...     (Decimal('1000'), Decimal('0'))
     True
```

### Comparing `trytond_account_asset-6.6.1/tests/scenario_account_asset_depreciated.rst` & `trytond_account_asset-6.8.0/tests/scenario_account_asset_depreciated.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 ==================================
 Account Asset Depreciated Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.account_asset.tests.tools \
     ...     import add_asset_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_asset')
 
 Create company::
 
@@ -73,15 +71,15 @@
 Depreciate the asset::
 
     >>> Asset = Model.get('account.asset')
     >>> asset = Asset()
     >>> asset.product = asset_product
     >>> asset.value = Decimal('1500.00')
     >>> asset.depreciated_amount = Decimal('500.00')
-    >>> asset.start_date = today + relativedelta(day=1, month=1)
+    >>> asset.start_date = fiscalyear.start_date
     >>> asset.purchase_date = asset.start_date
     >>> asset.end_date = (asset.start_date +
     ...     relativedelta(years=2, days=-1))
     >>> asset.quantity = 1
     >>> asset.residual_value = Decimal('100')
     >>> asset.click('create_lines')
     >>> len(asset.lines)
```

### Comparing `trytond_account_asset-6.6.1/tests/scenario_purchase_asset.rst` & `trytond_account_asset-6.8.0/tests/scenario_purchase_asset.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 =======================
 Purchase Asset Scenario
 =======================
 
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
     ...     set_fiscalyear_invoice_sequences
     >>> from trytond.modules.account_asset.tests.tools \
     ...     import add_asset_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_asset', 'purchase'])
 
 Create company::
```

### Comparing `trytond_account_asset-6.6.1/tests/test_module.py` & `trytond_account_asset-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/tests/tools.py` & `trytond_account_asset-6.8.0/tests/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model
-
 from trytond.modules.company.tests.tools import get_company
 
 
 def add_asset_accounts(accounts, company=None, config=None):
     "Add asset kind to accounts"
     Account = Model.get('account.account', config=config)
```

### Comparing `trytond_account_asset-6.6.1/trytond_account_asset.egg-info/PKG-INFO` & `trytond_account_asset-6.8.0/trytond_account_asset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-asset
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for assets management
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_asset
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account asset
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
 
 Account Asset Module
 ####################
 
 The account_asset module adds the depreciation of fixed assets.
```

### Comparing `trytond_account_asset-6.6.1/trytond_account_asset.egg-info/SOURCES.txt` & `trytond_account_asset-6.8.0/trytond_account_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/asset_form.xml` & `trytond_account_asset-6.8.0/view/asset_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/asset_line_form.xml` & `trytond_account_asset-6.8.0/view/asset_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/asset_tree.xml` & `trytond_account_asset-6.8.0/view/asset_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/asset_update_show_depreciation_form.xml` & `trytond_account_asset-6.8.0/view/asset_update_show_depreciation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/asset_update_start_form.xml` & `trytond_account_asset-6.8.0/view/asset_update_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/configuration_form.xml` & `trytond_account_asset-6.8.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_asset-6.6.1/view/template_form.xml` & `trytond_account_asset-6.8.0/view/template_form.xml`

 * *Files identical despite different names*

