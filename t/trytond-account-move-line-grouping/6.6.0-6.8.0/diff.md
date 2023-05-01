# Comparing `tmp/trytond_account_move_line_grouping-6.6.0.tar.gz` & `tmp/trytond_account_move_line_grouping-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_move_line_grouping-6.6.0.tar", last modified: Mon Oct 31 15:51:38 2022, max compression
+gzip compressed data, was "trytond_account_move_line_grouping-6.8.0.tar", last modified: Mon May  1 11:38:55 2023, max compression
```

## Comparing `trytond_account_move_line_grouping-6.6.0.tar` & `trytond_account_move_line_grouping-6.8.0.tar`

### file list

```diff
@@ -1,69 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:38.626532 trytond_account_move_line_grouping-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_account_move_line_grouping-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 15:51:37.000000 trytond_account_move_line_grouping-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_move_line_grouping-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2022-10-31 15:51:36.000000 trytond_account_move_line_grouping-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 15:51:36.000000 trytond_account_move_line_grouping-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_move_line_grouping-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2022-10-31 15:51:38.626532 trytond_account_move_line_grouping-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2022-10-27 11:24:44.000000 trytond_account_move_line_grouping-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2022-04-11 17:29:59.000000 trytond_account_move_line_grouping-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8999 2022-05-19 20:16:01.000000 trytond_account_move_line_grouping-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6703 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:38.626532 trytond_account_move_line_grouping-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2022-10-27 11:24:44.000000 trytond_account_move_line_grouping-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_account_move_line_grouping-6.6.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:38.623198 trytond_account_move_line_grouping-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3962 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3991 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3963 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4019 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3500 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3410 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3987 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3400 2022-10-29 07:50:33.000000 trytond_account_move_line_grouping-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:51:38.626532 trytond_account_move_line_grouping-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5472 2022-10-29 07:39:10.000000 trytond_account_move_line_grouping-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:38.623198 trytond_account_move_line_grouping-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_move_line_grouping-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3744 2022-04-11 18:07:16.000000 trytond_account_move_line_grouping-6.6.0/tests/scenario_account_move_line_grouping.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2022-04-16 16:30:56.000000 trytond_account_move_line_grouping-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_move_line_grouping-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2022-10-31 15:10:09.000000 trytond_account_move_line_grouping-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 15:51:35.000000 trytond_account_move_line_grouping-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:38.626532 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2022-10-31 15:51:38.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2022-10-31 15:51:38.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:51:38.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-31 15:51:38.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-10-11 21:22:07.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2022-10-31 15:51:38.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:51:38.000000 trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:38.623198 trytond_account_move_line_grouping-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      539 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1475 2022-04-11 17:29:31.000000 trytond_account_move_line_grouping-6.6.0/view/move_line_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/view/move_line_group_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/view/move_line_group_form_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      617 2022-04-08 16:23:26.000000 trytond_account_move_line_grouping-6.6.0/view/move_line_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/view/move_line_group_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2021-10-30 15:32:33.000000 trytond_account_move_line_grouping-6.6.0/view/move_line_group_list_payabale_receivable.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:55.243750 trytond_account_move_line_grouping-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-05-01 10:59:25.000000 trytond_account_move_line_grouping-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 10:59:25.000000 trytond_account_move_line_grouping-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2437 2023-05-01 11:38:55.243750 trytond_account_move_line_grouping-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10141 2023-04-21 08:36:08.000000 trytond_account_move_line_grouping-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5857 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:55.240416 trytond_account_move_line_grouping-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:55.237083 trytond_account_move_line_grouping-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3755 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3783 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3755 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3810 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3272 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3194 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3777 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3184 2023-04-30 10:46:36.000000 trytond_account_move_line_grouping-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:38:55.243750 trytond_account_move_line_grouping-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4626 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:55.237083 trytond_account_move_line_grouping-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3744 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/tests/scenario_account_move_line_grouping.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 10:59:19.000000 trytond_account_move_line_grouping-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:55.243750 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2437 2023-05-01 11:38:54.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2052 2023-05-01 11:38:55.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:38:54.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 11:38:54.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-05-01 11:38:54.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:38:54.000000 trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:55.240416 trytond_account_move_line_grouping-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      539 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1475 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/view/move_line_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/view/move_line_group_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/view/move_line_group_form_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      617 2023-04-28 07:46:16.000000 trytond_account_move_line_grouping-6.8.0/view/move_line_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-28 07:46:16.000000 trytond_account_move_line_grouping-6.8.0/view/move_line_group_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-04-15 07:12:15.000000 trytond_account_move_line_grouping-6.8.0/view/move_line_group_list_payabale_receivable.xml
```

### Comparing `trytond_account_move_line_grouping-6.6.0/COPYRIGHT` & `trytond_account_move_line_grouping-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2022 Cédric Krier
+Copyright (C) 2021-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_move_line_grouping-6.6.0/LICENSE` & `trytond_account_move_line_grouping-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/PKG-INFO` & `trytond_account_move_line_grouping-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_move_line_grouping
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to display account move line grouped
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-move-line-grouping
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_move_line_grouping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account line group
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
 
 #################################
 Account Move Line Grouping Module
 #################################
