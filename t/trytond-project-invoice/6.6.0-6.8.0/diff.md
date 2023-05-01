# Comparing `tmp/trytond_project_invoice-6.6.0.tar.gz` & `tmp/trytond_project_invoice-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_invoice-6.6.0.tar", last modified: Mon Oct 31 16:15:37 2022, max compression
+gzip compressed data, was "trytond_project_invoice-6.8.0.tar", last modified: Mon May  1 11:41:30 2023, max compression
```

## Comparing `trytond_project_invoice-6.6.0.tar` & `trytond_project_invoice-6.8.0.tar`

### file list

```diff
@@ -1,71 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_project_invoice-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_project_invoice-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2022-10-31 16:15:35.000000 trytond_project_invoice-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_project_invoice-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1941 2022-10-31 16:15:35.000000 trytond_project_invoice-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:15:34.000000 trytond_project_invoice-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:37.000000 trytond_project_invoice-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_project_invoice-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2767 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2020-01-28 10:46:04.000000 trytond_project_invoice-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2021-12-11 16:59:33.000000 trytond_project_invoice-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2020-01-28 10:46:04.000000 trytond_project_invoice-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2019-06-04 16:49:45.000000 trytond_project_invoice-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-11 16:59:33.000000 trytond_project_invoice-6.6.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:37.240782 trytond_project_invoice-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3399 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3799 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3068 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3917 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3823 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3177 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3427 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3806 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3068 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3856 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3097 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3122 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3784 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3285 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3317 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3743 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3115 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3517 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3347 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3537 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3068 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3068 2022-10-29 07:50:34.000000 trytond_project_invoice-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2020-03-28 12:06:53.000000 trytond_project_invoice-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    25886 2022-10-11 19:49:58.000000 trytond_project_invoice-6.6.0/project.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3222 2020-03-06 22:34:19.000000 trytond_project_invoice-6.6.0/project.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5180 2022-10-29 07:39:11.000000 trytond_project_invoice-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_project_invoice-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5746 2021-03-24 12:36:50.000000 trytond_project_invoice-6.6.0/tests/scenario_project_invoice_effort.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3408 2020-11-15 17:00:23.000000 trytond_project_invoice-6.6.0/tests/scenario_project_invoice_multiple_party.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5754 2021-03-24 12:36:50.000000 trytond_project_invoice-6.6.0/tests/scenario_project_invoice_progress.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6656 2021-11-22 09:16:05.000000 trytond_project_invoice-6.6.0/tests/scenario_project_invoice_timesheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2022-04-16 16:30:57.000000 trytond_project_invoice-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_project_invoice-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1336 2020-03-01 11:49:46.000000 trytond_project_invoice-6.6.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1250 2019-12-07 14:08:07.000000 trytond_project_invoice-6.6.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_project_invoice-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2022-10-31 16:15:33.000000 trytond_project_invoice-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2767 2022-10-31 16:15:36.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2105 2022-10-31 16:15:37.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:15:36.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 16:15:36.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:51.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2022-10-31 16:15:36.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:15:36.000000 trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:37.244115 trytond_project_invoice-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2021-10-07 13:08:06.000000 trytond_project_invoice-6.6.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2020-03-06 22:34:19.000000 trytond_project_invoice-6.6.0/view/work_invoiced_progress_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2020-03-06 22:34:19.000000 trytond_project_invoice-6.6.0/view/work_invoiced_progress_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2019-10-11 23:09:48.000000 trytond_project_invoice-6.6.0/view/work_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:30.792347 trytond_project_invoice-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2104 2023-05-01 11:01:07.000000 trytond_project_invoice-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:01:07.000000 trytond_project_invoice-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_invoice-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2023-05-01 11:41:30.792347 trytond_project_invoice-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:30.789013 trytond_project_invoice-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:30.785680 trytond_project_invoice-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3399 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3799 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3941 2023-04-30 10:46:36.000000 trytond_project_invoice-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3823 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3177 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3427 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3806 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3856 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3122 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3784 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3285 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3317 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3743 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3115 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3517 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2958 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3347 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3537 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2958 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3068 2023-04-29 08:02:40.000000 trytond_project_invoice-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    25780 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/project.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3222 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/project.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:41:30.792347 trytond_project_invoice-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4369 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:30.789013 trytond_project_invoice-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5639 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/scenario_project_invoice_effort.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3307 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/scenario_project_invoice_multiple_party.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5653 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/scenario_project_invoice_progress.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6633 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/scenario_project_invoice_timesheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1336 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1250 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-05-01 11:01:02.000000 trytond_project_invoice-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:30.792347 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2023-05-01 11:41:29.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2079 2023-05-01 11:41:30.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:41:29.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:41:29.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-05-01 11:41:29.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:41:29.000000 trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:41:30.789013 trytond_project_invoice-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/view/work_invoiced_progress_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/view/work_invoiced_progress_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_project_invoice-6.8.0/view/work_list.xml
```

### Comparing `trytond_project_invoice-6.6.0/CHANGELOG` & `trytond_project_invoice-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

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

