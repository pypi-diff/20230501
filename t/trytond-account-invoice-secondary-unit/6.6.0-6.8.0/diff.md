# Comparing `tmp/trytond_account_invoice_secondary_unit-6.6.0.tar.gz` & `tmp/trytond_account_invoice_secondary_unit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_secondary_unit-6.6.0.tar", last modified: Mon Oct 31 16:02:07 2022, max compression
+gzip compressed data, was "trytond_account_invoice_secondary_unit-6.8.0.tar", last modified: Mon May  1 11:54:28 2023, max compression
```

## Comparing `trytond_account_invoice_secondary_unit-6.6.0.tar` & `trytond_account_invoice_secondary_unit-6.8.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:07.582343 trytond_account_invoice_secondary_unit-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_invoice_secondary_unit-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_invoice_secondary_unit-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-10-31 16:02:05.000000 trytond_account_invoice_secondary_unit-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_invoice_secondary_unit-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      604 2022-10-31 16:02:04.000000 trytond_account_invoice_secondary_unit-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:02:04.000000 trytond_account_invoice_secondary_unit-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-10-11 23:19:17.000000 trytond_account_invoice_secondary_unit-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_invoice_secondary_unit-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2472 2022-10-31 16:02:07.582343 trytond_account_invoice_secondary_unit-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2019-10-11 23:19:17.000000 trytond_account_invoice_secondary_unit-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2021-12-11 16:59:32.000000 trytond_account_invoice_secondary_unit-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4952 2022-04-10 15:40:34.000000 trytond_account_invoice_secondary_unit-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2019-10-11 23:19:17.000000 trytond_account_invoice_secondary_unit-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:07.579010 trytond_account_invoice_secondary_unit-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2019-10-11 23:19:17.000000 trytond_account_invoice_secondary_unit-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:07.575676 trytond_account_invoice_secondary_unit-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      794 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-29 07:50:41.000000 trytond_account_invoice_secondary_unit-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:02:07.582343 trytond_account_invoice_secondary_unit-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5368 2022-10-29 07:39:10.000000 trytond_account_invoice_secondary_unit-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:07.579010 trytond_account_invoice_secondary_unit-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_invoice_secondary_unit-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2022-04-16 16:30:56.000000 trytond_account_invoice_secondary_unit-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2022-10-31 15:10:09.000000 trytond_account_invoice_secondary_unit-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2022-10-31 16:02:03.000000 trytond_account_invoice_secondary_unit-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:07.582343 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2472 2022-10-31 16:02:06.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2022-10-31 16:02:07.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:02:06.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2022-10-31 16:02:06.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-11-04 11:52:32.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2022-10-31 16:02:06.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:02:06.000000 trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:02:07.579010 trytond_account_invoice_secondary_unit-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2019-10-11 23:19:17.000000 trytond_account_invoice_secondary_unit-6.6.0/view/account_invoice_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:28.335329 trytond_account_invoice_secondary_unit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      767 2023-05-01 11:09:46.000000 trytond_account_invoice_secondary_unit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:09:46.000000 trytond_account_invoice_secondary_unit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2449 2023-05-01 11:54:28.335329 trytond_account_invoice_secondary_unit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4952 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:28.331996 trytond_account_invoice_secondary_unit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:28.331996 trytond_account_invoice_secondary_unit-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      794 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      785 2023-04-30 10:46:36.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-29 08:02:47.000000 trytond_account_invoice_secondary_unit-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:54:28.335329 trytond_account_invoice_secondary_unit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4527 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:28.331996 trytond_account_invoice_secondary_unit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-05-01 11:09:40.000000 trytond_account_invoice_secondary_unit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:28.335329 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2449 2023-05-01 11:54:27.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1468 2023-05-01 11:54:28.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:54:27.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-05-01 11:54:27.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-05-01 11:54:27.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:54:27.000000 trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:28.331996 trytond_account_invoice_secondary_unit-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_account_invoice_secondary_unit-6.8.0/view/account_invoice_line_form.xml
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/CHANGELOG` & `trytond_account_invoice_secondary_unit-6.8.0/CHANGELOG`

 * *Files 17% similar despite different names*

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

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/COPYRIGHT` & `trytond_account_invoice_secondary_unit-6.8.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2019-2022 Cédric Krier
-Copyright (C) 2019-2022 B2CK
+Copyright (C) 2019-2023 Cédric Krier
+Copyright (C) 2019-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/LICENSE` & `trytond_account_invoice_secondary_unit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/PKG-INFO` & `trytond_account_invoice_secondary_unit-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_secondary_unit
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add a secondary unit on invoice line
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_secondary_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton invoice secondary unit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,22 +37,22 @@
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
 
 Account Invoice Secondary Unit Module
 #####################################
 
 The account invoice secondary unit module adds a secondary unit of measure on
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/account.py` & `trytond_account_invoice_secondary_unit-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/bg.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/ca.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/cs.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/de.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/es.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/es_419.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/et.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/fa.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/fi.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/fr.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/hu.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/id.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/it.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/lo.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/lt.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/nl.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/pl.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/pt.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/ro.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/ro.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice.line,product_secondary_uom_category:"
 msgid "Product Secondary UOM Category"
-msgstr ""
+msgstr "Categorie Secundara UM pentru Produs"
 
 msgctxt "field:account.invoice.line,secondary_quantity:"
 msgid "Secondary Quantity"
-msgstr ""
+msgstr "Cantitate Secundara"
 
 msgctxt "field:account.invoice.line,secondary_unit:"
 msgid "Secondary Unit"
-msgstr ""
+msgstr "Unitate Secundara"
 
 msgctxt "field:account.invoice.line,secondary_unit_price:"
 msgid "Secondary Unit Price"
 msgstr "Preţ Unitate Secundara"
 
 msgctxt "view:account.invoice.line:"
 msgid "Quantity:"
-msgstr ""
+msgstr "Cantitate:"
 
 msgctxt "view:account.invoice.line:"
 msgid "Unit Price:"
 msgstr "Preţ Unitate:"
 
 msgctxt "view:account.invoice.line:"
 msgid "Unit:"
-msgstr ""
+msgstr "Unitate:"
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/ru.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/sl.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/tr.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/uk.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/locale/zh_CN.po` & `trytond_account_invoice_secondary_unit-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/setup.py` & `trytond_account_invoice_secondary_unit-6.8.0/setup.py`

 * *Files 17% similar despite different names*

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
 name = 'trytond_account_invoice_secondary_unit'
 
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
     description='Tryton module to add a secondary unit on invoice line',
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
-            'https://hg.tryton.org/modules/account_invoice_secondary_unit'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton invoice secondary unit',
     package_dir={'trytond.modules.account_invoice_secondary_unit': '.'},
     packages=(
         ['trytond.modules.account_invoice_secondary_unit']
         + ['trytond.modules.account_invoice_secondary_unit.%s' % p
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
     account_invoice_secondary_unit = trytond.modules.account_invoice_secondary_unit
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO` & `trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-secondary-unit
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add a secondary unit on invoice line
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_secondary_unit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton invoice secondary unit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,22 +37,22 @@
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
 
 Account Invoice Secondary Unit Module
 #####################################
 
 The account invoice secondary unit module adds a secondary unit of measure on
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt` & `trytond_account_invoice_secondary_unit-6.8.0/trytond_account_invoice_secondary_unit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

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
@@ -40,14 +36,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/account_invoice_line_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_invoice_secondary_unit-6.6.0/view/account_invoice_line_form.xml` & `trytond_account_invoice_secondary_unit-6.8.0/view/account_invoice_line_form.xml`

 * *Files identical despite different names*

