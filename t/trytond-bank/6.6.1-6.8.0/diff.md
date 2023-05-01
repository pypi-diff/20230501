# Comparing `tmp/trytond_bank-6.6.1.tar.gz` & `tmp/trytond_bank-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_bank-6.6.1.tar", last modified: Tue Dec  6 17:36:40 2022, max compression
+gzip compressed data, was "trytond_bank-6.8.0.tar", last modified: Mon May  1 11:46:18 2023, max compression
```

## Comparing `trytond_bank-6.6.1.tar` & `trytond_bank-6.8.0.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.918242 trytond_bank-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2022-12-06 17:36:39.000000 trytond_bank-6.6.1/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2094 2022-12-06 17:36:38.000000 trytond_bank-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-12-06 17:36:38.000000 trytond_bank-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2884 2022-12-06 17:36:40.918242 trytond_bank-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10271 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/bank.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5895 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/bank.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.914909 trytond_bank-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.918242 trytond_bank-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/icons/tryton-bank.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.911575 trytond_bank-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3294 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3503 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3518 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3533 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2942 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3337 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3675 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3553 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3108 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3525 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3904 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3206 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3513 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3372 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3498 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2914 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3386 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3011 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2881 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3026 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1572 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1368 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-12-06 17:36:40.918242 trytond_bank-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5111 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.914909 trytond_bank-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7283 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.918242 trytond_bank-6.6.1/trytond_bank.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2884 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-12-06 17:36:40.000000 trytond_bank-6.6.1/trytond_bank.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-12-06 17:36:40.914909 trytond_bank-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/view/bank_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/view/bank_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/view/bank_account_number_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/view/bank_account_number_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/view/bank_account_number_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/view/bank_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2022-11-30 22:27:13.000000 trytond_bank-6.6.1/view/bank_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2022-10-31 16:31:03.000000 trytond_bank-6.6.1/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.695919 trytond_bank-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2206 2023-05-01 11:04:16.000000 trytond_bank-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:04:15.000000 trytond_bank-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2887 2023-05-01 11:46:18.695919 trytond_bank-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10517 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/bank.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5895 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/bank.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.692586 trytond_bank-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.692586 trytond_bank-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/icons/tryton-bank.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.689253 trytond_bank-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3294 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3503 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3518 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3533 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2942 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3337 2023-04-30 10:46:36.000000 trytond_bank-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3675 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3553 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3108 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3525 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3904 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3206 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3513 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3372 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3498 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2914 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3386 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3011 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2881 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3026 2023-04-29 08:02:44.000000 trytond_bank-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1530 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1368 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:46:18.695919 trytond_bank-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4311 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.689253 trytond_bank-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7283 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2023-05-01 11:04:10.000000 trytond_bank-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.695919 trytond_bank-6.8.0/trytond_bank.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2887 2023-05-01 11:46:17.000000 trytond_bank-6.8.0/trytond_bank.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1822 2023-05-01 11:46:18.000000 trytond_bank-6.8.0/trytond_bank.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:46:17.000000 trytond_bank-6.8.0/trytond_bank.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2023-05-01 11:46:17.000000 trytond_bank-6.8.0/trytond_bank.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_bank-6.8.0/trytond_bank.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-05-01 11:46:17.000000 trytond_bank-6.8.0/trytond_bank.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:46:17.000000 trytond_bank-6.8.0/trytond_bank.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:18.692586 trytond_bank-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/view/bank_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/view/bank_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/view/bank_account_number_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/view/bank_account_number_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/view/bank_account_number_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/view/bank_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:15.000000 trytond_bank-6.8.0/view/bank_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:20.000000 trytond_bank-6.8.0/view/party_form.xml
```

### Comparing `trytond_bank-6.6.1/CHANGELOG` & `trytond_bank-6.8.0/CHANGELOG`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-Version 6.6.1 - 2022-12-06
+
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Deactivate numbers when account is deactivated
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_bank-6.6.1/COPYRIGHT` & `trytond_bank-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2013-2022 Cédric Krier.
-Copyright (C) 2013-2022 B2CK SPRL.
+Copyright (C) 2013-2023 Cédric Krier.
+Copyright (C) 2013-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_bank-6.6.1/LICENSE` & `trytond_bank-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/PKG-INFO` & `trytond_bank-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_bank
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with banks
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
-Project-URL: Source Code, https://hg.tryton.org/modules/bank
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton bank
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 Provides-Extra: SWIFT
 Provides-Extra: test
 License-File: LICENSE
 
 Bank Module
 ###########
```

### Comparing `trytond_bank-6.6.1/README.rst` & `trytond_bank-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/bank.py` & `trytond_bank-6.8.0/bank.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 except ImportError:
     BIC = IBAN = None
 
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Exclude, ModelSQL, ModelView, fields, sequence_ordered)
 from trytond.pool import Pool
+from trytond.pyson import Eval, If
 from trytond.tools import is_full_text, lstrip_wildcard
 
 from .exceptions import AccountValidationError, IBANValidationError, InvalidBIC
 
 
 class Bank(ModelSQL, ModelView):
     'Bank'
@@ -90,15 +91,19 @@
     __name__ = 'bank.account'
     bank = fields.Many2One(
         'bank', "Bank",
         help="The bank where the account is open.")
     owners = fields.Many2Many('bank.account-party.party', 'account', 'owner',
         'Owners')
     currency = fields.Many2One('currency.currency', 'Currency')
