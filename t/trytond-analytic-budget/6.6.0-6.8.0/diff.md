# Comparing `tmp/trytond_analytic_budget-6.6.0.tar.gz` & `tmp/trytond_analytic_budget-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_budget-6.6.0.tar", last modified: Mon Oct 31 15:55:18 2022, max compression
+gzip compressed data, was "trytond_analytic_budget-6.8.0.tar", last modified: Mon May  1 12:00:49 2023, max compression
```

## Comparing `trytond_analytic_budget-6.6.0.tar` & `trytond_analytic_budget-6.8.0.tar`

### file list

```diff
@@ -1,73 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:18.546396 trytond_analytic_budget-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_analytic_budget-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 15:55:16.000000 trytond_analytic_budget-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_analytic_budget-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-10-31 15:55:16.000000 trytond_analytic_budget-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2022-10-31 15:55:15.000000 trytond_analytic_budget-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_analytic_budget-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2659 2022-10-31 15:55:18.546396 trytond_analytic_budget-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-10-27 11:24:44.000000 trytond_analytic_budget-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2021-12-11 16:59:32.000000 trytond_analytic_budget-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7930 2022-10-11 19:49:57.000000 trytond_analytic_budget-6.6.0/analytic_account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8543 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/analytic_account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:18.543062 trytond_analytic_budget-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1336 2022-04-08 16:27:20.000000 trytond_analytic_budget-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-10-27 11:24:44.000000 trytond_analytic_budget-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_analytic_budget-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      948 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:18.539729 trytond_analytic_budget-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6005 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5934 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5869 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4988 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4916 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5876 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4910 2022-10-29 07:50:43.000000 trytond_analytic_budget-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:55:18.546396 trytond_analytic_budget-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5457 2022-10-29 07:39:10.000000 trytond_analytic_budget-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:18.539729 trytond_analytic_budget-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_analytic_budget-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4507 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/tests/scenario_analytic_budget.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2022-04-16 16:30:56.000000 trytond_analytic_budget-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_analytic_budget-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_analytic_budget-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2022-10-31 15:55:14.000000 trytond_analytic_budget-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:18.546396 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2659 2022-10-31 15:55:17.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2022-10-31 15:55:18.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:55:17.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 15:55:17.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-11-01 16:09:41.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      138 2022-10-31 15:55:17.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:55:17.000000 trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:18.543062 trytond_analytic_budget-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_copy_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      639 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_line_form_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2021-10-07 13:08:07.000000 trytond_analytic_budget-6.6.0/view/budget_line_tree_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2022-04-08 16:23:26.000000 trytond_analytic_budget-6.6.0/view/budget_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:49.213389 trytond_analytic_budget-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      497 2023-05-01 11:14:11.000000 trytond_analytic_budget-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-05-01 11:14:10.000000 trytond_analytic_budget-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2651 2023-05-01 12:00:49.213389 trytond_analytic_budget-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7903 2023-04-21 08:36:08.000000 trytond_analytic_budget-6.8.0/analytic_account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8543 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/analytic_account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:49.210055 trytond_analytic_budget-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1336 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      948 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:49.203389 trytond_analytic_budget-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5895 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6125 2023-04-30 10:46:36.000000 trytond_analytic_budget-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5934 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5869 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4988 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4916 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5876 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4910 2023-04-29 08:02:49.000000 trytond_analytic_budget-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:00:49.213389 trytond_analytic_budget-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4637 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:49.203389 trytond_analytic_budget-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4424 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/tests/scenario_analytic_budget.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2023-05-01 11:14:04.000000 trytond_analytic_budget-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:49.213389 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2651 2023-05-01 12:00:48.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2017 2023-05-01 12:00:49.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:00:48.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 12:00:48.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      138 2023-05-01 12:00:48.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:00:48.000000 trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:49.206722 trytond_analytic_budget-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_copy_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      639 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_line_form_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_line_tree_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_analytic_budget-6.8.0/view/budget_list.xml
```

### Comparing `trytond_analytic_budget-6.6.0/COPYRIGHT` & `trytond_analytic_budget-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2022 B2CK
-Copyright (C) 2021-2022 Cédric Krier
+Copyright (C) 2021-2023 B2CK
+Copyright (C) 2021-2023 Cédric Krier
 Copyright (C) 2020-2021 David Harper
 Copyright (C) 2019 Adrián Bernardi
 Copyright (C) 2016 Sergi Almacellas Abellana
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `trytond_analytic_budget-6.6.0/LICENSE` & `trytond_analytic_budget-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/PKG-INFO` & `trytond_analytic_budget-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_budget
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module that allows creating budgets for analytic accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-analytic-budget
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_budget
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account budget
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
 
 ######################
 Analytic Budget Module
 ######################
```

