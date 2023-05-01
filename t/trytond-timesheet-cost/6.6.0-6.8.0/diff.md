# Comparing `tmp/trytond_timesheet_cost-6.6.0.tar.gz` & `tmp/trytond_timesheet_cost-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_timesheet_cost-6.6.0.tar", last modified: Mon Oct 31 15:58:40 2022, max compression
+gzip compressed data, was "trytond_timesheet_cost-6.8.0.tar", last modified: Mon May  1 11:36:09 2023, max compression
```

## Comparing `trytond_timesheet_cost-6.6.0.tar` & `trytond_timesheet_cost-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:40.185994 trytond_timesheet_cost-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_timesheet_cost-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_timesheet_cost-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2022-10-31 15:58:38.000000 trytond_timesheet_cost-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:35.000000 trytond_timesheet_cost-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1593 2022-10-31 15:58:38.000000 trytond_timesheet_cost-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:58:37.000000 trytond_timesheet_cost-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:45.000000 trytond_timesheet_cost-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_timesheet_cost-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2022-10-31 15:58:40.185994 trytond_timesheet_cost-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      101 2019-06-04 16:49:46.000000 trytond_timesheet_cost-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2021-12-11 16:59:35.000000 trytond_timesheet_cost-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2022-10-11 19:49:59.000000 trytond_timesheet_cost-6.6.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2653 2019-12-05 21:37:26.000000 trytond_timesheet_cost-6.6.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:40.182661 trytond_timesheet_cost-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      101 2019-06-04 16:49:46.000000 trytond_timesheet_cost-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:40.182661 trytond_timesheet_cost-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1491 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1366 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1420 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1307 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1389 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1366 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1121 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1338 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1293 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1430 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1293 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1344 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1432 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2022-10-29 07:50:32.000000 trytond_timesheet_cost-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2019-08-09 14:52:54.000000 trytond_timesheet_cost-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:58:40.185994 trytond_timesheet_cost-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5049 2022-10-29 07:39:12.000000 trytond_timesheet_cost-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:40.182661 trytond_timesheet_cost-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:58.000000 trytond_timesheet_cost-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1899 2022-04-16 16:30:58.000000 trytond_timesheet_cost-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2021-12-11 16:59:35.000000 trytond_timesheet_cost-6.6.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)      989 2019-02-13 10:09:45.000000 trytond_timesheet_cost-6.6.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2022-10-31 15:10:09.000000 trytond_timesheet_cost-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2022-10-31 15:58:36.000000 trytond_timesheet_cost-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:40.185994 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2022-10-31 15:58:39.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1582 2022-10-31 15:58:40.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:58:39.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2022-10-31 15:58:39.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:48.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      112 2022-10-31 15:58:39.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:58:39.000000 trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:58:40.182661 trytond_timesheet_cost-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2019-02-13 10:09:45.000000 trytond_timesheet_cost-6.6.0/view/employee_cost_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2019-02-13 10:09:45.000000 trytond_timesheet_cost-6.6.0/view/employee_cost_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2019-10-11 21:50:16.000000 trytond_timesheet_cost-6.6.0/view/employee_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:09.251690 trytond_timesheet_cost-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1756 2023-05-01 10:57:30.000000 trytond_timesheet_cost-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 10:57:30.000000 trytond_timesheet_cost-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_timesheet_cost-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2023-05-01 11:36:09.251690 trytond_timesheet_cost-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2653 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:09.251690 trytond_timesheet_cost-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:09.248356 trytond_timesheet_cost-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1366 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1307 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1389 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1366 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1121 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1338 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1293 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1430 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1293 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1344 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1432 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-04-29 08:02:39.000000 trytond_timesheet_cost-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:36:09.251690 trytond_timesheet_cost-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4238 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:09.248356 trytond_timesheet_cost-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2587 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      989 2023-01-16 14:00:21.000000 trytond_timesheet_cost-6.8.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-05-01 10:57:25.000000 trytond_timesheet_cost-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:09.251690 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2023-05-01 11:36:08.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1556 2023-05-01 11:36:09.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:36:08.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-05-01 11:36:08.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      112 2023-05-01 11:36:08.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:36:08.000000 trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:09.248356 trytond_timesheet_cost-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_timesheet_cost-6.8.0/view/employee_cost_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-01-16 14:00:21.000000 trytond_timesheet_cost-6.8.0/view/employee_cost_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_timesheet_cost-6.8.0/view/employee_form.xml
```

### Comparing `trytond_timesheet_cost-6.6.0/CHANGELOG` & `trytond_timesheet_cost-6.8.0/CHANGELOG`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_timesheet_cost-6.6.0/LICENSE` & `trytond_timesheet_cost-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/PKG-INFO` & `trytond_timesheet_cost-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet_cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add cost on timesheet
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
-Project-URL: Source Code, https://hg.tryton.org/modules/timesheet_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton timesheet cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,20 +39,20 @@
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
 
 Timesheet Cost Module
 #####################
 
 The timesheet cost module adds cost price per employee.
```

