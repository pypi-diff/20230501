# Comparing `tmp/trytond_account_statement_aeb43-6.6.0.tar.gz` & `tmp/trytond_account_statement_aeb43-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_aeb43-6.6.0.tar", last modified: Mon Oct 31 16:05:18 2022, max compression
+gzip compressed data, was "trytond_account_statement_aeb43-6.8.0.tar", last modified: Mon May  1 11:39:53 2023, max compression
```

## Comparing `trytond_account_statement_aeb43-6.6.0.tar` & `trytond_account_statement_aeb43-6.8.0.tar`

### file list

```diff
@@ -1,59 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:05:18.838457 trytond_account_statement_aeb43-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_statement_aeb43-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_statement_aeb43-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2022-10-31 16:05:17.000000 trytond_account_statement_aeb43-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_statement_aeb43-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      799 2022-10-31 16:05:16.000000 trytond_account_statement_aeb43-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2022-10-31 16:05:16.000000 trytond_account_statement_aeb43-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_account_statement_aeb43-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_statement_aeb43-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2495 2022-10-31 16:05:18.838457 trytond_account_statement_aeb43-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2019-10-11 23:09:47.000000 trytond_account_statement_aeb43-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2019-06-04 16:49:46.000000 trytond_account_statement_aeb43-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:05:18.838457 trytond_account_statement_aeb43-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2019-10-11 23:09:47.000000 trytond_account_statement_aeb43-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:05:18.835124 trytond_account_statement_aeb43-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1780 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1982 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1801 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2022-10-29 07:50:33.000000 trytond_account_statement_aeb43-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:05:18.838457 trytond_account_statement_aeb43-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5294 2022-10-29 07:39:10.000000 trytond_account_statement_aeb43-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3868 2022-04-08 16:24:27.000000 trytond_account_statement_aeb43-6.6.0/statement.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2019-06-04 16:49:46.000000 trytond_account_statement_aeb43-6.6.0/statement.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:05:18.838457 trytond_account_statement_aeb43-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_statement_aeb43-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2019-06-04 16:49:46.000000 trytond_account_statement_aeb43-6.6.0/tests/n43.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3161 2022-04-08 16:23:26.000000 trytond_account_statement_aeb43-6.6.0/tests/scenario_account_statement_aeb43.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2022-04-16 16:30:56.000000 trytond_account_statement_aeb43-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_statement_aeb43-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2022-10-31 15:10:09.000000 trytond_account_statement_aeb43-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       93 2022-10-31 16:05:15.000000 trytond_account_statement_aeb43-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:05:18.838457 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2495 2022-10-31 16:05:18.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1547 2022-10-31 16:05:18.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:05:18.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2022-10-31 16:05:18.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:50.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2022-10-31 16:05:18.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:05:18.000000 trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:53.761143 trytond_account_statement_aeb43-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-05-01 11:00:03.000000 trytond_account_statement_aeb43-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      663 2023-05-01 11:00:03.000000 trytond_account_statement_aeb43-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2023-05-01 11:39:53.761143 trytond_account_statement_aeb43-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:53.757809 trytond_account_statement_aeb43-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:53.754476 trytond_account_statement_aeb43-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1780 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1805 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1982 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1801 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1805 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-04-30 10:46:36.000000 trytond_account_statement_aeb43-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-04-29 08:02:40.000000 trytond_account_statement_aeb43-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:39:53.761143 trytond_account_statement_aeb43-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4475 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3868 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/statement.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-6.8.0/statement.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:53.757809 trytond_account_statement_aeb43-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-01-16 14:00:20.000000 trytond_account_statement_aeb43-6.8.0/tests/n43.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3161 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/tests/scenario_account_statement_aeb43.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_statement_aeb43-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       93 2023-05-01 10:59:58.000000 trytond_account_statement_aeb43-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:39:53.761143 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2023-05-01 11:39:52.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-05-01 11:39:53.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:39:52.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-05-01 11:39:52.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-05-01 11:39:52.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:39:52.000000 trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/top_level.txt
```

### Comparing `trytond_account_statement_aeb43-6.6.0/CHANGELOG` & `trytond_account_statement_aeb43-6.8.0/CHANGELOG`

 * *Files 11% similar despite different names*

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

### Comparing `trytond_account_statement_aeb43-6.6.0/COPYRIGHT` & `trytond_account_statement_aeb43-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/LICENSE` & `trytond_account_statement_aeb43-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/PKG-INFO` & `trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_statement_aeb43
-Version: 6.6.0
+Name: trytond-account-statement-aeb43
+Version: 6.8.0
 Summary: Tryton module to import AEB43 statements
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement_aeb43
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement AEB 43
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 Account Statement AEB43 Module
 ##############################
 
 The Account Statement AEB43 module implements the import of the `Norm 43
```

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/bg.po` & `trytond_account_statement_aeb43-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/ca.po` & `trytond_account_statement_aeb43-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/cs.po` & `trytond_account_statement_aeb43-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/de.po` & `trytond_account_statement_aeb43-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/es.po` & `trytond_account_statement_aeb43-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/es_419.po` & `trytond_account_statement_aeb43-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/et.po` & `trytond_account_statement_aeb43-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/fa.po` & `trytond_account_statement_aeb43-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/fi.po` & `trytond_account_statement_aeb43-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/fr.po` & `trytond_account_statement_aeb43-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/hu.po` & `trytond_account_statement_aeb43-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/id.po` & `trytond_account_statement_aeb43-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/it.po` & `trytond_account_statement_aeb43-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/lo.po` & `trytond_account_statement_aeb43-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/lt.po` & `trytond_account_statement_aeb43-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/nl.po` & `trytond_account_statement_aeb43-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/pl.po` & `trytond_account_statement_aeb43-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/pt.po` & `trytond_account_statement_aeb43-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/ro.po` & `trytond_account_statement_aeb43-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/ru.po` & `trytond_account_statement_aeb43-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/sl.po` & `trytond_account_statement_aeb43-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/tr.po` & `trytond_account_statement_aeb43-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/uk.po` & `trytond_account_statement_aeb43-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/locale/zh_CN.po` & `trytond_account_statement_aeb43-6.8.0/locale/ro.po`

 * *Files 27% similar despite different names*

```diff
@@ -21,32 +21,51 @@
 "14:Returns and unpaids\n"
 "15:Payroll and social insurance\n"
 "16:Brokerage\n"
 "17:Interests, commissions and expenses\n"
 "98:Cancellations and seat corrections\n"
 "99:Others"
 msgstr ""
