# Comparing `tmp/trytond_currency-6.6.1.tar.gz` & `tmp/trytond_currency-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_currency-6.6.1.tar", last modified: Mon Jan  2 22:59:04 2023, max compression
+gzip compressed data, was "trytond_currency-6.8.0.tar", last modified: Mon May  1 11:37:17 2023, max compression
```

## Comparing `trytond_currency-6.6.1.tar` & `trytond_currency-6.8.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.217268 trytond_currency-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     3617 2023-01-02 22:59:01.000000 trytond_currency-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-01-02 22:59:00.000000 trytond_currency-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2599 2023-01-02 22:59:04.217268 trytond_currency-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15253 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6572 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.213935 trytond_currency-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-01-02 20:25:44.000000 trytond_currency-6.6.1/ecb.py
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1364 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.213935 trytond_currency-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/icons/tryton-currency.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.203935 trytond_currency-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5012 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5977 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4810 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5914 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5185 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5949 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5901 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5480 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5615 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5532 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5369 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5853 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5764 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5654 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5789 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5186 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5015 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6453 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5390 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/message.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.203935 trytond_currency-6.6.1/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3404 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/scripts/import_currencies.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-01-02 22:59:04.217268 trytond_currency-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4789 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.207268 trytond_currency-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/scenario_currency_compute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/scenario_currency_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1295 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/scenario_currency_rate_update.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14005 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2022-12-19 12:03:07.000000 trytond_currency-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.217268 trytond_currency-6.6.1/trytond_currency.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2599 2023-01-02 22:59:03.000000 trytond_currency-6.6.1/trytond_currency.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-01-02 22:59:04.000000 trytond_currency-6.6.1/trytond_currency.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:59:03.000000 trytond_currency-6.6.1/trytond_currency.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-01-02 22:59:03.000000 trytond_currency-6.6.1/trytond_currency.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:59:03.000000 trytond_currency-6.6.1/trytond_currency.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-01-02 22:59:03.000000 trytond_currency-6.6.1/trytond_currency.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-01-02 22:59:03.000000 trytond_currency-6.6.1/trytond_currency.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:59:04.210601 trytond_currency-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/currency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/currency_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/currency_rate_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/currency_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2022-12-19 12:02:49.000000 trytond_currency-6.6.1/view/currency_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3753 2023-05-01 10:58:17.000000 trytond_currency-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 10:58:17.000000 trytond_currency-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15851 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6572 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.299201 trytond_currency-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-21 08:36:08.000000 trytond_currency-6.8.0/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3150 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/ecb.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1364 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.299201 trytond_currency-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/icons/tryton-currency.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.292534 trytond_currency-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5012 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5977 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4810 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5914 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5185 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5949 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5901 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5480 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5615 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5532 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5369 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5853 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5764 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5654 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5806 2023-04-30 10:46:36.000000 trytond_currency-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5015 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6453 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5390 2023-04-29 08:02:39.000000 trytond_currency-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/message.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.292534 trytond_currency-6.8.0/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3316 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/scripts/import_currencies.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4760 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.295868 trytond_currency-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/scenario_currency_compute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/scenario_currency_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1295 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/scenario_currency_rate_update.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14824 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-05-01 10:58:12.000000 trytond_currency-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.302534 trytond_currency-6.8.0/trytond_currency.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-05-01 11:37:17.000000 trytond_currency-6.8.0/trytond_currency.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_currency-6.8.0/trytond_currency.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:37:16.000000 trytond_currency-6.8.0/trytond_currency.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:17.295868 trytond_currency-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      705 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/view/currency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/view/currency_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-01-16 14:00:20.000000 trytond_currency-6.8.0/view/currency_rate_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/currency_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2023-04-15 07:12:15.000000 trytond_currency-6.8.0/view/currency_tree.xml
```

### Comparing `trytond_currency-6.6.1/CHANGELOG` & `trytond_currency-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-Version 6.6.1 - 2023-01-02
+
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Make symbol of currency optional
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Allow rounding with opposite method
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 --------------------------
```

### Comparing `trytond_currency-6.6.1/COPYRIGHT` & `trytond_currency-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_currency-6.6.1/LICENSE` & `trytond_currency-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/PKG-INFO` & `trytond_currency-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-currency/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/currency
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton currency
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -40,21 +40,21 @@
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
 Provides-Extra: data
 Provides-Extra: test
 Provides-Extra: completion
 License-File: LICENSE
 
 ###############
 Currency Module
