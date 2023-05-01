# Comparing `tmp/trytond_production_work_timesheet-6.6.0.tar.gz` & `tmp/trytond_production_work_timesheet-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_work_timesheet-6.6.0.tar", last modified: Mon Oct 31 16:30:41 2022, max compression
+gzip compressed data, was "trytond_production_work_timesheet-6.8.0.tar", last modified: Mon May  1 12:02:28 2023, max compression
```

## Comparing `trytond_production_work_timesheet-6.6.0.tar` & `trytond_production_work_timesheet-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:30:41.257754 trytond_production_work_timesheet-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_production_work_timesheet-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_production_work_timesheet-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      611 2022-10-31 16:30:39.000000 trytond_production_work_timesheet-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_production_work_timesheet-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2022-10-31 16:30:39.000000 trytond_production_work_timesheet-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:30:38.000000 trytond_production_work_timesheet-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:51.000000 trytond_production_work_timesheet-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_production_work_timesheet-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2364 2022-10-31 16:30:41.257754 trytond_production_work_timesheet-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2019-06-04 16:49:45.000000 trytond_production_work_timesheet-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2021-12-11 16:59:33.000000 trytond_production_work_timesheet-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:30:41.254421 trytond_production_work_timesheet-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2019-06-04 16:49:45.000000 trytond_production_work_timesheet-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:30:41.254421 trytond_production_work_timesheet-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      673 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      636 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      621 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      641 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      634 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      561 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      839 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      646 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      689 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      647 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      671 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      603 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      667 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-29 07:50:44.000000 trytond_production_work_timesheet-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2021-12-11 16:59:33.000000 trytond_production_work_timesheet-6.6.0/routing.py
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2018-08-18 09:54:51.000000 trytond_production_work_timesheet-6.6.0/routing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:30:41.257754 trytond_production_work_timesheet-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5204 2022-10-29 07:39:11.000000 trytond_production_work_timesheet-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:30:41.254421 trytond_production_work_timesheet-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_production_work_timesheet-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3555 2022-10-27 22:35:30.000000 trytond_production_work_timesheet-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      639 2021-12-11 16:59:33.000000 trytond_production_work_timesheet-6.6.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:10:09.000000 trytond_production_work_timesheet-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2022-10-31 16:30:37.000000 trytond_production_work_timesheet-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:30:41.257754 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2364 2022-10-31 16:30:40.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1593 2022-10-31 16:30:41.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:30:40.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2022-10-31 16:30:40.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:12.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      125 2022-10-31 16:30:40.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:30:40.000000 trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:30:41.254421 trytond_production_work_timesheet-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2018-08-18 09:54:51.000000 trytond_production_work_timesheet-6.6.0/view/operation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2018-08-18 09:54:51.000000 trytond_production_work_timesheet-6.6.0/view/operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2018-08-18 09:54:51.000000 trytond_production_work_timesheet-6.6.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4321 2022-10-23 09:23:46.000000 trytond_production_work_timesheet-6.6.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2018-08-18 09:54:51.000000 trytond_production_work_timesheet-6.6.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:28.541288 trytond_production_work_timesheet-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1237 2023-05-01 11:15:23.000000 trytond_production_work_timesheet-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:15:22.000000 trytond_production_work_timesheet-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_work_timesheet-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-05-01 12:02:28.541288 trytond_production_work_timesheet-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:28.537955 trytond_production_work_timesheet-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:28.534621 trytond_production_work_timesheet-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      673 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      636 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-04-30 10:46:36.000000 trytond_production_work_timesheet-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      641 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      634 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      561 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      839 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      646 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      689 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      647 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      603 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-04-29 08:02:50.000000 trytond_production_work_timesheet-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/routing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-01-16 14:00:21.000000 trytond_production_work_timesheet-6.8.0/routing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:02:28.541288 trytond_production_work_timesheet-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4368 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:28.534621 trytond_production_work_timesheet-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3555 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      639 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-05-01 11:15:17.000000 trytond_production_work_timesheet-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:28.537955 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-05-01 12:02:27.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1567 2023-05-01 12:02:28.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:02:27.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 12:02:27.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      125 2023-05-01 12:02:27.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:02:27.000000 trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:28.537955 trytond_production_work_timesheet-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-01-16 14:00:21.000000 trytond_production_work_timesheet-6.8.0/view/operation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-01-16 14:00:21.000000 trytond_production_work_timesheet-6.8.0/view/operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_production_work_timesheet-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4321 2023-04-15 07:12:15.000000 trytond_production_work_timesheet-6.8.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-01-16 14:00:21.000000 trytond_production_work_timesheet-6.8.0/work.xml
```

### Comparing `trytond_production_work_timesheet-6.6.0/CHANGELOG` & `trytond_production_work_timesheet-6.8.0/CHANGELOG`

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

### Comparing `trytond_production_work_timesheet-6.6.0/COPYRIGHT` & `trytond_production_work_timesheet-6.8.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2016-2022 Cédric Krier
-Copyright (C) 2016-2022 B2CK
+Copyright (C) 2016-2023 Cédric Krier
+Copyright (C) 2016-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_production_work_timesheet-6.6.0/LICENSE` & `trytond_production_work_timesheet-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/PKG-INFO` & `trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_production_work_timesheet
-Version: 6.6.0
+Name: trytond-production-work-timesheet
+Version: 6.8.0
 Summary: Tryton module for timesheet on production work
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production_work_timesheet
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production work timesheet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 
 Production Work Timesheet Module
 ################################
 
 The production work timesheet module allows to enter timesheet for production