### Comparing `trytond_analytic_budget-6.6.0/__init__.py` & `trytond_analytic_budget-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/analytic_account.py` & `trytond_analytic_budget-6.8.0/analytic_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,15 @@
         cls._sql_constraints.append(
             ('budget_account_unique', Unique(t, t.budget, t.account),
                 'analytic_account.msg_budget_line_budget_account_unique'))
         cls.__access__.add('budget')
 
     @fields.depends('budget', '_parent_budget.root')
     def on_change_with_root(self, name=None):
-        if self.budget and self.budget.root:
-            return self.budget.root.id
+        return self.budget.root if self.budget else None
 
     @classmethod
     def _get_amount_group_key(cls, record):
         return (
             ('start_date', record.budget.start_date),
             ('end_date', record.budget.end_date),
             )
```

### Comparing `trytond_analytic_budget-6.6.0/analytic_account.xml` & `trytond_analytic_budget-6.8.0/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/doc/conf.py` & `trytond_analytic_budget-6.8.0/doc/conf.py`

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

### Comparing `trytond_analytic_budget-6.6.0/doc/design.rst` & `trytond_analytic_budget-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/doc/usage.rst` & `trytond_analytic_budget-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/bg.po` & `trytond_analytic_budget-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/ca.po` & `trytond_analytic_budget-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/cs.po` & `trytond_analytic_budget-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/de.po` & `trytond_analytic_budget-6.8.0/locale/fr.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,226 +1,223 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:analytic_account.budget,company:"
 msgid "Company"
-msgstr "Unternehmen"
+msgstr "Société"
 
 msgctxt "field:analytic_account.budget,end_date:"
 msgid "End Date"
-msgstr "Enddatum"
+msgstr "Date de fin"
 
 msgctxt "field:analytic_account.budget,lines:"
 msgid "Lines"
-msgstr "Positionen"
+msgstr "Lignes"
 
 msgctxt "field:analytic_account.budget,name:"
 msgid "Name"
-msgstr "Name"
+msgstr "Nom"
 
 msgctxt "field:analytic_account.budget,root:"
 msgid "Root"
-msgstr "Wurzel"
+msgstr "Racine"
 
 msgctxt "field:analytic_account.budget,root_lines:"
 msgid "Lines"
-msgstr "Positionen"
+msgstr "Lignes"
 
 msgctxt "field:analytic_account.budget,start_date:"
 msgid "Start Date"
-msgstr "Startdatum"
+msgstr "Date de début"
 
 msgctxt "field:analytic_account.budget.context,budget:"
 msgid "Budget"
 msgstr "Budget"
 
 msgctxt "field:analytic_account.budget.copy.start,company:"
 msgid "Company"
-msgstr "Unternehmen"
+msgstr "Société"
 
 msgctxt "field:analytic_account.budget.copy.start,end_date:"
 msgid "End Date"
-msgstr "Enddatum"
+msgstr "Date de fin"
 
 msgctxt "field:analytic_account.budget.copy.start,factor:"
 msgid "Factor"
-msgstr "Faktor"
+msgstr "Facteur"
 
 msgctxt "field:analytic_account.budget.copy.start,name:"
 msgid "Name"
-msgstr "Name"
+msgstr "Nom"
 
 msgctxt "field:analytic_account.budget.copy.start,start_date:"
 msgid "Start Date"
-msgstr "Startdatum"
+msgstr "Date de début"
 
 msgctxt "field:analytic_account.budget.line,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr "Compte"
 
 msgctxt "field:analytic_account.budget.line,actual_amount:"
 msgid "Actual Amount"