```

### Comparing `trytond_currency-6.6.1/currency.py` & `trytond_currency-6.8.0/currency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
+import decimal
 import logging
-from decimal import ROUND_HALF_EVEN, Decimal, localcontext
+from decimal import Decimal, localcontext
 
 from dateutil.relativedelta import relativedelta
 from sql import Window
 from sql.functions import NthValue
 
 from trytond.i18n import gettext
 from trytond.model import (
@@ -20,22 +21,33 @@
 from .ecb import RatesNotAvailableError, get_rates
 from .exceptions import RateError
 from .ir import rate_decimal
 
 logger = logging.getLogger(__name__)
 
 
+ROUNDING_OPPOSITES = {
+    decimal.ROUND_HALF_EVEN: decimal.ROUND_HALF_EVEN,
+    decimal.ROUND_HALF_UP: decimal.ROUND_HALF_DOWN,
+    decimal.ROUND_HALF_DOWN: decimal.ROUND_HALF_UP,
+    decimal.ROUND_UP: decimal.ROUND_DOWN,
+    decimal.ROUND_DOWN: decimal.ROUND_UP,
+    decimal.ROUND_CEILING: decimal.ROUND_FLOOR,
+    decimal.ROUND_FLOOR: decimal.ROUND_CEILING,
+    }
+
+
 class Currency(
         SymbolMixin, DigitsMixin, DeactivableMixin, ModelSQL, ModelView):
     'Currency'
     __name__ = 'currency.currency'
     name = fields.Char('Name', required=True, translate=True,
         help="The main identifier of the currency.")
     symbol = fields.Char(
-        "Symbol", size=10, required=True, strip=False,
+        "Symbol", size=10, strip=False,
         help="The symbol used for currency formating.")
     code = fields.Char('Code', size=3, required=True,
         help="The 3 chars ISO currency code.")
     numeric_code = fields.Char('Numeric Code', size=3,
         help="The 3 digits ISO currency code.")
     rate = fields.Function(fields.Numeric(
             "Current rate", digits=(rate_decimal * 2, rate_decimal)),
@@ -73,25 +85,28 @@
                 'p_sign_posn', 'n_sign_posn']:
             table_h.not_null_action(col, 'remove')
 
         # Migration from 5.2: remove country data
         cursor.execute(*data.delete(where=(data.module == 'currency')
                 & (data.model == cls.__name__)))
 
+        # Migration from 6.6: remove required on symbol
+        table_h.not_null_action('symbol', 'remove')
+
     @staticmethod
     def default_rounding():
         return Decimal('0.01')
 
     @staticmethod
     def default_digits():
         return 2
 
     @classmethod
     def check_xml_record(cls, records, values):
-        return True
+        pass
 
     @classmethod
     def search_global(cls, text):
         for record, rec_name, icon in super(Currency, cls).search_global(text):
             icon = icon or 'tryton-currency'
             yield record, rec_name, icon
 
@@ -144,16 +159,18 @@
         for rate in rates:
             id2rate[rate.id] = rate
         for currency_id in res.keys():
             if res[currency_id]:
                 res[currency_id] = id2rate[res[currency_id]].rate
         return res
 
-    def round(self, amount, rounding=ROUND_HALF_EVEN):
+    def round(self, amount, rounding=decimal.ROUND_HALF_EVEN, opposite=False):
         'Round the amount depending of the currency'
+        if opposite:
+            rounding = ROUNDING_OPPOSITES[rounding]
         return self._round(amount, self.rounding, rounding)
 
     @classmethod
     def _round(cls, amount, factor, rounding):
         if not factor:
             return amount
         with localcontext() as ctx:
@@ -238,14 +255,16 @@
         return query
 
     def get_symbol(self, sign, symbol=None):
         pool = Pool()
         Lang = pool.get('ir.lang')
         lang = Lang.get()
         symbol, position = super().get_symbol(sign, symbol=symbol)
+        if not symbol:
+            symbol = self.code
         if ((sign < 0 and lang.n_cs_precedes)
                 or (sign >= 0 and lang.p_cs_precedes)):
             position = 0
         return symbol, position
 
 
 class CurrencyRate(ModelSQL, ModelView):
@@ -283,15 +302,15 @@
     @staticmethod
     def default_date():
         Date = Pool().get('ir.date')
         return Date.today()
 
     @classmethod
     def check_xml_record(cls, records, values):
-        return True
+        pass
 
     def get_rec_name(self, name):
         return str(self.date)
 
 
 class CronFetchError(Exception):
     pass
```

### Comparing `trytond_currency-6.6.1/currency.xml` & `trytond_currency-6.8.0/currency.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/doc/conf.py` & `trytond_currency-6.8.0/doc/conf.py`

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

### Comparing `trytond_currency-6.6.1/doc/configuration.rst` & `trytond_currency-6.8.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/doc/design.rst` & `trytond_currency-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/doc/usage.rst` & `trytond_currency-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/ecb.py` & `trytond_currency-6.8.0/ecb.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/fields.py` & `trytond_currency-6.8.0/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/icons/LICENSE` & `trytond_currency-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/ir.py` & `trytond_currency-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/bg.po` & `trytond_currency-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/ca.po` & `trytond_currency-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/cs.po` & `trytond_currency-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/de.po` & `trytond_currency-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/es.po` & `trytond_currency-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/es_419.po` & `trytond_currency-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/et.po` & `trytond_currency-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/fa.po` & `trytond_currency-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/fi.po` & `trytond_currency-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/fr.po` & `trytond_currency-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/hu.po` & `trytond_currency-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/id.po` & `trytond_currency-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/it.po` & `trytond_currency-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/lo.po` & `trytond_currency-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/lt.po` & `trytond_currency-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/nl.po` & `trytond_currency-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/pl.po` & `trytond_currency-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/pt.po` & `trytond_currency-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/ro.po` & `trytond_currency-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,14 @@
 msgid "Run"
 msgstr "Rulează"
 
 msgctxt "model:ir.ui.menu,name:menu_cron_form"
 msgid "Scheduled Rate Updates"
 msgstr "Actualizari Curs Valutar Programate"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_currency"
 msgid "Currencies"
 msgstr "Valute"
 
 msgctxt "model:ir.ui.menu,name:menu_currency_form"
 msgid "Currencies"
 msgstr "Valute"
@@ -205,15 +204,15 @@
 
 msgctxt "selection:currency.cron,frequency:"
 msgid "Weekly"
 msgstr "Săptămânal"
 
 msgctxt "selection:currency.cron,source:"
 msgid "European Central Bank"
-msgstr ""
+msgstr "Banca Europeană Centrală"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Update Currency Rates"
 msgstr "Actualizare Cursuri Valutare"
 
 msgctxt "view:currency.currency:"
 msgid "Rates"
```

### Comparing `trytond_currency-6.6.1/locale/ru.po` & `trytond_currency-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/sl.po` & `trytond_currency-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/tr.po` & `trytond_currency-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/uk.po` & `trytond_currency-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/locale/zh_CN.po` & `trytond_currency-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/message.xml` & `trytond_currency-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/scripts/import_currencies.py` & `trytond_currency-6.8.0/scripts/import_currencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,17 @@
 
     records = []
     for currency in _progress(pycountry.currencies):
         code = currency.alpha_3
         if code in currencies:
             record = currencies[code]
         else:
-            record = Currency(code=code, symbol=None)
+            record = Currency(code=code)
         record.name = _remove_forbidden_chars(currency.name)
         record.numeric_code = currency.numeric
-        if not record.symbol:
-            record.symbol = currency.alpha_3
         records.append(record)
 
     Currency.save(records)
     return {c.code: c for c in records}
 
 
 def translate_currencies(currencies):
```

### Comparing `trytond_currency-6.6.1/setup.py` & `trytond_currency-6.8.0/setup.py`

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
@@ -37,38 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_currency'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.9', 'python-dateutil']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus'), 'pycountry']
 
 setup(name=name,
     version=version,
     description='Tryton module with currencies',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-currency/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/currency',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton currency',
     package_dir={'trytond.modules.currency': '.'},
     packages=(
         ['trytond.modules.currency']
         + ['trytond.modules.currency.%s' % p for p in find_packages()]
         ),
@@ -106,24 +106,24 @@
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
     platforms='any',
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'data': ['pycountry', get_require_version('proteus')],
         'test': tests_require,
         'completion': ['argcomplete'],
         },
     zip_safe=False,
```

### Comparing `trytond_currency-6.6.1/tests/scenario_currency_compute.rst` & `trytond_currency-6.8.0/tests/scenario_currency_compute.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/tests/scenario_currency_rate_update.rst` & `trytond_currency-6.8.0/tests/scenario_currency_rate_update.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/tests/test_module.py` & `trytond_currency-6.8.0/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import datetime
 import unittest
-from decimal import Decimal
+from decimal import ROUND_HALF_DOWN, Decimal
 
 from trytond import backend
 from trytond.modules.currency.ecb import (
     RatesNotAvailableError, UnsupportedCurrencyError, get_rates)
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
 from trytond.transaction import Transaction
@@ -19,19 +19,17 @@
     return Currency.create([{
                 'name': name,
                 'symbol': name,
                 'code': name,
                 }])[0]
 
 
-def add_currency_rate(currency, rate, date=None):
+def add_currency_rate(currency, rate, date=datetime.date.min):
     pool = Pool()
     Rate = pool.get('currency.currency.rate')
-    if date is None:
-        date = Rate.default_date()
     return Rate.create([{
                 'currency': currency.id,
                 'rate': rate,
                 'date': date,
                 }])[0]
 
 
@@ -140,14 +138,37 @@
         cu.save()
 
         rounded = cu.round(Decimal('1.2345'))
 
         self.assertEqual(rounded, Decimal('1.2345'))
 
     @with_transaction()
+    def test_round_opposite(self):
+        "Test the opposite rounding"
+        cu = create_currency('cu')
+        cu.save()
+
+        rounded = cu.round(Decimal('1.235'))
+        self.assertEqual(rounded, Decimal('1.24'))
+        opposite_rounded = cu.round(Decimal('1.235'), opposite=True)
+        self.assertEqual(opposite_rounded, Decimal('1.24'))
+
+    @with_transaction()
+    def test_round_opposite_HALF_DOWN(self):
+        "Test the oposite rounding of ROUND_HALF_DOWN"
+        cu = create_currency('cu')
+        cu.save()
+
+        rounded = cu.round(Decimal('1.235'), rounding=ROUND_HALF_DOWN)
+        self.assertEqual(rounded, Decimal('1.23'))
+        opposite_rounded = cu.round(
+            Decimal('1.235'), rounding=ROUND_HALF_DOWN, opposite=True)
+        self.assertEqual(opposite_rounded, Decimal('1.24'))
+
+    @with_transaction()
     def test_is_zero(self):
         "Test is zero"
         cu = create_currency('cu')
         cu.rounding = Decimal('0.001')
         cu.digits = 3
         cu.save()
```

### Comparing `trytond_currency-6.6.1/tests/tools.py` & `trytond_currency-6.8.0/tests/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Get currency with code"
     Currency = Model.get('currency.currency', config=config)
     CurrencyRate = Model.get('currency.currency.rate', config=config)
 
     currencies = Currency.find([('code', '=', code)])
     if not currencies:
         currency = Currency(name=_names.get(code, code),
-            symbol=_symbols.get(code, code), code=code,
+            symbol=_symbols.get(code), code=code,
             rounding=Decimal('0.01'))
         currency.save()
         rate = _rates.get(code)
         if rate is not None:
             CurrencyRate(date=datetime.date.min, rate=rate,
                 currency=currency).save()
     else:
```

### Comparing `trytond_currency-6.6.1/trytond_currency.egg-info/PKG-INFO` & `trytond_currency-6.8.0/trytond_currency.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-currency
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-currency/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/currency
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton currency
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -40,21 +40,21 @@
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
 Provides-Extra: data
 Provides-Extra: test
 Provides-Extra: completion
 License-File: LICENSE
 
 ###############
 Currency Module
```

### Comparing `trytond_currency-6.6.1/trytond_currency.egg-info/SOURCES.txt` & `trytond_currency-6.8.0/trytond_currency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/view/cron_form.xml` & `trytond_currency-6.8.0/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-6.6.1/view/currency_form.xml` & `trytond_currency-6.8.0/view/currency_form.xml`

 * *Files identical despite different names*

