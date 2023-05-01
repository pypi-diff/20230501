# Comparing `tmp/trytond_account_consolidation-6.6.0.tar.gz` & `tmp/trytond_account_consolidation-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_consolidation-6.6.0.tar", last modified: Mon Oct 31 16:00:16 2022, max compression
+gzip compressed data, was "trytond_account_consolidation-6.8.0.tar", last modified: Mon May  1 11:35:07 2023, max compression
```

## Comparing `trytond_account_consolidation-6.6.0.tar` & `trytond_account_consolidation-6.8.0.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:16.570729 trytond_account_consolidation-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)       47 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 16:00:14.000000 trytond_account_consolidation-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2022-10-31 16:00:13.000000 trytond_account_consolidation-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_consolidation-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2377 2022-10-31 16:00:16.567396 trytond_account_consolidation-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      745 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15623 2022-10-11 19:49:57.000000 trytond_account_consolidation-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10785 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    54958 2022-10-19 08:13:48.000000 trytond_account_consolidation-6.6.0/consolidation_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:16.564062 trytond_account_consolidation-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1272 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2022-10-27 11:24:44.000000 trytond_account_consolidation-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_account_consolidation-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1053 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:16.557395 trytond_account_consolidation-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5984 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6123 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6010 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5995 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5983 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:50:31.000000 trytond_account_consolidation-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:00:16.570729 trytond_account_consolidation-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5558 2022-10-29 07:39:09.000000 trytond_account_consolidation-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:16.560729 trytond_account_consolidation-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6715 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/tests/scenario_consolidation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1872 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 15:10:09.000000 trytond_account_consolidation-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2022-10-31 16:00:12.000000 trytond_account_consolidation-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:16.567396 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2377 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2591 2022-10-31 16:00:16.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:00:15.000000 trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:16.564062 trytond_account_consolidation-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      810 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/consolidation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2022-09-12 22:47:25.000000 trytond_account_consolidation-6.6.0/view/move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:07.620925 trytond_account_consolidation-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-05-01 10:56:53.000000 trytond_account_consolidation-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-05-01 10:56:52.000000 trytond_account_consolidation-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2363 2023-05-01 11:35:07.620925 trytond_account_consolidation-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15625 2023-04-28 07:46:16.000000 trytond_account_consolidation-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10785 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    54958 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/consolidation_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:07.617591 trytond_account_consolidation-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1272 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1053 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:07.610925 trytond_account_consolidation-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5986 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6125 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6012 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6029 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5985 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5180 2023-04-30 10:46:36.000000 trytond_account_consolidation-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:07.620925 trytond_account_consolidation-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4732 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:07.610925 trytond_account_consolidation-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6715 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/tests/scenario_consolidation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1872 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2023-05-01 10:56:47.000000 trytond_account_consolidation-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:07.620925 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2363 2023-05-01 11:35:06.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2553 2023-05-01 11:35:07.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:06.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:35:06.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-05-01 11:35:06.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:06.000000 trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:07.617591 trytond_account_consolidation-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      810 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/consolidation_balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/consolidation_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/view/consolidation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/view/consolidation_income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/consolidation_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/consolidation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/consolidation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:14.000000 trytond_account_consolidation-6.8.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-04-15 07:12:15.000000 trytond_account_consolidation-6.8.0/view/move_list.xml
```

### Comparing `trytond_account_consolidation-6.6.0/COPYRIGHT` & `trytond_account_consolidation-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2021 NaN-tic
-Copyright (C) 2022 B2CK
-Copyright (C) 2022 Cédric Krier
+Copyright (C) 2022-2023 B2CK
+Copyright (C) 2022-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_consolidation-6.6.0/LICENSE` & `trytond_account_consolidation-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/PKG-INFO` & `trytond_account_consolidation-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_consolidation
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module consolidate accounting of many companies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-consolidation
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_consolidation
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account consolidation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,19 +38,19 @@
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
 
 doc/index.rst
```

### Comparing `trytond_account_consolidation-6.6.0/__init__.py` & `trytond_account_consolidation-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/account.py` & `trytond_account_consolidation-6.8.0/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         return super().copy(consolidations, default=default)
 
 
 class ConsolidationBalanceSheetContext(ModelView):
     "Consolidation Balance Sheet Context"
     __name__ = 'account.consolidation.balance_sheet.context'
     date = fields.Date("Date", required=True)