```

### Comparing `trytond_account_move_line_grouping-6.6.0/__init__.py` & `trytond_account_move_line_grouping-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/account.py` & `trytond_account_move_line_grouping-6.8.0/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from sql import Literal, Null, Select, Window
+from sql import As, Literal, Null, Select, Window
 from sql.aggregate import BoolAnd, BoolOr, Min, Sum
 from sql.functions import CurrentTimestamp, FirstValue
 
 from trytond.model import ModelSQL, ModelView, fields
 from trytond.modules.account import MoveLineMixin
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Eval
+from trytond.pyson import Bool, Eval, If
 from trytond.transaction import Transaction
 
 
 class Move(metaclass=PoolMeta):
     __name__ = 'account.move'
 
     grouped_lines = fields.One2Many(
@@ -37,15 +37,21 @@
 
 
 class MoveLineGroup(MoveLineMixin, ModelSQL, ModelView):
     "Account Move Line Group"
     __name__ = 'account.move.line.group'
 
     move = fields.Many2One('account.move', "Move", readonly=True)
-    account = fields.Many2One('account.account', "Account", readonly=True)
+    account = fields.Many2One(
+        'account.account', "Account", readonly=True,
+        context={
+            'company': Eval('company', -1),
+            'period': Eval('period', -1),
+            },
+        depends={'company', 'period'})
     party = fields.Many2One(
         'party.party', "Party", readonly=True,
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     maturity_date = fields.Date("Maturity Date", readonly=True)
@@ -67,14 +73,19 @@
     delegated_amount = fields.Function(Monetary(
             "Delegated Amount",
             currency='amount_currency', digits='amount_currency',
             states={
                 'invisible': ~Eval('partially_reconciled', False),
                 }),
         'get_delegated_amount')
+    payable_receivable_balance = fields.Function(
+        Monetary(
+            "Payable/Receivable Balance",
+            currency='amount_currency', digits='amount_currency'),
+        'get_payable_receivable_balance')
 
     partially_reconciled = fields.Boolean(
         "Partially Reconciled", readonly=True)
     reconciled = fields.Boolean("Reconciled", readonly=True)
     amount_reconciled = Monetary(
         "Amount Reconciled",
         currency='currency', digits='currency', readonly=True)
@@ -139,14 +150,16 @@
             Literal(None).as_('write_uid'),
             Literal(None).as_('write_date'),
             ]
         grouped_columns = cls._grouped_columns(line)
         aggregated_columns = cls._aggregated_columns(line)
 
         columns = std_columns + grouped_columns + aggregated_columns
+        grouped_columns = [
+            c.expression if isinstance(c, As) else c for c in grouped_columns]
         return line.select(*columns, group_by=grouped_columns)
 
     @classmethod
     def _grouped_columns(cls, line):
         return [
             line.move,
             line.account,
@@ -173,21 +186,38 @@
     def get_states(cls):
         pool = Pool()
         Line = pool.get('account.move.line')
         return Line.fields_get(['state'])['state']['selection']
 
     @fields.depends('account')
     def on_change_with_currency(self, name=None):
-        if self.account:
-            return self.account.currency.id
+        return self.account.currency if self.account else None
 
     def get_delegated_amount(self, name):
         return self.amount_currency.round(
             sum(l.delegated_amount for l in self.lines if l.delegated_amount))
 
+    @classmethod
+    def view_attributes(cls):
+        attributes = super().view_attributes()
+        view_ids = cls._view_reconciliation_muted()
+        if Transaction().context.get('view_id') in view_ids:
+            attributes.append(
+                ('/tree', 'visual',
+                    If(Bool(Eval('reconciliation')), 'muted', '')))
+        return attributes
+
+    @classmethod
+    def _view_reconciliation_muted(cls):
+        pool = Pool()
+        ModelData = pool.get('ir.model.data')
+        return {ModelData.get_id(
+                'account_move_line_grouping',
+                'move_line_group_view_list_payable_receivable')}
+
 
 class MoveLineGroup_MoveLine(ModelSQL):
     "Account Move Line Group - Move Line"
     __name__ = 'account.move.line.group-move.line'
 
     group = fields.Many2One('account.move.line.group', "Group")
     line = fields.Many2One('account.move.line', "Line")
```

### Comparing `trytond_account_move_line_grouping-6.6.0/account.xml` & `trytond_account_move_line_grouping-6.8.0/account.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_account_move_line_grouping-6.6.0/account.xml` & `trytond_account_move_line_grouping-6.8.0/account.xml`

```diff
@@ -65,45 +65,30 @@
       <field name="keyword">tree_open</field>
       <field name="model">account.account,-1</field>
       <field name="action" ref="act_open_account"/>
     </record>
     <record model="ir.action.act_window" id="act_move_line_group_payable_receivable">
       <field name="name">Payable/Receivable Lines (Grouped)</field>
       <field name="res_model">account.move.line.group</field>
-      <field name="domain" eval="[['OR', ('account.type.receivable', '=', True), ('account.type.payable', '=', True)], If(Eval('active_ids', []) == [Eval('active_id')], ('party', '=', Eval('active_id')), ('party', 'in', Eval('active_ids'))), ('company', '=', Eval('context', {}).get('company', -1))]" pyson="1"/>
-      <field name="search_value" eval="[('reconciled', '=', False)]" pyson="1"/>
-      <field name="order" eval="[('date', 'DESC')]" pyson="1"/>
+      <field name="context_model">account.move.line.receivable_payable.context</field>
+      <field name="domain" eval="[('party', 'in', Eval('active_ids')), ('company', '=', Eval('context', {}).get('company', -1))]" pyson="1"/>
+      <field name="context_domain" eval="[['OR', If(Eval('receivable', True), ('account.type.receivable', '=', True), ('id', '&lt;', 0)), If(Eval('payable', True), ('account.type.payable', '=', True), ('id', '&lt;', 0))], If(Eval('reconciled', False), (), ('reconciled', '=', False))]" pyson="1"/>
+      <field name="search_value"/>
+      <field name="order" eval="[('maturity_date', 'ASC'), ('date', 'DESC'), ('id', 'DESC')]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_move_line_group_payable_receivable_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="move_line_group_view_list_payable_receivable"/>
       <field name="act_window" ref="act_move_line_group_payable_receivable"/>
     </record>
     <record model="ir.action.act_window.view" id="act_move_line_group_payable_receivable_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="move_line_group_view_form_payable_receivable"/>
       <field name="act_window" ref="act_move_line_group_payable_receivable"/>
     </record>
-    <record model="ir.action.act_window.domain" id="act_move_line_group_payable_receivable_domain_payable">
-      <field name="name">Payable</field>
-      <field name="sequence" eval="10"/>
-      <field name="domain" eval="[('account.type.payable', '=', True)]" pyson="1"/>
-      <field name="act_window" ref="act_move_line_group_payable_receivable"/>
-    </record>
-    <record model="ir.action.act_window.domain" id="act_move_line_group_payable_receivable_domain_receivable">
-      <field name="name">Receivable</field>
-      <field name="sequence" eval="20"/>
-      <field name="domain" eval="[('account.type.receivable', '=', True)]" pyson="1"/>
-      <field name="act_window" ref="act_move_line_group_payable_receivable"/>
-    </record>
-    <record model="ir.action.act_window.domain" id="act_move_line_group_payable_receivable_domain_all">
-      <field name="name">All</field>
-      <field name="sequence" eval="9999"/>
-      <field name="act_window" ref="act_move_line_group_payable_receivable"/>
-    </record>
     <record model="ir.action.keyword" id="act_move_line_group_payable_receivable_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">party.party,-1</field>
       <field name="action" ref="act_move_line_group_payable_receivable"/>
     </record>
     <record model="ir.action-res.group" id="act_move_line_group_payable_receivable-group_account">
       <field name="action" ref="act_move_line_group_payable_receivable"/>
```

### Comparing `trytond_account_move_line_grouping-6.6.0/doc/conf.py` & `trytond_account_move_line_grouping-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/bg.po` & `trytond_account_move_line_grouping-6.8.0/locale/nl.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,158 +1,151 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.move,grouped_lines:"
 msgid "Grouped Lines"
-msgstr ""
+msgstr "Gegroepeerde lijnen"
 
 msgctxt "field:account.move.line.group,account:"
 msgid "Account"
-msgstr ""
+msgstr "Rekening"
 
 msgctxt "field:account.move.line.group,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Bedrag"
 
 msgctxt "field:account.move.line.group,amount_currency:"
 msgid "Amount Currency"
-msgstr ""
+msgstr "Valuta bedrag"
 
 msgctxt "field:account.move.line.group,amount_reconciled:"
 msgid "Amount Reconciled"
-msgstr ""
+msgstr "Afgeletterd bedrag"
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Bedrag alternatieve valuta"
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
-msgstr ""
+msgstr "Bedrijf"
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Krediet"
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr ""
+msgstr "Effectieve datum"
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Debet"
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
-msgstr ""
+msgstr "Overgedragen bedrag"
 
 msgctxt "field:account.move.line.group,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Dagboek"
 
 msgctxt "field:account.move.line.group,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Regels"
 
 msgctxt "field:account.move.line.group,maturity_date:"
 msgid "Maturity Date"
-msgstr ""
+msgstr "Vervaldag"
 
 msgctxt "field:account.move.line.group,move:"
 msgid "Move"
-msgstr ""
+msgstr "Boeking"
 
 msgctxt "field:account.move.line.group,move_description:"
 msgid "Move Description"
-msgstr ""
+msgstr "Omschrijving boeking"
 
 msgctxt "field:account.move.line.group,move_origin:"
 msgid "Move Origin"
-msgstr ""
+msgstr "Oorsprong van de beweging"
 
 msgctxt "field:account.move.line.group,move_state:"
 msgid "Move State"
-msgstr ""
+msgstr "Status boeking"
 
 msgctxt "field:account.move.line.group,partially_reconciled:"
 msgid "Partially Reconciled"
-msgstr ""
+msgstr "Deels afgeletterd"
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
-msgstr ""
+msgstr "Relatiie"
+
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Betalen / Ontvangen Balans"
 
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
-msgstr ""
+msgstr "Periode"
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
-msgstr ""
+msgstr "Afgeletterd"
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
-msgstr ""
+msgstr "Tweede valuta"
 
 msgctxt "field:account.move.line.group,state:"
 msgid "State"
-msgstr ""
+msgstr "Staat"
 
 msgctxt "field:account.move.line.group-move.line,group:"
 msgid "Group"
-msgstr ""
+msgstr "Groep"
 
 msgctxt "field:account.move.line.group-move.line,line:"
 msgid "Line"
-msgstr ""
+msgstr "Regel"
 
 msgctxt "model:account.move.line.group,name:"
 msgid "Account Move Line Group"
-msgstr ""
+msgstr "Lijngroep boekhoudkundige bewegingen"
 
 msgctxt "model:account.move.line.group-move.line,name:"
 msgid "Account Move Line Group - Move Line"
-msgstr ""
+msgstr "Lijngroep boekhoudkundige bewegingen - Boekingslijn"
 
 msgctxt "model:ir.action,name:act_move_line_group_form"
 msgid "Account Move Lines (Grouped)"
-msgstr ""
+msgstr "Lijngroep boekhoudkundige bewegingen(Gegroepeerd)"
 
 msgctxt "model:ir.action,name:act_move_line_group_payable_receivable"
 msgid "Payable/Receivable Lines (Grouped)"
-msgstr ""
+msgstr "Te betalen/te ontvangen regels (gegroepeerd)"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
-msgstr ""
+msgstr "Boekingslijnen weergeven (gegroepeerd)"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr ""
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
+msgstr "Balans"
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
-msgstr ""
+msgstr "Krediet"
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
-msgstr ""
+msgstr "Debet"
 
 msgctxt "view:account.move.line.group:"
 msgid "Other Info"
-msgstr ""
+msgstr "Aanvullende informatie"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/ca.po` & `trytond_account_move_line_grouping-6.8.0/locale/fr.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,151 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.move,grouped_lines:"
 msgid "Grouped Lines"
-msgstr "Línies agrupades"
+msgstr "Lignes groupées"
 
 msgctxt "field:account.move.line.group,account:"
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.move.line.group,amount:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Montant"
 
 msgctxt "field:account.move.line.group,amount_currency:"
 msgid "Amount Currency"
-msgstr "Moneda de l'import"
+msgstr "Montant en devise"
 
 msgctxt "field:account.move.line.group,amount_reconciled:"
 msgid "Amount Reconciled"
-msgstr "Import conciliat"
+msgstr "Montant réconcilié"
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Import segona moneda"
+msgstr "Montant en devise secondaire"
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Société"
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
-msgstr "Haver"
+msgstr "Crédit"
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Devise"
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr "Data efectiva"
+msgstr "Date effective"
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
-msgstr "Deure"
+msgstr "Débit"
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
-msgstr "Import delegat"
+msgstr "Montant délégué"
 
 msgctxt "field:account.move.line.group,journal:"
 msgid "Journal"
-msgstr "Diari"
+msgstr "Journal"
 
 msgctxt "field:account.move.line.group,lines:"
 msgid "Lines"
-msgstr "Línies"
+msgstr "Lignes"
 
 msgctxt "field:account.move.line.group,maturity_date:"
 msgid "Maturity Date"
-msgstr "Data de venciment"
+msgstr "Date d'échéance"
 
 msgctxt "field:account.move.line.group,move:"
 msgid "Move"
-msgstr "Assentament"
+msgstr "Mouvement"
 
 msgctxt "field:account.move.line.group,move_description:"
 msgid "Move Description"
-msgstr "Descripció de l'assentament"
+msgstr "Description du mouvement"
 
 msgctxt "field:account.move.line.group,move_origin:"
 msgid "Move Origin"
-msgstr "Origen de l'assentament"
+msgstr "Origine du mouvement"
 
 msgctxt "field:account.move.line.group,move_state:"
 msgid "Move State"
-msgstr "Estat de l'assentament"
+msgstr "État du mouvement"
 
 msgctxt "field:account.move.line.group,partially_reconciled:"
 msgid "Partially Reconciled"
-msgstr "Conciliat parcialment"
+msgstr "Partiellement réconcilié"
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
-msgstr "Tercer"
+msgstr "Tiers"
+
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Balance à payer/recevoir"
 
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
-msgstr "Període"
+msgstr "Période"
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
-msgstr "Conciliat"
+msgstr "Réconciliée"
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Segona moneda"
+msgstr "Devise secondaire"
 
 msgctxt "field:account.move.line.group,state:"
 msgid "State"
-msgstr "Estat"
+msgstr "État"
 
 msgctxt "field:account.move.line.group-move.line,group:"
 msgid "Group"
-msgstr "Grup"
+msgstr "Groupe"
 
 msgctxt "field:account.move.line.group-move.line,line:"
 msgid "Line"
-msgstr "Línia"
+msgstr "Ligne"
 
 msgctxt "model:account.move.line.group,name:"
 msgid "Account Move Line Group"
-msgstr "Grup de línia d'assentament de compte"
+msgstr "Groupe de lignes de mouvements comptables"
 
 msgctxt "model:account.move.line.group-move.line,name:"
 msgid "Account Move Line Group - Move Line"
-msgstr "Grup de línia de moviment de compte - Apunt comptable"
+msgstr "Groupe de lignes de mouvements comptables - Ligne de mouvement"
 
 msgctxt "model:ir.action,name:act_move_line_group_form"
 msgid "Account Move Lines (Grouped)"
-msgstr "Apunts comptables (Agrupats)"
+msgstr "Lignes de mouvements comptables (groupées)"
 
 msgctxt "model:ir.action,name:act_move_line_group_payable_receivable"
 msgid "Payable/Receivable Lines (Grouped)"
-msgstr "Apunts a pagar/a cobrar (Agrupades)"
+msgstr "Lignes à payer/à recevoir (groupées)"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
-msgstr "Obre assentaments comptables (Agrupats)"
+msgstr "Ouvrir le mouvement comptable (groupé)"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr "Tot"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "A pagar"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "A cobrar"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
+msgstr "Balance"
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
-msgstr "Haver"
+msgstr "Crédit"
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
-msgstr "Deure"
+msgstr "Débit"
 
 msgctxt "view:account.move.line.group:"
 msgid "Other Info"
-msgstr "Informació addicional"
+msgstr "Autre information"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/cs.po` & `trytond_account_move_line_grouping-6.8.0/locale/id.po`

 * *Files 13% similar despite different names*

```diff
@@ -24,43 +24,43 @@
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
 msgstr ""
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
-msgstr ""
+msgstr "Perusahaan"
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Kredit"
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Mata Uang"
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr ""
+msgstr "Tanggal Efektif"
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Debit"
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
 msgstr ""
 
 msgctxt "field:account.move.line.group,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.move.line.group,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Baris"
 
 msgctxt "field:account.move.line.group,maturity_date:"
 msgid "Maturity Date"
 msgstr ""
 
 msgctxt "field:account.move.line.group,move:"
 msgid "Move"
@@ -80,19 +80,23 @@
 
 msgctxt "field:account.move.line.group,partially_reconciled:"
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
+msgstr "Pihak"
+
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
 msgstr ""
 
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
-msgstr ""
+msgstr "Periode"
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
@@ -126,33 +130,22 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
-msgstr ""
+msgstr "Kredit"
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
-msgstr ""
+msgstr "Debit"
 
 msgctxt "view:account.move.line.group:"
 msgid "Other Info"
-msgstr ""
+msgstr "Info Lain"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/de.po` & `trytond_account_move_line_grouping-6.8.0/locale/de.po`

 * *Files 7% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr "Teilweise abgestimmt"
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr "Partei"
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Forderungen/Verbindlichkeiten Saldo"
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr "Buchungszeitraum"
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr "Abgestimmt"
@@ -126,28 +130,17 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr "Buchungszeilen Forderungen/Verbindlichkeiten (Gruppiert)"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr "Buchungszeilen anzeigen (Gruppiert)"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr "Alle"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "Verbindlichkeiten"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "Forderungen"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
+msgstr "Saldo"
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr "Haben"
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/es.po` & `trytond_account_move_line_grouping-6.8.0/locale/es.po`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr "Conciliado parcialmente"
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr "Tercero"
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Saldo a pagar/a cobrar"
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr "Periodo"
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr "Conciliado"
@@ -126,28 +130,17 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr "Apuntes a pagar/a cobrar (Agrupados)"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr "Abrir cuenta de asiento (Agrupada)"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr "Todo"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "A pagar"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "A cobrar"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
+msgstr "Saldo"
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr "Haber"
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/es_419.po` & `trytond_account_move_line_grouping-6.8.0/locale/ca.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,158 +1,151 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.move,grouped_lines:"
 msgid "Grouped Lines"
-msgstr ""
+msgstr "Línies agrupades"
 
 msgctxt "field:account.move.line.group,account:"
 msgid "Account"
-msgstr ""
+msgstr "Compte"
 
 msgctxt "field:account.move.line.group,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Import"
 
 msgctxt "field:account.move.line.group,amount_currency:"
 msgid "Amount Currency"
-msgstr ""
+msgstr "Moneda de l'import"
 
 msgctxt "field:account.move.line.group,amount_reconciled:"
 msgid "Amount Reconciled"
-msgstr ""
+msgstr "Import conciliat"
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr ""
+msgstr "Import segona moneda"
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
-msgstr ""
+msgstr "Empresa"
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
-msgstr ""
+msgstr "Haver"
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr ""
+msgstr "Data efectiva"
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
-msgstr ""
+msgstr "Deure"
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
-msgstr ""
+msgstr "Import delegat"
 
 msgctxt "field:account.move.line.group,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Diari"
 
 msgctxt "field:account.move.line.group,lines:"
 msgid "Lines"
-msgstr ""
+msgstr "Línies"
 
 msgctxt "field:account.move.line.group,maturity_date:"
 msgid "Maturity Date"
-msgstr ""
+msgstr "Data de venciment"
 
 msgctxt "field:account.move.line.group,move:"
 msgid "Move"
-msgstr ""
+msgstr "Assentament"
 
 msgctxt "field:account.move.line.group,move_description:"
 msgid "Move Description"
-msgstr ""
+msgstr "Descripció de l'assentament"
 
 msgctxt "field:account.move.line.group,move_origin:"
 msgid "Move Origin"
-msgstr ""
+msgstr "Origen de l'assentament"
 
 msgctxt "field:account.move.line.group,move_state:"
 msgid "Move State"
-msgstr ""
+msgstr "Estat de l'assentament"
 
 msgctxt "field:account.move.line.group,partially_reconciled:"
 msgid "Partially Reconciled"
-msgstr ""
+msgstr "Conciliat parcialment"
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
-msgstr ""
+msgstr "Tercer"
+
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr "Saldo a pagar/a cobrar"
 
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
-msgstr ""
+msgstr "Període"
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
-msgstr ""
+msgstr "Conciliat"
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
-msgstr ""
+msgstr "Segona moneda"
 
 msgctxt "field:account.move.line.group,state:"
 msgid "State"
-msgstr ""
+msgstr "Estat"
 
 msgctxt "field:account.move.line.group-move.line,group:"
 msgid "Group"
-msgstr ""
+msgstr "Grup"
 
 msgctxt "field:account.move.line.group-move.line,line:"
 msgid "Line"
-msgstr ""
+msgstr "Línia"
 
 msgctxt "model:account.move.line.group,name:"
 msgid "Account Move Line Group"
-msgstr ""
+msgstr "Grup de línia d'assentament de compte"
 
 msgctxt "model:account.move.line.group-move.line,name:"
 msgid "Account Move Line Group - Move Line"
-msgstr ""
+msgstr "Grup de línia de moviment de compte - Apunt comptable"
 
 msgctxt "model:ir.action,name:act_move_line_group_form"
 msgid "Account Move Lines (Grouped)"
-msgstr ""
+msgstr "Apunts comptables (Agrupats)"
 
 msgctxt "model:ir.action,name:act_move_line_group_payable_receivable"
 msgid "Payable/Receivable Lines (Grouped)"
-msgstr ""
+msgstr "Apunts a pagar/a cobrar (Agrupades)"
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
-msgstr ""
+msgstr "Obre assentaments comptables (Agrupats)"
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr ""
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
+msgstr "Saldo"
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
-msgstr ""
+msgstr "Haver"
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
-msgstr ""
+msgstr "Deure"
 
 msgctxt "view:account.move.line.group:"
 msgid "Other Info"
-msgstr ""
+msgstr "Informació addicional"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/et.po` & `trytond_account_move_line_grouping-6.8.0/locale/it.po`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr ""
+msgstr "Decorrenza"
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
 msgstr ""
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/fa.po` & `trytond_account_move_line_grouping-6.8.0/locale/bg.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/fi.po` & `trytond_account_move_line_grouping-6.8.0/locale/cs.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/fr.po` & `trytond_account_move_line_grouping-6.8.0/locale/es_419.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,158 +1,151 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.move,grouped_lines:"
 msgid "Grouped Lines"
-msgstr "Lignes groupées"
+msgstr ""
 
 msgctxt "field:account.move.line.group,account:"
 msgid "Account"
-msgstr "Compte"
+msgstr ""
 
 msgctxt "field:account.move.line.group,amount:"
 msgid "Amount"
-msgstr "Montant"
+msgstr ""
 
 msgctxt "field:account.move.line.group,amount_currency:"
 msgid "Amount Currency"
-msgstr "Montant en devise"
+msgstr ""
 
 msgctxt "field:account.move.line.group,amount_reconciled:"
 msgid "Amount Reconciled"
-msgstr "Montant réconcilié"
+msgstr ""
 
 msgctxt "field:account.move.line.group,amount_second_currency:"
 msgid "Amount Second Currency"
-msgstr "Montant en devise secondaire"
+msgstr ""
 
 msgctxt "field:account.move.line.group,company:"
 msgid "Company"
-msgstr "Société"
+msgstr ""
 
 msgctxt "field:account.move.line.group,credit:"
 msgid "Credit"
-msgstr "Crédit"
+msgstr ""
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr ""
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr "Date effective"
+msgstr ""
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
-msgstr "Débit"
+msgstr ""
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
-msgstr "Montant délégué"
+msgstr ""
 
 msgctxt "field:account.move.line.group,journal:"
 msgid "Journal"
-msgstr "Journal"
+msgstr ""
 
 msgctxt "field:account.move.line.group,lines:"
 msgid "Lines"
-msgstr "Lignes"
+msgstr ""
 
 msgctxt "field:account.move.line.group,maturity_date:"
 msgid "Maturity Date"
-msgstr "Date d'échéance"
+msgstr ""
 
 msgctxt "field:account.move.line.group,move:"
 msgid "Move"
-msgstr "Mouvement"
+msgstr ""
 
 msgctxt "field:account.move.line.group,move_description:"
 msgid "Move Description"
-msgstr "Description du mouvement"
+msgstr ""
 
 msgctxt "field:account.move.line.group,move_origin:"
 msgid "Move Origin"
-msgstr "Origine du mouvement"
+msgstr ""
 
 msgctxt "field:account.move.line.group,move_state:"
 msgid "Move State"
-msgstr "État du mouvement"
+msgstr ""
 
 msgctxt "field:account.move.line.group,partially_reconciled:"
 msgid "Partially Reconciled"
-msgstr "Partiellement réconcilié"
+msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
-msgstr "Tiers"
+msgstr ""
+
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
 
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
-msgstr "Période"
+msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
-msgstr "Réconciliée"
+msgstr ""
 
 msgctxt "field:account.move.line.group,second_currency:"
 msgid "Second Currency"
-msgstr "Devise secondaire"
+msgstr ""
 
 msgctxt "field:account.move.line.group,state:"
 msgid "State"
-msgstr "État"
+msgstr ""
 
 msgctxt "field:account.move.line.group-move.line,group:"
 msgid "Group"
-msgstr "Groupe"
+msgstr ""
 
 msgctxt "field:account.move.line.group-move.line,line:"
 msgid "Line"
-msgstr "Ligne"
+msgstr ""
 
 msgctxt "model:account.move.line.group,name:"
 msgid "Account Move Line Group"
-msgstr "Groupe de lignes de mouvements comptables"
+msgstr ""
 
 msgctxt "model:account.move.line.group-move.line,name:"
 msgid "Account Move Line Group - Move Line"
-msgstr "Groupe de lignes de mouvements comptables - Ligne de mouvement"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_group_form"
 msgid "Account Move Lines (Grouped)"
-msgstr "Lignes de mouvements comptables (groupées)"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_group_payable_receivable"
 msgid "Payable/Receivable Lines (Grouped)"
-msgstr "Lignes à payer/à recevoir (groupées)"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
-msgstr "Ouvrir le mouvement comptable (groupé)"
+msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr "Toutes"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr "À payer"
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
-msgstr "À recevoir"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
+msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
-msgstr "Crédit"
+msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Debit"
-msgstr "Débit"
+msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Other Info"
-msgstr "Autre information"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/hu.po` & `trytond_account_move_line_grouping-6.8.0/locale/et.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/it.po` & `trytond_account_move_line_grouping-6.8.0/locale/fa.po`

 * *Files 22% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 msgctxt "field:account.move.line.group,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:account.move.line.group,date:"
 msgid "Effective Date"
-msgstr "Decorrenza"
+msgstr ""
 
 msgctxt "field:account.move.line.group,debit:"
 msgid "Debit"
 msgstr ""
 
 msgctxt "field:account.move.line.group,delegated_amount:"
 msgid "Delegated Amount"
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/lo.po` & `trytond_account_move_line_grouping-6.8.0/locale/fi.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/lt.po` & `trytond_account_move_line_grouping-6.8.0/locale/hu.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/pl.po` & `trytond_account_move_line_grouping-6.8.0/locale/lo.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/pt.po` & `trytond_account_move_line_grouping-6.8.0/locale/lt.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/ro.po` & `trytond_account_move_line_grouping-6.8.0/locale/pl.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/ru.po` & `trytond_account_move_line_grouping-6.8.0/locale/pt.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/sl.po` & `trytond_account_move_line_grouping-6.8.0/locale/ro.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/tr.po` & `trytond_account_move_line_grouping-6.8.0/locale/ru.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/uk.po` & `trytond_account_move_line_grouping-6.8.0/locale/sl.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/locale/zh_CN.po` & `trytond_account_move_line_grouping-6.8.0/locale/tr.po`

 * *Files 21% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 msgid "Partially Reconciled"
 msgstr ""
 
 msgctxt "field:account.move.line.group,party:"
 msgid "Party"
 msgstr ""
 
+msgctxt "field:account.move.line.group,payable_receivable_balance:"
+msgid "Payable/Receivable Balance"
+msgstr ""
+
 msgctxt "field:account.move.line.group,period:"
 msgid "Period"
 msgstr ""
 
 msgctxt "field:account.move.line.group,reconciled:"
 msgid "Reconciled"
 msgstr ""
@@ -126,27 +130,16 @@
 msgid "Payable/Receivable Lines (Grouped)"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_open_account"
 msgid "Open Move Account (Grouped)"
 msgstr ""
 
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_all"
-msgid "All"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_payable"
-msgid "Payable"
-msgstr ""
-
-msgctxt ""
-"model:ir.action.act_window.domain,name:act_move_line_group_payable_receivable_domain_receivable"
-msgid "Receivable"
+msgctxt "view:account.move.line.group:"
+msgid "Balance"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
 msgid "Credit"
 msgstr ""
 
 msgctxt "view:account.move.line.group:"
```

### Comparing `trytond_account_move_line_grouping-6.6.0/setup.py` & `trytond_account_move_line_grouping-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
@@ -37,64 +34,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_move_line_grouping'
 
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
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module to display account move line grouped',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/'
             'modules-account-move-line-grouping'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_move_line_grouping'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account line group',
     package_dir={'trytond.modules.account_move_line_grouping': '.'},
     packages=(
         ['trytond.modules.account_move_line_grouping']
         + ['trytond.modules.account_move_line_grouping.%s' % p
             for p in find_packages()]
@@ -131,27 +107,26 @@
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
     account_move_line_grouping = trytond.modules.account_move_line_grouping
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_move_line_grouping-6.6.0/tests/scenario_account_move_line_grouping.rst` & `trytond_account_move_line_grouping-6.8.0/tests/scenario_account_move_line_grouping.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/PKG-INFO` & `trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-move-line-grouping
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to display account move line grouped
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-move-line-grouping
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_move_line_grouping
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account line group
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
 
 #################################
 Account Move Line Grouping Module
 #################################
```

### Comparing `trytond_account_move_line_grouping-6.6.0/trytond_account_move_line_grouping.egg-info/SOURCES.txt` & `trytond_account_move_line_grouping-6.8.0/trytond_account_move_line_grouping.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_account_move_line_grouping-6.6.0/view/move_form.xml` & `trytond_account_move_line_grouping-6.8.0/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/view/move_line_group_form.xml` & `trytond_account_move_line_grouping-6.8.0/view/move_line_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/view/move_line_group_form_move.xml` & `trytond_account_move_line_grouping-6.8.0/view/move_line_group_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/view/move_line_group_form_payable_receivable.xml` & `trytond_account_move_line_grouping-6.8.0/view/move_line_group_form_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_move_line_grouping-6.6.0/view/move_line_group_list.xml` & `trytond_account_move_line_grouping-6.8.0/view/move_line_group_list.xml`

 * *Files identical despite different names*

