# Comparing `tmp/trytond_marketing_campaign-6.6.1.tar.gz` & `tmp/trytond_marketing_campaign-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_campaign-6.6.1.tar", last modified: Sat Apr  1 22:21:29 2023, max compression
+gzip compressed data, was "trytond_marketing_campaign-6.8.0.tar", last modified: Mon May  1 11:37:07 2023, max compression
```

## Comparing `trytond_marketing_campaign-6.6.1.tar` & `trytond_marketing_campaign-6.8.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:21:29.791170 trytond_marketing_campaign-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      171 2023-04-01 22:21:25.000000 trytond_marketing_campaign-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-04-01 22:21:24.000000 trytond_marketing_campaign-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2445 2023-04-01 22:21:29.791170 trytond_marketing_campaign-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1801 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:21:29.784503 trytond_marketing_campaign-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      873 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/doc/reference.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:21:29.774503 trytond_marketing_campaign-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5142 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5264 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5127 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5167 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5056 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3866 2023-03-26 09:48:03.000000 trytond_marketing_campaign-6.6.1/marketing.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4266 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      839 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1123 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3500 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/sale_opportunity_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/sale_opportunity_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3805 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2071 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:21:29.791170 trytond_marketing_campaign-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4779 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:21:29.777836 trytond_marketing_campaign-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5296 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/tests/scenario_marketing_campaign_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2022-12-19 12:03:07.000000 trytond_marketing_campaign-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:21:29.791170 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2445 2023-04-01 22:21:28.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-04-01 22:21:29.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:21:28.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-04-01 22:21:28.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:21:28.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-04-01 22:21:28.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:21:28.000000 trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:21:29.784503 trytond_marketing_campaign-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/campaign_mixin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/parameter_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/parameter_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/sale_opportunity_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/sale_opportunity_reporting_marketing_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/sale_opportunity_reporting_marketing_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      637 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1009 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/sale_reporting_marketing_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2022-12-19 12:02:49.000000 trytond_marketing_campaign-6.6.1/view/sale_reporting_marketing_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:07.755749 trytond_marketing_campaign-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-05-01 10:58:11.000000 trytond_marketing_campaign-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:58:11.000000 trytond_marketing_campaign-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2434 2023-05-01 11:37:07.755749 trytond_marketing_campaign-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1801 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:07.752416 trytond_marketing_campaign-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      873 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/doc/reference.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:07.749082 trytond_marketing_campaign-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5142 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5264 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5127 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5167 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5056 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-04-29 08:02:39.000000 trytond_marketing_campaign-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3858 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/marketing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4266 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      839 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1123 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3500 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/sale_opportunity_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/sale_opportunity_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3805 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2071 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:37:07.755749 trytond_marketing_campaign-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4740 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:07.749082 trytond_marketing_campaign-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5296 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/tests/scenario_marketing_campaign_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-05-01 10:58:06.000000 trytond_marketing_campaign-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:07.755749 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2434 2023-05-01 11:37:06.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2493 2023-05-01 11:37:07.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:37:06.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:37:06.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-05-01 11:37:06.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:37:06.000000 trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:07.752416 trytond_marketing_campaign-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/campaign_mixin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/parameter_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/parameter_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/sale_opportunity_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/sale_opportunity_reporting_marketing_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/sale_opportunity_reporting_marketing_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      637 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1009 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/sale_reporting_marketing_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_marketing_campaign-6.8.0/view/sale_reporting_marketing_list.xml
```

### Comparing `trytond_marketing_campaign-6.6.1/COPYRIGHT` & `trytond_marketing_campaign-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/LICENSE` & `trytond_marketing_campaign-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/PKG-INFO` & `trytond_marketing_campaign-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_campaign
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to manage marketing campaign
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-marketing-campaign
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/marketing_campaign
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing campaign sale UTM
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
 
 #########################
 Marketing Campaign Module
 #########################