+"01:Rambursări\n"
+"02:Venituri\n"
+"03:Debite\n"
+"04:Transferuri\n"
+"05:Amortizarea Împrumut\n"
+"06:Remitențe\n"
+"07:Abonamente\n"
+"08:Dividende\n"
+"09:Tranzacții pe acțiuni\n"
+"10:Verificări benzină\n"
+"11:Aparat Numărar\n"
+"12:Carduri de credit\n"
+"13:Operațiuni în străinătate\n"
+"14:Retururi și neplătite\n"
+"15:Salarizare și asigurări sociale\n"
+"16:Brokeraj\n"
+"17:Dobânzi, comisioane și cheltuieli\n"
+"98:Anulări și corecții de locuri\n"
+"99:Alte"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_document_number"
 msgid "Document Number"
-msgstr ""
+msgstr "Număr Document"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_first_reference"
 msgid "First Reference"
-msgstr ""
+msgstr "Prima Referinţa"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_operation_date"
 msgid "Operation Date"
-msgstr ""
+msgstr "Data Operare"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_record_type"
 msgid "Record Type"
-msgstr ""
+msgstr "Tip Înregistrare"
 
 msgctxt ""
 "model:account.statement.origin.information,string:information_second_reference"
 msgid "Second Reference"
-msgstr ""
+msgstr "Referunţa Secundara"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_statement_aeb43-6.6.0/setup.py` & `trytond_account_statement_aeb43-6.8.0/setup.py`

 * *Files 18% similar despite different names*

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
 name = 'trytond_account_statement_aeb43'
 
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
 
 requires = ['python-stdnum', 'csb43>=0.8']
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
     description='Tryton module to import AEB43 statements',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_statement_aeb43',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement AEB 43',
     package_dir={'trytond.modules.account_statement_aeb43': '.'},
     packages=(
         ['trytond.modules.account_statement_aeb43']
         + ['trytond.modules.account_statement_aeb43.%s' % p
             for p in find_packages()]
@@ -125,27 +103,26 @@
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
     account_statement_aeb43 = trytond.modules.account_statement_aeb43
     """,
     )
```

### Comparing `trytond_account_statement_aeb43-6.6.0/statement.py` & `trytond_account_statement_aeb43-6.8.0/statement.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/statement.xml` & `trytond_account_statement_aeb43-6.8.0/statement.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/tests/scenario_account_statement_aeb43.rst` & `trytond_account_statement_aeb43-6.8.0/tests/scenario_account_statement_aeb43.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/PKG-INFO` & `trytond_account_statement_aeb43-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-statement-aeb43
-Version: 6.6.0
+Name: trytond_account_statement_aeb43
+Version: 6.8.0
 Summary: Tryton module to import AEB43 statements
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement_aeb43
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement AEB 43
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 Account Statement AEB43 Module
 ##############################
 
 The Account Statement AEB43 module implements the import of the `Norm 43
```

### Comparing `trytond_account_statement_aeb43-6.6.0/trytond_account_statement_aeb43.egg-info/SOURCES.txt` & `trytond_account_statement_aeb43-6.8.0/trytond_account_statement_aeb43.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

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
 setup.py
@@ -42,14 +38,15 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/n43.txt
 ./tests/scenario_account_statement_aeb43.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

