# Comparing `tmp/trytond_account_invoice_history-6.6.1.tar.gz` & `tmp/trytond_account_invoice_history-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_history-6.6.1.tar", last modified: Sun Feb  5 21:22:59 2023, max compression
+gzip compressed data, was "trytond_account_invoice_history-6.8.0.tar", last modified: Mon May  1 11:44:04 2023, max compression
```

## Comparing `trytond_account_invoice_history-6.6.1.tar` & `trytond_account_invoice_history-6.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:22:59.031345 trytond_account_invoice_history-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2437 2023-02-05 21:22:55.000000 trytond_account_invoice_history-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-02-05 21:22:55.000000 trytond_account_invoice_history-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-02-05 21:22:59.031345 trytond_account_invoice_history-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3716 2023-02-05 20:48:28.000000 trytond_account_invoice_history-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/account_invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:22:59.031345 trytond_account_invoice_history-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:22:59.028012 trytond_account_invoice_history-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      234 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      252 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:22:59.031345 trytond_account_invoice_history-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4366 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:22:59.028012 trytond_account_invoice_history-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      540 2022-12-19 12:02:49.000000 trytond_account_invoice_history-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2022-12-19 12:03:07.000000 trytond_account_invoice_history-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:22:59.031345 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:22:58.000000 trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:04.440920 trytond_account_invoice_history-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2538 2023-05-01 11:02:50.000000 trytond_account_invoice_history-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:02:49.000000 trytond_account_invoice_history-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_history-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2440 2023-05-01 11:44:04.440920 trytond_account_invoice_history-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4044 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/account_invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:04.440920 trytond_account_invoice_history-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:04.437587 trytond_account_invoice_history-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      234 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      252 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-29 08:02:41.000000 trytond_account_invoice_history-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:44:04.440920 trytond_account_invoice_history-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4322 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:04.440920 trytond_account_invoice_history-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_account_invoice_history-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-05-01 11:02:44.000000 trytond_account_invoice_history-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:04.440920 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2440 2023-05-01 11:44:03.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-05-01 11:44:04.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:44:03.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-05-01 11:44:03.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-05-01 11:44:03.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:44:03.000000 trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/top_level.txt
```

### Comparing `trytond_account_invoice_history-6.6.1/CHANGELOG` & `trytond_account_invoice_history-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-Version 6.6.1 - 2023-02-05
+
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Add history on party tax identifier
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_invoice_history-6.6.1/COPYRIGHT` & `trytond_account_invoice_history-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-6.6.1/LICENSE` & `trytond_account_invoice_history-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-6.6.1/PKG-INFO` & `trytond_account_invoice_history-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_history
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to historize invoices
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_history
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice history
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
 License-File: LICENSE
 
 Account Invoice History Module
 ##############################
 
 The account invoice history module activates the historization of the invoice
 and its related fields.
```

### Comparing `trytond_account_invoice_history-6.6.1/__init__.py` & `trytond_account_invoice_history-6.8.0/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 from . import account, account_invoice, party
 
 
 def register():
     Pool.register(
         party.Party,
         party.Address,
+        party.Identifier,
         account.Invoice,
         account_invoice.PaymentTerm,
         account_invoice.PaymentTermLine,
         account_invoice.PaymentTermLineRelativeDelta,
         module='account_invoice_history', type_='model')
```

### Comparing `trytond_account_invoice_history-6.6.1/account.py` & `trytond_account_invoice_history-6.8.0/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,40 +33,46 @@
             table_h.drop_column('open_date')
 
     @classmethod
     def __setup__(cls):
         super(Invoice, cls).__setup__()
         cls._check_modify_exclude.add('numbered_at')
         cls.party.datetime_field = 'history_datetime'
+        cls.party_tax_identifier.datetime_field = 'history_datetime'
         cls.invoice_address.datetime_field = 'history_datetime'
         cls.payment_term.datetime_field = 'history_datetime'
 
     @classmethod
     def get_history_datetime(cls, invoices, name):
         pool = Pool()
         Party = pool.get('party.party')
         Address = pool.get('party.address')
+        Identifier = pool.get('party.identifier')
         PaymentTerm = pool.get('account.invoice.payment_term')
         table = cls.__table__()
         party = Party.__table__()
         address = Address.__table__()
+        identifier = Identifier.__table__()
         payment_term = PaymentTerm.__table__()
         cursor = Transaction().connection.cursor()
 
         invoice_ids = [i.id for i in invoices]
         datetimes = dict.fromkeys(invoice_ids)
         for ids in grouped_slice(invoice_ids):
             cursor.execute(*table
                 .join(party, condition=table.party == party.id)
                 .join(address, condition=table.invoice_address == address.id)
+                .join(identifier, 'LEFT',
+                    condition=table.party_tax_identifier == identifier.id)
                 .join(payment_term, 'LEFT',
                     condition=table.payment_term == payment_term.id)
                 .select(table.id,
                     Greatest(table.numbered_at, party.create_date,
-                        address.create_date, payment_term.create_date),
+                        address.create_date, identifier.create_date,
+                        payment_term.create_date),
                     where=reduce_ids(table.id, ids)
                     & (table.numbered_at != Null)
                     & (table.state.in_(cls._history_states()))))
             datetimes.update(cursor)
         return datetimes
 
     @classmethod
```

### Comparing `trytond_account_invoice_history-6.6.1/account_invoice.py` & `trytond_account_invoice_history-6.8.0/account_invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_history-6.6.1/doc/conf.py` & `trytond_account_invoice_history-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_invoice_history-6.6.1/setup.py` & `trytond_account_invoice_history-6.8.0/setup.py`

 * *Files 3% similar despite different names*

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
@@ -34,36 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_invoice_history'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 0.4']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 setup(name=name,
     version=version,
     description='Tryton module to historize invoices',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_invoice_history',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice history',
     package_dir={'trytond.modules.account_invoice_history': '.'},
     packages=(
         ['trytond.modules.account_invoice_history']
         + ['trytond.modules.account_invoice_history.%s' % p
             for p in find_packages()]
@@ -100,24 +100,24 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     account_invoice_history = trytond.modules.account_invoice_history
     """,
     )
```

### Comparing `trytond_account_invoice_history-6.6.1/tox.ini` & `trytond_account_invoice_history-6.8.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 commands =
-    coverage run --include=./**/account_invoice_history/* -m unittest discover -s tests
-    coverage report --include=./**/account_invoice_history/* --omit=*/tests/*
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

### Comparing `trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/PKG-INFO` & `trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-history
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to historize invoices
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_invoice_history
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice history
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
 License-File: LICENSE
 
 Account Invoice History Module
 ##############################
 
 The account invoice history module activates the historization of the invoice
 and its related fields.
```

### Comparing `trytond_account_invoice_history-6.6.1/trytond_account_invoice_history.egg-info/SOURCES.txt` & `trytond_account_invoice_history-6.8.0/trytond_account_invoice_history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

