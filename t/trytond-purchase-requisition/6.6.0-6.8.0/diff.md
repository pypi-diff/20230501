# Comparing `tmp/trytond_purchase_requisition-6.6.0.tar.gz` & `tmp/trytond_purchase_requisition-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_requisition-6.6.0.tar", last modified: Mon Oct 31 16:16:20 2022, max compression
+gzip compressed data, was "trytond_purchase_requisition-6.8.0.tar", last modified: Mon May  1 11:44:13 2023, max compression
```

## Comparing `trytond_purchase_requisition-6.6.0.tar` & `trytond_purchase_requisition-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:20.368075 trytond_purchase_requisition-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_purchase_requisition-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_purchase_requisition-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      611 2022-10-31 16:16:19.000000 trytond_purchase_requisition-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_purchase_requisition-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1571 2022-10-31 16:16:18.000000 trytond_purchase_requisition-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2022-10-31 16:16:17.000000 trytond_purchase_requisition-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:38.000000 trytond_purchase_requisition-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_purchase_requisition-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3596 2022-10-31 16:16:20.368075 trytond_purchase_requisition-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2020-06-04 11:08:34.000000 trytond_purchase_requisition-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2021-12-11 16:59:33.000000 trytond_purchase_requisition-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:20.364742 trytond_purchase_requisition-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2020-06-04 11:08:34.000000 trytond_purchase_requisition-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:20.361409 trytond_purchase_requisition-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6654 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6796 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6659 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5919 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6424 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7011 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6829 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6008 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6692 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6391 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6720 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6556 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6740 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5880 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6630 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5759 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2022-10-29 07:50:35.000000 trytond_purchase_requisition-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2019-10-11 23:09:48.000000 trytond_purchase_requisition-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    26432 2022-10-11 19:49:58.000000 trytond_purchase_requisition-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16169 2021-04-27 07:34:40.000000 trytond_purchase_requisition-6.6.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:16:20.368075 trytond_purchase_requisition-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5299 2022-10-29 07:39:11.000000 trytond_purchase_requisition-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:20.364742 trytond_purchase_requisition-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_purchase_requisition-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11566 2021-04-03 16:26:38.000000 trytond_purchase_requisition-6.6.0/tests/scenario_purchase_requisition.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2022-04-16 16:30:57.000000 trytond_purchase_requisition-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_purchase_requisition-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2022-10-31 15:10:09.000000 trytond_purchase_requisition-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-10-31 16:16:17.000000 trytond_purchase_requisition-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:20.364742 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3596 2022-10-31 16:16:19.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1978 2022-10-31 16:16:20.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:16:19.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2022-10-31 16:16:19.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:54.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2022-10-31 16:16:19.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:16:19.000000 trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:16:20.364742 trytond_purchase_requisition-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2019-02-13 10:09:38.000000 trytond_purchase_requisition-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1837 2021-10-07 13:08:07.000000 trytond_purchase_requisition-6.6.0/view/purchase_requisition_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2021-10-07 13:08:07.000000 trytond_purchase_requisition-6.6.0/view/purchase_requisition_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2022-04-08 16:23:26.000000 trytond_purchase_requisition-6.6.0/view/purchase_requisition_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2022-04-08 16:23:26.000000 trytond_purchase_requisition-6.6.0/view/purchase_requisition_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2022-04-08 16:23:26.000000 trytond_purchase_requisition-6.6.0/view/purchase_requisition_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:13.847703 trytond_purchase_requisition-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-05-01 11:02:56.000000 trytond_purchase_requisition-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-05-01 11:02:56.000000 trytond_purchase_requisition-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_requisition-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3583 2023-05-01 11:44:13.847703 trytond_purchase_requisition-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:13.844370 trytond_purchase_requisition-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:13.841037 trytond_purchase_requisition-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6654 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6796 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6659 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5919 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6424 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7011 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6829 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6008 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6692 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6391 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6720 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6556 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6740 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5881 2023-04-30 10:46:36.000000 trytond_purchase_requisition-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6630 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5759 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-04-29 08:02:41.000000 trytond_purchase_requisition-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    26524 2023-04-21 08:36:08.000000 trytond_purchase_requisition-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16169 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:44:13.847703 trytond_purchase_requisition-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4483 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:13.841037 trytond_purchase_requisition-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11510 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/tests/scenario_purchase_requisition.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-05-01 11:02:50.000000 trytond_purchase_requisition-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:13.847703 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3583 2023-05-01 11:44:12.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1952 2023-05-01 11:44:13.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:44:12.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-05-01 11:44:12.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2023-05-01 11:44:12.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:44:12.000000 trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:13.844370 trytond_purchase_requisition-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:21.000000 trytond_purchase_requisition-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1837 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/view/purchase_requisition_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/view/purchase_requisition_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/view/purchase_requisition_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/view/purchase_requisition_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-15 07:12:15.000000 trytond_purchase_requisition-6.8.0/view/purchase_requisition_tree.xml
```

### Comparing `trytond_purchase_requisition-6.6.0/CHANGELOG` & `trytond_purchase_requisition-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_purchase_requisition-6.6.0/COPYRIGHT` & `trytond_purchase_requisition-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/LICENSE` & `trytond_purchase_requisition-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/PKG-INFO` & `trytond_purchase_requisition-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_requisition
-Version: 6.6.0
+Version: 6.8.0
 Summary: Allows users to enter requests for product supply (requisition). This will create a "Purchase request" by line which will be treated by the purchasing department.
 Home-page: http://www.tryton.org
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_requisition
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase requisition
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
 
 Purchase Requisition Module
 ###########################
 
 The Purchase Requisition module allows users to create their purchase
