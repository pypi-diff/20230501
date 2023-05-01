# Comparing `tmp/trytond_project_revenue-6.6.0.tar.gz` & `tmp/trytond_project_revenue-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_revenue-6.6.0.tar", last modified: Mon Oct 31 16:09:19 2022, max compression
+gzip compressed data, was "trytond_project_revenue-6.8.0.tar", last modified: Mon May  1 11:47:26 2023, max compression
```

## Comparing `trytond_project_revenue-6.6.0.tar` & `trytond_project_revenue-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_project_revenue-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_project_revenue-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-10-31 16:09:18.000000 trytond_project_revenue-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_project_revenue-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2258 2022-10-31 16:09:17.000000 trytond_project_revenue-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:09:17.000000 trytond_project_revenue-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:37.000000 trytond_project_revenue-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_project_revenue-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2715 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2020-03-28 12:06:53.000000 trytond_project_revenue-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2021-12-11 16:59:33.000000 trytond_project_revenue-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2020-03-28 12:06:53.000000 trytond_project_revenue-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      888 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      861 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      873 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      863 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      764 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      858 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      995 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      778 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      895 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      740 2022-10-29 07:50:38.000000 trytond_project_revenue-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2022-10-11 19:49:58.000000 trytond_project_revenue-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2019-02-13 10:09:37.000000 trytond_project_revenue-6.6.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:09:19.401955 trytond_project_revenue-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5224 2022-10-29 07:39:11.000000 trytond_project_revenue-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_project_revenue-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3850 2020-07-09 09:37:12.000000 trytond_project_revenue-6.6.0/tests/scenario_project_revenue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2022-04-16 16:30:57.000000 trytond_project_revenue-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_project_revenue-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_project_revenue-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      171 2022-10-31 16:09:16.000000 trytond_project_revenue-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2715 2022-10-31 16:09:18.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1773 2022-10-31 16:09:19.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:09:18.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 16:09:18.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:58.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2022-10-31 16:09:18.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:09:18.000000 trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:09:19.398621 trytond_project_revenue-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2019-06-04 16:49:45.000000 trytond_project_revenue-6.6.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2021-10-07 13:08:06.000000 trytond_project_revenue-6.6.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2019-02-13 10:09:37.000000 trytond_project_revenue-6.6.0/view/work_form_purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2022-04-08 16:23:26.000000 trytond_project_revenue-6.6.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2022-04-08 16:23:26.000000 trytond_project_revenue-6.6.0/view/work_list_children.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2022-04-08 16:23:26.000000 trytond_project_revenue-6.6.0/view/work_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8218 2022-06-17 09:17:28.000000 trytond_project_revenue-6.6.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1512 2019-02-13 10:09:37.000000 trytond_project_revenue-6.6.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:26.960100 trytond_project_revenue-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-05-01 11:05:00.000000 trytond_project_revenue-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:05:00.000000 trytond_project_revenue-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_revenue-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2707 2023-05-01 11:47:26.960100 trytond_project_revenue-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:26.956766 trytond_project_revenue-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:26.953433 trytond_project_revenue-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      888 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      861 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-30 10:46:36.000000 trytond_project_revenue-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      863 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      764 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      858 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      995 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      778 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      824 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      740 2023-04-29 08:02:44.000000 trytond_project_revenue-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:21.000000 trytond_project_revenue-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:47:26.960100 trytond_project_revenue-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4413 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:26.953433 trytond_project_revenue-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3850 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/tests/scenario_project_revenue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      171 2023-05-01 11:04:55.000000 trytond_project_revenue-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:26.960100 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2707 2023-05-01 11:47:26.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1747 2023-05-01 11:47:26.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:47:26.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:47:26.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-05-01 11:47:26.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:47:26.000000 trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:47:26.956766 trytond_project_revenue-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-01-16 14:00:21.000000 trytond_project_revenue-6.8.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-01-16 14:00:21.000000 trytond_project_revenue-6.8.0/view/work_form_purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/view/work_list_children.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_project_revenue-6.8.0/view/work_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8212 2023-04-21 08:36:08.000000 trytond_project_revenue-6.8.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1512 2023-01-16 14:00:21.000000 trytond_project_revenue-6.8.0/work.xml
```

### Comparing `trytond_project_revenue-6.6.0/CHANGELOG` & `trytond_project_revenue-6.8.0/CHANGELOG`

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

### Comparing `trytond_project_revenue-6.6.0/LICENSE` & `trytond_project_revenue-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/PKG-INFO` & `trytond_project_revenue-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_project_revenue
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add revenue on project
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
-Project-URL: Source Code, https://hg.tryton.org/modules/project_revenue
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project revenue
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
 
 Project Revenue Module
 ######################
 
 The project revenue module computes revenue and cost per task and project.
```

### Comparing `trytond_project_revenue-6.6.0/locale/bg.po` & `trytond_project_revenue-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/ca.po` & `trytond_project_revenue-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/cs.po` & `trytond_project_revenue-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/de.po` & `trytond_project_revenue-6.8.0/locale/fa.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,cost:"
 msgid "Cost"
-msgstr "Kosten"
+msgstr "هزینه"
 
+#, fuzzy
 msgctxt "field:project.work,currency:"
 msgid "Currency"
-msgstr "Währung"
+msgstr "رقم های واحد پول"
 
 msgctxt "field:project.work,list_price:"
 msgid "List Price"
-msgstr "Listenpreis"
+msgstr "لیست قیمت"
 
 msgctxt "field:project.work,product:"
 msgid "Product"
-msgstr "Artikel"
+msgstr "محصول"
 
 msgctxt "field:project.work,purchase_lines:"
 msgid "Purchase Lines"
