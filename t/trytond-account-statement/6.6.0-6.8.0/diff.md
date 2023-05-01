# Comparing `tmp/trytond_account_statement-6.6.0.tar.gz` & `tmp/trytond_account_statement-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement-6.6.0.tar", last modified: Mon Oct 31 16:02:56 2022, max compression
+gzip compressed data, was "trytond_account_statement-6.8.0.tar", last modified: Mon May  1 11:56:13 2023, max compression
```

## Comparing `trytond_account_statement-6.6.0.tar` & `trytond_account_statement-6.8.0.tar`

### file list

```diff
@@ -1,81 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:56.203050 trytond_account_statement-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_statement-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_statement-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 16:02:54.000000 trytond_account_statement-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_statement-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     4005 2022-10-31 16:02:53.000000 trytond_account_statement-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2022-10-31 16:02:53.000000 trytond_account_statement-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:18.000000 trytond_account_statement-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_statement-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4736 2022-10-31 16:02:56.203050 trytond_account_statement-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2440 2020-06-04 11:08:33.000000 trytond_account_statement-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2021-12-11 16:59:32.000000 trytond_account_statement-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2798 2021-12-11 16:59:32.000000 trytond_account_statement-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2022-04-08 16:23:26.000000 trytond_account_statement-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:56.199716 trytond_account_statement-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2440 2020-06-04 11:08:33.000000 trytond_account_statement-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2019-06-04 16:49:44.000000 trytond_account_statement-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4146 2022-10-23 16:32:37.000000 trytond_account_statement-6.6.0/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3163 2021-04-27 07:34:40.000000 trytond_account_statement-6.6.0/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:56.193050 trytond_account_statement-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14824 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15289 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13362 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15715 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15321 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13478 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14097 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16393 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13336 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15396 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14238 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13392 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14042 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15383 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13546 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15611 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13318 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14251 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12965 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14721 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14011 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13562 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12649 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13564 2022-10-29 07:50:41.000000 trytond_account_statement-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2989 2021-02-12 19:20:09.000000 trytond_account_statement-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2020-03-01 11:49:44.000000 trytond_account_statement-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:02:56.203050 trytond_account_statement-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5245 2022-10-29 07:39:10.000000 trytond_account_statement-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51346 2021-10-07 13:08:06.000000 trytond_account_statement-6.6.0/statement.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    45733 2022-10-15 14:01:54.000000 trytond_account_statement-6.6.0/statement.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19449 2021-11-23 23:59:55.000000 trytond_account_statement-6.6.0/statement.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:56.196383 trytond_account_statement-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_statement-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14921 2022-04-08 16:24:27.000000 trytond_account_statement-6.6.0/tests/scenario_account_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3021 2022-04-08 16:23:26.000000 trytond_account_statement-6.6.0/tests/scenario_statement_origin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3523 2022-04-08 16:24:27.000000 trytond_account_statement-6.6.0/tests/scenario_statement_origin_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2022-04-16 16:30:56.000000 trytond_account_statement-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_statement-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      712 2022-10-31 15:10:09.000000 trytond_account_statement-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2022-10-31 16:02:51.000000 trytond_account_statement-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:56.203050 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4736 2022-10-31 16:02:55.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2575 2022-10-31 16:02:56.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:02:55.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 16:02:55.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2022-10-31 16:02:55.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:02:55.000000 trytond_account_statement-6.6.0/trytond_account_statement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:56.196383 trytond_account_statement-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2021-10-07 13:08:06.000000 trytond_account_statement-6.6.0/view/line_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2021-10-07 13:08:06.000000 trytond_account_statement-6.6.0/view/line_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1713 2021-10-07 13:08:06.000000 trytond_account_statement-6.6.0/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2019-06-04 16:49:44.000000 trytond_account_statement-6.6.0/view/statement_import_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2021-06-28 22:31:36.000000 trytond_account_statement-6.6.0/view/statement_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-04-08 16:23:26.000000 trytond_account_statement-6.6.0/view/statement_journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      839 2022-04-08 16:24:27.000000 trytond_account_statement-6.6.0/view/statement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2022-04-08 16:24:27.000000 trytond_account_statement-6.6.0/view/statement_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2022-04-08 16:24:27.000000 trytond_account_statement-6.6.0/view/statement_line_tree_editable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2021-10-07 13:08:06.000000 trytond_account_statement-6.6.0/view/statement_origin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2021-10-07 13:08:06.000000 trytond_account_statement-6.6.0/view/statement_origin_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2020-09-11 23:31:15.000000 trytond_account_statement-6.6.0/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:13.239964 trytond_account_statement-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4257 2023-05-01 11:10:56.000000 trytond_account_statement-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:10:56.000000 trytond_account_statement-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4736 2023-05-01 11:56:13.239964 trytond_account_statement-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2450 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      869 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2798 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:13.236631 trytond_account_statement-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2450 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4140 2023-04-21 08:36:08.000000 trytond_account_statement-6.8.0/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3163 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:13.233297 trytond_account_statement-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14710 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15126 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13248 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15542 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15156 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13364 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13944 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16210 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13222 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15273 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14124 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13278 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13928 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15269 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13432 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15440 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13204 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14137 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12851 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14607 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13897 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13448 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12535 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13450 2023-04-30 10:46:36.000000 trytond_account_statement-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2828 2023-04-21 08:36:08.000000 trytond_account_statement-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:56:13.239964 trytond_account_statement-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4432 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51346 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/statement.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    45119 2023-04-21 08:36:08.000000 trytond_account_statement-6.8.0/statement.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19449 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/statement.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:13.236631 trytond_account_statement-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15166 2023-04-21 08:36:08.000000 trytond_account_statement-6.8.0/tests/scenario_account_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3029 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/tests/scenario_statement_origin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/tests/scenario_statement_origin_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-05-01 11:10:50.000000 trytond_account_statement-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:13.239964 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4736 2023-05-01 11:56:12.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2549 2023-05-01 11:56:13.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:56:12.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:56:12.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-05-01 11:56:12.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:56:12.000000 trytond_account_statement-6.8.0/trytond_account_statement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:13.236631 trytond_account_statement-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/line_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/line_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1713 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:20.000000 trytond_account_statement-6.8.0/view/statement_import_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      839 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-04-28 07:46:16.000000 trytond_account_statement-6.8.0/view/statement_line_tree_editable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_origin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-28 07:46:16.000000 trytond_account_statement-6.8.0/view/statement_origin_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_account_statement-6.8.0/view/statement_tree.xml
```

### Comparing `trytond_account_statement-6.6.0/CHANGELOG` & `trytond_account_statement-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Split line also when amount to pay of invoice is zero
+* Allow line with amount of zero
+* Remove support for Python 3.7
+* Add support for Python 3.11
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Require party on statement line if account requires one
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_statement-6.6.0/COPYRIGHT` & `trytond_account_statement-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_statement-6.6.0/LICENSE` & `trytond_account_statement-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/PKG-INFO` & `trytond_account_statement-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with account statements
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement
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
 
 Account Statement Module
 ########################
 
 The account_statement module allows to book statements. Statement can be used
