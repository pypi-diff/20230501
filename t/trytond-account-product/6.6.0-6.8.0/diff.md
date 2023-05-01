# Comparing `tmp/trytond_account_product-6.6.0.tar.gz` & `tmp/trytond_account_product-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_product-6.6.0.tar", last modified: Mon Oct 31 15:55:02 2022, max compression
+gzip compressed data, was "trytond_account_product-6.8.0.tar", last modified: Mon May  1 12:03:49 2023, max compression
```

## Comparing `trytond_account_product-6.6.0.tar` & `trytond_account_product-6.8.0.tar`

### file list

```diff
@@ -1,76 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:02.379494 trytond_account_product-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_account_product-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_product-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 15:55:00.000000 trytond_account_product-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_product-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     3724 2022-10-31 15:55:00.000000 trytond_account_product-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2022-10-31 15:54:59.000000 trytond_account_product-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:17.000000 trytond_account_product-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_product-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2612 2022-10-31 15:55:02.379494 trytond_account_product-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2022-10-27 11:24:44.000000 trytond_account_product-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      968 2021-12-11 16:59:32.000000 trytond_account_product-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3210 2022-04-10 15:40:34.000000 trytond_account_product-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2021-10-30 15:32:31.000000 trytond_account_product-6.6.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2022-04-10 15:40:34.000000 trytond_account_product-6.6.0/analytic_account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      827 2019-06-04 16:49:44.000000 trytond_account_product-6.6.0/analytic_account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2022-04-10 15:40:34.000000 trytond_account_product-6.6.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2019-06-04 16:49:44.000000 trytond_account_product-6.6.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:02.372827 trytond_account_product-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-01-05 17:22:47.000000 trytond_account_product-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1917 2022-04-08 16:27:20.000000 trytond_account_product-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2022-10-27 11:24:44.000000 trytond_account_product-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_account_product-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2021-01-05 17:22:47.000000 trytond_account_product-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2020-01-23 23:15:17.000000 trytond_account_product-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:02.372827 trytond_account_product-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6065 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6179 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2022-10-29 07:50:44.000000 trytond_account_product-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6165 2022-10-29 07:50:44.000000 trytond_account_product-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6211 2022-10-29 07:50:44.000000 trytond_account_product-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5275 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5923 2022-10-29 07:50:44.000000 trytond_account_product-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6770 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6243 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5845 2022-10-29 07:50:44.000000 trytond_account_product-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5142 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6158 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6253 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5034 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6486 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5050 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5950 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5963 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6209 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5809 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2022-10-29 07:50:44.000000 trytond_account_product-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4930 2022-10-29 07:50:45.000000 trytond_account_product-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2019-10-11 23:09:47.000000 trytond_account_product-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16220 2022-10-11 19:49:57.000000 trytond_account_product-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3202 2021-10-30 15:32:31.000000 trytond_account_product-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:55:02.379494 trytond_account_product-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5343 2022-10-29 07:39:10.000000 trytond_account_product-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:02.372827 trytond_account_product-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_product-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4093 2022-04-16 16:30:56.000000 trytond_account_product-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_account_product-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2022-10-31 15:54:58.000000 trytond_account_product-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:02.376161 trytond_account_product-6.6.0/trytond_account_product.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2612 2022-10-31 15:55:01.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2069 2022-10-31 15:55:02.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:55:01.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 15:55:01.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:14.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2022-10-31 15:55:01.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:55:01.000000 trytond_account_product-6.6.0/trytond_account_product.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:02.372827 trytond_account_product-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2019-06-04 16:49:44.000000 trytond_account_product-6.6.0/view/analytic_account_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-04-08 16:23:26.000000 trytond_account_product-6.6.0/view/analytic_account_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1262 2021-04-27 07:34:40.000000 trytond_account_product-6.6.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2020-05-19 17:03:19.000000 trytond_account_product-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      533 2019-06-04 16:49:44.000000 trytond_account_product-6.6.0/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2019-06-04 16:49:44.000000 trytond_account_product-6.6.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2022-04-08 16:23:26.000000 trytond_account_product-6.6.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:49.422292 trytond_account_product-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-05-01 11:16:20.000000 trytond_account_product-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:16:19.000000 trytond_account_product-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_product-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2604 2023-05-01 12:03:49.422292 trytond_account_product-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      968 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3210 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/analytic_account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/analytic_account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-01-16 14:00:20.000000 trytond_account_product-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:49.418959 trytond_account_product-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:49.415625 trytond_account_product-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6065 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6173 2023-04-30 10:46:36.000000 trytond_account_product-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6164 2023-04-30 10:46:36.000000 trytond_account_product-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6206 2023-04-30 10:46:36.000000 trytond_account_product-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5275 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5923 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6770 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6243 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5845 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5142 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6158 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6253 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5034 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6486 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5050 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5950 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6023 2023-04-30 10:46:36.000000 trytond_account_product-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6209 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5809 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4930 2023-04-29 08:02:51.000000 trytond_account_product-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16178 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3202 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:03:49.422292 trytond_account_product-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4532 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:49.415625 trytond_account_product-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4093 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 11:16:14.000000 trytond_account_product-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:49.422292 trytond_account_product-6.8.0/trytond_account_product.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2604 2023-05-01 12:03:48.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2031 2023-05-01 12:03:49.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:03:48.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 12:03:48.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      139 2023-05-01 12:03:48.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:03:48.000000 trytond_account_product-6.8.0/trytond_account_product.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:49.418959 trytond_account_product-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/view/analytic_account_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/view/analytic_account_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1262 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      533 2023-01-16 14:00:20.000000 trytond_account_product-6.8.0/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-01-16 14:00:20.000000 trytond_account_product-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_account_product-6.8.0/view/template_tree.xml
```

### Comparing `trytond_account_product-6.6.0/CHANGELOG` & `trytond_account_product-6.8.0/CHANGELOG`

 * *Files 7% similar despite different names*

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
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_product-6.6.0/COPYRIGHT` & `trytond_account_product-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 Copyright (C) 2004-2008 Tiny SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_account_product-6.6.0/LICENSE` & `trytond_account_product-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/PKG-INFO` & `trytond_account_product-6.8.0/trytond_account_product.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_product
-Version: 6.6.0
+Name: trytond-account-product
+Version: 6.8.0
 Summary: Tryton module to add accounting on product
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-product/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_product
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account product
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
 
 ######################
 Account Product Module
 ######################
```

