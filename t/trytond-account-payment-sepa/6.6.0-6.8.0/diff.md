# Comparing `tmp/trytond_account_payment_sepa-6.6.0.tar.gz` & `tmp/trytond_account_payment_sepa-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_sepa-6.6.0.tar", last modified: Mon Oct 31 16:14:10 2022, max compression
+gzip compressed data, was "trytond_account_payment_sepa-6.8.0.tar", last modified: Mon May  1 11:58:50 2023, max compression
```

## Comparing `trytond_account_payment_sepa-6.6.0.tar` & `trytond_account_payment_sepa-6.8.0.tar`

### file list

```diff
@@ -1,100 +1,97 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.116182 trytond_account_payment_sepa-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_payment_sepa-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_payment_sepa-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2022-10-31 16:14:08.000000 trytond_account_payment_sepa-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_payment_sepa-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2525 2022-10-31 16:14:08.000000 trytond_account_payment_sepa-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:14:07.000000 trytond_account_payment_sepa-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_payment_sepa-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2022-10-31 16:14:10.116182 trytond_account_payment_sepa-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1901 2020-06-04 11:08:32.000000 trytond_account_payment_sepa-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2021-12-11 16:59:32.000000 trytond_account_payment_sepa-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1948 2022-04-10 15:40:34.000000 trytond_account_payment_sepa-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1056 2019-10-11 23:09:47.000000 trytond_account_payment_sepa-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.112848 trytond_account_payment_sepa-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1901 2020-06-04 11:08:32.000000 trytond_account_payment_sepa-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      240 2019-10-11 23:09:47.000000 trytond_account_payment_sepa-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.109515 trytond_account_payment_sepa-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14910 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16985 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14377 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17220 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16868 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16064 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17244 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17008 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14691 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14237 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16454 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15217 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14491 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16939 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14648 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16059 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13793 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14999 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15868 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14360 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14512 2022-10-29 07:50:42.000000 trytond_account_payment_sepa-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81515 2021-10-30 15:16:00.000000 trytond_account_payment_sepa-6.6.0/mandate.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2022-04-11 21:47:59.000000 trytond_account_payment_sepa-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4832 2022-04-10 15:40:34.000000 trytond_account_payment_sepa-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2021-10-30 15:32:31.000000 trytond_account_payment_sepa-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    34267 2022-10-11 19:49:57.000000 trytond_account_payment_sepa-6.6.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15511 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4236 2022-10-11 19:45:04.000000 trytond_account_payment_sepa-6.6.0/sepa_handler.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:14:10.116182 trytond_account_payment_sepa-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5352 2022-10-29 07:39:10.000000 trytond_account_payment_sepa-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.109515 trytond_account_payment_sepa-6.6.0/template/
--rw-r--r--   0 ced       (1000) ced       (1000)     4112 2019-10-11 23:09:47.000000 trytond_account_payment_sepa-6.6.0/template/base.003.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2021-04-03 16:26:38.000000 trytond_account_payment_sepa-6.6.0/template/base.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4970 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/template/pain.001.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4356 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/template/pain.001.001.05.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3590 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/template/pain.001.003.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/template/pain.008.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4824 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/template/pain.008.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/template/pain.008.003.02.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.112848 trytond_account_payment_sepa-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2022-04-16 16:30:56.000000 trytond_account_payment_sepa-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.01.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    54092 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.01.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1394 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    63410 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.03.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    88101 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2159 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.04.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    86922 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/camt.054.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    44938 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/pain.001.001.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    45912 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/pain.001.001.05.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    19514 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/pain.001.003.03.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    43173 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/pain.008.001.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    44121 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/pain.008.001.04.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    25935 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/tests/pain.008.003.02.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    15710 2022-04-16 16:30:56.000000 trytond_account_payment_sepa-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2022-10-31 15:10:09.000000 trytond_account_payment_sepa-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2022-10-31 16:14:06.000000 trytond_account_payment_sepa-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.116182 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2022-10-31 16:14:09.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3426 2022-10-31 16:14:10.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:14:09.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2022-10-31 16:14:09.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:08.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2022-10-31 16:14:09.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:14:09.000000 trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:14:10.112848 trytond_account_payment_sepa-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2018-08-18 09:54:15.000000 trytond_account_payment_sepa-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2019-06-04 16:49:44.000000 trytond_account_payment_sepa-6.6.0/view/mandate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2019-10-11 23:09:47.000000 trytond_account_payment_sepa-6.6.0/view/mandate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2019-10-11 23:09:47.000000 trytond_account_payment_sepa-6.6.0/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2019-06-04 16:49:44.000000 trytond_account_payment_sepa-6.6.0/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2019-10-11 23:09:47.000000 trytond_account_payment_sepa-6.6.0/view/party_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2021-10-30 15:32:31.000000 trytond_account_payment_sepa-6.6.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1027 2020-02-03 23:04:29.000000 trytond_account_payment_sepa-6.6.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-04-10 15:39:30.000000 trytond_account_payment_sepa-6.6.0/view/payment_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.125244 trytond_account_payment_sepa-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2688 2023-05-01 11:12:50.000000 trytond_account_payment_sepa-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:12:50.000000 trytond_account_payment_sepa-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4200 2023-05-01 11:58:50.125244 trytond_account_payment_sepa-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1948 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1056 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.118578 trytond_account_payment_sepa-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      240 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.098577 trytond_account_payment_sepa-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14910 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16985 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14377 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17220 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16868 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16064 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17244 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17008 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14691 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14237 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16454 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15217 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14491 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16939 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14648 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16059 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13793 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14999 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15868 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14360 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2023-04-29 08:02:48.000000 trytond_account_payment_sepa-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14512 2023-04-29 08:02:49.000000 trytond_account_payment_sepa-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81515 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/mandate.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4832 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    34292 2023-04-21 08:36:08.000000 trytond_account_payment_sepa-6.8.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15511 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4236 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/sepa_handler.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:50.125244 trytond_account_payment_sepa-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4535 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.101911 trytond_account_payment_sepa-6.8.0/template/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4112 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/base.003.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/base.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4970 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.001.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4356 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.001.001.05.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3590 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.001.003.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.008.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4824 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.008.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/template/pain.008.003.02.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.115244 trytond_account_payment_sepa-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    54092 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1394 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    63410 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    88101 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2159 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    86922 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    44938 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.001.001.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    45912 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.001.001.05.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    19514 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.001.003.03.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    43173 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.008.001.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    44121 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.008.001.04.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    25935 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/tests/pain.008.003.02.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    15710 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-05-01 11:12:44.000000 trytond_account_payment_sepa-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.121911 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4200 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3400 2023-05-01 11:58:50.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:49.000000 trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:50.118578 trytond_account_payment_sepa-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/view/mandate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/mandate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-01-16 14:00:20.000000 trytond_account_payment_sepa-6.8.0/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/party_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1027 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_account_payment_sepa-6.8.0/view/payment_list.xml
```

### Comparing `trytond_account_payment_sepa-6.6.0/CHANGELOG` & `trytond_account_payment_sepa-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

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
 * Store sepa message id and sepa payment info id
