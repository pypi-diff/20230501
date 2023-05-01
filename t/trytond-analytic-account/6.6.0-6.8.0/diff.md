# Comparing `tmp/trytond_analytic_account-6.6.0.tar.gz` & `tmp/trytond_analytic_account-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_account-6.6.0.tar", last modified: Mon Oct 31 15:51:52 2022, max compression
+gzip compressed data, was "trytond_analytic_account-6.8.0.tar", last modified: Mon May  1 12:01:49 2023, max compression
```

## Comparing `trytond_analytic_account-6.6.0.tar` & `trytond_analytic_account-6.8.0.tar`

### file list

```diff
@@ -1,82 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:52.753404 trytond_analytic_account-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_analytic_account-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_analytic_account-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 15:51:51.000000 trytond_analytic_account-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_analytic_account-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2022-10-31 15:51:50.000000 trytond_analytic_account-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2022-10-31 15:51:50.000000 trytond_analytic_account-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:24.000000 trytond_analytic_account-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_analytic_account-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3553 2022-10-31 15:51:52.753404 trytond_analytic_account-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2019-10-11 23:09:47.000000 trytond_analytic_account-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2022-07-17 22:04:14.000000 trytond_analytic_account-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18532 2022-10-11 19:49:57.000000 trytond_analytic_account-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9177 2022-07-17 22:04:14.000000 trytond_analytic_account-6.6.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      581 2019-06-04 16:49:44.000000 trytond_analytic_account-6.6.0/analytic_account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:52.750070 trytond_analytic_account-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2019-10-11 23:09:47.000000 trytond_analytic_account-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2019-06-04 16:49:44.000000 trytond_analytic_account-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11373 2022-10-23 08:02:56.000000 trytond_analytic_account-6.6.0/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5544 2021-04-27 07:34:40.000000 trytond_analytic_account-6.6.0/line.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:52.746737 trytond_analytic_account-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8430 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8047 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7461 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8161 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8068 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7193 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7851 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8650 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7448 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8143 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7841 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7487 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8139 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8722 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7639 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8191 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7666 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8029 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7256 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8397 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7985 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7439 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7103 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7679 2022-10-29 07:50:44.000000 trytond_analytic_account-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2019-10-11 23:09:47.000000 trytond_analytic_account-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2022-04-10 15:40:35.000000 trytond_analytic_account-6.6.0/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2021-04-27 07:34:40.000000 trytond_analytic_account-6.6.0/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:51:52.753404 trytond_analytic_account-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5203 2022-10-29 07:39:10.000000 trytond_analytic_account-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:52.746737 trytond_analytic_account-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_analytic_account-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5994 2021-07-02 14:50:26.000000 trytond_analytic_account-6.6.0/tests/scenario_analytic_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11115 2022-04-16 16:30:56.000000 trytond_analytic_account-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_analytic_account-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2022-10-31 15:10:09.000000 trytond_analytic_account-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2022-10-31 15:51:49.000000 trytond_analytic_account-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:52.750070 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3553 2022-10-31 15:51:52.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2484 2022-10-31 15:51:52.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:51:52.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 15:51:52.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:12.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-31 15:51:52.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:51:52.000000 trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:52.750070 trytond_analytic_account-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-07-17 22:04:14.000000 trytond_analytic_account-6.6.0/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      499 2018-08-18 09:54:24.000000 trytond_analytic_account-6.6.0/view/account_distribution_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2019-12-28 17:16:43.000000 trytond_analytic_account-6.6.0/view/account_distribution_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2019-10-11 23:09:47.000000 trytond_analytic_account-6.6.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2022-04-08 16:23:26.000000 trytond_analytic_account-6.6.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2022-04-08 16:23:26.000000 trytond_analytic_account-6.6.0/view/account_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2022-04-08 16:23:26.000000 trytond_analytic_account-6.6.0/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2022-07-17 22:04:14.000000 trytond_analytic_account-6.6.0/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2018-08-18 09:54:24.000000 trytond_analytic_account-6.6.0/view/analytic_account_entry_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2019-12-28 17:16:43.000000 trytond_analytic_account-6.6.0/view/analytic_account_entry_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2018-08-18 09:54:24.000000 trytond_analytic_account-6.6.0/view/line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2019-12-28 17:16:43.000000 trytond_analytic_account-6.6.0/view/line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2018-08-18 09:54:24.000000 trytond_analytic_account-6.6.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      743 2022-04-08 16:23:26.000000 trytond_analytic_account-6.6.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2018-08-18 09:54:24.000000 trytond_analytic_account-6.6.0/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2022-04-08 16:23:26.000000 trytond_analytic_account-6.6.0/view/rule_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:49.354135 trytond_analytic_account-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3365 2023-05-01 11:14:55.000000 trytond_analytic_account-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:14:55.000000 trytond_analytic_account-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_account-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3544 2023-05-01 12:01:49.350802 trytond_analytic_account-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19410 2023-04-21 08:36:08.000000 trytond_analytic_account-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9177 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/analytic_account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:49.350802 trytond_analytic_account-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11351 2023-04-21 08:36:08.000000 trytond_analytic_account-6.8.0/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5544 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/line.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:49.344135 trytond_analytic_account-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8636 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8368 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7667 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8495 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8393 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7399 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8057 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8856 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7654 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8488 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8047 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7693 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8345 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8928 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7845 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8530 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7872 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8235 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7463 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8603 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8191 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7645 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7309 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7885 2023-04-30 10:46:36.000000 trytond_analytic_account-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1748 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2958 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:01:49.354135 trytond_analytic_account-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4391 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:49.344135 trytond_analytic_account-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7232 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/tests/scenario_analytic_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11115 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-05-01 11:14:49.000000 trytond_analytic_account-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:49.350802 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3544 2023-05-01 12:01:48.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2458 2023-05-01 12:01:49.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:48.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 12:01:48.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-05-01 12:01:48.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:01:48.000000 trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:49.347468 trytond_analytic_account-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      499 2023-01-16 14:00:20.000000 trytond_analytic_account-6.8.0/view/account_distribution_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_distribution_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-01-16 14:00:20.000000 trytond_analytic_account-6.8.0/view/analytic_account_entry_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/analytic_account_entry_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-01-16 14:00:20.000000 trytond_analytic_account-6.8.0/view/line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_analytic_account-6.8.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      743 2023-04-28 07:46:16.000000 trytond_analytic_account-6.8.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-01-16 14:00:20.000000 trytond_analytic_account-6.8.0/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_analytic_account-6.8.0/view/rule_list.xml
```

### Comparing `trytond_analytic_account-6.6.0/CHANGELOG` & `trytond_analytic_account-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

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
 * Use context model for chart of analytic accounts
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_analytic_account-6.6.0/COPYRIGHT` & `trytond_analytic_account-6.8.0/COPYRIGHT`

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

### Comparing `trytond_analytic_account-6.6.0/LICENSE` & `trytond_analytic_account-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/PKG-INFO` & `trytond_analytic_account-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_account
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for analytic accounting
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
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_account
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account
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
 
 Analytic Account Module
 #######################
 
 The analytic account module adds the fundamentals required to analyse