### Comparing `trytond_account_product-6.6.0/__init__.py` & `trytond_account_product-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/account.py` & `trytond_account_product-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/account.xml` & `trytond_account_product-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/analytic_account.py` & `trytond_account_product-6.8.0/analytic_account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/analytic_account.xml` & `trytond_account_product-6.8.0/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/configuration.py` & `trytond_account_product-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/doc/conf.py` & `trytond_account_product-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_product-6.6.0/doc/design.rst` & `trytond_account_product-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/doc/usage.rst` & `trytond_account_product-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/bg.po` & `trytond_account_product-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/ca.po` & `trytond_account_product-6.8.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 msgctxt "field:product.category,supplier_taxes:"
 msgid "Supplier Taxes"
 msgstr "Impostos de proveïdor"
 
 msgctxt "field:product.category,supplier_taxes_deductible_rate:"
 msgid "Supplier Taxes Deductible Rate"
-msgstr "Percentage impostos proveïdor deduïble"
+msgstr "Rati impostos proveïdor deduïble"
 
 msgctxt "field:product.category,supplier_taxes_used:"
 msgid "Supplier Taxes Used"
 msgstr "Impostos de proveïdor usats"
 
 msgctxt "field:product.category,taxes_parent:"
 msgid "Use the Parent's Taxes"
```

### Comparing `trytond_account_product-6.6.0/locale/cs.po` & `trytond_account_product-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/de.po` & `trytond_account_product-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 msgctxt "field:analytic_account.rule,product:"
 msgid "Product"
 msgstr "Artikel"
 
 msgctxt "field:analytic_account.rule,product_category:"
 msgid "Product Category"
-msgstr "Artikel Kategorie"
+msgstr "Artikelkategorie"
 
 msgctxt "field:product.category,account_expense:"
 msgid "Account Expense"
 msgstr "Aufwandskonto"
 
 msgctxt "field:product.category,account_parent:"
 msgid "Use Parent's accounts"
```

### Comparing `trytond_account_product-6.6.0/locale/es.po` & `trytond_account_product-6.8.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 msgctxt "field:product.category,supplier_taxes:"
 msgid "Supplier Taxes"
 msgstr "Impuestos de proveedor"
 
 msgctxt "field:product.category,supplier_taxes_deductible_rate:"
 msgid "Supplier Taxes Deductible Rate"
