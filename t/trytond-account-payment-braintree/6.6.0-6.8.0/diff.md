# Comparing `tmp/trytond_account_payment_braintree-6.6.0.tar.gz` & `tmp/trytond_account_payment_braintree-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_braintree-6.6.0.tar", last modified: Mon Oct 31 16:08:06 2022, max compression
+gzip compressed data, was "trytond_account_payment_braintree-6.8.0.tar", last modified: Mon May  1 11:41:39 2023, max compression
```

## Comparing `trytond_account_payment_braintree-6.6.0.tar` & `trytond_account_payment_braintree-6.8.0.tar`

### file list

```diff
@@ -1,77 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:08:06.827566 trytond_account_payment_braintree-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2078 2022-04-08 16:28:15.000000 trytond_account_payment_braintree-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_payment_braintree-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2022-10-31 16:08:05.000000 trytond_account_payment_braintree-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_payment_braintree-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2022-10-31 16:08:04.000000 trytond_account_payment_braintree-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:08:04.000000 trytond_account_payment_braintree-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_payment_braintree-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4607 2022-10-31 16:08:06.824233 trytond_account_payment_braintree-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2353 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1081 2022-07-17 17:15:34.000000 trytond_account_payment_braintree-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46483 2022-10-11 19:49:57.000000 trytond_account_payment_braintree-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17629 2022-04-11 18:44:50.000000 trytond_account_payment_braintree-6.6.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     3101 2022-04-10 15:40:34.000000 trytond_account_payment_braintree-6.6.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:08:06.820900 trytond_account_payment_braintree-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2353 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:08:06.814233 trytond_account_payment_braintree-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13948 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13893 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13949 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14005 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11780 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11779 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13780 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11698 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2022-10-29 07:50:34.000000 trytond_account_payment_braintree-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      618 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2238 2022-07-17 17:15:34.000000 trytond_account_payment_braintree-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2021-10-30 15:32:31.000000 trytond_account_payment_braintree-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2857 2021-12-11 16:59:32.000000 trytond_account_payment_braintree-6.6.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:08:06.827566 trytond_account_payment_braintree-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5437 2022-10-29 07:39:10.000000 trytond_account_payment_braintree-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:08:06.817566 trytond_account_payment_braintree-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_payment_braintree-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8936 2022-04-11 18:44:50.000000 trytond_account_payment_braintree-6.6.0/tests/scenario_account_payment_braintree.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-04-16 16:30:56.000000 trytond_account_payment_braintree-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2022-04-25 16:11:52.000000 trytond_account_payment_braintree-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:10:09.000000 trytond_account_payment_braintree-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2022-10-31 16:08:03.000000 trytond_account_payment_braintree-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:08:06.824233 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4607 2022-10-31 16:08:06.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2301 2022-10-31 16:08:06.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:08:06.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2022-10-31 16:08:06.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-10-13 07:23:31.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2022-10-31 16:08:06.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:08:06.000000 trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:08:06.820900 trytond_account_payment_braintree-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2022-04-08 16:23:26.000000 trytond_account_payment_braintree-6.6.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2022-07-17 17:15:34.000000 trytond_account_payment_braintree-6.6.0/view/customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/view/customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/view/customer_payment_method_delete_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      634 2021-10-30 15:32:31.000000 trytond_account_payment_braintree-6.6.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2272 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2020-10-08 20:25:22.000000 trytond_account_payment_braintree-6.6.0/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      760 2022-04-11 18:44:50.000000 trytond_account_payment_braintree-6.6.0/view/refund_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2022-04-11 18:44:50.000000 trytond_account_payment_braintree-6.6.0/view/refund_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:39.862459 trytond_account_payment_braintree-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2023-05-01 11:01:14.000000 trytond_account_payment_braintree-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:01:13.000000 trytond_account_payment_braintree-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4595 2023-05-01 11:41:39.862459 trytond_account_payment_braintree-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46420 2023-04-21 08:36:08.000000 trytond_account_payment_braintree-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17629 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     3098 2023-04-21 08:36:08.000000 trytond_account_payment_braintree-6.8.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:39.859126 trytond_account_payment_braintree-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:39.852459 trytond_account_payment_braintree-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13948 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13873 2023-04-30 10:46:36.000000 trytond_account_payment_braintree-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13949 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14005 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11780 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11779 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13780 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11698 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-04-29 08:02:40.000000 trytond_account_payment_braintree-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      618 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2238 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2716 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:41:39.862459 trytond_account_payment_braintree-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4589 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:39.852459 trytond_account_payment_braintree-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8860 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/tests/scenario_account_payment_braintree.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-05-01 11:01:08.000000 trytond_account_payment_braintree-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:39.862459 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4595 2023-05-01 11:41:39.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-05-01 11:41:39.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:41:39.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 11:41:39.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      173 2023-05-01 11:41:39.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:41:39.000000 trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:39.859126 trytond_account_payment_braintree-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/customer_payment_method_delete_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      634 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2272 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      760 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/refund_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-6.8.0/view/refund_list.xml
```

### Comparing `trytond_account_payment_braintree-6.6.0/COPYRIGHT` & `trytond_account_payment_braintree-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2022 B2CK
-Copyright (C) 2020-2022 Cédric Krier
+Copyright (C) 2020-2023 B2CK
+Copyright (C) 2020-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_payment_braintree-6.6.0/LICENSE` & `trytond_account_payment_braintree-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/PKG-INFO` & `trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_payment_braintree
-Version: 6.6.0
+Name: trytond-account-payment-braintree
+Version: 6.8.0
 Summary: Tryton module for Braintree payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_braintree
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment braintree
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
 
 Account Payment Braintree Module
 ################################
 
 The account_payment_braintree module allows receipt of payments using
