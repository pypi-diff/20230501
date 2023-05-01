# Comparing `tmp/trytond_project_plan-6.6.0.tar.gz` & `tmp/trytond_project_plan-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_plan-6.6.0.tar", last modified: Mon Oct 31 16:00:00 2022, max compression
+gzip compressed data, was "trytond_project_plan-6.8.0.tar", last modified: Mon May  1 11:40:03 2023, max compression
```

## Comparing `trytond_project_plan-6.6.0.tar` & `trytond_project_plan-6.8.0.tar`

### file list

```diff
@@ -1,62 +1,59 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:00.723832 trytond_project_plan-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_project_plan-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_project_plan-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2022-10-31 15:59:58.000000 trytond_project_plan-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_project_plan-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2022-10-31 15:59:57.000000 trytond_project_plan-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:59:57.000000 trytond_project_plan-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:37.000000 trytond_project_plan-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_project_plan-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3424 2022-10-31 16:00:00.723832 trytond_project_plan-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2019-10-11 23:09:48.000000 trytond_project_plan-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2021-12-11 16:59:33.000000 trytond_project_plan-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2107 2022-10-11 19:49:58.000000 trytond_project_plan-6.6.0/allocation.py
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2019-02-13 10:09:37.000000 trytond_project_plan-6.6.0/allocation.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:00.717165 trytond_project_plan-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2019-10-11 23:09:48.000000 trytond_project_plan-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:00.713832 trytond_project_plan-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3766 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3187 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3121 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3203 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2743 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3339 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2706 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2629 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2772 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3128 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2750 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3212 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3603 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3112 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3001 2022-10-29 07:50:33.000000 trytond_project_plan-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:00:00.723832 trytond_project_plan-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5032 2022-10-29 07:39:11.000000 trytond_project_plan-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:00.717165 trytond_project_plan-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_project_plan-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2022-04-16 16:30:57.000000 trytond_project_plan-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2022-10-31 15:10:09.000000 trytond_project_plan-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2022-10-31 15:59:56.000000 trytond_project_plan-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:00.720498 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3424 2022-10-31 15:59:59.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2022-10-31 16:00:00.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:59:59.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2022-10-31 15:59:59.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:51.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2022-10-31 15:59:59.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:59:59.000000 trytond_project_plan-6.6.0/trytond_project_plan.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:00.717165 trytond_project_plan-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2019-02-13 10:09:37.000000 trytond_project_plan-6.6.0/view/allocation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2019-02-13 10:09:37.000000 trytond_project_plan-6.6.0/view/allocation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2019-06-04 16:49:45.000000 trytond_project_plan-6.6.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22865 2022-10-11 19:49:58.000000 trytond_project_plan-6.6.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)      965 2019-02-13 10:09:37.000000 trytond_project_plan-6.6.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:03.811267 trytond_project_plan-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2253 2023-05-01 11:00:10.000000 trytond_project_plan-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:00:10.000000 trytond_project_plan-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3419 2023-05-01 11:40:03.811267 trytond_project_plan-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2107 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/allocation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/allocation.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:03.807934 trytond_project_plan-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:03.804600 trytond_project_plan-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3766 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3187 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3140 2023-04-30 10:46:36.000000 trytond_project_plan-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3203 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2743 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3339 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2706 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2629 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2772 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3128 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2750 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3212 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3603 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3112 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3001 2023-04-29 08:02:40.000000 trytond_project_plan-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:40:03.811267 trytond_project_plan-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4223 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:03.804600 trytond_project_plan-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2023-05-01 11:00:04.000000 trytond_project_plan-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:03.807934 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3419 2023-05-01 11:40:02.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1464 2023-05-01 11:40:03.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:40:02.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2023-05-01 11:40:02.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-05-01 11:40:02.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:40:02.000000 trytond_project_plan-6.8.0/trytond_project_plan.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:03.807934 trytond_project_plan-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/view/allocation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/view/allocation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22865 2023-04-15 07:12:15.000000 trytond_project_plan-6.8.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      965 2023-01-16 14:00:21.000000 trytond_project_plan-6.8.0/work.xml
```

### Comparing `trytond_project_plan-6.6.0/CHANGELOG` & `trytond_project_plan-6.8.0/CHANGELOG`

 * *Files 13% similar despite different names*

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

### Comparing `trytond_project_plan-6.6.0/COPYRIGHT` & `trytond_project_plan-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2009-2013 Bertrand Chenal.
-Copyright (C) 2009-2022 Cédric Krier.
-Copyright (C) 2009-2022 B2CK SPRL.
+Copyright (C) 2009-2023 Cédric Krier.
+Copyright (C) 2009-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_project_plan-6.6.0/LICENSE` & `trytond_project_plan-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/PKG-INFO` & `trytond_project_plan-6.8.0/trytond_project_plan.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_project_plan
-Version: 6.6.0
+Name: trytond-project-plan
+Version: 6.8.0
 Summary: Tryton module to add planning capabilities on projects
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
-Project-URL: Source Code, https://hg.tryton.org/modules/project_plan
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project planning
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
 
 Project Plan Module
 ###################
 
 The Project Plan module adds planning features on top of the Project
 module.