-msgstr "Porcentaje de impuestos de proveedor deducible"
+msgstr "Ratio de impuestos de proveedor deducible"
 
 msgctxt "field:product.category,supplier_taxes_used:"
 msgid "Supplier Taxes Used"
 msgstr "Impuestos de proveedor usados"
 
 msgctxt "field:product.category,taxes_parent:"
 msgid "Use the Parent's Taxes"
```

### Comparing `trytond_account_product-6.6.0/locale/es_419.po` & `trytond_account_product-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/et.po` & `trytond_account_product-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/fa.po` & `trytond_account_product-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/fi.po` & `trytond_account_product-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/fr.po` & `trytond_account_product-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/hu.po` & `trytond_account_product-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/id.po` & `trytond_account_product-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/it.po` & `trytond_account_product-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/lo.po` & `trytond_account_product-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/lt.po` & `trytond_account_product-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/nl.po` & `trytond_account_product-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/pl.po` & `trytond_account_product-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/pt.po` & `trytond_account_product-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/ro.po` & `trytond_account_product-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 msgctxt "help:product.category,account_parent:"
 msgid "Use the accounts defined on the parent category."
 msgstr "Utilizare conturi definite la categoria părintelui."
 
 msgctxt "help:product.category,accounting:"
 msgid "Check to indicate the category is used for accounting."
-msgstr ""
+msgstr "Bifaţi dacă categoria este utilizata pentru contabilitate."
 
 msgctxt "help:product.category,customer_taxes:"
 msgid "The taxes to apply when selling products of this category."
 msgstr "Taxele de aplicat când se vând produse din aceasta categorie."
 
 msgctxt "help:product.category,supplier_taxes:"
 msgid "The taxes to apply when purchasing products of this category."
```

### Comparing `trytond_account_product-6.6.0/locale/ru.po` & `trytond_account_product-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/sl.po` & `trytond_account_product-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/tr.po` & `trytond_account_product-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/uk.po` & `trytond_account_product-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/locale/zh_CN.po` & `trytond_account_product-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/message.xml` & `trytond_account_product-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/product.py` & `trytond_account_product-6.8.0/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,16 @@
     @property
     @fields.depends(methods=['get_taxes'])
     def supplier_taxes_deductible_rate_used(self):
         return self.get_taxes('supplier_taxes_deductible_rate_used')
 
     @classmethod
     def copy(cls, templates, default=None):
-        context = Transaction().context
         default = default.copy() if default else {}
-        if context.get('_check_access'):
+        if Transaction().check_access:
             default.setdefault(
                 'account_category',
                 cls.default_get(
                     ['account_category'],
                     with_rec_name=False).get('account_category'))
         return super().copy(templates, default=default)
```

### Comparing `trytond_account_product-6.6.0/product.xml` & `trytond_account_product-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/setup.py` & `trytond_account_product-6.8.0/setup.py`

 * *Files 16% similar despite different names*

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
@@ -37,61 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_product'
 
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
 
 tests_require = [get_require_version('trytond_analytic_account')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add accounting on product',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
         'https://docs.tryton.org/projects/modules-account-product/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_product',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account product',
     package_dir={'trytond.modules.account_product': '.'},
     packages=(
         ['trytond.modules.account_product']
         + ['trytond.modules.account_product.%s' % p for p in find_packages()]
         ),
@@ -127,28 +105,27 @@
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
     account_product = trytond.modules.account_product
     """,
     )
```

### Comparing `trytond_account_product-6.6.0/tests/test_module.py` & `trytond_account_product-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/trytond_account_product.egg-info/PKG-INFO` & `trytond_account_product-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-product
-Version: 6.6.0
+Name: trytond_account_product
+Version: 6.8.0
 Summary: Tryton module to add accounting on product
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-product/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_product
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account product
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
 
 ######################
 Account Product Module
 ######################
```

### Comparing `trytond_account_product-6.6.0/trytond_account_product.egg-info/SOURCES.txt` & `trytond_account_product-6.8.0/trytond_account_product.egg-info/SOURCES.txt`

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
```

### Comparing `trytond_account_product-6.6.0/view/category_form.xml` & `trytond_account_product-6.8.0/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/view/configuration_form.xml` & `trytond_account_product-6.8.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_product-6.6.0/view/create_chart_properties_form.xml` & `trytond_account_product-6.8.0/view/create_chart_properties_form.xml`

 * *Files identical despite different names*

