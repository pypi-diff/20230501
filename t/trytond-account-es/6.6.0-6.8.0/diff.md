# Comparing `tmp/trytond_account_es-6.6.0.tar.gz` & `tmp/trytond_account_es-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es-6.6.0.tar", last modified: Mon Oct 31 16:22:41 2022, max compression
+gzip compressed data, was "trytond_account_es-6.8.0.tar", last modified: Mon May  1 11:36:57 2023, max compression
```

## Comparing `trytond_account_es-6.6.0.tar` & `trytond_account_es-6.8.0.tar`

### file list

```diff
@@ -1,106 +1,103 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:41.270555 trytond_account_es-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_es-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_es-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-31 16:22:39.000000 trytond_account_es-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_es-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1864 2022-10-31 16:22:39.000000 trytond_account_es-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2022-10-31 16:22:38.000000 trytond_account_es-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_es-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2382 2022-10-31 16:22:41.270555 trytond_account_es-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      929 2019-11-04 12:36:52.000000 trytond_account_es-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6178 2022-04-10 15:40:34.000000 trytond_account_es-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)   454573 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   417528 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/account_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1356 2022-04-10 15:40:34.000000 trytond_account_es-6.6.0/account_payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2020-02-22 17:31:05.000000 trytond_account_es-6.6.0/account_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   311163 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/account_pyme.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1186 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/aeat111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/aeat115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2022-04-21 16:32:34.000000 trytond_account_es-6.6.0/aeat303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1087 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/aeat347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/aeat349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/create_chart.xsl
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:41.267222 trytond_account_es-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      929 2019-11-04 12:36:52.000000 trytond_account_es-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:41.257221 trytond_account_es-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10593 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10727 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10656 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10242 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9321 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10537 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9119 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9682 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10407 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9020 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:33.000000 trytond_account_es-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2022-10-29 07:50:32.000000 trytond_account_es-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2019-10-11 23:09:47.000000 trytond_account_es-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2021-04-27 07:34:40.000000 trytond_account_es-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36550 2022-10-21 23:09:53.000000 trytond_account_es-6.6.0/reporting_tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12080 2021-04-27 07:35:27.000000 trytond_account_es-6.6.0/reporting_tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:22:41.270555 trytond_account_es-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4617 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   149065 2022-10-21 22:41:26.000000 trytond_account_es-6.6.0/tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1501 2020-10-08 07:32:41.000000 trytond_account_es-6.6.0/tax_groups.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   156737 2022-10-21 22:41:26.000000 trytond_account_es-6.6.0/tax_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   154545 2022-10-21 22:41:26.000000 trytond_account_es-6.6.0/tax_pyme.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:41.263888 trytond_account_es-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     1347 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/tests/111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/tests/115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2022-04-21 16:32:34.000000 trytond_account_es-6.6.0/tests/303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2022-04-21 16:32:34.000000 trytond_account_es-6.6.0/tests/303_compensate.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/tests/347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2022-04-27 09:23:00.000000 trytond_account_es-6.6.0/tests/349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_es-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4589 2021-02-27 09:39:44.000000 trytond_account_es-6.6.0/tests/scenario_ec_operation_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8621 2021-04-27 07:34:40.000000 trytond_account_es-6.6.0/tests/scenario_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4261 2021-10-30 15:16:00.000000 trytond_account_es-6.6.0/tests/scenario_reporting_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5349 2021-04-29 10:27:12.000000 trytond_account_es-6.6.0/tests/scenario_reporting_cancelled_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2021-02-21 18:19:37.000000 trytond_account_es-6.6.0/tests/scenario_reporting_compensate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4668 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/tests/scenario_reporting_surcharge_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-04-16 16:30:55.000000 trytond_account_es-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_es-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/tests/vat_book.csv
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-10-31 15:10:09.000000 trytond_account_es-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2022-10-31 16:22:37.000000 trytond_account_es-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:41.267222 trytond_account_es-6.6.0/trytond_account_es.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2382 2022-10-31 16:22:40.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3431 2022-10-31 16:22:41.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:22:40.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2022-10-31 16:22:40.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:49.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2022-10-31 16:22:40.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:22:40.000000 trytond_account_es-6.6.0/trytond_account_es.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:41.267222 trytond_account_es-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/view/es_ec_operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2020-04-12 21:04:56.000000 trytond_account_es-6.6.0/view/es_ec_operation_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2020-02-22 17:31:05.000000 trytond_account_es-6.6.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/view/print_aeat_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2019-10-11 23:09:47.000000 trytond_account_es-6.6.0/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2019-10-11 23:09:47.000000 trytond_account_es-6.6.0/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2021-04-27 07:34:40.000000 trytond_account_es-6.6.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2021-04-27 07:34:40.000000 trytond_account_es-6.6.0/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2021-04-27 07:34:40.000000 trytond_account_es-6.6.0/view/vat_book_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2021-04-27 07:34:40.000000 trytond_account_es-6.6.0/view/vat_book_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/view/vat_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2021-10-07 13:08:06.000000 trytond_account_es-6.6.0/view/vat_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2019-06-04 16:49:46.000000 trytond_account_es-6.6.0/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:57.025616 trytond_account_es-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2023-05-01 10:58:05.000000 trytond_account_es-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-05-01 10:58:05.000000 trytond_account_es-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2384 2023-05-01 11:36:57.025616 trytond_account_es-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   454573 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   417528 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/account_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1356 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/account_payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:14.000000 trytond_account_es-6.8.0/account_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   311163 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/account_pyme.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1186 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/aeat111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/aeat115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/aeat303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1087 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/aeat347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/aeat349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/create_chart.xsl
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:57.022282 trytond_account_es-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_es-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:57.012282 trytond_account_es-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10593 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10727 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10656 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10242 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9321 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10537 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9119 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9682 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10407 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9020 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2023-04-29 08:02:39.000000 trytond_account_es-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36721 2023-04-21 08:36:08.000000 trytond_account_es-6.8.0/reporting_tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12080 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/reporting_tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:36:57.025616 trytond_account_es-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3811 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   149065 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tax_groups.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   156737 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tax_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   154545 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tax_pyme.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:57.018949 trytond_account_es-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/tests/111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/tests/115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/303_compensate.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4589 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/scenario_ec_operation_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8625 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/scenario_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4268 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/scenario_reporting_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5349 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/scenario_reporting_cancelled_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4400 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/scenario_reporting_compensate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4672 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/scenario_reporting_surcharge_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tests/vat_book.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-05-01 10:57:59.000000 trytond_account_es-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:57.025616 trytond_account_es-6.8.0/trytond_account_es.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2384 2023-05-01 11:36:56.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3405 2023-05-01 11:36:56.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:36:56.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:36:56.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 11:36:56.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:36:56.000000 trytond_account_es-6.8.0/trytond_account_es.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:57.022282 trytond_account_es-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/es_ec_operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/es_ec_operation_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-01-16 14:00:20.000000 trytond_account_es-6.8.0/view/print_aeat_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/vat_book_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/vat_book_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/vat_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view/vat_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_account_es-6.8.0/view.xml
```

### Comparing `trytond_account_es-6.6.0/CHANGELOG` & `trytond_account_es-6.8.0/CHANGELOG`

 * *Files 16% similar despite different names*

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
 * Remove 61 tax code no more used in AEAT303
```

