# Comparing `tmp/trytond_account_invoice_watermark-6.6.1.tar.gz` & `tmp/trytond_account_invoice_watermark-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_watermark-6.6.1.tar", last modified: Mon Jan  2 23:00:43 2023, max compression
+gzip compressed data, was "trytond_account_invoice_watermark-6.8.0.tar", last modified: Mon May  1 11:50:24 2023, max compression
```

## Comparing `trytond_account_invoice_watermark-6.6.1.tar` & `trytond_account_invoice_watermark-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 23:00:43.072144 trytond_account_invoice_watermark-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-01-02 23:00:40.000000 trytond_account_invoice_watermark-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-01-02 23:00:39.000000 trytond_account_invoice_watermark-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2561 2023-01-02 23:00:43.072144 trytond_account_invoice_watermark-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2648 2023-01-02 20:25:44.000000 trytond_account_invoice_watermark-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1167 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 23:00:43.068810 trytond_account_invoice_watermark-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    31593 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/invoice_watermark_draft.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    30602 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/invoice_watermark_paid.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 23:00:43.065477 trytond_account_invoice_watermark-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      479 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      479 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-01-02 23:00:43.072144 trytond_account_invoice_watermark-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4776 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 23:00:43.068810 trytond_account_invoice_watermark-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/tests/scenario_account_invoice_watermark.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2022-12-19 12:02:49.000000 trytond_account_invoice_watermark-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-12-19 12:03:07.000000 trytond_account_invoice_watermark-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 23:00:43.072144 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2561 2023-01-02 23:00:42.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-01-02 23:00:43.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 23:00:42.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-01-02 23:00:42.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 23:00:42.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-01-02 23:00:42.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-01-02 23:00:42.000000 trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:24.048964 trytond_account_invoice_watermark-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-05-01 11:06:54.000000 trytond_account_invoice_watermark-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:06:54.000000 trytond_account_invoice_watermark-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2543 2023-05-01 11:50:24.048964 trytond_account_invoice_watermark-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2648 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1167 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:24.045631 trytond_account_invoice_watermark-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    31593 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/invoice_watermark_draft.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    30602 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/invoice_watermark_paid.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:24.042297 trytond_account_invoice_watermark-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      479 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      479 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-29 08:02:45.000000 trytond_account_invoice_watermark-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:50:24.048964 trytond_account_invoice_watermark-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4715 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:24.045631 trytond_account_invoice_watermark-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2931 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/tests/scenario_account_invoice_watermark.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:06:49.000000 trytond_account_invoice_watermark-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:24.048964 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2543 2023-05-01 11:50:23.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-05-01 11:50:23.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:50:23.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 11:50:23.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-05-01 11:50:23.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:50:23.000000 trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/top_level.txt
```

### Comparing `trytond_account_invoice_watermark-6.6.1/COPYRIGHT` & `trytond_account_invoice_watermark-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2022 B2CK
-Copyright (C) 2021-2022 Cédric Krier
+Copyright (C) 2021-2023 B2CK
+Copyright (C) 2021-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_watermark-6.6.1/LICENSE` & `trytond_account_invoice_watermark-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-6.6.1/PKG-INFO` & `trytond_account_invoice_watermark-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_watermark
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add watermark to invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-watermark
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_watermark
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice watermark
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
 
 ################################
 Account Invoice Watermark Module
 ################################
```

### Comparing `trytond_account_invoice_watermark-6.6.1/account.py` & `trytond_account_invoice_watermark-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-6.6.1/account.xml` & `trytond_account_invoice_watermark-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-6.6.1/doc/conf.py` & `trytond_account_invoice_watermark-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_invoice_watermark-6.6.1/invoice_watermark_draft.fodt` & `trytond_account_invoice_watermark-6.8.0/invoice_watermark_draft.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-6.6.1/invoice_watermark_paid.fodt` & `trytond_account_invoice_watermark-6.8.0/invoice_watermark_paid.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-6.6.1/setup.py` & `trytond_account_invoice_watermark-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -37,41 +34,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_invoice_watermark'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['PyPDF2']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module to add watermark to invoice',
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
             'modules-account-invoice-watermark'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_invoice_watermark'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice watermark',
     package_dir={'trytond.modules.account_invoice_watermark': '.'},
     packages=(
         ['trytond.modules.account_invoice_watermark']
         + ['trytond.modules.account_invoice_watermark.%s' % p
             for p in find_packages()]
@@ -109,24 +108,24 @@
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

### Comparing `trytond_account_invoice_watermark-6.6.1/tests/scenario_account_invoice_watermark.rst` & `trytond_account_invoice_watermark-6.8.0/tests/scenario_account_invoice_watermark.rst`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     >>> pdf_contains(content, "DRAFT")
     False
     >>> pdf_contains(content, "PAID")
     False
 
 Print paid invoice::
 
-    >>> pay = Wizard('account.invoice.pay', [invoice])
+    >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> invoice.state
     'paid'
     >>> content = invoice_report.execute([invoice])[1]
     >>> pdf_contains(content, "PAID")
     True
```

### Comparing `trytond_account_invoice_watermark-6.6.1/tests/tools.py` & `trytond_account_invoice_watermark-6.8.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/PKG-INFO` & `trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-watermark
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add watermark to invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-watermark
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_watermark
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice watermark
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
 
 ################################
 Account Invoice Watermark Module
 ################################
```

### Comparing `trytond_account_invoice_watermark-6.6.1/trytond_account_invoice_watermark.egg-info/SOURCES.txt` & `trytond_account_invoice_watermark-6.8.0/trytond_account_invoice_watermark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

