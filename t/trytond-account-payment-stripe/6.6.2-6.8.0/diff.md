# Comparing `tmp/trytond_account_payment_stripe-6.6.2.tar.gz` & `tmp/trytond_account_payment_stripe-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_stripe-6.6.2.tar", last modified: Sat Mar  4 12:11:42 2023, max compression
+gzip compressed data, was "trytond_account_payment_stripe-6.8.0.tar", last modified: Mon May  1 11:53:27 2023, max compression
```

## Comparing `trytond_account_payment_stripe-6.6.2.tar` & `trytond_account_payment_stripe-6.8.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:11:42.959450 trytond_account_payment_stripe-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     1941 2023-03-04 12:11:38.000000 trytond_account_payment_stripe-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-03-04 12:11:37.000000 trytond_account_payment_stripe-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4835 2023-03-04 12:11:42.959450 trytond_account_payment_stripe-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2529 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      953 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5183 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     5067 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:11:42.949450 trytond_account_payment_stripe-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2529 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1274 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/email_checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1091 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:11:42.929449 trytond_account_payment_stripe-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17701 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17573 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17713 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14745 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14708 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17994 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17665 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14826 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16182 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16208 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17320 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16909 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14655 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16569 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14625 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    70087 2023-02-27 18:02:47.000000 trytond_account_payment_stripe-6.6.2/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18234 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2914 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 12:11:42.962783 trytond_account_payment_stripe-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4558 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:11:42.936116 trytond_account_payment_stripe-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10504 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8780 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe_dispute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3198 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe_identical.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5210 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe_intent.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2023-02-17 18:53:13.000000 trytond_account_payment_stripe-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:11:42.959450 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4835 2023-03-04 12:11:42.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2582 2023-03-04 12:11:42.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:11:42.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-03-04 12:11:42.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-17 18:53:04.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-03-04 12:11:42.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 12:11:42.000000 trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:11:42.946116 trytond_account_payment_stripe-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/customer_source_detach_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2519 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      955 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/refund_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2022-12-19 12:02:49.000000 trytond_account_payment_stripe-6.6.2/view/refund_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:27.861245 trytond_account_payment_stripe-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-05-01 11:09:05.000000 trytond_account_payment_stripe-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:09:05.000000 trytond_account_payment_stripe-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4830 2023-05-01 11:53:27.861245 trytond_account_payment_stripe-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5183 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     5064 2023-04-21 08:36:08.000000 trytond_account_payment_stripe-6.8.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:27.861245 trytond_account_payment_stripe-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2539 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1274 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/email_checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:27.851245 trytond_account_payment_stripe-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17701 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17557 2023-04-30 10:46:36.000000 trytond_account_payment_stripe-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17713 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14745 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14708 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17994 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17665 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14826 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16182 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16208 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17320 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16909 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14655 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16569 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14625 2023-04-29 08:02:46.000000 trytond_account_payment_stripe-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-04-29 08:02:47.000000 trytond_account_payment_stripe-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    70122 2023-04-21 08:36:08.000000 trytond_account_payment_stripe-6.8.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18234 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2861 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:53:27.861245 trytond_account_payment_stripe-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4503 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:27.854578 trytond_account_payment_stripe-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10345 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8648 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe_dispute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3211 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe_identical.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5295 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe_intent.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2023-05-01 11:09:00.000000 trytond_account_payment_stripe-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:27.861245 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4830 2023-05-01 11:53:26.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2582 2023-05-01 11:53:27.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:53:26.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:53:26.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-05-01 11:53:26.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:53:26.000000 trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:27.857912 trytond_account_payment_stripe-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-6.8.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/customer_source_detach_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-6.8.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      955 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/refund_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-6.8.0/view/refund_list.xml
```

### Comparing `trytond_account_payment_stripe-6.6.2/CHANGELOG` & `trytond_account_payment_stripe-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 
-Version 6.6.2 - 2023-03-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2023-02-17
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_payment_stripe-6.6.2/COPYRIGHT` & `trytond_account_payment_stripe-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/LICENSE` & `trytond_account_payment_stripe-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/PKG-INFO` & `trytond_account_payment_stripe-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for Stripe payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_stripe
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment stripe
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
 
 Account Payment Stripe Module
 #############################
 
 The account_payment_stripe module allows to receive payment from `Stripe`_.
