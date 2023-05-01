# Comparing `tmp/trytond_sale_stock_quantity-6.6.1.tar.gz` & `tmp/trytond_sale_stock_quantity-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_stock_quantity-6.6.1.tar", last modified: Mon Jan  2 22:27:30 2023, max compression
+gzip compressed data, was "trytond_sale_stock_quantity-6.8.0.tar", last modified: Mon May  1 12:03:07 2023, max compression
```

## Comparing `trytond_sale_stock_quantity-6.6.1.tar` & `trytond_sale_stock_quantity-6.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:27:30.334393 trytond_sale_stock_quantity-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1401 2023-01-02 22:27:27.000000 trytond_sale_stock_quantity-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-01-02 22:27:26.000000 trytond_sale_stock_quantity-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2608 2023-01-02 22:27:30.334393 trytond_sale_stock_quantity-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-12-19 12:02:58.000000 trytond_sale_stock_quantity-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:27:30.331060 trytond_sale_stock_quantity-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:27:30.327726 trytond_sale_stock_quantity-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      832 2022-12-19 12:02:58.000000 trytond_sale_stock_quantity-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      990 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      859 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      826 2022-12-19 12:02:58.000000 trytond_sale_stock_quantity-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      913 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2022-12-19 12:02:58.000000 trytond_sale_stock_quantity-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9729 2023-01-02 20:25:44.000000 trytond_sale_stock_quantity-6.6.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-01-02 22:27:30.334393 trytond_sale_stock_quantity-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4520 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:27:30.331060 trytond_sale_stock_quantity-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:58.000000 trytond_sale_stock_quantity-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6045 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/tests/scenario_sale_stock_quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      546 2022-12-19 12:02:57.000000 trytond_sale_stock_quantity-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2022-12-19 12:03:07.000000 trytond_sale_stock_quantity-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:27:30.334393 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2608 2023-01-02 22:27:29.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-01-02 22:27:30.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:27:29.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-01-02 22:27:29.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:27:29.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-01-02 22:27:29.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-01-02 22:27:29.000000 trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:07.491772 trytond_sale_stock_quantity-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1464 2023-05-01 11:15:52.000000 trytond_sale_stock_quantity-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:15:51.000000 trytond_sale_stock_quantity-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_stock_quantity-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 12:03:07.488438 trytond_sale_stock_quantity-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_sale_stock_quantity-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:07.488438 trytond_sale_stock_quantity-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_sale_stock_quantity-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:07.485105 trytond_sale_stock_quantity-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      832 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      990 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      859 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      826 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-04-30 10:46:36.000000 trytond_sale_stock_quantity-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-04-29 08:02:50.000000 trytond_sale_stock_quantity-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10527 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:03:07.491772 trytond_sale_stock_quantity-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4480 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:07.488438 trytond_sale_stock_quantity-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6077 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/tests/scenario_sale_stock_quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-05-01 11:15:46.000000 trytond_sale_stock_quantity-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:03:07.488438 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 12:03:06.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-05-01 12:03:07.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:03:06.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 12:03:06.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-05-01 12:03:06.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:03:06.000000 trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/top_level.txt
```

### Comparing `trytond_sale_stock_quantity-6.6.1/CHANGELOG` & `trytond_sale_stock_quantity-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-Version 6.6.1 - 2023-01-02
+
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

### Comparing `trytond_sale_stock_quantity-6.6.1/COPYRIGHT` & `trytond_sale_stock_quantity-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2022 Cédric Krier.
-Copyright (C) 2015-2022 B2CK SPRL.
+Copyright (C) 2015-2023 Cédric Krier.
+Copyright (C) 2015-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_stock_quantity-6.6.1/LICENSE` & `trytond_sale_stock_quantity-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/PKG-INFO` & `trytond_sale_stock_quantity-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_stock_quantity
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add stock warning on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_stock_quantity
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 
 Sale Stock Quantity
 ###################
 
 The sale_stock_quantity module check the stock quantity of the products when
