# Comparing `tmp/trytond_stock_quantity_early_planning-6.6.0.tar.gz` & `tmp/trytond_stock_quantity_early_planning-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_quantity_early_planning-6.6.0.tar", last modified: Mon Oct 31 16:28:14 2022, max compression
+gzip compressed data, was "trytond_stock_quantity_early_planning-6.8.0.tar", last modified: Mon May  1 11:46:57 2023, max compression
```

## Comparing `trytond_stock_quantity_early_planning-6.6.0.tar` & `trytond_stock_quantity_early_planning-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:14.848892 trytond_stock_quantity_early_planning-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:02.000000 trytond_stock_quantity_early_planning-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 16:28:13.000000 trytond_stock_quantity_early_planning-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_quantity_early_planning-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2022-10-31 16:28:12.000000 trytond_stock_quantity_early_planning-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:28:12.000000 trytond_stock_quantity_early_planning-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_quantity_early_planning-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2553 2022-10-31 16:28:14.848892 trytond_stock_quantity_early_planning-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2022-10-27 11:24:45.000000 trytond_stock_quantity_early_planning-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:14.838891 trytond_stock_quantity_early_planning-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1692 2022-04-08 16:27:20.000000 trytond_stock_quantity_early_planning-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2022-10-27 11:24:45.000000 trytond_stock_quantity_early_planning-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:45.000000 trytond_stock_quantity_early_planning-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:14.828891 trytond_stock_quantity_early_planning-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4526 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:37.000000 trytond_stock_quantity_early_planning-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4531 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4557 2022-10-29 07:50:37.000000 trytond_stock_quantity_early_planning-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4575 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3865 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3823 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4480 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2022-10-29 07:50:38.000000 trytond_stock_quantity_early_planning-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:28:14.848892 trytond_stock_quantity_early_planning-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5618 2022-10-29 07:39:12.000000 trytond_stock_quantity_early_planning-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21291 2022-10-11 20:47:14.000000 trytond_stock_quantity_early_planning-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6786 2022-04-08 16:23:27.000000 trytond_stock_quantity_early_planning-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:14.828891 trytond_stock_quantity_early_planning-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_quantity_early_planning-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5243 2022-09-29 07:07:38.000000 trytond_stock_quantity_early_planning-6.6.0/tests/scenario_stock_quantity_early_planning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4902 2022-10-11 20:43:52.000000 trytond_stock_quantity_early_planning-6.6.0/tests/scenario_stock_quantity_early_planning_incoming.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2022-04-16 16:30:57.000000 trytond_stock_quantity_early_planning-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_quantity_early_planning-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2022-10-31 15:10:09.000000 trytond_stock_quantity_early_planning-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2022-10-31 16:28:11.000000 trytond_stock_quantity_early_planning-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:14.845558 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2553 2022-10-31 16:28:14.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1971 2022-10-31 16:28:14.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:28:14.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2022-10-31 16:28:14.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-03-28 12:58:17.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2022-10-31 16:28:14.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:28:14.000000 trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:28:14.835558 trytond_stock_quantity_early_planning-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1483 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/view/quantity_early_plan_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2021-04-03 16:26:39.000000 trytond_stock_quantity_early_planning-6.6.0/view/quantity_early_plan_generate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2022-04-08 16:23:27.000000 trytond_stock_quantity_early_planning-6.6.0/view/quantity_early_plan_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:57.346399 trytond_stock_quantity_early_planning-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-05-01 11:04:41.000000 trytond_stock_quantity_early_planning-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 11:04:41.000000 trytond_stock_quantity_early_planning-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2531 2023-05-01 11:46:57.346399 trytond_stock_quantity_early_planning-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:57.343066 trytond_stock_quantity_early_planning-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1692 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:57.339732 trytond_stock_quantity_early_planning-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4526 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4531 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4557 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4575 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3865 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3823 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4480 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-04-29 08:02:44.000000 trytond_stock_quantity_early_planning-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:46:57.346399 trytond_stock_quantity_early_planning-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4744 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21215 2023-04-21 08:36:08.000000 trytond_stock_quantity_early_planning-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6786 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:57.343066 trytond_stock_quantity_early_planning-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5182 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/tests/scenario_stock_quantity_early_planning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4842 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/tests/scenario_stock_quantity_early_planning_incoming.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2023-05-01 11:04:36.000000 trytond_stock_quantity_early_planning-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:57.346399 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2531 2023-05-01 11:46:56.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1933 2023-05-01 11:46:57.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:46:56.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-05-01 11:46:56.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-05-01 11:46:56.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:46:56.000000 trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:57.343066 trytond_stock_quantity_early_planning-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1483 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/view/quantity_early_plan_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/view/quantity_early_plan_generate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-6.8.0/view/quantity_early_plan_list.xml
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/CHANGELOG` & `trytond_stock_quantity_early_planning-6.8.0/CHANGELOG`

 * *Files 18% similar despite different names*

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
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/COPYRIGHT` & `trytond_stock_quantity_early_planning-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2022 Cédric Krier
+Copyright (C) 2021-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/LICENSE` & `trytond_stock_quantity_early_planning-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/PKG-INFO` & `trytond_stock_quantity_early_planning-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_quantity_early_planning
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to plan earlier shipments and productions
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-quantity-early-planning
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_quantity_early_planning
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock planning shipment production
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 ####################################
 Stock Quantity Early Planning Module
 ####################################
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/__init__.py` & `trytond_stock_quantity_early_planning-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/doc/conf.py` & `trytond_stock_quantity_early_planning-6.8.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
-modules_url = 'https://docs.tryton.org/projects/modules-{module}/en/{series}/'
-trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+import os
+
+base_url = os.environ.get('DOC_BASE_URL')
+if base_url:
+    modules_url = base_url + '/modules-{module}/'
+    trytond_url = base_url + '/server/'
+else:
+    modules_url = (
+        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
+    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
 
 
 def get_info():
     import configparser
-    import os
     import subprocess
     import sys
 
     module_dir = os.path.dirname(os.path.dirname(__file__))
 
     config = configparser.ConfigParser()
     config.read_file(open(os.path.join(module_dir, 'tryton.cfg')))
@@ -22,15 +29,18 @@
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
@@ -53,9 +63,10 @@
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
+linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
-del get_info, info, modules_url, trytond_url
+del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/doc/design.rst` & `trytond_stock_quantity_early_planning-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/bg.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/ca.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/cs.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/de.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/es.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/es_419.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/et.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/fa.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/fi.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/fr.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/hu.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/id.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/it.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/lo.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/lt.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/nl.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/pl.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/pt.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/ro.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/ru.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/sl.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/tr.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/uk.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/locale/zh_CN.po` & `trytond_stock_quantity_early_planning-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/setup.py` & `trytond_stock_quantity_early_planning-6.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     content = re.sub(
         r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
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
@@ -37,67 +34,45 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_quantity_early_planning'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-
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
+
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
-    'python-dateutil',
     get_require_version('proteus'),
     get_require_version('trytond_production'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module to plan earlier shipments and productions',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": ('https://docs.tryton.org/projects/'
             'modules-stock-quantity-early-planning'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": ('https://hg.tryton.org/modules/'
-            'stock_quantity_early_planning'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock planning shipment production',
     package_dir={'trytond.modules.stock_quantity_early_planning': '.'},
     packages=(
         ['trytond.modules.stock_quantity_early_planning']
         + ['trytond.modules.stock_quantity_early_planning.%s' % p
             for p in find_packages()]
@@ -135,27 +110,26 @@
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
     stock_quantity_early_planning = trytond.modules.stock_quantity_early_planning
     """,  # noqa: E501
     )
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/stock.py` & `trytond_stock_quantity_early_planning-6.8.0/stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,20 +200,18 @@
         return Location.get_default_warehouse()
 
     @fields.depends('origin')
     def on_change_with_warehouse(self, name=None):
         pool = Pool()
         Move = pool.get('stock.move')
         if isinstance(self.origin, Move) and self.origin.id >= 0:
-            warehouse = self.origin.from_location.warehouse
-            if warehouse:
-                return warehouse.id
+            return self.origin.from_location.warehouse
         elif (isinstance(self.origin, Model) and self.origin.id >= 0
-                and getattr(self.origin, 'warehouse', None)):
-            return self.origin.warehouse.id
+                and hasattr(self.origin, 'warehouse')):
+            return self.origin.warehouse
 
     def get_moves(self, name):
         pool = Pool()
         ShipmentOut = pool.get('stock.shipment.out')
         ShipmentInReturn = pool.get('stock.shipment.in.return')
         ShipmentInternal = pool.get('stock.shipment.internal')
         moves = []
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/stock.xml` & `trytond_stock_quantity_early_planning-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-6.6.0/tests/scenario_stock_quantity_early_planning.rst` & `trytond_stock_quantity_early_planning-6.8.0/tests/scenario_stock_quantity_early_planning.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 ======================================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
 
     >>> today = dt.date.today()
-    >>> week1 = today + relativedelta(weeks=1)
-    >>> week2 = today + relativedelta(weeks=2)
-    >>> week3 = today + relativedelta(weeks=3)
-    >>> week4 = today + relativedelta(weeks=4)
+    >>> week1 = today + dt.timedelta(weeks=1)
+    >>> week2 = today + dt.timedelta(weeks=2)
+    >>> week3 = today + dt.timedelta(weeks=3)
+    >>> week4 = today + dt.timedelta(weeks=4)
 
 Activate modules::
 
     >>> config = activate_modules('stock_quantity_early_planning')
 
     >>> Company = Model.get('company.company')
     >>> Location = Model.get('stock.location')
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/tests/scenario_stock_quantity_early_planning_incoming.rst` & `trytond_stock_quantity_early_planning-6.8.0/tests/scenario_stock_quantity_early_planning_incoming.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 ===============================================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
 
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
 
     >>> today = dt.date.today()
-    >>> week1 = today + relativedelta(weeks=1)
-    >>> week2 = today + relativedelta(weeks=2)
-    >>> week3 = today + relativedelta(weeks=3)
+    >>> week1 = today + dt.timedelta(weeks=1)
+    >>> week2 = today + dt.timedelta(weeks=2)
+    >>> week3 = today + dt.timedelta(weeks=3)
 
 Activate modules::
 
     >>> config = activate_modules('stock_quantity_early_planning')
 
     >>> Company = Model.get('company.company')
     >>> Location = Model.get('stock.location')
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO` & `trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-quantity-early-planning
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to plan earlier shipments and productions
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-quantity-early-planning
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_quantity_early_planning
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock planning shipment production
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 ####################################
 Stock Quantity Early Planning Module
 ####################################
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt` & `trytond_stock_quantity_early_planning-6.8.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt`

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
 setup.py
```

### Comparing `trytond_stock_quantity_early_planning-6.6.0/view/quantity_early_plan_form.xml` & `trytond_stock_quantity_early_planning-6.8.0/view/quantity_early_plan_form.xml`

 * *Files identical despite different names*