-msgstr "IST-Betrag"
+msgstr "Montant réel"
 
 msgctxt "field:analytic_account.budget.line,amount:"
 msgid "Amount"
-msgstr "Betrag"
+msgstr "Montant"
 
 msgctxt "field:analytic_account.budget.line,budget:"
 msgid "Budget"
 msgstr "Budget"
 
 msgctxt "field:analytic_account.budget.line,children:"
 msgid "Children"
-msgstr "Untergeordnet (Budgetposition)"
+msgstr "Enfants"
 
 msgctxt "field:analytic_account.budget.line,company:"
 msgid "Company"
-msgstr "Unternehmen"
+msgstr "Société"
 
 msgctxt "field:analytic_account.budget.line,currency:"
 msgid "Currency"
-msgstr "Währung"
+msgstr "Devise"
 
 msgctxt "field:analytic_account.budget.line,current_name:"
 msgid "Current Name"
-msgstr "Name"
+msgstr "Nom actuel"
 
 msgctxt "field:analytic_account.budget.line,left:"
 msgid "Left"
-msgstr "Links"
+msgstr "Gauche"
 
 msgctxt "field:analytic_account.budget.line,name:"
 msgid "Name"
-msgstr "Name"
+msgstr "Nom"
 
 msgctxt "field:analytic_account.budget.line,parent:"
 msgid "Parent"
-msgstr "Übergeordnet (Budgetposition)"
+msgstr "Parent"
 
 msgctxt "field:analytic_account.budget.line,percentage:"
 msgid "Percentage"
-msgstr "Budgetauslastung (%)"
+msgstr "Pourcentage"
 
 msgctxt "field:analytic_account.budget.line,right:"
 msgid "Right"
-msgstr "Rechts"
+msgstr "Droite"
 
 msgctxt "field:analytic_account.budget.line,root:"
 msgid "Root"
-msgstr "Wurzel"
+msgstr "Racine"
 
 msgctxt "field:analytic_account.budget.line,total_amount:"
 msgid "Total Amount"
-msgstr "SOLL-Betrag (kumuliert)"
+msgstr "Montant total"
 
 msgctxt "help:analytic_account.budget,company:"
 msgid "The company that the budget is associated with."
-msgstr "Das Unternehmen dem dieses Budget zugeordnet ist."
+msgstr "La société à laquelle le budget est associé."
 
 msgctxt "help:analytic_account.budget.copy.start,factor:"
 msgid "The percentage to apply to the budget line amounts."
-msgstr ""
-"Der Prozentsatz der auf die Beträge der Budgetpositionen angewendet wird."
+msgstr "Le pourcentage à appliquer aux montants des lignes budgétaires."
 
 msgctxt "help:analytic_account.budget.line,actual_amount:"
 msgid "The total amount booked against the budget line."
-msgstr "Der gegen diese Budgetposition gebuchte kumulierte IST-Betrag."
+msgstr "Le montant total comptabilisé sur la ligne budgétaire."
 
 msgctxt "help:analytic_account.budget.line,amount:"
 msgid "The amount allocated to the budget line."
-msgstr "Der SOLL-Betrag für diese Budgetposition."
+msgstr "Le montant alloué à la ligne budgétaire."
 
 msgctxt "help:analytic_account.budget.line,children:"
 msgid "Used to add structure below the budget."
-msgstr "Ermöglicht den Aufbau einer Struktur unterhalb dieser Budgetposition."
+msgstr "Utilisé pour ajouter une structure sous le budget."
 
 msgctxt "help:analytic_account.budget.line,parent:"
 msgid "Used to add structure above the budget."
-msgstr "Ermöglicht die Zuordnung zu einer übergeordneten Budgetposition."
+msgstr "Utilisé pour ajouter une structure au-dessus du budget."
 
 msgctxt "help:analytic_account.budget.line,percentage:"
 msgid "The percentage of booked amount of the budget line."
-msgstr "Der Prozentsatz des IST-Betrags gegenüber dem SOLL-Betrag."
+msgstr "Le pourcentage du montant comptabilisé de la ligne budgétaire."
 
 msgctxt "help:analytic_account.budget.line,total_amount:"
 msgid "The total amount allocated to the budget line and its children."
