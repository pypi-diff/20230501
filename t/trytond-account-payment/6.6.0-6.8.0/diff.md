# Comparing `tmp/trytond_account_payment-6.6.0.tar.gz` & `tmp/trytond_account_payment-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment-6.6.0.tar", last modified: Mon Oct 31 16:04:49 2022, max compression
+gzip compressed data, was "trytond_account_payment-6.8.0.tar", last modified: Mon May  1 12:03:28 2023, max compression
```

## Comparing `trytond_account_payment-6.6.0.tar` & `trytond_account_payment-6.8.0.tar`

### file list

```diff
@@ -1,90 +1,88 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.418029 trytond_account_payment-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_payment-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_payment-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2022-10-31 16:04:48.000000 trytond_account_payment-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_payment-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2702 2022-10-31 16:04:47.000000 trytond_account_payment-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:04:46.000000 trytond_account_payment-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:14.000000 trytond_account_payment-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_payment-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3666 2022-10-31 16:04:49.414696 trytond_account_payment-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2022-04-11 18:44:50.000000 trytond_account_payment-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1302 2022-04-08 16:24:27.000000 trytond_account_payment-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22805 2022-06-21 08:27:53.000000 trytond_account_payment-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7883 2022-04-11 20:24:07.000000 trytond_account_payment-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.414696 trytond_account_payment-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2022-04-11 18:44:50.000000 trytond_account_payment-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2019-06-04 16:49:44.000000 trytond_account_payment-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.414696 trytond_account_payment-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:30.000000 trytond_account_payment-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2020-04-26 13:06:29.000000 trytond_account_payment-6.6.0/icons/tryton-payment.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.411363 trytond_account_payment-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    17359 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17487 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15773 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17807 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17399 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15231 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16968 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18151 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15760 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17735 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16231 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15991 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16366 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19432 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16932 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17517 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16085 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16892 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14958 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17330 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16897 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15760 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14585 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16006 2022-10-29 07:50:44.000000 trytond_account_payment-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2019-10-11 23:09:47.000000 trytond_account_payment-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5715 2022-10-11 19:49:57.000000 trytond_account_payment-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2548 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23466 2022-10-11 19:49:57.000000 trytond_account_payment-6.6.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23762 2022-04-11 21:35:58.000000 trytond_account_payment-6.6.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:04:49.418029 trytond_account_payment-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5391 2022-10-29 07:39:10.000000 trytond_account_payment-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.411363 trytond_account_payment-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_payment-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5512 2022-04-11 20:24:07.000000 trytond_account_payment-6.6.0/tests/scenario_account_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3084 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/tests/scenario_account_payment_direct_debit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3496 2022-04-11 18:44:50.000000 trytond_account_payment-6.6.0/tests/scenario_account_payment_dunning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4120 2022-04-11 18:44:50.000000 trytond_account_payment-6.6.0/tests/scenario_account_payment_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2555 2022-04-11 20:24:07.000000 trytond_account_payment-6.6.0/tests/scenario_account_payment_planning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2022-04-16 16:30:56.000000 trytond_account_payment-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_payment-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_account_payment-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2022-10-31 16:04:46.000000 trytond_account_payment-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.414696 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3666 2022-10-31 16:04:48.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3149 2022-10-31 16:04:49.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:04:48.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 16:04:48.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:14.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2022-10-31 16:04:48.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:04:48.000000 trytond_account_payment-6.6.0/trytond_account_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:04:49.414696 trytond_account_payment-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2018-08-18 09:54:14.000000 trytond_account_payment-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2018-08-18 09:54:14.000000 trytond_account_payment-6.6.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/view/move_line_create_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2018-08-18 09:54:14.000000 trytond_account_payment-6.6.0/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      789 2022-04-08 16:23:26.000000 trytond_account_payment-6.6.0/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-04-11 17:36:02.000000 trytond_account_payment-6.6.0/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2018-08-18 09:54:14.000000 trytond_account_payment-6.6.0/view/move_line_pay_ask_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2019-06-04 16:49:44.000000 trytond_account_payment-6.6.0/view/move_line_pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/view/party_reception_direct_debit_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1770 2022-04-11 18:44:50.000000 trytond_account_payment-6.6.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2021-10-30 15:32:31.000000 trytond_account_payment-6.6.0/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2022-04-08 16:23:26.000000 trytond_account_payment-6.6.0/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2020-09-12 16:32:24.000000 trytond_account_payment-6.6.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2022-06-21 08:25:49.000000 trytond_account_payment-6.6.0/view/payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      543 2022-04-11 18:44:50.000000 trytond_account_payment-6.6.0/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2020-07-08 22:22:00.000000 trytond_account_payment-6.6.0/view/payment_process_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.928704 trytond_account_payment-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-05-01 11:16:06.000000 trytond_account_payment-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:16:05.000000 trytond_account_payment-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3662 2023-05-01 12:03:28.925371 trytond_account_payment-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1392 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1302 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22832 2023-04-21 08:36:08.000000 trytond_account_payment-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7883 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.922037 trytond_account_payment-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1392 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.922037 trytond_account_payment-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/icons/tryton-payment.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.915371 trytond_account_payment-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17611 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17723 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16037 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18067 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17642 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15462 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17228 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18413 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16024 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17978 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16499 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16237 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16613 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19657 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17190 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17767 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16349 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17135 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15203 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17581 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17146 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16024 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14816 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16273 2023-04-30 10:46:36.000000 trytond_account_payment-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5703 2023-04-21 08:36:08.000000 trytond_account_payment-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2548 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    23454 2023-04-21 08:36:08.000000 trytond_account_payment-6.8.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24489 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:03:28.928704 trytond_account_payment-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4580 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.918704 trytond_account_payment-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5549 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/scenario_account_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2598 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/scenario_account_payment_blocked_direct_debit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3132 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/scenario_account_payment_direct_debit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3503 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/scenario_account_payment_dunning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4120 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/scenario_account_payment_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/scenario_account_payment_planning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 11:16:00.000000 trytond_account_payment-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.925371 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3662 2023-05-01 12:03:28.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3237 2023-05-01 12:03:28.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:03:28.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 12:03:28.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-05-01 12:03:28.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:03:28.000000 trytond_account_payment-6.8.0/trytond_account_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:28.922037 trytond_account_payment-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_payment-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_account_payment-6.8.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/move_line_create_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-21 08:36:08.000000 trytond_account_payment-6.8.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      789 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_account_payment-6.8.0/view/move_line_pay_ask_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/move_line_pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/party_reception_direct_debit_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1770 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_account_payment-6.8.0/view/payment_process_start_form.xml
```

### Comparing `trytond_account_payment-6.6.0/CHANGELOG` & `trytond_account_payment-6.8.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Skip blocked payments when creating direct debits
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add identical party from payments
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_payment-6.6.0/COPYRIGHT` & `trytond_account_payment-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_payment-6.6.0/LICENSE` & `trytond_account_payment-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/PKG-INFO` & `trytond_account_payment-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment
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
 
 Account Payment Module
 ######################
 
 The account_payment module allows to generate grouped payments for receivable
