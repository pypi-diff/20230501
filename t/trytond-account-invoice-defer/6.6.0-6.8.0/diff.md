# Comparing `tmp/trytond_account_invoice_defer-6.6.0.tar.gz` & `tmp/trytond_account_invoice_defer-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_defer-6.6.0.tar", last modified: Mon Oct 31 16:01:20 2022, max compression
+gzip compressed data, was "trytond_account_invoice_defer-6.8.0.tar", last modified: Mon May  1 12:02:48 2023, max compression
```

## Comparing `trytond_account_invoice_defer-6.6.0.tar` & `trytond_account_invoice_defer-6.8.0.tar`

### file list

```diff
@@ -1,69 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:20.224988 trytond_account_invoice_defer-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_account_invoice_defer-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 16:01:18.000000 trytond_account_invoice_defer-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_invoice_defer-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2022-10-31 16:01:17.000000 trytond_account_invoice_defer-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:01:16.000000 trytond_account_invoice_defer-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_invoice_defer-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2507 2022-10-31 16:01:20.224988 trytond_account_invoice_defer-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2022-10-27 11:24:44.000000 trytond_account_invoice_defer-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18220 2022-10-11 19:49:57.000000 trytond_account_invoice_defer-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8380 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:20.221654 trytond_account_invoice_defer-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1844 2022-04-08 16:27:20.000000 trytond_account_invoice_defer-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2022-10-27 11:24:44.000000 trytond_account_invoice_defer-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_account_invoice_defer-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2022-04-08 16:27:20.000000 trytond_account_invoice_defer-6.6.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:20.218321 trytond_account_invoice_defer-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5844 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6074 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5849 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5961 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4801 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5896 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4777 2022-10-29 07:50:44.000000 trytond_account_invoice_defer-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1240 2022-04-08 16:23:26.000000 trytond_account_invoice_defer-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:01:20.224988 trytond_account_invoice_defer-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5436 2022-10-29 07:39:10.000000 trytond_account_invoice_defer-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:20.218321 trytond_account_invoice_defer-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_invoice_defer-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3828 2021-10-30 15:32:31.000000 trytond_account_invoice_defer-6.6.0/tests/scenario_account_invoice_defer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2022-04-16 16:30:56.000000 trytond_account_invoice_defer-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_invoice_defer-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1770 2021-10-30 15:32:31.000000 trytond_account_invoice_defer-6.6.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 15:10:09.000000 trytond_account_invoice_defer-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2022-10-31 16:01:15.000000 trytond_account_invoice_defer-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:20.224988 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2507 2022-10-31 16:01:19.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1849 2022-10-31 16:01:20.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:01:19.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:01:19.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-04-12 20:11:35.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2022-10-31 16:01:19.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:01:19.000000 trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:20.218321 trytond_account_invoice_defer-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      964 2021-10-07 13:08:06.000000 trytond_account_invoice_defer-6.6.0/view/invoice_deferred_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2021-10-07 13:08:06.000000 trytond_account_invoice_defer-6.6.0/view/invoice_deferred_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2021-04-27 07:35:27.000000 trytond_account_invoice_defer-6.6.0/view/invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-05-01 11:15:38.000000 trytond_account_invoice_defer-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 11:15:37.000000 trytond_account_invoice_defer-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18427 2023-04-29 11:01:18.000000 trytond_account_invoice_defer-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8380 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.078197 trytond_account_invoice_defer-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1844 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.071530 trytond_account_invoice_defer-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5844 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-04-30 10:46:36.000000 trytond_account_invoice_defer-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5849 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4801 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5896 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4777 2023-04-29 08:02:50.000000 trytond_account_invoice_defer-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4610 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.074864 trytond_account_invoice_defer-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/scenario_account_invoice_defer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-05-01 11:15:31.000000 trytond_account_invoice_defer-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.081531 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1811 2023-05-01 12:02:48.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:02:47.000000 trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:48.074864 trytond_account_invoice_defer-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      964 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/invoice_deferred_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/invoice_deferred_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_account_invoice_defer-6.8.0/view/invoice_line_form.xml
```

### Comparing `trytond_account_invoice_defer-6.6.0/COPYRIGHT` & `trytond_account_invoice_defer-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_invoice_defer-6.6.0/LICENSE` & `trytond_account_invoice_defer-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/PKG-INFO` & `trytond_account_invoice_defer-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_defer
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-defer
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_defer
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice defer expense revenue
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
 
 ############################
 Account Invoice Defer Module
 ############################