@@ -144,15 +144,15 @@
 
 A wizard to import statements from an external system. It creates statements
 with origins filled.
 
 Configuration
 *************
 
-The account_statement module uses the section `account_statement` to retrieve
+The account_statement module uses the section ``account_statement`` to retrieve
 some parameters:
 
-- `filestore`: a boolean value to store origin file in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store origin file in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore.
-  The default value is `None`.
+- ``store_prefix``: the prefix to use with the FileStore.
+  The default value is ``None``.
```

### Comparing `trytond_account_statement-6.6.0/README.rst` & `trytond_account_statement-6.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 A wizard to import statements from an external system. It creates statements
 with origins filled.
 
 Configuration
 *************
 
-The account_statement module uses the section `account_statement` to retrieve
+The account_statement module uses the section ``account_statement`` to retrieve
 some parameters:
 
-- `filestore`: a boolean value to store origin file in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store origin file in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore.
-  The default value is `None`.
+- ``store_prefix``: the prefix to use with the FileStore.
+  The default value is ``None``.
```

### Comparing `trytond_account_statement-6.6.0/__init__.py` & `trytond_account_statement-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/account.py` & `trytond_account_statement-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/doc/index.rst` & `trytond_account_statement-6.8.0/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 A wizard to import statements from an external system. It creates statements
 with origins filled.
 
 Configuration
 *************
 