@@ -72,19 +72,20 @@
 - Party.
 - Line.
 - Amount.
 - Date.
 - Description.
 
 A payment can be created from an payable or receivable *Account Move Line*
-using the `Pay Lines` action. The amount is computed from the debit/credit
+using the ``Pay Lines`` action. The amount is computed from the debit/credit
 deducing existing payments for this line.
 
-Direct debit payments can be created from the wizard `Create Direct Debit` for
-all the parties that are configured with at least one *Direct Debits* record.
+Direct debit payments can be created from the wizard ``Create Direct Debit``
+for all the parties that are configured with at least one *Direct Debits*
+record.
 
 The payment can be in one of this states:
 
 * Draft
 
   The payment is in preparation.
```

### Comparing `trytond_account_payment-6.6.0/README.rst` & `trytond_account_payment-6.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 - Party.
 - Line.
 - Amount.
 - Date.
 - Description.
 
 A payment can be created from an payable or receivable *Account Move Line*
-using the `Pay Lines` action. The amount is computed from the debit/credit
+using the ``Pay Lines`` action. The amount is computed from the debit/credit
 deducing existing payments for this line.
 
-Direct debit payments can be created from the wizard `Create Direct Debit` for
-all the parties that are configured with at least one *Direct Debits* record.
+Direct debit payments can be created from the wizard ``Create Direct Debit``
+for all the parties that are configured with at least one *Direct Debits*
+record.
 
 The payment can be in one of this states:
 
 * Draft
 
   The payment is in preparation.
