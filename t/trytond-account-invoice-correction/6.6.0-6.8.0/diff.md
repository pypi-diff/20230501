# Comparing `tmp/trytond_account_invoice_correction-6.6.0.tar.gz` & `tmp/trytond_account_invoice_correction-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_correction-6.6.0.tar", last modified: Mon Oct 31 16:01:02 2022, max compression
+gzip compressed data, was "trytond_account_invoice_correction-6.8.0.tar", last modified: Mon May  1 11:38:46 2023, max compression
```

## Comparing `trytond_account_invoice_correction-6.6.0.tar` & `trytond_account_invoice_correction-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:02.528064 trytond_account_invoice_correction-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_invoice_correction-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_invoice_correction-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2022-10-31 16:01:00.000000 trytond_account_invoice_correction-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_invoice_correction-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1079 2022-10-31 16:00:59.000000 trytond_account_invoice_correction-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2022-10-31 16:00:59.000000 trytond_account_invoice_correction-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:27.000000 trytond_account_invoice_correction-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_invoice_correction-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2631 2022-10-31 16:01:02.528064 trytond_account_invoice_correction-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2019-02-13 10:09:27.000000 trytond_account_invoice_correction-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2021-12-11 16:59:32.000000 trytond_account_invoice_correction-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:02.521397 trytond_account_invoice_correction-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2019-02-13 10:09:27.000000 trytond_account_invoice_correction-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2776 2022-04-10 15:40:34.000000 trytond_account_invoice_correction-6.6.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2019-06-04 16:49:44.000000 trytond_account_invoice_correction-6.6.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:02.521397 trytond_account_invoice_correction-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      858 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      877 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      908 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      864 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      849 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      896 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      795 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      855 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      865 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      782 2022-10-29 07:50:33.000000 trytond_account_invoice_correction-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:01:02.528064 trytond_account_invoice_correction-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5295 2022-10-29 07:39:10.000000 trytond_account_invoice_correction-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:02.521397 trytond_account_invoice_correction-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_invoice_correction-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2116 2020-07-09 09:36:53.000000 trytond_account_invoice_correction-6.6.0/tests/scenario_invoice_correction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2022-04-16 16:30:56.000000 trytond_account_invoice_correction-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_invoice_correction-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2022-10-31 15:10:09.000000 trytond_account_invoice_correction-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:00:58.000000 trytond_account_invoice_correction-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:02.528064 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2631 2022-10-31 16:01:01.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1634 2022-10-31 16:01:02.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:01:01.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-31 16:01:01.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:50.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2022-10-31 16:01:01.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:01:01.000000 trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:01:02.521397 trytond_account_invoice_correction-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2020-07-08 22:22:00.000000 trytond_account_invoice_correction-6.6.0/view/correct_start_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2019-06-04 16:49:44.000000 trytond_account_invoice_correction-6.6.0/view/invoice_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:46.510308 trytond_account_invoice_correction-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1242 2023-05-01 10:59:18.000000 trytond_account_invoice_correction-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-05-01 10:59:18.000000 trytond_account_invoice_correction-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2612 2023-05-01 11:38:46.510308 trytond_account_invoice_correction-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:46.506975 trytond_account_invoice_correction-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2776 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:46.503641 trytond_account_invoice_correction-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      858 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      877 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      752 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      908 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      864 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      849 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      896 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      795 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      855 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      846 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      865 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      752 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      782 2023-04-29 08:02:40.000000 trytond_account_invoice_correction-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:38:46.510308 trytond_account_invoice_correction-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4458 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:46.503641 trytond_account_invoice_correction-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2096 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/tests/scenario_invoice_correction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 10:59:12.000000 trytond_account_invoice_correction-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:46.510308 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2612 2023-05-01 11:38:45.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-05-01 11:38:46.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:38:45.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 11:38:45.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:38:45.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:38:45.000000 trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:46.506975 trytond_account_invoice_correction-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_account_invoice_correction-6.8.0/view/correct_start_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-01-16 14:00:20.000000 trytond_account_invoice_correction-6.8.0/view/invoice_form.xml
```

### Comparing `trytond_account_invoice_correction-6.6.0/CHANGELOG` & `trytond_account_invoice_correction-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_invoice_correction-6.6.0/COPYRIGHT` & `trytond_account_invoice_correction-6.8.0/COPYRIGHT`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2014-2022 Nicolas Évrard.
-Copyright (C) 2014-2022 B2CK SPRL.
-Copyright (C) 2016-2022 Cédric Krier
+Copyright (C) 2014-2023 Nicolas Évrard.
+Copyright (C) 2014-2023 B2CK SPRL.
+Copyright (C) 2016-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_correction-6.6.0/LICENSE` & `trytond_account_invoice_correction-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/PKG-INFO` & `trytond_account_invoice_correction-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_correction
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to correct invoice
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_correction
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton invoice correction
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
 
 Account Invoice Correction Module
 #################################
 
 The account invoice correction module adds a wizard on invoice which allows
```