-The account_statement module uses the section `account_statement` to retrieve
+The account_statement module uses the section ``account_statement`` to retrieve
 some parameters:
 
-- `filestore`: a boolean value to store origin file in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store origin file in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore.
-  The default value is `None`.
+- ``store_prefix``: the prefix to use with the FileStore.
+  The default value is ``None``.
```

### Comparing `trytond_account_statement-6.6.0/journal.py` & `trytond_account_statement-6.8.0/journal.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @fields.depends('company')
     def on_change_with_company_party(self, name=None):
-        if self.company:
-            return self.company.party.id
+        return self.company.party if self.company else None
 
     @staticmethod
     def default_validation():
         return 'balance'
 
     @classmethod
     def get_by_bank_account(cls, company, number):
```

### Comparing `trytond_account_statement-6.6.0/journal.xml` & `trytond_account_statement-6.8.0/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/locale/bg.po` & `trytond_account_statement-6.8.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -411,18 +411,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/ca.po` & `trytond_account_statement-6.8.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -371,18 +371,14 @@
 "Per importar el extracte el diari \"%(journal)s\" ha de tenir la moneda "
 "\"%(currency)s\" en comptes de \"%(journal_currency)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Només es permet un diari per compte bancari."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "L'import de la línia d'extracte no pot ser zero."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 "Per contabilitzar l'assentament \"%(move)s\" heu de comptabilitzat "
 "l'extracte \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
```

### Comparing `trytond_account_statement-6.6.0/locale/cs.po` & `trytond_account_statement-6.8.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -383,18 +383,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/de.po` & `trytond_account_statement-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -373,18 +373,14 @@
 "\"%(journal)s\" die Währung \"%(currency)s\" verwendet werden anstatt "
 "\"%(journal_currency)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Es ist nur ein Journal pro Bankkonto erlaubt."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "Der Betrag einer Kontoauszugsposition darf nicht null sein."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 "Damit der Buchungssatz \"%(move)s\" festgeschrieben werden kann, muss zuerst"
 " der Auszug \"%(statement)s\" festgeschrieben werden."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
```

### Comparing `trytond_account_statement-6.6.0/locale/es.po` & `trytond_account_statement-6.8.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -372,18 +372,14 @@
 "Para importar extractos, el diario \"%(journal)s\" debe tener la moneda "
 "\"%(currency)s\" en lugar de \"%(journal_currency)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Solo se permite un diario por cuenta bancaria."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "El importe de línea de extracto no puede ser cero."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 "Para contabilizar el asiento \"%(move)s\" teneis que contabilizar el "
 "extracto \"%(statement)s\"."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
```

### Comparing `trytond_account_statement-6.6.0/locale/es_419.po` & `trytond_account_statement-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -380,18 +380,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/et.po` & `trytond_account_statement-6.8.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -374,18 +374,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "Aruande rea väärtus ei saa olla null."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/fa.po` & `trytond_account_statement-6.8.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -379,18 +379,14 @@
 "برای وارد کردن اضهارنامه، روزنامه : \"%(journal)s\" باید دارای ارز : "
 "\"%(currency)s\"بجای: \"%(journal_currency)s\" باشد."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "در هر حساب بانکی تنها یک روزنامه مجاز است."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "مبلغ سطر اظهارنامه نمی تواند صفر باشد."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr "برای حذف اظهارنامه : \"%(statement)s\" شما باید ابتدا آنرا لغو کنید."
```

### Comparing `trytond_account_statement-6.6.0/locale/fi.po` & `trytond_account_statement-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -381,18 +381,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/fr.po` & `trytond_account_statement-6.8.0/locale/fr.po`

 * *Files 4% similar despite different names*

```diff
@@ -346,15 +346,15 @@
 "model:ir.action.act_window.domain,name:act_statement_form_domain_draft"
 msgid "Draft"
 msgstr "Brouillons"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_posted"
 msgid "Posted"
-msgstr "Postés"
+msgstr "Comptabilisés"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_statement_form_domain_validated"
 msgid "Validated"
 msgstr "Validés"
 
 msgctxt "model:ir.message,text:msg_import_no_journal"