### Comparing `trytond_project_invoice-6.6.0/COPYRIGHT` & `trytond_project_invoice-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2013-2022 Cédric Krier.
-Copyright (C) 2013-2022 B2CK SPRL.
+Copyright (C) 2013-2023 Cédric Krier.
+Copyright (C) 2013-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_project_invoice-6.6.0/LICENSE` & `trytond_project_invoice-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/PKG-INFO` & `trytond_project_invoice-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_project_invoice
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to invoice projects
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
-Project-URL: Source Code, https://hg.tryton.org/modules/project_invoice
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project invoice
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
 
 Project Invoice Module
 ######################
 
 The Project Invoice module adds invoice methods on project.
```

### Comparing `trytond_project_invoice-6.6.0/__init__.py` & `trytond_project_invoice-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/invoice.py` & `trytond_project_invoice-6.8.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/bg.po` & `trytond_project_invoice-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/ca.po` & `trytond_project_invoice-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/cs.po` & `trytond_project_invoice-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/de.po` & `trytond_project_invoice-6.8.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 msgctxt "field:project.work.invoiced_progress,progress:"
 msgid "Progress"
 msgstr "Fortschritt"
 
 msgctxt "field:project.work.invoiced_progress,work:"
 msgid "Work"
-msgstr "Tätigkeit"
+msgstr "Projektaufgabe"
 
 msgctxt "field:timesheet.line,invoice_line:"
 msgid "Invoice Line"
 msgstr "Rechnungsposition"
 
 msgctxt "help:project.work,project_invoice_timesheet_up_to:"
 msgid ""
@@ -77,19 +77,19 @@
 msgid "To invoice work \"%(work)s\" you must configure a default account revenue."
 msgstr ""
 "Damit Projekt \"%(work)s\" fakturiert werden kann, muss ein "
 "Standardertragskonto konfiguriert werden."
 
 msgctxt "model:ir.message,text:msg_missing_list_price"
 msgid "There is no list price on work \"%(work)s\"."
-msgstr "Fehlender Listenpreis für Aufgabe \"%(work)s\"."
+msgstr "Fehlender Listenpreis für Projektaufgabe \"%(work)s\"."
 
 msgctxt "model:ir.message,text:msg_missing_party"
 msgid "There is no party on work \"%(work)s\"."
-msgstr "Fehlende Partei für Aufgabe \"%(work)s\"."
+msgstr "Fehlende Partei für Projektaufgabe \"%(work)s\"."
 
 msgctxt "model:ir.message,text:msg_modify_invoiced_line"
 msgid "You cannot modify an invoiced line."
 msgstr "Eine festgeschriebene Rechnungsposition kann nicht geändert werden."
 
 msgctxt "model:ir.message,text:msg_product_missing_account_revenue"
 msgid ""
@@ -101,15 +101,15 @@
 
 msgctxt "model:ir.model.button,string:work_invoice_button"
 msgid "Invoice"
 msgstr "Rechnung erstellen"
 
 msgctxt "model:project.work.invoiced_progress,name:"
 msgid "Work Invoiced Progress"
