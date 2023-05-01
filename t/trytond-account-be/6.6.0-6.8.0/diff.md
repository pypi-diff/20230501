# Comparing `tmp/trytond_account_be-6.6.0.tar.gz` & `tmp/trytond_account_be-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_be-6.6.0.tar", last modified: Mon Oct 31 16:22:26 2022, max compression
+gzip compressed data, was "trytond_account_be-6.8.0.tar", last modified: Mon May  1 11:56:43 2023, max compression
```

## Comparing `trytond_account_be-6.6.0.tar` & `trytond_account_be-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:26.203662 trytond_account_be-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_be-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_be-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-31 16:22:24.000000 trytond_account_be-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_be-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2432 2022-10-31 16:22:24.000000 trytond_account_be-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 16:22:23.000000 trytond_account_be-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:02.000000 trytond_account_be-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_be-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2016 2022-10-31 16:22:26.203662 trytond_account_be-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2019-06-04 16:49:43.000000 trytond_account_be-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2021-12-11 16:59:32.000000 trytond_account_be-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6571 2022-04-10 15:40:34.000000 trytond_account_be-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1491 2021-02-27 17:17:01.000000 trytond_account_be-6.6.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   300012 2022-09-01 20:05:40.000000 trytond_account_be-6.6.0/account_be.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   247325 2022-09-01 20:05:40.000000 trytond_account_be-6.6.0/account_be_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   247800 2022-09-01 20:05:40.000000 trytond_account_be-6.6.0/account_be_nl.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:26.200329 trytond_account_be-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2019-06-04 16:49:43.000000 trytond_account_be-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:26.200329 trytond_account_be-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1247 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1372 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1099 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1228 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1096 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1220 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1040 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-10-29 07:50:42.000000 trytond_account_be-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2020-09-17 22:06:40.000000 trytond_account_be-6.6.0/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:22:26.203662 trytond_account_be-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4251 2022-04-16 16:30:55.000000 trytond_account_be-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   165864 2019-06-04 16:49:43.000000 trytond_account_be-6.6.0/tax_be.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   156133 2020-09-17 22:06:40.000000 trytond_account_be-6.6.0/tax_be_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   155970 2020-09-17 22:06:40.000000 trytond_account_be-6.6.0/tax_be_nl.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:26.200329 trytond_account_be-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_be-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2022-04-16 16:30:55.000000 trytond_account_be-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2022-10-31 15:10:09.000000 trytond_account_be-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2022-10-31 16:22:22.000000 trytond_account_be-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:26.203662 trytond_account_be-6.6.0/trytond_account_be.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2016 2022-10-31 16:22:25.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1585 2022-10-31 16:22:26.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:22:25.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2022-10-31 16:22:25.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       73 2022-10-31 16:22:25.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:22:25.000000 trytond_account_be-6.6.0/trytond_account_be.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:26.200329 trytond_account_be-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2019-06-04 16:49:43.000000 trytond_account_be-6.6.0/view/vat_customer_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2021-10-07 13:08:06.000000 trytond_account_be-6.6.0/view/vat_customer_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:43.027001 trytond_account_be-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2595 2023-05-01 11:11:17.000000 trytond_account_be-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:11:17.000000 trytond_account_be-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_be-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2023-05-01 11:56:43.023667 trytond_account_be-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6824 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   300012 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/account_be.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   247325 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/account_be_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   247800 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/account_be_nl.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:43.023667 trytond_account_be-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      540 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:43.020334 trytond_account_be-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1247 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1372 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1099 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1228 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1096 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1220 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1040 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-29 08:02:48.000000 trytond_account_be-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:56:43.027001 trytond_account_be-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3444 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   169644 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/tax_be.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   159994 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/tax_be_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   159831 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/tax_be_nl.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:43.020334 trytond_account_be-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 11:11:11.000000 trytond_account_be-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:43.023667 trytond_account_be-6.8.0/trytond_account_be.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2023-05-01 11:56:42.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1559 2023-05-01 11:56:42.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:56:42.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:56:42.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       73 2023-05-01 11:56:42.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:56:42.000000 trytond_account_be-6.8.0/trytond_account_be.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:43.020334 trytond_account_be-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-16 14:00:20.000000 trytond_account_be-6.8.0/view/vat_customer_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:14.000000 trytond_account_be-6.8.0/view/vat_customer_list.xml
```

### Comparing `trytond_account_be-6.6.0/CHANGELOG` & `trytond_account_be-6.8.0/CHANGELOG`

 * *Files 15% similar despite different names*

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
 * Add support for Python 3.10
```