-    numbers = fields.One2Many('bank.account.number', 'account', 'Numbers',
+    numbers = fields.One2Many(
+        'bank.account.number', 'account', 'Numbers',
+        domain=[
+            If(~Eval('active'), ('active', '=', False), ()),
+            ],
         help="Add the numbers which identify the bank account.")
 
     def get_rec_name(self, name):
         for number in self.numbers:
             if number.number:
                 name = number.number
                 break
@@ -167,20 +172,23 @@
         Bank = pool.get('bank')
         if IBAN and self.iban:
             iban = IBAN(self.iban)
             if iban.bic:
                 return Bank.from_bic(iban.bic)
 
 
-class AccountNumber(sequence_ordered(), ModelSQL, ModelView):
+class AccountNumber(DeactivableMixin, sequence_ordered(), ModelSQL, ModelView):
     'Bank Account Number'
     __name__ = 'bank.account.number'
     _rec_name = 'number'
     account = fields.Many2One(
         'bank.account', "Account", required=True, ondelete='CASCADE',
+        domain=[
+            If(Eval('active'), ('active', '=', True), ()),
+            ],
         help="The bank account which is identified by the number.")
     type = fields.Selection([
             ('iban', 'IBAN'),
             ('other', 'Other'),
             ], 'Type', required=True)
     number = fields.Char('Number')
     number_compact = fields.Char('Number Compact', readonly=True)
```

### Comparing `trytond_bank-6.6.1/bank.xml` & `trytond_bank-6.8.0/bank.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/doc/index.rst` & `trytond_bank-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/icons/LICENSE` & `trytond_bank-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/bg.po` & `trytond_bank-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/ca.po` & `trytond_bank-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/cs.po` & `trytond_bank-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/de.po` & `trytond_bank-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/es.po` & `trytond_bank-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/es_419.po` & `trytond_bank-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/et.po` & `trytond_bank-6.8.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 msgctxt "field:bank,bic:"
 msgid "BIC"
 msgstr "BIC"
 
 msgctxt "field:bank,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:bank.account,bank:"
 msgid "Bank"
 msgstr "Pank"
 
 msgctxt "field:bank.account,currency:"
 msgid "Currency"
```

### Comparing `trytond_bank-6.6.1/locale/fa.po` & `trytond_bank-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/fi.po` & `trytond_bank-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/fr.po` & `trytond_bank-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/hu.po` & `trytond_bank-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/id.po` & `trytond_bank-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/it.po` & `trytond_bank-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/lo.po` & `trytond_bank-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/lt.po` & `trytond_bank-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/nl.po` & `trytond_bank-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/pl.po` & `trytond_bank-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/pt.po` & `trytond_bank-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/ro.po` & `trytond_bank-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/ru.po` & `trytond_bank-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/sl.po` & `trytond_bank-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/tr.po` & `trytond_bank-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/uk.po` & `trytond_bank-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/locale/zh_CN.po` & `trytond_bank-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/message.xml` & `trytond_bank-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/party.py` & `trytond_bank-6.8.0/party.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,16 @@
         return [bool_op,
             domain,
             ('bank_accounts.numbers.rec_name',) + tuple(clause[1:]),
             ]
 
     @classmethod
     def copy(cls, parties, default=None):
-        context = Transaction().context
         default = default.copy() if default else {}
-        if context.get('_check_access'):
+        if Transaction().check_access:
             default.setdefault(
                 'bank_accounts',
                 cls.default_get(
                     ['bank_accounts'],
                     with_rec_name=False).get('bank_accounts'))
         return super().copy(parties, default=default)
```

### Comparing `trytond_bank-6.6.1/party.xml` & `trytond_bank-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/setup.py` & `trytond_bank-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
 name = 'trytond_bank'
 
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
 
 requires = ['python-stdnum', 'python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = ['schwifty']
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module with banks',
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
-        "Source Code": 'https://hg.tryton.org/modules/bank',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton bank',
     package_dir={'trytond.modules.bank': '.'},
     packages=(
         ['trytond.modules.bank']
         + ['trytond.modules.bank.%s' % p for p in find_packages()]
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
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'SWIFT': ['schwifty>=2020.01.0'],
         'test': tests_require,
         },
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     bank = trytond.modules.bank
     """,
     )
```

### Comparing `trytond_bank-6.6.1/tests/test_module.py` & `trytond_bank-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_bank-6.6.1/trytond_bank.egg-info/PKG-INFO` & `trytond_bank-6.8.0/trytond_bank.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-bank
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with banks
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
-Project-URL: Source Code, https://hg.tryton.org/modules/bank
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton bank
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 Provides-Extra: SWIFT
 Provides-Extra: test
 License-File: LICENSE
 
 Bank Module
 ###########
```

### Comparing `trytond_bank-6.6.1/trytond_bank.egg-info/SOURCES.txt` & `trytond_bank-6.8.0/trytond_bank.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

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
 bank.py
@@ -56,14 +52,15 @@
 ./view/bank_account_list.xml
 ./view/bank_account_number_form.xml
 ./view/bank_account_number_list.xml
 ./view/bank_account_number_list_sequence.xml
 ./view/bank_form.xml
 ./view/bank_list.xml
 ./view/party_form.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-bank.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

### Comparing `trytond_bank-6.6.1/view/bank_account_form.xml` & `trytond_bank-6.8.0/view/bank_account_form.xml`

 * *Files identical despite different names*