```

### Comparing `trytond_production_work_timesheet-6.6.0/locale/bg.po` & `trytond_production_work_timesheet-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/ca.po` & `trytond_production_work_timesheet-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/cs.po` & `trytond_production_work_timesheet-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/de.po` & `trytond_production_work_timesheet-6.8.0/locale/de.po`

 * *Files 16% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
 msgctxt "field:production.work,timesheet_lines:"
 msgid "Timesheet Lines"
 msgstr "Zeiterfassungspositionen"
 
 msgctxt "field:production.work,timesheet_work:"
 msgid "Timesheet Work"
-msgstr "Tätigkeit"
+msgstr "Aufgabe"
 
 msgctxt "field:production.work,timesheet_works:"
 msgid "Timesheet Works"
-msgstr "Tätigkeiten"
+msgstr "Aufgaben"
```

### Comparing `trytond_production_work_timesheet-6.6.0/locale/es.po` & `trytond_production_work_timesheet-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/es_419.po` & `trytond_production_work_timesheet-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/et.po` & `trytond_production_work_timesheet-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/fa.po` & `trytond_production_work_timesheet-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/fi.po` & `trytond_production_work_timesheet-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/fr.po` & `trytond_production_work_timesheet-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/hu.po` & `trytond_production_work_timesheet-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/id.po` & `trytond_production_work_timesheet-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/it.po` & `trytond_production_work_timesheet-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/lo.po` & `trytond_production_work_timesheet-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/lt.po` & `trytond_production_work_timesheet-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/nl.po` & `trytond_production_work_timesheet-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/pl.po` & `trytond_production_work_timesheet-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/pt.po` & `trytond_production_work_timesheet-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/ro.po` & `trytond_production_work_timesheet-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/ru.po` & `trytond_production_work_timesheet-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/sl.po` & `trytond_production_work_timesheet-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/tr.po` & `trytond_production_work_timesheet-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/uk.po` & `trytond_production_work_timesheet-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/locale/zh_CN.po` & `trytond_production_work_timesheet-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/routing.xml` & `trytond_production_work_timesheet-6.8.0/routing.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/setup.py` & `trytond_production_work_timesheet-6.8.0/setup.py`

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
@@ -34,61 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_production_work_timesheet'
 
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
     description='Tryton module for timesheet on production work',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/production_work_timesheet'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton production work timesheet',
     package_dir={'trytond.modules.production_work_timesheet': '.'},
     packages=(
         ['trytond.modules.production_work_timesheet']
         + ['trytond.modules.production_work_timesheet.%s' % p
             for p in find_packages()]
@@ -125,27 +102,26 @@
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
     production_work_timesheet = trytond.modules.production_work_timesheet
     """,
     )
```

### Comparing `trytond_production_work_timesheet-6.6.0/tests/test_module.py` & `trytond_production_work_timesheet-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/timesheet.py` & `trytond_production_work_timesheet-6.8.0/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/PKG-INFO` & `trytond_production_work_timesheet-6.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-production-work-timesheet
-Version: 6.6.0
+Name: trytond_production_work_timesheet
+Version: 6.8.0
 Summary: Tryton module for timesheet on production work
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production_work_timesheet
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production work timesheet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 
 Production Work Timesheet Module
 ################################
 
 The production work timesheet module allows to enter timesheet for production
```

### Comparing `trytond_production_work_timesheet-6.6.0/trytond_production_work_timesheet.egg-info/SOURCES.txt` & `trytond_production_work_timesheet-6.8.0/trytond_production_work_timesheet.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

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
 routing.py
@@ -48,14 +44,15 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/operation_form.xml
 ./view/operation_list.xml
 ./view/work_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_production_work_timesheet-6.6.0/work.py` & `trytond_production_work_timesheet-6.8.0/work.py`

 * *Files identical despite different names*

