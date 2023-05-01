# Comparing `tmp/trytond_production_work-6.6.1.tar.gz` & `tmp/trytond_production_work-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_work-6.6.1.tar", last modified: Mon Jan  2 22:56:56 2023, max compression
+gzip compressed data, was "trytond_production_work-6.8.0.tar", last modified: Mon May  1 11:37:27 2023, max compression
```

## Comparing `trytond_production_work-6.6.1.tar` & `trytond_production_work-6.8.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:56:56.978617 trytond_production_work-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1345 2023-01-02 22:56:54.000000 trytond_production_work-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-01-02 22:56:53.000000 trytond_production_work-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3820 2023-01-02 22:56:56.975283 trytond_production_work-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1551 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:56:56.975283 trytond_production_work-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1551 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:56:56.965283 trytond_production_work-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6718 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6572 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5974 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6677 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6607 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5756 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6117 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6406 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5948 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6611 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6352 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5739 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6193 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6767 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5998 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6467 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6195 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6263 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5610 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6778 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6209 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6212 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5602 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6178 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4938 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)      734 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1139 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/routing.py
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/routing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-01-02 22:56:56.978617 trytond_production_work-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4405 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:56:56.968617 trytond_production_work-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7072 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/tests/scenario_production_work.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2022-12-19 12:03:07.000000 trytond_production_work-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:56:56.975283 trytond_production_work-6.6.1/trytond_production_work.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3820 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2319 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-01-02 22:56:56.000000 trytond_production_work-6.6.1/trytond_production_work.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-01-02 22:56:56.971950 trytond_production_work-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/operation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_center_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_center_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      749 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_center_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_center_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_center_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      580 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_cycle_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_cycle_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      774 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/view/work_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12275 2022-12-19 12:03:07.000000 trytond_production_work-6.6.1/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15351 2022-12-19 12:02:50.000000 trytond_production_work-6.6.1/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:27.522661 trytond_production_work-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1408 2023-05-01 10:58:25.000000 trytond_production_work-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-05-01 10:58:25.000000 trytond_production_work-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3816 2023-05-01 11:37:27.522661 trytond_production_work-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:27.515994 trytond_production_work-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1555 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:27.512661 trytond_production_work-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6718 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6572 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5974 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6669 2023-04-30 10:46:36.000000 trytond_production_work-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6607 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5756 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6117 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6406 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5948 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6611 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6352 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5739 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6193 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6767 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5998 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6467 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6195 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6263 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5610 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6778 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6209 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-04-29 08:02:39.000000 trytond_production_work-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4938 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      734 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1139 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/routing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/routing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:37:27.522661 trytond_production_work-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4369 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:27.512661 trytond_production_work-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7001 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/tests/scenario_production_work.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 10:58:18.000000 trytond_production_work-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:27.519328 trytond_production_work-6.8.0/trytond_production_work.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3816 2023-05-01 11:37:26.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2319 2023-05-01 11:37:27.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:37:26.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:37:26.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      202 2023-05-01 11:37:26.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:37:26.000000 trytond_production_work-6.8.0/trytond_production_work.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:27.515994 trytond_production_work-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/view/operation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/view/work_center_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/work_center_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/view/work_center_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/work_center_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/work_center_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      580 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/view/work_cycle_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-01-16 14:00:21.000000 trytond_production_work-6.8.0/view/work_cycle_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      774 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/view/work_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12362 2023-04-21 08:36:08.000000 trytond_production_work-6.8.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15351 2023-04-15 07:12:15.000000 trytond_production_work-6.8.0/work.xml
```

### Comparing `trytond_production_work-6.6.1/CHANGELOG` & `trytond_production_work-6.8.0/CHANGELOG`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-Version 6.6.1 - 2023-01-02
+
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

### Comparing `trytond_production_work-6.6.1/COPYRIGHT` & `trytond_production_work-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2022 Cédric Krier.
-Copyright (C) 2015-2022 B2CK SPRL.
+Copyright (C) 2015-2023 Cédric Krier.
+Copyright (C) 2015-2023 B2CK SPRL.
 Copyright (C) 2013-2015 NaN·tic.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_production_work-6.6.1/LICENSE` & `trytond_production_work-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/PKG-INFO` & `trytond_production_work-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_production_work
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for production work
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production_work
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production work
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
 
 Production Work Module
 ######################
 
 The production work module allows to manage work order for each production.
@@ -61,15 +61,15 @@
 
 Work Center
 ***********
 
 Work center are places in the warehouse where production operations are
 performed. They can be organized in a tree structure and each center can be
 linked to a category. A cost can be defined on the work center with two