```

### Comparing `trytond_account_invoice_defer-6.6.0/__init__.py` & `trytond_account_invoice_defer-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/account.py` & `trytond_account_invoice_defer-6.8.0/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Unique, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.modules.account.exceptions import AccountMissing
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval, If
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 from trytond.wizard import StateTransition, Wizard
 
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'account.configuration'
 
     deferred_account_revenue = fields.MultiValue(fields.Many2One(
@@ -68,16 +68,19 @@
             })
     type = fields.Selection([
             ('out', "Customer"),
             ('in', "Supplier"),
             ], "Type", required=True,
         states=_states)
     journal = fields.Many2One(
-        'account.journal', "Journal", required=True,
-        states=_states,
+        'account.journal', "Journal",
+        states={
+            'readonly': _states['readonly'],
+            'required': Eval('state') != 'draft',
+            },
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     invoice_line = fields.Many2One(
         'account.invoice.line', "Invoice Line", required=True,
         domain=[
@@ -143,29 +146,38 @@
                 'run': {
                     'invisible': Eval('state') != 'draft',
                     'depends': ['state'],
                     },
                 })
 
     @classmethod
+    def __register__(cls, module_name):
+        table_h = cls.__table_handler__(module_name)
+        super().__register__(module_name)
+
+        # Migration from 6.6: drop not null on journal
+        table_h.not_null_action('journal', 'remove')
+
+    @classmethod
     def _journal_types(cls, type):
         if type == 'out':
             return ['revenue']
         else:
             return ['expense']
 
     @fields.depends('type')
-    def on_change_type(self):
-        Journal = self.__class__.journal.get_target()
-        journal_types = self.__class__._journal_types(self.type)
-        journals = Journal.search([
-                ('type', 'in', journal_types),
-                ], limit=1)
-        if journals:
-            self.journal, = journals
+    def on_change_with_journal(self, pattern=None):
+        pool = Pool()
+        Journal = pool.get('account.journal')
+        pattern = pattern.copy() if pattern is not None else {}
+        pattern.setdefault('type', {
+                'out': 'revenue',
+                'in': 'expense',
+                }.get(self.type))
+        return Journal.find(pattern)
 
     @fields.depends('invoice_line', 'start_date', 'company')
     def on_change_invoice_line(self):
         pool = Pool()
         Currency = pool.get('currency.currency')
         if self.invoice_line:
             if not self.start_date:
@@ -185,26 +197,25 @@
 
     @classmethod
     def default_state(cls):
         return 'draft'
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @classmethod
     @ModelView.button
     @Workflow.transition('running')
     def run(cls, deferrals):
         pool = Pool()
         Period = pool.get('account.period')
         # Ensure it starts at an opened period
         for deferral in deferrals:
-            Period.find(deferral.company.id, deferral.start_date)
+            Period.find(deferral.company, deferral.start_date)
         # Set state before create moves and defer amount to pass assert
         cls.write(deferrals, {'state': 'running'})
         cls.create_moves(deferrals)
         # defer_amount is called after create_moves to be sure that
         # create_moves call get_move with the invoice period if needed.
         cls.defer_amount(deferrals)
         cls.close_try(deferrals)
@@ -269,42 +280,39 @@
         Move.save(moves)
         to_save = []
         for deferral in deferrals:
             if deferral.moves:
                 last_move = deferral.moves[-1]
                 if last_move.period.end_date >= deferral.end_date:
                     remainder = deferral.amount_remainder
-                    if remainder > 0:
-                        for line in last_move.lines:
-                            if line.debit:
-                                line.debit += remainder
-                            else:
-                                line.credit += remainder
-                    elif remainder < 0:
+                    if remainder:
                         for line in last_move.lines:
                             if line.debit:
                                 line.debit -= remainder
                             else:
                                 line.credit -= remainder
-                    if remainder:
+                        last_move.lines = last_move.lines
                         to_save.append(last_move)
         Move.save(to_save)
         Move.post(moves)
 
     @property
     def amount_daily(self):
         days = (self.end_date - self.start_date).days + 1
         return self.amount / days
 
     @property
     def amount_remainder(self):
-        period = self.invoice_line.invoice.move.period
-        return abs(self.amount) - sum(
-            l.credit for m in self.moves for l in m.lines
-            if m.period != period)
+        balance = 0
+        for move in self.moves:
+            income_account = self.invoice_line.account.current(move.date)
+            for line in move.lines:
+                if line.account == income_account:
+                    balance += line.debit - line.credit
+        return balance
 
     def get_move(self, period=None):
         pool = Pool()
         Move = pool.get('account.move')
         Line = pool.get('account.move.line')
         Configuration = pool.get('account.configuration')
         configuration = Configuration(1)
@@ -379,15 +387,15 @@
     __name__ = 'account.invoice.deferred.create_moves'
     start_state = 'create_moves'
     create_moves = StateTransition()
 
     def transition_create_moves(self):
         pool = Pool()
         InvoiceDeferred = pool.get('account.invoice.deferred')
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             deferrals = InvoiceDeferred.search([
                     ('state', '=', 'running'),
                     ])
         deferrals = InvoiceDeferred.browse(deferrals)
         InvoiceDeferred.create_moves(deferrals)
         InvoiceDeferred.close_try(deferrals)
         return 'end'
```

### Comparing `trytond_account_invoice_defer-6.6.0/account.xml` & `trytond_account_invoice_defer-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/doc/conf.py` & `trytond_account_invoice_defer-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_invoice_defer-6.6.0/doc/design.rst` & `trytond_account_invoice_defer-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/bg.po` & `trytond_account_invoice_defer-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/ca.po` & `trytond_account_invoice_defer-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/cs.po` & `trytond_account_invoice_defer-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/de.po` & `trytond_account_invoice_defer-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_invoice_deferred_companies"
 msgid "User in companies"
 msgstr "Benutzer im Unternehmen"
 
 msgctxt "model:ir.ui.menu,name:menu_invoice_deferred_create_moves"
 msgid "Create Invoices Deferred Moves"
-msgstr "Buchungessätze für Rechnungsabgrenzung erstellen"
+msgstr "Buchungssätze für Rechnungsabgrenzung erstellen"
 
 msgctxt "model:ir.ui.menu,name:menu_invoice_deferred_in_form"
 msgid "Supplier Invoices Deferred"
 msgstr "Rechnungsabgrenzung Lieferantenrechnungen"
 
 msgctxt "model:ir.ui.menu,name:menu_invoice_deferred_out_form"
 msgid "Customer Invoices Deferred"
```

### Comparing `trytond_account_invoice_defer-6.6.0/locale/es.po` & `trytond_account_invoice_defer-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/es_419.po` & `trytond_account_invoice_defer-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/et.po` & `trytond_account_invoice_defer-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/fa.po` & `trytond_account_invoice_defer-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/fi.po` & `trytond_account_invoice_defer-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/fr.po` & `trytond_account_invoice_defer-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/hu.po` & `trytond_account_invoice_defer-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/id.po` & `trytond_account_invoice_defer-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/it.po` & `trytond_account_invoice_defer-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/lo.po` & `trytond_account_invoice_defer-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/lt.po` & `trytond_account_invoice_defer-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/nl.po` & `trytond_account_invoice_defer-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/pl.po` & `trytond_account_invoice_defer-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/pt.po` & `trytond_account_invoice_defer-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/ro.po` & `trytond_account_invoice_defer-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/ru.po` & `trytond_account_invoice_defer-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/sl.po` & `trytond_account_invoice_defer-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/tr.po` & `trytond_account_invoice_defer-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/uk.po` & `trytond_account_invoice_defer-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/locale/zh_CN.po` & `trytond_account_invoice_defer-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/message.xml` & `trytond_account_invoice_defer-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_defer-6.6.0/setup.py` & `trytond_account_invoice_defer-6.8.0/setup.py`

 * *Files 21% similar despite different names*

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
@@ -37,62 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_invoice_defer'
 
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
     description='Tryton module to defer expense and revenue',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-account-invoice-defer'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_invoice_defer',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice defer expense revenue',
     package_dir={'trytond.modules.account_invoice_defer': '.'},
     packages=(
         ['trytond.modules.account_invoice_defer']
         + ['trytond.modules.account_invoice_defer.%s' % p
             for p in find_packages()]
@@ -130,27 +107,26 @@
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
     account_invoice_defer = trytond.modules.account_invoice_defer
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_invoice_defer-6.6.0/tests/scenario_account_invoice_defer.rst` & `trytond_account_invoice_defer-6.8.0/tests/scenario_account_invoice_defer.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
     >>> from trytond.modules.account_invoice_defer.tests.tools import (
     ...     add_deferred_accounts)
 
+    >>> today = dt.date.today()
+
 Activate modules::
 
     >>> config = activate_modules('account_invoice_defer')
 
     >>> Invoice = Model.get('account.invoice')
     >>> InvoiceDeferred = Model.get('account.invoice.deferred')
     >>> Party = Model.get('party.party')
@@ -32,15 +34,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = add_deferred_accounts(get_accounts(company))
@@ -77,15 +79,15 @@
     >>> invoice.party = party
     >>> line = invoice.lines.new()
     >>> line.product = product
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('1000')
     >>> line.defer_from = period.start_date
     >>> line.defer_to = line.defer_from + dt.timedelta(days=499)
-    >>> invoice.invoice_date = dt.date.today()
+    >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> invoice_line, = invoice.lines
 
 Check invoice deferred and run it::
 
     >>> deferral, = InvoiceDeferred.find([])
     >>> deferral.invoice_line == invoice_line
```

### Comparing `trytond_account_invoice_defer-6.6.0/tests/tools.py` & `trytond_account_invoice_defer-6.8.0/tests/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model
 from proteus.config import get_config
-
 from trytond.modules.company.tests.tools import get_company
 
 
 def add_deferred_accounts(accounts, company=None, config=None):
     "Add deferred to accounts"
     if not config:
         config = get_config()
```

### Comparing `trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/PKG-INFO` & `trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-defer
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to defer expense and revenue
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-defer
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_defer
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice defer expense revenue
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
 
 ############################
 Account Invoice Defer Module
 ############################
```

### Comparing `trytond_account_invoice_defer-6.6.0/trytond_account_invoice_defer.egg-info/SOURCES.txt` & `trytond_account_invoice_defer-6.8.0/trytond_account_invoice_defer.egg-info/SOURCES.txt`

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
```

### Comparing `trytond_account_invoice_defer-6.6.0/view/invoice_deferred_form.xml` & `trytond_account_invoice_defer-6.8.0/view/invoice_deferred_form.xml`

 * *Files identical despite different names*