-msgstr ""
-"Der kumulierte SOLL-Betrag für diese Budgetposition und untergeordnete "
-"Positionen."
+msgstr "Le montant total alloué à la ligne budgétaire et à ses enfants."
 
 msgctxt "model:analytic_account.budget,name:"
 msgid "Analytic Budget"
-msgstr "Kostenrechnungsbudget"
+msgstr "Budget analytique"
 
 msgctxt "model:analytic_account.budget.context,name:"
 msgid "Analytic Budget Context"
-msgstr "Kostenrechnungsbudget Kontext"
+msgstr "Contexte budgétaire analytique"
 
 msgctxt "model:analytic_account.budget.copy.start,name:"
 msgid "Copy Analytic Budget"
-msgstr "Kostenrechnungsbudget kopieren"
+msgstr "Copier le budget analytique"
 
 msgctxt "model:analytic_account.budget.line,name:"
 msgid "Analytic Budget"
-msgstr "Kostenrechnungsbudget"
+msgstr "Budget analytique"
 
 msgctxt "model:ir.action,name:act_budget_form"
 msgid "Analytic Budgets"
-msgstr "Kostenrechnungsbudgets"
+msgstr "Budgets analytiques"
 
 msgctxt "model:ir.action,name:act_budget_line_form"
 msgid "Budget Lines"
-msgstr "Budgetpositionen"
+msgstr "Lignes budgétaires"
 
 msgctxt "model:ir.action,name:act_budget_report"
 msgid "Analytic Budgets"
-msgstr "Kostenrechnungsbudgets"
+msgstr "Budgets analytiques"
 
 msgctxt "model:ir.action,name:wizard_budget_copy"
 msgid "Copy Budget"
-msgstr "Budget kopieren"
+msgstr "Copier le budget"
 
 msgctxt "model:ir.model.button,string:budget_copy_button"
 msgid "Copy"
-msgstr "Kopieren"
+msgstr "Copier"
 
 msgctxt "model:ir.model.button,string:budget_update_lines_button"
 msgid "Update Lines"
-msgstr "Positionen aktualisieren"
+msgstr "Mettre à jour les lignes"
 
 msgctxt "model:ir.rule.group,name:rule_group_budget_companies"
 msgid "User in companies"
-msgstr "Benutzer im Unternehmen"
+msgstr "Utilisateur dans les sociétés"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_form"
 msgid "Analytic Budgets"
-msgstr "Kostenrechnungsbudgets"
+msgstr "Budgets analytiques"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_report"
 msgid "Analytic Budgets"
-msgstr "Kostenrechnungsbudgets"
+msgstr "Budgets analytiques"
 
 msgctxt "view:analytic_account.budget.copy.start:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.budget.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.budget.line:"
 msgid "Name"
-msgstr "Name"
+msgstr "Nom"
 
 msgctxt "view:analytic_account.budget.line:"
 msgid "Name:"
-msgstr "Name:"
+msgstr "Nom :"
 
 msgctxt "wizard_button:analytic_account.budget.copy,start,copy:"
 msgid "Copy"
-msgstr "Kopieren"
+msgstr "Copier"
 
 msgctxt "wizard_button:analytic_account.budget.copy,start,end:"
 msgid "Cancel"
-msgstr "Abbrechen"
+msgstr "Annuler"
```

### Comparing `trytond_analytic_budget-6.6.0/locale/es.po` & `trytond_analytic_budget-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/es_419.po` & `trytond_analytic_budget-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/et.po` & `trytond_analytic_budget-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/fa.po` & `trytond_analytic_budget-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/fi.po` & `trytond_analytic_budget-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/fr.po` & `trytond_analytic_budget-6.8.0/locale/de.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,223 +1,226 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:analytic_account.budget,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Unternehmen"
 
 msgctxt "field:analytic_account.budget,end_date:"
 msgid "End Date"
-msgstr "Date de fin"
+msgstr "Enddatum"
 
 msgctxt "field:analytic_account.budget,lines:"
 msgid "Lines"
-msgstr "Lignes"
+msgstr "Positionen"
 
 msgctxt "field:analytic_account.budget,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Name"
 
 msgctxt "field:analytic_account.budget,root:"
 msgid "Root"