@@ -114,15 +114,15 @@
 
 .. _source: https://stripe.com/docs/sources
 .. _`payment method`: https://stripe.com/docs/payments/payment-methods
 
 Configuration
 *************
 
-The account_payment_stripe module uses the section `account_payment_stripe` to
-retrieve some parameters:
+The account_payment_stripe module uses the section ``account_payment_stripe``
+to retrieve some parameters:
 
-- `sources_cache`: defines the duration in seconds the sources are kept in the
-  cache. The default value is `15 * 60`.
+- ``sources_cache``: defines the duration in seconds the sources are kept in
+  the cache. The default value is ``15 * 60``.
 
-- `max_network_retries`: defines the maximum number of retries the Stripe
-  library may perform. The default value is `3`.
+- ``max_network_retries``: defines the maximum number of retries the Stripe
+  library may perform. The default value is ``3``.
```

### Comparing `trytond_account_payment_stripe-6.6.2/README.rst` & `trytond_account_payment_stripe-6.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 .. _source: https://stripe.com/docs/sources
 .. _`payment method`: https://stripe.com/docs/payments/payment-methods
 
 Configuration
 *************
 
-The account_payment_stripe module uses the section `account_payment_stripe` to
-retrieve some parameters:
+The account_payment_stripe module uses the section ``account_payment_stripe``
+to retrieve some parameters:
 
-- `sources_cache`: defines the duration in seconds the sources are kept in the
-  cache. The default value is `15 * 60`.
+- ``sources_cache``: defines the duration in seconds the sources are kept in
+  the cache. The default value is ``15 * 60``.
 
-- `max_network_retries`: defines the maximum number of retries the Stripe
-  library may perform. The default value is `3`.
+- ``max_network_retries``: defines the maximum number of retries the Stripe
+  library may perform. The default value is ``3``.
```

### Comparing `trytond_account_payment_stripe-6.6.2/__init__.py` & `trytond_account_payment_stripe-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/checkout.html` & `trytond_account_payment_stripe-6.8.0/checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/common.py` & `trytond_account_payment_stripe-6.8.0/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.stripe_customer = None
         self.stripe_customer_source = None
         self.stripe_customer_source_selection = None
 
     @fields.depends('journal')
     def on_change_with_stripe_account(self, name=None):
         if self.journal and self.journal.process_method == 'stripe':