```

### Comparing `trytond_account_payment-6.6.0/__init__.py` & `trytond_account_payment-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/account.py` & `trytond_account_payment-6.8.0/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from trytond.i18n import gettext
 from trytond.model import ModelSQL, ModelView, fields
 from trytond.modules.company.model import CompanyValueMixin
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, Id, If
 from trytond.tools.multivalue import migrate_property
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import BlockedWarning, GroupWarning
 from .payment import KINDS
 
 
 class MoveLine(metaclass=PoolMeta):
     __name__ = 'account.move.line'
     payment_amount = fields.Function(Monetary(
-            "Payment Amount",
+            "Amount to Pay",
             currency='payment_currency', digits='payment_currency',
             states={
                 'invisible': ~Eval('payment_kind'),
                 }),
         'get_payment_amount', searcher='search_payment_amount')
     payment_currency = fields.Function(fields.Many2One(
             'currency.currency', "Payment Currency"),
@@ -196,25 +196,26 @@
             ('payment_amount', '!=', 0),
             ('move_state', '=', 'posted'),
             ['OR',
                 ('debit', '>', 0),
                 ('credit', '<', 0),
                 ],
             ('maturity_date', '<=', date),
+            ('payment_blocked', '!=', True),
             ]
 
     @classmethod
     def pay_direct_debit(cls, date=None):
         pool = Pool()
         Date = pool.get('ir.date')
         Payment = pool.get('account.payment')
         Reception = pool.get('party.party.reception_direct_debit')
         if date is None:
             date = Date.today()
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             lines = cls.search(cls._pay_direct_debit_domain(date))
 
         payments = []
         for line in lines:
             if not line.payment_amount:
                 # SQLite fails to search for payment_amount != 0
                 continue
```

### Comparing `trytond_account_payment-6.6.0/account.xml` & `trytond_account_payment-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/doc/index.rst` & `trytond_account_payment-6.8.0/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 - Party.
 - Line.
 - Amount.
 - Date.
 - Description.
 
 A payment can be created from an payable or receivable *Account Move Line*
-using the `Pay Lines` action. The amount is computed from the debit/credit
+using the ``Pay Lines`` action. The amount is computed from the debit/credit
 deducing existing payments for this line.
 
-Direct debit payments can be created from the wizard `Create Direct Debit` for
-all the parties that are configured with at least one *Direct Debits* record.
+Direct debit payments can be created from the wizard ``Create Direct Debit``
+for all the parties that are configured with at least one *Direct Debits*
+record.
 
 The payment can be in one of this states:
 
 * Draft
 
   The payment is in preparation.
```

### Comparing `trytond_account_payment-6.6.0/icons/LICENSE` & `trytond_account_payment-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/locale/bg.po` & `trytond_account_payment-6.8.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Платена сума"
+msgid "Amount to Pay"
+msgstr "Редове за плащане"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -466,14 +466,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Обработване"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/ca.po` & `trytond_account_payment-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 msgstr "Seqüència de grups de pagament"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Domiciliació Bancària"
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Import del pagament"
+msgid "Amount to Pay"
+msgstr "Import a pagar"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Bloquejat"
 
 msgctxt "field:account.move.line,payment_currency:"
 msgid "Payment Currency"
