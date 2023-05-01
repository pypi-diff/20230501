# Comparing `tmp/trytond_marketing_automation-6.6.2.tar.gz` & `tmp/trytond_marketing_automation-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_automation-6.6.2.tar", last modified: Sat Apr  1 22:22:36 2023, max compression
+gzip compressed data, was "trytond_marketing_automation-6.8.0.tar", last modified: Mon May  1 11:40:33 2023, max compression
```

## Comparing `trytond_marketing_automation-6.6.2.tar` & `trytond_marketing_automation-6.8.0.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:22:36.745236 trytond_marketing_automation-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-04-01 22:22:32.000000 trytond_marketing_automation-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-04-01 22:22:31.000000 trytond_marketing_automation-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4716 2023-04-01 22:22:36.745236 trytond_marketing_automation-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2448 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      865 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:22:36.741903 trytond_marketing_automation-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2448 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/empty.gif
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      590 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:22:36.731903 trytond_marketing_automation-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13679 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13528 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13802 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11771 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13654 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11017 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11641 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13437 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10898 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10870 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31958 2023-03-18 10:58:52.000000 trytond_marketing_automation-6.6.2/marketing_automation.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16627 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/marketing_automation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1574 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1683 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1305 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)      539 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:22:36.745236 trytond_marketing_automation-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4593 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:22:36.735236 trytond_marketing_automation-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/reminder.html
--rw-r--r--   0 ced       (1000) ced       (1000)     6467 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/scenario_marketing_automation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/scenario_marketing_automation_unsubscribable.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      177 2022-12-19 12:03:07.000000 trytond_marketing_automation-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:22:36.745236 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4716 2023-04-01 22:22:35.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2390 2023-04-01 22:22:36.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:22:35.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-04-01 22:22:35.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:22:35.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-04-01 22:22:35.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:22:35.000000 trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      554 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/unsubscribe.html
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:22:36.738570 trytond_marketing_automation-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/activity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/activity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/record_activity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/record_activity_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/record_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/record_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/scenario_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/view/scenario_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2022-12-19 12:02:49.000000 trytond_marketing_automation-6.6.2/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:33.841640 trytond_marketing_automation-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-05-01 11:00:29.000000 trytond_marketing_automation-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 11:00:29.000000 trytond_marketing_automation-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4733 2023-05-01 11:40:33.841640 trytond_marketing_automation-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2478 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      883 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:33.838307 trytond_marketing_automation-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2478 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/empty.gif
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1367 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:33.831640 trytond_marketing_automation-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13972 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13810 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14096 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12060 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13940 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11291 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11915 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13716 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11154 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11126 2023-04-30 10:46:36.000000 trytond_marketing_automation-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32458 2023-04-29 22:04:03.000000 trytond_marketing_automation-6.8.0/marketing_automation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16627 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/marketing_automation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1574 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1683 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      539 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:40:33.841640 trytond_marketing_automation-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4540 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:33.834973 trytond_marketing_automation-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/reminder.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     6808 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/scenario_marketing_automation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/scenario_marketing_automation_unsubscribable.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-05-01 11:00:24.000000 trytond_marketing_automation-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:33.841640 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4733 2023-05-01 11:40:32.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2454 2023-05-01 11:40:33.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:40:32.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:40:32.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-05-01 11:40:32.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:40:32.000000 trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      554 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/unsubscribe.html
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:33.838307 trytond_marketing_automation-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/activity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/activity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/ir_email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/record_activity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/record_activity_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/record_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/record_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/scenario_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/view/scenario_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-04-15 07:12:15.000000 trytond_marketing_automation-6.8.0/web.py
```

### Comparing `trytond_marketing_automation-6.6.2/CHANGELOG` & `trytond_marketing_automation-6.8.0/CHANGELOG`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
-Version 6.6.2 - 2023-04-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2022-11-17
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Archive emails sent
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow party to be unsubscribed from scenario
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_marketing_automation-6.6.2/COPYRIGHT` & `trytond_marketing_automation-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/LICENSE` & `trytond_marketing_automation-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/PKG-INFO` & `trytond_marketing_automation-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_automation
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module to plan, coordinate and manage marketing campaigns
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
-Project-URL: Source Code, https://hg.tryton.org/modules/marketing_automation
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing automation
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
 
 Marketing Automation Module
 ###########################
 
 The marketing_automation module allows marketing actions to be automated. It is
@@ -100,20 +100,20 @@
 -------
 
 Send E-Mail
 ...........
 
 The activity send an e-mail to the party defined on the record.
 The E-mail is composed using an HTML `Genshi <https://genshi.edgewall.org/>`_
