# Comparing `tmp/trytond_analytic_invoice-6.6.0.tar.gz` & `tmp/trytond_analytic_invoice-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_invoice-6.6.0.tar", last modified: Mon Oct 31 16:14:24 2022, max compression
+gzip compressed data, was "trytond_analytic_invoice-6.8.0.tar", last modified: Mon May  1 11:59:59 2023, max compression
```

## Comparing `trytond_analytic_invoice-6.6.0.tar` & `trytond_analytic_invoice-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:24.926397 trytond_analytic_invoice-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_analytic_invoice-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_analytic_invoice-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 16:14:23.000000 trytond_analytic_invoice-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_analytic_invoice-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2431 2022-10-31 16:14:22.000000 trytond_analytic_invoice-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 16:14:22.000000 trytond_analytic_invoice-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:25.000000 trytond_analytic_invoice-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_analytic_invoice-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2022-10-31 16:14:24.926397 trytond_analytic_invoice-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2019-06-04 16:49:44.000000 trytond_analytic_invoice-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2021-12-11 16:59:32.000000 trytond_analytic_invoice-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2320 2022-04-10 15:40:35.000000 trytond_analytic_invoice-6.6.0/asset.py
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2018-08-18 09:54:25.000000 trytond_analytic_invoice-6.6.0/asset.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:24.923064 trytond_analytic_invoice-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2019-06-04 16:49:44.000000 trytond_analytic_invoice-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3629 2022-04-11 20:29:38.000000 trytond_analytic_invoice-6.6.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2018-08-18 09:54:25.000000 trytond_analytic_invoice-6.6.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:24.919730 trytond_analytic_invoice-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      595 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      600 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      648 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      595 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-10-29 07:50:43.000000 trytond_analytic_invoice-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:14:24.926397 trytond_analytic_invoice-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5309 2022-10-29 07:39:10.000000 trytond_analytic_invoice-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:24.923064 trytond_analytic_invoice-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_analytic_invoice-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3940 2020-07-09 09:37:02.000000 trytond_analytic_invoice-6.6.0/tests/scenario_analytic_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4642 2021-04-27 07:34:40.000000 trytond_analytic_invoice-6.6.0/tests/scenario_analytic_invoice_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2022-04-16 16:30:56.000000 trytond_analytic_invoice-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_analytic_invoice-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2022-10-31 15:10:09.000000 trytond_analytic_invoice-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 16:14:21.000000 trytond_analytic_invoice-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:24.926397 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2022-10-31 16:14:24.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1672 2022-10-31 16:14:24.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:14:24.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 16:14:24.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:10.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2022-10-31 16:14:24.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:14:24.000000 trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:24.923064 trytond_analytic_invoice-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2018-08-18 09:54:25.000000 trytond_analytic_invoice-6.6.0/view/asset_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2019-06-04 16:49:44.000000 trytond_analytic_invoice-6.6.0/view/invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:59.712775 trytond_analytic_invoice-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2594 2023-05-01 11:13:35.000000 trytond_analytic_invoice-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:13:35.000000 trytond_analytic_invoice-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_invoice-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-05-01 11:59:59.712775 trytond_analytic_invoice-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      616 2023-04-21 08:36:08.000000 trytond_analytic_invoice-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2565 2023-04-21 08:36:08.000000 trytond_analytic_invoice-6.8.0/asset.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-01-16 14:00:20.000000 trytond_analytic_invoice-6.8.0/asset.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:59.709441 trytond_analytic_invoice-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3559 2023-04-21 08:36:08.000000 trytond_analytic_invoice-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_analytic_invoice-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:59.706108 trytond_analytic_invoice-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-30 10:46:36.000000 trytond_analytic_invoice-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      595 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      600 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      648 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      595 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-29 08:02:49.000000 trytond_analytic_invoice-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:59:59.712775 trytond_analytic_invoice-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4497 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:59.709441 trytond_analytic_invoice-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3822 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/tests/scenario_analytic_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5113 2023-04-21 08:36:08.000000 trytond_analytic_invoice-6.8.0/tests/scenario_analytic_invoice_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_analytic_invoice-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 11:13:30.000000 trytond_analytic_invoice-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:59.712775 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-05-01 11:59:58.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1646 2023-05-01 11:59:59.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:59:58.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 11:59:58.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-05-01 11:59:58.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:59:58.000000 trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:59.709441 trytond_analytic_invoice-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:20.000000 trytond_analytic_invoice-6.8.0/view/asset_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_analytic_invoice-6.8.0/view/invoice_line_form.xml
```

### Comparing `trytond_analytic_invoice-6.6.0/CHANGELOG` & `trytond_analytic_invoice-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

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