-msgstr "Racine"
+msgstr "Wurzel"
 
 msgctxt "field:analytic_account.budget,root_lines:"
 msgid "Lines"
-msgstr "Lignes"
+msgstr "Positionen"
 
 msgctxt "field:analytic_account.budget,start_date:"
 msgid "Start Date"
-msgstr "Date de début"
+msgstr "Startdatum"
 
 msgctxt "field:analytic_account.budget.context,budget:"
 msgid "Budget"
 msgstr "Budget"
 
 msgctxt "field:analytic_account.budget.copy.start,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Unternehmen"
 
 msgctxt "field:analytic_account.budget.copy.start,end_date:"
 msgid "End Date"
-msgstr "Date de fin"
+msgstr "Enddatum"
 
 msgctxt "field:analytic_account.budget.copy.start,factor:"
 msgid "Factor"
-msgstr "Facteur"
+msgstr "Faktor"
 
 msgctxt "field:analytic_account.budget.copy.start,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Name"
 
 msgctxt "field:analytic_account.budget.copy.start,start_date:"
 msgid "Start Date"
-msgstr "Date de début"
+msgstr "Startdatum"
 
 msgctxt "field:analytic_account.budget.line,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr "Konto"
 
 msgctxt "field:analytic_account.budget.line,actual_amount:"
 msgid "Actual Amount"
-msgstr "Montant réel"
+msgstr "IST-Betrag"
 
 msgctxt "field:analytic_account.budget.line,amount:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Betrag"
 
 msgctxt "field:analytic_account.budget.line,budget:"
 msgid "Budget"
 msgstr "Budget"
 
 msgctxt "field:analytic_account.budget.line,children:"
 msgid "Children"
-msgstr "Enfants"
+msgstr "Untergeordnet (Budgetposition)"
 
 msgctxt "field:analytic_account.budget.line,company:"
 msgid "Company"
-msgstr "Société"
+msgstr "Unternehmen"
 
 msgctxt "field:analytic_account.budget.line,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Währung"
 
 msgctxt "field:analytic_account.budget.line,current_name:"
 msgid "Current Name"
-msgstr "Nom actuel"
+msgstr "Name"
 
 msgctxt "field:analytic_account.budget.line,left:"
 msgid "Left"
-msgstr "Gauche"
+msgstr "Links"
 
 msgctxt "field:analytic_account.budget.line,name:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Name"
 
 msgctxt "field:analytic_account.budget.line,parent:"
 msgid "Parent"
-msgstr "Parent"
+msgstr "Übergeordnet (Budgetposition)"
 
 msgctxt "field:analytic_account.budget.line,percentage:"
 msgid "Percentage"
-msgstr "Pourcentage"
+msgstr "Budgetauslastung (%)"
 
 msgctxt "field:analytic_account.budget.line,right:"
 msgid "Right"
-msgstr "Droite"
+msgstr "Rechts"
 
 msgctxt "field:analytic_account.budget.line,root:"
 msgid "Root"
-msgstr "Racine"
+msgstr "Wurzel"
 
 msgctxt "field:analytic_account.budget.line,total_amount:"
 msgid "Total Amount"
-msgstr "Montant total"
+msgstr "SOLL-Betrag (kumuliert)"
 
 msgctxt "help:analytic_account.budget,company:"
 msgid "The company that the budget is associated with."
-msgstr "La société à laquelle le budget est associé."
+msgstr "Das Unternehmen dem dieses Budget zugeordnet ist."
 
 msgctxt "help:analytic_account.budget.copy.start,factor:"
 msgid "The percentage to apply to the budget line amounts."
-msgstr "Le pourcentage à appliquer aux montants des lignes budgétaires."
+msgstr ""
+"Der Prozentsatz der auf die Beträge der Budgetpositionen angewendet wird."
 
 msgctxt "help:analytic_account.budget.line,actual_amount:"
 msgid "The total amount booked against the budget line."
-msgstr "Le montant total comptabilisé sur la ligne budgétaire."
+msgstr "Der gegen diese Budgetposition gebuchte kumulierte IST-Betrag."
 
 msgctxt "help:analytic_account.budget.line,amount:"
 msgid "The amount allocated to the budget line."