```

### Comparing `trytond_purchase_requisition-6.6.0/README.rst` & `trytond_purchase_requisition-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/__init__.py` & `trytond_purchase_requisition-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/doc/index.rst` & `trytond_purchase_requisition-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/bg.po` & `trytond_purchase_requisition-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/ca.po` & `trytond_purchase_requisition-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/cs.po` & `trytond_purchase_requisition-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/de.po` & `trytond_purchase_requisition-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/es.po` & `trytond_purchase_requisition-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/es_419.po` & `trytond_purchase_requisition-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/et.po` & `trytond_purchase_requisition-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/fa.po` & `trytond_purchase_requisition-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/fi.po` & `trytond_purchase_requisition-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/fr.po` & `trytond_purchase_requisition-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/hu.po` & `trytond_purchase_requisition-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/id.po` & `trytond_purchase_requisition-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/it.po` & `trytond_purchase_requisition-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/lo.po` & `trytond_purchase_requisition-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/lt.po` & `trytond_purchase_requisition-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/nl.po` & `trytond_purchase_requisition-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/pl.po` & `trytond_purchase_requisition-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/pt.po` & `trytond_purchase_requisition-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/ro.po` & `trytond_purchase_requisition-6.8.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 msgctxt "field:purchase.requisition,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:purchase.requisition,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valută"
 
 msgctxt "field:purchase.requisition,description:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:purchase.requisition,employee:"
 msgid "Employee"
```

### Comparing `trytond_purchase_requisition-6.6.0/locale/ru.po` & `trytond_purchase_requisition-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/sl.po` & `trytond_purchase_requisition-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/tr.po` & `trytond_purchase_requisition-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/uk.po` & `trytond_purchase_requisition-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/locale/zh_CN.po` & `trytond_purchase_requisition-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/message.xml` & `trytond_purchase_requisition-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/purchase.py` & `trytond_purchase_requisition-6.8.0/purchase.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,18 @@
         'purchase.requisition', 'Requisition',
         ondelete='CASCADE', required=True)
     supplier = fields.Many2One('party.party', 'Supplier', states=_states)
     product = fields.Many2One(
         'product.product', 'Product',
         ondelete='RESTRICT',
         domain=[
-            ('purchasable', '=', True),
+            If((Eval('purchase_requisition_state') == 'draft')
+                & ~(Eval('quantity', 0) < 0),
+                ('purchasable', '=', True),
+                ()),
             ],
         states=_states)
     product_uom_category = fields.Function(
         fields.Many2One('product.uom.category', "Product UOM Category"),
         'on_change_with_product_uom_category')
     description = fields.Text("Description", states=_states)
     summary = fields.Function(fields.Char('Summary'), 'on_change_with_summary')
