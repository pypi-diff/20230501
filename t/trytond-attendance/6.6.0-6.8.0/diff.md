# Comparing `tmp/trytond_attendance-6.6.0.tar.gz` & `tmp/trytond_attendance-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_attendance-6.6.0.tar", last modified: Mon Oct 31 15:55:32 2022, max compression
+gzip compressed data, was "trytond_attendance-6.8.0.tar", last modified: Mon May  1 11:44:57 2023, max compression
```

## Comparing `trytond_attendance-6.6.0.tar` & `trytond_attendance-6.8.0.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.899938 trytond_attendance-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_attendance-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_attendance-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2022-10-31 15:55:31.000000 trytond_attendance-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_attendance-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-10-31 15:55:30.000000 trytond_attendance-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2022-10-31 15:55:30.000000 trytond_attendance-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35310 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_attendance-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2022-10-31 15:55:32.899938 trytond_attendance-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2021-12-11 16:59:33.000000 trytond_attendance-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15214 2022-10-20 08:55:44.000000 trytond_attendance-6.6.0/attendance.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15304 2021-10-07 13:08:59.000000 trytond_attendance-6.6.0/attendance.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.896604 trytond_attendance-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2020-07-09 09:37:03.000000 trytond_attendance-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.896604 trytond_attendance-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:31.000000 trytond_attendance-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/icons/tryton-attendance.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.896604 trytond_attendance-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6277 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6496 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6252 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6374 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5700 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5281 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6199 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5093 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5146 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5161 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5099 2022-10-29 07:50:36.000000 trytond_attendance-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:55:32.899938 trytond_attendance-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5201 2022-10-29 07:39:10.000000 trytond_attendance-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.896604 trytond_attendance-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_attendance-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2021-10-07 13:08:59.000000 trytond_attendance-6.6.0/tests/scenario_attendance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2020-05-20 22:05:02.000000 trytond_attendance-6.6.0/tests/scenario_attendance_sheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2425 2020-05-20 22:04:24.000000 trytond_attendance-6.6.0/tests/scenario_attendance_timesheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2022-04-16 16:30:56.000000 trytond_attendance-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_attendance-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-10-31 15:10:09.000000 trytond_attendance-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2022-10-31 15:55:29.000000 trytond_attendance-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.899938 trytond_attendance-6.6.0/trytond_attendance.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2022-10-31 15:55:32.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2192 2022-10-31 15:55:32.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:55:32.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2022-10-31 15:55:32.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-10-13 07:23:31.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2022-10-31 15:55:32.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:55:32.000000 trytond_attendance-6.6.0/trytond_attendance.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:55:32.896604 trytond_attendance-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/attendance_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2022-04-13 16:47:05.000000 trytond_attendance-6.6.0/view/attendance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2022-04-08 16:23:26.000000 trytond_attendance-6.6.0/view/period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/sheet_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/sheet_form_timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/sheet_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/sheet_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2022-04-08 16:23:26.000000 trytond_attendance-6.6.0/view/sheet_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2020-05-20 21:51:27.000000 trytond_attendance-6.6.0/view/sheet_list_timesheet.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.321576 trytond_attendance-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-05-01 11:03:22.000000 trytond_attendance-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-05-01 11:03:21.000000 trytond_attendance-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35310 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2121 2023-05-01 11:44:57.321576 trytond_attendance-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15214 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/attendance.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15304 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/attendance.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.318243 trytond_attendance-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.318243 trytond_attendance-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/icons/tryton-attendance.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.311576 trytond_attendance-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6277 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6530 2023-04-30 10:46:36.000000 trytond_attendance-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6252 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6374 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5700 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5281 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6201 2023-04-30 10:46:36.000000 trytond_attendance-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5093 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5146 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5161 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5099 2023-04-29 08:02:43.000000 trytond_attendance-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:44:57.321576 trytond_attendance-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4395 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.311576 trytond_attendance-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tests/scenario_attendance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tests/scenario_attendance_sheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tests/scenario_attendance_timesheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-05-01 11:03:16.000000 trytond_attendance-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.318243 trytond_attendance-6.8.0/trytond_attendance.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2121 2023-05-01 11:44:56.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2166 2023-05-01 11:44:57.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:44:56.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:44:56.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-05-01 11:44:56.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:44:56.000000 trytond_attendance-6.8.0/trytond_attendance.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:57.314910 trytond_attendance-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/attendance_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/attendance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/sheet_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/sheet_form_timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/sheet_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/sheet_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/sheet_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_attendance-6.8.0/view/sheet_list_timesheet.xml
```

### Comparing `trytond_attendance-6.6.0/COPYRIGHT` & `trytond_attendance-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2020 Sergi Almacellas Abellana
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

