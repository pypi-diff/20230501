# Comparing `tmp/trytond_timesheet-6.6.0.tar.gz` & `tmp/trytond_timesheet-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_timesheet-6.6.0.tar", last modified: Mon Oct 31 15:54:19 2022, max compression
+gzip compressed data, was "trytond_timesheet-6.8.0.tar", last modified: Mon May  1 11:38:07 2023, max compression
```

## Comparing `trytond_timesheet-6.6.0.tar` & `trytond_timesheet-6.8.0.tar`

### file list

```diff
@@ -1,81 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.502204 trytond_timesheet-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_timesheet-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_timesheet-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-10-31 15:54:18.000000 trytond_timesheet-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:35.000000 trytond_timesheet-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2716 2022-10-31 15:54:17.000000 trytond_timesheet-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:54:17.000000 trytond_timesheet-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_timesheet-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3092 2022-10-31 15:54:19.502204 trytond_timesheet-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      919 2019-06-04 16:49:46.000000 trytond_timesheet-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      672 2021-12-11 16:59:35.000000 trytond_timesheet-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.498870 trytond_timesheet-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      919 2019-06-04 16:49:46.000000 trytond_timesheet-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1321 2019-06-04 16:49:46.000000 trytond_timesheet-6.6.0/doc/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2019-06-04 16:49:46.000000 trytond_timesheet-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.498870 trytond_timesheet-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:45.000000 trytond_timesheet-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2020-05-20 21:51:27.000000 trytond_timesheet-6.6.0/icons/tryton-timesheet.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13039 2022-10-11 19:49:59.000000 trytond_timesheet-6.6.0/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10228 2021-04-27 07:34:41.000000 trytond_timesheet-6.6.0/line.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.495537 trytond_timesheet-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     9371 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9902 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8502 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10106 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9983 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8435 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9025 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10508 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8489 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10027 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9060 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8280 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9027 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10246 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8550 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9736 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8814 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9805 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8058 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9521 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9570 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8585 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11175 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9502 2022-10-29 07:50:33.000000 trytond_timesheet-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      931 2019-08-09 14:52:53.000000 trytond_timesheet-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4620 2022-09-12 22:47:25.000000 trytond_timesheet-6.6.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:54:19.502204 trytond_timesheet-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5140 2022-10-29 07:39:12.000000 trytond_timesheet-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.498870 trytond_timesheet-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:58.000000 trytond_timesheet-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2022-04-16 16:30:58.000000 trytond_timesheet-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2021-02-27 17:17:02.000000 trytond_timesheet-6.6.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2022-10-31 15:10:09.000000 trytond_timesheet-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      146 2022-10-31 15:54:16.000000 trytond_timesheet-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.502204 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3092 2022-10-31 15:54:18.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2246 2022-10-31 15:54:19.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:54:18.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2022-10-31 15:54:18.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:49.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      100 2022-10-31 15:54:18.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:54:18.000000 trytond_timesheet-6.6.0/trytond_timesheet.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2020-03-01 11:49:51.000000 trytond_timesheet-6.6.0/user.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:19.498870 trytond_timesheet-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/view/hours_employee_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/view/hours_employee_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2021-10-07 13:09:32.000000 trytond_timesheet-6.6.0/view/hours_employee_monthly_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2019-10-11 21:50:16.000000 trytond_timesheet-6.6.0/view/hours_employee_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2021-10-07 13:09:32.000000 trytond_timesheet-6.6.0/view/hours_employee_weekly_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/view/line_enter_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/view/line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2022-04-08 16:23:27.000000 trytond_timesheet-6.6.0/view/line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/view/work_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      681 2021-04-27 07:34:41.000000 trytond_timesheet-6.6.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2019-02-13 10:09:45.000000 trytond_timesheet-6.6.0/view/work_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2019-10-11 21:50:16.000000 trytond_timesheet-6.6.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2019-10-11 21:50:16.000000 trytond_timesheet-6.6.0/view/work_list_report.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7794 2022-10-11 19:49:59.000000 trytond_timesheet-6.6.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5388 2021-04-27 07:34:41.000000 trytond_timesheet-6.6.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.009818 trytond_timesheet-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2985 2023-05-01 10:58:52.000000 trytond_timesheet-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 10:58:51.000000 trytond_timesheet-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2023-05-01 11:38:07.006484 trytond_timesheet-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      672 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.006484 trytond_timesheet-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1387 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/doc/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.006484 trytond_timesheet-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/icons/tryton-timesheet.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13136 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14834 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/line.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.003151 trytond_timesheet-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10163 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10858 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9294 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11155 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10948 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9227 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10045 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11300 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9281 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10999 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9852 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9072 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9819 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11038 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9342 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10672 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9606 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10597 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8850 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10313 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10362 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9377 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12376 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10483 2023-04-30 10:46:36.000000 trytond_timesheet-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4563 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:38:07.009818 trytond_timesheet-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4322 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.003151 trytond_timesheet-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      146 2023-05-01 10:58:46.000000 trytond_timesheet-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.006484 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2023-05-01 11:38:06.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2220 2023-05-01 11:38:06.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:38:06.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-05-01 11:38:06.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2023-05-01 11:38:06.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:38:06.000000 trytond_timesheet-6.8.0/trytond_timesheet.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/user.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:38:07.003151 trytond_timesheet-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/view/hours_employee_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/view/hours_employee_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/view/hours_employee_monthly_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-28 07:46:16.000000 trytond_timesheet-6.8.0/view/hours_employee_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/view/hours_employee_weekly_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/view/line_enter_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/view/line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-28 07:46:16.000000 trytond_timesheet-6.8.0/view/line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/view/work_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      681 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 trytond_timesheet-6.8.0/view/work_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/view/work_list_report.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7794 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5388 2023-04-15 07:12:15.000000 trytond_timesheet-6.8.0/work.xml
```

### Comparing `trytond_timesheet-6.6.0/CHANGELOG` & `trytond_timesheet-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Include supervised employees in timesheet reporting
+* Add access rules for weekly and monthly reporting
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.10
```

### Comparing `trytond_timesheet-6.6.0/COPYRIGHT` & `trytond_timesheet-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_timesheet-6.6.0/LICENSE` & `trytond_timesheet-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/PKG-INFO` & `trytond_timesheet-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with timesheets
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
-Project-URL: Source Code, https://hg.tryton.org/modules/timesheet
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton timesheet
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
 
 Timesheet Module
 ################
 
 The timesheet module allow to track the time spent by employees on
 various works. This module also comes with several reports that show
```

### Comparing `trytond_timesheet-6.6.0/README.rst` & `trytond_timesheet-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/__init__.py` & `trytond_timesheet-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/doc/index.rst` & `trytond_timesheet-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/doc/user_application.rst` & `trytond_timesheet-6.8.0/doc/user_application.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Timesheet User Application
 ##########################
 
 The timesheet module defines some routes for user applications:
 
