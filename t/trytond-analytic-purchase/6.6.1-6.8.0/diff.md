# Comparing `tmp/trytond_analytic_purchase-6.6.1.tar.gz` & `tmp/trytond_analytic_purchase-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_analytic_purchase-6.6.1.tar", last modified: Sat Mar  4 12:06:58 2023, max compression
+gzip compressed data, was "trytond_analytic_purchase-6.8.0.tar", last modified: Mon May  1 11:50:43 2023, max compression
```

## Comparing `trytond_analytic_purchase-6.6.1.tar` & `trytond_analytic_purchase-6.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:06:58.923045 trytond_analytic_purchase-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2450 2023-03-04 12:06:53.000000 trytond_analytic_purchase-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-03-04 12:06:52.000000 trytond_analytic_purchase-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2449 2023-03-04 12:06:58.923045 trytond_analytic_purchase-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:06:58.919712 trytond_analytic_purchase-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:06:58.913046 trytond_analytic_purchase-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2342 2023-02-27 17:46:08.000000 trytond_analytic_purchase-6.6.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 12:06:58.923045 trytond_analytic_purchase-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4448 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:06:58.916379 trytond_analytic_purchase-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4654 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/tests/scenario_analytic_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      542 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      109 2022-12-19 12:03:07.000000 trytond_analytic_purchase-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:06:58.923045 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2449 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 12:06:58.000000 trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:06:58.916379 trytond_analytic_purchase-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-12-19 12:02:49.000000 trytond_analytic_purchase-6.6.1/view/purchase_line_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:43.579207 trytond_analytic_purchase-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-05-01 11:07:07.000000 trytond_analytic_purchase-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:07:07.000000 trytond_analytic_purchase-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_analytic_purchase-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2439 2023-05-01 11:50:43.579207 trytond_analytic_purchase-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:43.575873 trytond_analytic_purchase-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:43.572540 trytond_analytic_purchase-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-29 08:02:45.000000 trytond_analytic_purchase-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2300 2023-04-21 08:36:08.000000 trytond_analytic_purchase-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-01-16 14:00:20.000000 trytond_analytic_purchase-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:50:43.579207 trytond_analytic_purchase-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4410 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:43.575873 trytond_analytic_purchase-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4535 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/tests/scenario_analytic_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_analytic_purchase-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      109 2023-05-01 11:07:02.000000 trytond_analytic_purchase-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:43.579207 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2439 2023-05-01 11:50:42.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-05-01 11:50:43.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:50:42.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:50:42.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 11:50:42.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:50:42.000000 trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:43.575873 trytond_analytic_purchase-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:20.000000 trytond_analytic_purchase-6.8.0/view/purchase_line_form.xml
```

### Comparing `trytond_analytic_purchase-6.6.1/CHANGELOG` & `trytond_analytic_purchase-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-03-04
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

### Comparing `trytond_analytic_purchase-6.6.1/COPYRIGHT` & `trytond_analytic_purchase-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_analytic_purchase-6.6.1/LICENSE` & `trytond_analytic_purchase-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_analytic_purchase-6.6.1/PKG-INFO` & `trytond_analytic_purchase-6.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_analytic_purchase
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add analytic accounting on purchase
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
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_purchase
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account purchase
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
 
 Analytic Purchase Module
 ########################
 
 The analytic purchase module allows to set analytic accounts on purchase line.
```

### Comparing `trytond_analytic_purchase-6.6.1/doc/conf.py` & `trytond_analytic_purchase-6.8.0/doc/conf.py`

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

### Comparing `trytond_analytic_purchase-6.6.1/purchase.py` & `trytond_analytic_purchase-6.8.0/purchase.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,17 @@
         origins = super(AnalyticAccountEntry, cls)._get_origin()
         return origins + ['purchase.line']
 
     @fields.depends('origin')
     def on_change_with_company(self, name=None):
         pool = Pool()
         PurchaseLine = pool.get('purchase.line')
-        company = super(AnalyticAccountEntry, self).on_change_with_company(
-            name)
+        company = super().on_change_with_company(name)
         if isinstance(self.origin, PurchaseLine) and self.origin.purchase:
-            company = self.origin.purchase.company.id
+            company = self.origin.purchase.company
         return company
 
     @classmethod
     def search_company(cls, name, clause):
         operator = clause[1]
         if operator.startswith('!') or operator.startswith('not '):
             bool_op = 'AND'
```

### Comparing `trytond_analytic_purchase-6.6.1/setup.py` & `trytond_analytic_purchase-6.8.0/setup.py`

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
@@ -34,38 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_analytic_purchase'
 
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
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module to add analytic accounting on purchase',
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
-        "Source Code": 'https://hg.tryton.org/modules/analytic_purchase',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton analytic account purchase',
     package_dir={'trytond.modules.analytic_purchase': '.'},
     packages=(
         ['trytond.modules.analytic_purchase']
         + ['trytond.modules.analytic_purchase.%s' % p for p in find_packages()]
         ),
@@ -101,24 +101,24 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_analytic_purchase-6.6.1/tests/scenario_analytic_purchase.rst` & `trytond_analytic_purchase-6.8.0/tests/scenario_analytic_purchase.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 ==========================
 Analytic Purchase Scenario
 ==========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from operator import attrgetter
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('analytic_purchase')
 
 Create company::
```

### Comparing `trytond_analytic_purchase-6.6.1/tox.ini` & `trytond_analytic_purchase-6.8.0/tox.ini`

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
-    coverage run --include=./**/analytic_purchase/* -m unittest discover -s tests
-    coverage report --include=./**/analytic_purchase/* --omit=*/tests/*
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

### Comparing `trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/PKG-INFO` & `trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-analytic-purchase
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to add analytic accounting on purchase
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
-Project-URL: Source Code, https://hg.tryton.org/modules/analytic_purchase
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton analytic account purchase
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
 
 Analytic Purchase Module
 ########################
 
 The analytic purchase module allows to set analytic accounts on purchase line.
```

### Comparing `trytond_analytic_purchase-6.6.1/trytond_analytic_purchase.egg-info/SOURCES.txt` & `trytond_analytic_purchase-6.8.0/trytond_analytic_purchase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