-methods: `Per Cycle` or `Per Hour`.
+methods: ``Per Cycle`` or ``Per Hour``.
 
 Work
 ****
 
 Works define for a production which operation to do at which work center.
 They also contains the number of cycles consumed to perform the operation.
```

### Comparing `trytond_production_work-6.6.1/README.rst` & `trytond_production_work-6.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Work Center
 ***********
 
 Work center are places in the warehouse where production operations are
 performed. They can be organized in a tree structure and each center can be
 linked to a category. A cost can be defined on the work center with two
-methods: `Per Cycle` or `Per Hour`.
+methods: ``Per Cycle`` or ``Per Hour``.
 
 Work
 ****
 
 Works define for a production which operation to do at which work center.
 They also contains the number of cycles consumed to perform the operation.
```

### Comparing `trytond_production_work-6.6.1/doc/conf.py` & `trytond_production_work-6.8.0/doc/conf.py`

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

### Comparing `trytond_production_work-6.6.1/doc/index.rst` & `trytond_production_work-6.8.0/doc/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Work Center
 ***********
 
 Work center are places in the warehouse where production operations are
 performed. They can be organized in a tree structure and each center can be
 linked to a category. A cost can be defined on the work center with two
-methods: `Per Cycle` or `Per Hour`.
+methods: ``Per Cycle`` or ``Per Hour``.
 
 Work
 ****
 
 Works define for a production which operation to do at which work center.
 They also contains the number of cycles consumed to perform the operation.
```

### Comparing `trytond_production_work-6.6.1/locale/bg.po` & `trytond_production_work-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/ca.po` & `trytond_production_work-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/cs.po` & `trytond_production_work-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/de.po` & `trytond_production_work-6.8.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 msgctxt "field:production.work.cycle,cost:"
 msgid "Cost"
 msgstr "Kosten"
 
 msgctxt "field:production.work.cycle,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:production.work.cycle,state:"
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:production.work.cycle,work:"
 msgid "Work"
@@ -112,15 +112,15 @@
 
 msgctxt "model:ir.action,name:act_work_center_tree"
 msgid "Work Centers"
 msgstr "Arbeitsplätze"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "Arbeitsaufträge"
+msgstr "Aufgaben"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
 msgstr "Alle"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_draft"
 msgid "Draft"
@@ -200,15 +200,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_work_center_tree"
 msgid "Work Centers"
 msgstr "Arbeitsplätze"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr "Arbeitsaufträge"
+msgstr "Aufgaben"
 
 msgctxt "model:production.work,name:"
 msgid "Production Work"
 msgstr "Arbeitsgang"
 
 msgctxt "model:production.work.center,name:"
 msgid "Work Center"
```

### Comparing `trytond_production_work-6.6.1/locale/es.po` & `trytond_production_work-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/es_419.po` & `trytond_production_work-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/et.po` & `trytond_production_work-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/fa.po` & `trytond_production_work-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/fi.po` & `trytond_production_work-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/fr.po` & `trytond_production_work-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/hu.po` & `trytond_production_work-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/id.po` & `trytond_production_work-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/it.po` & `trytond_production_work-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/lo.po` & `trytond_production_work-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/lt.po` & `trytond_production_work-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/nl.po` & `trytond_production_work-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/pl.po` & `trytond_production_work-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/pt.po` & `trytond_production_work-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/ro.po` & `trytond_production_work-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/ru.po` & `trytond_production_work-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/sl.po` & `trytond_production_work-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/tr.po` & `trytond_production_work-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/uk.po` & `trytond_production_work-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/locale/zh_CN.po` & `trytond_production_work-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/message.xml` & `trytond_production_work-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/production.py` & `trytond_production_work-6.8.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/production.xml` & `trytond_production_work-6.8.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/routing.py` & `trytond_production_work-6.8.0/routing.py`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/routing.xml` & `trytond_production_work-6.8.0/routing.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/setup.py` & `trytond_production_work-6.8.0/setup.py`

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
 name = 'trytond_production_work'
 
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
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for production work',
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
-        "Source Code": 'https://hg.tryton.org/modules/production_work',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton production work',
     package_dir={'trytond.modules.production_work': '.'},
     packages=(
         ['trytond.modules.production_work']
         + ['trytond.modules.production_work.%s' % p for p in find_packages()]
         ),
@@ -102,23 +102,23 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_production_work-6.6.1/tests/scenario_production_work.rst` & `trytond_production_work-6.8.0/tests/scenario_production_work.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ========================
 Production Work Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('production_work')
 
 Create company::
 
