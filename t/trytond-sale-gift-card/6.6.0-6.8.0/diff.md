# Comparing `tmp/trytond_sale_gift_card-6.6.0.tar.gz` & `tmp/trytond_sale_gift_card-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_gift_card-6.6.0.tar", last modified: Mon Oct 31 16:16:49 2022, max compression
+gzip compressed data, was "trytond_sale_gift_card-6.8.0.tar", last modified: Mon May  1 11:43:45 2023, max compression
```

## Comparing `trytond_sale_gift_card-6.6.0.tar` & `trytond_sale_gift_card-6.8.0.tar`

### file list

```diff
@@ -1,87 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:49.968506 trytond_sale_gift_card-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:02.000000 trytond_sale_gift_card-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       41 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 16:16:48.000000 trytond_sale_gift_card-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_gift_card-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2022-10-31 16:16:47.000000 trytond_sale_gift_card-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:16:47.000000 trytond_sale_gift_card-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_gift_card-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2365 2022-10-31 16:16:49.968506 trytond_sale_gift_card-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      206 2022-10-27 11:24:45.000000 trytond_sale_gift_card-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2021-12-11 16:59:34.000000 trytond_sale_gift_card-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3420 2022-04-10 15:40:35.000000 trytond_sale_gift_card-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1081 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:49.965172 trytond_sale_gift_card-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      206 2022-10-27 11:24:45.000000 trytond_sale_gift_card-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:45.000000 trytond_sale_gift_card-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1042 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2021-05-16 16:13:13.000000 trytond_sale_gift_card-6.6.0/email.html
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30315 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/gift_card.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:49.961839 trytond_sale_gift_card-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7217 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7376 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7255 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7120 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5833 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5792 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6936 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2022-10-29 07:50:35.000000 trytond_sale_gift_card-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      803 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2459 2022-04-11 21:24:34.000000 trytond_sale_gift_card-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    17911 2022-10-11 19:49:58.000000 trytond_sale_gift_card-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7886 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:16:49.968506 trytond_sale_gift_card-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5355 2022-10-29 07:39:11.000000 trytond_sale_gift_card-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2009 2022-04-10 15:40:35.000000 trytond_sale_gift_card-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:49.965172 trytond_sale_gift_card-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_gift_card-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5456 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/tests/scenario_sale_gift_card.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3729 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/tests/scenario_sale_gift_card_goods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6184 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/tests/scenario_sale_point_gift_card.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2022-04-16 16:30:57.000000 trytond_sale_gift_card-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_gift_card-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2022-10-31 15:10:09.000000 trytond_sale_gift_card-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2022-10-31 16:16:46.000000 trytond_sale_gift_card-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:49.968506 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2365 2022-10-31 16:16:49.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2582 2022-10-31 16:16:49.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:16:49.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 16:16:49.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-05-03 13:57:50.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2022-10-31 16:16:49.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:16:49.000000 trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:49.965172 trytond_sale_gift_card-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      509 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/view/account_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2021-10-07 13:08:07.000000 trytond_sale_gift_card-6.6.0/view/gift_card_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-04-08 16:23:26.000000 trytond_sale_gift_card-6.6.0/view/gift_card_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-10-11 19:49:58.000000 trytond_sale_gift_card-6.6.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/view/sale_point_sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/view/sale_point_sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2021-10-30 15:32:32.000000 trytond_sale_gift_card-6.6.0/view/sale_point_sale_pay_gift_card_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2021-04-27 07:34:41.000000 trytond_sale_gift_card-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:45.257349 trytond_sale_gift_card-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-05-01 11:02:37.000000 trytond_sale_gift_card-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:02:36.000000 trytond_sale_gift_card-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2358 2023-05-01 11:43:45.257349 trytond_sale_gift_card-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3420 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:45.254015 trytond_sale_gift_card-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      206 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1042 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/email.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-29 22:04:03.000000 trytond_sale_gift_card-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30315 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/gift_card.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:45.247348 trytond_sale_gift_card-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7217 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7376 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7255 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7120 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5833 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5792 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6936 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-04-29 08:02:41.000000 trytond_sale_gift_card-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      803 2023-04-29 22:04:03.000000 trytond_sale_gift_card-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2459 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    17908 2023-04-29 22:04:03.000000 trytond_sale_gift_card-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7886 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:43:45.257349 trytond_sale_gift_card-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4545 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2009 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:45.250682 trytond_sale_gift_card-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5456 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tests/scenario_sale_gift_card.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3729 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tests/scenario_sale_gift_card_goods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6144 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tests/scenario_sale_point_gift_card.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-05-01 11:02:31.000000 trytond_sale_gift_card-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:45.257349 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2358 2023-05-01 11:43:44.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2544 2023-05-01 11:43:45.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:43:44.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:43:44.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 11:43:44.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:43:44.000000 trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:45.254015 trytond_sale_gift_card-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      509 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/account_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/gift_card_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/gift_card_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/sale_point_sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/sale_point_sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/sale_point_sale_pay_gift_card_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_gift_card-6.8.0/view/template_form.xml
```

### Comparing `trytond_sale_gift_card-6.6.0/COPYRIGHT` & `trytond_sale_gift_card-6.8.0/COPYRIGHT`

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

### Comparing `trytond_sale_gift_card-6.6.0/LICENSE` & `trytond_sale_gift_card-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/PKG-INFO` & `trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_sale_gift_card
-Version: 6.6.0
+Name: trytond-sale-gift-card
+Version: 6.8.0
 Summary: Tryton module to manage gift cards
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_gift_card
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale gift card
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
 
 #####################
 Sale Gift Card Module
 #####################