```

### Comparing `trytond_project_plan-6.6.0/README.rst` & `trytond_project_plan-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/allocation.py` & `trytond_project_plan-6.8.0/allocation.py`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/allocation.xml` & `trytond_project_plan-6.8.0/allocation.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/doc/index.rst` & `trytond_project_plan-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/bg.po` & `trytond_project_plan-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/ca.po` & `trytond_project_plan-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/cs.po` & `trytond_project_plan-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/de.po` & `trytond_project_plan-6.8.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 msgctxt "field:project.allocation,percentage:"
 msgid "Percentage"
 msgstr "Prozentsatz"
 
 msgctxt "field:project.allocation,work:"
 msgid "Work"
-msgstr "Tätigkeit"
+msgstr "Projektaufgabe"
 
 msgctxt "field:project.predecessor_successor,predecessor:"
 msgid "Predecessor"
 msgstr "Vorgänger"
 
 msgctxt "field:project.predecessor_successor,successor:"
 msgid "Successor"
@@ -60,15 +60,15 @@
 
 msgctxt "field:project.work,constraint_start_time:"
 msgid "Constraint Start Time"
 msgstr "Fixe Startzeit"
 
 msgctxt "field:project.work,duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:project.work,early_finish_date:"
 msgid "Early Finish"
 msgstr "Frühestes Enddatum"
 
 msgctxt "field:project.work,early_finish_time:"
 msgid "Early Finish Time"
@@ -108,15 +108,15 @@
 
 msgctxt "field:project.work,successors:"
 msgid "Successors"
 msgstr "Nachfolger"
 
 msgctxt "model:ir.action,name:wizard_leveling"
 msgid "Tasks Leveling"
-msgstr "Aufgaben abgleichen"
+msgstr "Projektaufgaben abgleichen"
 
 msgctxt "model:project.allocation,name:"
 msgid "Allocation"
 msgstr "Zuordnung"
 
 msgctxt "model:project.predecessor_successor,name:"
 msgid "Predecessor - Successor"
```

### Comparing `trytond_project_plan-6.6.0/locale/es.po` & `trytond_project_plan-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/es_419.po` & `trytond_project_plan-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/et.po` & `trytond_project_plan-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/fa.po` & `trytond_project_plan-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/fi.po` & `trytond_project_plan-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/fr.po` & `trytond_project_plan-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/hu.po` & `trytond_project_plan-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/id.po` & `trytond_project_plan-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/it.po` & `trytond_project_plan-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/lo.po` & `trytond_project_plan-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/lt.po` & `trytond_project_plan-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/nl.po` & `trytond_project_plan-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/pl.po` & `trytond_project_plan-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/pt.po` & `trytond_project_plan-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/ro.po` & `trytond_project_plan-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/ru.po` & `trytond_project_plan-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/sl.po` & `trytond_project_plan-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/tr.po` & `trytond_project_plan-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/uk.po` & `trytond_project_plan-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/locale/zh_CN.po` & `trytond_project_plan-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/setup.py` & `trytond_project_plan-6.8.0/setup.py`

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
@@ -34,59 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_project_plan'
 
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
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module to add planning capabilities on projects',
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
-        "Source Code": 'https://hg.tryton.org/modules/project_plan',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton project planning',
     package_dir={'trytond.modules.project_plan': '.'},
     packages=(
         ['trytond.modules.project_plan']
         + ['trytond.modules.project_plan.%s' % p for p in find_packages()]
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
     project_plan = trytond.modules.project_plan
     """,
     )
```

### Comparing `trytond_project_plan-6.6.0/trytond_project_plan.egg-info/PKG-INFO` & `trytond_project_plan-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-project-plan
-Version: 6.6.0
+Name: trytond_project_plan
+Version: 6.8.0
 Summary: Tryton module to add planning capabilities on projects
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
-Project-URL: Source Code, https://hg.tryton.org/modules/project_plan
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project planning
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
 
 Project Plan Module
 ###################
 
 The Project Plan module adds planning features on top of the Project
 module.
```

### Comparing `trytond_project_plan-6.6.0/trytond_project_plan.egg-info/SOURCES.txt` & `trytond_project_plan-6.8.0/trytond_project_plan.egg-info/SOURCES.txt`

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
 allocation.py
@@ -46,14 +42,15 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/allocation_form.xml
 ./view/allocation_tree.xml
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

### Comparing `trytond_project_plan-6.6.0/view/work_form.xml` & `trytond_project_plan-6.8.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/work.py` & `trytond_project_plan-6.8.0/work.py`

 * *Files identical despite different names*

### Comparing `trytond_project_plan-6.6.0/work.xml` & `trytond_project_plan-6.8.0/work.xml`

 * *Files identical despite different names*