@@ -111,11 +111,11 @@
 
 .. _payment method: https://developers.braintreepayments.com/guides/payment-methods
 
 Configuration
 *************
 
 The account_payment_braintree module uses the section
-`account_payment_braintree` to retrieve some parameters:
+``account_payment_braintree`` to retrieve some parameters:
 
-- `payment_methods_cache`: defines the duration in seconds that payment methods
-  are kept in the cache. The default value is `15 * 60`.
+- ``payment_methods_cache``: defines the duration in seconds that payment
+  methods are kept in the cache. The default value is ``15 * 60``.
```

### Comparing `trytond_account_payment_braintree-6.6.0/README.rst` & `trytond_account_payment_braintree-6.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,11 +57,11 @@
 
 .. _payment method: https://developers.braintreepayments.com/guides/payment-methods
 
 Configuration
 *************
 
 The account_payment_braintree module uses the section
-`account_payment_braintree` to retrieve some parameters:
+``account_payment_braintree`` to retrieve some parameters:
 
-- `payment_methods_cache`: defines the duration in seconds that payment methods
-  are kept in the cache. The default value is `15 * 60`.
+- ``payment_methods_cache``: defines the duration in seconds that payment
+  methods are kept in the cache. The default value is ``15 * 60``.
```

### Comparing `trytond_account_payment_braintree-6.6.0/__init__.py` & `trytond_account_payment_braintree-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/account.py` & `trytond_account_payment_braintree-6.8.0/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,21 +612,19 @@
 
     @classmethod
     def default_state(cls):
         return 'draft'
 
     @fields.depends('payment', '_parent_payment.currency')
     def on_change_with_currency(self, name=None):
-        if self.payment and self.payment.currency:
-            return self.payment.currency.id
+        return self.payment.currency if self.payment else None
 
     @fields.depends('payment', '_parent_payment.company')
     def on_change_with_company(self, name=None):
