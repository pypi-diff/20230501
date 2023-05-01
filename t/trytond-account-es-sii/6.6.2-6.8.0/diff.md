# Comparing `tmp/trytond_account_es_sii-6.6.2.tar.gz` & `tmp/trytond_account_es_sii-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es_sii-6.6.2.tar", last modified: Sat Mar  4 12:26:16 2023, max compression
+gzip compressed data, was "trytond_account_es_sii-6.8.0.tar", last modified: Mon May  1 11:42:26 2023, max compression
```

## Comparing `trytond_account_es_sii-6.6.2.tar` & `trytond_account_es_sii-6.8.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:26:16.658896 trytond_account_es_sii-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-03-04 12:26:10.000000 trytond_account_es_sii-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2023-03-04 12:26:09.000000 trytond_account_es_sii-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-03-04 12:26:16.655563 trytond_account_es_sii-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23375 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5887 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:26:16.642229 trytond_account_es_sii-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1056 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:26:16.618896 trytond_account_es_sii-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5430 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5476 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5558 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4430 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5484 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4392 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1040 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      979 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 12:26:16.658896 trytond_account_es_sii-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4587 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12629 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:26:16.622229 trytond_account_es_sii-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21311 2023-02-27 17:29:14.000000 trytond_account_es_sii-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      135 2022-12-19 12:03:07.000000 trytond_account_es_sii-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:26:16.655563 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-03-04 12:26:15.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1816 2023-03-04 12:26:16.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:26:15.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-03-04 12:26:15.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:26:15.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      129 2023-03-04 12:26:15.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 12:26:15.000000 trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:26:16.632229 trytond_account_es_sii-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/invoice_sii_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      274 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/invoice_sii_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2022-12-19 12:02:49.000000 trytond_account_es_sii-6.6.2/view/tax_template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-05-01 11:01:46.000000 trytond_account_es_sii-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 11:01:45.000000 trytond_account_es_sii-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23865 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5887 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.029699 trytond_account_es_sii-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1085 2023-04-30 10:46:36.000000 trytond_account_es_sii-6.8.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.026365 trytond_account_es_sii-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5430 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5476 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5566 2023-04-30 10:46:36.000000 trytond_account_es_sii-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4430 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5484 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4392 2023-04-29 08:02:41.000000 trytond_account_es_sii-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      979 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4582 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12629 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.026365 trytond_account_es_sii-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2039 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    21334 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-28 07:46:16.000000 trytond_account_es_sii-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2023-05-01 11:01:40.000000 trytond_account_es_sii-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.033032 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1938 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:25.000000 trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:26.029699 trytond_account_es_sii-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/invoice_sii_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/invoice_sii_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-04-15 07:12:15.000000 trytond_account_es_sii-6.8.0/view/tax_template_form.xml
```

### Comparing `trytond_account_es_sii-6.6.2/LICENSE` & `trytond_account_es_sii-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/PKG-INFO` & `trytond_account_es_sii-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_es_sii
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module that sends invoices to the Spanish SII webservice
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_es_sii
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account sii spain
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
 
 ##########################
 Acounts Spanish SII Module
 ##########################
```

### Comparing `trytond_account_es_sii-6.6.2/__init__.py` & `trytond_account_es_sii-6.8.0/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,7 +16,10 @@
         account.Tax,
         account.FiscalYear,
         account.Period,
         account.Invoice,
         account.InvoiceSII,
         party.Identifier,
         module='account_es_sii', type_='model')
+    Pool.register(
+        account.RenewFiscalYear,
+        module='account_es_sii', type_='wizard')
```

### Comparing `trytond_account_es_sii-6.6.2/account.py` & `trytond_account_es_sii-6.8.0/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,28 @@
         periods = []
         for fiscalyear in fiscalyears:
             periods.extend(
                 p for p in fiscalyear.periods if p.type == 'standard')
         Period.write(periods, {name: value})
 
 