@@ -403,14 +403,24 @@
 msgstr "A aprovar"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "A processar"
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Tot"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr "Pendent"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "No podeu eliminar el tercer \"%(party)s\" mentre tingui pagaments pendents "
 "amb l'empresa \"%(company)s\"."
```

### Comparing `trytond_account_payment-6.6.0/locale/cs.po` & `trytond_account_payment-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -195,18 +196,17 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.payment.journal,currency:"
 msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.payment.journal,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:account.payment.journal,process_method:"
 msgid "Process Method"
 msgstr ""
 
 msgctxt "field:party.party,payment_direct_debit:"
 msgid "Direct Debit"
@@ -428,14 +428,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processing"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/de.po` & `trytond_account_payment-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 msgstr "Nummernkreis Zahlungslauf"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Lastschrifteinzug"
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Betrag"
+msgid "Amount to Pay"
+msgstr "Zahlbarer Betrag"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Gesperrt"
 
 msgctxt "field:account.move.line,payment_currency:"
 msgid "Payment Currency"
@@ -406,14 +406,24 @@
 msgstr "Zu Genehmigen"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Auszuführen"
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Alle"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr "Ausstehend"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "Partei \"%(party)s\" kann nicht gelöscht werden, solange noch Zahlungen bei "
 "Unternehmen \"%(company)s\" ausstehen."
@@ -460,15 +470,15 @@
 
 msgctxt "model:ir.model.button,string:payment_draft_button"
 msgid "Draft"
 msgstr "Entwurf"
 
 msgctxt "model:ir.model.button,string:payment_fail_button"
 msgid "Fail"
-msgstr "Erfolglos markieren"
+msgstr "Fehlgeschlagen markieren"
 
 msgctxt "model:ir.model.button,string:payment_group_succeed_button"
 msgid "Succeed"
 msgstr "Erfolgreich markieren"
 
 msgctxt "model:ir.model.button,string:payment_proceed_button"
 msgid "Processing"
```

### Comparing `trytond_account_payment-6.6.0/locale/es.po` & `trytond_account_payment-6.8.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 msgstr "Secuencia de grupos de pago"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Domiciliación bancaria"
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Importe del pago"
+msgid "Amount to Pay"
+msgstr "Importe a pagar"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Bloqueado"
 
 msgctxt "field:account.move.line,payment_currency:"
 msgid "Payment Currency"
@@ -403,14 +403,24 @@
 msgstr "A aprobar"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "A procesar"
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Todo"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr "Pendiente"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "No puede eliminar el tercero \"%(party)s\" mientras tenga pagos pendientes "
 "con la empresa \"%(company)s\"."
```

### Comparing `trytond_account_payment-6.6.0/locale/es_419.po` & `trytond_account_payment-6.8.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
+msgid "Amount to Pay"
 msgstr ""
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
@@ -413,14 +413,24 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr ""
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/et.po` & `trytond_account_payment-6.8.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr "Maksegrupi jada"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Otsene deebet"
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Tasumise väärtus"
+msgid "Amount to Pay"
+msgstr "Tasumisele kuuluvad read"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Blokeeritud"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -426,14 +427,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Protsessi"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Kõik"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "Osapoolt \"%(osapooli)\" ei saa kustutada kuni neil on ootel tasumised "
 "ettevõttega \"%(ettevõtetega)\""
```

### Comparing `trytond_account_payment-6.6.0/locale/fa.po` & `trytond_account_payment-6.8.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr "توالی گروه پرداخت"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "پرداخت مستقیم"
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "مبلغ پرداختی"
+msgid "Amount to Pay"
+msgstr "خطوط برای پرداخت"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "مسدود شده"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -427,14 +428,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "پردازش"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "همه"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "شما نمیتوانید نهاد/سازمان : \"%(party)s\" را حذف کنید در حالی که آنها در "
 "انتظار پرداخت با شرکت: \"%(company)s\" هستند."
