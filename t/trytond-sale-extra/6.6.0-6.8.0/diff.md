# Comparing `tmp/trytond_sale_extra-6.6.0.tar.gz` & `tmp/trytond_sale_extra-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_extra-6.6.0.tar", last modified: Mon Oct 31 16:16:35 2022, max compression
+gzip compressed data, was "trytond_sale_extra-6.8.0.tar", last modified: Mon May  1 11:59:39 2023, max compression
```

## Comparing `trytond_sale_extra-6.6.0.tar` & `trytond_sale_extra-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:35.138290 trytond_sale_extra-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_extra-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_extra-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-31 16:16:33.000000 trytond_sale_extra-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_extra-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1433 2022-10-31 16:16:33.000000 trytond_sale_extra-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:16:32.000000 trytond_sale_extra-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:02.000000 trytond_sale_extra-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_extra-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3379 2022-10-31 16:16:35.138290 trytond_sale_extra-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2018-08-18 09:55:02.000000 trytond_sale_extra-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2021-12-11 16:59:34.000000 trytond_sale_extra-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:35.134957 trytond_sale_extra-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2018-08-18 09:55:02.000000 trytond_sale_extra-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:35.134957 trytond_sale_extra-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2189 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1976 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1970 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1765 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2008 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2151 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1840 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1921 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1970 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1979 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2028 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1997 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2022-10-29 07:50:43.000000 trytond_sale_extra-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8920 2022-10-11 19:49:58.000000 trytond_sale_extra-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4683 2021-04-27 07:34:41.000000 trytond_sale_extra-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:16:35.138290 trytond_sale_extra-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5153 2022-10-29 07:39:11.000000 trytond_sale_extra-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:35.134957 trytond_sale_extra-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_extra-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4718 2020-07-09 09:37:18.000000 trytond_sale_extra-6.6.0/tests/scenario_sale_extra.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-04-16 16:30:57.000000 trytond_sale_extra-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_extra-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-10-31 15:10:09.000000 trytond_sale_extra-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 16:16:31.000000 trytond_sale_extra-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:35.134957 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3379 2022-10-31 16:16:34.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1638 2022-10-31 16:16:35.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:16:34.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2022-10-31 16:16:34.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:10.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2022-10-31 16:16:34.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:16:34.000000 trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:35.134957 trytond_sale_extra-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      732 2018-08-18 09:55:02.000000 trytond_sale_extra-6.6.0/view/extra_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2018-08-18 09:55:02.000000 trytond_sale_extra-6.6.0/view/extra_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2019-10-11 23:09:48.000000 trytond_sale_extra-6.6.0/view/extra_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2019-10-11 23:09:48.000000 trytond_sale_extra-6.6.0/view/extra_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2022-04-08 16:23:26.000000 trytond_sale_extra-6.6.0/view/extra_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:39.975863 trytond_sale_extra-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-05-01 11:13:22.000000 trytond_sale_extra-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:13:22.000000 trytond_sale_extra-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_extra-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3376 2023-05-01 11:59:39.975863 trytond_sale_extra-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-01-16 14:00:21.000000 trytond_sale_extra-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:39.972530 trytond_sale_extra-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-01-16 14:00:21.000000 trytond_sale_extra-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:39.969196 trytond_sale_extra-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2189 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1976 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1765 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2008 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2151 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1840 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1921 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1970 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1979 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2028 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2199 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1997 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1808 2023-04-29 08:02:49.000000 trytond_sale_extra-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8876 2023-04-21 08:36:08.000000 trytond_sale_extra-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4683 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:59:39.975863 trytond_sale_extra-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4347 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:39.972530 trytond_sale_extra-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4617 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/tests/scenario_sale_extra.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 11:13:16.000000 trytond_sale_extra-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:39.975863 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3376 2023-05-01 11:59:39.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1612 2023-05-01 11:59:39.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:59:39.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:59:39.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-05-01 11:59:39.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:59:39.000000 trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:39.972530 trytond_sale_extra-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      732 2023-01-16 14:00:21.000000 trytond_sale_extra-6.8.0/view/extra_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-01-16 14:00:21.000000 trytond_sale_extra-6.8.0/view/extra_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/view/extra_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/view/extra_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_sale_extra-6.8.0/view/extra_list.xml
```

### Comparing `trytond_sale_extra-6.6.0/CHANGELOG` & `trytond_sale_extra-6.8.0/CHANGELOG`

 * *Files 15% similar despite different names*

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

### Comparing `trytond_sale_extra-6.6.0/COPYRIGHT` & `trytond_sale_extra-6.8.0/COPYRIGHT`

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

### Comparing `trytond_sale_extra-6.6.0/LICENSE` & `trytond_sale_extra-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/PKG-INFO` & `trytond_sale_extra-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_extra
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale extra
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_extra
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale extra premium cost
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
 
 Sale Extra
 ##########
 
 The sale_extra module allows to add extra line on sale based on criteria.