```

### Comparing `trytond_sale_stock_quantity-6.6.1/doc/conf.py` & `trytond_sale_stock_quantity-6.8.0/doc/conf.py`

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

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/bg.po` & `trytond_sale_stock_quantity-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/ca.po` & `trytond_sale_stock_quantity-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/cs.po` & `trytond_sale_stock_quantity-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/de.po` & `trytond_sale_stock_quantity-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/es.po` & `trytond_sale_stock_quantity-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/es_419.po` & `trytond_sale_stock_quantity-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/et.po` & `trytond_sale_stock_quantity-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/fa.po` & `trytond_sale_stock_quantity-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/fi.po` & `trytond_sale_stock_quantity-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/fr.po` & `trytond_sale_stock_quantity-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/hu.po` & `trytond_sale_stock_quantity-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/id.po` & `trytond_sale_stock_quantity-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/it.po` & `trytond_sale_stock_quantity-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/lo.po` & `trytond_sale_stock_quantity-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/lt.po` & `trytond_sale_stock_quantity-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/nl.po` & `trytond_sale_stock_quantity-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/pl.po` & `trytond_sale_stock_quantity-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/pt.po` & `trytond_sale_stock_quantity-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/ro.po` & `trytond_sale_stock_quantity-6.8.0/locale/ro.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_product_forecast_quantity_lower"
 msgid ""
 "The forecast quantity (%(forecast_quantity)s) of product \"%(product)s\" is "
 "lower than the quantity (%(quantity)s)."
 msgstr ""
-"Cantitatea estimata (%(forecast_quantity)s%(default_uom)s) pentru rândul "
-"\"%(line)s\" este mai mică decât cantitatea proprie (%(quantity)s%(unit)s)."
+"Cantitatea estimata (%(forecast_quantity)s) din produsul \"%(product)s\" "
+"este mai mică decât cantitatea (%(quantity)s)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_stock_quantity"
 msgid ""
 "The forcast quantity (%(forecast_quantity)s) for line \"%(line)s\" is lower "
 "than its quantity (%(quantity)s)."
 msgstr ""
-"Cantitatea estimata (%(forecast_quantity)s%(default_uom)s) pentru rândul "
-"\"%(line)s\" este mai mică decât cantitatea proprie (%(quantity)s%(unit)s)."
+"Cantitatea estimata (%(forecast_quantity)s) pentru rândul \"%(line)s\" este "
+"mai mică decât cantitatea proprie (%(quantity)s)."
 
 msgctxt "model:res.group,name:group_sale_stock_quantity"
 msgid "Sale Stock Quantity"
 msgstr "Vânzare Cantitate Stoc"
```

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/ru.po` & `trytond_sale_stock_quantity-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/sl.po` & `trytond_sale_stock_quantity-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/tr.po` & `trytond_sale_stock_quantity-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/uk.po` & `trytond_sale_stock_quantity-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/locale/zh_CN.po` & `trytond_sale_stock_quantity-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/message.xml` & `trytond_sale_stock_quantity-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/sale.py` & `trytond_sale_stock_quantity-6.8.0/sale.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 import datetime
 from collections import defaultdict
+from itertools import groupby
+from operator import attrgetter
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 
@@ -81,42 +83,44 @@
                 user_id = transaction.context.get('user', user_id)
             if user_id == 0:
                 return True
             user = User(user_id)
             return group in user.groups
 
         def filter_line(line):
-            return (line.product
+            return (line.warehouse
+                and line.product
                 and line.product.type == 'goods'
                 and not line.product.consumable
                 and line.quantity > 0
                 # Use getattr as supply_on_sale comes from sale_supply module
                 and not getattr(line, 'supply_on_sale', False))
 
-        def get_delta(date):
+        def get_delta(date, warehouse, products):
             'Compute quantity delta at the date'
             if date in date2delta:
-                return date2delta[date]
+                return date2delta[warehouse][date]
 
             with transaction.set_context(forecast=True,
                     stock_date_start=date,
                     stock_date_end=date):
                 pbl = defaultdict(int)
-                for sub_product_ids in grouped_slice(product_ids):
+                for sub_products in grouped_slice(products):
+                    sub_product_ids = [p.id for p in sub_products]
                     pbl.update(Product.products_by_location(
-                            [self.warehouse.id],
+                            [warehouse.id],
                             with_childs=True,
-                            grouping_filter=(list(sub_product_ids),)))
+                            grouping_filter=(sub_product_ids,)))
             delta = {}
             for key, qty in pbl.items():
                 _, product_id = key
                 delta[product_id] = qty