-template with `record` in the evaluation context.
-All `<a>` elements have their `href` replaced by a shortened version used to
-trigger children activities. If the `href` value is `unsubscribe`, it is
+template with ``record`` in the evaluation context.
+All ``<a>`` elements have their ``href`` replaced by a shortened version used
+to trigger children activities. If the ``href`` value is ``unsubscribe``, it is
 replaced by the URL which allows the recipient to block their record for the
 scenario.
-A empty image is automatically added at the end of the `<body>` to track when
+A empty image is automatically added at the end of the ``<body>`` to track when
 emails are opened.
 
 Record
 ******
 
 It stores a reference to the records included in each scenario. If the record
 is blocked, no activity will be triggered for the record.
@@ -127,13 +127,14 @@
 due.
 
 Configuration
 *************
 
 The marketing_automation module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the email.
-    - `automation_base`: The base URL without a path for the unsubscribe URL
+    - ``email_from``: The default ``From`` for the email.
+    - ``automation_base``: The base URL without a path for the unsubscribe URL
       and the empty image.
-      The default value is created using the configuration `[web]` `hostname`.
+      The default value is created using the configuration ``[web]``
+      ``hostname``.
```

### Comparing `trytond_marketing_automation-6.6.2/README.rst` & `trytond_marketing_automation-6.8.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 -------
 
 Send E-Mail
 ...........
 
 The activity send an e-mail to the party defined on the record.
 The E-mail is composed using an HTML `Genshi <https://genshi.edgewall.org/>`_
-template with `record` in the evaluation context.
-All `<a>` elements have their `href` replaced by a shortened version used to
-trigger children activities. If the `href` value is `unsubscribe`, it is
+template with ``record`` in the evaluation context.
+All ``<a>`` elements have their ``href`` replaced by a shortened version used
+to trigger children activities. If the ``href`` value is ``unsubscribe``, it is
 replaced by the URL which allows the recipient to block their record for the
 scenario.
-A empty image is automatically added at the end of the `<body>` to track when
+A empty image is automatically added at the end of the ``<body>`` to track when
 emails are opened.
 
 Record
 ******
 
 It stores a reference to the records included in each scenario. If the record
 is blocked, no activity will be triggered for the record.
@@ -73,13 +73,14 @@
 due.
 
 Configuration
 *************
 
 The marketing_automation module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the email.
-    - `automation_base`: The base URL without a path for the unsubscribe URL
+    - ``email_from``: The default ``From`` for the email.
+    - ``automation_base``: The base URL without a path for the unsubscribe URL
       and the empty image.