@@ -489,21 +492,19 @@
 
     @classmethod
     def _unit_categories(cls):
         return ['product_uom_category']
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @fields.depends('requisition', '_parent_requisition.currency')
     def on_change_with_currency(self, name=None):
-        if self.requisition and self.requisition.currency:
-            return self.requisition.currency.id
+        return self.requisition.currency if self.requisition else None
 
     @classmethod
     def get_purchase_requisition_states(cls):
         pool = Pool()
         Requisition = pool.get('purchase.requisition')
         return Requisition.fields_get(['state'])['state']['selection']
```

### Comparing `trytond_purchase_requisition-6.6.0/purchase.xml` & `trytond_purchase_requisition-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/setup.py` & `trytond_purchase_requisition-6.8.0/setup.py`

 * *Files 14% similar despite different names*

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
@@ -34,62 +31,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_purchase_requisition'
 
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
     description=('Allows users to enter requests for product supply '
         '(requisition). This will create a "Purchase request" by line '
         'which will be treated by the purchasing department.'),
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/purchase_requisition',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton purchase requisition',
     package_dir={'trytond.modules.purchase_requisition': '.'},
     packages=(
         ['trytond.modules.purchase_requisition']
         + ['trytond.modules.purchase_requisition.%s' % p
             for p in find_packages()]
@@ -125,27 +103,26 @@
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
     purchase_requisition = trytond.modules.purchase_requisition
     """,
     )
```

### Comparing `trytond_purchase_requisition-6.6.0/tests/scenario_purchase_requisition.rst` & `trytond_purchase_requisition-6.8.0/tests/scenario_purchase_requisition.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 =============================
 Purchase Requisition Scenario
 =============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import (create_company,
     ...     get_company)
     >>> from trytond.modules.account.tests.tools import (create_chart,
     ...     get_accounts)
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate purchase_requisition Module::
 
     >>> config = activate_modules(['purchase_requisition'])
 
 Create company::
```

### Comparing `trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/PKG-INFO` & `trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-purchase-requisition
-Version: 6.6.0
+Version: 6.8.0
 Summary: Allows users to enter requests for product supply (requisition). This will create a "Purchase request" by line which will be treated by the purchasing department.
 Home-page: http://www.tryton.org
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/purchase_requisition
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton purchase requisition
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
 
 Purchase Requisition Module
 ###########################
 
 The Purchase Requisition module allows users to create their purchase
```

### Comparing `trytond_purchase_requisition-6.6.0/trytond_purchase_requisition.egg-info/SOURCES.txt` & `trytond_purchase_requisition-6.8.0/trytond_purchase_requisition.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
 message.xml
@@ -49,14 +45,15 @@
 ./tests/test_scenario.py
 ./view/configuration_form.xml
 ./view/purchase_requisition_form.xml
 ./view/purchase_requisition_line_form.xml
 ./view/purchase_requisition_line_list.xml
 ./view/purchase_requisition_line_list_sequence.xml
 ./view/purchase_requisition_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_purchase_requisition-6.6.0/view/purchase_requisition_form.xml` & `trytond_purchase_requisition-6.8.0/view/purchase_requisition_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_requisition-6.6.0/view/purchase_requisition_line_form.xml` & `trytond_purchase_requisition-6.8.0/view/purchase_requisition_line_form.xml`

 * *Files identical despite different names*