### Comparing `trytond_account_es-6.6.0/COPYRIGHT` & `trytond_account_es-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/LICENSE` & `trytond_account_es-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/PKG-INFO` & `trytond_account_es-6.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: trytond_account_es
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton with Spanish chart of accounts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_es
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart spanish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Spanish
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
 
 Spanish Account Module
 ######################
 
 The Spanish account module defines the following charts of account:
@@ -56,8 +56,8 @@
 thanks to the create_variant.xsl XSLT script. The script will produce on the
 standard output the desired XML file. The XSLT script can be launched with the
 following commands::
 
     xsltproc --stringparam chart <chart> create_chart.xsl account.xml
     xsltproc --stringparam chart <chart> create_chart.xsl tax.xml
 
-where ``chart`` is `normal` or `pyme`
+where ``chart`` is ``normal`` or ``pyme``.
```

### Comparing `trytond_account_es-6.6.0/README.rst` & `trytond_account_es-6.8.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 thanks to the create_variant.xsl XSLT script. The script will produce on the
 standard output the desired XML file. The XSLT script can be launched with the
 following commands::
 
     xsltproc --stringparam chart <chart> create_chart.xsl account.xml
     xsltproc --stringparam chart <chart> create_chart.xsl tax.xml
 
-where ``chart`` is `normal` or `pyme`
+where ``chart`` is ``normal`` or ``pyme``.
```

### Comparing `trytond_account_es-6.6.0/__init__.py` & `trytond_account_es-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/account.py` & `trytond_account_es-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/account.xml` & `trytond_account_es-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/account_normal.xml` & `trytond_account_es-6.8.0/account_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/account_payment.py` & `trytond_account_es-6.8.0/account_payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/account_payment.xml` & `trytond_account_es-6.8.0/account_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/account_pyme.xml` & `trytond_account_es-6.8.0/account_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/aeat111.txt` & `trytond_account_es-6.8.0/aeat111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/aeat303.txt` & `trytond_account_es-6.8.0/aeat303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/aeat347.txt` & `trytond_account_es-6.8.0/aeat347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/aeat349.txt` & `trytond_account_es-6.8.0/aeat349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/company.py` & `trytond_account_es-6.8.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/create_chart.xsl` & `trytond_account_es-6.8.0/create_chart.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/doc/index.rst` & `trytond_account_es-6.8.0/doc/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 thanks to the create_variant.xsl XSLT script. The script will produce on the
 standard output the desired XML file. The XSLT script can be launched with the
 following commands::
 
     xsltproc --stringparam chart <chart> create_chart.xsl account.xml
     xsltproc --stringparam chart <chart> create_chart.xsl tax.xml
 