-            return self.journal.stripe_account.id
+            return self.journal.stripe_account
 
     @fields.depends('stripe_customer', 'stripe_customer_source')
     def get_stripe_customer_sources(self):
         sources = [('', '')]
         if self.stripe_customer:
             sources.extend(self.stripe_customer.sources())
         if (self.stripe_customer_source
```

### Comparing `trytond_account_payment_stripe-6.6.2/doc/conf.py` & `trytond_account_payment_stripe-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_payment_stripe-6.6.2/doc/index.rst` & `trytond_account_payment_stripe-6.8.0/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 .. _source: https://stripe.com/docs/sources
 .. _`payment method`: https://stripe.com/docs/payments/payment-methods
 
 Configuration
 *************
 
-The account_payment_stripe module uses the section `account_payment_stripe` to
-retrieve some parameters:
+The account_payment_stripe module uses the section ``account_payment_stripe``
+to retrieve some parameters:
 
-- `sources_cache`: defines the duration in seconds the sources are kept in the
-  cache. The default value is `15 * 60`.
+- ``sources_cache``: defines the duration in seconds the sources are kept in
+  the cache. The default value is ``15 * 60``.
 
-- `max_network_retries`: defines the maximum number of retries the Stripe
-  library may perform. The default value is `3`.
+- ``max_network_retries``: defines the maximum number of retries the Stripe
+  library may perform. The default value is ``3``.
```

### Comparing `trytond_account_payment_stripe-6.6.2/email_checkout.html` & `trytond_account_payment_stripe-6.8.0/email_checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/ir.py` & `trytond_account_payment_stripe-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/bg.po` & `trytond_account_payment_stripe-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/ca.po` & `trytond_account_payment_stripe-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/cs.po` & `trytond_account_payment_stripe-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/de.po` & `trytond_account_payment_stripe-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -44,19 +44,19 @@
 
 msgctxt "field:account.payment,stripe_customer:"
 msgid "Stripe Customer"
 msgstr "Stripe Kunde"
 
 msgctxt "field:account.payment,stripe_customer_payment_method:"
 msgid "Stripe Payment Method"
-msgstr "Stripe Zahlungsmethode"
+msgstr "Stripe Zahlungsart"
 
 msgctxt "field:account.payment,stripe_customer_payment_method_selection:"
 msgid "Stripe Customer Payment Method"
-msgstr "Stripe Kunde Zahlungsmethode"
+msgstr "Stripe Kunde Zahlungsart"
 
 msgctxt "field:account.payment,stripe_customer_source:"
 msgid "Stripe Customer Source"
 msgstr "Stripe Kunde Ursprung"
 
 msgctxt "field:account.payment,stripe_customer_source_selection:"
 msgid "Stripe Customer Source"
@@ -599,15 +599,15 @@
 
 msgctxt "view:account.payment:"
 msgid "Payment Intent:"
 msgstr "Zahlungsabsicht:"
 
 msgctxt "view:account.payment:"
 msgid "Payment Method:"
-msgstr "Zahlungsmethode:"
+msgstr "Zahlungsart:"
 
 msgctxt "view:account.payment:"
 msgid "Source:"
 msgstr "Source:"
 
 msgctxt "view:account.payment:"
 msgid "Stripe"
@@ -619,15 +619,15 @@
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Customer:"
 msgstr "Kunde:"
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Payment Method:"
-msgstr "Zahlungsmethode:"
+msgstr "Zahlungsart:"
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Source:"
 msgstr "Source:"
 
 msgctxt ""
 "wizard_button:account.payment.stripe.customer.source.detach,ask,detach:"
```

### Comparing `trytond_account_payment_stripe-6.6.2/locale/es.po` & `trytond_account_payment_stripe-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/es_419.po` & `trytond_account_payment_stripe-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/et.po` & `trytond_account_payment_stripe-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/fa.po` & `trytond_account_payment_stripe-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/fi.po` & `trytond_account_payment_stripe-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/fr.po` & `trytond_account_payment_stripe-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/hu.po` & `trytond_account_payment_stripe-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/id.po` & `trytond_account_payment_stripe-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/it.po` & `trytond_account_payment_stripe-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/lo.po` & `trytond_account_payment_stripe-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/lt.po` & `trytond_account_payment_stripe-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/nl.po` & `trytond_account_payment_stripe-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/pl.po` & `trytond_account_payment_stripe-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/pt.po` & `trytond_account_payment_stripe-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/ro.po` & `trytond_account_payment_stripe-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/ru.po` & `trytond_account_payment_stripe-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/sl.po` & `trytond_account_payment_stripe-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/tr.po` & `trytond_account_payment_stripe-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/uk.po` & `trytond_account_payment_stripe-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/locale/zh_CN.po` & `trytond_account_payment_stripe-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/message.xml` & `trytond_account_payment_stripe-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/party.py` & `trytond_account_payment_stripe-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/party.xml` & `trytond_account_payment_stripe-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/payment.py` & `trytond_account_payment_stripe-6.8.0/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     fields)
 from trytond.modules.account_payment.exceptions import (
     PaymentValidationError, ProcessError)
 from trytond.modules.company.model import (
     employee_field, reset_employee, set_employee)
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
-from trytond.pyson import Eval
+from trytond.pyson import Eval, TimeDelta
 from trytond.report import Report, get_email
 from trytond.rpc import RPC
 from trytond.sendmail import sendmail_transactional
 from trytond.tools import sql_pairing
 from trytond.tools.email_ import set_from_header
 from trytond.transaction import Transaction
 from trytond.url import http_host
@@ -761,21 +761,19 @@
 
     @classmethod
     def default_stripe_idempotency_key(cls):
         return uuid.uuid4().hex
 
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
     def default_state(cls):
         return 'draft'
 
     @classmethod
     def create(cls, vlist):