@@ -372,23 +372,19 @@
 "Pour importer le relevé, le journal « %(journal)s » doit avoir la devise "
 "« %(currency)s » au lieu de « %(journal_currency)s »."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Seulement un journal est permis par compte bancaire."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "Le montant de la ligne de relevé ne peut pas être zéro."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
-"Pour poster le mouvement « %(move)s », vous devez poster le relevé "
-"« %(statement)s »."
+"Pour comptabiliser le mouvement « %(move)s », vous devez comptabiliser le "
+"relevé « %(statement)s »."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr "Pour supprimer le relevé « %(statement)s », vous devez l'annuler."
 
 msgctxt "model:ir.message,text:msg_statement_invoice_paid_cancelled"
 msgid ""
@@ -406,16 +402,16 @@
 "La validation des relevés enlèvera les factures payées des autres relevés."
 
 msgctxt "model:ir.message,text:msg_statement_post_pending_amount"
 msgid ""
 "To post statement \"%(statement)s\" you must create lines for pending "
 "%(amount)s of origin \"%(origin)s\"."
 msgstr ""
-"Pour poster le relevé « %(statement)s », vous devez créer des lignes pour "
-"les %(amount)s en attente sur l'origine « %(origin)s »."
+"Pour comptabiliser le relevé « %(statement)s », vous devez créer des lignes "
+"pour les %(amount)s en attente sur l'origine « %(origin)s »."
 
 msgctxt "model:ir.message,text:msg_statement_wrong_end_balance"
 msgid ""
 "To validate statement \"%(statement)s\" you must change lines to have end "
 "balance of %(end_balance)s instead of %(amount)s."
 msgstr ""
 "Pour valider le relevé « %(statement)s », vous devez changer les lignes pour"
@@ -437,27 +433,27 @@
 "amount of %(total_amount)s instead of %(amount)s."
 msgstr ""
 "Pour valider le relevé « %(statement)s », vous devez changer les lignes pour"
 " avoir un montant total de %(total_amount)s au lieu de %(amount)s."
 
 msgctxt "model:ir.model.button,confirm:statement_post_button"
 msgid "Are you sure you want to post the statement?"
-msgstr "Êtes-vous sûr de vouloir poster le relevé ?"
+msgstr "Êtes-vous sûr de vouloir comptabiliser le relevé ?"
 
 msgctxt "model:ir.model.button,string:statement_cancel_button"
 msgid "Cancel"
 msgstr "Annuler"
 
 msgctxt "model:ir.model.button,string:statement_draft_button"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "model:ir.model.button,string:statement_post_button"
 msgid "Post"
-msgstr "Poster"
+msgstr "Comptabiliser"
 
 msgctxt "model:ir.model.button,string:statement_reconcile_button"
 msgid "Reconcile"
 msgstr "Réconcilier"
 
 msgctxt "model:ir.model.button,string:statement_validate_button"
 msgid "Validate"
@@ -557,15 +553,15 @@
 
 msgctxt "selection:account.statement,state:"
 msgid "Draft"
 msgstr "Brouillon"
 
 msgctxt "selection:account.statement,state:"
 msgid "Posted"
-msgstr "Posté"
+msgstr "Comptabilisé"
 
 msgctxt "selection:account.statement,state:"
 msgid "Validated"
 msgstr "Validé"
 
 msgctxt "selection:account.statement.journal,validation:"
 msgid "Amount"