-msgstr "Le montant alloué à la ligne budgétaire."
+msgstr "Der SOLL-Betrag für diese Budgetposition."
 
 msgctxt "help:analytic_account.budget.line,children:"
 msgid "Used to add structure below the budget."
-msgstr "Utilisé pour ajouter une structure sous le budget."
+msgstr "Ermöglicht den Aufbau einer Struktur unterhalb dieser Budgetposition."
 
 msgctxt "help:analytic_account.budget.line,parent:"
 msgid "Used to add structure above the budget."
-msgstr "Utilisé pour ajouter une structure au-dessus du budget."
+msgstr "Ermöglicht die Zuordnung zu einer übergeordneten Budgetposition."
 
 msgctxt "help:analytic_account.budget.line,percentage:"
 msgid "The percentage of booked amount of the budget line."
-msgstr "Le pourcentage du montant comptabilisé de la ligne budgétaire."
+msgstr "Der Prozentsatz des IST-Betrags gegenüber dem SOLL-Betrag."
 
 msgctxt "help:analytic_account.budget.line,total_amount:"
 msgid "The total amount allocated to the budget line and its children."
-msgstr "Le montant total alloué à la ligne budgétaire et à ses enfants."
+msgstr ""
+"Der kumulierte SOLL-Betrag für diese Budgetposition und untergeordnete "
+"Positionen."
 
 msgctxt "model:analytic_account.budget,name:"
 msgid "Analytic Budget"
-msgstr "Budget analytique"
+msgstr "Budget Kosten- und Leistungsrechnung"
 
 msgctxt "model:analytic_account.budget.context,name:"
 msgid "Analytic Budget Context"
-msgstr "Contexte budgétaire analytique"
+msgstr "Budget Kosten- und Leistungsrechnung Kontext"
 
 msgctxt "model:analytic_account.budget.copy.start,name:"
 msgid "Copy Analytic Budget"
-msgstr "Copier le budget analytique"
+msgstr "Budget Kosten- und Leistungsrechnung kopieren"
 
 msgctxt "model:analytic_account.budget.line,name:"
 msgid "Analytic Budget"
-msgstr "Budget analytique"
+msgstr "Budget Kosten- und Leistungsrechnung"
 
 msgctxt "model:ir.action,name:act_budget_form"
 msgid "Analytic Budgets"
-msgstr "Budgets analytiques"
+msgstr "Budgets Kosten- und Leistungsrechnung"
 
 msgctxt "model:ir.action,name:act_budget_line_form"
 msgid "Budget Lines"
-msgstr "Lignes budgétaires"
+msgstr "Budgetpositionen"
 
 msgctxt "model:ir.action,name:act_budget_report"
 msgid "Analytic Budgets"
-msgstr "Budgets analytiques"
+msgstr "Budgets Kosten- und Leistungsrechnung"
 
 msgctxt "model:ir.action,name:wizard_budget_copy"
 msgid "Copy Budget"
-msgstr "Copier le budget"
+msgstr "Budget kopieren"
 
 msgctxt "model:ir.model.button,string:budget_copy_button"
 msgid "Copy"
-msgstr "Copier"
+msgstr "Kopieren"
 
 msgctxt "model:ir.model.button,string:budget_update_lines_button"
 msgid "Update Lines"
-msgstr "Mettre à jour les lignes"
+msgstr "Positionen aktualisieren"
 
 msgctxt "model:ir.rule.group,name:rule_group_budget_companies"
 msgid "User in companies"
-msgstr "Utilisateur dans les sociétés"
+msgstr "Benutzer im Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_form"
 msgid "Analytic Budgets"
-msgstr "Budgets analytiques"
+msgstr "Budgets Kosten- und Leistungsrechnung"
 
 msgctxt "model:ir.ui.menu,name:menu_budget_report"
 msgid "Analytic Budgets"
-msgstr "Budgets analytiques"
+msgstr "Budgets Kosten- und Leistungsrechnung"
 
 msgctxt "view:analytic_account.budget.copy.start:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.budget.line:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.budget.line:"
 msgid "Name"
-msgstr "Nom"
+msgstr "Name"
 
 msgctxt "view:analytic_account.budget.line:"
 msgid "Name:"
