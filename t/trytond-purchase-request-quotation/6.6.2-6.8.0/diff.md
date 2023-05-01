# Comparing `tmp/trytond_purchase_request_quotation-6.6.2.tar.gz` & `tmp/trytond_purchase_request_quotation-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request_quotation-6.6.2.tar", last modified: Sun Feb  5 21:14:57 2023, max compression
+gzip compressed data, was "trytond_purchase_request_quotation-6.8.0.tar", last modified: Mon May  1 11:59:50 2023, max compression
```

## Comparing `trytond_purchase_request_quotation-6.6.2.tar` & `trytond_purchase_request_quotation-6.8.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:14:57.613456 trytond_purchase_request_quotation-6.6.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     1145 2023-02-05 21:14:54.000000 trytond_purchase_request_quotation-6.6.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-02-05 21:14:53.000000 trytond_purchase_request_quotation-6.6.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3439 2023-02-05 21:14:57.613456 trytond_purchase_request_quotation-6.6.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:14:57.610122 trytond_purchase_request_quotation-6.6.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:53.000000 trytond_purchase_request_quotation-6.6.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:14:57.606789 trytond_purchase_request_quotation-6.6.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9592 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9500 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9604 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7997 2022-12-19 12:02:53.000000 trytond_purchase_request_quotation-6.6.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9028 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10221 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9448 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8242 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8775 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:53.000000 trytond_purchase_request_quotation-6.6.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8474 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9360 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8033 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:53.000000 trytond_purchase_request_quotation-6.6.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7981 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8422 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23425 2023-02-05 20:48:28.000000 trytond_purchase_request_quotation-6.6.2/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11790 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1237 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    65125 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/quotation.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:14:57.613456 trytond_purchase_request_quotation-6.6.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4551 2022-12-19 12:02:53.000000 trytond_purchase_request_quotation-6.6.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:14:57.606789 trytond_purchase_request_quotation-6.6.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7773 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/tests/scenario_purchase_request_quotation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2023-01-02 22:41:13.000000 trytond_purchase_request_quotation-6.6.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:14:57.613456 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3439 2023-02-05 21:14:56.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-02-05 21:14:57.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:14:56.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-02-05 21:14:56.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:14:56.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-02-05 21:14:56.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:14:56.000000 trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:14:57.610122 trytond_purchase_request_quotation-6.6.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2022-12-19 12:02:54.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_create_ask_suppliers_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_create_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      980 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_line_list_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2022-12-19 12:02:50.000000 trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:50.522661 trytond_purchase_request_quotation-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-05-01 11:13:29.000000 trytond_purchase_request_quotation-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-05-01 11:13:28.000000 trytond_purchase_request_quotation-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3420 2023-05-01 11:59:50.522661 trytond_purchase_request_quotation-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:50.515994 trytond_purchase_request_quotation-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:50.512660 trytond_purchase_request_quotation-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9592 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9500 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9604 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7997 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9028 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10221 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9448 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8242 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8775 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8474 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9360 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8033 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7981 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8422 2023-04-29 08:02:49.000000 trytond_purchase_request_quotation-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    23419 2023-04-21 08:36:08.000000 trytond_purchase_request_quotation-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11790 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1237 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    65125 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/quotation.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:59:50.522661 trytond_purchase_request_quotation-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4489 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:50.512660 trytond_purchase_request_quotation-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7774 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/tests/scenario_purchase_request_quotation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2023-05-01 11:13:23.000000 trytond_purchase_request_quotation-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:50.519327 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3420 2023-05-01 11:59:49.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-05-01 11:59:50.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:59:49.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 11:59:49.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-05-01 11:59:49.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:59:49.000000 trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:50.515994 trytond_purchase_request_quotation-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_create_ask_suppliers_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-01-16 14:00:21.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_create_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      980 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_line_list_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_list.xml
```

### Comparing `trytond_purchase_request_quotation-6.6.2/CHANGELOG` & `trytond_purchase_request_quotation-6.8.0/CHANGELOG`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-Version 6.6.2 - 2023-02-05
---------------------------
-* Bug fixes (see mercurial logs for details)
 
-Version 6.6.1 - 2022-12-06
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

### Comparing `trytond_purchase_request_quotation-6.6.2/COPYRIGHT` & `trytond_purchase_request_quotation-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/LICENSE` & `trytond_purchase_request_quotation-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/PKG-INFO` & `trytond_purchase_request_quotation-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request_quotation
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for purchase request quotation
 Home-page: http://www.tryton.org
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_request_quotation
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase request for quotation
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
 
 Purchase Request For Quotation Module
 #####################################
 
 The Purchase Request for Quotation module allows users to ask quotations