-msgstr "Nach Forstschritt fakturierte Aufgabe"
+msgstr "Nach Fortschritt fakturierte Projektaufgabe"
 
 msgctxt "model:res.group,name:group_project_invoice"
 msgid "Project Invoice"
 msgstr "Projekt Fakturierung"
 
 msgctxt "selection:project.work,project_invoice_method:"
 msgid "Manual"
```

### Comparing `trytond_project_invoice-6.6.0/locale/es.po` & `trytond_project_invoice-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/es_419.po` & `trytond_project_invoice-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/et.po` & `trytond_project_invoice-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/fa.po` & `trytond_project_invoice-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/fi.po` & `trytond_project_invoice-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/fr.po` & `trytond_project_invoice-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/hu.po` & `trytond_project_invoice-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/id.po` & `trytond_project_invoice-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/it.po` & `trytond_project_invoice-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/lo.po` & `trytond_project_invoice-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/lt.po` & `trytond_project_invoice-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/nl.po` & `trytond_project_invoice-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/pl.po` & `trytond_project_invoice-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/pt.po` & `trytond_project_invoice-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/ro.po` & `trytond_project_invoice-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/ru.po` & `trytond_project_invoice-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/sl.po` & `trytond_project_invoice-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/tr.po` & `trytond_project_invoice-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/uk.po` & `trytond_project_invoice-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/locale/zh_CN.po` & `trytond_project_invoice-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/message.xml` & `trytond_project_invoice-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/project.py` & `trytond_project_invoice-6.8.0/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             ('effort', "On Effort"))
 
     @classmethod
     def _get_quantity_to_invoice_effort(cls, works):
         quantities = {}
         for work in works:
             if (work.progress == 1
-                    and work.list_price
+                    and work.invoice_unit_price
                     and not work.invoice_line):
                 if work.price_list_hour:
                     quantity = work.effort_hours
                 else:
                     quantity = 1
                 if work.unit_to_invoice:
                     quantity = work.unit_to_invoice.round(quantity)
@@ -111,27 +111,27 @@
         progress = Progress.__table__()
 
         invoiced_progress = {}
         quantities = {}
         for sub_works in grouped_slice(works):
             sub_works = list(sub_works)
             where = reduce_ids(
-                table.id, [x.id for x in sub_works if x.list_price])
+                table.id, [x.id for x in sub_works if x.invoice_unit_price])
             cursor.execute(*table.join(progress,
                     condition=progress.work == table.id
                     ).select(table.id, Sum(progress.progress),
                     where=where,
                     group_by=table.id))
             invoiced_progress.update(dict(cursor))
 
             for work in sub_works:
                 delta = (
                     (work.progress or 0)
                     - invoiced_progress.get(work.id, 0.0))
-                if work.list_price and delta > 0:
+                if work.invoice_unit_price and delta > 0:
                     quantity = delta
                     if work.price_list_hour:
                         quantity *= work.effort_hours
                     if work.unit_to_invoice:
                         quantity = work.unit_to_invoice.round(quantity)
                     quantities[work.id] = quantity
         return quantities
@@ -284,15 +284,15 @@
                         if not isinstance(duration, datetime.timedelta):
                             duration = datetime.timedelta(seconds=duration)
                         durations[twork2work[twork_id]] += duration
 
         quantities = {}
         for work in works:
             duration = durations[work.id]
-            if work.list_price:
+            if work.invoice_unit_price:
                 hours = duration.total_seconds() / 60 / 60
                 if work.unit_to_invoice:
                     hours = work.unit_to_invoice.round(hours)
                 quantities[work.id] = hours
         return quantities
 
     @classmethod
@@ -504,21 +504,19 @@
                 invoice_line = work._get_invoice_line(key, invoice, lines)
                 invoice_line.invoice = invoice.id
                 invoice_line.save()
                 origins = defaultdict(list)
                 for line in lines:
                     for origin in line['origins']:
                         origins[origin.__class__].append(origin)