```

### Comparing `trytond_account_payment_sepa-6.6.0/COPYRIGHT` & `trytond_account_payment_sepa-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_payment_sepa-6.6.0/LICENSE` & `trytond_account_payment_sepa-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/PKG-INFO` & `trytond_account_payment_sepa-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_sepa
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for SEPA payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_sepa
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment SEPA
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
 
 Account Payment SEPA Module
 ###########################
 
 The account_payment_sepa module allows to generate SEPA files for a Payment
@@ -84,15 +84,15 @@
   - Creditor
   - Shared
   - Service Level
 
 Group
 *****
 
-The Group has a field `SEPA Messages` containing the XML messages.
+The Group has a field ``SEPA Messages`` containing the XML messages.
 
 Mandate
 *******
 
 The Mandate stores information for the Direct Debit. It is mainly defined by:
 
 - Party.
@@ -131,22 +131,22 @@
 For incoming message camt.054, each booked entry will succeed the corresponding
 payment if any return information is found. Otherwise it will fail and the
 return reason will be stored on it.
 
 Party
 *****
 
-The Party has a field `SEPA Creditor Identifier` used for the party of the
+The Party has a field ``SEPA Creditor Identifier`` used for the party of the
 company.
 
 
 Configuration
 *************
 
-The account_payment_sepa module uses the section `account_payment_sepa` to
+The account_payment_sepa module uses the section ``account_payment_sepa`` to
 retrieve some parameters:
 