```

### Comparing `trytond_account_statement-6.6.0/locale/hu.po` & `trytond_account_statement-6.8.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -372,18 +372,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/id.po` & `trytond_account_statement-6.8.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -370,18 +370,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/it.po` & `trytond_account_statement-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -398,18 +398,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/lo.po` & `trytond_account_statement-6.8.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -412,18 +412,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/lt.po` & `trytond_account_statement-6.8.0/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -386,18 +386,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/nl.po` & `trytond_account_statement-6.8.0/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -372,18 +372,14 @@
 "Om een bankafschrift te importeren, moet het dagboek \"%(journal)s\" de "
 "valuta \"%(currency)s\" hebben in plaats van \"%(journal_currency)s\"."
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Per bankrekening is slechts één dagboek toegestaan."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr "Het bedrag van een bankafschrift regel kan niet nul zijn."
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 "Om de boeking \"%(move)s\" te boeken moet u eerst bankafschrift "
 "\"%(statement)s\" boeken."
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
```

### Comparing `trytond_account_statement-6.6.0/locale/pl.po` & `trytond_account_statement-6.8.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -380,18 +380,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/pt.po` & `trytond_account_statement-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -391,18 +391,14 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr "Apenas um diário é permitido por conta bancária."
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/ro.po` & `trytond_account_statement-6.8.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -370,18 +370,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/ru.po` & `trytond_account_statement-6.8.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -425,18 +425,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/sl.po` & `trytond_account_statement-6.8.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -403,18 +403,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/tr.po` & `trytond_account_statement-6.8.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -392,18 +392,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/uk.po` & `trytond_account_statement-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -368,18 +368,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/locale/zh_CN.po` & `trytond_account_statement-6.8.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -391,18 +391,14 @@
 "\"%(currency)s\" instead of \"%(journal_currency)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_journal_bank_account_unique"
 msgid "Only one journal is allowed per bank account."
 msgstr ""
 
-msgctxt "model:ir.message,text:msg_line_amount_non_zero"
-msgid "Statement line amount cannot be zero."
-msgstr ""
-
 msgctxt "model:ir.message,text:msg_post_statement_move"
 msgid "To post the move \"%(move)s\" you must post the statement \"%(statement)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_statement_delete_cancel"
 msgid "To delete statement \"%(statement)s\" you must cancel it."
 msgstr ""
```

### Comparing `trytond_account_statement-6.6.0/message.xml` & `trytond_account_statement-6.8.0/message.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account_statement-6.6.0/message.xml` & `trytond_account_statement-6.8.0/message.xml`

```diff
@@ -32,15 +32,12 @@
     </record>
     <record model="ir.message" id="msg_statement_paid_invoice_draft">
       <field name="text">The validation of the statements will remove paid invoices from other statements.</field>
     </record>
     <record model="ir.message" id="msg_statement_post_pending_amount">
       <field name="text">To post statement &quot;%(statement)s&quot; you must create lines for pending %(amount)s of origin &quot;%(origin)s&quot;.</field>
     </record>
-    <record model="ir.message" id="msg_line_amount_non_zero">
-      <field name="text">Statement line amount cannot be zero.</field>
-    </record>
     <record model="ir.message" id="msg_post_statement_move">
       <field name="text">To post the move &quot;%(move)s&quot; you must post the statement &quot;%(statement)s&quot;.</field>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_statement-6.6.0/setup.py` & `trytond_account_statement-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
 name = 'trytond_account_statement'
 
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
 
 requires = ['python-sql >= 0.4']
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
     description='Tryton module with account statements',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_statement',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement',
     package_dir={'trytond.modules.account_statement': '.'},
     packages=(
         ['trytond.modules.account_statement']
         + ['trytond.modules.account_statement.%s' % p for p in find_packages()]
         ),