### Comparing `trytond_account_be-6.6.0/COPYRIGHT` & `trytond_account_be-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2011 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_be-6.6.0/LICENSE` & `trytond_account_be-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/PKG-INFO` & `trytond_account_be-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: trytond_account_be
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with Belgian chart of accounts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_be
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart belgian
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: French
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
 License-File: LICENSE
 
 Belgian Account Module
 ######################
 
 The Belgian account module defines the standard chart of account.
```

### Comparing `trytond_account_be-6.6.0/README.rst` & `trytond_account_be-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/account.py` & `trytond_account_be-6.8.0/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # this repository contains the full copyright notices and license terms.
 from sql import Literal
 from sql.aggregate import Max, Min, Sum
 from sql.functions import Position
 from sql.operators import Concat
 
 from trytond.model import ModelSQL, ModelView, fields
+from trytond.modules.account.exceptions import FiscalYearNotFoundError
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 from trytond.transaction import Transaction
 
 
 class AccountTemplate(metaclass=PoolMeta):
@@ -158,10 +159,15 @@
         return Transaction().context.get('company')
 
     @classmethod
     def default_fiscalyear(cls):
         pool = Pool()
         FiscalYear = pool.get('account.fiscalyear')
         context = Transaction().context
-        return context.get(
-            'fiscalyear',
-            FiscalYear.find(context.get('company'), exception=False))
+        if 'fiscalyear' not in context:
+            try:
+                fiscalyear = FiscalYear.find(
+                    cls.default_company(), test_state=False)
+            except FiscalYearNotFoundError:
+                return None
+            return fiscalyear.id
+        return context['fiscalyear']
```

### Comparing `trytond_account_be-6.6.0/account.xml` & `trytond_account_be-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/account_be.xml` & `trytond_account_be-6.8.0/account_be.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/account_be_fr.xml` & `trytond_account_be-6.8.0/account_be_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/account_be_nl.xml` & `trytond_account_be-6.8.0/account_be_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/doc/index.rst` & `trytond_account_be-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/bg.po` & `trytond_account_be-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/ca.po` & `trytond_account_be-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/cs.po` & `trytond_account_be-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/de.po` & `trytond_account_be-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/es.po` & `trytond_account_be-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/es_419.po` & `trytond_account_be-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/et.po` & `trytond_account_be-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/fa.po` & `trytond_account_be-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/fi.po` & `trytond_account_be-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/fr.po` & `trytond_account_be-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/hu.po` & `trytond_account_be-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/id.po` & `trytond_account_be-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/it.po` & `trytond_account_be-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/lo.po` & `trytond_account_be-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/lt.po` & `trytond_account_be-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/nl.po` & `trytond_account_be-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/pl.po` & `trytond_account_be-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/pt.po` & `trytond_account_be-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/ro.po` & `trytond_account_be-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/ru.po` & `trytond_account_be-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/sl.po` & `trytond_account_be-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/tr.po` & `trytond_account_be-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/uk.po` & `trytond_account_be-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/locale/zh_CN.po` & `trytond_account_be-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/localize.xsl` & `trytond_account_be-6.8.0/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/setup.py` & `trytond_account_be-6.8.0/setup.py`

 * *Files 16% similar despite different names*

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
@@ -34,59 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_be'
 
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
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module with Belgian chart of accounts',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_be',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account chart belgian',
     package_dir={'trytond.modules.account_be': '.'},
     packages=(
         ['trytond.modules.account_be']
         + ['trytond.modules.account_be.%s' % p for p in find_packages()]
         ),
@@ -103,25 +80,24 @@
         'Intended Audience :: Legal Industry',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: Dutch',
         'Natural Language :: French',
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     account_be = trytond.modules.account_be
     """,
     )
```

### Comparing `trytond_account_be-6.6.0/tax_be.xml` & `trytond_account_be-6.8.0/tax_be.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_account_be-6.6.0/tax_be.xml` & `trytond_account_be-6.8.0/tax_be.xml`