-where ``chart`` is `normal` or `pyme`
+where ``chart`` is ``normal`` or ``pyme``.
```

### Comparing `trytond_account_es-6.6.0/locale/bg.po` & `trytond_account_es-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/ca.po` & `trytond_account_es-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/cs.po` & `trytond_account_es-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/de.po` & `trytond_account_es-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/es.po` & `trytond_account_es-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/es_419.po` & `trytond_account_es-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/et.po` & `trytond_account_es-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/fa.po` & `trytond_account_es-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/fi.po` & `trytond_account_es-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/fr.po` & `trytond_account_es-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/hu.po` & `trytond_account_es-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/id.po` & `trytond_account_es-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/it.po` & `trytond_account_es-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/lo.po` & `trytond_account_es-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/lt.po` & `trytond_account_es-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/nl.po` & `trytond_account_es-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/pl.po` & `trytond_account_es-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/pt.po` & `trytond_account_es-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/ro.po` & `trytond_account_es-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/ru.po` & `trytond_account_es-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/sl.po` & `trytond_account_es-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/tr.po` & `trytond_account_es-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/uk.po` & `trytond_account_es-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/locale/zh_CN.po` & `trytond_account_es-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/party.py` & `trytond_account_es-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/reporting_tax.py` & `trytond_account_es-6.8.0/reporting_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from sql import Literal, Null
 from sql.aggregate import Count, Min, Sum
 from sql.conditionals import Case, Coalesce
 from sql.functions import CurrentTimestamp, Extract
 from sql.operators import Exists
 
 from trytond.i18n import gettext