```

### Comparing `trytond_purchase_request_quotation-6.6.2/README.rst` & `trytond_purchase_request_quotation-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/__init__.py` & `trytond_purchase_request_quotation-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/doc/conf.py` & `trytond_purchase_request_quotation-6.8.0/doc/conf.py`

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

### Comparing `trytond_purchase_request_quotation-6.6.2/doc/index.rst` & `trytond_purchase_request_quotation-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/bg.po` & `trytond_purchase_request_quotation-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/ca.po` & `trytond_purchase_request_quotation-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/cs.po` & `trytond_purchase_request_quotation-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/de.po` & `trytond_purchase_request_quotation-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/es.po` & `trytond_purchase_request_quotation-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/es_419.po` & `trytond_purchase_request_quotation-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/et.po` & `trytond_purchase_request_quotation-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/fa.po` & `trytond_purchase_request_quotation-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/fi.po` & `trytond_purchase_request_quotation-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/fr.po` & `trytond_purchase_request_quotation-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/hu.po` & `trytond_purchase_request_quotation-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/id.po` & `trytond_purchase_request_quotation-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/it.po` & `trytond_purchase_request_quotation-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/lo.po` & `trytond_purchase_request_quotation-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/lt.po` & `trytond_purchase_request_quotation-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/nl.po` & `trytond_purchase_request_quotation-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/pl.po` & `trytond_purchase_request_quotation-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/pt.po` & `trytond_purchase_request_quotation-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/ro.po` & `trytond_purchase_request_quotation-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/ru.po` & `trytond_purchase_request_quotation-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/sl.po` & `trytond_purchase_request_quotation-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/tr.po` & `trytond_purchase_request_quotation-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/uk.po` & `trytond_purchase_request_quotation-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/locale/zh_CN.po` & `trytond_purchase_request_quotation-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/purchase.py` & `trytond_purchase_request_quotation-6.8.0/purchase.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,16 +357,15 @@
             self.unit = self.request.uom
             if self.request.company:
                 self.currency = self.request.company.currency
             self.supply_date = self.request.supply_date or datetime.date.max
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @classmethod
     def get_quotation_state(cls):
         pool = Pool()
         Quotation = pool.get('purchase.request.quotation')
         return (Quotation.fields_get(
             ['state'])['state']['selection'])
```

### Comparing `trytond_purchase_request_quotation-6.6.2/purchase.xml` & `trytond_purchase_request_quotation-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/purchase_request.xml` & `trytond_purchase_request_quotation-6.8.0/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/quotation.fodt` & `trytond_purchase_request_quotation-6.8.0/quotation.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/setup.py` & `trytond_purchase_request_quotation-6.8.0/setup.py`

 * *Files 4% similar despite different names*

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
@@ -34,16 +31,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_request_quotation'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -53,23 +53,22 @@
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module for purchase request quotation',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": (
-            'https://hg.tryton.org/modules/purchase_request_quotation'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase request for quotation',
     package_dir={'trytond.modules.purchase_request_quotation': '.'},
     packages=(
         ['trytond.modules.purchase_request_quotation']
         + ['trytond.modules.purchase_request_quotation.%s' % p
             for p in find_packages()]
@@ -106,23 +105,23 @@
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

### Comparing `trytond_purchase_request_quotation-6.6.2/tests/scenario_purchase_request_quotation.rst` & `trytond_purchase_request_quotation-6.8.0/tests/scenario_purchase_request_quotation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 =======================================
 Purchase Request For Quotation Scenario
 =======================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_chart, get_accounts)
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate purchase_request_quotation Module::
 
     >>> config = activate_modules(['purchase_request_quotation',
     ...     'purchase_requisition'])
 
 Create company::
```

### Comparing `trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/PKG-INFO` & `trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-purchase-request-quotation
-Version: 6.6.2
+Version: 6.8.0
 Summary: Tryton module for purchase request quotation
 Home-page: http://www.tryton.org
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_request_quotation
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase request for quotation
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
 
 Purchase Request For Quotation Module
 #####################################
 
 The Purchase Request for Quotation module allows users to ask quotations
```

### Comparing `trytond_purchase_request_quotation-6.6.2/trytond_purchase_request_quotation.egg-info/SOURCES.txt` & `trytond_purchase_request_quotation-6.8.0/trytond_purchase_request_quotation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/view/purchase_request_form.xml` & `trytond_purchase_request_quotation-6.8.0/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_form.xml` & `trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-6.6.2/view/purchase_request_quotation_line_form.xml` & `trytond_purchase_request_quotation-6.8.0/view/purchase_request_quotation_line_form.xml`

 * *Files identical despite different names*