-- `filestore`: a boolean value to store SEPA message in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store SEPA message in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore. The default value is
-  `None`.
+- ``store_prefix``: the prefix to use with the FileStore. The default value is
+  ``None``.
```

### Comparing `trytond_account_payment_sepa-6.6.0/README.rst` & `trytond_account_payment_sepa-6.8.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   - Creditor
   - Shared
   - Service Level
 
 Group
 *****
 
-The Group has a field `SEPA Messages` containing the XML messages.
+The Group has a field ``SEPA Messages`` containing the XML messages.
 
 Mandate
 *******
 
 The Mandate stores information for the Direct Debit. It is mainly defined by:
 
 - Party.
@@ -76,22 +76,22 @@
 For incoming message camt.054, each booked entry will succeed the corresponding
 payment if any return information is found. Otherwise it will fail and the
 return reason will be stored on it.
 
 Party
 *****
 
-The Party has a field `SEPA Creditor Identifier` used for the party of the
+The Party has a field ``SEPA Creditor Identifier`` used for the party of the
 company.
 
 
 Configuration
 *************
 
-The account_payment_sepa module uses the section `account_payment_sepa` to
+The account_payment_sepa module uses the section ``account_payment_sepa`` to
 retrieve some parameters:
 
-- `filestore`: a boolean value to store SEPA message in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store SEPA message in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore. The default value is
-  `None`.
+- ``store_prefix``: the prefix to use with the FileStore. The default value is
+  ``None``.
```

### Comparing `trytond_account_payment_sepa-6.6.0/__init__.py` & `trytond_account_payment_sepa-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/account.py` & `trytond_account_payment_sepa-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/account.xml` & `trytond_account_payment_sepa-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/doc/index.rst` & `trytond_account_payment_sepa-6.8.0/doc/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   - Creditor
   - Shared
   - Service Level
 
 Group
 *****
 
-The Group has a field `SEPA Messages` containing the XML messages.
+The Group has a field ``SEPA Messages`` containing the XML messages.
 
 Mandate
 *******
 
 The Mandate stores information for the Direct Debit. It is mainly defined by:
 
 - Party.
@@ -76,22 +76,22 @@
 For incoming message camt.054, each booked entry will succeed the corresponding
 payment if any return information is found. Otherwise it will fail and the
 return reason will be stored on it.
 
 Party
 *****
 
-The Party has a field `SEPA Creditor Identifier` used for the party of the
+The Party has a field ``SEPA Creditor Identifier`` used for the party of the
 company.
 
 
 Configuration
 *************
 
-The account_payment_sepa module uses the section `account_payment_sepa` to
+The account_payment_sepa module uses the section ``account_payment_sepa`` to
 retrieve some parameters:
 
