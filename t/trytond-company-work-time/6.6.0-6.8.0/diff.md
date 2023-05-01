# Comparing `tmp/trytond_company_work_time-6.6.0.tar.gz` & `tmp/trytond_company_work_time-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_company_work_time-6.6.0.tar", last modified: Mon Oct 31 15:49:59 2022, max compression
+gzip compressed data, was "trytond_company_work_time-6.8.0.tar", last modified: Mon May  1 11:43:08 2023, max compression
```

## Comparing `trytond_company_work_time-6.6.0.tar` & `trytond_company_work_time-6.8.0.tar`

### file list

```diff
@@ -1,59 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:49:59.508424 trytond_company_work_time-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_company_work_time-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_company_work_time-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-10-31 15:49:58.000000 trytond_company_work_time-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_company_work_time-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2171 2022-10-31 15:49:57.000000 trytond_company_work_time-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:49:57.000000 trytond_company_work_time-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:31.000000 trytond_company_work_time-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_company_work_time-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2022-10-31 15:49:59.508424 trytond_company_work_time-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2019-02-13 10:09:31.000000 trytond_company_work_time-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2021-12-11 16:59:33.000000 trytond_company_work_time-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2022-10-23 16:32:09.000000 trytond_company_work_time-6.6.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2019-02-13 10:09:31.000000 trytond_company_work_time-6.6.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:49:59.505090 trytond_company_work_time-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2019-02-13 10:09:31.000000 trytond_company_work_time-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:49:59.505090 trytond_company_work_time-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      690 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      620 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      612 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      616 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      580 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2022-10-29 07:50:35.000000 trytond_company_work_time-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2020-03-01 11:49:45.000000 trytond_company_work_time-6.6.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:49:59.508424 trytond_company_work_time-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5060 2022-10-29 07:39:10.000000 trytond_company_work_time-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:49:59.505090 trytond_company_work_time-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_company_work_time-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2022-04-16 16:30:56.000000 trytond_company_work_time-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-10-31 15:10:09.000000 trytond_company_work_time-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 15:49:56.000000 trytond_company_work_time-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:49:59.508424 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2022-10-31 15:49:58.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1393 2022-10-31 15:49:59.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:49:58.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 15:49:58.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:52.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2022-10-31 15:49:58.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:49:58.000000 trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:49:59.505090 trytond_company_work_time-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2021-03-24 12:36:50.000000 trytond_company_work_time-6.6.0/view/company_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:08.336890 trytond_company_work_time-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2334 2023-05-01 11:02:11.000000 trytond_company_work_time-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:02:11.000000 trytond_company_work_time-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_company_work_time-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2023-05-01 11:43:08.336890 trytond_company_work_time-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-01-16 14:00:20.000000 trytond_company_work_time-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-01-16 14:00:20.000000 trytond_company_work_time-6.8.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:08.333557 trytond_company_work_time-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-01-16 14:00:20.000000 trytond_company_work_time-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:08.333557 trytond_company_work_time-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      690 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      620 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      686 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      612 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      616 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      580 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-29 08:02:41.000000 trytond_company_work_time-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:43:08.336890 trytond_company_work_time-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4246 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:08.333557 trytond_company_work_time-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:02:05.000000 trytond_company_work_time-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:08.336890 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2023-05-01 11:43:07.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1367 2023-05-01 11:43:08.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:43:07.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:43:07.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-05-01 11:43:07.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:43:07.000000 trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:43:08.333557 trytond_company_work_time-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      710 2023-04-15 07:12:15.000000 trytond_company_work_time-6.8.0/view/company_form.xml
```

### Comparing `trytond_company_work_time-6.6.0/CHANGELOG` & `trytond_company_work_time-6.8.0/CHANGELOG`

 * *Files 14% similar despite different names*

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

### Comparing `trytond_company_work_time-6.6.0/COPYRIGHT` & `trytond_company_work_time-6.8.0/COPYRIGHT`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2022 Cédric Krier.
+Copyright (C) 2009-2023 Cédric Krier.
 Copyright (C) 2009-2012 Bertrand Chenal.
-Copyright (C) 2009-2022 B2CK SPRL.
+Copyright (C) 2009-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_company_work_time-6.6.0/LICENSE` & `trytond_company_work_time-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/PKG-INFO` & `trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_company_work_time
-Version: 6.6.0
+Name: trytond-company-work-time
+Version: 6.8.0
 Summary: Tryton module to add work time on company
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
-Project-URL: Source Code, https://hg.tryton.org/modules/company_work_time
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton company work time
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
 License-File: LICENSE
 
 Company Work Time Module
 ########################
 
 The Company Work Time module adds 4 new fields (Hours per Work Day,
 Hours per Work Week, Hours per Work Month, Hours per Work Year) on the
```

### Comparing `trytond_company_work_time-6.6.0/company.py` & `trytond_company_work_time-6.8.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/company.xml` & `trytond_company_work_time-6.8.0/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/bg.po` & `trytond_company_work_time-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/ca.po` & `trytond_company_work_time-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/de.po` & `trytond_company_work_time-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/es.po` & `trytond_company_work_time-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/et.po` & `trytond_company_work_time-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/fa.po` & `trytond_company_work_time-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/fr.po` & `trytond_company_work_time-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/hu.po` & `trytond_company_work_time-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/id.po` & `trytond_company_work_time-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/it.po` & `trytond_company_work_time-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/lo.po` & `trytond_company_work_time-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/lt.po` & `trytond_company_work_time-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/nl.po` & `trytond_company_work_time-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/pl.po` & `trytond_company_work_time-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/pt.po` & `trytond_company_work_time-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/ro.po` & `trytond_company_work_time-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/ru.po` & `trytond_company_work_time-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/locale/sl.po` & `trytond_company_work_time-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/res.py` & `trytond_company_work_time-6.8.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_company_work_time-6.6.0/setup.py` & `trytond_company_work_time-6.8.0/setup.py`

 * *Files 7% similar despite different names*

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
 name = 'trytond_company_work_time'
 
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
     description='Tryton module to add work time on company',
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
-        "Source Code": 'https://hg.tryton.org/modules/company_work_time',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton company work time',
     package_dir={'trytond.modules.company_work_time': '.'},
     packages=(
         ['trytond.modules.company_work_time']
         + ['trytond.modules.company_work_time.%s' % p for p in find_packages()]
         ),
@@ -123,24 +100,23 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     company_work_time = trytond.modules.company_work_time
     """,
     )
```

### Comparing `trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/PKG-INFO` & `trytond_company_work_time-6.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-company-work-time
-Version: 6.6.0
+Name: trytond_company_work_time
+Version: 6.8.0
 Summary: Tryton module to add work time on company
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
-Project-URL: Source Code, https://hg.tryton.org/modules/company_work_time
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton company work time
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
 License-File: LICENSE
 
 Company Work Time Module
 ########################
 
 The Company Work Time module adds 4 new fields (Hours per Work Day,
 Hours per Work Week, Hours per Work Month, Hours per Work Year) on the
```

### Comparing `trytond_company_work_time-6.6.0/trytond_company_work_time.egg-info/SOURCES.txt` & `trytond_company_work_time-6.8.0/trytond_company_work_time.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
 company.py
@@ -42,14 +38,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/company_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_company_work_time-6.6.0/view/company_form.xml` & `trytond_company_work_time-6.8.0/view/company_form.xml`

 * *Files identical despite different names*