```

### Comparing `trytond_account_payment-6.6.0/locale/fi.po` & `trytond_account_payment-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -427,14 +428,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processing"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/fr.po` & `trytond_account_payment-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 msgstr "Séquence de groupe de paiements"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Prélèvement automatique"
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Montant du paiement"
+msgid "Amount to Pay"
+msgstr "Montant à payer"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Bloquée"
 
 msgctxt "field:account.move.line,payment_currency:"
 msgid "Payment Currency"
@@ -403,14 +403,24 @@
 msgstr "À approuver"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "À traiter"
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Tous"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr "En attentes"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "Vous ne pouvez pas effacer le tiers « %(party)s » tant qu'il y a des "
 "paiements en attente avec la société « %(company)s »."
```

### Comparing `trytond_account_payment-6.6.0/locale/hu.po` & `trytond_account_payment-6.8.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -450,14 +451,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processing"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Összes"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/id.po` & `trytond_account_payment-6.8.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Jumlah"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Diblokir"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -415,14 +416,24 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Proses"
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "Anda tidak dapat manghapus pihak \"%(party)s\" selagi ada pembayaran yang "
 "tertunda dengan perusahaan \"%(company)s\"."
```

### Comparing `trytond_account_payment-6.6.0/locale/it.po` & `trytond_account_payment-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 msgid "Payment Group Sequence"
 msgstr "Sequenza gruppo pagamenti"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Importo pagamento"
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Bloccato"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -439,14 +440,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processa"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/lo.po` & `trytond_account_payment-6.8.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr "ລໍຳດັບໝວດການຈ່າຍ"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "ການຫັກບັນຊີທະນາຄານ"
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "ມູນຄ່າການຈ່າຍ"
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "ກັ້ນໄວ້"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -440,14 +441,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "ດຳເນີນການ"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/lt.po` & `trytond_account_payment-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr "Mokėjimo grupės numeruotė"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Tiesioginis debetas"
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Mokėjimo suma"
+msgid "Amount to Pay"
+msgstr "Mokėtinos eilutės"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Blokuoti"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -427,14 +428,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Process"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Visi"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/nl.po` & `trytond_account_payment-6.8.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgstr "Volgorde van de betalingsgroepen"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Automatische incasso"
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
+msgid "Amount to Pay"
 msgstr "Te betalen bedrag"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "geblokkeerd"
 
 msgctxt "field:account.move.line,payment_currency:"
@@ -403,14 +403,24 @@
 msgstr "Goed te keuren"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Te verwerken"
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Alles"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr "In behandeling"
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 "U kunt de relatie \"% (party) s\" niet verwijderen terwijl ze facturen in "
 "behandeling hebben bij bedrijf \"%(company)s\"."
```

### Comparing `trytond_account_payment-6.6.0/locale/pl.po` & `trytond_account_payment-6.8.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -442,14 +443,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processing"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/pt.po` & `trytond_account_payment-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr "Sequência do Grupo de Pagamento"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Débito Direto"
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Montante do Pagamento"
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Bloqueado"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -440,14 +441,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processar"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/ro.po` & `trytond_account_payment-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Suma"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -51,15 +52,15 @@
 
 msgctxt "field:account.move.line.pay.ask_journal,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:account.move.line.pay.ask_journal,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:account.move.line.pay.ask_journal,journal:"
 msgid "Journal"
 msgstr "Jurnal"
 
 msgctxt "field:account.move.line.pay.ask_journal,journals:"
 msgid "Journals"