-from trytond.model import ModelSQL, ModelView, fields
-from trytond.model.modelsql import convert_from
+from trytond.model import ModelSQL, ModelView, convert_from, fields
+from trytond.modules.account.exceptions import FiscalYearNotFoundError
 from trytond.modules.account_eu.account import ECSalesList, ECSalesListContext
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Eval, If
 from trytond.report import Report
 from trytond.transaction import Transaction
 from trytond.wizard import (
@@ -752,16 +752,21 @@
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def default_fiscalyear(cls):
         pool = Pool()
-        Fiscalyear = pool.get('account.fiscalyear')
-        return Fiscalyear.find(cls.default_company(), exception=False)
+        FiscalYear = pool.get('account.fiscalyear')
+        try:
+            fiscalyear = FiscalYear.find(
+                cls.default_company(), test_state=False)
+        except FiscalYearNotFoundError:
+            return None
+        return fiscalyear.id
 
 
 class ESVATBook(ModelSQL, ModelView):
     "Spanish VAT Book"
     __name__ = 'account.reporting.vat_book_es'
 
     invoice = fields.Many2One('account.invoice', "Invoice")
```

### Comparing `trytond_account_es-6.6.0/reporting_tax.xml` & `trytond_account_es-6.8.0/reporting_tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/setup.py` & `trytond_account_es-6.8.0/setup.py`

 * *Files 22% similar despite different names*

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
 name = 'trytond_account_es'
 
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
 
 requires = ['python-sql >= 1.1.0', 'phonenumbers']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_account_asset'),
     get_require_version('trytond_account_payment_sepa'),
     get_require_version('trytond_sale_advance_payment'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton with Spanish chart of accounts',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_es',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account chart spanish',
     package_dir={'trytond.modules.account_es': '.'},
     packages=(
         ['trytond.modules.account_es']
         + ['trytond.modules.account_es.%s' % p for p in find_packages()]
         ),
@@ -109,28 +87,27 @@
         'Intended Audience :: Financial and Insurance Industry',
         'Intended Audience :: Legal Industry',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: Spanish',
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
     account_es = trytond.modules.account_es
     """,
     )
```

### Comparing `trytond_account_es-6.6.0/tax.xml` & `trytond_account_es-6.8.0/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tax_groups.xml` & `trytond_account_es-6.8.0/tax_groups.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tax_normal.xml` & `trytond_account_es-6.8.0/tax_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tax_pyme.xml` & `trytond_account_es-6.8.0/tax_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/111.txt` & `trytond_account_es-6.8.0/tests/111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/115.txt` & `trytond_account_es-6.8.0/tests/115.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/303.txt` & `trytond_account_es-6.8.0/tests/303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/303_compensate.txt` & `trytond_account_es-6.8.0/tests/303_compensate.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/347.txt` & `trytond_account_es-6.8.0/tests/347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/349.txt` & `trytond_account_es-6.8.0/tests/349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/scenario_ec_operation_list.rst` & `trytond_account_es-6.8.0/tests/scenario_ec_operation_list.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/scenario_reporting.rst` & `trytond_account_es-6.8.0/tests/scenario_reporting.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 =============================
 Account ES Reporting Scenario
 =============================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.tools import file_open
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts, create_fiscalyear)
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
@@ -29,15 +28,16 @@
     >>> tax_identifier.type = 'eu_vat'
     >>> tax_identifier.code = 'ESB01000009'
     >>> company.party.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, datetime.date(2018, 1, 1)))
+    ...     create_fiscalyear(
+    ...         company, (dt.date(2018, 1, 1), dt.date(2018, 12, 31))))
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company, 'account_es.pgc_0_pyme')
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_account_es-6.6.0/tests/scenario_reporting_alternate_currency.rst` & `trytond_account_es-6.8.0/tests/scenario_reporting_alternate_currency.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ================================================
 Account ES Reporting Alternate Currency Scenario
 ================================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.currency.tests.tools import get_currency
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts, create_fiscalyear)
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
@@ -27,15 +27,15 @@
     >>> eur = get_currency('EUR')
     >>> _ = create_company(currency=currency)
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company, 'account_es.pgc_0_pyme')
     >>> accounts = get_accounts(company)
     >>> expense = accounts['expense']