-msgstr "Nom :"
+msgstr "Name:"
 
 msgctxt "wizard_button:analytic_account.budget.copy,start,copy:"
 msgid "Copy"
-msgstr "Copier"
+msgstr "Kopieren"
 
 msgctxt "wizard_button:analytic_account.budget.copy,start,end:"
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Abbrechen"
```

### Comparing `trytond_analytic_budget-6.6.0/locale/hu.po` & `trytond_analytic_budget-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/id.po` & `trytond_analytic_budget-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/it.po` & `trytond_analytic_budget-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/lo.po` & `trytond_analytic_budget-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/lt.po` & `trytond_analytic_budget-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/nl.po` & `trytond_analytic_budget-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/pl.po` & `trytond_analytic_budget-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/pt.po` & `trytond_analytic_budget-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/ro.po` & `trytond_analytic_budget-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/ru.po` & `trytond_analytic_budget-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/sl.po` & `trytond_analytic_budget-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/tr.po` & `trytond_analytic_budget-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/uk.po` & `trytond_analytic_budget-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/locale/zh_CN.po` & `trytond_analytic_budget-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/setup.py` & `trytond_analytic_budget-6.8.0/setup.py`

 * *Files 11% similar despite different names*

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
@@ -37,63 +34,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_analytic_budget'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-
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
+
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description=(
         'Tryton module that allows creating budgets for analytic accounts'),
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
         'https://docs.tryton.org/projects/modules-analytic-budget',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/analytic_budget',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton analytic account budget',
     package_dir={'trytond.modules.analytic_budget': '.'},
     packages=(
         ['trytond.modules.analytic_budget']
         + ['trytond.modules.analytic_budget.%s' % p
             for p in find_packages()]
@@ -131,28 +108,27 @@
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
     analytic_budget = trytond.modules.analytic_budget
     """,  # noqa: E501
     )
```

### Comparing `trytond_analytic_budget-6.6.0/tests/scenario_analytic_budget.rst` & `trytond_analytic_budget-6.8.0/tests/scenario_analytic_budget.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 ========================
 Analytic Budget Scenario
 ========================
 
 Imports::
 
-    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
-    >>> today = dt.date.today()
 
 Activate the analytic_budget module::
 
     >>> config = activate_modules('analytic_budget')
 
     >>> AnalyticAccount = Model.get('analytic_account.account')
     >>> Budget = Model.get('analytic_account.budget')
@@ -121,15 +119,15 @@
     >>> other_analytic_budget.actual_amount
     Decimal('-40.00')
     >>> other_analytic_budget.percentage
     Decimal('0.8000')
 
 Copy the budget without amounts::
 
-    >>> copy_budget = Wizard('analytic_account.budget.copy', [budget])
+    >>> copy_budget = budget.click('copy_button')
     >>> copy_budget.form.start_date = next_period.start_date
     >>> copy_budget.form.end_date = next_period.end_date
     >>> copy_budget.form.factor = Decimal('1.2')
     >>> copy_budget.execute('copy')
     >>> new_budget, = copy_budget.actions[0]
     >>> new_budget.start_date == next_period.start_date
     True
```

### Comparing `trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/PKG-INFO` & `trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-analytic-budget
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module that allows creating budgets for analytic accounts
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-analytic-budget
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_budget
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account budget
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
 
 ######################
 Analytic Budget Module
 ######################
```

### Comparing `trytond_analytic_budget-6.6.0/trytond_analytic_budget.egg-info/SOURCES.txt` & `trytond_analytic_budget-6.8.0/trytond_analytic_budget.egg-info/SOURCES.txt`

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
 analytic_account.py
```

### Comparing `trytond_analytic_budget-6.6.0/view/budget_copy_start_form.xml` & `trytond_analytic_budget-6.8.0/view/budget_copy_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/view/budget_form.xml` & `trytond_analytic_budget-6.8.0/view/budget_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/view/budget_line_form.xml` & `trytond_analytic_budget-6.8.0/view/budget_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_budget-6.6.0/view/budget_line_form_amount.xml` & `trytond_analytic_budget-6.8.0/view/budget_line_form_amount.xml`

 * *Files identical despite different names*