```

### Comparing `trytond_sale_extra-6.6.0/README.rst` & `trytond_sale_extra-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/doc/index.rst` & `trytond_sale_extra-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/bg.po` & `trytond_sale_extra-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/ca.po` & `trytond_sale_extra-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/cs.po` & `trytond_sale_extra-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/de.po` & `trytond_sale_extra-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/es.po` & `trytond_sale_extra-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/es_419.po` & `trytond_sale_extra-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/et.po` & `trytond_sale_extra-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/fa.po` & `trytond_sale_extra-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/fi.po` & `trytond_sale_extra-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/fr.po` & `trytond_sale_extra-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/hu.po` & `trytond_sale_extra-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/id.po` & `trytond_sale_extra-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/it.po` & `trytond_sale_extra-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/lo.po` & `trytond_sale_extra-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/lt.po` & `trytond_sale_extra-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/nl.po` & `trytond_sale_extra-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/pl.po` & `trytond_sale_extra-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/pt.po` & `trytond_sale_extra-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/ro.po` & `trytond_sale_extra-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/ru.po` & `trytond_sale_extra-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/sl.po` & `trytond_sale_extra-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/tr.po` & `trytond_sale_extra-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/uk.po` & `trytond_sale_extra-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/locale/zh_CN.po` & `trytond_sale_extra-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/sale.py` & `trytond_sale_extra-6.8.0/sale.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,41 +22,44 @@
     @Workflow.transition('quotation')
     def quote(cls, sales):
         pool = Pool()
         Line = pool.get('sale.line')
 
         super(Sale, cls).quote(sales)
 
-        lines_to_delete = []
+        # State must be draft to add or delete lines
+        # because extra must be set after to have correct amount
+        cls.write(sales, {'state': 'draft'})
+        removed = []
         for sale in sales:
-            sale.set_extra(lines_to_delete)
-        if lines_to_delete:
-            Line.delete(lines_to_delete)
+            removed.extend(sale.set_extra())
+        Line.delete(removed)
         cls.save(sales)
 
-    def set_extra(self, lines_to_delete):
+    def set_extra(self):
         'Set extra lines and fill lines_to_delete'
         pool = Pool()
         Extra = pool.get('sale.extra')
-
+        removed = []
         extra_lines = Extra.get_lines(self)
         extra2lines = {line.extra: line for line in extra_lines}
         lines = list(self.lines)
         for line in list(lines):
             if line.type != 'line' or not line.extra:
                 continue
             if line.extra in extra2lines:
                 del extra2lines[line.extra]
                 continue
             else:
                 lines.remove(line)
-                lines_to_delete.append(line)
+                removed.append(line)
         if extra2lines:
             lines.extend(extra2lines.values())
         self.lines = lines
+        return removed
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'sale.line'
 
     extra = fields.Many2One('sale.extra.line', 'Extra', ondelete='RESTRICT')
 
@@ -124,16 +127,15 @@
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @classmethod
     def _extras_domain(cls, sale):
         return [
             ['OR',
                 ('start_date', '<=', sale.sale_date),
                 ('start_date', '=', None),
@@ -147,40 +149,33 @@
                 ('price_list', '=',
                     sale.price_list.id if sale.price_list else None),
                 ],
             ('company', '=', sale.company.id),
             ]
 
     @classmethod
-    def get_lines(cls, sale, pattern=None):
+    def get_lines(cls, sale, pattern=None, line_pattern=None):
         'Yield extra sale lines'
         pool = Pool()
         Currency = pool.get('currency.currency')
         extras = cls.search(cls._extras_domain(sale))
-        if pattern is None:
-            pattern = {}
-        else:
-            pattern = pattern.copy()
-        pattern['sale_amount'] = Currency.compute(sale.currency,
-            sale.untaxed_amount, sale.company.currency)
+        pattern = pattern.copy() if pattern is not None else {}
+        line_pattern = line_pattern.copy() if line_pattern is not None else {}
+        sale_amount = Currency.compute(
+            sale.currency, sale.untaxed_amount, sale.company.currency)
+        pattern.setdefault('sale_amount', sale_amount)
+        line_pattern.setdefault('sale_amount', sale_amount)
 
         for extra in extras:
-            epattern = pattern.copy()
-            epattern.update(extra.get_pattern(sale))
-            if extra.match(epattern):
+            if extra.match(pattern):
                 for line in extra.lines:
-                    lpattern = epattern.copy()
-                    lpattern.update(line.get_pattern(sale))
-                    if line.match(lpattern):
+                    if line.match(line_pattern):
                         yield line.get_line(sale)
                         break
 
-    def get_pattern(self, sale):
-        return {}
-
     def match(self, pattern):
         pattern = pattern.copy()
         sale_amount = pattern.pop('sale_amount')
 
         match = super().match(pattern)
 
         if self.sale_amount is not None:
@@ -216,33 +211,28 @@
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('extra')
         cls._order.insert(1, ('extra', 'ASC'))
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @fields.depends('product')
     def on_change_product(self):
         if self.product:
             self.unit = self.product.sale_uom
 
     @staticmethod
     def default_free():
         return False
 
     @fields.depends('extra', '_parent_extra.currency')
     def on_change_with_currency(self, name=None):
-        if self.extra and self.extra.currency:
-            return self.extra.currency.id
-
-    def get_pattern(self, sale):
-        return {}
+        return self.extra.currency if self.extra else None
 
     def match(self, pattern):
         pattern = pattern.copy()
         sale_amount = pattern.pop('sale_amount')
 
         match = super().match(pattern)
```

### Comparing `trytond_sale_extra-6.6.0/sale.xml` & `trytond_sale_extra-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/setup.py` & `trytond_sale_extra-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
 name = 'trytond_sale_extra'
 
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
 
 requires = ['python-sql']
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
     description='Tryton module for sale extra',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_extra',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale extra premium cost',
     package_dir={'trytond.modules.sale_extra': '.'},
     packages=(
         ['trytond.modules.sale_extra']
         + ['trytond.modules.sale_extra.%s' % p for p in find_packages()]
         ),
@@ -123,28 +101,27 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     sale_extra = trytond.modules.sale_extra
     """,
     )
```

### Comparing `trytond_sale_extra-6.6.0/tests/scenario_sale_extra.rst` & `trytond_sale_extra-6.8.0/tests/scenario_sale_extra.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ===================
 Sale Extra Scenario
 ===================
 
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
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     create_payment_term
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('sale_extra')
 
 Create company::
 
@@ -54,26 +52,26 @@
     >>> unit, = ProductUom.find([('name', '=', 'Unit')])
 
     >>> template = ProductTemplate()
     >>> template.name = 'Product'
     >>> template.default_uom = unit
     >>> template.type = 'goods'
     >>> template.salable = True
-    >>> template.lead_time = datetime.timedelta(0)
+    >>> template.lead_time = dt.timedelta(0)
     >>> template.list_price = Decimal('20')
     >>> template.account_category = account_category
     >>> template.save()
     >>> product, = template.products
 
     >>> extra_template = ProductTemplate()
     >>> extra_template.name = 'Extra'
     >>> extra_template.default_uom = unit
     >>> extra_template.type = 'service'
     >>> extra_template.salable = True
-    >>> extra_template.lead_time = datetime.timedelta(0)
+    >>> extra_template.lead_time = dt.timedelta(0)
     >>> extra_template.list_price = Decimal('3')
     >>> extra_template.account_category = account_category
     >>> extra_template.save()
     >>> extra_product, = extra_template.products
 
 Create payment term::
```

### Comparing `trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/PKG-INFO` & `trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-extra
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sale extra
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_extra
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale extra premium cost
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
 
 Sale Extra
 ##########
 
 The sale_extra module allows to add extra line on sale based on criteria.
```

### Comparing `trytond_sale_extra-6.6.0/trytond_sale_extra.egg-info/SOURCES.txt` & `trytond_sale_extra-6.8.0/trytond_sale_extra.egg-info/SOURCES.txt`

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
 sale.py
@@ -46,14 +42,15 @@
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/extra_form.xml
 ./view/extra_line_form.xml
 ./view/extra_line_list.xml
 ./view/extra_line_list_sequence.xml
 ./view/extra_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_sale_extra-6.6.0/view/extra_form.xml` & `trytond_sale_extra-6.8.0/view/extra_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_extra-6.6.0/view/extra_line_form.xml` & `trytond_sale_extra-6.8.0/view/extra_line_form.xml`

 * *Files identical despite different names*