-    - `GET` `/<database_name>/timesheet/employees`:
-      return the list of the user employees as dictionary with the keys: `id`
-      and `name`.
+    - ``GET`` ``/<database_name>/timesheet/employees``:
+      return the list of the user employees as dictionary with the keys: ``id``
+      and ``name``.
 
-    - `GET` `/<database_name>/timesheet/employee/<int:employee>/works`:
+    - ``GET`` ``/<database_name>/timesheet/employee/<int:employee>/works``:
       return the list of works available for the employee. The works are
-      dictionary with keys: `id`, `name`, `start` and `end`. The dates are in
-      the format `%Y-%m-%d`.
+      dictionary with keys: ``id``, ``name``, ``start`` and ``end``. The dates
+      are in the format ``%Y-%m-%d``.
 
-    - `GET` `/<database_name>/timesheet/employee/<int:employee>/lines/<date>`:
+    - ``GET`` ``/<database_name>/timesheet/employee/<int:employee>/lines/<date>``:
       return the list of timesheet lines for the employee at the date
-      (`%Y-%m-%d'). The lines are dictionary with keys: `id`, `work`,
-      `work.name`, `duration`, `description` and `uuid`. The duration is in
-      seconds.
+      (``%Y-%m-%d``). The lines are dictionary with keys: ``id``, ``work``,
+      ``work.name``, ``duration``, ``description`` and ``uuid``. The duration
+      is in seconds.
 
-    - `POST` `/<database_name>/timesheet/line`:
+    - ``POST`` ``/<database_name>/timesheet/line``:
       Create a line using the data as dictionary of value. The date must be in
-      the format `%Y-%m-%d` and the `duration` in seconds. If a `uuid` value is
-      provided, it will update the record if found instead of create a new one.
+      the format ``%Y-%m-%d`` and the ``duration`` in seconds. If a ``uuid``
+      value is provided, it will update the record if found instead of create a
+      new one.
 
-    - `PUT` `/<database_name>/timesheet/line/<int:line>`:
-      Update the line using the data like for the `POST`.
+    - ``PUT`` ``/<database_name>/timesheet/line/<int:line>``:
+      Update the line using the data like for the ``POST``.
 
-    - `DELETE` `/<database_name>/timesheet/line/<int:line>`:
+    - ``DELETE`` ``/<database_name>/timesheet/line/<int:line>``:
       Delete the line
```

### Comparing `trytond_timesheet-6.6.0/icons/LICENSE` & `trytond_timesheet-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/line.py` & `trytond_timesheet-6.8.0/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sql import Literal
 from sql.aggregate import Max, Sum
 from sql.functions import Extract
 
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, Unique, fields
 from trytond.pool import Pool
-from trytond.pyson import Date, Eval, PYSONEncoder
+from trytond.pyson import Date, Eval, PYSONEncoder, TimeDelta
 from trytond.transaction import Transaction
 from trytond.wizard import Button, StateAction, StateView, Wizard
 
 from .exceptions import DurationValidationError
 
 
 class Line(ModelSQL, ModelView):
@@ -34,15 +34,19 @@
                 ('end_date', '>=', Eval('date', None)),
                 ],
             ],
         help="The employee who spends the time.")
     date = fields.Date(
         "Date", required=True,
         help="When the time is spent.")