-      The default value is created using the configuration `[web]` `hostname`.
+      The default value is created using the configuration ``[web]``
+      ``hostname``.
```

### Comparing `trytond_marketing_automation-6.6.2/__init__.py` & `trytond_marketing_automation-6.8.0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 __all__ = ['register', 'routes']
 
 
 def register():
     Pool.register(
         ir.Cron,
+        ir.Email,
         marketing_automation.Scenario,
         marketing_automation.Activity,
         marketing_automation.Record,
         marketing_automation.RecordActivity,
         party.Party,
         party.PartyUnsubscribedScenario,
         web.ShortenedURL,
```

### Comparing `trytond_marketing_automation-6.6.2/doc/conf.py` & `trytond_marketing_automation-6.8.0/doc/conf.py`

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

### Comparing `trytond_marketing_automation-6.6.2/doc/index.rst` & `trytond_marketing_automation-6.8.0/doc/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 -------
 
 Send E-Mail
 ...........
 
 The activity send an e-mail to the party defined on the record.
 The E-mail is composed using an HTML `Genshi <https://genshi.edgewall.org/>`_
-template with `record` in the evaluation context.
-All `<a>` elements have their `href` replaced by a shortened version used to
-trigger children activities. If the `href` value is `unsubscribe`, it is
+template with ``record`` in the evaluation context.
+All ``<a>`` elements have their ``href`` replaced by a shortened version used
+to trigger children activities. If the ``href`` value is ``unsubscribe``, it is
 replaced by the URL which allows the recipient to block their record for the
 scenario.
-A empty image is automatically added at the end of the `<body>` to track when
+A empty image is automatically added at the end of the ``<body>`` to track when
 emails are opened.
 
 Record
 ******
 
 It stores a reference to the records included in each scenario. If the record
 is blocked, no activity will be triggered for the record.
@@ -73,13 +73,14 @@
 due.
 
 Configuration
 *************
 
 The marketing_automation module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the email.
-    - `automation_base`: The base URL without a path for the unsubscribe URL
+    - ``email_from``: The default ``From`` for the email.
+    - ``automation_base``: The base URL without a path for the unsubscribe URL
       and the empty image.
-      The default value is created using the configuration `[web]` `hostname`.
+      The default value is created using the configuration ``[web]``
+      ``hostname``.
```

### Comparing `trytond_marketing_automation-6.6.2/locale/bg.po` & `trytond_marketing_automation-6.8.0/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/ca.po` & `trytond_marketing_automation-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Activitat"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr "Registre"
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Acció"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Fills"
@@ -212,14 +220,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr "Si es marca els tercer també es de-suscribeixen de l'escenari."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Activitats"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr "Correus electrònics"
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr "Activitats del registre"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Registres"
```

### Comparing `trytond_marketing_automation-6.6.2/locale/cs.po` & `trytond_marketing_automation-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/de.po` & `trytond_marketing_automation-6.8.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Aktivität"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr "Datensatz"
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Aktion"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Untergeordnet"
@@ -213,14 +221,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr "Wenn ausgewählt, dann werden Parteien auch vom Szenario abgemeldet."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Aktivitäten"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr "E-Mails"
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr "Datensatzaktivitäten"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Datensätze"
```

### Comparing `trytond_marketing_automation-6.6.2/locale/es.po` & `trytond_marketing_automation-6.8.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Actividad"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr "Registro"
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Acción"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Hijos"
@@ -213,14 +221,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr "Si se marca los terceros también se de-suscriben del escenario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Actividades"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr "Correos electrónicos"
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr "Registro de actividades"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Registros"
```

### Comparing `trytond_marketing_automation-6.6.2/locale/es_419.po` & `trytond_marketing_automation-6.8.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/et.po` & `trytond_marketing_automation-6.8.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Aktiviteet"
+
+#, fuzzy
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr "Kirje"
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Toiming"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Alamjaotus"
@@ -205,14 +215,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Aktiviteedid"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr "Kirje aktiviteedid"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Kirjed"
```

### Comparing `trytond_marketing_automation-6.6.2/locale/fa.po` & `trytond_marketing_automation-6.8.0/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/fi.po` & `trytond_marketing_automation-6.8.0/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/fr.po` & `trytond_marketing_automation-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Activité"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr "Enregistrement"
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Action"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Enfants"
@@ -215,14 +223,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr "Si cochée, les tiers sont également désabonnées du scénario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Activés"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr "E-mails"
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr "Enregistrements d'activités"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Enregistrements"
```

### Comparing `trytond_marketing_automation-6.6.2/locale/hu.po` & `trytond_marketing_automation-6.8.0/locale/hu.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/id.po` & `trytond_marketing_automation-6.8.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Aktivitas"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Tindakan"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Cabang"
@@ -203,14 +212,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/it.po` & `trytond_marketing_automation-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Attività"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Azione"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Figlio"
@@ -208,14 +217,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Attività"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/lo.po` & `trytond_marketing_automation-6.8.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/lt.po` & `trytond_marketing_automation-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/nl.po` & `trytond_marketing_automation-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr "Activiteit"
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr "Record"
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Actie"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Onderliggende niveaus"
@@ -216,14 +224,18 @@
 msgstr ""
 "Indien aangevinkt worden de relaties ook uitgeschreven uit het scenario."
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr "Activiteiten"
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr "E-mails"
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr "Activiteiten opnemen"
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr "Records"
```

### Comparing `trytond_marketing_automation-6.6.2/locale/pl.po` & `trytond_marketing_automation-6.8.0/locale/pl.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/pt.po` & `trytond_marketing_automation-6.8.0/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/ro.po` & `trytond_marketing_automation-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr "Acțiune"
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr "Copii"
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/ru.po` & `trytond_marketing_automation-6.8.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/sl.po` & `trytond_marketing_automation-6.8.0/locale/sl.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/tr.po` & `trytond_marketing_automation-6.8.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/uk.po` & `trytond_marketing_automation-6.8.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/locale/zh_CN.po` & `trytond_marketing_automation-6.8.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,marketing_automation_activity:"
+msgid "Activity"
+msgstr ""
+
+msgctxt "field:ir.email,marketing_automation_record:"
+msgid "Record"
+msgstr ""
+
 msgctxt "field:marketing.automation.activity,action:"
 msgid "Action"
 msgstr ""
 
 msgctxt "field:marketing.automation.activity,children:"
 msgid "Children"
 msgstr ""
@@ -203,14 +211,18 @@
 msgid "If checked parties are also unsubscribed from the scenario."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_activity_tree"
 msgid "Activities"
 msgstr ""
 
+msgctxt "model:ir.action,name:act_ir_email_form_relate_activity"
+msgid "E-mails"
+msgstr ""
+
 msgctxt "model:ir.action,name:act_record_activity_form"
 msgid "Record Activities"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_record_form"
 msgid "Records"
 msgstr ""
```

### Comparing `trytond_marketing_automation-6.6.2/marketing_automation.py` & `trytond_marketing_automation-6.8.0/marketing_automation.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
     EvalEnvironment, Index, ModelSQL, ModelView, Unique, Workflow, dualmethod,
     fields)
 from trytond.pool import Pool