-            date2delta[date] = delta
+            date2delta[warehouse][date] = delta
             return delta
-        date2delta = {}
+        date2delta = defaultdict(dict)
 
         def raise_(line_id, message_values):
             if not in_group():
                 raise StockQuantityError(
                     gettext('sale_stock_quantity.msg_sale_stock_quantity',
                         **message_values))
             warning_name = 'stock_quantity_warning_%s' % line_id
@@ -125,71 +129,83 @@
                     gettext('sale_stock_quantity.msg_sale_stock_quantity',
                         **message_values))
 
         with Transaction().set_context(company=self.company.id):
             today = Date.today()
         lang = Lang.get()
         sale_date = self.sale_date or today
-        product_ids = {l.product.id for l in filter(filter_line, self.lines)}
-        product_ids = list(product_ids)
 
-        with transaction.set_context(
-                locations=[self.warehouse.id],
-                stock_date_end=sale_date,
-                stock_assign=True):
-            products = Product.browse(product_ids)
-        quantities = {p: p.forecast_quantity for p in products}
-
-        # Remove quantities from other sales
-        for sub_product_ids in grouped_slice(product_ids):
-            lines = Line.search([
-                    ('sale.company', '=', self.company.id),
-                    ('sale.state', 'in', self._stock_quantity_states()),
-                    ('sale.id', '!=', self.id),
-                    ['OR',
-                        ('sale.sale_date', '<=', sale_date),
-                        ('sale.sale_date', '=', None),
-                        ],
-                    ('product', 'in', sub_product_ids),
-                    ('quantity', '>', 0),
-                    ])
-            for line in lines:
-                product = line.product
-                date = line.sale.sale_date or today
-                if date > today or line.warehouse != self.warehouse:
-                    continue
-                quantity = Uom.compute_qty(line.unit, line.quantity,
-                    product.default_uom, round=False)
-                quantities[product] -= quantity
+        lines = filter(filter_line, self.lines)
+        lines = list(lines)
 
-        for line in filter(filter_line, self.lines):
+        quantities = defaultdict(lambda: defaultdict(int))
+        w_getter = attrgetter('warehouse')
+        w_products = {}
+        for warehouse, w_lines in groupby(
+                sorted(lines, key=w_getter), key=w_getter):
+            w_products[warehouse] = products = {l.product for l in w_lines}
+            with transaction.set_context(
+                    locations=[warehouse.id],
+                    stock_date_end=sale_date,
+                    stock_assign=True):
+                products = Product.browse(products)
+            quantities[warehouse].update(
+                (p, p.forecast_quantity) for p in products)
+
+            # Remove quantities from other sales
+            for sub_products in grouped_slice(products):
+                other_lines = Line.search([
+                        ('sale.company', '=', self.company.id),
+                        ('sale.state', 'in', self._stock_quantity_states()),
+                        ('sale.id', '!=', self.id),
+                        ['OR',
+                            ('sale.sale_date', '<=', sale_date),
+                            ('sale.sale_date', '=', None),
+                            ],
+                        ('product', 'in', sub_products),
+                        ('quantity', '>', 0),
+                        ])
+                for line in other_lines:
+                    if line.warehouse != warehouse:
+                        continue
+                    product = line.product
+                    date = line.sale.sale_date or today
+                    if date > today:
+                        continue
+                    quantity = Uom.compute_qty(line.unit, line.quantity,
+                        product.default_uom, round=False)
+                    quantities[line.warehouse][product] -= quantity
+
+        for line in lines:
+            warehouse = line.warehouse
             product = line.product
             quantity = Uom.compute_qty(line.unit, line.quantity,
                 product.default_uom, round=False)
             next_supply_date = self._stock_quantity_next_supply_date(product)
             message_values = {
                 'line': line.rec_name,
                 'forecast_quantity': lang.format_number_symbol(
-                    quantities[product], product.default_uom,
-                    product.default_uom.digits),
+                    quantities[warehouse][product],
+                    product.default_uom, product.default_uom.digits),
                 'quantity': lang.format_number_symbol(
                     line.quantity, line.unit, line.unit.digits),
                 }