@@ -412,14 +413,24 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr ""
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/ru.po` & `trytond_account_payment-6.8.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Сумма оплаты"
+msgid "Amount to Pay"
+msgstr "Строки к оплате"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -467,14 +467,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Обработка"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "Все"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/sl.po` & `trytond_account_payment-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr "Štetje plačilnih skupin"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr "Direktna bremenitev"
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr "Znesek plačila"
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr "Zamrznjeno"
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -440,14 +441,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Obdelava"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/tr.po` & `trytond_account_payment-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -195,17 +196,18 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.payment.journal,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment.journal,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:account.payment.journal,process_method:"
 msgid "Process Method"
 msgstr ""
 
 msgctxt "field:party.party,payment_direct_debit:"
 msgid "Direct Debit"
@@ -427,14 +429,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processing"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "All"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/uk.po` & `trytond_account_payment-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
+msgid "Amount to Pay"
 msgstr ""
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 msgctxt "field:account.move.line,payment_currency:"
@@ -400,14 +400,24 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr ""
 
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr ""
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/locale/zh_CN.po` & `trytond_account_payment-6.8.0/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
-msgid "Payment Amount"
-msgstr ""
+msgid "Amount to Pay"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
@@ -436,14 +437,25 @@
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_domain_to_process"
 msgid "To Process"
 msgstr "Processing"
 
+#, fuzzy
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
+msgid "All"
+msgstr "全部"
+
+msgctxt ""
+"model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
+msgid "Pending"
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
```

### Comparing `trytond_account_payment-6.6.0/message.xml` & `trytond_account_payment-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/party.py` & `trytond_account_payment-6.8.0/party.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,26 +79,24 @@
         'on_change_with_currency')
     process_method = fields.Function(
         fields.Selection('get_process_methods', "Process Method"),
         'on_change_with_process_method')
 
     @fields.depends('journal')
     def on_change_with_company(self, name=None):
-        if self.journal:
-            return self.journal.company.id
+        return self.journal.company if self.journal else None
 
     @classmethod
     def search_company(cls, name, clause):
         nested = clause[0][len(name):]
         return [('journal.' + name + nested, *clause[1:])]
 
     @fields.depends('journal')
     def on_change_with_currency(self, name=None):
-        if self.journal:
-            return self.journal.currency.id
+        return self.journal.currency if self.journal else None
 
     @classmethod
     def get_process_methods(cls):
         pool = Pool()
         Journal = pool.get('account.payment.journal')
         name = 'process_method'
         return Journal.fields_get([name])[name]['selection']
```

### Comparing `trytond_account_payment-6.6.0/party.xml` & `trytond_account_payment-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/payment.py` & `trytond_account_payment-6.8.0/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,16 +265,15 @@
             else:
                 return [('id', reverse[clause[1]], query_not_completed)]
         else:
             return []
 
     @fields.depends('journal')
     def on_change_with_currency(self, name=None):
