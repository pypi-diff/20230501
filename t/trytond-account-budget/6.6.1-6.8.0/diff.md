# Comparing `tmp/trytond_account_budget-6.6.1.tar.gz` & `tmp/trytond_account_budget-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_budget-6.6.1.tar", last modified: Fri Feb 17 18:54:42 2023, max compression
+gzip compressed data, was "trytond_account_budget-6.8.0.tar", last modified: Mon May  1 11:45:09 2023, max compression
```

## Comparing `trytond_account_budget-6.6.1.tar` & `trytond_account_budget-6.8.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:54:42.110468 trytond_account_budget-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-02-17 18:54:38.000000 trytond_account_budget-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-02-17 18:54:38.000000 trytond_account_budget-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2628 2023-02-17 18:54:42.110468 trytond_account_budget-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29394 2023-02-09 23:32:13.000000 trytond_account_budget-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10646 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:54:42.107135 trytond_account_budget-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1610 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1258 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:54:42.097135 trytond_account_budget-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10355 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10701 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10398 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10285 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8446 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8354 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10411 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8266 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      822 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-17 18:54:42.110468 trytond_account_budget-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4638 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:54:42.100468 trytond_account_budget-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6079 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/tests/scenario_account_budget.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2022-12-19 12:03:07.000000 trytond_account_budget-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:54:42.110468 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2628 2023-02-17 18:54:41.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-02-17 18:54:42.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-17 18:54:41.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-02-17 18:54:41.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-17 18:54:41.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-02-17 18:54:41.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-17 18:54:41.000000 trytond_account_budget-6.6.1/trytond_account_budget.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-17 18:54:42.103801 trytond_account_budget-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_copy_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_form_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      563 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_period_list_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_line_tree_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2022-12-19 12:02:48.000000 trytond_account_budget-6.6.1/view/budget_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:09.168390 trytond_account_budget-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      497 2023-05-01 11:03:29.000000 trytond_account_budget-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-05-01 11:03:28.000000 trytond_account_budget-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-01 11:45:09.168390 trytond_account_budget-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29824 2023-04-21 08:36:08.000000 trytond_account_budget-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10646 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:09.165057 trytond_account_budget-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:09.155056 trytond_account_budget-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10355 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10701 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10398 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10300 2023-04-30 10:46:36.000000 trytond_account_budget-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8446 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8354 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10411 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8266 2023-04-29 08:02:43.000000 trytond_account_budget-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      822 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:45:09.168390 trytond_account_budget-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4603 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:09.158390 trytond_account_budget-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6047 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/tests/scenario_account_budget.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-05-01 11:03:22.000000 trytond_account_budget-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:09.168390 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-01 11:45:08.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-05-01 11:45:09.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:45:08.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:45:08.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-05-01 11:45:08.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:45:08.000000 trytond_account_budget-6.8.0/trytond_account_budget.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:09.161723 trytond_account_budget-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_copy_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_form_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      563 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-28 07:46:16.000000 trytond_account_budget-6.8.0/view/budget_line_period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-04-28 07:46:16.000000 trytond_account_budget-6.8.0/view/budget_line_period_list_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_line_tree_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:14.000000 trytond_account_budget-6.8.0/view/budget_list.xml
```

### Comparing `trytond_account_budget-6.6.1/COPYRIGHT` & `trytond_account_budget-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/LICENSE` & `trytond_account_budget-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/PKG-INFO` & `trytond_account_budget-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_budget
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module that allows budgets to be setup for accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-budget
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_budget
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account budget
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
 
 #####################
 Account Budget Module
 #####################
```

### Comparing `trytond_account_budget-6.6.1/__init__.py` & `trytond_account_budget-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/account.py` & `trytond_account_budget-6.8.0/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from sql.aggregate import Sum
 from sql.conditionals import Coalesce
 
 from trytond.i18n import gettext
 from trytond.model import (
     Index, ModelSQL, ModelView, Unique, fields, sequence_ordered, tree)