### Comparing `trytond_analytic_invoice-6.6.0/COPYRIGHT` & `trytond_analytic_invoice-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2012 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_analytic_invoice-6.6.0/LICENSE` & `trytond_analytic_invoice-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/PKG-INFO` & `trytond_analytic_invoice-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_invoice
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add analytic accounting on invoice
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
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_invoice
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account invoice
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
 
 Analytic Invoice Module
 #######################
 
 The analytic invoice modules allows to set analytic accounts on invoice line.
```

### Comparing `trytond_analytic_invoice-6.6.0/asset.py` & `trytond_analytic_invoice-6.8.0/asset.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,7 +53,16 @@
                     if line.account != account:
                         continue
                     analytic_lines = []
                     for entry in self.analytic_accounts:
                         analytic_lines.extend(
                             entry.get_analytic_lines(line, move.date))
                     line.analytic_lines = analytic_lines
+
+
+class UpdateAsset(metaclass=PoolMeta):
+    __name__ = 'account.asset.update'
+
+    def get_move(self, asset):
+        move = super().get_move(asset)
+        asset.set_analytic_lines(move, self.show_move.counterpart_account)
+        return move
```

### Comparing `trytond_analytic_invoice-6.6.0/invoice.py` & `trytond_analytic_invoice-6.8.0/invoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,19 +72,18 @@
     def on_change_with_company(self, name=None):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
         try:
             Asset = pool.get('account.asset')
         except KeyError:
             Asset = None
-        company = super(AnalyticAccountEntry, self).on_change_with_company(
-            name)
+        company = super().on_change_with_company(name=name)
         if (isinstance(self.origin, InvoiceLine)
                 or (Asset and isinstance(self.origin, Asset))):
-            company = self.origin.company.id if self.origin.company else None
+            company = self.origin.company
         return company
 
     @classmethod
     def search_company(cls, name, clause):
         pool = Pool()
         domain = super(AnalyticAccountEntry, cls).search_company(name, clause),
         domain = ['OR',
```

### Comparing `trytond_analytic_invoice-6.6.0/locale/bg.po` & `trytond_analytic_invoice-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/ca.po` & `trytond_analytic_invoice-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/de.po` & `trytond_analytic_invoice-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/es.po` & `trytond_analytic_invoice-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/et.po` & `trytond_analytic_invoice-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/fa.po` & `trytond_analytic_invoice-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/fr.po` & `trytond_analytic_invoice-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/it.po` & `trytond_analytic_invoice-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/lo.po` & `trytond_analytic_invoice-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/nl.po` & `trytond_analytic_invoice-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/pt.po` & `trytond_analytic_invoice-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/ro.po` & `trytond_analytic_invoice-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/ru.po` & `trytond_analytic_invoice-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/locale/sl.po` & `trytond_analytic_invoice-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_analytic_invoice-6.6.0/setup.py` & `trytond_analytic_invoice-6.8.0/setup.py`

 * *Files 14% similar despite different names*

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
@@ -34,62 +31,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_analytic_invoice'
 
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
 
 tests_require = [get_require_version('proteus')]
 for dep in ['account_asset']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add analytic accounting on invoice',
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
-        "Source Code": 'https://hg.tryton.org/modules/analytic_invoice',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton analytic account invoice',
     package_dir={'trytond.modules.analytic_invoice': '.'},
     packages=(
         ['trytond.modules.analytic_invoice']
         + ['trytond.modules.analytic_invoice.%s' % p for p in find_packages()]
         ),
@@ -125,28 +103,27 @@
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
     analytic_invoice = trytond.modules.analytic_invoice
     """,
     )
```

### Comparing `trytond_analytic_invoice-6.6.0/tests/scenario_analytic_invoice.rst` & `trytond_analytic_invoice-6.8.0/tests/scenario_analytic_invoice.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 =========================
 Analytic Invoice Scenario
 =========================
 
 Imports::
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('analytic_invoice')
 
 Create company::
```

### Comparing `trytond_analytic_invoice-6.6.0/tests/scenario_analytic_invoice_asset.rst` & `trytond_analytic_invoice-6.8.0/tests/scenario_analytic_invoice_asset.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 =====================================
 Analytic Invoice with Assets Scenario
 =====================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.account_asset.tests.tools \
     ...     import add_asset_accounts
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
+    >>> next_month = today + relativedelta(day=1, month=1)
+    >>> next_next_month = next_month + relativedelta(months=1)
 
 Activate modules::
 
     >>> config = activate_modules(['analytic_invoice', 'account_asset'])
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, (today, next_next_month)))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_asset_accounts(get_accounts(company), company)
     >>> revenue = accounts['revenue']