```

### Comparing `trytond_marketing_campaign-6.6.1/__init__.py` & `trytond_marketing_campaign-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/doc/conf.py` & `trytond_marketing_campaign-6.8.0/doc/conf.py`

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

### Comparing `trytond_marketing_campaign-6.6.1/doc/design.rst` & `trytond_marketing_campaign-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/doc/reference.rst` & `trytond_marketing_campaign-6.8.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/bg.po` & `trytond_marketing_campaign-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/ca.po` & `trytond_marketing_campaign-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/cs.po` & `trytond_marketing_campaign-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/de.po` & `trytond_marketing_campaign-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/es.po` & `trytond_marketing_campaign-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/es_419.po` & `trytond_marketing_campaign-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/et.po` & `trytond_marketing_campaign-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/fa.po` & `trytond_marketing_campaign-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/fi.po` & `trytond_marketing_campaign-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/fr.po` & `trytond_marketing_campaign-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/hu.po` & `trytond_marketing_campaign-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/id.po` & `trytond_marketing_campaign-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/it.po` & `trytond_marketing_campaign-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/lo.po` & `trytond_marketing_campaign-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/lt.po` & `trytond_marketing_campaign-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/nl.po` & `trytond_marketing_campaign-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/pl.po` & `trytond_marketing_campaign-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/pt.po` & `trytond_marketing_campaign-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/ro.po` & `trytond_marketing_campaign-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/ru.po` & `trytond_marketing_campaign-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/sl.po` & `trytond_marketing_campaign-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/tr.po` & `trytond_marketing_campaign-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/uk.po` & `trytond_marketing_campaign-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/locale/zh_CN.po` & `trytond_marketing_campaign-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/marketing.py` & `trytond_marketing_campaign-6.8.0/marketing.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from sql.functions import Lower
 from sql.operators import Equal
 
 from trytond.i18n import lazy_gettext
 from trytond.model import (
     DeactivableMixin, Exclude, Model, ModelSQL, ModelView, fields)
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 
 class Parameter(DeactivableMixin, ModelSQL, ModelView):
 
     name = fields.Char("Name", required=True)
 
     @classmethod
@@ -45,15 +45,15 @@
                 values['name'] = values['name'].lower()
             args.extend((parameters, values))
         super().write(*args)
 
     @classmethod
     def from_name(cls, name, create=True):
         name = name.strip().lower()
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             records = cls.search([
                     ('name', '=', name),
                     ])
         if records:
             record, = records
         elif create:
             record = cls(name=name)
```

### Comparing `trytond_marketing_campaign-6.6.1/marketing.xml` & `trytond_marketing_campaign-6.8.0/marketing.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/message.xml` & `trytond_marketing_campaign-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/sale.py` & `trytond_marketing_campaign-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/sale.xml` & `trytond_marketing_campaign-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/sale_opportunity_reporting.py` & `trytond_marketing_campaign-6.8.0/sale_opportunity_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/sale_opportunity_reporting.xml` & `trytond_marketing_campaign-6.8.0/sale_opportunity_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/sale_reporting.py` & `trytond_marketing_campaign-6.8.0/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/sale_reporting.xml` & `trytond_marketing_campaign-6.8.0/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/setup.py` & `trytond_marketing_campaign-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -37,16 +34,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_marketing_campaign'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -58,23 +58,23 @@
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module to manage marketing campaign',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-marketing-campaign'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/marketing_campaign',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton marketing campaign sale UTM',
     package_dir={'trytond.modules.marketing_campaign': '.'},
     packages=(
         ['trytond.modules.marketing_campaign']
         + ['trytond.modules.marketing_campaign.%s' % p
             for p in find_packages()]
@@ -112,23 +112,23 @@
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

### Comparing `trytond_marketing_campaign-6.6.1/tests/scenario_marketing_campaign_sale.rst` & `trytond_marketing_campaign-6.8.0/tests/scenario_marketing_campaign_sale.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/tox.ini` & `trytond_marketing_campaign-6.8.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/marketing_campaign/* -m unittest discover -s tests
-    coverage report --include=./**/marketing_campaign/* --omit=*/tests/*
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

### Comparing `trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/PKG-INFO` & `trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-marketing-campaign
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to manage marketing campaign
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-marketing-campaign
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/marketing_campaign
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing campaign sale UTM
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
 
 #########################
 Marketing Campaign Module
 #########################
```

### Comparing `trytond_marketing_campaign-6.6.1/trytond_marketing_campaign.egg-info/SOURCES.txt` & `trytond_marketing_campaign-6.8.0/trytond_marketing_campaign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/view/campaign_mixin_form.xml` & `trytond_marketing_campaign-6.8.0/view/campaign_mixin_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/view/sale_opportunity_reporting_context_form.xml` & `trytond_marketing_campaign-6.8.0/view/sale_opportunity_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/view/sale_opportunity_reporting_marketing_context_form.xml` & `trytond_marketing_campaign-6.8.0/view/sale_opportunity_reporting_marketing_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/view/sale_reporting_context_form.xml` & `trytond_marketing_campaign-6.8.0/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_campaign-6.6.1/view/sale_reporting_marketing_context_form.xml` & `trytond_marketing_campaign-6.8.0/view/sale_reporting_marketing_context_form.xml`

 * *Files identical despite different names*