+from trytond.modules.account.exceptions import FiscalYearNotFoundError
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
 from trytond.rpc import RPC
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.transaction import Transaction
 from trytond.wizard import (
@@ -178,21 +179,20 @@
 
     @classmethod
     def default_right(cls):
         return 0
 
     @fields.depends('budget', '_parent_budget.company')
     def on_change_with_company(self, name=None):
-        if self.budget and self.budget.company:
-            return self.budget.company.id
+        return self.budget.company if self.budget else None
 
     @fields.depends('budget', '_parent_budget.company')
     def on_change_with_currency(self, name=None):
         if self.budget and self.budget.company:
-            return self.budget.company.currency.id
+            return self.budget.company.currency
 
     @classmethod
     def get_total_amount(cls, records, name):
         transaction = Transaction()
         cursor = transaction.connection.cursor()
         table = cls.__table__()
         children = cls.__table__()
@@ -242,16 +242,14 @@
 
     @classmethod
     def copy(cls, records, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
-        default.setdefault('left', 0)
-        default.setdefault('right', 0)
         if 'budget' in default and 'children.budget' not in default:
             default['children.budget'] = default['budget']
         if 'amount' in default and 'children.amount' not in default:
             default['children.amount'] = default['amount']
         return super().copy(records, default=default)
 
 
@@ -278,27 +276,29 @@
     def default_budget(cls):
         pool = Pool()
         Budget = pool.get('account.budget')
         FiscalYear = pool.get('account.fiscalyear')
         context = Transaction().context
         if 'budget' in context:
             return context.get('budget')
-        fiscalyear_id = FiscalYear.find(
-            context.get('company'), exception=False)
+        try:
+            fiscalyear = FiscalYear.find(
+                context.get('company'), test_state=False)
+        except FiscalYearNotFoundError:
+            return None
         budgets = Budget.search([
-                ('fiscalyear', '=', fiscalyear_id),
+                ('fiscalyear', '=', fiscalyear.id),
                 ], limit=1)
         if budgets:
             budget, = budgets
             return budget.id
 
     @fields.depends('budget')
     def on_change_with_fiscalyear(self, name=None):
-        if self.budget:
-            return self.budget.fiscalyear.id
+        return self.budget.fiscalyear if self.budget else None
 
 
 class Budget(BudgetMixin, ModelSQL, ModelView):
     "Account Budget"
     __name__ = 'account.budget'
 
     fiscalyear = fields.Many2One(
@@ -329,16 +329,31 @@
                 'copy_button': {},
                 })
 
     @classmethod
     def default_fiscalyear(cls):
         pool = Pool()
         FiscalYear = pool.get('account.fiscalyear')
-        context = Transaction().context
-        return FiscalYear.find(context.get('company'), exception=False)
+        try:
+            fiscalyear = FiscalYear.find(
+                cls.default_company(), test_state=False)
+        except FiscalYearNotFoundError:
+            return None
+        return fiscalyear.id
+
+    @fields.depends('company', 'fiscalyear')
+    def on_change_company(self):
+        pool = Pool()
+        FiscalYear = pool.get('account.fiscalyear')
+        if not self.fiscalyear or self.fiscalyear.company != self.company:
+            try:
+                self.fiscalyear = FiscalYear.find(
+                    self.company, test_state=False)
+            except FiscalYearNotFoundError:
+                pass
 
     def get_rec_name(self, name):
         return '%s - %s' % (self.name, self.fiscalyear.rec_name)
 
     @classmethod
     def search_rec_name(cls, name, clause):
         if clause[1].startswith('!') or clause[1].startswith('not '):
@@ -480,16 +495,15 @@
             })
         cls.__rpc__.update({
                 'create_period': RPC(readonly=False, instantiate=0),
                 })
 
     @fields.depends('parent', '_parent_parent.account_type')
     def on_change_with_parent_account_type(self, name=None):
-        if self.parent and self.parent.account_type:
-            return self.parent.account_type.id
+        return self.parent.account_type if self.parent else None
 
     @fields.depends('account_type')
     def on_change_with_current_name(self, name=None):
         name = super().on_change_with_current_name(name)
         if self.account_type:
             name = self.account_type.name
         return name
@@ -625,25 +639,23 @@
                 '.msg_budget_line_period_budget_line_period_unique'))
         cls.__access__.add('budget_line')
         cls._order.insert(0, ('period', 'DESC'))
 
     @fields.depends('budget_line', '_parent_budget_line.company')
     def on_change_with_currency(self, name=None):
         if self.budget_line and self.budget_line.company:
-            return self.budget_line.company.currency.id
+            return self.budget_line.company.currency
 
     @fields.depends(
         'budget_line',
         '_parent_budget_line.budget',
         '_parent_budget_line._parent_budget.fiscalyear')
     def on_change_with_fiscalyear(self, name=None):
-        if (self.budget_line
-                and self.budget_line.budget
-                and self.budget_line.budget.fiscalyear):
-            return self.budget_line.budget.fiscalyear.id
+        if self.budget_line and self.budget_line.budget:
+            return self.budget_line.budget.fiscalyear
 
     @classmethod
     def get_total_amount(cls, periods, name):
         amounts = {}
         with Transaction().set_context(periods=None):
             periods = cls.browse(periods)
         for period in periods:
```

### Comparing `trytond_account_budget-6.6.1/account.xml` & `trytond_account_budget-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/doc/conf.py` & `trytond_account_budget-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_budget-6.6.1/doc/design.rst` & `trytond_account_budget-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/doc/reference.rst` & `trytond_account_budget-6.8.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/doc/usage.rst` & `trytond_account_budget-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/bg.po` & `trytond_account_budget-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/ca.po` & `trytond_account_budget-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/cs.po` & `trytond_account_budget-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/de.po` & `trytond_account_budget-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/es.po` & `trytond_account_budget-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/es_419.po` & `trytond_account_budget-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/et.po` & `trytond_account_budget-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/fa.po` & `trytond_account_budget-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/fi.po` & `trytond_account_budget-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/fr.po` & `trytond_account_budget-6.8.0/locale/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:account.budget.context,periods:"
 msgid "Periods"
 msgstr "Périodes"
 
 msgctxt "field:account.budget.context,posted:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisés"
 
 msgctxt "field:account.budget.copy.start,company:"
 msgid "Company"
 msgstr "Société"
 
 msgctxt "field:account.budget.copy.start,factor:"
 msgid "Factor"
