# Comparing `tmp/trytond_commission-6.6.1.tar.gz` & `tmp/trytond_commission-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_commission-6.6.1.tar", last modified: Sat Mar  4 11:59:28 2023, max compression
+gzip compressed data, was "trytond_commission-6.8.0.tar", last modified: Mon May  1 11:52:46 2023, max compression
```

## Comparing `trytond_commission-6.6.1.tar` & `trytond_commission-6.8.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.554843 trytond_commission-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2363 2023-03-04 11:59:23.000000 trytond_commission-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-03-04 11:59:23.000000 trytond_commission-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2517 2023-03-04 11:59:28.554843 trytond_commission-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22653 2023-02-27 17:43:57.000000 trytond_commission-6.6.1/commission.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14458 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/commission.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7545 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/commission_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8742 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/commission_reporting.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.534843 trytond_commission-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      872 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.534843 trytond_commission-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/icons/tryton-commission.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     9082 2023-02-27 17:43:57.000000 trytond_commission-6.6.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3713 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/invoice.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.464842 trytond_commission-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16314 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17192 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15228 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17627 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17297 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14178 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15826 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17040 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15215 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17520 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15741 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14712 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16162 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16499 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15442 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17601 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15612 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14376 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16267 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16122 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15215 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14133 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15454 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1193 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3639 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:59:28.554843 trytond_commission-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4727 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2131 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1154 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/stock_reporting_margin.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.478175 trytond_commission-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tests/scenario_agent_selection.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7370 2023-02-27 17:43:57.000000 trytond_commission-6.6.1/tests/scenario_commission.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3896 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tests/scenario_commission_credit_posted_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5799 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tests/scenario_commission_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3670 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2022-12-19 12:03:07.000000 trytond_commission-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.548176 trytond_commission-6.6.1/trytond_commission.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2517 2023-03-04 11:59:27.000000 trytond_commission-6.6.1/trytond_commission.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4120 2023-03-04 11:59:28.000000 trytond_commission-6.6.1/trytond_commission.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:59:27.000000 trytond_commission-6.6.1/trytond_commission.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-03-04 11:59:27.000000 trytond_commission-6.6.1/trytond_commission.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:59:27.000000 trytond_commission-6.6.1/trytond_commission.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-03-04 11:59:27.000000 trytond_commission-6.6.1/trytond_commission.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:59:27.000000 trytond_commission-6.6.1/trytond_commission.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:59:28.524843 trytond_commission-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/account_invoice_credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/agent_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/agent_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/agent_selection_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/agent_selection_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/agent_selection_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/commission_create_invoice_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/commission_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/commission_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/plan_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/plan_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/plan_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/plan_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/plan_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_agent_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_agent_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_agent_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_agent_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_agent_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_agent_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/stock_reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-12-19 12:02:49.000000 trytond_commission-6.6.1/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.497398 trytond_commission-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2469 2023-05-01 11:08:39.000000 trytond_commission-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:08:38.000000 trytond_commission-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2514 2023-05-01 11:52:46.494065 trytond_commission-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22624 2023-04-21 08:36:08.000000 trytond_commission-6.8.0/commission.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14458 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/commission.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/commission_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8742 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/commission_reporting.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.490732 trytond_commission-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      872 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.494065 trytond_commission-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/icons/tryton-commission.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     9082 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3713 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/invoice.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.477398 trytond_commission-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16314 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17192 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15228 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17627 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17297 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14178 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15826 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17040 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15215 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17532 2023-04-30 10:46:36.000000 trytond_commission-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15741 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14712 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16162 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16499 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15442 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17601 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15612 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14377 2023-04-30 10:46:36.000000 trytond_commission-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16267 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16122 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15215 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14133 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15454 2023-04-29 08:02:45.000000 trytond_commission-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      682 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1193 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3639 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:52:46.497398 trytond_commission-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4696 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2131 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1154 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/stock_reporting_margin.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.480732 trytond_commission-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/scenario_agent_selection.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7332 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/scenario_commission.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3896 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/scenario_commission_credit_posted_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5819 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/scenario_commission_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3670 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-05-01 11:08:33.000000 trytond_commission-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.494065 trytond_commission-6.8.0/trytond_commission.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2514 2023-05-01 11:52:45.000000 trytond_commission-6.8.0/trytond_commission.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4120 2023-05-01 11:52:46.000000 trytond_commission-6.8.0/trytond_commission.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:52:45.000000 trytond_commission-6.8.0/trytond_commission.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:52:45.000000 trytond_commission-6.8.0/trytond_commission.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_commission-6.8.0/trytond_commission.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-05-01 11:52:45.000000 trytond_commission-6.8.0/trytond_commission.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:52:45.000000 trytond_commission-6.8.0/trytond_commission.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:46.490732 trytond_commission-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/account_invoice_credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/agent_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/agent_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/agent_selection_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/agent_selection_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/agent_selection_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/commission_create_invoice_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/commission_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/commission_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/plan_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/plan_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/plan_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/plan_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/plan_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_agent_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_agent_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_agent_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_agent_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_agent_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_agent_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_commission-6.8.0/view/stock_reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_commission-6.8.0/view/template_form.xml
```

### Comparing `trytond_commission-6.6.1/CHANGELOG` & `trytond_commission-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Allow searching reporting records by name
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow creating manual commission
 * Include commission to stock margin report