-        if self.journal:
-            return self.journal.currency.id
+        return self.journal.currency if self.journal else None
 
     @classmethod
     def search_currency(cls, name, clause):
         return [('journal.' + clause[0],) + tuple(clause[1:])]
 
 
 _STATES = {
@@ -474,16 +473,15 @@
 
     @staticmethod
     def default_state():
         return 'draft'
 
     @fields.depends('journal')
     def on_change_with_currency(self, name=None):
-        if self.journal:
-            return self.journal.currency.id
+        return self.journal.currency if self.journal else None
 
     @classmethod
     def search_currency(cls, name, clause):
         return [('journal.' + clause[0],) + tuple(clause[1:])]
 
     @classmethod
     def order_amount(cls, tables):
```

### Comparing `trytond_account_payment-6.6.0/payment.xml` & `trytond_account_payment-6.8.0/payment.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_payment-6.6.0/payment.xml` & `trytond_account_payment-6.8.0/payment.xml`

```diff
@@ -100,14 +100,27 @@
       <field name="act_window" ref="act_payment_group_form"/>
     </record>
     <record model="ir.action.act_window.view" id="act_payment_group_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="payment_group_view_form"/>
       <field name="act_window" ref="act_payment_group_form"/>
     </record>
+    <record model="ir.action.act_window.domain" id="act_payment_group_form_domain_not_completed">
+      <field name="name">Pending</field>
+      <field name="sequence" eval="10"/>
+      <field name="domain" eval="[('payment_complete', '=', False)]" pyson="1"/>
+      <field name="count" eval="True"/>
+      <field name="act_window" ref="act_payment_group_form"/>
+    </record>
+    <record model="ir.action.act_window.domain" id="act_payment_group_form_domain_all">
+      <field name="name">All</field>
+      <field name="sequence" eval="9999"/>
+      <field name="domain"/>
+      <field name="act_window" ref="act_payment_group_form"/>
+    </record>
     <menuitem parent="menu_payments" action="act_payment_group_form" sequence="30" id="menu_payment_group_form"/>
     <record model="ir.rule.group" id="rule_group_payment_group_companies">
       <field name="name">User in companies</field>
       <field name="model" search="[('model', '=', 'account.payment.group')]"/>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_group_companies">
```

### Comparing `trytond_account_payment-6.6.0/setup.py` & `trytond_account_payment-6.8.0/setup.py`

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
@@ -34,65 +31,46 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_payment'
 
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
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_account_dunning'),
     ]
 for dep in ['account_invoice']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for payment',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_payment',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment',
     package_dir={'trytond.modules.account_payment': '.'},
     packages=(
         ['trytond.modules.account_payment']
         + ['trytond.modules.account_payment.%s' % p for p in find_packages()]
         ),
@@ -129,28 +107,27 @@
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
     account_payment = trytond.modules.account_payment
     """,
     )
```

### Comparing `trytond_account_payment-6.6.0/tests/scenario_account_payment.rst` & `trytond_account_payment-6.8.0/tests/scenario_account_payment.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 ================
 Payment Scenario
 ================
 
 Imports::
-    >>> import datetime
+
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> tomorrow = datetime.date.today() + datetime.timedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_payment')
 
 Create company::
 
@@ -34,15 +37,15 @@
     >>> user = User(config.user)
     >>> user.employees.append(employee)
     >>> user.employee = employee
     >>> user.save()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, (today, tomorrow))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> payable = accounts['payable']
```

### Comparing `trytond_account_payment-6.6.0/tests/scenario_account_payment_direct_debit.rst` & `trytond_account_payment-6.8.0/tests/scenario_account_payment_direct_debit.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
 
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
+    >>> after_tomorrow = tomorrow + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_payment')
 
     >>> Journal = Model.get('account.journal')
     >>> Move = Model.get('account.move')
@@ -30,15 +31,15 @@
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, (today, after_tomorrow))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
@@ -79,15 +80,15 @@
     ...     account=accounts['revenue'],
     ...     credit=Decimal('200.00'))
     >>> move.click('post')
 
 Create direct debit::
 
     >>> create_direct_debit = Wizard('account.move.line.create_direct_debit')
-    >>> create_direct_debit.form.date = tomorrow + dt.timedelta(days=1)
+    >>> create_direct_debit.form.date = after_tomorrow
     >>> create_direct_debit.execute('create_')
 
     >>> payment, = Payment.find([])
     >>> payment.amount
     Decimal('100.00')
     >>> payment.party == customer1
     True
@@ -95,12 +96,12 @@
     True
     >>> payment.journal == payment_journal
     True
 
 Re-run create direct debit does nothing::
 
     >>> create_direct_debit = Wizard('account.move.line.create_direct_debit')
-    >>> create_direct_debit.form.date = tomorrow + dt.timedelta(days=1)
+    >>> create_direct_debit.form.date = after_tomorrow
     >>> create_direct_debit.execute('create_')
 
     >>> Payment.find([]) == [payment]
     True