-        if self.payment and self.payment.company:
-            return self.payment.company.id
+        return self.payment.company if self.payment else None
 
     @classmethod
     def copy(cls, refunds, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
```

### Comparing `trytond_account_payment_braintree-6.6.0/account.xml` & `trytond_account_payment_braintree-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/checkout.html` & `trytond_account_payment_braintree-6.8.0/checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/common.py` & `trytond_account_payment_braintree-6.8.0/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         except AttributeError:
             pass
         self.braintree_customer = None
 
     @fields.depends('journal')
     def on_change_with_braintree_account(self, name=None):
         if self.journal and self.journal.process_method == 'braintree':
-            return self.journal.braintree_account.id
+            return self.journal.braintree_account
 
     @fields.depends('braintree_customer', 'braintree_customer_method')
     def get_braintree_customer_methods(self):
         methods = [('', '')]
         if self.braintree_customer:
             methods.extend(self.braintree_customer.payment_methods())
         if (self.braintree_customer_method
```

### Comparing `trytond_account_payment_braintree-6.6.0/doc/index.rst` & `trytond_account_payment_braintree-6.8.0/doc/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,11 +57,11 @@
 
 .. _payment method: https://developers.braintreepayments.com/guides/payment-methods
 
 Configuration
 *************
 
 The account_payment_braintree module uses the section
-`account_payment_braintree` to retrieve some parameters:
+``account_payment_braintree`` to retrieve some parameters:
 
-- `payment_methods_cache`: defines the duration in seconds that payment methods
-  are kept in the cache. The default value is `15 * 60`.
+- ``payment_methods_cache``: defines the duration in seconds that payment
+  methods are kept in the cache. The default value is ``15 * 60``.
```

### Comparing `trytond_account_payment_braintree-6.6.0/ir.py` & `trytond_account_payment_braintree-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/bg.po` & `trytond_account_payment_braintree-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/ca.po` & `trytond_account_payment_braintree-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/cs.po` & `trytond_account_payment_braintree-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/de.po` & `trytond_account_payment_braintree-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 "field:account.payment.braintree.customer.payment_method.delete.ask,customer:"
 msgid "Customer"
 msgstr "Kunde"
 
 msgctxt ""
 "field:account.payment.braintree.customer.payment_method.delete.ask,payment_method:"
 msgid "Payment Method"
-msgstr "Zahlungsmethode"
+msgstr "Zahlungsart"
 
 msgctxt "field:account.payment.braintree.refund,amount:"
 msgid "Amount"
 msgstr "Betrag"
 
 msgctxt "field:account.payment.braintree.refund,approved_by:"
 msgid "Approved by"
@@ -232,15 +232,15 @@
 msgctxt "model:account.payment.braintree.customer.identical,name:"
 msgid "Braintree Customer Identical"
 msgstr "Braintree Kunde Identisch"
 
 msgctxt ""
 "model:account.payment.braintree.customer.payment_method.delete.ask,name:"
 msgid "Delete Customer Payment Method"
-msgstr "Zahlungsmethode Kunde löschen"
+msgstr "Zahlungsart Kunde löschen"
 
 msgctxt "model:account.payment.braintree.refund,name:"
 msgid "Braintree Payment Refund"
 msgstr "Braintree Zahlung Erstattung"
 
 msgctxt "model:ir.action,name:act_account_form"
 msgid "Braintree Accounts"
@@ -328,15 +328,15 @@
 
 msgctxt "model:ir.model.button,string:customer_braintree_checkout_button"
 msgid "Add Card"
 msgstr "Karte hinzufügen"
 
 msgctxt "model:ir.model.button,string:customer_payment_method_delete_button"
 msgid "Delete Payment Method"
-msgstr "Zahlungsmethode löschen"
+msgstr "Zahlungsart löschen"
 
 msgctxt "model:ir.model.button,string:payment_braintree_checkout_button"
 msgid "Braintree Checkout"
 msgstr "Braintree Checkout"
 
 msgctxt "model:ir.model.button,string:payment_braintree_pull_button"
 msgid "Braintree Pull"
@@ -464,15 +464,15 @@
 
 msgctxt "view:account.payment:"
 msgid "Nonce:"
 msgstr "Nonce:"
 
 msgctxt "view:account.payment:"
 msgid "Payment Method:"
-msgstr "Zahlungsmethode:"
+msgstr "Zahlungsart:"
 
 msgctxt "view:account.payment:"
 msgid "Settle:"
 msgstr "Ausgleich:"
 
 msgctxt "view:account.payment:"
 msgid "Settled:"
@@ -484,15 +484,15 @@
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Customer:"
 msgstr "Kunde:"
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Payment Method:"
-msgstr "Zahlungsmethode:"
+msgstr "Zahlungsart:"
 
 msgctxt ""
 "wizard_button:account.payment.braintree.customer.payment_method.delete,ask,delete_:"
 msgid "Delete"
 msgstr "Löschen"
 
 msgctxt ""
```

### Comparing `trytond_account_payment_braintree-6.6.0/locale/es.po` & `trytond_account_payment_braintree-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/es_419.po` & `trytond_account_payment_braintree-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/et.po` & `trytond_account_payment_braintree-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/fa.po` & `trytond_account_payment_braintree-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/fi.po` & `trytond_account_payment_braintree-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/fr.po` & `trytond_account_payment_braintree-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/hu.po` & `trytond_account_payment_braintree-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/id.po` & `trytond_account_payment_braintree-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/it.po` & `trytond_account_payment_braintree-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/lo.po` & `trytond_account_payment_braintree-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/lt.po` & `trytond_account_payment_braintree-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/nl.po` & `trytond_account_payment_braintree-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/pl.po` & `trytond_account_payment_braintree-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/pt.po` & `trytond_account_payment_braintree-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/ro.po` & `trytond_account_payment_braintree-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/ru.po` & `trytond_account_payment_braintree-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/sl.po` & `trytond_account_payment_braintree-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/tr.po` & `trytond_account_payment_braintree-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/uk.po` & `trytond_account_payment_braintree-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/locale/zh_CN.po` & `trytond_account_payment_braintree-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/message.xml` & `trytond_account_payment_braintree-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/party.py` & `trytond_account_payment_braintree-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/party.xml` & `trytond_account_payment_braintree-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/routes.py` & `trytond_account_payment_braintree-6.8.0/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import http.client
 import logging
 
-try:
-    from http import HTTPStatus
-except ImportError:
-    from http import client as HTTPStatus
-
 import braintree
-from werkzeug.exceptions import abort
-from werkzeug.wrappers import Response
 
-from trytond.protocols.wrappers import with_pool, with_transaction
+from trytond.protocols.wrappers import (
+    HTTPStatus, Response, abort, with_pool, with_transaction)
 from trytond.wsgi import app
 
 logger = logging.getLogger(__name__)
 
 
 @app.route(
     '/<database_name>/account_payment_braintree/checkout/<model>/<id>',
```

### Comparing `trytond_account_payment_braintree-6.6.0/setup.py` & `trytond_account_payment_braintree-6.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     if slice:
         content = '\n'.join(content.splitlines()[slice])
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
@@ -37,61 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_payment_braintree'
 
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
 
-requires = ['braintree >= 3.38.0', 'werkzeug']
+requires = ['braintree >= 3.38.0']
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
     description='Tryton module for Braintree payment',
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
-            'https://hg.tryton.org/modules/account_payment_braintree'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment braintree',
     package_dir={'trytond.modules.account_payment_braintree': '.'},
     packages=(
         ['trytond.modules.account_payment_braintree']
         + ['trytond.modules.account_payment_braintree.%s' % p
             for p in find_packages()]
@@ -129,27 +106,26 @@
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
     account_payment_braintree = trytond.modules.account_payment_braintree
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_payment_braintree-6.6.0/tests/scenario_account_payment_braintree.rst` & `trytond_account_payment_braintree-6.8.0/tests/scenario_account_payment_braintree.rst`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,15 @@
     >>> payment.amount = amount = Decimal(random.randint(0, 1999))
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
 
 Checkout the payment::
 
-    >>> action_id = payment.click('braintree_checkout')
-    >>> checkout = Wizard('account.payment.braintree.checkout', [payment])
+    >>> checkout = payment.click('braintree_checkout')
     >>> bool(payment.braintree_checkout_id)
     True
 
     >>> Payment.write([payment.id], {
     ...     'braintree_nonce': Nonces.Transactable,
     ...     }, config.context)
```

### Comparing `trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/PKG-INFO` & `trytond_account_payment_braintree-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-payment-braintree
-Version: 6.6.0
+Name: trytond_account_payment_braintree
+Version: 6.8.0
 Summary: Tryton module for Braintree payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_braintree
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment braintree
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
 
 Account Payment Braintree Module
 ################################
 
 The account_payment_braintree module allows receipt of payments using
@@ -111,11 +111,11 @@
 
 .. _payment method: https://developers.braintreepayments.com/guides/payment-methods
 
 Configuration
 *************
 
 The account_payment_braintree module uses the section
-`account_payment_braintree` to retrieve some parameters:
+``account_payment_braintree`` to retrieve some parameters:
 
-- `payment_methods_cache`: defines the duration in seconds that payment methods
-  are kept in the cache. The default value is `15 * 60`.
+- ``payment_methods_cache``: defines the duration in seconds that payment
+  methods are kept in the cache. The default value is ``15 * 60``.
```

### Comparing `trytond_account_payment_braintree-6.6.0/trytond_account_payment_braintree.egg-info/SOURCES.txt` & `trytond_account_payment_braintree-6.8.0/trytond_account_payment_braintree.egg-info/SOURCES.txt`

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
@@ -66,14 +62,15 @@
 ./view/customer_payment_method_delete_ask_form.xml
 ./view/party_reception_direct_debit_form.xml
 ./view/payment_form.xml
 ./view/payment_journal_form.xml
 ./view/payment_list.xml
 ./view/refund_form.xml
 ./view/refund_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_payment_braintree-6.6.0/view/account_form.xml` & `trytond_account_payment_braintree-6.8.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/view/customer_form.xml` & `trytond_account_payment_braintree-6.8.0/view/customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/view/party_reception_direct_debit_form.xml` & `trytond_account_payment_braintree-6.8.0/view/party_reception_direct_debit_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/view/payment_form.xml` & `trytond_account_payment_braintree-6.8.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-6.6.0/view/refund_form.xml` & `trytond_account_payment_braintree-6.8.0/view/refund_form.xml`

 * *Files identical despite different names*