@@ -124,28 +102,27 @@
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
     account_statement = trytond.modules.account_statement
     """,
     )
```

### Comparing `trytond_account_statement-6.6.0/statement.fodt` & `trytond_account_statement-6.8.0/statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/statement.py` & `trytond_account_statement-6.8.0/statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sql.aggregate import Max, Sum
 from sql.conditionals import Coalesce
 from sql.operators import Concat
 
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
-    Check, DictSchemaMixin, Index, ModelSQL, ModelView, Workflow, fields,
+    DictSchemaMixin, Index, ModelSQL, ModelView, Workflow, fields,
     sequence_ordered)
 from trytond.model.exceptions import AccessError
 from trytond.modules.company import CompanyReport
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
 from trytond.rpc import RPC
@@ -227,16 +227,15 @@
             return
 
         statement, = statements
         self.start_balance = statement.end_balance
 
     @fields.depends('journal')
     def on_change_with_currency(self, name=None):
-        if self.journal:
-            return self.journal.currency.id
+        return self.journal.currency if self.journal else None
 
     @fields.depends('start_balance', 'end_balance')
     def on_change_with_balance(self, name=None):
         return ((getattr(self, 'end_balance', 0) or 0)
             - (getattr(self, 'start_balance', 0) or 0))
 
     @fields.depends('origins', 'lines', 'journal', 'company')
@@ -281,46 +280,39 @@
                             invoice_id2amount_to_pay[line.invoice.id] = (
                                 line.amount + amount_to_pay)
                     else:
                         line.invoice = None
             origin.lines = lines
         self.origins = origins
 
-    @fields.depends('lines', 'journal', 'company')
+    @fields.depends('lines')
     def on_change_lines(self):
         pool = Pool()
         Line = pool.get('account.statement.line')
-        if not self.journal or not self.lines or not self.company:
-            return
-        if self.journal.currency != self.company.currency:
-            return
 
-        invoices = set()
-        for line in self.lines:
-            if (line.invoice
-                    and line.invoice.currency == self.company.currency):
-                invoices.add(line.invoice)
+        invoices = {l.invoice for l in self.lines if l.invoice}
         invoice_id2amount_to_pay = {}
         for invoice in invoices:
             if invoice.type == 'out':
                 sign = -1
             else:
                 sign = 1
             invoice_id2amount_to_pay[invoice.id] = sign * invoice.amount_to_pay
 
         lines = list(self.lines)
         line_offset = 0
         for index, line in enumerate(self.lines or []):
             if line.invoice and line.id:
                 if line.invoice.id not in invoice_id2amount_to_pay:
                     continue
+                if getattr(line, 'amount', None) is None:
+                    continue
                 amount_to_pay = invoice_id2amount_to_pay[line.invoice.id]
-                if (amount_to_pay
-                        and getattr(line, 'amount', None)
-                        and (line.amount >= 0) == (amount_to_pay <= 0)):
+                if ((line.amount > 0) == (amount_to_pay < 0)
+                        or not amount_to_pay):
                     if abs(line.amount) > abs(amount_to_pay):
                         new_line = Line()
                         for field_name, field in Line._fields.items():
                             if field_name == 'id':
                                 continue
                             try:
                                 setattr(new_line, field_name,
@@ -550,14 +542,16 @@
 
         move_lines = []
         for move, statement, lines in moves:
             amount = 0
             amount_second_currency = 0
             for line in lines:
                 move_line = line.get_move_line()
+                if not move_line:
+                    continue
                 move_line.move = move
                 amount += move_line.debit - move_line.credit
                 if move_line.amount_second_currency:
                     amount_second_currency += move_line.amount_second_currency
                 move_lines.append((move_line, line))
 
             move_line = statement._get_move_line(
@@ -572,17 +566,17 @@
 
     def _get_move(self, key):
         'Return Move for the grouping key'
         pool = Pool()
         Move = pool.get('account.move')
         Period = pool.get('account.period')
 
-        period_id = Period.find(self.company.id, date=key['date'])
+        period = Period.find(self.company, date=key['date'])
         return Move(
-            period=period_id,
+            period=period,
             journal=self.journal.journal,
             date=key['date'],
             origin=self,
             company=self.company,
             description=str(key['number']),
             )
 
@@ -719,25 +713,24 @@
         @fields.depends('statement', '_parent_statement.state')
         def on_change_with_statement_state(self, name=None):
             if self.statement:
                 return self.statement.state
 
         @fields.depends('statement', '_parent_statement.company')
         def on_change_with_company(self, name=None):
-            if self.statement and self.statement.company:
-                return self.statement.company.id
+            return self.statement.company if self.statement else None
 
         @classmethod
         def search_company(cls, name, clause):
             return [('statement.' + clause[0],) + tuple(clause[1:])]
 
         @fields.depends('statement', '_parent_statement.journal')
         def on_change_with_currency(self, name=None):
             if self.statement and self.statement.journal:
-                return self.statement.journal.currency.id
+                return self.statement.journal.currency
 
     return Mixin
 
 
 _states = {
     'readonly': Eval('statement_state') != 'draft',
     }
@@ -753,14 +746,15 @@
             ],
         depends=['company'])
     related_to = fields.Reference(
         "Related To", 'get_relations',
         domain={
             'account.invoice': [
                 ('company', '=', Eval('company', -1)),
+                ('currency', '=', Eval('currency', -1)),
                 If(Bool(Eval('party')),
                     ['OR',
                         ('party', '=', Eval('party', -1)),
                         ('alternative_payees', '=', Eval('party', -1)),
                         ],
                     []),
                 If(Bool(Eval('account')),
@@ -794,19 +788,14 @@
                 | Bool(Eval('origin', 0))),
             }
         cls.account.required = True
         cls.party.states = {
             'required': (Eval('party_required', False)
                 & (Eval('statement_state') == 'draft')),
             }
-        t = cls.__table__()
-        cls._sql_constraints += [
-            ('check_statement_line_amount', Check(t, t.amount != 0),
-                'account_statement.msg_line_amount_non_zero'),
-            ]
 
     @classmethod
     def __register__(cls, module):
         table = cls.__table__()
 
         super().__register__(module)
 
@@ -817,14 +806,17 @@
         if table_h.column_exist('invoice'):
             cursor.execute(*table.update(
                     [table.related_to],
                     [Concat('account.invoice,', table.invoice)],
                     where=table.invoice != Null))
             table_h.drop_column('invoice')
 
+        # Migration from 6.6: Allow amount of zero
+        table_h.drop_constraint('check_statement_line_amount')
+
     @property
     @fields.depends('related_to')
     def invoice(self):
         pool = Pool()
         Invoice = pool.get('account.invoice')
         related_to = getattr(self, 'related_to', None)
         if isinstance(related_to, Invoice) and related_to.id >= 0:
@@ -875,38 +867,26 @@
                 self.invoice = None
 
     @fields.depends(
         'amount', 'party', 'account', 'date',
         'statement', '_parent_statement.journal',
         methods=['invoice'])
     def on_change_amount(self):
-        Currency = Pool().get('currency.currency')
         if self.party:
             with Transaction().set_context(date=self.date):
                 if self.account and self.account not in (
                         self.party.account_receivable_used,
                         self.party.account_payable_used):
                     # The user has entered a non-default value, we keep it.
                     pass
                 elif self.amount:
                     if self.amount > Decimal("0.0"):
                         self.account = self.party.account_receivable_used
                     else:
                         self.account = self.party.account_payable_used
-        if self.invoice:
-            if self.amount and self.statement and self.statement.journal:
-                invoice = self.invoice
-                journal = self.statement.journal
-                with Transaction().set_context(date=invoice.currency_date):
-                    amount_to_pay = Currency.compute(invoice.currency,
-                        invoice.amount_to_pay, journal.currency)
-                if abs(self.amount) > amount_to_pay:
-                    self.invoice = None
-            else:
-                self.invoice = None
 
     @fields.depends('account', methods=['invoice'])
     def on_change_account(self):
         if self.invoice:
             if self.account:
                 if self.invoice.account != self.account:
                     self.invoice = None
@@ -945,19 +925,19 @@
                 self.account = self.origin.account
             else:
                 self.on_change_party()
 
     @fields.depends('origin', '_parent_origin.company')
     def on_change_with_company(self, name=None):
         try:
-            company = super(Line, self).on_change_with_company()
+            company = super().on_change_with_company()
         except AttributeError:
             company = None
-        if self.origin and self.origin.company:
-            return self.origin.company.id
+        if self.origin and hasattr(self.origin, 'company'):
+            company = self.origin.company
         return company
 
     @fields.depends('origin', '_parent_origin.statement_state')
     def on_change_with_statement_state(self, name=None):
         try:
             state = super(Line, self).on_change_with_statement_state()
         except AttributeError:
@@ -1000,16 +980,23 @@
             # get_reconcile_lines_for_amount
             if line.invoice in invoice_payments:
                 Invoice.add_payment_lines(invoice_payments)
                 invoice_payments.clear()
                 MoveLine.reconcile(*to_reconcile)
                 to_reconcile.clear()
 
+            if move_line.second_currency:
+                amount = move_line.amount_second_currency
+                currency = move_line.second_currency
+            else:
+                amount = move_line.credit - move_line.debit
+                currency = line.company.currency
+
             reconcile_lines = line.invoice.get_reconcile_lines_for_amount(
-                move_line.credit - move_line.debit, party=line.party)
+                amount, currency, party=line.party)
 
             assert move_line.account == line.invoice.account
 
             invoice_payments[line.invoice].append(move_line.id)
             if not reconcile_lines[1]:
                 to_reconcile.append(reconcile_lines[0] + [move_line])
         if invoice_payments:
@@ -1039,14 +1026,16 @@
         '''
         Return the move line for the statement line
         '''
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         Currency = Pool().get('currency.currency')
         zero = Decimal("0.0")
+        if not self.amount:
+            return
         with Transaction().set_context(date=self.date):
             amount = Currency.compute(self.statement.journal.currency,
                 self.amount, self.statement.company.currency)
         if self.statement.journal.currency != self.statement.company.currency:
             second_currency = self.statement.journal.currency.id
             amount_second_currency = -self.amount
         else:
```

### Comparing `trytond_account_statement-6.6.0/statement.xml` & `trytond_account_statement-6.8.0/statement.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/tests/scenario_account_statement.rst` & `trytond_account_statement-6.8.0/tests/scenario_account_statement.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 ==========================
 Account Statement Scenario
 ==========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_statement', 'account_invoice'])
 
 Create company::
 
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
     >>> receivable = accounts['receivable']
@@ -182,14 +183,23 @@
     >>> statement_line.amount = Decimal('-60')
     >>> statement_line.party = supplier
     >>> statement_line.account == payable
     True
     >>> statement_line.related_to = supplier_invoice
     >>> statement_line.amount
     Decimal('-50.00')
+    >>> statement_line = statement.lines[-1]
+    >>> statement_line.amount
+    Decimal('-10.00')
+
+Try to overpay supplier invoice::
+
+    >>> statement_line.related_to = supplier_invoice
+    >>> statement_line.amount
+    Decimal('-0.00')
     >>> statement_line = statement.lines.pop()
     >>> statement_line.amount
     Decimal('-10.00')
 
     >>> statement.save()
 
 Validate statement::
```

### Comparing `trytond_account_statement-6.6.0/tests/scenario_statement_origin.rst` & `trytond_account_statement-6.8.0/tests/scenario_statement_origin.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 =================================
 Account Statement Origin Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement')
 
 Create company::
 
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
     >>> receivable = accounts['receivable']
```

### Comparing `trytond_account_statement-6.6.0/tests/scenario_statement_origin_invoices.rst` & `trytond_account_statement-6.8.0/tests/scenario_statement_origin_invoices.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 ==========================================
 Account Statement Origin Invoices Scenario
 ==========================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement')
 
 Create company::
 
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
     >>> receivable = accounts['receivable']
```

### Comparing `trytond_account_statement-6.6.0/trytond_account_statement.egg-info/PKG-INFO` & `trytond_account_statement-6.8.0/trytond_account_statement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-statement
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with account statements
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement
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
 
 Account Statement Module
 ########################
 
 The account_statement module allows to book statements. Statement can be used
@@ -144,15 +144,15 @@
 
 A wizard to import statements from an external system. It creates statements
 with origins filled.
 
 Configuration
 *************
 
-The account_statement module uses the section `account_statement` to retrieve
+The account_statement module uses the section ``account_statement`` to retrieve
 some parameters:
 
-- `filestore`: a boolean value to store origin file in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store origin file in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore.
-  The default value is `None`.
+- ``store_prefix``: the prefix to use with the FileStore.
+  The default value is ``None``.
```

### Comparing `trytond_account_statement-6.6.0/trytond_account_statement.egg-info/SOURCES.txt` & `trytond_account_statement-6.8.0/trytond_account_statement.egg-info/SOURCES.txt`

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
 ./view/statement_journal_tree.xml
 ./view/statement_line_form.xml
 ./view/statement_line_tree.xml
 ./view/statement_line_tree_editable.xml
 ./view/statement_origin_form.xml
 ./view/statement_origin_tree.xml
 ./view/statement_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_statement-6.6.0/view/line_group_form.xml` & `trytond_account_statement-6.8.0/view/line_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/view/statement_form.xml` & `trytond_account_statement-6.8.0/view/statement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/view/statement_journal_form.xml` & `trytond_account_statement-6.8.0/view/statement_journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/view/statement_line_form.xml` & `trytond_account_statement-6.8.0/view/statement_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/view/statement_line_tree_editable.xml` & `trytond_account_statement-6.8.0/view/statement_line_tree_editable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-6.6.0/view/statement_origin_form.xml` & `trytond_account_statement-6.8.0/view/statement_origin_form.xml`

 * *Files identical despite different names*