### Comparing `trytond_timesheet_cost-6.6.0/company.py` & `trytond_timesheet_cost-6.8.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/company.xml` & `trytond_timesheet_cost-6.8.0/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/bg.po` & `trytond_timesheet_cost-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/ca.po` & `trytond_timesheet_cost-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/cs.po` & `trytond_timesheet_cost-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/de.po` & `trytond_timesheet_cost-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/es.po` & `trytond_timesheet_cost-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/es_419.po` & `trytond_timesheet_cost-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/et.po` & `trytond_timesheet_cost-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/fa.po` & `trytond_timesheet_cost-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/fi.po` & `trytond_timesheet_cost-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/fr.po` & `trytond_timesheet_cost-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/hu.po` & `trytond_timesheet_cost-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/id.po` & `trytond_timesheet_cost-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/it.po` & `trytond_timesheet_cost-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/lo.po` & `trytond_timesheet_cost-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/lt.po` & `trytond_timesheet_cost-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/nl.po` & `trytond_timesheet_cost-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/pl.po` & `trytond_timesheet_cost-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/pt.po` & `trytond_timesheet_cost-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/ro.po` & `trytond_timesheet_cost-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/ru.po` & `trytond_timesheet_cost-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/sl.po` & `trytond_timesheet_cost-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/tr.po` & `trytond_timesheet_cost-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/uk.po` & `trytond_timesheet_cost-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/locale/zh_CN.po` & `trytond_timesheet_cost-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/setup.py` & `trytond_timesheet_cost-6.8.0/setup.py`

 * *Files 11% similar despite different names*

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
 name = 'trytond_timesheet_cost'
 
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
 
 requires = ['python-sql >= 0.4']
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
     description='Tryton module to add cost on timesheet',
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
-        "Source Code": 'https://hg.tryton.org/modules/timesheet_cost',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton timesheet cost',
     package_dir={'trytond.modules.timesheet_cost': '.'},
     packages=(
         ['trytond.modules.timesheet_cost']
         + ['trytond.modules.timesheet_cost.%s' % p for p in find_packages()]
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
     timesheet_cost = trytond.modules.timesheet_cost
     """,
     )
```

### Comparing `trytond_timesheet_cost-6.6.0/tests/test_module.py` & `trytond_timesheet_cost-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/timesheet.py` & `trytond_timesheet_cost-6.8.0/timesheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from sql import Null
 
 from trytond.model import fields
 from trytond.pool import Pool, PoolMeta
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 from .company import price_digits
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'timesheet.line'
 
@@ -61,17 +61,17 @@
 
     @classmethod
     def write(cls, *args):
         super().write(*args)
         cls.sync_cost(sum(args[0:None:2], []))
 
     @classmethod
+    @without_check_access
     def sync_cost(cls, lines):
-        with Transaction().set_context(_check_access=False):
-            to_write = []
-            lines = cls.browse(lines)
-            for line in lines:
-                cost_price = line.employee.compute_cost_price(date=line.date)
-                if cost_price != line.cost_price:
-                    to_write.extend([[line], {'cost_price': cost_price}])
-            if to_write:
-                cls.write(*to_write)
+        to_write = []
+        lines = cls.browse(lines)
+        for line in lines:
+            cost_price = line.employee.compute_cost_price(date=line.date)
+            if cost_price != line.cost_price:
+                to_write.extend([[line], {'cost_price': cost_price}])
+        if to_write:
+            cls.write(*to_write)
```

### Comparing `trytond_timesheet_cost-6.6.0/timesheet.xml` & `trytond_timesheet_cost-6.8.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/PKG-INFO` & `trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-timesheet-cost
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add cost on timesheet
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
-Project-URL: Source Code, https://hg.tryton.org/modules/timesheet_cost
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton timesheet cost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,20 +39,20 @@
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
 
 Timesheet Cost Module
 #####################
 
 The timesheet cost module adds cost price per employee.
```

### Comparing `trytond_timesheet_cost-6.6.0/trytond_timesheet_cost.egg-info/SOURCES.txt` & `trytond_timesheet_cost-6.8.0/trytond_timesheet_cost.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

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
@@ -48,14 +44,15 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/employee_cost_price_form.xml
 ./view/employee_cost_price_tree.xml
 ./view/employee_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