```

### Comparing `trytond_account_payment-6.6.0/tests/scenario_account_payment_dunning.rst` & `trytond_account_payment-6.8.0/tests/scenario_account_payment_dunning.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
     >>> expense_journal, = Journal.find([('code', '=', 'EXP')])
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, today)
     >>> fiscalyear.click('create_period')
 
 Create dunning procedure::
 
     >>> procedure = Procedure(name='Procedure')
     >>> level = procedure.levels.new(overdue=dt.timedelta(0))
     >>> procedure.save()
```

### Comparing `trytond_account_payment-6.6.0/tests/scenario_account_payment_invoice.rst` & `trytond_account_payment-6.8.0/tests/scenario_account_payment_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/tests/scenario_account_payment_planning.rst` & `trytond_account_payment-6.8.0/tests/scenario_account_payment_planning.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 =========================
 Payment Planning Scenario
 =========================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + datetime.timedelta(days=1)
-    >>> next_week = today + datetime.timedelta(weeks=1)
+
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
+    >>> next_week = today + dt.timedelta(weeks=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_payment')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, (today, next_week))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> payable = accounts['payable']
```

### Comparing `trytond_account_payment-6.6.0/tests/test_module.py` & `trytond_account_payment-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/trytond_account_payment.egg-info/PKG-INFO` & `trytond_account_payment-6.8.0/trytond_account_payment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-payment
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment
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
 
 Account Payment Module
 ######################
 
 The account_payment module allows to generate grouped payments for receivable
@@ -72,19 +72,20 @@
 - Party.
 - Line.
 - Amount.
 - Date.
 - Description.
 
 A payment can be created from an payable or receivable *Account Move Line*
-using the `Pay Lines` action. The amount is computed from the debit/credit
+using the ``Pay Lines`` action. The amount is computed from the debit/credit
 deducing existing payments for this line.
 
-Direct debit payments can be created from the wizard `Create Direct Debit` for
-all the parties that are configured with at least one *Direct Debits* record.
+Direct debit payments can be created from the wizard ``Create Direct Debit``
+for all the parties that are configured with at least one *Direct Debits*
+record.
 
 The payment can be in one of this states:
 
 * Draft
 
   The payment is in preparation.
```

### Comparing `trytond_account_payment-6.6.0/trytond_account_payment.egg-info/SOURCES.txt` & `trytond_account_payment-6.8.0/trytond_account_payment.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
@@ -52,14 +48,15 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_account_payment.rst
+./tests/scenario_account_payment_blocked_direct_debit.rst
 ./tests/scenario_account_payment_direct_debit.rst
 ./tests/scenario_account_payment_dunning.rst
 ./tests/scenario_account_payment_invoice.rst
 ./tests/scenario_account_payment_planning.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/configuration_form.xml
@@ -76,14 +73,15 @@
 ./view/payment_form.xml
 ./view/payment_group_form.xml
 ./view/payment_group_list.xml
 ./view/payment_journal_form.xml
 ./view/payment_journal_list.xml
 ./view/payment_list.xml
 ./view/payment_process_start_form.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-payment.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
@@ -105,14 +103,15 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_account_payment.rst
+tests/scenario_account_payment_blocked_direct_debit.rst
 tests/scenario_account_payment_direct_debit.rst
 tests/scenario_account_payment_dunning.rst
 tests/scenario_account_payment_invoice.rst
 tests/scenario_account_payment_planning.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_account_payment.egg-info/PKG-INFO
```

### Comparing `trytond_account_payment-6.6.0/view/move_line_list.xml` & `trytond_account_payment-6.8.0/view/move_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/view/payment_form.xml` & `trytond_account_payment-6.8.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/view/payment_group_form.xml` & `trytond_account_payment-6.8.0/view/payment_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/view/payment_group_list.xml` & `trytond_account_payment-6.8.0/view/payment_group_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-6.6.0/view/payment_list.xml` & `trytond_account_payment-6.8.0/view/payment_list.xml`

 * *Files identical despite different names*