-- `filestore`: a boolean value to store SEPA message in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store SEPA message in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore. The default value is
-  `None`.
+- ``store_prefix``: the prefix to use with the FileStore. The default value is
+  ``None``.
```

### Comparing `trytond_account_payment_sepa-6.6.0/locale/bg.po` & `trytond_account_payment_sepa-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/ca.po` & `trytond_account_payment_sepa-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/cs.po` & `trytond_account_payment_sepa-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/de.po` & `trytond_account_payment_sepa-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/es.po` & `trytond_account_payment_sepa-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/es_419.po` & `trytond_account_payment_sepa-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/et.po` & `trytond_account_payment_sepa-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/fa.po` & `trytond_account_payment_sepa-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/fi.po` & `trytond_account_payment_sepa-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/fr.po` & `trytond_account_payment_sepa-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/hu.po` & `trytond_account_payment_sepa-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/id.po` & `trytond_account_payment_sepa-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/it.po` & `trytond_account_payment_sepa-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/lo.po` & `trytond_account_payment_sepa-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/lt.po` & `trytond_account_payment_sepa-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/nl.po` & `trytond_account_payment_sepa-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/pl.po` & `trytond_account_payment_sepa-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/pt.po` & `trytond_account_payment_sepa-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/ro.po` & `trytond_account_payment_sepa-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/ru.po` & `trytond_account_payment_sepa-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/sl.po` & `trytond_account_payment_sepa-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/tr.po` & `trytond_account_payment_sepa-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/uk.po` & `trytond_account_payment_sepa-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/locale/zh_CN.po` & `trytond_account_payment_sepa-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/mandate.fodt` & `trytond_account_payment_sepa-6.8.0/mandate.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/message.xml` & `trytond_account_payment_sepa-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/party.py` & `trytond_account_payment_sepa-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/party.xml` & `trytond_account_payment_sepa-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/payment.py` & `trytond_account_payment_sepa-6.8.0/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,16 +151,15 @@
         Company = pool.get('company.company')
         company_id = cls.default_company()
         if company_id:
             return Company(company_id).party.id
 
     @fields.depends('company')
     def on_change_with_company_party(self, name=None):
-        if self.company:
-            return self.company.party.id
+        return self.company.party if self.company else None
 
     @staticmethod
     def default_sepa_charge_bearer():
         return 'SLEV'
 
 
 def remove_comment(stream):
@@ -681,15 +680,15 @@
         default.setdefault('payments', [])
         default.setdefault('signature_date', None)
         default.setdefault('identification', None)
         return super(Mandate, cls).copy(mandates, default=default)
 
     @property
     def is_valid(self):
-        if self.state == 'validated':
+        if self.state == 'validated' and self.account_number.active:
             if self.type == 'one-off':
                 if not self.has_payments:
                     return True
             else:
                 return True
         return False
```

### Comparing `trytond_account_payment_sepa-6.6.0/payment.xml` & `trytond_account_payment_sepa-6.8.0/payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/sepa_handler.py` & `trytond_account_payment_sepa-6.8.0/sepa_handler.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/setup.py` & `trytond_account_payment_sepa-6.8.0/setup.py`

 * *Files 11% similar despite different names*

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
 name = 'trytond_account_payment_sepa'
 
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
 
 requires = ['Genshi', 'lxml', 'python-dateutil', 'python-stdnum >= 1.0']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = []
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module for SEPA payment',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_payment_sepa',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment SEPA',
     package_dir={'trytond.modules.account_payment_sepa': '.'},
     packages=(
         ['trytond.modules.account_payment_sepa']
         + ['trytond.modules.account_payment_sepa.%s' % p
             for p in find_packages()]
@@ -127,28 +104,27 @@
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
     account_payment_sepa = trytond.modules.account_payment_sepa
     """,
     )
```