@@ -919,14 +917,17 @@
         states={
             'invisible': ~Eval('webhook_identifier'),
             },
         help="The Stripe's signing secret of the webhook.")
     last_event = fields.Char("Last Event", readonly=True, strip=False)
     setup_intent_delay = fields.TimeDelta(
         "Setup Intent Delay", required=True,
+        domain=[
+            ('setup_intent_delay', '>=', TimeDelta()),
+            ],
         help="The delay before cancelling setup intent not succeeded.")
 
     @classmethod
     def __setup__(cls):
         super(Account, cls).__setup__()
         cls._buttons.update({
                 'new_identifier': {
```

### Comparing `trytond_account_payment_stripe-6.6.2/payment.xml` & `trytond_account_payment_stripe-6.8.0/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/routes.py` & `trytond_account_payment_stripe-6.8.0/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import http.client
 import json
 import logging
 
 import stripe
-from werkzeug.exceptions import abort
-from werkzeug.wrappers import Response
 
-from trytond.protocols.wrappers import with_pool, with_transaction
+from trytond.protocols.wrappers import (
+    Response, abort, with_pool, with_transaction)
 from trytond.wsgi import app
 
 logger = logging.getLogger(__name__)
 
 
 @app.route(
     '/<database_name>/account_payment_stripe/checkout/<model>/<id>',
```

### Comparing `trytond_account_payment_stripe-6.6.2/setup.py` & `trytond_account_payment_stripe-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -34,38 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_payment_stripe'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
-requires = ['stripe >= 2.32.0', 'werkzeug']
+requires = ['stripe >= 2.32.0']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for Stripe payment',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_payment_stripe',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment stripe',
     package_dir={'trytond.modules.account_payment_stripe': '.'},
     packages=(
         ['trytond.modules.account_payment_stripe']
         + ['trytond.modules.account_payment_stripe.%s' % p
             for p in find_packages()]
@@ -103,24 +103,24 @@
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

### Comparing `trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe.rst` & `trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 ===============================
 Account Payment Stripe Scenario
 ===============================
 
 Imports::
 
     >>> import os
-    >>> import datetime
+    >>> import datetime as dt
     >>> import time
     >>> from decimal import Decimal
     >>> import stripe
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
 
+    >>> today = dt.date.today()
+
+    >>> FETCH_SLEEP = 1
+
 Activate modules::
 
     >>> config = activate_modules('account_payment_stripe')
 
 Create company::
 
     >>> Company = Model.get('company.company')
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, today)
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
 
 Create Stripe account::
@@ -89,24 +93,23 @@
     >>> payment.description = 'Testing'
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
 
 Checkout the payment::
 
-    >>> action_id = payment.click('stripe_checkout')
-    >>> checkout = Wizard('account.payment.stripe.checkout', [payment])
+    >>> checkout = payment.click('stripe_checkout')
     >>> bool(payment.stripe_checkout_id)
     True
 
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4242424242424242',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Payment.write([payment.id], {
     ...     'stripe_token': token.id,
     ...     'stripe_chargeable': True,
     ...     'stripe_payment_intent_id': None,  # Remove intent from checkout
@@ -115,15 +118,15 @@
 Process the payment::
 
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> bool(payment.stripe_captured)
     True
 
@@ -132,23 +135,22 @@
     >>> previous_idempotency_key = payment.stripe_idempotency_key
     >>> payment, = payment.duplicate()
     >>> payment.stripe_idempotency_key != previous_idempotency_key
     True
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
-    >>> action_id = payment.click('stripe_checkout')
-    >>> checkout = Wizard('account.payment.stripe.checkout', [payment])
+    >>> checkout = payment.click('stripe_checkout')
     >>> bool(payment.stripe_checkout_id)
     True
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4000000000000002',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Payment.write([payment.id], {
     ...     'stripe_token': token.id,
     ...     'stripe_chargeable': True,
     ...     'stripe_payment_intent_id': None,  # Remove intent from checkout
@@ -165,24 +167,23 @@
     >>> Customer = Model.get('account.payment.stripe.customer')
     >>> stripe_customer = Customer()
     >>> stripe_customer.party = customer
     >>> stripe_customer.stripe_account = stripe_account
 
 Checkout the customer::
 
-    >>> action_id = stripe_customer.click('stripe_checkout')
-    >>> checkout = Wizard('account.payment.stripe.checkout', [stripe_customer])
+    >>> checkout = stripe_customer.click('stripe_checkout')
     >>> bool(stripe_customer.stripe_checkout_id)
     True
 
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4012888888881881',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Customer.write(
     ...     [stripe_customer.id], {'stripe_token': token.id}, config.context)
 
 Run cron::
@@ -213,35 +214,34 @@
 Make payment with customer::
 
     >>> payment, = payment.duplicate()
     >>> payment.stripe_customer = stripe_customer
     >>> payment.save()
     >>> _, source = Payment.get_stripe_customer_sources(payment.id, config.context)
     >>> source_id, source_name = source
-    >>> source_name == 'Visa ****1881 12/%s' % (datetime.date.today().year + 1)
+    >>> source_name == 'Visa ****1881 12/%s' % (today.year + 1)
     True
     >>> payment.stripe_customer_source = source_id
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
 
 Detach source::
 
-    >>> detach = Wizard(
-    ...     'account.payment.stripe.customer.source.detach', [stripe_customer])
+    >>> detach = stripe_customer.click('detach_source')
     >>> detach.form.source = source_id
     >>> detach.execute('detach')
 
     >>> cus = stripe.Customer.retrieve(
     ...     stripe_customer.stripe_customer_id, expand=['sources'])
     >>> len(cus.sources)
     0
@@ -276,15 +276,15 @@
 
 Checkout the capture payment::
 
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4242424242424242',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Payment.write([payment.id], {
     ...     'stripe_token': token.id,
     ...     }, config.context)
 
@@ -300,15 +300,15 @@
 Capture lower amount::
 
     >>> payment.amount = Decimal('40')
     >>> payment.click('stripe_do_capture')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> bool(payment.stripe_captured)
     True
 
@@ -320,14 +320,15 @@
     >>> refund.amount = Decimal('38')
     >>> refund.click('submit')
     >>> refund.click('approve')
     >>> cron_refund_create, = Cron.find([
     ...     ('method', '=', 'account.payment.stripe.refund|stripe_create'),
     ...     ])
     >>> cron_refund_create.click('run_once')
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
 
     >>> payment.reload()
     >>> payment.amount
     Decimal('2.00')
     >>> payment.state
     'succeeded'
@@ -339,14 +340,15 @@
 
     >>> refund = Refund()
     >>> refund.payment = payment
     >>> refund.amount = Decimal('2')
     >>> refund.click('submit')
     >>> refund.click('approve')
     >>> cron_refund_create.click('run_once')
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
 
     >>> payment.reload()
     >>> payment.amount
     Decimal('0.00')
     >>> payment.state
     'failed'
@@ -358,11 +360,12 @@
 
     >>> refund = Refund()
     >>> refund.payment = payment
     >>> refund.amount = Decimal('10')
     >>> refund.click('submit')
     >>> refund.click('approve')
     >>> cron_refund_create.click('run_once')
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> refund.reload()
     >>> refund.state
     'failed'
```

### Comparing `trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe_dispute.rst` & `trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe_dispute.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 =======================================
 Account Payment Stripe Dispute Scenario
 =======================================
 
 Imports::
 
     >>> import os
-    >>> import datetime
+    >>> import datetime as dt
     >>> import time
     >>> from decimal import Decimal
     >>> import stripe
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
 
+    >>> today = dt.date.today()
+
+    >>> FETCH_SLEEP = 1
+
 Activate modules::
 
     >>> config = activate_modules('account_payment_stripe')
 
 Create company::
 
     >>> Company = Model.get('company.company')
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, today)
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
 
 Create Stripe account::