```

### Comparing `trytond_commission-6.6.1/COPYRIGHT` & `trytond_commission-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/LICENSE` & `trytond_commission-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/PKG-INFO` & `trytond_commission-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_commission
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for commission
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
-Project-URL: Source Code, https://hg.tryton.org/modules/commission
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton commission
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
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 #################
 Commission Module
 #################
```

### Comparing `trytond_commission-6.6.1/__init__.py` & `trytond_commission-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/commission.py` & `trytond_commission-6.8.0/commission.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from trytond.model import (
     MatchMixin, ModelSQL, ModelView, fields, sequence_ordered)
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits, round_price
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, Id, If
 from trytond.tools import decistmt, grouped_slice, reduce_ids
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 from trytond.wizard import Button, StateAction, StateView, Wizard
 
 from .exceptions import FormulaError
 
 
 class Agent(ModelSQL, ModelView):
     'Commission Agent'
@@ -182,16 +182,15 @@
         super().__setup__()
         cls.__access__.add('agent')
         cls._order.insert(0, ('party', 'ASC NULLS LAST'))
         cls._order.insert(1, ('employee', 'ASC NULLS LAST'))
 
     @fields.depends('agent', '_parent_agent.company')
     def on_change_with_company(self, name=None):
-        if self.agent:
-            return self.agent.company.id
+        return self.agent.company if self.agent else None
 
     @classmethod
     def search_company(cls, name, clause):
         return [('agent.' + clause[0],) + tuple(clause[1:])]
 
     def match(self, pattern):
         pool = Pool()
@@ -405,16 +404,15 @@
                 and self.base_amount is None):
             return Currency.compute(
                 self.origin.invoice.currency, self.origin.amount,
                 self.agent.currency, round=False)
 
     @fields.depends('agent')
     def on_change_with_currency(self, name=None):
-        if self.agent:
-            return self.agent.currency.id
+        return self.agent.currency if self.agent else None
 
     @fields.depends('agent')
     def on_change_with_type_(self, name=None):
         if self.agent:
             return {
                 'agent': 'out',
                 'principal': 'in',
@@ -595,15 +593,15 @@
             agents = [agent.id for agent in self.ask.agents]
             domain.append(('agent', 'in', agents))
         return domain
 
     def do_create_(self, action):
         pool = Pool()
         Commission = pool.get('commission')
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             commissions = Commission.search(self.get_domain(),
                 order=[('agent', 'DESC'), ('date', 'DESC')])
         commissions = Commission.browse(commissions)
         Commission.invoice(commissions)
         invoice_ids = list({c.invoice_line.invoice.id for c in commissions})
         return action, {'res_id': invoice_ids}
```

### Comparing `trytond_commission-6.6.1/commission.xml` & `trytond_commission-6.8.0/commission.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/commission_reporting.py` & `trytond_commission-6.8.0/commission_reporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,21 @@
                     getattr(ts, name, 0) or 0
                     for ts in self.time_series_all])
             return chart.render_sparktext()
 
     def get_currency(self, name):
         return self.agent.currency.id
 
+    def get_rec_name(self, name):
+        return self.agent.rec_name
+
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('agent.rec_name', *clause[1:])]
+
 
 class AgentTimeseries(Agent):
     "Commission Reporting per Agent"
     __name__ = 'commission.reporting.agent.time_series'
 
     date = fields.Date("Date")
     time_series = None
```

### Comparing `trytond_commission-6.6.1/commission_reporting.xml` & `trytond_commission-6.8.0/commission_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/doc/conf.py` & `trytond_commission-6.8.0/doc/conf.py`

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

### Comparing `trytond_commission-6.6.1/doc/design.rst` & `trytond_commission-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/doc/usage.rst` & `trytond_commission-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/icons/LICENSE` & `trytond_commission-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/icons/tryton-commission.svg` & `trytond_commission-6.8.0/icons/tryton-commission.svg`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/invoice.py` & `trytond_commission-6.8.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/invoice.xml` & `trytond_commission-6.8.0/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/ir.py` & `trytond_commission-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/bg.po` & `trytond_commission-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/ca.po` & `trytond_commission-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/cs.po` & `trytond_commission-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/de.po` & `trytond_commission-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/es.po` & `trytond_commission-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/es_419.po` & `trytond_commission-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/et.po` & `trytond_commission-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/fa.po` & `trytond_commission-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/fi.po` & `trytond_commission-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/fr.po` & `trytond_commission-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -610,15 +610,15 @@
 
 msgctxt "selection:commission.plan,commission_method:"
 msgid "On Payment"
 msgstr "Au paiement"
 
 msgctxt "selection:commission.plan,commission_method:"
 msgid "On Posting"
-msgstr "Au postage"
+msgstr "À la comptabilisation"
 
 msgctxt "selection:commission.reporting.context,period:"
 msgid "Day"
 msgstr "Jour"
 
 msgctxt "selection:commission.reporting.context,period:"
 msgid "Month"
```