-from trytond.pyson import Eval, If, PYSONDecoder
+from trytond.pyson import Eval, If, PYSONDecoder, TimeDelta
 from trytond.report import Report
 from trytond.sendmail import SMTPDataManager, sendmail_transactional
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.tools.email_ import set_from_header
 from trytond.transaction import Transaction
 from trytond.url import http_host
 from trytond.wsgi import Base64Converter
@@ -299,14 +299,18 @@
     condition = fields.Char("Condition",
         help="The PYSON statement that the record must match "
         "in order to execute the activity.\n"
         'The record is represented by "self".')
 
     delay = fields.TimeDelta(
         "Delay",
+        domain=['OR',
+            ('delay', '=', None),
+            ('delay', '>=', TimeDelta()),
+            ],
         states={
             'required': Eval('negative', False),
             },
         help="After how much time the action should be executed.")
 
     action = fields.Selection([
             (None, ''),
@@ -527,14 +531,15 @@
                 contact.name or party.rec_name,
                 contact.email)
 
     def execute_send_email(
             self, record_activity, smtpd_datamanager=None, **kwargs):
         pool = Pool()
         WebShortener = pool.get('web.shortened_url')
+        Email = pool.get('ir.email')
         record = record_activity.record
 
         with Transaction().set_context(language=record.language):
             record = record.__class__(record.id)
             translated = self.__class__(self.id)
 
         to = self._email_recipient(record.record)
@@ -611,14 +616,24 @@
         msg.attach(part)
 
         to_addrs = [a for _, a in getaddresses([to])]
         if to_addrs:
             sendmail_transactional(
                 from_, to_addrs, msg, datamanager=smtpd_datamanager)
 
+            email = Email(
+                recipients=to,
+                addresses=[{'address': a} for a in to_addrs],
+                subject=title,
+                resource=record.record,
+                marketing_automation_activity=self,
+                marketing_automation_record=record,
+                )
+            email.save()
+
     def email_context(self, record):
         return {
             'record': record.record,
             'format_date': Report.format_date,
             'format_datetime': Report.format_datetime,
             'format_timedelta': Report.format_timedelta,
             'format_currency': Report.format_currency,
```

### Comparing `trytond_marketing_automation-6.6.2/marketing_automation.xml` & `trytond_marketing_automation-6.8.0/marketing_automation.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/message.xml` & `trytond_marketing_automation-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/mixin.py` & `trytond_marketing_automation-6.8.0/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/party.py` & `trytond_marketing_automation-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/routes.py` & `trytond_marketing_automation-6.8.0/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from werkzeug.utils import redirect
-from werkzeug.wrappers import Response
 
-from trytond.protocols.wrappers import with_pool, with_transaction
+from trytond.protocols.wrappers import (
+    Response, redirect, with_pool, with_transaction)
 from trytond.tools import file_open
 from trytond.transaction import Transaction
 from trytond.wsgi import app
 
 
 @app.route('/m/<base64:database_name>/unsubscribe')
 @with_pool
```

### Comparing `trytond_marketing_automation-6.6.2/sale.py` & `trytond_marketing_automation-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/setup.py` & `trytond_marketing_automation-6.8.0/setup.py`

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
@@ -34,18 +31,21 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_marketing_automation'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
-requires = ['werkzeug', 'Genshi']
+requires = ['Genshi']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
@@ -53,22 +53,22 @@
 
 setup(name=name,
     version=version,
     description='Tryton module to plan, '
     'coordinate and manage marketing campaigns',
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
-        "Source Code": 'https://hg.tryton.org/modules/marketing_automation',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton marketing automation',
     package_dir={'trytond.modules.marketing_automation': '.'},
     packages=(
         ['trytond.modules.marketing_automation']
         + ['trytond.modules.marketing_automation.%s' % p
             for p in find_packages()]
@@ -107,23 +107,23 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_marketing_automation-6.6.2/tests/scenario_marketing_automation.rst` & `trytond_marketing_automation-6.8.0/tests/scenario_marketing_automation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     >>> manager = patch.object(
     ...     marketing_automation, 'SMTPDataManager').start()
 
 Activate modules::
 
     >>> config = activate_modules('marketing_automation')
 
+    >>> Email = Model.get('ir.email')
+
 Create a party::
 
     >>> Party = Model.get('party.party')
     >>> party = Party()
     >>> party.name = "Michael Scott"
     >>> contact = party.contact_mechanisms.new()
     >>> contact.type = 'email'
@@ -151,14 +153,26 @@
     >>> click_url.record == record_activity
     True
     >>> click_url.method
     'marketing.automation.record.activity|on_email_clicked'
     >>> record.uuid in msg
     True
 
+    >>> email, = Email.find([])
+    >>> email.recipients
+    'Michael Scott <michael@example.com>'
+    >>> email.subject
+    'Hello'
+    >>> email.resource == party
+    True
+    >>> email.marketing_automation_activity == root_activity
+    True
+    >>> bool(email.marketing_automation_record)
+    True
+
 Trigger open email and reminder after delay::
 
     >>> record_activity.click('on_email_opened')
 
     >>> open_activity, = RecordActivity.find([
     ...         ('record', '=', record.id),
     ...         ('activity', '=', email_opened.id),
```

### Comparing `trytond_marketing_automation-6.6.2/tests/scenario_marketing_automation_unsubscribable.rst` & `trytond_marketing_automation-6.8.0/tests/scenario_marketing_automation_unsubscribable.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/PKG-INFO` & `trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-marketing-automation
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module to plan, coordinate and manage marketing campaigns
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
-Project-URL: Source Code, https://hg.tryton.org/modules/marketing_automation
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing automation
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
 
 Marketing Automation Module
 ###########################
 
 The marketing_automation module allows marketing actions to be automated. It is
@@ -100,20 +100,20 @@
 -------
 
 Send E-Mail
 ...........
 
 The activity send an e-mail to the party defined on the record.
 The E-mail is composed using an HTML `Genshi <https://genshi.edgewall.org/>`_
-template with `record` in the evaluation context.
-All `<a>` elements have their `href` replaced by a shortened version used to
-trigger children activities. If the `href` value is `unsubscribe`, it is
+template with ``record`` in the evaluation context.
+All ``<a>`` elements have their ``href`` replaced by a shortened version used
+to trigger children activities. If the ``href`` value is ``unsubscribe``, it is
 replaced by the URL which allows the recipient to block their record for the
 scenario.
-A empty image is automatically added at the end of the `<body>` to track when
+A empty image is automatically added at the end of the ``<body>`` to track when
 emails are opened.
 
 Record
 ******
 
 It stores a reference to the records included in each scenario. If the record
 is blocked, no activity will be triggered for the record.
@@ -127,13 +127,14 @@
 due.
 
 Configuration
 *************
 
 The marketing_automation module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the email.
-    - `automation_base`: The base URL without a path for the unsubscribe URL
+    - ``email_from``: The default ``From`` for the email.
+    - ``automation_base``: The base URL without a path for the unsubscribe URL
       and the empty image.
-      The default value is created using the configuration `[web]` `hostname`.
+      The default value is created using the configuration ``[web]``
+      ``hostname``.
```

### Comparing `trytond_marketing_automation-6.6.2/trytond_marketing_automation.egg-info/SOURCES.txt` & `trytond_marketing_automation-6.8.0/trytond_marketing_automation.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 empty.gif
 exceptions.py
 ir.py
+ir.xml
 marketing_automation.py
 marketing_automation.xml
 message.xml
 mixin.py
 party.py
 party.xml
 routes.py
@@ -20,14 +21,15 @@
 tryton.cfg
 unsubscribe.html
 web.py
 ./__init__.py
 ./empty.gif
 ./exceptions.py
 ./ir.py
+./ir.xml
 ./marketing_automation.py
 ./marketing_automation.xml
 ./message.xml
 ./mixin.py
 ./party.py
 ./party.xml
 ./routes.py
@@ -64,14 +66,15 @@
 ./tests/reminder.html
 ./tests/scenario_marketing_automation.rst
 ./tests/scenario_marketing_automation_unsubscribable.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/activity_form.xml
 ./view/activity_tree.xml
+./view/ir_email_form.xml
 ./view/party_form.xml
 ./view/record_activity_form.xml
 ./view/record_activity_list.xml
 ./view/record_form.xml
 ./view/record_list.xml
 ./view/scenario_form.xml
 ./view/scenario_list.xml
@@ -113,14 +116,15 @@
 trytond_marketing_automation.egg-info/dependency_links.txt
 trytond_marketing_automation.egg-info/entry_points.txt
 trytond_marketing_automation.egg-info/not-zip-safe
 trytond_marketing_automation.egg-info/requires.txt
 trytond_marketing_automation.egg-info/top_level.txt
 view/activity_form.xml
 view/activity_tree.xml
+view/ir_email_form.xml
 view/party_form.xml
 view/record_activity_form.xml
 view/record_activity_list.xml
 view/record_form.xml
 view/record_list.xml
 view/scenario_form.xml
 view/scenario_list.xml
```

### Comparing `trytond_marketing_automation-6.6.2/unsubscribe.html` & `trytond_marketing_automation-6.8.0/unsubscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/view/activity_form.xml` & `trytond_marketing_automation-6.8.0/view/activity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/view/record_activity_form.xml` & `trytond_marketing_automation-6.8.0/view/record_activity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/view/scenario_form.xml` & `trytond_marketing_automation-6.8.0/view/scenario_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_automation-6.6.2/web.py` & `trytond_marketing_automation-6.8.0/web.py`

 * *Files identical despite different names*