@@ -74,39 +78,38 @@
     >>> payment.party = customer
     >>> payment.amount = Decimal('42')
     >>> payment.description = 'Testing'
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
 
-    >>> _ = payment.click('stripe_checkout')
-    >>> checkout = Wizard('account.payment.stripe.checkout', [payment])
+    >>> checkout = payment.click('stripe_checkout')
     >>> bool(payment.stripe_checkout_id)
     True
 
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4000000000000259',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Payment.write([payment.id], {
     ...     'stripe_token': token.id,
     ...     'stripe_chargeable': True,
     ...     'stripe_payment_intent_id': None,  # Remove intent from checkout
     ...     }, config.context)
 
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> bool(payment.stripe_captured)
     True
 
@@ -167,39 +170,38 @@
     >>> payment.party = customer
     >>> payment.amount = Decimal('42')
     >>> payment.description = 'Testing'
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
 
-    >>> _ = payment.click('stripe_checkout')
-    >>> checkout = Wizard('account.payment.stripe.checkout', [payment])
+    >>> checkout = payment.click('stripe_checkout')
     >>> bool(payment.stripe_checkout_id)
     True
 
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4000000000000259',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Payment.write([payment.id], {
     ...     'stripe_token': token.id,
     ...     'stripe_chargeable': True,
     ...     'stripe_payment_intent_id': None,  # Remove intent from checkout
     ...     }, config.context)
 
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> bool(payment.stripe_captured)
     True
 