### Comparing `trytond_attendance-6.6.0/LICENSE` & `trytond_attendance-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/PKG-INFO` & `trytond_attendance-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_attendance
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for recording employee attendance
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
-Project-URL: Source Code, https://hg.tryton.org/modules/attendance
+Project-URL: Source Code, https://code.tryton.org/tryton
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -35,18 +35,18 @@
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
 
 doc/index.rst
```

### Comparing `trytond_attendance-6.6.0/__init__.py` & `trytond_attendance-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/attendance.py` & `trytond_attendance-6.8.0/attendance.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/attendance.xml` & `trytond_attendance-6.8.0/attendance.xml`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/doc/index.rst` & `trytond_attendance-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/icons/LICENSE` & `trytond_attendance-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/bg.po` & `trytond_attendance-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/ca.po` & `trytond_attendance-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/cs.po` & `trytond_attendance-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/de.po` & `trytond_attendance-6.8.0/locale/de.po`

 * *Files 4% similar despite different names*

```diff
@@ -40,39 +40,39 @@
 
 msgctxt "field:attendance.sheet,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:attendance.sheet,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:attendance.sheet,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
 msgctxt "field:attendance.sheet,lines:"
 msgid "Lines"
 msgstr "Einträge"
 
 msgctxt "field:attendance.sheet,timesheet_duration:"
 msgid "Timesheet Duration"
-msgstr "Zeiterfassung Dauer"
+msgstr "Erfasste Gesamtzeit"
 
 msgctxt "field:attendance.sheet.line,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:attendance.sheet.line,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:attendance.sheet.line,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:attendance.sheet.line,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
 msgctxt "field:attendance.sheet.line,from_:"
 msgid "From"
@@ -117,15 +117,15 @@
 
 msgctxt "model:ir.action,name:act_attendance"
 msgid "Attendances"
 msgstr "Anwesenheiten"
 
 msgctxt "model:ir.action,name:act_period_list"
 msgid "Periods"
-msgstr "Lagerperioden"
+msgstr "Anwesenheitszeiträume"
 
 msgctxt "model:ir.action,name:act_sheet"
 msgid "Sheets"
 msgstr "Listen"
 
 msgctxt "model:ir.message,text:msg_close_period_previous_open"
 msgid "To close period \"%(period)s\" you must first close \"%(other_period)s\"."
@@ -212,15 +212,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_main_attendance"
 msgid "Attendance"
 msgstr "Anwesenheit"
 
 msgctxt "model:ir.ui.menu,name:menu_period_list"
 msgid "Periods"
-msgstr "Lagerperioden"
+msgstr "Anwesenheitszeiträume"
 
 msgctxt "model:ir.ui.menu,name:menu_sheet"
 msgid "Sheets"
 msgstr "Listen"
 
 msgctxt "model:res.group,name:group_attendance_admin"
 msgid "Attendance Administration"
```

### Comparing `trytond_attendance-6.6.0/locale/es.po` & `trytond_attendance-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/es_419.po` & `trytond_attendance-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/et.po` & `trytond_attendance-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/fa.po` & `trytond_attendance-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/fi.po` & `trytond_attendance-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/fr.po` & `trytond_attendance-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/hu.po` & `trytond_attendance-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/id.po` & `trytond_attendance-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/it.po` & `trytond_attendance-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/lo.po` & `trytond_attendance-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/lt.po` & `trytond_attendance-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/nl.po` & `trytond_attendance-6.8.0/locale/nl.po`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 msgctxt "field:attendance.line,employee:"
 msgid "Employee"
 msgstr "Werknemer"
 
 msgctxt "field:attendance.line,type:"
 msgid "Type"
-msgstr "Type"
+msgstr "Soort"
 
 msgctxt "field:attendance.period,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:attendance.period,ends_at:"
 msgid "Ends at"
@@ -40,51 +40,51 @@
 
 msgctxt "field:attendance.sheet,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:attendance.sheet,duration:"
 msgid "Duration"