-    posted = fields.Boolean("Posted Move", help="Only include posted moves.")
+    posted = fields.Boolean("Posted Moves", help="Only include posted moves.")
     companies = fields.Many2Many('company.company', None, None, "Companies")
     currency = fields.Many2One('currency.currency', "Currency", required=True)
 
     comparison = fields.Boolean("Comparison")
     date_cmp = fields.Date(
         "Date",
         states={
@@ -369,15 +369,15 @@
         domain=[
             If(Eval('from_date') & Eval('to_date'),
                 ('to_date', '>=', Eval('from_date')),
                 ()),
             ])
     companies = fields.Many2Many('company.company', None, None, "Companies")
     currency = fields.Many2One('currency.currency', "Currency", required=True)
-    posted = fields.Boolean('Posted Move', help="Only include posted moves.")
+    posted = fields.Boolean('Posted Moves', help="Only include posted moves.")
     comparison = fields.Boolean('Comparison')
     from_date_cmp = fields.Date(
         "From Date",
         domain=[
             If(Eval('to_date_cmp') & Eval('from_date_cmp'),
                 ('from_date_cmp', '<=', Eval('to_date_cmp')),
                 ()),
```

### Comparing `trytond_account_consolidation-6.6.0/account.xml` & `trytond_account_consolidation-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/consolidation_statement.fodt` & `trytond_account_consolidation-6.8.0/consolidation_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/doc/conf.py` & `trytond_account_consolidation-6.8.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-modules_url = 'https://docs.tryton.org/projects/modules-{module}/en/{series}/'
-trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+import os
+
+base_url = os.environ.get('DOC_BASE_URL')
+if base_url:
+    modules_url = base_url + '/modules-{module}/'
+    trytond_url = base_url + '/server/'
+else:
+    modules_url = (
+        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
+    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
 
 
 def get_info():
     import configparser
-    import os
     import subprocess
     import sys
 
     module_dir = os.path.dirname(os.path.dirname(__file__))
 
     config = configparser.ConfigParser()
     config.read_file(open(os.path.join(module_dir, 'tryton.cfg')))
@@ -22,15 +29,18 @@
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
@@ -53,9 +63,10 @@
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
+linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
-del get_info, info, modules_url, trytond_url
+del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_account_consolidation-6.6.0/doc/design.rst` & `trytond_account_consolidation-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/doc/usage.rst` & `trytond_account_consolidation-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/locale/bg.po` & `trytond_account_consolidation-6.8.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/ca.po` & `trytond_account_consolidation-6.8.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr "Data"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Assentaments comptabilitzats"
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr "Empreses"
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr "Des de la data"
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr "Des de la data"
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Assentaments comptabilitzats"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr "Fins a la data"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/cs.po` & `trytond_account_consolidation-6.8.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/de.po` & `trytond_account_consolidation-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr "Datum"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Nur festgeschriebene Buchungssätze"
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr "Unternehmen"
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr "Von Datum"
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr "Von Datum"
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Nur festgeschriebene Buchungssätze"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr "Bis Datum"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/es.po` & `trytond_account_consolidation-6.8.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr "Fecha"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr "Fecha"
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asientos contabilizados"
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr "Empresas"
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr "Desde la fecha"
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr "Desde la fecha"
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr "Asientos contabilizados"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr "Hasta la fecha"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/es_419.po` & `trytond_account_consolidation-6.8.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/et.po` & `trytond_account_consolidation-6.8.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/fa.po` & `trytond_account_consolidation-6.8.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/fi.po` & `trytond_account_consolidation-6.8.0/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/fr.po` & `trytond_account_consolidation-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 msgstr "Date"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr "Date"
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Mouvement posté"
+msgid "Posted Moves"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr "Sociétés"
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
 msgid "Comparison"
@@ -83,16 +83,16 @@
 msgstr "Date de début"
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr "Date de début"
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
-msgstr "Mouvement posté"
+msgid "Posted Moves"
+msgstr "Mouvements comptabilisés"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr "Date de fin"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
 msgid "To Date"
@@ -108,19 +108,19 @@
 
 msgctxt "field:account.move.line,consolidation_company:"
 msgid "Consolidation Company"
 msgstr "Société de consolidation"
 
 msgctxt "help:account.consolidation.balance_sheet.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "help:account.consolidation.income_statement.context,posted:"
 msgid "Only include posted moves."
-msgstr "Inclure seulement les mouvements postés."
+msgstr "Inclure seulement les mouvements comptabilisés."
 
 msgctxt "model:account.consolidation,name:"
 msgid "Account Consolidation"
 msgstr "Consolidation de compte"
 
 msgctxt "model:account.consolidation.balance_sheet.context,name:"
 msgid "Consolidation Balance Sheet Context"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/hu.po` & `trytond_account_consolidation-6.8.0/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/id.po` & `trytond_account_consolidation-6.8.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/it.po` & `trytond_account_consolidation-6.8.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/lo.po` & `trytond_account_consolidation-6.8.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/lt.po` & `trytond_account_consolidation-6.8.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/nl.po` & `trytond_account_consolidation-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 msgstr "Datum"
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
-msgstr "Bevestigde boeking"
+msgid "Posted Moves"
+msgstr "Geboekte boekingen"
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr "Bedrijven"
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
 msgid "Comparison"
@@ -83,16 +83,16 @@
 msgstr "Vanaf datum"
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr "Vanaf datum"
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
-msgstr "Bevestigde boeking"
+msgid "Posted Moves"
+msgstr "Geboekte boekingen"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr "Tot datum"
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
 msgid "To Date"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/pl.po` & `trytond_account_consolidation-6.8.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/pt.po` & `trytond_account_consolidation-6.8.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/ro.po` & `trytond_account_consolidation-6.8.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/ru.po` & `trytond_account_consolidation-6.8.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/sl.po` & `trytond_account_consolidation-6.8.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/tr.po` & `trytond_account_consolidation-6.8.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/uk.po` & `trytond_account_consolidation-6.8.0/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/locale/zh_CN.po` & `trytond_account_consolidation-6.8.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,date_cmp:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.balance_sheet.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,companies:"
 msgid "Companies"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,comparison:"
@@ -83,15 +83,15 @@
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,from_date_cmp:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,posted:"
-msgid "Posted Move"
+msgid "Posted Moves"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date:"
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:account.consolidation.income_statement.context,to_date_cmp:"
```

### Comparing `trytond_account_consolidation-6.6.0/setup.py` & `trytond_account_consolidation-6.8.0/setup.py`

 * *Files 8% similar despite different names*

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
@@ -37,65 +34,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_consolidation'
 
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
     get_require_version('trytond_account_invoice'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description="Tryton module consolidate accounting of many companies",
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-account-consolidation'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_consolidation',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account consolidation',
     package_dir={'trytond.modules.account_consolidation': '.'},
     packages=(
         ['trytond.modules.account_consolidation']
         + ['trytond.modules.account_consolidation.%s' % p
             for p in find_packages()]
@@ -133,28 +110,27 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     account_consolidation = trytond.modules.account_consolidation
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_consolidation-6.6.0/tests/scenario_consolidation.rst` & `trytond_account_consolidation-6.8.0/tests/scenario_consolidation.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/tests/scenario_invoice.rst` & `trytond_account_consolidation-6.8.0/tests/scenario_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/PKG-INFO` & `trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-consolidation
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module consolidate accounting of many companies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-consolidation
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_consolidation
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account consolidation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,19 +38,19 @@
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
 
 doc/index.rst
```

### Comparing `trytond_account_consolidation-6.6.0/trytond_account_consolidation.egg-info/SOURCES.txt` & `trytond_account_consolidation-6.8.0/trytond_account_consolidation.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
```

### Comparing `trytond_account_consolidation-6.6.0/view/consolidation_balance_sheet_context_form.xml` & `trytond_account_consolidation-6.8.0/view/consolidation_balance_sheet_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/view/consolidation_form.xml` & `trytond_account_consolidation-6.8.0/view/consolidation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_consolidation-6.6.0/view/consolidation_income_statement_context_form.xml` & `trytond_account_consolidation-6.8.0/view/consolidation_income_statement_context_form.xml`

 * *Files identical despite different names*