@@ -238,53 +240,52 @@
     >>> payment.party = customer
     >>> payment.amount = Decimal('42')
     >>> payment.description = 'Testing'
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
 
-    >>> _ = payment.click('stripe_checkout')
-    >>> checkout = Wizard('account.payment.stripe.checkout', [payment])
+    >>> checkout = payment.click('stripe_checkout')
     >>> bool(payment.stripe_checkout_id)
     True
 
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4000000000000259',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> Payment.write([payment.id], {
     ...     'stripe_token': token.id,
     ...     'stripe_chargeable': True,
     ...     'stripe_payment_intent_id': None,  # Remove intent from checkout
     ...     }, config.context)
 
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> bool(payment.stripe_captured)
     True
 
 Simulate charge.dispute.closed event::
 
     >>> charge = stripe.Charge.retrieve(payment.stripe_charge_id)
     >>> dispute = stripe.Dispute.modify(charge.dispute,
     ...     evidence={'uncategorized_text': 'winning_evidence'})
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> payment.amount
     Decimal('42.00')
     >>> payment.stripe_dispute_reason
```

### Comparing `trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe_identical.rst` & `trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe_identical.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     >>> import stripe
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
 
+    >>> today = dt.date.today()
+
 Activate modules::
 
     >>> config = activate_modules('account_payment_stripe')
 
     >>> Company = Model.get('company.company')
     >>> Cron = Model.get('ir.cron')
     >>> StripeAccount = Model.get('account.payment.stripe.account')
@@ -61,15 +63,15 @@
     >>> stripe_customer1.party = customer1
     >>> stripe_customer1.stripe_account = stripe_account
     >>> _ = stripe_customer1.click('stripe_checkout')
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4012888888881881',
     ...         'exp_month': 12,
-    ...         'exp_year': dt.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> StripeCustomer.write(
     ...     [stripe_customer1.id], {'stripe_token': token.id}, config.context)
 
 Run cron::
@@ -86,15 +88,15 @@
     >>> stripe_customer2.party = customer2
     >>> stripe_customer2.stripe_account = stripe_account
     >>> _ = stripe_customer2.click('stripe_checkout')
     >>> token = stripe.Token.create(
     ...     card={
     ...         'number': '4012888888881881',
     ...         'exp_month': 12,
-    ...         'exp_year': dt.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         },
     ...     )
     >>> StripeCustomer.write(
     ...     [stripe_customer2.id], {'stripe_token': token.id}, config.context)
 
 Run cron::
```

### Comparing `trytond_account_payment_stripe-6.6.2/tests/scenario_account_payment_stripe_intent.rst` & `trytond_account_payment_stripe-6.8.0/tests/scenario_account_payment_stripe_intent.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 ======================================
 Account Payment Stripe Intent Scenario
 ======================================
 
 Imports::
 
     >>> import os
-    >>> import datetime
+    >>> import datetime as dt
     >>> import time
     >>> from decimal import Decimal
     >>> import stripe
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
 