-msgstr "duur"
+msgstr "Duur"
 
 msgctxt "field:attendance.sheet,employee:"
 msgid "Employee"
 msgstr "Werknemer"
 
 msgctxt "field:attendance.sheet,lines:"
 msgid "Lines"
 msgstr "Regels"
 
 msgctxt "field:attendance.sheet,timesheet_duration:"
 msgid "Timesheet Duration"
-msgstr "Urenstaatduur"
+msgstr "Urenstaat Duur"
 
 msgctxt "field:attendance.sheet.line,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
 msgctxt "field:attendance.sheet.line,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:attendance.sheet.line,duration:"
 msgid "Duration"
-msgstr "duur"
+msgstr "Duur"
 
 msgctxt "field:attendance.sheet.line,employee:"
 msgid "Employee"
 msgstr "Werknemer"
 
 msgctxt "field:attendance.sheet.line,from_:"
 msgid "From"
 msgstr "Van"
 
 msgctxt "field:attendance.sheet.line,sheet:"
 msgid "Sheet"
-msgstr "Fiche"
+msgstr "Staat"
 
 msgctxt "field:attendance.sheet.line,to:"
 msgid "To"
 msgstr "Tot"
 
 msgctxt "help:attendance.line,company:"
 msgid "The company which the employee attended."
@@ -104,141 +104,141 @@
 
 msgctxt "model:attendance.period,name:"
 msgid "Attendance Period"
 msgstr "Aanwezigheidsperiode"
 
 msgctxt "model:attendance.sheet,name:"
 msgid "Attendance Sheet"
-msgstr "Aanwezigheids fiche"
+msgstr "Aanwezigheidsstaat"
 
 msgctxt "model:attendance.sheet.line,name:"
 msgid "Attendance SheetLine"
-msgstr "Lijn aanwezigheids- fiche"
+msgstr "Aanwezigheidsstaat regel"
 
 msgctxt "model:ir.action,name:act_attendance"
 msgid "Attendances"
 msgstr "Aanwezigen"
 
 msgctxt "model:ir.action,name:act_period_list"
 msgid "Periods"
 msgstr "Periodes"
 
 msgctxt "model:ir.action,name:act_sheet"
 msgid "Sheets"
-msgstr "Fiche"
+msgstr "Staten"
 
 msgctxt "model:ir.message,text:msg_close_period_previous_open"
 msgid "To close period \"%(period)s\" you must first close \"%(other_period)s\"."
 msgstr ""
-"Om periode \"%(period)s\" te sluiten, moet je eerst \"% other_period)s\" "
+"Om periode \"%(period)s\" te sluiten, moet u eerst \"% other_period)s\" "
 "sluiten."
 
 msgctxt "model:ir.message,text:msg_delete_period_close"
 msgid "To delete attendance \"%(attendance)s\" you must reopen period \"%(period)s\"."
 msgstr ""
 "Om aanwezigheid \"%(attendance)s\" te verwijderen, moet u periode "
 "\"%(period)s\" opnieuw openen."
 
 msgctxt "model:ir.message,text:msg_draft_period_previous_closed"
 msgid ""
 "To change period \"%(period)s\" you must first change \"%(other_period)s\" "
 "to draft."
 msgstr ""
-"Om periode \"%(period)s\" te sluiten, moet je eerst \"% other_period)s\" "
+"Om periode \"%(period)s\" te sluiten, moet u eerst \"% other_period)s\" "
 "terug in concept zetten."
 
 msgctxt "model:ir.message,text:msg_modify_period_close"
 msgid "To modify attendance \"%(attendance)s\" you must reopen period \"%(period)s\"."
 msgstr ""
 "Om aanwezigheid \"%(attendance)s\" te wijzigen, moet u periode "
 "\"%(period)s\" opnieuw openen."
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
-msgstr "Afsluiten"
+msgstr "Sluiten"
 
 msgctxt "model:ir.model.button,string:period_draft_button"
 msgid "Draft"
 msgstr "Concept"
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance"
 msgid "Own attendance"
-msgstr "Eigen aanwezigheden"
+msgstr "Eigen aanwezigheid"
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_admin"
 msgid "Any attendance"
-msgstr "Elke aanwezigheid"
+msgstr "Alle aanwezigheid"
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.rule.group,name:rule_group_period_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet"
 msgid "Own attendance sheet"
-msgstr "Eigen aanwezigheids-fiche"
+msgstr "Eigen aanwezigheidsstaat"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_admin"
 msgid "Any attendance sheet"