### Comparing `trytond_account_payment_sepa-6.6.0/template/base.003.xml` & `trytond_account_payment_sepa-6.8.0/template/base.003.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/base.xml` & `trytond_account_payment_sepa-6.8.0/template/base.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/pain.001.001.03.xml` & `trytond_account_payment_sepa-6.8.0/template/pain.001.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/pain.001.001.05.xml` & `trytond_account_payment_sepa-6.8.0/template/pain.001.001.05.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/pain.001.003.03.xml` & `trytond_account_payment_sepa-6.8.0/template/pain.001.003.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/pain.008.001.02.xml` & `trytond_account_payment_sepa-6.8.0/template/pain.008.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/pain.008.001.04.xml` & `trytond_account_payment_sepa-6.8.0/template/pain.008.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/template/pain.008.003.02.xml` & `trytond_account_payment_sepa-6.8.0/template/pain.008.003.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.01.xml` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.01.xsd` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.01.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.02.xml` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.02.xsd` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.03.xml` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.03.xsd` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.04.xml` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/camt.054.001.04.xsd` & `trytond_account_payment_sepa-6.8.0/tests/camt.054.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/pain.001.001.03.xsd` & `trytond_account_payment_sepa-6.8.0/tests/pain.001.001.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/pain.001.001.05.xsd` & `trytond_account_payment_sepa-6.8.0/tests/pain.001.001.05.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/pain.001.003.03.xsd` & `trytond_account_payment_sepa-6.8.0/tests/pain.001.003.03.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/pain.008.001.02.xsd` & `trytond_account_payment_sepa-6.8.0/tests/pain.008.001.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/pain.008.001.04.xsd` & `trytond_account_payment_sepa-6.8.0/tests/pain.008.001.04.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/pain.008.003.02.xsd` & `trytond_account_payment_sepa-6.8.0/tests/pain.008.003.02.xsd`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/tests/test_module.py` & `trytond_account_payment_sepa-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/PKG-INFO` & `trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-payment-sepa
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for SEPA payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_sepa
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment SEPA
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
 
 Account Payment SEPA Module
 ###########################
 
 The account_payment_sepa module allows to generate SEPA files for a Payment
@@ -84,15 +84,15 @@
   - Creditor
   - Shared
   - Service Level
 
 Group
 *****
 
-The Group has a field `SEPA Messages` containing the XML messages.
+The Group has a field ``SEPA Messages`` containing the XML messages.
 
 Mandate
 *******
 
 The Mandate stores information for the Direct Debit. It is mainly defined by:
 
 - Party.
@@ -131,22 +131,22 @@
 For incoming message camt.054, each booked entry will succeed the corresponding
 payment if any return information is found. Otherwise it will fail and the
 return reason will be stored on it.
 
 Party
 *****
 
-The Party has a field `SEPA Creditor Identifier` used for the party of the
+The Party has a field ``SEPA Creditor Identifier`` used for the party of the
 company.
 
 
 Configuration
 *************
 
-The account_payment_sepa module uses the section `account_payment_sepa` to
+The account_payment_sepa module uses the section ``account_payment_sepa`` to
 retrieve some parameters:
 
-- `filestore`: a boolean value to store SEPA message in the FileStore.
-  The default value is `False`.
+- ``filestore``: a boolean value to store SEPA message in the FileStore.
+  The default value is ``False``.
 
-- `store_prefix`: the prefix to use with the FileStore. The default value is
-  `None`.
+- ``store_prefix``: the prefix to use with the FileStore. The default value is
+  ``None``.
```

### Comparing `trytond_account_payment_sepa-6.6.0/trytond_account_payment_sepa.egg-info/SOURCES.txt` & `trytond_account_payment_sepa-6.8.0/trytond_account_payment_sepa.egg-info/SOURCES.txt`

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
@@ -89,14 +85,15 @@
 ./view/party_identifier_form.xml
 ./view/party_reception_direct_debit_form.xml
 ./view/payment_form.xml
 ./view/payment_group_form.xml
 ./view/payment_group_list.xml
 ./view/payment_journal_form.xml
 ./view/payment_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_payment_sepa-6.6.0/view/mandate_form.xml` & `trytond_account_payment_sepa-6.8.0/view/mandate_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/view/message_form.xml` & `trytond_account_payment_sepa-6.8.0/view/message_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/view/payment_form.xml` & `trytond_account_payment_sepa-6.8.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa-6.6.0/view/payment_journal_form.xml` & `trytond_account_payment_sepa-6.8.0/view/payment_journal_form.xml`

 * *Files identical despite different names*