+    >>> today = dt.date.today()
+
+    >>> FETCH_SLEEP = 1
+
 Activate modules::
 
     >>> config = activate_modules('account_payment_stripe')
 
 Create company::
 
     >>> Company = Model.get('company.company')
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company)
+    >>> fiscalyear = create_fiscalyear(company, today)
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
 
 Create Stripe account::
@@ -76,15 +80,15 @@
 
     >>> _ = customer.click('stripe_checkout')
     >>> payment_method = stripe.PaymentMethod.create(
     ...     type='card',
     ...     card={
     ...         'number': '4000000000003055',
     ...         'exp_month': 12,
-    ...         'exp_year': datetime.date.today().year + 1,
+    ...         'exp_year': today.year + 1,
     ...         'cvc': '123',
     ...         })
     >>> setup_intent = stripe.SetupIntent.confirm(
     ...     customer.stripe_setup_intent_id,
     ...     payment_method=payment_method)
     >>> cron_update_intent, = Cron.find([
     ...     ('method', '=', 'account.payment.stripe.customer|stripe_intent_update'),
@@ -113,15 +117,15 @@
 Process off-session the payment::
 
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'succeeded'
     >>> bool(payment.stripe_captured)
     True
 
@@ -134,15 +138,15 @@
     >>> refund.click('submit')
     >>> refund.click('approve')
     >>> cron_refund_create, = Cron.find([
     ...     ('method', '=', 'account.payment.stripe.refund|stripe_create'),
     ...     ])
     >>> cron_refund_create.click('run_once')
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'failed'
 
 Cancel payment intent::
 
@@ -162,12 +166,12 @@
     >>> process_payment = Wizard('account.payment.process', [payment])
     >>> process_payment.execute('process')
     >>> payment.state
     'processing'
 
     >>> _ = stripe.PaymentIntent.cancel(payment.stripe_payment_intent_id)
 
-    >>> time.sleep(1)
+    >>> time.sleep(FETCH_SLEEP)
     >>> cron_fetch_events.click('run_once')
     >>> payment.reload()
     >>> payment.state
     'failed'
```

### Comparing `trytond_account_payment_stripe-6.6.2/tox.ini` & `trytond_account_payment_stripe-6.8.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/account_payment_stripe/* -m unittest discover -s tests
-    coverage report --include=./**/account_payment_stripe/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/PKG-INFO` & `trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-payment-stripe
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for Stripe payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_stripe
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment stripe
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
 
 Account Payment Stripe Module
 #############################
 
 The account_payment_stripe module allows to receive payment from `Stripe`_.
@@ -114,15 +114,15 @@
 
 .. _source: https://stripe.com/docs/sources
 .. _`payment method`: https://stripe.com/docs/payments/payment-methods
 
 Configuration
 *************
 
-The account_payment_stripe module uses the section `account_payment_stripe` to
-retrieve some parameters:
+The account_payment_stripe module uses the section ``account_payment_stripe``
+to retrieve some parameters:
 
-- `sources_cache`: defines the duration in seconds the sources are kept in the
-  cache. The default value is `15 * 60`.
+- ``sources_cache``: defines the duration in seconds the sources are kept in
+  the cache. The default value is ``15 * 60``.
 
-- `max_network_retries`: defines the maximum number of retries the Stripe
-  library may perform. The default value is `3`.
+- ``max_network_retries``: defines the maximum number of retries the Stripe
+  library may perform. The default value is ``3``.
```

### Comparing `trytond_account_payment_stripe-6.6.2/trytond_account_payment_stripe.egg-info/SOURCES.txt` & `trytond_account_payment_stripe-6.8.0/trytond_account_payment_stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/view/account_form.xml` & `trytond_account_payment_stripe-6.8.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/view/customer_form.xml` & `trytond_account_payment_stripe-6.8.0/view/customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/view/party_reception_direct_debit_form.xml` & `trytond_account_payment_stripe-6.8.0/view/party_reception_direct_debit_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/view/payment_form.xml` & `trytond_account_payment_stripe-6.8.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-6.6.2/view/refund_form.xml` & `trytond_account_payment_stripe-6.8.0/view/refund_form.xml`

 * *Files identical despite different names*