-msgstr "elke aanwezigheids-fiche"
+msgstr "Alle aanwezigheidsstaten"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_line"
 msgid "Own attendance sheet line"
-msgstr "Eigen aanwezigheids-fiche lijn"
+msgstr "Eigen aanwezigheidsstaat regel"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_line_admin"
 msgid "Any attendance sheet line"
-msgstr "Elke aanwezigheids-fiche lijn"
+msgstr "Alle aanwezigheidsstaat regel"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_line_companies"
 msgid "User in companies"
 msgstr "Gebruiker in bedrijven"
 
 msgctxt "model:ir.ui.menu,name:menu_attendance"
 msgid "Attendances"
-msgstr "Aanwezigheden"
+msgstr "Aanwezigheid"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Instellingen"
 
 msgctxt "model:ir.ui.menu,name:menu_main_attendance"
 msgid "Attendance"
-msgstr "Aanwezigheden"
+msgstr "Aanwezigheid"
 
 msgctxt "model:ir.ui.menu,name:menu_period_list"
 msgid "Periods"
 msgstr "Periodes"
 
 msgctxt "model:ir.ui.menu,name:menu_sheet"
 msgid "Sheets"
-msgstr "Fiches"
+msgstr "Staten"
 
 msgctxt "model:res.group,name:group_attendance_admin"
 msgid "Attendance Administration"
-msgstr "Aanwezigheidsadministratie"
+msgstr "Aanwezigheid Administratie"
 
 msgctxt "selection:attendance.line,type:"
 msgid "In"
-msgstr "In"
+msgstr "Inkomend"
 
 msgctxt "selection:attendance.line,type:"
 msgid "Out"
-msgstr "Uit"
+msgstr "Uitgaand"
 
 msgctxt "selection:attendance.period,state:"
 msgid "Closed"
-msgstr "Afgesloten"
+msgstr "Gesloten"
 
 msgctxt "selection:attendance.period,state:"
 msgid "Draft"
 msgstr "Concept"
 
 msgctxt "view:attendance.line:"
 msgid "Date"
```

### Comparing `trytond_attendance-6.6.0/locale/pl.po` & `trytond_attendance-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/pt.po` & `trytond_attendance-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/ro.po` & `trytond_attendance-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/ru.po` & `trytond_attendance-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/sl.po` & `trytond_attendance-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/tr.po` & `trytond_attendance-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/uk.po` & `trytond_attendance-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/locale/zh_CN.po` & `trytond_attendance-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/message.xml` & `trytond_attendance-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/setup.py` & `trytond_attendance-6.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     if slice:
         content = '\n'.join(content.splitlines()[slice])
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
 name = 'trytond_attendance'
 
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
     get_require_version('trytond_timesheet'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for recording employee attendance',
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
-        "Source Code": 'https://hg.tryton.org/modules/attendance',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='',
     package_dir={'trytond.modules.attendance': '.'},
     packages=(
         ['trytond.modules.attendance']
         + ['trytond.modules.attendance.%s' % p
             for p in find_packages()]
@@ -129,27 +107,26 @@
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
     attendance = trytond.modules.attendance
     """,
     )
```

### Comparing `trytond_attendance-6.6.0/tests/scenario_attendance.rst` & `trytond_attendance-6.8.0/tests/scenario_attendance.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/tests/scenario_attendance_sheet.rst` & `trytond_attendance-6.8.0/tests/scenario_attendance_sheet.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/tests/scenario_attendance_timesheet.rst` & `trytond_attendance-6.8.0/tests/scenario_attendance_timesheet.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-6.6.0/trytond_attendance.egg-info/PKG-INFO` & `trytond_attendance-6.8.0/trytond_attendance.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-attendance
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for recording employee attendance
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
-Project-URL: Source Code, https://hg.tryton.org/modules/attendance
+Project-URL: Source Code, https://code.tryton.org/tryton
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -35,18 +35,18 @@
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
 
 doc/index.rst
```

### Comparing `trytond_attendance-6.6.0/trytond_attendance.egg-info/SOURCES.txt` & `trytond_attendance-6.8.0/trytond_attendance.egg-info/SOURCES.txt`

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
 attendance.py
@@ -58,14 +54,15 @@
 ./view/period_list.xml
 ./view/sheet_form.xml
 ./view/sheet_form_timesheet.xml
 ./view/sheet_line_form.xml
 ./view/sheet_line_list.xml
 ./view/sheet_list.xml
 ./view/sheet_list_timesheet.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-attendance.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