+class RenewFiscalYear(metaclass=PoolMeta):
+    __name__ = 'account.fiscalyear.renew'
+
+    def create_fiscalyear(self):
+        fiscalyear = super().create_fiscalyear()
+        previous_fiscalyear = self.start.previous_fiscalyear
+        periods = [
+            p for p in previous_fiscalyear.periods if p.type == 'standard']
+        if periods:
+            last_period = periods[-1]
+            fiscalyear.es_sii_send_invoices = last_period.es_sii_send_invoices
+        return fiscalyear
+
+
 class Period(metaclass=PoolMeta):
     __name__ = 'account.period'
     es_sii_send_invoices = fields.Boolean(
         "Send invoices to SII",
         states={
             'invisible': Eval('type') != 'standard',
             },
```

### Comparing `trytond_account_es_sii-6.6.2/account.xml` & `trytond_account_es_sii-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/doc/conf.py` & `trytond_account_es_sii-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_es_sii-6.6.2/doc/configuration.rst` & `trytond_account_es_sii-6.8.0/doc/configuration.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 .. warning::
     The private key must be unencrypted.
 
 How to obtain the certificate and private keys?
 -----------------------------------------------
 
 Both values should be extracted from the p12 certificate issued by the
-`FNMT <https://www.sede.fnmt.gob.es/certificados>`_.
+`FNMT <https://www.sede.fnmt.gob.es/certificados/certificado-de-representante>`_.
 The certificate should be related to the company presenting the information
 or an authorized party.
 
 Given a ``cert.p12`` certificate its keys can be extracted with following
 commands:
 
 .. code-block:: console
```

### Comparing `trytond_account_es_sii-6.6.2/doc/design.rst` & `trytond_account_es_sii-6.8.0/doc/design.rst`

 * *Files 8% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 When the invoice is correctly set it stores the secure validation code of
 the delivery.
 If there are any error with the invoice, the error code and description are
 stored.
 
 .. seealso::
 
-   The SSI Invoices can be foun by opening the main menu item:
+   The SSI Invoices can be found by opening the main menu item:
 
       |Financial --> Invoices --> SII Invoices|__
 
       .. |Financial --> Invoices --> SII Invoices| replace:: :menuselection:`Financial --> Invoices --> SII Invoices`
       __ https://demo.tryton.org/model/account.invoice.sii
```

### Comparing `trytond_account_es_sii-6.6.2/locale/bg.po` & `trytond_account_es_sii-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/ca.po` & `trytond_account_es_sii-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/cs.po` & `trytond_account_es_sii-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/de.po` & `trytond_account_es_sii-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/es.po` & `trytond_account_es_sii-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/es_419.po` & `trytond_account_es_sii-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/et.po` & `trytond_account_es_sii-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/fa.po` & `trytond_account_es_sii-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/fi.po` & `trytond_account_es_sii-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/fr.po` & `trytond_account_es_sii-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
 msgctxt "model:ir.message,text:msg_es_sii_posted_invoices"
 msgid ""
 "You can not change the SII setting for period \"%(period)s\" because there "
 "are already posted invoices."
 msgstr ""
 "Vous ne pouvez pas modifier le paramètre SII pour la période « %(period)s » "
-"car il y a déjà des factures postées."
+"car il y a déjà des factures comptabilisées."
 
 msgctxt "model:ir.message,text:msg_missing_sii_url"
 msgid ""
 "To send invoices to SII service, you need to set an URL on the account "
 "configuration."
 msgstr ""
 "Pour envoyer des factures au service SII, vous devez définir une URL dans la"
@@ -168,15 +168,15 @@
 
 msgctxt "selection:account.credential.sii,es_sii_environment:"
 msgid "Staging"
 msgstr "Staging"
 
 msgctxt "selection:account.invoice.sii,state:"
 msgid "Pending"
-msgstr "En attente"
+msgstr "En attentes"
 
 msgctxt "selection:account.invoice.sii,state:"
 msgid "Rejected"
 msgstr "Rejetée"
 
 msgctxt "selection:account.invoice.sii,state:"
 msgid "Sent"
```

### Comparing `trytond_account_es_sii-6.6.2/locale/hu.po` & `trytond_account_es_sii-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/id.po` & `trytond_account_es_sii-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/it.po` & `trytond_account_es_sii-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/lo.po` & `trytond_account_es_sii-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/lt.po` & `trytond_account_es_sii-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/nl.po` & `trytond_account_es_sii-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/pl.po` & `trytond_account_es_sii-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/pt.po` & `trytond_account_es_sii-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/ro.po` & `trytond_account_es_sii-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/ru.po` & `trytond_account_es_sii-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/sl.po` & `trytond_account_es_sii-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/tr.po` & `trytond_account_es_sii-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/uk.po` & `trytond_account_es_sii-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/locale/zh_CN.po` & `trytond_account_es_sii-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/message.xml` & `trytond_account_es_sii-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/party.py` & `trytond_account_es_sii-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/setup.py` & `trytond_account_es_sii-6.8.0/setup.py`

 * *Files 1% similar despite different names*

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
@@ -37,39 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_es_sii'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['zeep', 'requests']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = []
+tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module that sends invoices to the Spanish SII '
     'webservice',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_es_sii',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account sii spain',
     package_dir={'trytond.modules.account_es_sii': '.'},
     packages=(
         ['trytond.modules.account_es_sii']
         + ['trytond.modules.account_es_sii.%s' % p
             for p in find_packages()]
@@ -107,24 +107,24 @@
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

### Comparing `trytond_account_es_sii-6.6.2/tax.xml` & `trytond_account_es_sii-6.8.0/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/tests/test_module.py` & `trytond_account_es_sii-6.8.0/tests/test_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
             fiscalyear = set_invoice_sequences(get_fiscalyear(company))
             fiscalyear.save()
             FiscalYear.create_period([fiscalyear])
             fiscalyear.es_sii_send_invoices = True
             fiscalyear.save()
 
             currency = create_currency('gbp')
-            add_currency_rate(currency, 2)
+            add_currency_rate(currency, 2, fiscalyear.start_date)
 
             party = create_party('Customer', 'eu_vat', 'ES00000000T')
             tax, = Tax.search([
                     ('company', '=', company.id),
                     ('name', '=', 'IVA 21% (bienes)'),
                     ('group.kind', '=', 'sale'),
                     ])
```

### Comparing `trytond_account_es_sii-6.6.2/tox.ini` & `trytond_account_es_sii-6.8.0/tox.ini`

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
-    coverage run --include=./**/account_es_sii/* -m unittest discover -s tests
-    coverage report --include=./**/account_es_sii/* --omit=*/tests/*
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

### Comparing `trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/PKG-INFO` & `trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-es-sii
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module that sends invoices to the Spanish SII webservice
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_es_sii
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account sii spain
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
 
 ##########################
 Acounts Spanish SII Module
 ##########################
```

### Comparing `trytond_account_es_sii-6.6.2/trytond_account_es_sii.egg-info/SOURCES.txt` & `trytond_account_es_sii-6.8.0/trytond_account_es_sii.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 ./locale/ro.po
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
+./tests/scenario_renew_fiscalyear.rst
 ./tests/test_module.py
+./tests/test_scenario.py
 ./view/configuration_form.xml
 ./view/fiscalyear_form.xml
 ./view/invoice_sii_form.xml
 ./view/invoice_sii_list.xml
 ./view/period_form.xml
 ./view/tax_form.xml
 ./view/tax_template_form.xml
@@ -83,15 +85,17 @@
 locale/ro.po
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
+tests/scenario_renew_fiscalyear.rst
 tests/test_module.py
+tests/test_scenario.py
 trytond_account_es_sii.egg-info/PKG-INFO
 trytond_account_es_sii.egg-info/SOURCES.txt
 trytond_account_es_sii.egg-info/dependency_links.txt
 trytond_account_es_sii.egg-info/entry_points.txt
 trytond_account_es_sii.egg-info/not-zip-safe
 trytond_account_es_sii.egg-info/requires.txt
 trytond_account_es_sii.egg-info/top_level.txt
```

### Comparing `trytond_account_es_sii-6.6.2/view/tax_form.xml` & `trytond_account_es_sii-6.8.0/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es_sii-6.6.2/view/tax_template_form.xml` & `trytond_account_es_sii-6.8.0/view/tax_template_form.xml`

 * *Files identical despite different names*