-msgstr "Einkaufspositionen"
+msgstr "خطوط خرید"
 
 msgctxt "field:project.work,revenue:"
 msgid "Revenue"
-msgstr "Ertrag"
+msgstr "درآمد"
 
 msgctxt "field:purchase.line,work:"
 msgid "Work Effort"
-msgstr "Aufgabe Aufwand"
+msgstr "تلاش کار"
 
 msgctxt "help:purchase.line,work:"
 msgid "Add to the cost of the work effort."
-msgstr "Zu den Kosten des Arbeitsaufwands hinzufügen."
+msgstr "اضافه کردن هزینه تلاش کار."
 
 msgctxt "view:project.work:"
 msgid "Purchases"
-msgstr "Einkäufe"
+msgstr "خریدها"
 
 msgctxt "view:purchase.line:"
 msgid "Project"
-msgstr "Projekt"
+msgstr "پروژه"
```

### Comparing `trytond_project_revenue-6.6.0/locale/es.po` & `trytond_project_revenue-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/es_419.po` & `trytond_project_revenue-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/et.po` & `trytond_project_revenue-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/fa.po` & `trytond_project_revenue-6.8.0/locale/fi.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,cost:"
 msgid "Cost"
-msgstr "هزینه"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:project.work,currency:"
 msgid "Currency"
-msgstr "رقم های واحد پول"
+msgstr ""
 
 msgctxt "field:project.work,list_price:"
 msgid "List Price"
-msgstr "لیست قیمت"
+msgstr ""
 
 msgctxt "field:project.work,product:"
 msgid "Product"
-msgstr "محصول"
+msgstr ""
 
 msgctxt "field:project.work,purchase_lines:"
 msgid "Purchase Lines"
-msgstr "خطوط خرید"
+msgstr ""
 
 msgctxt "field:project.work,revenue:"
 msgid "Revenue"
-msgstr "درآمد"
+msgstr ""
 
 msgctxt "field:purchase.line,work:"
 msgid "Work Effort"
-msgstr "تلاش کار"
+msgstr ""
 
 msgctxt "help:purchase.line,work:"
 msgid "Add to the cost of the work effort."
-msgstr "اضافه کردن هزینه تلاش کار."
+msgstr ""
 
 msgctxt "view:project.work:"
 msgid "Purchases"
-msgstr "خریدها"
+msgstr ""
 
 msgctxt "view:purchase.line:"
 msgid "Project"
-msgstr "پروژه"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_project_revenue-6.6.0/locale/fi.po` & `trytond_project_revenue-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/fr.po` & `trytond_project_revenue-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/hu.po` & `trytond_project_revenue-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/id.po` & `trytond_project_revenue-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/it.po` & `trytond_project_revenue-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/lo.po` & `trytond_project_revenue-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/lt.po` & `trytond_project_revenue-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/nl.po` & `trytond_project_revenue-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/pl.po` & `trytond_project_revenue-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/pt.po` & `trytond_project_revenue-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/ro.po` & `trytond_project_revenue-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/ru.po` & `trytond_project_revenue-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/sl.po` & `trytond_project_revenue-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/tr.po` & `trytond_project_revenue-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/locale/uk.po` & `trytond_project_revenue-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/purchase.py` & `trytond_project_revenue-6.8.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/setup.py` & `trytond_project_revenue-6.8.0/setup.py`

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
@@ -34,61 +31,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_project_revenue'
 
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
 
 tests_require = [get_require_version('proteus'),
     get_require_version('trytond_purchase')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add revenue on project',
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
-        "Source Code": 'https://hg.tryton.org/modules/project_revenue',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton project revenue',
     package_dir={'trytond.modules.project_revenue': '.'},
     packages=(
         ['trytond.modules.project_revenue']
         + ['trytond.modules.project_revenue.%s' % p for p in find_packages()]
         ),
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
     project_revenue = trytond.modules.project_revenue
     """,
     )
```

### Comparing `trytond_project_revenue-6.6.0/tests/scenario_project_revenue.rst` & `trytond_project_revenue-6.8.0/tests/scenario_project_revenue.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/PKG-INFO` & `trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-project-revenue
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add revenue on project
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
-Project-URL: Source Code, https://hg.tryton.org/modules/project_revenue
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project revenue
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
 
 Project Revenue Module
 ######################
 
 The project revenue module computes revenue and cost per task and project.
```

### Comparing `trytond_project_revenue-6.6.0/trytond_project_revenue.egg-info/SOURCES.txt` & `trytond_project_revenue-6.8.0/trytond_project_revenue.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
 purchase.py
@@ -51,14 +47,15 @@
 ./tests/test_scenario.py
 ./view/purchase_line_form.xml
 ./view/work_form.xml
 ./view/work_form_purchase.xml
 ./view/work_list.xml
 ./view/work_list_children.xml
 ./view/work_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_project_revenue-6.6.0/view/work_form.xml` & `trytond_project_revenue-6.8.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_revenue-6.6.0/work.py` & `trytond_project_revenue-6.8.0/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,15 @@
             else:
                 revenue = work.list_price
             revenues[work.id] = work.company.currency.round(revenue)
         return revenues
 
     @fields.depends('company')
     def on_change_with_currency(self, name=None):
-        if self.company:
-            return self.company.currency.id
+        return self.company.currency if self.company else None
 
     @fields.depends('product', 'company')
     def on_change_product(self):
         pool = Pool()
         User = pool.get('res.user')
         ModelData = pool.get('ir.model.data')
         Uom = pool.get('product.uom')
```

### Comparing `trytond_project_revenue-6.6.0/work.xml` & `trytond_project_revenue-6.8.0/work.xml`

 * *Files identical despite different names*