### Comparing `trytond_account_invoice_correction-6.6.0/invoice.py` & `trytond_account_invoice_correction-6.8.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/invoice.xml` & `trytond_account_invoice_correction-6.8.0/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/bg.po` & `trytond_account_invoice_correction-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/ca.po` & `trytond_account_invoice_correction-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/cs.po` & `trytond_account_invoice_correction-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/de.po` & `trytond_account_invoice_correction-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/es.po` & `trytond_account_invoice_correction-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/es_419.po` & `trytond_account_invoice_correction-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/et.po` & `trytond_account_invoice_correction-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/fa.po` & `trytond_account_invoice_correction-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/fi.po` & `trytond_account_invoice_correction-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/fr.po` & `trytond_account_invoice_correction-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/hu.po` & `trytond_account_invoice_correction-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/id.po` & `trytond_account_invoice_correction-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/it.po` & `trytond_account_invoice_correction-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/lo.po` & `trytond_account_invoice_correction-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/lt.po` & `trytond_account_invoice_correction-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/nl.po` & `trytond_account_invoice_correction-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/pl.po` & `trytond_account_invoice_correction-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/pt.po` & `trytond_account_invoice_correction-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/ro.po` & `trytond_account_invoice_correction-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/ru.po` & `trytond_account_invoice_correction-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/sl.po` & `trytond_account_invoice_correction-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/tr.po` & `trytond_account_invoice_correction-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/uk.po` & `trytond_account_invoice_correction-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/locale/zh_CN.po` & `trytond_account_invoice_correction-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_correction-6.6.0/setup.py` & `trytond_account_invoice_correction-6.8.0/setup.py`

 * *Files 24% similar despite different names*

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
@@ -34,61 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_invoice_correction'
 
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
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to correct invoice',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_invoice_correction'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton invoice correction',
     package_dir={'trytond.modules.account_invoice_correction': '.'},
     packages=(
         ['trytond.modules.account_invoice_correction']
         + ['trytond.modules.account_invoice_correction.%s' % p
             for p in find_packages()]
@@ -125,28 +102,27 @@
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
     account_invoice_correction = trytond.modules.account_invoice_correction
     """,
     )
```

### Comparing `trytond_account_invoice_correction-6.6.0/tests/scenario_invoice_correction.rst` & `trytond_account_invoice_correction-6.8.0/tests/scenario_invoice_correction.rst`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     >>> line.unit_price = Decimal('40')
     >>> invoice.click('post')
     >>> invoice.state
     'posted'
 
 Correct invoice::
 
-    >>> correct = Wizard('account.invoice.correct', [invoice])
+    >>> correct = invoice.click('correct')
     >>> correct.form.lines.extend(correct.form.lines.find(
     ...         [('description', '=', "Revenue 1")]))
     >>> correct.execute('correct')
     >>> invoices, = correct.actions
     >>> invoice, = invoices
     >>> [(l.quantity, l.unit_price) for l in invoice.lines]
     [(-5.0, Decimal('30')), (5.0, Decimal('30'))]
```

### Comparing `trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/PKG-INFO` & `trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-correction
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to correct invoice
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_correction
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton invoice correction
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
 
 Account Invoice Correction Module
 #################################
 
 The account invoice correction module adds a wizard on invoice which allows
```

### Comparing `trytond_account_invoice_correction-6.6.0/trytond_account_invoice_correction.egg-info/SOURCES.txt` & `trytond_account_invoice_correction-6.8.0/trytond_account_invoice_correction.egg-info/SOURCES.txt`

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
 invoice.py
@@ -43,14 +39,15 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_invoice_correction.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/correct_start_view_form.xml
 ./view/invoice_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