### Comparing `trytond_commission-6.6.1/locale/hu.po` & `trytond_commission-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/id.po` & `trytond_commission-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/it.po` & `trytond_commission-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/lo.po` & `trytond_commission-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/lt.po` & `trytond_commission-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/nl.po` & `trytond_commission-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/pl.po` & `trytond_commission-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/pt.po` & `trytond_commission-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/ro.po` & `trytond_commission-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 #, fuzzy
 msgctxt "field:commission,base_amount:"
 msgid "Base Amount"
 msgstr "Suma"
 
 msgctxt "field:commission,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:commission,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:commission,invoice_line:"
 msgid "Invoice Line"
```

### Comparing `trytond_commission-6.6.1/locale/ru.po` & `trytond_commission-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/sl.po` & `trytond_commission-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/tr.po` & `trytond_commission-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/uk.po` & `trytond_commission-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/locale/zh_CN.po` & `trytond_commission-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/message.xml` & `trytond_commission-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/party.py` & `trytond_commission-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/product.py` & `trytond_commission-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/sale.py` & `trytond_commission-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/sale.xml` & `trytond_commission-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/setup.py` & `trytond_commission-6.8.0/setup.py`

 * *Files 6% similar despite different names*

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
 name = 'trytond_commission'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['simpleeval', 'python-sql', 'python-dateutil']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -58,22 +58,22 @@
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module for commission',
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
-        "Source Code": 'https://hg.tryton.org/modules/commission',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton commission',
     package_dir={'trytond.modules.commission': '.'},
     packages=(
         ['trytond.modules.commission']
         + ['trytond.modules.commission.%s' % p for p in find_packages()]
         ),
@@ -110,24 +110,24 @@
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
         'sparklines': ['pygal'],
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
```

### Comparing `trytond_commission-6.6.1/stock.py` & `trytond_commission-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/stock_reporting_margin.py` & `trytond_commission-6.8.0/stock_reporting_margin.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/stock_reporting_margin.xml` & `trytond_commission-6.8.0/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/tests/scenario_agent_selection.rst` & `trytond_commission-6.8.0/tests/scenario_agent_selection.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ========================
 Agent Selection Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, get_accounts)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules(['commission', 'sale'])
 
 Create company::
```

### Comparing `trytond_commission-6.6.1/tests/scenario_commission.rst` & `trytond_commission-6.8.0/tests/scenario_commission.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ===================
 Commission Scenario
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
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts, create_tax
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('commission')
 
     >>> ReportingAgent = Model.get('commission.reporting.agent')
     >>> ReportingAgentTimeseries = Model.get('commission.reporting.agent.time_series')
@@ -29,15 +29,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, (today, tomorrow)))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_commission-6.6.1/tests/scenario_commission_credit_posted_invoice.rst` & `trytond_commission-6.8.0/tests/scenario_commission_credit_posted_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/tests/scenario_commission_stock.rst` & `trytond_commission-6.8.0/tests/scenario_commission_stock.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, (yesterday, today)))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_commission-6.6.1/tests/test_module.py` & `trytond_commission-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/trytond_commission.egg-info/PKG-INFO` & `trytond_commission-6.8.0/trytond_commission.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-commission
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for commission
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
-Project-URL: Source Code, https://hg.tryton.org/modules/commission
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton commission
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
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 #################
 Commission Module
 #################
```

### Comparing `trytond_commission-6.6.1/trytond_commission.egg-info/SOURCES.txt` & `trytond_commission-6.8.0/trytond_commission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/view/agent_selection_form.xml` & `trytond_commission-6.8.0/view/agent_selection_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/view/commission_form.xml` & `trytond_commission-6.8.0/view/commission_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/view/invoice_line_form.xml` & `trytond_commission-6.8.0/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/view/plan_line_form.xml` & `trytond_commission-6.8.0/view/plan_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_commission-6.6.1/view/reporting_context_form.xml` & `trytond_commission-6.8.0/view/reporting_context_form.xml`

 * *Files identical despite different names*