```diff
@@ -2643,14 +2643,77 @@
     <record model="account.tax.code.template" id="tax_code_V_B_62">
       <field name="name" lang="fr">B. Diverses régularisations T.V.A. en faveur du déclarant</field>
       <field name="name" lang="nl">B. Diverse btw-regularisaties in het voordeel van de aangever</field>
       <field name="code">62</field>
       <field name="parent" ref="tax_code_V"/>
       <field name="account" ref="root"/>
     </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_6_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_6_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_12_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_12_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_21_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_21_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_6_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_6_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_12_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_12_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_21_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_21_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_6_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_6_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_12_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_12_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record model="account.tax.code.line.template" id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_21_1">
+      <field name="code" ref="tax_code_V_B_62"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_21_1"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
     <record model="account.tax.code.template" id="tax_code_V_C_64">
       <field name="name" lang="fr">C. T.V.A. à récupérer mentionnée sur les notes de crédit délivrées</field>
       <field name="name" lang="nl">C. Te recupereren btw vermeld op uitgereikte creditnota's</field>
       <field name="code">64</field>
       <field name="parent" ref="tax_code_V"/>
       <field name="account" ref="root"/>
     </record>
```

### Comparing `trytond_account_be-6.6.0/tax_be_fr.xml` & `trytond_account_be-6.8.0/tax_be_fr.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_account_be-6.6.0/tax_be_fr.xml` & `trytond_account_be-6.8.0/tax_be_fr.xml`

```diff
@@ -2515,14 +2515,77 @@
     </record>
     <record id="tax_code_V_B_62_fr" model="account.tax.code.template">
       <field name="name">B. Diverses régularisations T.V.A. en faveur du déclarant</field>
       <field name="code">62</field>
       <field name="parent" ref="tax_code_V_fr"/>
       <field name="account" ref="root_fr"/>
     </record>
+    <record id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_6_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_6_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_12_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_12_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_21_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_21_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_6_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_6_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_12_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_12_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_21_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_21_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_6_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_6_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_12_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_12_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_21_1_fr" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_fr"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_21_1_fr"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
     <record id="tax_code_V_C_64_fr" model="account.tax.code.template">
       <field name="name">C. T.V.A. à récupérer mentionnée sur les notes de crédit délivrées</field>
       <field name="code">64</field>
       <field name="parent" ref="tax_code_V_fr"/>
       <field name="account" ref="root_fr"/>
     </record>
     <record id="tax_code_V_C_64-tva_vente_biens_6_fr" model="account.tax.code.line.template">
```

### Comparing `trytond_account_be-6.6.0/tax_be_nl.xml` & `trytond_account_be-6.8.0/tax_be_nl.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_account_be-6.6.0/tax_be_nl.xml` & `trytond_account_be-6.8.0/tax_be_nl.xml`

```diff
@@ -2515,14 +2515,77 @@
     </record>
     <record id="tax_code_V_B_62_nl" model="account.tax.code.template">
       <field name="name">B. Diverse btw-regularisaties in het voordeel van de aangever</field>
       <field name="code">62</field>
       <field name="parent" ref="tax_code_V_nl"/>
       <field name="account" ref="root_nl"/>
     </record>
+    <record id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_6_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_6_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_12_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_12_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_marchandises_intracommunautaires_21_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_marchandises_intracommunautaires_21_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_6_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_6_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_12_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_12_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_frais_biens_intracommunautaires_21_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_frais_biens_intracommunautaires_21_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_6_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_6_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_12_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_12_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
+    <record id="tax_code_V_B_62-tva_achat_investissement_intracommunautaires_21_1_nl" model="account.tax.code.line.template">
+      <field name="code" ref="tax_code_V_B_62_nl"/>
+      <field name="tax" ref="tva_achat_investissement_intracommunautaires_21_1_nl"/>
+      <field name="operator">+</field>
+      <field name="amount">tax</field>
+      <field name="type">credit</field>
+    </record>
     <record id="tax_code_V_C_64_nl" model="account.tax.code.template">
       <field name="name">C. Te recupereren btw vermeld op uitgereikte creditnota's</field>
       <field name="code">64</field>
       <field name="parent" ref="tax_code_V_nl"/>
       <field name="account" ref="root_nl"/>
     </record>
     <record id="tax_code_V_C_64-tva_vente_biens_6_nl" model="account.tax.code.line.template">
```

### Comparing `trytond_account_be-6.6.0/tests/test_module.py` & `trytond_account_be-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_be-6.6.0/trytond_account_be.egg-info/PKG-INFO` & `trytond_account_be-6.8.0/trytond_account_be.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: trytond-account-be
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with Belgian chart of accounts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_be
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart belgian
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: French
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
 License-File: LICENSE
 
 Belgian Account Module
 ######################
 
 The Belgian account module defines the standard chart of account.
```

### Comparing `trytond_account_be-6.6.0/trytond_account_be.egg-info/SOURCES.txt` & `trytond_account_be-6.8.0/trytond_account_be.egg-info/SOURCES.txt`

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
@@ -52,14 +48,15 @@
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/vat_customer_context_form.xml
 ./view/vat_customer_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