@@ -175,15 +175,14 @@
     True
     >>> work2.state
     'request'
 
 Run the production::
 
     >>> production.click('assign_try')
-    True
     >>> production.click('run')
     >>> production.state
     'running'
 
 Test works::
 
     >>> work1, work2 = production.works
@@ -212,15 +211,15 @@
     >>> cycle2.state
     'cancelled'
     >>> work2.reload()
     >>> work2.state
     'draft'
     >>> work2.click('start')
     >>> cycle2, = [c for c in work2.active_cycles]
-    >>> cycle2.duration = datetime.timedelta(hours=1)
+    >>> cycle2.duration = dt.timedelta(hours=1)
     >>> cycle2.save()
     >>> work2.click('stop')
     >>> work2.state
     'finished'
     >>> cycle2.reload()
     >>> cycle2.state
     'done'
```

### Comparing `trytond_production_work-6.6.1/trytond_production_work.egg-info/PKG-INFO` & `trytond_production_work-6.8.0/trytond_production_work.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-production-work
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module for production work
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
-Project-URL: Source Code, https://hg.tryton.org/modules/production_work
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton production work
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
 
 Production Work Module
 ######################
 
 The production work module allows to manage work order for each production.
@@ -61,15 +61,15 @@
 
 Work Center
 ***********
 
 Work center are places in the warehouse where production operations are
 performed. They can be organized in a tree structure and each center can be
 linked to a category. A cost can be defined on the work center with two
-methods: `Per Cycle` or `Per Hour`.
+methods: ``Per Cycle`` or ``Per Hour``.
 
 Work
 ****
 
 Works define for a production which operation to do at which work center.
 They also contains the number of cycles consumed to perform the operation.
```

### Comparing `trytond_production_work-6.6.1/trytond_production_work.egg-info/SOURCES.txt` & `trytond_production_work-6.8.0/trytond_production_work.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/view/production_form.xml` & `trytond_production_work-6.8.0/view/production_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/view/work_center_form.xml` & `trytond_production_work-6.8.0/view/work_center_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/view/work_cycle_form.xml` & `trytond_production_work-6.8.0/view/work_cycle_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/view/work_form.xml` & `trytond_production_work-6.8.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_work-6.6.1/work.py` & `trytond_production_work-6.8.0/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, Workflow, fields,
     sequence_ordered, tree)
 from trytond.model.exceptions import AccessError
 from trytond.modules.product import price_digits, round_price
 from trytond.pool import Pool
-from trytond.pyson import Bool, Eval, If
+from trytond.pyson import Bool, Eval, If, TimeDelta
 from trytond.transaction import Transaction
 
 from .exceptions import PickerError
 
 
 class WorkCenterCategory(ModelSQL, ModelView):
     'Work Center Category'
@@ -167,25 +167,23 @@
         table = cls.__table_handler__(module_name)
 
         # Migration from 5.4: Drop not null on work_center
         table.not_null_action('work_center', 'remove')
 
     @fields.depends('operation')
     def on_change_with_work_center_category(self, name=None):
-        if self.operation and self.operation.work_center_category:
-            return self.operation.work_center_category.id
+        return self.operation.work_center_category if self.operation else None
 
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @fields.depends('production', '_parent_production.warehouse')
     def on_change_with_warehouse(self, name=None):
-        if self.production:
-            return self.production.warehouse.id
+        return self.production.warehouse if self.production else None
 
     @classmethod
     def default_state(cls):
         return 'request'
 
     @classmethod
     @ModelView.button
@@ -279,15 +277,20 @@
 
 
 class WorkCycle(Workflow, ModelSQL, ModelView):
     'Work Cycle'
     __name__ = 'production.work.cycle'
     work = fields.Many2One(
         'production.work', "Work", required=True, ondelete='CASCADE')
-    duration = fields.TimeDelta('Duration',
+    duration = fields.TimeDelta(
+        "Duration",
+        domain=['OR',
+            ('duration', '=', None),
+            ('duration', '>=', TimeDelta()),
+            ],
         states={
             'required': Eval('state') == 'done',
             'readonly': Eval('state').in_(['done', 'draft', 'cancelled']),
             })
     cost = fields.Numeric('Cost', digits=price_digits, readonly=True)
     state = fields.Selection([
             ('draft', 'Draft'),
```

### Comparing `trytond_production_work-6.6.1/work.xml` & `trytond_production_work-6.8.0/work.xml`

 * *Files identical despite different names*