@@ -94,15 +97,15 @@
     >>> supplier_invoice.party = supplier
     >>> invoice_line = supplier_invoice.lines.new()
     >>> invoice_line.product = asset_product
     >>> invoice_line.quantity = 1
     >>> invoice_line.unit_price = Decimal('1000')
     >>> entry, = invoice_line.analytic_accounts
     >>> entry.account = analytic_account
-    >>> supplier_invoice.invoice_date = today + relativedelta(day=1, month=1)
+    >>> supplier_invoice.invoice_date = next_month
     >>> supplier_invoice.click('post')
     >>> supplier_invoice.state
     'posted'
     >>> invoice_line, = supplier_invoice.lines
     >>> analytic_account.debit
     Decimal('0.00')
     >>> analytic_account.credit
@@ -117,24 +120,36 @@
     >>> asset.residual_value = Decimal(0)
     >>> asset.click('create_lines')
     >>> asset.click('run')
 
 Create Moves for 1 month::
 
     >>> create_moves = Wizard('account.asset.create_moves')
-    >>> create_moves.form.date = (supplier_invoice.invoice_date
-    ...     + relativedelta(months=1))
+    >>> create_moves.form.date = next_next_month
     >>> create_moves.execute('create_moves')
     >>> analytic_account.reload()
     >>> analytic_account.debit
     Decimal('100.00')
     >>> analytic_account.credit
     Decimal('0.00')
 
+Update the asset::
+
+    >>> update = Wizard('account.asset.update', [asset])
+    >>> update.form.value = Decimal('950.00')
+    >>> update.execute('update_asset')
+    >>> update.form.date = update.form.next_depreciation_date
+    >>> update.execute('create_move')
+    >>> analytic_account.reload()
+    >>> analytic_account.debit
+    Decimal('150.00')
+    >>> analytic_account.credit
+    Decimal('0.00')
+
 Close the asset::
 
     >>> asset.click('close')
     >>> analytic_account.reload()
     >>> analytic_account.debit
     Decimal('1000.00')
     >>> analytic_account.credit
-    Decimal('0.00')
+    Decimal('0.00')
```

### Comparing `trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/PKG-INFO` & `trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-analytic-invoice
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add analytic accounting on invoice
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
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_invoice
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account invoice
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
 
 Analytic Invoice Module
 #######################
 
 The analytic invoice modules allows to set analytic accounts on invoice line.
```

### Comparing `trytond_analytic_invoice-6.6.0/trytond_analytic_invoice.egg-info/SOURCES.txt` & `trytond_analytic_invoice-6.8.0/trytond_analytic_invoice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
 asset.py
@@ -48,14 +44,15 @@
 ./tests/__init__.py
 ./tests/scenario_analytic_invoice.rst
 ./tests/scenario_analytic_invoice_asset.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/asset_form.xml
 ./view/invoice_line_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