```

### Comparing `trytond_analytic_account-6.6.0/README.rst` & `trytond_analytic_account-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/__init__.py` & `trytond_analytic_account-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/account.py` & `trytond_analytic_account-6.8.0/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from sql.aggregate import Sum
 from sql.conditionals import Coalesce
 
 from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, Unique, fields, tree)
+from trytond.model.exceptions import AccessError
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Eval, If, PYSONDecoder, PYSONEncoder
-from trytond.tools import is_full_text, lstrip_wildcard
+from trytond.tools import grouped_slice, is_full_text, lstrip_wildcard
 from trytond.transaction import Transaction
 
 from .exceptions import AccountValidationError
 
 
 class Account(
         DeactivableMixin, tree('distribution_parents'), tree(),
@@ -139,16 +140,15 @@
             if sum((d.ratio for d in account.distributions)) != 1:
                 raise AccountValidationError(
                     gettext('analytic_account.msg_invalid_distribution',
                         account=account.rec_name))
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @fields.depends('parent', 'type',
         '_parent_parent.id', '_parent_parent.root', '_parent_parent.type')
     def on_change_parent(self):
         if (self.parent and self.parent.id is not None and self.parent.id > 0
                 and self.type != 'root'):
             if self.parent.type == 'root':
@@ -298,14 +298,34 @@
                     rounding = self.currency.rounding.copy_sign(remainder)
                     result[i] = (account, current_amount + rounding)
                     remainder -= rounding
                     i = (i + 1) % len(result)
             assert sum(a for _, a in result) == amount
             return result
 
+    @classmethod
+    def write(cls, *args):
+        pool = Pool()
+        Entry = pool.get('analytic.account.entry')
+        actions = iter(args)
+        for records, values in zip(actions, actions):
+            if 'root' in values:
+                for sub_records in grouped_slice(records):
+                    entries = Entry.search([
+                            ('account', 'in', list(map(int, sub_records))),
+                            ],
+                        limit=1, order=[])
+                    if entries:
+                        entry, = entries
+                        raise AccessError(gettext(
+                                'analytic_account'
+                                '.msg_analytic_account_root_change',
+                                account=entry.account.rec_name))
+        super().write(*args)
+
 
 class AccountContext(ModelView):
     'Open Chart of Accounts'
     __name__ = 'analytic_account.account.context'
     start_date = fields.Date('Start Date')
     end_date = fields.Date('End Date')
 
@@ -332,16 +352,15 @@
     @classmethod
     def __setup__(cls):
         super(AccountDistribution, cls).__setup__()
         cls._order.insert(0, ('ratio', 'DESC'))
 
     @fields.depends('parent', '_parent_parent.root')
     def on_change_with_root(self, name=None):
-        if self.parent:
-            return self.parent.root.id
+        return self.parent.root if self.parent else None
 
 
 class AnalyticAccountEntry(ModelView, ModelSQL):
     'Analytic Account Entry'
     __name__ = 'analytic.account.entry'
     origin = fields.Reference('Origin', selection='get_origin')
     root = fields.Many2One(
```

### Comparing `trytond_analytic_account-6.6.0/account.xml` & `trytond_analytic_account-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/analytic_account.xml` & `trytond_analytic_account-6.8.0/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/doc/index.rst` & `trytond_analytic_account-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/line.py` & `trytond_analytic_account-6.8.0/line.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,20 +78,20 @@
     @staticmethod
     def default_credit():
         return Decimal(0)
 
     @fields.depends('move_line', '_parent_move_line.account')
     def on_change_with_currency(self, name=None):
         if self.move_line and self.move_line.account:
-            return self.move_line.account.company.currency.id
+            return self.move_line.account.company.currency
 
     @fields.depends('move_line', '_parent_move_line.account')
     def on_change_with_company(self, name=None):
         if self.move_line and self.move_line.account:
-            return self.move_line.account.company.id
+            return self.move_line.account.company
 
     @classmethod
     def search_company(cls, name, clause):
         return [('move_line.account.' + clause[0],) + tuple(clause[1:])]
 
     @fields.depends('move_line', '_parent_move_line.date',
         '_parent_move_line.debit', '_parent_move_line.credit')
@@ -154,27 +154,27 @@
         MoveLine = pool.get('account.move.line')
         super(Move, cls).post(moves)
         lines = [l for m in moves for l in m.lines]
         MoveLine.apply_rule(lines)
         MoveLine.set_analytic_state(lines)
         MoveLine.save(lines)
 
-    def cancel(self, default=None):
-        'Reverse credit/debit of analytic lines'
-        pool = Pool()
-        AnalyticLine = pool.get('analytic_account.line')
-        cancel_move = super(Move, self).cancel(default)
-        analytic_lines = []
-        for line in cancel_move.lines:
-            for analytic_line in line.analytic_lines:
-                analytic_line.debit, analytic_line.credit = (
-                    analytic_line.credit, analytic_line.debit)
-                analytic_lines.append(analytic_line)
-        AnalyticLine.save(analytic_lines)
-        return cancel_move
+    def _cancel_default(self, reversal=False):
+        default = super()._cancel_default(reversal=reversal)
+        if reversal:
+            default['lines.analytic_lines.debit'] = (
+                lambda data: data['credit'])
+            default['lines.analytic_lines.credit'] = (
+                lambda data: data['debit'])
+        else:
+            default['lines.analytic_lines.debit'] = (
+                lambda data: data['debit'] * -1)
+            default['lines.analytic_lines.credit'] = (
+                lambda data: data['credit'] * -1)
+        return default
 
 
 class MoveLine(metaclass=PoolMeta):
     __name__ = 'account.move.line'
     analytic_lines = fields.One2Many('analytic_account.line', 'move_line',
             'Analytic Lines')
     analytic_state = fields.Selection([
```

### Comparing `trytond_analytic_account-6.6.0/line.xml` & `trytond_analytic_account-6.8.0/line.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/locale/bg.po` & `trytond_analytic_account-6.8.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/ca.po` & `trytond_analytic_account-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,22 @@
 msgid "Open Account"
 msgstr "Obre compte"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr "Regles"
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+"No es pot canviar l'arrel del compte analític \"%(account)s\" perquè està "
+"associat amb un apunt analític."
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 "La suma de la distribució del compte \"%(account)s\" ha de ser 100%% per "
 "poder-lo guardar."
```

### Comparing `trytond_analytic_account-6.6.0/locale/cs.po` & `trytond_analytic_account-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/de.po` & `trytond_analytic_account-6.8.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,22 @@
 msgid "Open Account"
 msgstr "Kostenstelle öffnen"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr "Regeln"
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+"Die Wurzel der Kostenstelle \"%(account)s\" kann nicht geändert werden, da "
+"bereits Kosten verbucht wurden."
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 "Um Kostenstelle \"%(account)s\" speichern zu können, muss die Summe aller "
 "Verteilungen 100%% ergeben."
@@ -261,15 +269,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
 msgstr "Kostenstellenplan"
 
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr "Kostenrechnung"
+msgstr "Kosten- und Leistungsrechnung"
 
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
 msgstr "Kostenpositionen vervollständigen"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
```

### Comparing `trytond_analytic_account-6.6.0/locale/es.po` & `trytond_analytic_account-6.8.0/locale/sl.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,340 +1,361 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.move.line,analytic_lines:"
 msgid "Analytic Lines"
-msgstr "Líneas analíticas"
+msgstr "Analitične postavke"
 
 msgctxt "field:account.move.line,analytic_state:"
 msgid "Analytic State"
-msgstr "Estado analítico"
+msgstr "Analitično stanje"
 
 msgctxt "field:analytic.account.entry,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Konto"
 
 msgctxt "field:analytic.account.entry,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Družba"
 
 msgctxt "field:analytic.account.entry,origin:"
 msgid "Origin"
-msgstr "Origen"
+msgstr "Poreklo"
 
 msgctxt "field:analytic.account.entry,root:"
 msgid "Root Analytic"
-msgstr "Cuenta raíz analítica"
+msgstr "Koren"
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
 msgstr "Saldo"
 
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr "Hijos"
+msgstr "Podkonti"
 
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Šifra"
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Družba"
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
-msgstr "Haber"
+msgstr "Kredit"
 
 msgctxt "field:analytic_account.account,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valuta"
 
 msgctxt "field:analytic_account.account,debit:"
 msgid "Debit"
-msgstr "Debe"
+msgstr "Debet"
 
 msgctxt "field:analytic_account.account,distribution_parents:"
 msgid "Distribution Parents"
-msgstr "Padres de la distribución"
+msgstr "Matične porazdelitve"
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
-msgstr "Distribuciones"
+msgstr "Porazdelitve"
 
 msgctxt "field:analytic_account.account,name:"
 msgid "Name"
-msgstr "Nombre"
+msgstr "Naziv"
 
 msgctxt "field:analytic_account.account,note:"
 msgid "Note"
-msgstr "Nota"
+msgstr "Opomba"
 
 msgctxt "field:analytic_account.account,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr "Matični konto"
 
 msgctxt "field:analytic_account.account,root:"
 msgid "Root"
-msgstr "Raíz"
+msgstr "Koren"
 
 msgctxt "field:analytic_account.account,state:"
 msgid "State"
-msgstr "Estado"
+msgstr "Stanje"
 
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr "Tip"
 
+#, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr "Fecha final"
+msgstr "Končni datum"
 
+#, fuzzy
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
-msgstr "Fecha inicial"
+msgstr "Začetni datum"
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Konto"
 
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr "Matična porazdelitev"
 
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
-msgstr "Porcentaje"
+msgstr "Delež"
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
-msgstr "Raíz"
+msgstr "Koren"
 
 msgctxt "field:analytic_account.line,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Konto"
 
 msgctxt "field:analytic_account.line,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Družba"
 
 msgctxt "field:analytic_account.line,credit:"
 msgid "Credit"
-msgstr "Haber"
+msgstr "Kredit"
 
+#, fuzzy
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valuta"
 
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr "Fecha"
+msgstr "Datum"
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
-msgstr "Debe"
+msgstr "Debet"
 
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
-msgstr "Apunte contable"
+msgstr "Postavka knjižbe"
 
 msgctxt "field:analytic_account.rule,account:"
 msgid "Account"
-msgstr "Cuenta"
+msgstr "Konto"
 
 msgctxt "field:analytic_account.rule,analytic_accounts:"
 msgid "Analytic Accounts"
-msgstr "Cuentas analíticas"
+msgstr "Analitični konti"
 
 msgctxt "field:analytic_account.rule,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr "Cuentas analíticas"
+msgstr "Število analitičnih kontov"
 
 msgctxt "field:analytic_account.rule,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Družba"
 
 msgctxt "field:analytic_account.rule,journal:"
 msgid "Journal"
-msgstr "Diario"
+msgstr "Dnevnik"
 
 msgctxt "field:analytic_account.rule,party:"
 msgid "Party"
-msgstr "Tercero"
+msgstr "Partner"
 
 msgctxt "field:analytic_account.rule,party_visible:"
 msgid "Party Visible"
-msgstr "Tercero visible"
+msgstr "Partner viden"
 
 msgctxt "model:analytic.account.entry,name:"
 msgid "Analytic Account Entry"
-msgstr "Asiento cuenta analítica"
+msgstr "Vnos analitičnega konta"
 
 msgctxt "model:analytic_account.account,name:"
 msgid "Analytic Account"
-msgstr "Cuenta analítica"
+msgstr "Analitični konto"
 
+#, fuzzy
 msgctxt "model:analytic_account.account.context,name:"
 msgid "Open Chart of Accounts"
-msgstr "Abrir plan contable"
+msgstr "Odpri kontni načrt"
 
 msgctxt "model:analytic_account.account.distribution,name:"
 msgid "Analytic Account Distribution"
-msgstr "Distribución de contabilidad analítica"
+msgstr "Porazdelitev analitičnih kontov"
 
 msgctxt "model:analytic_account.line,name:"
 msgid "Analytic Line"
-msgstr "Línea analítica"
+msgstr "Analitična postavka"
 
 msgctxt "model:analytic_account.rule,name:"
 msgid "Analytic Rule"
-msgstr "Regla analítica"
+msgstr "Analitično pravilo"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_account_list"
 msgid "Accounts"
-msgstr "Cuentas"
+msgstr "Konto"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
-msgstr "Cuentas"
+msgstr "Konto"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Abrir plan de cuentas analíticas"
+msgstr "Open Chart of Analytic Accounts"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Analytic Lines"
-msgstr "Líneas analíticas"
+msgstr "Analytic Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_move_line_form_completion"
 msgid "Analytic Lines to Complete"
-msgstr "Lineas analíticas a completar"
+msgstr "Analytic Lines to Complete"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Account"
-msgstr "Abrir cuenta"
+msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
-msgstr "Reglas"
+msgstr ""
+
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
-"Para grabar la cuenta \"%(account)s\" la suma de sus distribuciones debe ser"
-" 100%%."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_root_origin_unique"
 msgid "Only one account is allowed by analytic root and origin."
-msgstr ""
-"Sólo se puede seleccionar una cuenta por cada origen y raíz analítica."
+msgstr "Dovoljen je samo en konto na analitični koren in poreklo."
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
-msgstr "Aplicar reglas analíticas"
+msgstr "Analytic Rules"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_entry_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
-msgstr "Usuario en las empresas"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
-msgstr "Cuentas"
+msgstr "Konto"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
-msgstr "Cuentas"
+msgstr "Konto"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Abrir plan de cuentas analítico"
+msgstr "Open Chart of Analytic Accounts"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr "Analítica"
+msgstr "Analitično"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
-msgstr "Lineas analíticas a completar"
+msgstr "Analytic Lines to Complete"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
-msgstr "Reglas"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:res.group,name:group_analytic_admin"
 msgid "Analytic Administration"
-msgstr "Administración de analítica"
+msgstr "Analytic Administration"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "V pripravi"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Valid"
-msgstr "Válido"
+msgstr "Odobreno"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Closed"
-msgstr "Cerrada"
+msgstr "Zaprto"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Draft"
-msgstr "Borrador"
+msgstr "V pripravi"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Opened"
-msgstr "Abierta"
+msgstr "Odprto"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Distribution"
-msgstr "Distribución"
+msgstr "Porazdelitev"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Normal"
-msgstr "Normal"
+msgstr "Normalno"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Root"
-msgstr "Raíz"
+msgstr "Koren"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "View"
-msgstr "Vista"
+msgstr "Vpogled"
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
-msgstr "Analítica"
+msgstr "Analitično"
 
 msgctxt "view:account.move.line:"
 msgid "Credit"
-msgstr "Haber"
+msgstr "Kredit"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
-msgstr "Debe"
+msgstr "Debet"
 
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
-msgstr "Información general"
+msgstr "Splošno"
 
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
-msgstr "Notas"
+msgstr "Opombe"
```

### Comparing `trytond_analytic_account-6.6.0/locale/es_419.po` & `trytond_analytic_account-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,20 @@
 msgid "Open Account"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/et.po` & `trytond_analytic_account-6.8.0/locale/et.po`

 * *Files 3% similar despite different names*

```diff
@@ -221,14 +221,20 @@
 msgid "Open Account"
 msgstr "Avatud konto"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/fa.po` & `trytond_analytic_account-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,20 @@
 msgid "Open Account"
 msgstr "بازکردن حساب‌"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr "برای ذخیره حساب : \"%(account)s\" مجموع توزیع آنها باید %100 باشد."
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/fi.po` & `trytond_analytic_account-6.8.0/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/fr.po` & `trytond_analytic_account-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,22 @@
 msgid "Open Account"
 msgstr "Ouvrir le compte"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr "Règles"
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+"Vous ne pouvez pas modifier la racine du compte analytique « %(account)s » "
+"qui est associé à des entrées de compte analytique."
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 "Pour enregistrer le compte « %(account)s », la somme de ses distribution "
 "doit être de 100%%."
```

### Comparing `trytond_analytic_account-6.6.0/locale/hu.po` & `trytond_analytic_account-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/id.po` & `trytond_analytic_account-6.8.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,20 @@
 msgid "Open Account"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/it.po` & `trytond_analytic_account-6.8.0/locale/it.po`

 * *Files 5% similar despite different names*

```diff
@@ -221,14 +221,20 @@
 msgid "Open Account"
 msgstr "Account aperto"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 "Per salvare il conto \"%(account)s\" la somma delle loro distribuzioni deve "
 "essere 100%%."
```

### Comparing `trytond_analytic_account-6.6.0/locale/lo.po` & `trytond_analytic_account-6.8.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/lt.po` & `trytond_analytic_account-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/nl.po` & `trytond_analytic_account-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,22 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr "Regels"
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+"U kunt de basis van de analytische grootboekrekening \"%(account)s\" niet "
+"wijzigen omdat er een analytische regel is gekoppeld."
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 "Om de rekening \"%(account)s\" te bewaren moet de som van hun "
 "distributies(verdelingen) 100%% zijn."
```

### Comparing `trytond_analytic_account-6.6.0/locale/pl.po` & `trytond_analytic_account-6.8.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/pt.po` & `trytond_analytic_account-6.8.0/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 #, fuzzy
```

### Comparing `trytond_analytic_account-6.6.0/locale/ro.po` & `trytond_analytic_account-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "field:analytic_account.account,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:analytic_account.account,debit:"
 msgid "Debit"
 msgstr "Debit"
 
 msgctxt "field:analytic_account.account,distribution_parents:"
 msgid "Distribution Parents"
@@ -218,14 +218,20 @@
 msgid "Open Account"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/ru.po` & `trytond_analytic_account-6.8.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/sl.po` & `trytond_analytic_account-6.8.0/locale/tr.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,247 +1,252 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.move.line,analytic_lines:"
 msgid "Analytic Lines"
-msgstr "Analitične postavke"
+msgstr "Analytic Lines"
 
 msgctxt "field:account.move.line,analytic_state:"
 msgid "Analytic State"
-msgstr "Analitično stanje"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,origin:"
 msgid "Origin"
-msgstr "Poreklo"
+msgstr ""
 
 msgctxt "field:analytic.account.entry,root:"
 msgid "Root Analytic"
-msgstr "Koren"
+msgstr ""
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr "Podkonti"
+msgstr ""
 
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr "Šifra"
+msgstr ""
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
-msgstr "Kredit"
+msgstr ""
 
 msgctxt "field:analytic_account.account,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 msgctxt "field:analytic_account.account,debit:"
 msgid "Debit"
-msgstr "Debet"
+msgstr ""
 
 msgctxt "field:analytic_account.account,distribution_parents:"
 msgid "Distribution Parents"
-msgstr "Matične porazdelitve"
+msgstr ""
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
-msgstr "Porazdelitve"
+msgstr ""
 
 msgctxt "field:analytic_account.account,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr ""
 
 msgctxt "field:analytic_account.account,note:"
 msgid "Note"
-msgstr "Opomba"
+msgstr ""
 
 msgctxt "field:analytic_account.account,parent:"
 msgid "Parent"
-msgstr "Matični konto"
+msgstr ""
 
 msgctxt "field:analytic_account.account,root:"
 msgid "Root"
-msgstr "Koren"
+msgstr ""
 
 msgctxt "field:analytic_account.account,state:"
 msgid "State"
-msgstr "Stanje"
+msgstr ""
 
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
-msgstr "Tip"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr "Končni datum"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
-msgstr "Začetni datum"
+msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
-msgstr "Matična porazdelitev"
+msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
-msgstr "Delež"
+msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
-msgstr "Koren"
+msgstr ""
 
 msgctxt "field:analytic_account.line,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
 msgctxt "field:analytic_account.line,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:analytic_account.line,credit:"
 msgid "Credit"
-msgstr "Kredit"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr ""
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
-msgstr "Debet"
+msgstr ""
 
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
-msgstr "Postavka knjižbe"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts:"
 msgid "Analytic Accounts"
-msgstr "Analitični konti"
+msgstr "Analytic Accounts"
 
+#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr "Število analitičnih kontov"
+msgstr "Analytic Accounts"
 
 msgctxt "field:analytic_account.rule,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,journal:"
 msgid "Journal"
-msgstr "Dnevnik"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,party:"
 msgid "Party"
-msgstr "Partner"
+msgstr ""
 
 msgctxt "field:analytic_account.rule,party_visible:"
 msgid "Party Visible"
-msgstr "Partner viden"
+msgstr ""
 
 msgctxt "model:analytic.account.entry,name:"
 msgid "Analytic Account Entry"
-msgstr "Vnos analitičnega konta"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:analytic_account.account,name:"
 msgid "Analytic Account"
-msgstr "Analitični konto"
+msgstr "Analytic Account"
 
 #, fuzzy
 msgctxt "model:analytic_account.account.context,name:"
 msgid "Open Chart of Accounts"
-msgstr "Odpri kontni načrt"
+msgstr "Open Chart of Analytic Accounts"
 
 msgctxt "model:analytic_account.account.distribution,name:"
 msgid "Analytic Account Distribution"
-msgstr "Porazdelitev analitičnih kontov"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:analytic_account.line,name:"
 msgid "Analytic Line"
-msgstr "Analitična postavka"
+msgstr "Analytic Lines"
 
+#, fuzzy
 msgctxt "model:analytic_account.rule,name:"
 msgid "Analytic Rule"
-msgstr "Analitično pravilo"
+msgstr "Analytic Rules"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_account_list"
 msgid "Accounts"
-msgstr "Konto"
+msgstr "Open Account"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
-msgstr "Konto"
+msgstr "Open Account"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Analytic Accounts"
 msgstr "Open Chart of Analytic Accounts"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Analytic Lines"
 msgstr "Analytic Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_move_line_form_completion"
 msgid "Analytic Lines to Complete"
 msgstr "Analytic Lines to Complete"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_root_origin_unique"
 msgid "Only one account is allowed by analytic root and origin."
-msgstr "Dovoljen je samo en konto na analitični koren in poreklo."
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
 msgstr "Analytic Rules"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
@@ -259,97 +264,95 @@
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
-msgstr "Konto"
+msgstr "Open Account"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
-msgstr "Konto"
+msgstr "Open Account"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
 msgstr "Open Chart of Analytic Accounts"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr "Analitično"
+msgstr "Analytic Lines"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
 msgstr "Analytic Lines to Complete"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:res.group,name:group_analytic_admin"
 msgid "Analytic Administration"
 msgstr "Analytic Administration"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Draft"
-msgstr "V pripravi"
+msgstr ""
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Valid"
-msgstr "Odobreno"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Closed"
-msgstr "Zaprto"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Draft"
-msgstr "V pripravi"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Opened"
-msgstr "Odprto"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Distribution"
-msgstr "Porazdelitev"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Normal"
-msgstr "Normalno"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Root"
-msgstr "Koren"
+msgstr ""
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "View"
-msgstr "Vpogled"
+msgstr ""
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
-msgstr "Analitično"
+msgstr ""
 
 msgctxt "view:account.move.line:"
 msgid "Credit"
-msgstr "Kredit"
+msgstr ""
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
-msgstr "Debet"
+msgstr ""
 
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
-msgstr "Splošno"
+msgstr ""
 
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
-msgstr "Opombe"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_analytic_account-6.6.0/locale/tr.po` & `trytond_analytic_account-6.8.0/locale/zh_CN.po`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 msgid "Root Analytic"
 msgstr ""
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr ""
+msgstr "子项"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr ""
+msgstr "语言编码"
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
@@ -59,53 +61,61 @@
 msgid "Distribution Parents"
 msgstr ""
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,note:"
 msgid "Note"
-msgstr ""
+msgstr "注释"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "上级"
 
 msgctxt "field:analytic_account.account,root:"
 msgid "Root"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
+#, fuzzy
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
-msgstr ""
+msgstr "类型"
 
+#, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "写入日期"
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "上级"
 
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
 msgstr ""
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
@@ -123,17 +133,18 @@
 msgid "Credit"
 msgstr ""
 
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
 msgstr ""
 
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
@@ -224,14 +235,20 @@
 msgid "Open Account"
 msgstr "Open Account"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
@@ -319,34 +336,37 @@
 msgid "Normal"
 msgstr ""
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Root"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:analytic_account.account,type:"
 msgid "View"
-msgstr ""
+msgstr "视图"
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
 msgstr ""
 
 msgctxt "view:account.move.line:"
 msgid "Credit"
-msgstr ""
+msgstr "贷方"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
-msgstr ""
+msgstr "借方"
 
+#, fuzzy
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
-msgstr ""
+msgstr "注释"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_analytic_account-6.6.0/locale/uk.po` & `trytond_analytic_account-6.8.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,20 @@
 msgid "Open Account"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
```

### Comparing `trytond_analytic_account-6.6.0/locale/zh_CN.po` & `trytond_analytic_account-6.8.0/locale/es.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,366 +1,348 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.move.line,analytic_lines:"
 msgid "Analytic Lines"
-msgstr "Analytic Lines"
+msgstr "Líneas analíticas"
 
 msgctxt "field:account.move.line,analytic_state:"
 msgid "Analytic State"
-msgstr ""
+msgstr "Estado analítico"
 
 msgctxt "field:analytic.account.entry,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
 msgctxt "field:analytic.account.entry,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:analytic.account.entry,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origen"
 
 msgctxt "field:analytic.account.entry,root:"
 msgid "Root Analytic"
-msgstr ""
+msgstr "Cuenta raíz analítica"
 
 msgctxt "field:analytic_account.account,balance:"
 msgid "Balance"
-msgstr ""
+msgstr "Saldo"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,childs:"
 msgid "Children"
-msgstr "子项"
+msgstr "Hijos"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,code:"
 msgid "Code"
-msgstr "语言编码"
+msgstr "Código"
 
 msgctxt "field:analytic_account.account,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:analytic_account.account,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Haber"
 
 msgctxt "field:analytic_account.account,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:analytic_account.account,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Debe"
 
 msgctxt "field:analytic_account.account,distribution_parents:"
 msgid "Distribution Parents"
-msgstr ""
+msgstr "Padres de la distribución"
 
 msgctxt "field:analytic_account.account,distributions:"
 msgid "Distributions"
-msgstr ""
+msgstr "Distribuciones"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nombre"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,note:"
 msgid "Note"
-msgstr "注释"
+msgstr "Nota"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,parent:"
 msgid "Parent"
-msgstr "上级"
+msgstr "Padre"
 
 msgctxt "field:analytic_account.account,root:"
 msgid "Root"
-msgstr ""
+msgstr "Raíz"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Estado"
 
-#, fuzzy
 msgctxt "field:analytic_account.account,type:"
 msgid "Type"
-msgstr "类型"
+msgstr "Tipo"
 
-#, fuzzy
 msgctxt "field:analytic_account.account.context,end_date:"
 msgid "End Date"
-msgstr "日期格式"
+msgstr "Fecha final"
 
-#, fuzzy
 msgctxt "field:analytic_account.account.context,start_date:"
 msgid "Start Date"
-msgstr "写入日期"
+msgstr "Fecha inicial"
 
 msgctxt "field:analytic_account.account.distribution,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
-#, fuzzy
 msgctxt "field:analytic_account.account.distribution,parent:"
 msgid "Parent"
-msgstr "上级"
+msgstr "Padre"
 
 msgctxt "field:analytic_account.account.distribution,ratio:"
 msgid "Ratio"
-msgstr ""
+msgstr "Porcentaje"
 
 msgctxt "field:analytic_account.account.distribution,root:"
 msgid "Root"
-msgstr ""
+msgstr "Raíz"
 
 msgctxt "field:analytic_account.line,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
 msgctxt "field:analytic_account.line,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:analytic_account.line,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Haber"
 
 msgctxt "field:analytic_account.line,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:analytic_account.line,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Fecha"
 
 msgctxt "field:analytic_account.line,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Debe"
 
 msgctxt "field:analytic_account.line,move_line:"
 msgid "Account Move Line"
-msgstr ""
+msgstr "Apunte contable"
 
 msgctxt "field:analytic_account.rule,account:"
 msgid "Account"
-msgstr ""
+msgstr "Cuenta"
 
-#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts:"
 msgid "Analytic Accounts"
-msgstr "Analytic Accounts"
+msgstr "Cuentas analíticas"
 
-#, fuzzy
 msgctxt "field:analytic_account.rule,analytic_accounts_size:"
 msgid "Analytic Accounts Size"
-msgstr "Analytic Accounts"
+msgstr "Cuentas analíticas"
 
 msgctxt "field:analytic_account.rule,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:analytic_account.rule,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Diario"
 
 msgctxt "field:analytic_account.rule,party:"
 msgid "Party"
-msgstr ""
+msgstr "Tercero"
 
 msgctxt "field:analytic_account.rule,party_visible:"
 msgid "Party Visible"
-msgstr ""
+msgstr "Tercero visible"
 
 msgctxt "model:analytic.account.entry,name:"
 msgid "Analytic Account Entry"
-msgstr ""
+msgstr "Asiento cuenta analítica"
 
-#, fuzzy
 msgctxt "model:analytic_account.account,name:"
 msgid "Analytic Account"
-msgstr "Analytic Account"
+msgstr "Cuenta analítica"
 
-#, fuzzy
 msgctxt "model:analytic_account.account.context,name:"
 msgid "Open Chart of Accounts"
-msgstr "Open Chart of Analytic Accounts"
+msgstr "Abrir plan contable"
 
 msgctxt "model:analytic_account.account.distribution,name:"
 msgid "Analytic Account Distribution"
-msgstr ""
+msgstr "Distribución de contabilidad analítica"
 
-#, fuzzy
 msgctxt "model:analytic_account.line,name:"
 msgid "Analytic Line"
-msgstr "Analytic Lines"
+msgstr "Línea analítica"
 
-#, fuzzy
 msgctxt "model:analytic_account.rule,name:"
 msgid "Analytic Rule"
-msgstr "Analytic Rules"
+msgstr "Regla analítica"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_list"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Cuentas"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Cuentas"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Open Chart of Analytic Accounts"
+msgstr "Abrir plan de cuentas analíticas"
 
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Analytic Lines"
-msgstr "Analytic Lines"
+msgstr "Líneas analíticas"
 
 msgctxt "model:ir.action,name:act_move_line_form_completion"
 msgid "Analytic Lines to Complete"
-msgstr "Analytic Lines to Complete"
+msgstr "Lineas analíticas a completar"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Account"
-msgstr "Open Account"
+msgstr "Abrir cuenta"
 
 msgctxt "model:ir.action,name:act_rule_form"
 msgid "Rules"
+msgstr "Reglas"
+
+msgctxt "model:ir.message,text:msg_analytic_account_root_change"
+msgid ""
+"You cannot change the root of the analytic account \"%(account)s\" which is "
+"associated with analytic account entry."
 msgstr ""
+"No puede cambiar la raíz de la cuenta analítica \"%(account)s\" porque está "
+"asociada con un apunte analítico."
 
 msgctxt "model:ir.message,text:msg_invalid_distribution"
 msgid ""
 "To save account \"%(account)s\" the sum of their distributions must be "
 "100%%."
 msgstr ""
+"Para grabar la cuenta \"%(account)s\" la suma de sus distribuciones debe ser"
+" 100%%."
 
 msgctxt "model:ir.message,text:msg_root_origin_unique"
 msgid "Only one account is allowed by analytic root and origin."
 msgstr ""
+"Sólo se puede seleccionar una cuenta por cada origen y raíz analítica."
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:line_apply_analytic_rules_button"
 msgid "Apply Analytic Rules"
-msgstr "Analytic Rules"
+msgstr "Aplicar reglas analíticas"
 
 msgctxt "model:ir.rule.group,name:rule_group_account_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_entry_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuario en las empresas"
 
 msgctxt "model:ir.rule.group,name:rule_group_rule_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Usuario en las empresas"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_list"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Cuentas"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree"
 msgid "Accounts"
-msgstr "Open Account"
+msgstr "Cuentas"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_account_tree_chart"
 msgid "Chart of Analytic Accounts"
-msgstr "Open Chart of Analytic Accounts"
+msgstr "Abrir plan de cuentas analítico"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_analytic_account_configuration"
 msgid "Analytic"
-msgstr "Analytic Lines"
+msgstr "Analítica"
 
 msgctxt "model:ir.ui.menu,name:menu_completion"
 msgid "Analytic Lines to Complete"
-msgstr "Analytic Lines to Complete"
+msgstr "Lineas analíticas a completar"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_form"
 msgid "Rules"
-msgstr ""
+msgstr "Reglas"
 
 msgctxt "model:res.group,name:group_analytic_admin"
 msgid "Analytic Administration"
-msgstr "Analytic Administration"
+msgstr "Administración de analítica"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Draft"
-msgstr ""
+msgstr "Borrador"
 
 msgctxt "selection:account.move.line,analytic_state:"
 msgid "Valid"
-msgstr ""
+msgstr "Válido"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Closed"
-msgstr ""
+msgstr "Cerrada"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Borrador"
 
 msgctxt "selection:analytic_account.account,state:"
 msgid "Opened"
-msgstr ""
+msgstr "Abierta"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Distribution"
-msgstr ""
+msgstr "Distribución"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Normal"
-msgstr ""
+msgstr "Normal"
 
 msgctxt "selection:analytic_account.account,type:"
 msgid "Root"
-msgstr ""
+msgstr "Raíz"
 
-#, fuzzy
 msgctxt "selection:analytic_account.account,type:"
 msgid "View"
-msgstr "视图"
+msgstr "Vista"
 
 msgctxt "view:account.move.line:"
 msgid "Analytic"
-msgstr ""
+msgstr "Analítica"
 
 msgctxt "view:account.move.line:"
 msgid "Credit"
-msgstr "贷方"
+msgstr "Haber"
 
 msgctxt "view:account.move.line:"
 msgid "Debit"
-msgstr "借方"
+msgstr "Debe"
 
-#, fuzzy
 msgctxt "view:analytic_account.account.distribution:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:analytic_account.account:"
 msgid "General Information"
-msgstr ""
+msgstr "Información general"
 
-#, fuzzy
 msgctxt "view:analytic_account.account:"
 msgid "Notes"
-msgstr "注释"
+msgstr "Notas"
```

### Comparing `trytond_analytic_account-6.6.0/message.xml` & `trytond_analytic_account-6.8.0/message.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_analytic_account-6.6.0/message.xml` & `trytond_analytic_account-6.8.0/message.xml`

```diff
@@ -5,9 +5,12 @@
   <data grouped="1">
     <record model="ir.message" id="msg_invalid_distribution">
       <field name="text">To save account &quot;%(account)s&quot; the sum of their distributions must be 100%%.</field>
     </record>
     <record model="ir.message" id="msg_root_origin_unique">
       <field name="text">Only one account is allowed by analytic root and origin.</field>
     </record>
+    <record model="ir.message" id="msg_analytic_account_root_change">
+      <field name="text">You cannot change the root of the analytic account &quot;%(account)s&quot; which is associated with analytic account entry.</field>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_analytic_account-6.6.0/rule.py` & `trytond_analytic_account-6.8.0/rule.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/rule.xml` & `trytond_analytic_account-6.8.0/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/setup.py` & `trytond_analytic_account-6.8.0/setup.py`

 * *Files 21% similar despite different names*

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_analytic_account'
 
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
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for analytic accounting',
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
-        "Source Code": 'https://hg.tryton.org/modules/analytic_account',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton analytic account',
     package_dir={'trytond.modules.analytic_account': '.'},
     packages=(
         ['trytond.modules.analytic_account']
         + ['trytond.modules.analytic_account.%s' % p for p in find_packages()]
         ),
@@ -123,28 +101,27 @@
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
     analytic_account = trytond.modules.analytic_account
     """,
     )
```

### Comparing `trytond_analytic_account-6.6.0/tests/scenario_analytic_account.rst` & `trytond_analytic_account-6.8.0/tests/scenario_analytic_account.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 =========================
 Analytic Account Scenario
 =========================
 
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
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('analytic_account')
 
+    >>> Reconciliation = Model.get('account.move.reconciliation')
+
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
@@ -92,15 +91,15 @@
     >>> move.click('post')
     >>> analytic_account.reload()
     >>> analytic_account.credit
     Decimal('42.00')
     >>> analytic_account.debit
     Decimal('0.00')
 
-Cancel Move::
+Cancel reversal move::
 
     >>> cancel_move = Wizard('account.move.cancel', [move])
     >>> cancel_move.form.description = 'Cancel'
     >>> cancel_move.execute('cancel')
     >>> move.reload()
     >>> line, = [l for l in move.lines if l.account == receivable]
     >>> bool(line.reconciliation)
@@ -111,14 +110,40 @@
     True
     >>> analytic_account.reload()
     >>> analytic_account.credit
     Decimal('42.00')
     >>> analytic_account.debit
     Decimal('42.00')
 
+    >>> reconciliations = {
+    ...     l.reconciliation for l in cancel_move.lines if l.reconciliation}
+    >>> Reconciliation.delete(list(reconciliations))
+    >>> cancel_move.reload()
+    >>> cancel_move.delete()
+
+Cancel move::
+
+    >>> cancel_move = Wizard('account.move.cancel', [move])
+    >>> cancel_move.form.description = 'Cancel'
+    >>> cancel_move.form.reversal = False
+    >>> cancel_move.execute('cancel')
+    >>> move.reload()
+    >>> line, = [l for l in move.lines if l.account == receivable]
+    >>> bool(line.reconciliation)
+    True
+    >>> cancel_move, = [l.move for l in line.reconciliation.lines
+    ...     if l.move != move]
+    >>> cancel_move.origin == move
+    True
+    >>> analytic_account.reload()
+    >>> analytic_account.credit
+    Decimal('0.00')
+    >>> analytic_account.debit
+    Decimal('0.00')
+
 Create Move without analytic accounts::
 
     >>> move = Move()
     >>> move.period = period
     >>> move.journal = journal_revenue
     >>> move.date = period.start_date
     >>> line = move.lines.new()
@@ -179,7 +204,23 @@
     >>> balance_non_deferral.form.credit_account = account_pl
     >>> balance_non_deferral.form.debit_account = account_pl
     >>> balance_non_deferral.execute('balance')
     >>> move, = balance_non_deferral.actions[0]
     >>> move.click('post')
     >>> [l for l in move.lines if l.analytic_lines]
     []
+
+Prevent changing root of account with entries::
+
+    >>> root2 = AnalyticAccount(type='root', name="Root2")
+    >>> root2.save()
+    >>> analytic_account.root = root2
+    >>> analytic_account.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    Traceback (most recent call last):
+        ...
+    AccessError: ...
+
+    >>> analytic_account.reload()
+    >>> analytic_account.code = "1"
+    >>> analytic_account.save()
+    >>> analytic_account.code
+    '1'
```

### Comparing `trytond_analytic_account-6.6.0/tests/test_module.py` & `trytond_analytic_account-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/PKG-INFO` & `trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-analytic-account
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for analytic accounting
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
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_account
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account
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
 
 Analytic Account Module
 #######################
 
 The analytic account module adds the fundamentals required to analyse
```

### Comparing `trytond_analytic_account-6.6.0/trytond_analytic_account.egg-info/SOURCES.txt` & `trytond_analytic_account-6.8.0/trytond_analytic_account.egg-info/SOURCES.txt`

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
@@ -71,14 +67,15 @@
 ./view/analytic_account_entry_tree.xml
 ./view/line_form.xml
 ./view/line_tree.xml
 ./view/move_line_form.xml
 ./view/move_line_list.xml
 ./view/rule_form.xml
 ./view/rule_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_analytic_account-6.6.0/view/account_form.xml` & `trytond_analytic_account-6.8.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/view/move_line_list.xml` & `trytond_analytic_account-6.8.0/view/move_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_analytic_account-6.6.0/view/rule_form.xml` & `trytond_analytic_account-6.8.0/view/rule_form.xml`

 * *Files identical despite different names*