-    duration = fields.TimeDelta('Duration', 'company_work_time', required=True)
+    duration = fields.TimeDelta(
+        'Duration', 'company_work_time', required=True,
+        domain=[
+            ('duration', '>=', TimeDelta()),
+            ])
     work = fields.Many2One(
         'timesheet.work', "Work", required=True,
         domain=[
             ('company', '=', Eval('company', -1)),
             ['OR',
                 ('timesheet_start_date', '=', None),
                 ('timesheet_start_date', '<=', Eval('date', None)),
```

### Comparing `trytond_timesheet-6.6.0/locale/bg.po` & `trytond_timesheet-6.8.0/locale/sl.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,211 +1,198 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Продължителност"
+msgstr "Trajanje"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Служител"
+msgstr "Zaposlenec"
 
-#, fuzzy
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Крайна дата"
+msgstr "Konec"
 
-#, fuzzy
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Начална дата"
+msgstr "Začetek"
 
-#, fuzzy
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Продължителност"
+msgstr "Trajanje"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Служител"
+msgstr "Zaposlenec"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Месец"
+msgstr "Mesec"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "Година"
+msgstr "Leto"
 
-#, fuzzy
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Продължителност"
+msgstr "Trajanje"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Служител"
+msgstr "Zaposlenec"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Седмица"
+msgstr "Teden"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "Година"
+msgstr "Leto"
 
-#, fuzzy
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Družba"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Datum"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Описание"
+msgstr "Opis"
 
-#, fuzzy
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Продължителност"
+msgstr "Trajanje"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Служител"
+msgstr "Zaposlenec"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Задача"
+msgstr "Naloga"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "Дата"
+msgstr "Datum"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Служител"
+msgstr "Zaposlenec"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Фирма"
+msgstr "Družba"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr ""
+msgstr "Trajanje"
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Име"
+msgstr "Naziv"
 
-#, fuzzy
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Източник"
+msgstr "Poreklo"
 
-#, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Ред от график"
+msgstr "Konec evidence"
 
-#, fuzzy
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Редове от график"
+msgstr "Evidenca dela"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr ""
+msgstr "Začetek evidence"
 
-#, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Задача"
+msgstr "Naloga"
 
-#, fuzzy
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "От дата"
+msgstr "Od"
 
-#, fuzzy
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "До дата"
+msgstr "Do"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
-msgstr ""
+msgstr "Družba, za katero se evidentira čas."
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
-msgstr ""
+msgstr "Dan evidentiranja časa."
 
 msgctxt "help:timesheet.line,description:"
 msgid "Additional description of the work done."
-msgstr ""
+msgstr "Dodaten opis opravljene naloge."
 
 msgctxt "help:timesheet.line,employee:"
 msgid "The employee who spends the time."
-msgstr ""
+msgstr "Zaposlenec, katerega čas se evidentira."
 
 msgctxt "help:timesheet.line,work:"
 msgid "The work on which the time is spent."
-msgstr ""
+msgstr "Naloga, za katero se evidentira čas."
 
 msgctxt "help:timesheet.line.enter.start,date:"
 msgid "When the time is spent."
-msgstr ""
+msgstr "Dan evidentiranja časa."
 
 msgctxt "help:timesheet.line.enter.start,employee:"
 msgid "The employee who spends the time."
-msgstr ""
+msgstr "Zaposlenec, katerega čas se evidentira."
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
-msgstr ""
+msgstr "Poveži nalogo z družbo."
 
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr ""
+msgstr "Skupen čas, porabljen na nalogi."
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
-msgstr ""
+msgstr "Glavni identifikator naloge."
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
-msgstr ""
+msgstr "Povezuje porabljen čas z drugimi zapisi."
 
 msgctxt "help:timesheet.work,timesheet_end_date:"
 msgid "Restrict adding lines after the date."
-msgstr ""
+msgstr "Evidentiranje časa po tem datumu je onemogočeno."
 
 msgctxt "help:timesheet.work,timesheet_lines:"
 msgid "Spend time on this work."
-msgstr ""
+msgstr "Evidentiranje časa, porabljenega na nalogi."
 
 msgctxt "help:timesheet.work,timesheet_start_date:"
 msgid "Restrict adding lines before the date."
-msgstr ""
+msgstr "Evidentiranje časa pred tem datumom je onemogočeno."
 
 msgctxt "help:timesheet.work.context,from_date:"
 msgid "Do not take into account lines before the date."
-msgstr ""
+msgstr "Evidenca časa pred tem datumom se ne upošteva."
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
-msgstr ""
+msgstr "Evidenca časa po tem datumu se ne upošteva."
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
 #, fuzzy
@@ -219,63 +206,96 @@
 msgstr "Hours per Employee per Week"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr ""
+msgstr "Vnos postavk"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
-msgstr "Редове от график"
+msgstr "Timesheet Lines"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Зачади"
+msgstr "Works"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr ""
+msgstr "Trajanje na postavki \"%(line)s\" mora biti nenegativno."
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr ""
+msgstr "Poreklo mora biti unikatno po družbi."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -294,15 +314,15 @@
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Configuration"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "Часове на служител"
+msgstr "Hours per Employee"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
 #, fuzzy
@@ -311,17 +331,18 @@
 msgstr "Hours per Employee per Week"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr ""
+msgstr "Vnos postavk"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
 #, fuzzy
@@ -333,68 +354,65 @@
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Зачади"
+msgstr "Works"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Часове на служител"
+msgstr "Ure po zaposlencu"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
-msgstr ""
+msgstr "Ure po kontekstu zaposlenca"
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Часове за служител за месец"
+msgstr "Mesečne ure po zaposlencu"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Часове на служител за седмица"
+msgstr "Tedenske ure po zaposlencu"
 
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Ред от график"
+msgstr "Evidenca dela"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr ""
+msgstr "Vnos postavk"
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Задача"
+msgstr "Naloga"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr ""
+msgstr "Kontekst naloge"
 
-#, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "Управление на графици"
+msgstr "Evidenca dela"
 
-#, fuzzy
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Продължителност"
+msgstr "Trajanje"
 
-#, fuzzy
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Продължителност"
+msgstr "Trajanje"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "Отказ"
+msgstr "Prekliči"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "Въвеждане"
+msgstr "Vnos"
```

### Comparing `trytond_timesheet-6.6.0/locale/ca.po` & `trytond_timesheet-6.8.0/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -248,17 +248,47 @@
 msgid "Work origin must be unique by company."
 msgstr "L'origen ha de ser únic per empresa."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "Qualsevol hora d'empleat"
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Hores pròpies"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "Hores de qualsevol empleat"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Hores pròpies"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "Hores de qualsevol empleat"
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
-msgstr "Hores del propi empleat"
+msgid "Own hours"
+msgstr "Hores pròpies"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Hores dels empleats supervisats"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Hores dels empleats supervisats"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Hores dels empleats supervisats"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Línies del full de treball pròpies"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
```

### Comparing `trytond_timesheet-6.6.0/locale/cs.po` & `trytond_timesheet-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Pabaigos data"
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Pradžios data"
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
@@ -48,15 +48,15 @@
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
 msgstr ""
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
@@ -85,15 +85,15 @@
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:timesheet.work,name:"
@@ -251,16 +251,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -273,15 +303,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Nuostatos"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
@@ -297,15 +327,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Ataskaitos"
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_timesheet-6.6.0/locale/de.po` & `trytond_timesheet-6.8.0/locale/de.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
@@ -16,15 +16,15 @@
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
 msgstr "Startdatum"
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
@@ -32,15 +32,15 @@
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
 msgstr "Jahr"
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
@@ -60,27 +60,27 @@
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
 msgstr "Beschreibung"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
 msgstr "Mitarbeiter"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr "UUID"
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Tätigkeit"
+msgstr "Aufgabe"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
 msgstr "Datum"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
@@ -88,15 +88,15 @@
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr "Zeiterfassung Dauer"
+msgstr "Erfasste Gesamtzeit"
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
@@ -112,15 +112,15 @@
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
 msgstr "Zeiterfassung Beginn"
 
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Tätigkeit"
+msgstr "Aufgabe"
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
 msgstr "Von Datum"
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
@@ -172,15 +172,15 @@
 
 msgctxt "help:timesheet.work,timesheet_end_date:"
 msgid "Restrict adding lines after the date."
 msgstr "Hinzufügen von Positionen nach dem Datum beschränken."
 
 msgctxt "help:timesheet.work,timesheet_lines:"
 msgid "Spend time on this work."
-msgstr "Zeit für diese Aufgabe aufwenden."
+msgstr "Aufgewendete Zeiten für die Aufgabe."
 
 msgctxt "help:timesheet.work,timesheet_start_date:"
 msgid "Restrict adding lines before the date."
 msgstr "Hinzufügen von Positionen vor dem Datum beschränken."
 
 msgctxt "help:timesheet.work.context,from_date:"
 msgid "Do not take into account lines before the date."
@@ -212,54 +212,85 @@
 
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Zeiterfassungspositionen"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "Tätigkeiten"
+msgstr "Aufgaben"
 
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Tätigkeiten"
+msgstr "Aufgaben"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr "Alle"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr "Offen"
 
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr "Die Zeitdauer von Zeile \"%(line)s\" muss positiv sein."
+msgstr ""
+"Die erfasste Zeit der Zeiterfassungsposition \"%(line)s\" muss positiv sein."
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr "Die UUID der Zeiterfassungsposition muss eindeutig sein."
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
-"Die mit der Tätigkeit \"%(work)s\" und Ihrer Herkunft verknüpften "
-"Unternehmen weichen voneinander ab."
+"Die mit der Aufgabe \"%(work)s\" und Ihrer Herkunft verknüpften Unternehmen "
+"weichen voneinander ab."
 
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
 msgstr ""
 "Die Herkunft der Arbeit pro Unternehmen kann nur einmal vergeben werden."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "Alle Mitarbeiterzeiten"
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Eigene Monatliche Zeiten"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "Alle Monatlichen Mitarbeiterzeiten"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Eigene Wöchentliche Zeiten"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "Alle Wöchentlichen Mitarbeiterzeiten"
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
-msgstr "Zeiterfassungspositionen Auswertung (Nur Eigene)"
+msgid "Own hours"
+msgstr "Eigene Zeiten"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Alle Zeiten betreuter Mitarbeiter"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Alle monatlichen Zeiten betreuter Mitarbeiter"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Alle wöchentlichen Zeiten betreuter Mitarbeiter"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Eigene Zeiterfassungspositionen"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
@@ -303,19 +334,19 @@
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Zeiterfassung"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr "Tätigkeiten"
+msgstr "Aufgaben"
 
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Tätigkeiten"
+msgstr "Aufgaben"
 
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Zeiterfassung Administration"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
@@ -339,31 +370,31 @@
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
 msgstr "Eingabe Zeilen"
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Tätigkeit"
+msgstr "Aufgabe"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr "Tätigkeit Kontext"
+msgstr "Aufgabe Kontext"
 
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
 msgstr "Zeiterfassung"
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
 msgstr "Abbrechen"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
```

### Comparing `trytond_timesheet-6.6.0/locale/es.po` & `trytond_timesheet-6.8.0/locale/es.po`

 * *Files 3% similar despite different names*

```diff
@@ -247,17 +247,47 @@
 msgid "Work origin must be unique by company."
 msgstr "El origen debe ser único por empresa."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "Cualquier hora de empleado"
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Horas propias"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "Horas de cualquier empleado"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Horas propias"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "Horas de cualquier empleado"
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
-msgstr "Horas del propio empleado"
+msgid "Own hours"
+msgstr "Horas propias"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Horas de los empleados supervisados"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Horas de los empleados supervisados"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Horas de los empleados supervisados"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Lineas del parte de trabajo propias"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
```

### Comparing `trytond_timesheet-6.6.0/locale/es_419.po` & `trytond_timesheet-6.8.0/locale/es_419.po`

 * *Files 3% similar despite different names*

```diff
@@ -250,16 +250,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
```

### Comparing `trytond_timesheet-6.6.0/locale/et.po` & `trytond_timesheet-6.8.0/locale/et.po`

 * *Files 4% similar despite different names*

```diff
@@ -248,18 +248,55 @@
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "Kõigi töötajate tunnid"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Oma töötaja tunnid"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "Kõigi töötajate tunnid"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Oma töötaja tunnid"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "Kõigi töötajate tunnid"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
 msgstr "Oma töötaja tunnid"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Kõigi töötajate tunnid"
+
+#, fuzzy
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Kõigi töötajate tunnid"
+
+#, fuzzy
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Kõigi töötajate tunnid"
+
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Oma tööajatabeli rida"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
 msgstr "Kõik tööaja tabeli read"
```

### Comparing `trytond_timesheet-6.6.0/locale/fa.po` & `trytond_timesheet-6.8.0/locale/fa.po`

 * *Files 6% similar despite different names*

```diff
@@ -247,16 +247,46 @@
 msgid "Work origin must be unique by company."
 msgstr "منشا باید در هر شرکتی منحصر به فرد باشد."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
```

### Comparing `trytond_timesheet-6.6.0/locale/fi.po` & `trytond_timesheet-6.8.0/locale/ro.po`

 * *Files 3% similar despite different names*

```diff
@@ -48,83 +48,79 @@
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
 msgstr ""
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr ""
+msgstr "Descriere"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Works"
+msgstr ""
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr ""
+msgstr "Data"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Angajat"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
 msgstr ""
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
-#, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Timesheet Lines"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Timesheet Lines"
+msgstr ""
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Works"
+msgstr ""
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
@@ -192,43 +188,43 @@
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
-msgstr "Hours per Employee"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_hours_employee_monthly_form"
 msgid "Hours per Employee per Month"
-msgstr "Hours per Employee per Month"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
-msgstr "Hours per Employee per Week"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
-msgstr "Enter Timesheet"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
-msgstr "Timesheet Lines"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "Works"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Works"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
@@ -250,16 +246,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -272,97 +298,91 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Configurare"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "Hours per Employee"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
-msgstr "Hours per Employee per Month"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
-msgstr "Hours per Employee per Week"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
-msgstr "Enter Timesheet"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Raportare"
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
-msgstr "Timesheet"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr "Works"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Works"
+msgstr ""
 
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
-msgstr "Timesheet Administration"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Hours per Employee"
+msgstr ""
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Hours per Employee per Month"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Hours per Employee per Week"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Timesheet Lines"
+msgstr ""
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Works"
+msgstr ""
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "Timesheet"
+msgstr ""
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
```

### Comparing `trytond_timesheet-6.6.0/locale/fr.po` & `trytond_timesheet-6.8.0/locale/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -247,17 +247,47 @@
 msgid "Work origin must be unique by company."
 msgstr "L'origine doit être unique par société."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "N'importe quelles heures d'employés"
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Heures propres"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "N'importe quelles heures d'employés"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Heures propres"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "N'importe quelles heures d'employés"
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
-msgstr "Heures d'employé propre"
+msgid "Own hours"
+msgstr "Heures propres"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Heures d'employés supervisés"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Heures d'employés supervisés"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Heures d'employés supervisés"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Ligne de feuille de présence propre"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
```

### Comparing `trytond_timesheet-6.6.0/locale/hu.po` & `trytond_timesheet-6.8.0/locale/it.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,137 +1,134 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Időtartam"
+msgstr "Durata"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Alkalmazott"
+msgstr "Dipendente"
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr ""
+msgstr "Data finale"
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Data iniziale"
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Időtartam"
+msgstr "Durata"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Alkalmazott"
+msgstr "Dipendente"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Hónap"
+msgstr "Mese"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "Év"
+msgstr "Anno"
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Időtartam"
+msgstr "Durata"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Alkalmazott"
+msgstr "Dipendente"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Hét"
+msgstr "Settimana"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "Év"
+msgstr "Anno"
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Társaság"
+msgstr "Azienda"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Data"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Leírás"
+msgstr "Descrizione"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Időtartam"
+msgstr "Durata"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Alkalmazott"
+msgstr "Dipendente"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Tevékenység"
+msgstr "Lavoro"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "Dátum"
+msgstr "Data"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Alkalmazott"
+msgstr "Dipendente"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Társaság"
+msgstr "Azienda"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr "Időtartam"
+msgstr "Durata timesheet"
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Név"
+msgstr "Nome"
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Időkövetés vége"
+msgstr "Fine timesheet"
 
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Időpozíció"
+msgstr "Righe timesheet"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr "Időkövetés kezdete"
+msgstr "inizio timesheet"
 
-#, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Tevékenység"
+msgstr "Lavoro"
 
-#, fuzzy
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "Dátumtól"
+msgstr "Data Iniziale"
 
-#, fuzzy
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "Dátumig"
+msgstr "a data"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
 msgstr ""
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
@@ -160,15 +157,15 @@
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
 msgstr ""
 
 #, fuzzy
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr "Az össz idő, ami erre a feladatra lett fordítva"
+msgstr "Tempo totale speso nel lavoro"
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
 msgstr ""
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
@@ -213,62 +210,93 @@
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr "Sor hozzáadás"
+msgstr "Inserire righe"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Timesheet Lines"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Tevékenység"
+msgstr "Works"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr "A \"%(line)s\" sor időtartama pozitívnak kell lenni."
+msgstr "La durata della riga \"%(line)s\" dev'essere positiva."
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr ""
+msgstr "L'origine dev'essere unica per azienda."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -279,23 +307,22 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Configurazione"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "Óra per alkalmazott"
+msgstr "Hours per Employee"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
 #, fuzzy
@@ -307,86 +334,84 @@
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr "Sor hozzáadás"
+msgstr "Inserire righe"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Tevékenység"
+msgstr "Works"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Óra per alkalmazott"
+msgstr "Ore per dipendente"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
-msgstr ""
+msgstr "Context ore per dipendente"
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Óra per alkalmazott per hónap"
+msgstr "Ore per dipendente per mese"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Óra per alkalmazott per hét"
+msgstr "Ore per dipendente per settimana"
 
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Időpozíció"
+msgstr "Riga timesheet"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr "Sor hozzáadás"
+msgstr "Inserire righe"
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Tevékenység"
+msgstr "Lavoro"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr ""
+msgstr "Context lavoro"
 
-#, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "Időtartam"
+msgstr "Timesheet"
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Időtartam"
+msgstr "Durata"
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Időtartam"
+msgstr "Durata"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "Mégse"
+msgstr "Annulla"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "Bevitel"
+msgstr "Invio"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_timesheet-6.6.0/locale/id.po` & `trytond_timesheet-6.8.0/locale/id.po`

 * *Files 2% similar despite different names*

```diff
@@ -246,16 +246,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
```

### Comparing `trytond_timesheet-6.6.0/locale/it.po` & `trytond_timesheet-6.8.0/locale/pl.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,134 +1,136 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "Czas trwania"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Pracownik"
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Data finale"
+msgstr "Data ukończenia"
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Data iniziale"
+msgstr "Data rozpoczęcia"
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "Czas trwania"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Pracownik"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Mese"
+msgstr "Miesiąc"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "Anno"
+msgstr "Rok"
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "Czas trwania"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Pracownik"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Settimana"
+msgstr "Tydzień"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "Anno"
+msgstr "Rok"
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Firma"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Opis"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "Czas trwania"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Pracownik"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Lavoro"
+msgstr "Praca"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Dipendente"
+msgstr "Pracownik"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Firma"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr "Durata timesheet"
+msgstr ""
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Nome"
+msgstr "Nazwa"
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr "Źródło"
 
+#, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Fine timesheet"
+msgstr "Timesheet Lines"
 
+#, fuzzy
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Righe timesheet"
+msgstr "Timesheet Lines"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr "inizio timesheet"
+msgstr ""
 
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Lavoro"
+msgstr "Praca"
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "Data Iniziale"
+msgstr "Od dnia"
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "a data"
+msgstr "Do dnia"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
 msgstr ""
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
@@ -154,18 +156,17 @@
 msgid "The employee who spends the time."
 msgstr ""
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr "Tempo totale speso nel lavoro"
+msgstr "Całkowity czas pracy"
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
 msgstr ""
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
@@ -202,23 +203,21 @@
 msgstr "Hours per Employee per Month"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
 msgstr "Hours per Employee per Week"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr "Inserire righe"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Timesheet Lines"
 
 #, fuzzy
@@ -235,38 +234,66 @@
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr "La durata della riga \"%(line)s\" dev'essere positiva."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr "L'origine dev'essere unica per azienda."
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -279,15 +306,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurazione"
+msgstr "Konfiguracja"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
 #, fuzzy
@@ -296,92 +323,91 @@
 msgstr "Hours per Employee per Month"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
 msgstr "Hours per Employee per Week"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr "Inserire righe"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
 msgstr "Works"
 
-#, fuzzy
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Ore per dipendente"
+msgstr "Godziny wg pracownika"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
-msgstr "Context ore per dipendente"
+msgstr ""
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Ore per dipendente per mese"
+msgstr "Godziny wg pracownika na miesiąc"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Ore per dipendente per settimana"
+msgstr "Godziny wg pracownika na tydzień"
 
+#, fuzzy
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Riga timesheet"
+msgstr "Timesheet Lines"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr "Inserire righe"
+msgstr ""
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Lavoro"
+msgstr "Praca"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr "Context lavoro"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "Czas trwania"
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "Czas trwania"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Anuluj"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "Invio"
+msgstr "Wprowadź"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_timesheet-6.6.0/locale/lo.po` & `trytond_timesheet-6.8.0/locale/lo.po`

 * *Files 6% similar despite different names*

```diff
@@ -257,16 +257,46 @@
 msgid "Work origin must be unique by company."
 msgstr "ສຳນັກງານເດີມຕ້ອງບໍ່ຊໍ້າກັນ."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
```

### Comparing `trytond_timesheet-6.6.0/locale/lt.po` & `trytond_timesheet-6.8.0/locale/cs.po`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Pabaigos data"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Pradžios data"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
@@ -48,15 +48,15 @@
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
 msgstr ""
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
 msgstr ""
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
@@ -85,15 +85,15 @@
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:timesheet.work,name:"
@@ -251,16 +251,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -273,15 +303,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Nuostatos"
+msgstr "Configuration"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
@@ -297,15 +327,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Ataskaitos"
+msgstr "Reporting"
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_timesheet-6.6.0/locale/nl.po` & `trytond_timesheet-6.8.0/locale/nl.po`

 * *Files 4% similar despite different names*

```diff
@@ -248,17 +248,47 @@
 msgid "Work origin must be unique by company."
 msgstr "De oorsprong van het werk moet uniek zijn per bedrijf."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "Elke medewerkers uren"
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Eigen uren"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "Uren alle medewerkers"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Eigen uren"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "Uren alle medewerkers"
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
-msgstr "Eigen medewerkersuren"
+msgid "Own hours"
+msgstr "Eigen uren"
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Uren medewerkers leidinggevende"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Uren medewerkers leidinggevende"
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Uren medewerkers leidinggevende"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Eigen urenstaatregel"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
```

### Comparing `trytond_timesheet-6.6.0/locale/pl.po` & `trytond_timesheet-6.8.0/locale/fi.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Czas trwania"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Data ukończenia"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Data rozpoczęcia"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Czas trwania"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Miesiąc"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "Rok"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Czas trwania"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Tydzień"
+msgstr ""
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "Rok"
+msgstr ""
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr ""
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr ""
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Czas trwania"
+msgstr ""
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr ""
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Praca"
+msgstr "Works"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Pracownik"
+msgstr ""
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr ""
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
 msgstr ""
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Nazwa"
+msgstr ""
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Źródło"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
 msgstr "Timesheet Lines"
 
 #, fuzzy
@@ -112,25 +113,26 @@
 msgid "Timesheet Lines"
 msgstr "Timesheet Lines"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Praca"
+msgstr "Works"
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "Od dnia"
+msgstr ""
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "Do dnia"
+msgstr ""
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
 msgstr ""
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
@@ -158,15 +160,15 @@
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
 msgstr ""
 
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr "Całkowity czas pracy"
+msgstr ""
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
 msgstr ""
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
@@ -188,48 +190,42 @@
 msgid "Do not take into account lines before the date."
 msgstr ""
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_monthly_form"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
 msgstr "Hours per Employee per Week"
 
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Timesheet Lines"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
 msgstr "Works"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
 msgstr "Works"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
@@ -254,16 +250,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -276,27 +302,24 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Konfiguracja"
+msgstr "Configuration"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
 msgstr "Hours per Employee per Week"
 
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
@@ -305,79 +328,80 @@
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
 msgstr "Works"
 
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
+#, fuzzy
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Godziny wg pracownika"
+msgstr "Hours per Employee"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Godziny wg pracownika na miesiąc"
+msgstr "Hours per Employee per Month"
 
+#, fuzzy
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Godziny wg pracownika na tydzień"
+msgstr "Hours per Employee per Week"
 
 #, fuzzy
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
 msgstr "Timesheet Lines"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Praca"
+msgstr "Works"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
 msgstr "Timesheet"
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Czas trwania"
+msgstr ""
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Czas trwania"
+msgstr ""
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "Anuluj"
+msgstr ""
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "Wprowadź"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_timesheet-6.6.0/locale/pt.po` & `trytond_timesheet-6.8.0/locale/pt.po`

 * *Files 3% similar despite different names*

```diff
@@ -254,16 +254,46 @@
 msgid "Work origin must be unique by company."
 msgstr "A origem deve ser única por empresa."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
```

### Comparing `trytond_timesheet-6.6.0/locale/ro.po` & `trytond_timesheet-6.8.0/locale/tr.po`

 * *Files 16% similar despite different names*

```diff
@@ -48,79 +48,83 @@
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
 msgstr ""
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
 msgstr ""
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr ""
+msgstr "Works"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr ""
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
 msgstr ""
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr ""
+msgstr "Timesheet Lines"
 
+#, fuzzy
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr ""
+msgstr "Timesheet Lines"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr ""
+msgstr "Works"
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
@@ -188,74 +192,106 @@
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
-msgstr ""
+msgstr "Hours per Employee"
 
 msgctxt "model:ir.action,name:act_hours_employee_monthly_form"
 msgid "Hours per Employee per Month"
-msgstr ""
+msgstr "Hours per Employee per Month"
 
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
-msgstr ""
+msgstr "Hours per Employee per Week"
 
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
-msgstr ""
+msgstr "Enter Timesheet"
 
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
-msgstr ""
+msgstr "Timesheet Lines"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr ""
+msgstr "Works"
 
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr ""
+msgstr "Works"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr ""
+msgstr "İş \"%(line)s\" süresi pozitif olmalı"
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr ""
+msgstr "Kök her firma için özgün olmalı."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -268,91 +304,97 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Configuration"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr ""
+msgstr "Hours per Employee"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
-msgstr ""
+msgstr "Hours per Employee per Month"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
-msgstr ""
+msgstr "Hours per Employee per Week"
 
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
-msgstr ""
+msgstr "Enter Timesheet"
 
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Raportare"
+msgstr "Reporting"
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
-msgstr ""
+msgstr "Timesheet"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr ""
+msgstr "Works"
 
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr ""
+msgstr "Works"
 
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
-msgstr ""
+msgstr "Timesheet Administration"
 
+#, fuzzy
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr ""
+msgstr "Hours per Employee"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr ""
+msgstr "Hours per Employee per Month"
 
+#, fuzzy
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr ""
+msgstr "Hours per Employee per Week"
 
+#, fuzzy
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr ""
+msgstr "Timesheet Lines"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr ""
+msgstr "Works"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr ""
+msgstr "Timesheet"
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
 msgstr ""
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_timesheet-6.6.0/locale/ru.po` & `trytond_timesheet-6.8.0/locale/bg.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,145 +1,147 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 #, fuzzy
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Продолжительность"
+msgstr "Продължителност"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Служител"
 
 #, fuzzy
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Дата окончания"
+msgstr "Крайна дата"
 
 #, fuzzy
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Дата начала"
+msgstr "Начална дата"
 
 #, fuzzy
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Продолжительность"
+msgstr "Продължителност"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Служител"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Месяц"
+msgstr "Месец"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "Год"
+msgstr "Година"
 
 #, fuzzy
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Продолжительность"
+msgstr "Продължителност"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Служител"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Неделя"
+msgstr "Седмица"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "Год"
+msgstr "Година"
 
 #, fuzzy
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Фирма"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
 msgstr "Дата"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
 msgstr "Описание"
 
 #, fuzzy
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Продолжительность"
+msgstr "Продължителност"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Служител"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Работа"
+msgstr "Задача"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
 msgstr "Дата"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Сотрудник"
+msgstr "Служител"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Организация"
+msgstr "Фирма"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
 msgstr ""
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Наименование"
+msgstr "Име"
 
 #, fuzzy
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Первоисточник"
+msgstr "Източник"
 
+#, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Конечная дата табеля"
+msgstr "Ред от график"
 
+#, fuzzy
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Строки табеля"
+msgstr "Редове от график"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr "Начальная дата табеля"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Работа"
+msgstr "Задача"
 
 #, fuzzy
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "Начальная дата"
+msgstr "От дата"
 
 #, fuzzy
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "Конечная дата"
+msgstr "До дата"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
 msgstr ""
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
@@ -217,33 +219,32 @@
 msgstr "Hours per Employee per Week"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr "Ввод строк"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
-msgstr "Timesheet Lines"
+msgstr "Редове от график"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Работы"
+msgstr "Зачади"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
@@ -265,16 +266,46 @@
 msgid "Work origin must be unique by company."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -293,15 +324,15 @@
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Configuration"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "Часы на сотрудника"
+msgstr "Часове на служител"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
 #, fuzzy
@@ -310,18 +341,17 @@
 msgstr "Hours per Employee per Week"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr "Ввод строк"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
 #, fuzzy
@@ -333,68 +363,68 @@
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Работы"
+msgstr "Зачади"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Часы на сотрудника"
+msgstr "Часове на служител"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
 msgstr ""
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Часы на сотрудника в месяц"
+msgstr "Часове за служител за месец"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Часы на сотрудника в неделю"
+msgstr "Часове на служител за седмица"
 
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Строка табеля"
+msgstr "Ред от график"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr "Ввод строк"
+msgstr ""
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Работа"
+msgstr "Задача"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "Табель"
+msgstr "Управление на графици"
 
 #, fuzzy
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Продолжительность"
+msgstr "Продължителност"
 
 #, fuzzy
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Продолжительность"
+msgstr "Продължителност"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Отказ"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "Ввод"
+msgstr "Въвеждане"
```

### Comparing `trytond_timesheet-6.6.0/locale/sl.po` & `trytond_timesheet-6.8.0/locale/ru.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,198 +1,209 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Trajanje"
+msgstr "Продолжительность"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Сотрудник"
 
+#, fuzzy
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Konec"
+msgstr "Дата окончания"
 
+#, fuzzy
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Začetek"
+msgstr "Дата начала"
 
+#, fuzzy
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Trajanje"
+msgstr "Продолжительность"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Сотрудник"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Mesec"
+msgstr "Месяц"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "Leto"
+msgstr "Год"
 
+#, fuzzy
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Trajanje"
+msgstr "Продолжительность"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Сотрудник"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Teden"
+msgstr "Неделя"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "Leto"
+msgstr "Год"
 
+#, fuzzy
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Учет.орг."
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr "Дата"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "Описание"
 
+#, fuzzy
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Trajanje"
+msgstr "Продолжительность"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Сотрудник"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Naloga"
+msgstr "Работа"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "Datum"
+msgstr "Дата"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Zaposlenec"
+msgstr "Сотрудник"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Организация"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr "Trajanje"
+msgstr ""
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Naziv"
+msgstr "Наименование"
 
+#, fuzzy
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Poreklo"
+msgstr "Первоисточник"
 
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Konec evidence"
+msgstr "Конечная дата табеля"
 
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Evidenca dela"
+msgstr "Строки табеля"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr "Začetek evidence"
+msgstr "Начальная дата табеля"
 
+#, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Naloga"
+msgstr "Работа"
 
+#, fuzzy
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "Od"
+msgstr "Начальная дата"
 
+#, fuzzy
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "Do"
+msgstr "Конечная дата"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
-msgstr "Družba, za katero se evidentira čas."
+msgstr ""
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
-msgstr "Dan evidentiranja časa."
+msgstr ""
 
 msgctxt "help:timesheet.line,description:"
 msgid "Additional description of the work done."
-msgstr "Dodaten opis opravljene naloge."
+msgstr ""
 
 msgctxt "help:timesheet.line,employee:"
 msgid "The employee who spends the time."
-msgstr "Zaposlenec, katerega čas se evidentira."
+msgstr ""
 
 msgctxt "help:timesheet.line,work:"
 msgid "The work on which the time is spent."
-msgstr "Naloga, za katero se evidentira čas."
+msgstr ""
 
 msgctxt "help:timesheet.line.enter.start,date:"
 msgid "When the time is spent."
-msgstr "Dan evidentiranja časa."
+msgstr ""
 
 msgctxt "help:timesheet.line.enter.start,employee:"
 msgid "The employee who spends the time."
-msgstr "Zaposlenec, katerega čas se evidentira."
+msgstr ""
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
-msgstr "Poveži nalogo z družbo."
+msgstr ""
 
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr "Skupen čas, porabljen na nalogi."
+msgstr ""
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
-msgstr "Glavni identifikator naloge."
+msgstr ""
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
-msgstr "Povezuje porabljen čas z drugimi zapisi."
+msgstr ""
 
 msgctxt "help:timesheet.work,timesheet_end_date:"
 msgid "Restrict adding lines after the date."
-msgstr "Evidentiranje časa po tem datumu je onemogočeno."
+msgstr ""
 
 msgctxt "help:timesheet.work,timesheet_lines:"
 msgid "Spend time on this work."
-msgstr "Evidentiranje časa, porabljenega na nalogi."
+msgstr ""
 
 msgctxt "help:timesheet.work,timesheet_start_date:"
 msgid "Restrict adding lines before the date."
-msgstr "Evidentiranje časa pred tem datumom je onemogočeno."
+msgstr ""
 
 msgctxt "help:timesheet.work.context,from_date:"
 msgid "Do not take into account lines before the date."
-msgstr "Evidenca časa pred tem datumom se ne upošteva."
+msgstr ""
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
-msgstr "Evidenca časa po tem datumu se ne upošteva."
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
 #, fuzzy
@@ -209,63 +220,91 @@
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr "Vnos postavk"
+msgstr "Ввод строк"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Timesheet Lines"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Works"
+msgstr "Работы"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr "Trajanje na postavki \"%(line)s\" mora biti nenegativno."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr "Poreklo mora biti unikatno po družbi."
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -284,15 +323,15 @@
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Configuration"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "Hours per Employee"
+msgstr "Часы на сотрудника"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
 #, fuzzy
@@ -304,15 +343,15 @@
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr "Vnos postavk"
+msgstr "Ввод строк"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
 #, fuzzy
@@ -324,65 +363,68 @@
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Works"
+msgstr "Работы"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Ure po zaposlencu"
+msgstr "Часы на сотрудника"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
-msgstr "Ure po kontekstu zaposlenca"
+msgstr ""
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Mesečne ure po zaposlencu"
+msgstr "Часы на сотрудника в месяц"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Tedenske ure po zaposlencu"
+msgstr "Часы на сотрудника в неделю"
 
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Evidenca dela"
+msgstr "Строка табеля"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr "Vnos postavk"
+msgstr "Ввод строк"
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Naloga"
+msgstr "Работа"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr "Kontekst naloge"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "Evidenca dela"
+msgstr "Табель"
 
+#, fuzzy
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr "Trajanje"
+msgstr "Продолжительность"
 
+#, fuzzy
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr "Trajanje"
+msgstr "Продолжительность"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Отменить"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "Vnos"
+msgstr "Ввод"
```

### Comparing `trytond_timesheet-6.6.0/locale/tr.po` & `trytond_timesheet-6.8.0/locale/hu.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,137 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Alkalmazott"
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
 msgstr ""
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Alkalmazott"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr ""
+msgstr "Hónap"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr ""
+msgstr "Év"
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Alkalmazott"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr ""
+msgstr "Hét"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr ""
+msgstr "Év"
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr ""
+msgstr "Társaság"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr ""
+msgstr "Dátum"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr ""
+msgstr "Leírás"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Alkalmazott"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Works"
+msgstr "Tevékenység"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr ""
+msgstr "Dátum"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr ""
+msgstr "Alkalmazott"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr ""
+msgstr "Társaság"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr ""
+msgstr "Név"
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Timesheet Lines"
+msgstr "Időkövetés vége"
 
-#, fuzzy
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Timesheet Lines"
+msgstr "Időpozíció"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr ""
+msgstr "Időkövetés kezdete"
 
 #, fuzzy
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Works"
+msgstr "Tevékenység"
 
+#, fuzzy
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr ""
+msgstr "Dátumtól"
 
+#, fuzzy
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr ""
+msgstr "Dátumig"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
 msgstr ""
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
@@ -158,17 +157,18 @@
 msgid "The employee who spends the time."
 msgstr ""
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr ""
+msgstr "Az össz idő, ami erre a feladatra lett fordítva"
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
 msgstr ""
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
@@ -190,78 +190,115 @@
 msgid "Do not take into account lines before the date."
 msgstr ""
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
 msgstr "Hours per Employee"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_monthly_form"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
 msgstr "Hours per Employee per Week"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr ""
+msgstr "Sor hozzáadás"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Timesheet Lines"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
 msgstr "Works"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Works"
+msgstr "Tevékenység"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr "İş \"%(line)s\" süresi pozitif olmalı"
+msgstr "A \"%(line)s\" sor időtartama pozitívnak kell lenni."
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr "Kök her firma için özgün olmalı."
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr ""
 
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr ""
+
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
+msgstr ""
+
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr ""
+
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
@@ -272,108 +309,114 @@
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Configuration"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "Hours per Employee"
+msgstr "Óra per alkalmazott"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
 msgstr "Hours per Employee per Month"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
 msgstr "Hours per Employee per Week"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
 msgstr "Enter Timesheet"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr ""
+msgstr "Sor hozzáadás"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Reporting"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
 msgstr "Timesheet"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
 msgstr "Works"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "Works"
+msgstr "Tevékenység"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
 msgstr "Timesheet Administration"
 
-#, fuzzy
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "Hours per Employee"
+msgstr "Óra per alkalmazott"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "Hours per Employee per Month"
+msgstr "Óra per alkalmazott per hónap"
 
-#, fuzzy
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "Hours per Employee per Week"
+msgstr "Óra per alkalmazott per hét"
 
-#, fuzzy
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "Timesheet Lines"
+msgstr "Időpozíció"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr ""
+msgstr "Sor hozzáadás"
 
-#, fuzzy
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "Works"
+msgstr "Tevékenység"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "Timesheet"
+msgstr "Időtartam"
 
 msgctxt "view:timesheet.hours_employee:"
 msgid "Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "view:timesheet.line:"
 msgid "Duration"
-msgstr ""
+msgstr "Időtartam"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Mégse"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr ""
+msgstr "Bevitel"
```

### Comparing `trytond_timesheet-6.6.0/locale/uk.po` & `trytond_timesheet-6.8.0/locale/uk.po`

 * *Files 11% similar despite different names*

```diff
@@ -247,18 +247,56 @@
 msgid "Work origin must be unique by company."
 msgstr "Походження роботи має бути унікальним для компанії."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "Будь-які години працівника"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "Власні години працівника"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "Будь-які години працівника"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "Власні години працівника"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "Будь-які години працівника"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
 msgstr "Власні години працівника"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "Будь-які години працівника"
+
+#, fuzzy
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "Будь-які години працівника"
+
+#, fuzzy
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "Будь-які години працівника"
+
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "Власний рядок табеля"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
 msgstr "Будь-який рядок табеля"
```

### Comparing `trytond_timesheet-6.6.0/locale/zh_CN.po` & `trytond_timesheet-6.8.0/locale/zh_CN.po`

 * *Files 8% similar despite different names*

```diff
@@ -248,18 +248,55 @@
 msgstr "工作来源必须按公司唯一."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
 msgstr "任意雇员工时"
 
 #, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
+msgid "Own hours"
+msgstr "自有雇员工时"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
+msgid "Any employee hours"
+msgstr "任意雇员工时"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
+msgid "Own hours"
+msgstr "自有雇员工时"
+
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
+msgid "Any employee hours"
+msgstr "任意雇员工时"
+
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
-msgid "Own employee hours"
+msgid "Own hours"
 msgstr "自有雇员工时"
 
+#, fuzzy
+msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
+msgid "Supervised employee's hours"
+msgstr "任意雇员工时"
+
+#, fuzzy
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
+msgid "Supervised employee's hours"
+msgstr "任意雇员工时"
+
+#, fuzzy
+msgctxt ""
+"model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
+msgid "Supervised employee's hours"
+msgstr "任意雇员工时"
+
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
 msgstr "自有雇员时间表明细"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
 msgstr "任意雇员工时间表明细"
```

### Comparing `trytond_timesheet-6.6.0/message.xml` & `trytond_timesheet-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/routes.py` & `trytond_timesheet-6.8.0/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 
-from werkzeug.exceptions import abort
-from werkzeug.wrappers import Response
-
 from trytond.protocols.wrappers import (
-    allow_null_origin, user_application, with_pool, with_transaction)
+    Response, abort, allow_null_origin, user_application, with_pool,
+    with_transaction)
 from trytond.transaction import Transaction
 from trytond.wsgi import app
 
 timesheet_application = user_application('timesheet')
 
 
 @app.route('/<database_name>/timesheet/employees', methods=['GET'])
```

### Comparing `trytond_timesheet-6.6.0/setup.py` & `trytond_timesheet-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
@@ -37,59 +34,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_timesheet'
 
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
 
-requires = ['python-sql', 'werkzeug']
+requires = ['python-sql']
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
     description='Tryton module with timesheets',
     long_description=read('README.rst', slice=slice(0, -5)),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/timesheet',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton timesheet',
     package_dir={'trytond.modules.timesheet': '.'},
     packages=(
         ['trytond.modules.timesheet']
         + ['trytond.modules.timesheet.%s' % p for p in find_packages()]
         ),
@@ -126,24 +103,23 @@
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
     timesheet = trytond.modules.timesheet
     """,
     )
```

### Comparing `trytond_timesheet-6.6.0/timesheet.xml` & `trytond_timesheet-6.8.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/trytond_timesheet.egg-info/PKG-INFO` & `trytond_timesheet-6.8.0/trytond_timesheet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-timesheet
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with timesheets
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
-Project-URL: Source Code, https://hg.tryton.org/modules/timesheet
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton timesheet
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
 
 Timesheet Module
 ################
 
 The timesheet module allow to track the time spent by employees on
 various works. This module also comes with several reports that show
```

### Comparing `trytond_timesheet-6.6.0/trytond_timesheet.egg-info/SOURCES.txt` & `trytond_timesheet-6.8.0/trytond_timesheet.egg-info/SOURCES.txt`

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
 exceptions.py
@@ -67,14 +63,15 @@
 ./view/line_form.xml
 ./view/line_tree.xml
 ./view/work_context_form.xml
 ./view/work_form.xml
 ./view/work_graph.xml
 ./view/work_list.xml
 ./view/work_list_report.xml
+doc/conf.py
 doc/index.rst
 doc/user_application.rst
 icons/LICENSE
 icons/tryton-timesheet.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
```

### Comparing `trytond_timesheet-6.6.0/view/line_form.xml` & `trytond_timesheet-6.8.0/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/view/work_form.xml` & `trytond_timesheet-6.8.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/work.py` & `trytond_timesheet-6.8.0/work.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-6.6.0/work.xml` & `trytond_timesheet-6.8.0/work.xml`

 * *Files identical despite different names*