@@ -164,15 +164,15 @@
 
 msgctxt "help:account.budget,fiscalyear:"
 msgid "The fiscal year the budget applies to."
 msgstr "L'année fiscale auquel le budget s'applique."
 
 msgctxt "help:account.budget.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.budget.copy.start,factor:"
 msgid "The percentage to apply to the budget line amounts."
 msgstr "Le pourcentage à appliquer aux montants des lignes budgétaires."
 
 msgctxt "help:account.budget.copy.start,fiscalyear:"
 msgid "The fiscal year during which the new budget will apply."
```

### Comparing `trytond_account_budget-6.6.1/locale/hu.po` & `trytond_account_budget-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/id.po` & `trytond_account_budget-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/it.po` & `trytond_account_budget-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/lo.po` & `trytond_account_budget-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/lt.po` & `trytond_account_budget-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/nl.po` & `trytond_account_budget-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/pl.po` & `trytond_account_budget-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/pt.po` & `trytond_account_budget-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/ro.po` & `trytond_account_budget-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/ru.po` & `trytond_account_budget-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/sl.po` & `trytond_account_budget-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/tr.po` & `trytond_account_budget-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/uk.po` & `trytond_account_budget-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/locale/zh_CN.po` & `trytond_account_budget-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/message.xml` & `trytond_account_budget-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/setup.py` & `trytond_account_budget-6.8.0/setup.py`

 * *Files 4% similar despite different names*

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
@@ -37,39 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_budget'
 
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
     description='Tryton module that allows budgets to be setup for accounts',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
         'https://docs.tryton.org/projects/modules-account-budget',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_budget',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account budget',
     package_dir={'trytond.modules.account_budget': '.'},
     packages=(
         ['trytond.modules.account_budget']
         + ['trytond.modules.account_budget.%s' % p
             for p in find_packages()]
@@ -107,24 +107,24 @@
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

### Comparing `trytond_account_budget-6.6.1/tests/scenario_account_budget.rst` & `trytond_account_budget-6.8.0/tests/scenario_account_budget.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,18 @@
     >>> company = get_company()
 
 Create a fiscal year::
 
     >>> fiscalyear = create_fiscalyear(company)
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
-    >>> next_fiscalyear = create_fiscalyear(
-    ...     company, fiscalyear.end_date + dt.timedelta(days=1))
-    >>> next_fiscalyear.click('create_period')
+
+    >>> renew_fiscalyear = Wizard('account.fiscalyear.renew')
+    >>> renew_fiscalyear.execute('create_')
+    >>> next_fiscalyear, = renew_fiscalyear.actions[0]
 
 Create a chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
 Create the parties::
@@ -126,16 +127,15 @@
     >>> expense_budget.actual_amount
     Decimal('60.00')
     >>> expense_budget.percentage
     Decimal('1.2000')
 
 Create periods::
 
-    >>> create_periods = Wizard(
-    ...     'account.budget.line.create_periods', [pl_budget])
+    >>> create_periods = pl_budget.click('create_periods')
     >>> create_periods.execute('create_periods')
     >>> revenue_budget, expense_budget = pl_budget.children
     >>> len(pl_budget.periods)
     12
     >>> all(p.total_amount == Decimal('-8.33') for p in pl_budget.periods)
     True
     >>> len(revenue_budget.periods)
```

### Comparing `trytond_account_budget-6.6.1/tox.ini` & `trytond_account_budget-6.8.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/account_budget/* -m unittest discover -s tests
-    coverage report --include=./**/account_budget/* --omit=*/tests/*
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

### Comparing `trytond_account_budget-6.6.1/trytond_account_budget.egg-info/PKG-INFO` & `trytond_account_budget-6.8.0/trytond_account_budget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-budget
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module that allows budgets to be setup for accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-budget
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_budget
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account budget
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
 
 #####################
 Account Budget Module
 #####################
```

### Comparing `trytond_account_budget-6.6.1/trytond_account_budget.egg-info/SOURCES.txt` & `trytond_account_budget-6.8.0/trytond_account_budget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/view/budget_form.xml` & `trytond_account_budget-6.8.0/view/budget_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/view/budget_line_form.xml` & `trytond_account_budget-6.8.0/view/budget_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/view/budget_line_form_amount.xml` & `trytond_account_budget-6.8.0/view/budget_line_form_amount.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_budget-6.6.1/view/budget_line_period_form.xml` & `trytond_account_budget-6.8.0/view/budget_line_period_form.xml`

 * *Files identical despite different names*

