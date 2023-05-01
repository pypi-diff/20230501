# Comparing `tmp/trytond_account_eu-6.6.0.tar.gz` & `tmp/trytond_account_eu-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_eu-6.6.0.tar", last modified: Mon Oct 31 16:00:46 2022, max compression
+gzip compressed data, was "trytond_account_eu-6.8.0.tar", last modified: Mon May  1 11:48:06 2023, max compression
```

## Comparing `trytond_account_eu-6.6.0.tar` & `trytond_account_eu-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:46.884503 trytond_account_eu-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_eu-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_eu-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-31 16:00:45.000000 trytond_account_eu-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_eu-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2022-10-31 16:00:44.000000 trytond_account_eu-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:00:44.000000 trytond_account_eu-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_account_eu-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_eu-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2287 2022-10-31 16:00:46.881170 trytond_account_eu-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2019-06-04 16:49:46.000000 trytond_account_eu-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2021-12-11 16:59:32.000000 trytond_account_eu-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5203 2022-04-10 15:40:34.000000 trytond_account_eu-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2021-02-27 17:17:01.000000 trytond_account_eu-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:46.881170 trytond_account_eu-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2019-06-04 16:49:46.000000 trytond_account_eu-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:46.881170 trytond_account_eu-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1846 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1866 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1913 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1509 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1713 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1825 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1713 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1580 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1892 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1500 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1548 2022-10-29 07:50:38.000000 trytond_account_eu-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:00:46.884503 trytond_account_eu-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5003 2022-10-29 07:39:10.000000 trytond_account_eu-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:46.881170 trytond_account_eu-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_eu-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-04-16 16:30:55.000000 trytond_account_eu-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-10-31 15:10:09.000000 trytond_account_eu-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2022-10-31 16:00:43.000000 trytond_account_eu-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:46.881170 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2287 2022-10-31 16:00:46.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2022-10-31 16:00:46.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:00:46.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2022-10-31 16:00:46.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:58.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2022-10-31 16:00:46.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:00:46.000000 trytond_account_eu-6.6.0/trytond_account_eu.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:46.881170 trytond_account_eu-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2021-10-07 13:08:06.000000 trytond_account_eu-6.6.0/view/ec_sales_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2019-06-04 16:49:46.000000 trytond_account_eu-6.6.0/view/ec_sales_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2019-06-04 16:49:46.000000 trytond_account_eu-6.6.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2019-06-04 16:49:46.000000 trytond_account_eu-6.6.0/view/tax_template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:06.940596 trytond_account_eu-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1163 2023-05-01 11:05:26.000000 trytond_account_eu-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:05:25.000000 trytond_account_eu-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_eu-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-05-01 11:48:06.940596 trytond_account_eu-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-01-16 14:00:20.000000 trytond_account_eu-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5456 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:06.937263 trytond_account_eu-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-01-16 14:00:20.000000 trytond_account_eu-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:06.933929 trytond_account_eu-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1846 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1866 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1913 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1509 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1713 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1825 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1713 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1580 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1892 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1500 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1548 2023-04-29 08:02:45.000000 trytond_account_eu-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:48:06.940596 trytond_account_eu-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4197 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:06.933929 trytond_account_eu-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2023-05-01 11:05:20.000000 trytond_account_eu-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:06.940596 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-05-01 11:48:06.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1472 2023-05-01 11:48:06.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:48:06.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:48:06.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-05-01 11:48:06.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:48:06.000000 trytond_account_eu-6.8.0/trytond_account_eu.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:06.937263 trytond_account_eu-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_eu-6.8.0/view/ec_sales_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-01-16 14:00:20.000000 trytond_account_eu-6.8.0/view/ec_sales_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_eu-6.8.0/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-01-16 14:00:20.000000 trytond_account_eu-6.8.0/view/tax_template_form.xml
```

### Comparing `trytond_account_eu-6.6.0/CHANGELOG` & `trytond_account_eu-6.8.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_account_eu-6.6.0/COPYRIGHT` & `trytond_account_eu-6.8.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2022 Cédric Krier
-Copyright (C) 2017-2022 B2CK
+Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_eu-6.6.0/LICENSE` & `trytond_account_eu-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/PKG-INFO` & `trytond_account_eu-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_eu
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for european accounting
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_eu
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account europe vat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Account Europe Module
 #####################
 
 The account_eu module implements common accounting requirements in Europe.
```

### Comparing `trytond_account_eu-6.6.0/account.py` & `trytond_account_eu-6.8.0/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from sql import Literal, Null
 from sql.aggregate import Min, Sum
 from sql.functions import CurrentTimestamp
 
 from trytond.model import ModelSQL, ModelView, fields
+from trytond.modules.account.exceptions import FiscalYearNotFoundError
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval
 from trytond.transaction import Transaction
 
 
 class TaxTemplate(metaclass=PoolMeta):
@@ -128,10 +129,15 @@
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

### Comparing `trytond_account_eu-6.6.0/account.xml` & `trytond_account_eu-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/bg.po` & `trytond_account_eu-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/ca.po` & `trytond_account_eu-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/cs.po` & `trytond_account_eu-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/de.po` & `trytond_account_eu-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/es.po` & `trytond_account_eu-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/es_419.po` & `trytond_account_eu-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/et.po` & `trytond_account_eu-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/fa.po` & `trytond_account_eu-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/fi.po` & `trytond_account_eu-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/fr.po` & `trytond_account_eu-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/hu.po` & `trytond_account_eu-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/id.po` & `trytond_account_eu-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/it.po` & `trytond_account_eu-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/lo.po` & `trytond_account_eu-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/lt.po` & `trytond_account_eu-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/nl.po` & `trytond_account_eu-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/pl.po` & `trytond_account_eu-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/pt.po` & `trytond_account_eu-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/ro.po` & `trytond_account_eu-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/ru.po` & `trytond_account_eu-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/sl.po` & `trytond_account_eu-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/tr.po` & `trytond_account_eu-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/uk.po` & `trytond_account_eu-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/locale/zh_CN.po` & `trytond_account_eu-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_eu-6.6.0/setup.py` & `trytond_account_eu-6.8.0/setup.py`

 * *Files 14% similar despite different names*

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_eu'
 
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
 
 tests_require = []
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for european accounting',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_eu',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account europe vat',
     package_dir={'trytond.modules.account_eu': '.'},
     packages=(
         ['trytond.modules.account_eu']
         + ['trytond.modules.account_eu.%s' % p for p in find_packages()]
         ),
@@ -122,27 +100,26 @@
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
     account_eu = trytond.modules.account_eu
     """,
     )
```

### Comparing `trytond_account_eu-6.6.0/trytond_account_eu.egg-info/PKG-INFO` & `trytond_account_eu-6.8.0/trytond_account_eu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-eu
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for european accounting
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_eu
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account europe vat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Account Europe Module
 #####################
 
 The account_eu module implements common accounting requirements in Europe.
```

### Comparing `trytond_account_eu-6.6.0/trytond_account_eu.egg-info/SOURCES.txt` & `trytond_account_eu-6.8.0/trytond_account_eu.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
@@ -43,14 +39,15 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/ec_sales_list.xml
 ./view/ec_sales_list_context_form.xml
 ./view/tax_form.xml
 ./view/tax_template_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