```

### Comparing `trytond_account_es-6.6.0/tests/scenario_reporting_cancelled_invoices.rst` & `trytond_account_es-6.8.0/tests/scenario_reporting_cancelled_invoices.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/tests/scenario_reporting_compensate.rst` & `trytond_account_es-6.8.0/tests/scenario_reporting_compensate.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 =========================================
 Account ES Compensated Reporting Scenario
 =========================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.tools import file_open
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts, create_fiscalyear)
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_es', 'account_invoice'])
 
 Create company::
 
@@ -29,15 +28,16 @@
     >>> tax_identifier.type = 'eu_vat'
     >>> tax_identifier.code = 'ESB01000009'
     >>> company.party.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, datetime.date(2018, 1, 1)))
+    ...     create_fiscalyear(
+    ...         company, (dt.date(2018, 1, 1), dt.date(2018, 12, 31))))
     >>> fiscalyear.click('create_period')
     >>> previous_period = fiscalyear.periods[0]
     >>> period = fiscalyear.periods[1]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company, 'account_es.pgc_0_pyme')
```

### Comparing `trytond_account_es-6.6.0/tests/scenario_reporting_surcharge_tax.rst` & `trytond_account_es-6.8.0/tests/scenario_reporting_surcharge_tax.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 ===========================================
 Account ES Reporting Surcharge Tax Scenario
 ===========================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.tools import file_open
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts, create_fiscalyear)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_es')
 
 Create company::
 
@@ -29,15 +28,16 @@
     >>> tax_identifier.type = 'eu_vat'
     >>> tax_identifier.code = 'ESB01000009'
     >>> company.party.save()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company, datetime.date(2020, 1, 1)))
+    ...     create_fiscalyear(
+    ...         company, (dt.date(2020, 1, 1), dt.date(2020, 12, 31))))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company, 'account_es.pgc_0_pyme')
     >>> accounts = get_accounts(company)
     >>> expense = accounts['expense']
```

### Comparing `trytond_account_es-6.6.0/trytond_account_es.egg-info/PKG-INFO` & `trytond_account_es-6.8.0/trytond_account_es.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: trytond-account-es
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton with Spanish chart of accounts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_es
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart spanish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Spanish
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
 
 Spanish Account Module
 ######################
 
 The Spanish account module defines the following charts of account:
@@ -56,8 +56,8 @@
 thanks to the create_variant.xsl XSLT script. The script will produce on the
 standard output the desired XML file. The XSLT script can be launched with the
 following commands::
 
     xsltproc --stringparam chart <chart> create_chart.xsl account.xml
     xsltproc --stringparam chart <chart> create_chart.xsl tax.xml
 
-where ``chart`` is `normal` or `pyme`
+where ``chart`` is ``normal`` or ``pyme``.
```

### Comparing `trytond_account_es-6.6.0/trytond_account_es.egg-info/SOURCES.txt` & `trytond_account_es-6.8.0/trytond_account_es.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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
@@ -107,14 +103,15 @@
 ./view/tax_code_template_form.xml
 ./view/tax_form.xml
 ./view/tax_template_form.xml
 ./view/vat_book_context_form.xml
 ./view/vat_book_list.xml
 ./view/vat_list_context_form.xml
 ./view/vat_list_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_es-6.6.0/view/tax_form.xml` & `trytond_account_es-6.8.0/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/view/tax_template_form.xml` & `trytond_account_es-6.8.0/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/view/vat_book_list.xml` & `trytond_account_es-6.8.0/view/vat_book_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/view/vat_list_list.xml` & `trytond_account_es-6.8.0/view/vat_list_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-6.6.0/view.xml` & `trytond_account_es-6.8.0/view.xml`

 * *Files identical despite different names*