```

### Comparing `trytond_sale_gift_card-6.6.0/__init__.py` & `trytond_sale_gift_card-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/account.py` & `trytond_sale_gift_card-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/account.xml` & `trytond_sale_gift_card-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/doc/conf.py` & `trytond_sale_gift_card-6.8.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-modules_url = 'https://docs.tryton.org/projects/modules-{module}/en/{series}/'
-trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+import os
+
+base_url = os.environ.get('DOC_BASE_URL')
+if base_url:
+    modules_url = base_url + '/modules-{module}/'
+    trytond_url = base_url + '/server/'
+else:
+    modules_url = (
+        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
+    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
 
 
 def get_info():
     import configparser
-    import os
     import subprocess
     import sys
 
     module_dir = os.path.dirname(os.path.dirname(__file__))
 
     config = configparser.ConfigParser()
     config.read_file(open(os.path.join(module_dir, 'tryton.cfg')))
@@ -22,15 +29,18 @@
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
@@ -53,9 +63,10 @@
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
+linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
-del get_info, info, modules_url, trytond_url
+del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_sale_gift_card-6.6.0/doc/design.rst` & `trytond_sale_gift_card-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/doc/usage.rst` & `trytond_sale_gift_card-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/email.html` & `trytond_sale_gift_card-6.8.0/email.html`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/gift_card.fodt` & `trytond_sale_gift_card-6.8.0/gift_card.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/bg.po` & `trytond_sale_gift_card-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/ca.po` & `trytond_sale_gift_card-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/cs.po` & `trytond_sale_gift_card-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/de.po` & `trytond_sale_gift_card-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/es.po` & `trytond_sale_gift_card-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/es_419.po` & `trytond_sale_gift_card-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/et.po` & `trytond_sale_gift_card-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/fa.po` & `trytond_sale_gift_card-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/fi.po` & `trytond_sale_gift_card-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/fr.po` & `trytond_sale_gift_card-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/hu.po` & `trytond_sale_gift_card-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/id.po` & `trytond_sale_gift_card-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/it.po` & `trytond_sale_gift_card-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/lo.po` & `trytond_sale_gift_card-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/lt.po` & `trytond_sale_gift_card-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/nl.po` & `trytond_sale_gift_card-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/pl.po` & `trytond_sale_gift_card-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/pt.po` & `trytond_sale_gift_card-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/ro.po` & `trytond_sale_gift_card-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/ru.po` & `trytond_sale_gift_card-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/sl.po` & `trytond_sale_gift_card-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/tr.po` & `trytond_sale_gift_card-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/uk.po` & `trytond_sale_gift_card-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/locale/zh_CN.po` & `trytond_sale_gift_card-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/message.xml` & `trytond_sale_gift_card-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/product.py` & `trytond_sale_gift_card-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/sale.py` & `trytond_sale_gift_card-6.8.0/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,8 +548,8 @@
     currency = fields.Function(
         fields.Many2One('currency.currency', "Currency"),
         'on_change_with_currency')
 
     @fields.depends('sale')
     def on_change_with_currency(self, name=None):
         if self.sale and self.sale.company:
-            return self.sale.company.currency.id
+            return self.sale.company.currency
```

### Comparing `trytond_sale_gift_card-6.6.0/sale.xml` & `trytond_sale_gift_card-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/setup.py` & `trytond_sale_gift_card-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
@@ -37,63 +34,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_gift_card'
 
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
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_sale_point'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description="Tryton module to manage gift cards",
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_gift_card',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale gift card',
     package_dir={'trytond.modules.sale_gift_card': '.'},
     packages=(
         ['trytond.modules.sale_gift_card']
         + ['trytond.modules.sale_gift_card.%s' % p
             for p in find_packages()]
@@ -131,27 +109,26 @@
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
     sale_gift_card = trytond.modules.sale_gift_card
     """,  # noqa: E501
     )
```

### Comparing `trytond_sale_gift_card-6.6.0/stock.py` & `trytond_sale_gift_card-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/tests/scenario_sale_gift_card.rst` & `trytond_sale_gift_card-6.8.0/tests/scenario_sale_gift_card.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/tests/scenario_sale_gift_card_goods.rst` & `trytond_sale_gift_card-6.8.0/tests/scenario_sale_gift_card_goods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_gift_card-6.6.0/tests/scenario_sale_point_gift_card.rst` & `trytond_sale_gift_card-6.8.0/tests/scenario_sale_point_gift_card.rst`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     >>> line.quantity = 10
     >>> sale.save()
     >>> sale.total
     Decimal('500.00')
 
 Overpay::
 
-    >>> payment = Wizard('sale.point.sale.pay', [sale])
+    >>> payment = sale.click('pay')
     >>> payment.form.method = payment_method
     >>> payment.form.amount = Decimal('600.00')
     >>> payment.execute('pay')
 
     >>> payment.form.amount
     Decimal('-100.00')
 
@@ -197,15 +197,15 @@
     >>> sale.gift_cards.append(GiftCard(gift_card.id))
     >>> sale.save()
     >>> sale.total
     Decimal('150.00')
 
 Pay::
 
-    >>> payment = Wizard('sale.point.sale.pay', [sale])
+    >>> payment = sale.click('pay')
     >>> payment.form.method = payment_method
     >>> payment.execute('pay')
 
     >>> sale.state
     'done'
     >>> sale.total
     Decimal('150.00')
```

### Comparing `trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/PKG-INFO` & `trytond_sale_gift_card-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-sale-gift-card
-Version: 6.6.0
+Name: trytond_sale_gift_card
+Version: 6.8.0
 Summary: Tryton module to manage gift cards
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_gift_card
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale gift card
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
 
 #####################
 Sale Gift Card Module
 #####################
```

### Comparing `trytond_sale_gift_card-6.6.0/trytond_sale_gift_card.egg-info/SOURCES.txt` & `trytond_sale_gift_card-6.8.0/trytond_sale_gift_card.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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
```

### Comparing `trytond_sale_gift_card-6.6.0/view/gift_card_form.xml` & `trytond_sale_gift_card-6.8.0/view/gift_card_form.xml`

 * *Files identical despite different names*