-                # TODO: remove when _check_access ignores record rule
-                with Transaction().set_user(0):
-                    for klass, records in origins.items():
-                        klass.save(records)  # Store first new origins
-                        klass.write(records, {
-                                'invoice_line': invoice_line.id,
-                                })
+                for klass, records in origins.items():
+                    klass.save(records)  # Store first new origins
+                    klass.write(records, {
+                            'invoice_line': invoice_line.id,
+                            })
         Invoice.update_taxes(invoices)
 
     def _get_invoice(self):
         "Return invoice for the work"
         pool = Pool()
         Invoice = pool.get('account.invoice')
         Journal = pool.get('account.journal')
```

### Comparing `trytond_project_invoice-6.6.0/project.xml` & `trytond_project_invoice-6.8.0/project.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/setup.py` & `trytond_project_invoice-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
 name = 'trytond_project_invoice'
 
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
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to invoice projects',
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
-        "Source Code": 'https://hg.tryton.org/modules/project_invoice',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton project invoice',
     package_dir={'trytond.modules.project_invoice': '.'},
     packages=(
         ['trytond.modules.project_invoice']
         + ['trytond.modules.project_invoice.%s' % p for p in find_packages()]
         ),
@@ -124,27 +102,26 @@
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
     project_invoice = trytond.modules.project_invoice
     """,
     )
```

### Comparing `trytond_project_invoice-6.6.0/tests/scenario_project_invoice_effort.rst` & `trytond_project_invoice-6.8.0/tests/scenario_project_invoice_effort.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ===============================
 Project Invoice Effort Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_chart, \
     ...     get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
 
@@ -116,28 +114,28 @@
     >>> ProjectWork = Model.get('project.work')
     >>> project = ProjectWork()
     >>> project.name = 'Test effort'
     >>> project.type = 'project'
     >>> project.party = customer
     >>> project.project_invoice_method = 'effort'
     >>> project.product = product
-    >>> project.effort_duration = datetime.timedelta(hours=1)
+    >>> project.effort_duration = dt.timedelta(hours=1)
     >>> task = project.children.new()
     >>> task.name = 'Task 1'
     >>> task.type = 'task'
     >>> task.product = product
-    >>> task.effort_duration = datetime.timedelta(hours=5)
+    >>> task.effort_duration = dt.timedelta(hours=5)
     >>> task_no_effort = project.children.new()
     >>> task_no_effort.name = "Task 2"
     >>> task_no_effort.type = 'task'
     >>> task_no_effort.effort_duration = None
     >>> task_fixed = project.children.new()
     >>> task_fixed.name = "Task 2"
     >>> task_fixed.type = 'task'
-    >>> task_fixed.effort_duration = datetime.timedelta(hours=2)
+    >>> task_fixed.effort_duration = dt.timedelta(hours=2)
     >>> task_fixed.product = product_fixed
     >>> project.save()
     >>> task, task_no_effort, task_fixed = project.children
 
 Check project amounts::
 
     >>> project.reload()
```

### Comparing `trytond_project_invoice-6.6.0/tests/scenario_project_invoice_multiple_party.rst` & `trytond_project_invoice-6.8.0/tests/scenario_project_invoice_multiple_party.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 =========================================
 Project Invoice Multiple Parties Scenario
 =========================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_chart, \
     ...     get_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
 
@@ -66,23 +64,23 @@
     >>> ProjectWork = Model.get('project.work')
     >>> project = ProjectWork()
     >>> project.name = 'Test multiple party'
     >>> project.type = 'project'
     >>> project.party = customer1
     >>> project.project_invoice_method = 'effort'
     >>> project.product = product
-    >>> project.effort_duration = datetime.timedelta(hours=1)
+    >>> project.effort_duration = dt.timedelta(hours=1)
 
     >>> subproject = project.children.new()
     >>> subproject.name = 'Subproject'
     >>> subproject.type = 'project'
     >>> subproject.party = customer2
     >>> subproject.project_invoice_method = 'effort'
     >>> subproject.product = product
-    >>> subproject.effort_duration = datetime.timedelta(hours=5)
+    >>> subproject.effort_duration = dt.timedelta(hours=5)
 
     >>> project.save()
     >>> subproject, = project.children
 
 Check project amounts::
 
     >>> project.reload()
```

### Comparing `trytond_project_invoice-6.6.0/tests/scenario_project_invoice_progress.rst` & `trytond_project_invoice-6.8.0/tests/scenario_project_invoice_progress.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 =================================
 Project Invoice Progress Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_chart, \
     ...     get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
 
@@ -120,20 +118,20 @@
     >>> TimesheetWork = Model.get('timesheet.work')
     >>> project = ProjectWork()
     >>> project.name = 'Test effort'
     >>> project.type = 'project'
     >>> project.party = customer
     >>> project.project_invoice_method = 'progress'
     >>> project.product = product
-    >>> project.effort_duration = datetime.timedelta(hours=1)
+    >>> project.effort_duration = dt.timedelta(hours=1)
     >>> task = project.children.new()
     >>> task.name = 'Task 1'
     >>> task.type = 'task'
     >>> task.product = product
-    >>> task.effort_duration = datetime.timedelta(hours=5)
+    >>> task.effort_duration = dt.timedelta(hours=5)
     >>> task_fixed = project.children.new()
     >>> task_fixed.name = 'Task 2'
     >>> task_fixed.type = 'task'
     >>> task_fixed.product = product
     >>> task_fixed.product = product_fixed
     >>> project.save()
     >>> task, task_fixed = project.children
```

### Comparing `trytond_project_invoice-6.6.0/tests/scenario_project_invoice_timesheet.rst` & `trytond_project_invoice-6.8.0/tests/scenario_project_invoice_timesheet.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 ==================================
 Project Invoice Timesheet Scenario
 ==================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_chart, \
     ...     get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     create_payment_term
-    >>> today = datetime.date.today()
-    >>> yesterday = today - datetime.timedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
 
@@ -131,21 +132,21 @@
 
 Create timesheets::
 
     >>> TimesheetLine = Model.get('timesheet.line')
     >>> line = TimesheetLine()
     >>> line.date = yesterday
     >>> line.employee = employee
-    >>> line.duration = datetime.timedelta(hours=3)
+    >>> line.duration = dt.timedelta(hours=3)
     >>> line.work, = task.timesheet_works
     >>> line.save()
     >>> line = TimesheetLine()
     >>> line.date = today
     >>> line.employee = employee
-    >>> line.duration = datetime.timedelta(hours=2)
+    >>> line.duration = dt.timedelta(hours=2)
     >>> line.work, = project.timesheet_works
     >>> line.save()
 
 Check project amounts::
 
     >>> project.reload()
     >>> project.amount_to_invoice
@@ -195,15 +196,15 @@
 
 Create more timesheets::
 
     >>> set_user(project_user)
     >>> TimesheetLine = Model.get('timesheet.line')
     >>> line = TimesheetLine()
     >>> line.employee = employee
-    >>> line.duration = datetime.timedelta(hours=4)
+    >>> line.duration = dt.timedelta(hours=4)
     >>> line.work, = task.timesheet_works
     >>> line.save()
 
 Check project amounts::
 
     >>> project.reload()
     >>> project.amount_to_invoice
```

### Comparing `trytond_project_invoice-6.6.0/timesheet.py` & `trytond_project_invoice-6.8.0/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/timesheet.xml` & `trytond_project_invoice-6.8.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/PKG-INFO` & `trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-project-invoice
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to invoice projects
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
-Project-URL: Source Code, https://hg.tryton.org/modules/project_invoice
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project invoice
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
 
 Project Invoice Module
 ######################
 
 The Project Invoice module adds invoice methods on project.
```

### Comparing `trytond_project_invoice-6.6.0/trytond_project_invoice.egg-info/SOURCES.txt` & `trytond_project_invoice-6.8.0/trytond_project_invoice.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
@@ -58,14 +54,15 @@
 ./tests/scenario_project_invoice_timesheet.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/work_form.xml
 ./view/work_invoiced_progress_form.xml
 ./view/work_invoiced_progress_list.xml
 ./view/work_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_project_invoice-6.6.0/view/work_form.xml` & `trytond_project_invoice-6.8.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-6.6.0/view/work_invoiced_progress_form.xml` & `trytond_project_invoice-6.8.0/view/work_invoiced_progress_form.xml`

 * *Files identical despite different names*