-            if (quantities[product] < quantity
+            if (quantities[warehouse][product] < quantity
                     and sale_date < next_supply_date):
                 raise_(line.id, message_values)
             # Update quantities if the same product is many times in lines
-            quantities[product] -= quantity
+            quantities[warehouse][product] -= quantity
 
             # Check other dates until next supply date
             if next_supply_date != datetime.date.max:
-                forecast_quantity = quantities[product]
+                products = w_products[warehouse]
+                forecast_quantity = quantities[warehouse][product]
                 date = sale_date + datetime.timedelta(1)
                 while date < next_supply_date:
-                    delta = get_delta(date)
+                    delta = get_delta(date, warehouse, products)
                     forecast_quantity += delta.get(product.id, 0)
                     if forecast_quantity < 0:
                         message_values['forecast_quantity'] = forecast_quantity
                         raise_(line.id, message_values)
                     date += datetime.timedelta(1)
```

### Comparing `trytond_sale_stock_quantity-6.6.1/sale.xml` & `trytond_sale_stock_quantity-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-6.6.1/setup.py` & `trytond_sale_stock_quantity-6.8.0/setup.py`

 * *Files 1% similar despite different names*

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
 name = 'trytond_sale_stock_quantity'
 
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
 
@@ -53,22 +53,22 @@
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module to add stock warning on sale',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_stock_quantity',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale stock',
     package_dir={'trytond.modules.sale_stock_quantity': '.'},
     packages=(
         ['trytond.modules.sale_stock_quantity']
         + ['trytond.modules.sale_stock_quantity.%s' % p
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

### Comparing `trytond_sale_stock_quantity-6.6.1/tests/scenario_sale_stock_quantity.rst` & `trytond_sale_stock_quantity-6.8.0/tests/scenario_sale_stock_quantity.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 ===================
 Sale Stock Quantity
 ===================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.stock.exceptions import InventoryFutureWarning
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
+    >>> later = today + dt.timedelta(days=2)
 
 Activate modules::
 
     >>> config = activate_modules(['sale_stock_quantity', 'stock_supply'])
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, (today, later)))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> revenue = accounts['revenue']
@@ -73,15 +75,15 @@
     >>> template.save()
     >>> product, = template.products
 
     >>> ProductSupplier = Model.get('purchase.product_supplier')
     >>> product_supplier = ProductSupplier()
     >>> product_supplier.template = template
     >>> product_supplier.party = supplier
-    >>> product_supplier.lead_time = datetime.timedelta(3)
+    >>> product_supplier.lead_time = dt.timedelta(3)
     >>> product_supplier.save()
 
 Create payment term::
 
     >>> payment_term = create_payment_term()
     >>> payment_term.save()
 
@@ -161,15 +163,15 @@
     StockQuantityWarning: ...
     >>> sale.delete()
 
 Make an inventory of 3 products in 2 days::
 
     >>> inventory = Inventory()
     >>> inventory.location = storage
-    >>> inventory.date = today + datetime.timedelta(2)
+    >>> inventory.date = later
     >>> inventory_line = inventory.lines.new(product=product)
     >>> inventory_line.quantity = 3.0
     >>> inventory_line.expected_quantity = 5.0
     >>> try:
     ...     inventory.click('confirm')
     ... except InventoryFutureWarning as e:
     ...     Model.get('res.user.warning')(user=config.user, name=e.name).save()
```

### Comparing `trytond_sale_stock_quantity-6.6.1/tox.ini` & `trytond_sale_stock_quantity-6.8.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/sale_stock_quantity/* -m unittest discover -s tests
-    coverage report --include=./**/sale_stock_quantity/* --omit=*/tests/*
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

### Comparing `trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/PKG-INFO` & `trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-stock-quantity
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add stock warning on sale
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_stock_quantity
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
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
 
 Sale Stock Quantity
 ###################
 
 The sale_stock_quantity module check the stock quantity of the products when
```

### Comparing `trytond_sale_stock_quantity-6.6.1/trytond_sale_stock_quantity.egg-info/SOURCES.txt` & `trytond_sale_stock_quantity-6.8.0/trytond_sale_stock_quantity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

