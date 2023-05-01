# Comparing `tmp/trytond_project-6.6.0.tar.gz` & `tmp/trytond_project-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project-6.6.0.tar", last modified: Mon Oct 31 15:56:58 2022, max compression
+gzip compressed data, was "trytond_project-6.8.0.tar", last modified: Mon May  1 11:50:52 2023, max compression
```

## Comparing `trytond_project-6.6.0.tar` & `trytond_project-6.8.0.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.227845 trytond_project-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:02.000000 trytond_project-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_project-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-10-31 15:56:56.000000 trytond_project-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_project-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     3244 2022-10-31 15:56:56.000000 trytond_project-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:56:55.000000 trytond_project-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:52.000000 trytond_project-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_project-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2406 2022-10-31 15:56:58.227845 trytond_project-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2022-10-27 11:24:44.000000 trytond_project-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2021-12-11 16:59:33.000000 trytond_project-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.224512 trytond_project-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-10-07 13:08:06.000000 trytond_project-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3201 2022-10-17 07:22:05.000000 trytond_project-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2022-10-27 11:24:44.000000 trytond_project-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_project-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2021-10-07 13:08:06.000000 trytond_project-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2020-01-28 10:46:04.000000 trytond_project-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.224512 trytond_project-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:38.000000 trytond_project-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2019-06-04 16:49:45.000000 trytond_project-6.6.0/icons/tryton-project.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2020-12-04 09:17:30.000000 trytond_project-6.6.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.221178 trytond_project-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7030 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7344 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6073 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7651 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7328 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6144 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6341 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6047 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7386 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6313 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5869 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6241 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6580 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6122 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7287 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6289 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7010 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5840 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7286 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6624 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6061 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5865 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6959 2022-10-29 07:50:39.000000 trytond_project-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2020-01-28 10:46:04.000000 trytond_project-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2021-12-11 16:59:33.000000 trytond_project-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1458 2022-04-08 16:27:20.000000 trytond_project-6.6.0/project.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:56:58.227845 trytond_project-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5281 2022-10-29 07:39:11.000000 trytond_project-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.221178 trytond_project-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_project-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2201 2020-04-30 22:22:16.000000 trytond_project-6.6.0/tests/scenario_project_status.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7386 2022-06-17 09:17:27.000000 trytond_project-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_project-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1288 2021-12-11 16:59:33.000000 trytond_project-6.6.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1117 2019-06-04 16:49:45.000000 trytond_project-6.6.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2022-10-31 15:10:09.000000 trytond_project-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2022-10-31 15:56:54.000000 trytond_project-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.224512 trytond_project-6.6.0/trytond_project.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2406 2022-10-31 15:56:57.000000 trytond_project-6.6.0/trytond_project.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2059 2022-10-31 15:56:58.000000 trytond_project-6.6.0/trytond_project.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:56:57.000000 trytond_project-6.6.0/trytond_project.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2022-10-31 15:56:57.000000 trytond_project-6.6.0/trytond_project.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:00.000000 trytond_project-6.6.0/trytond_project.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2022-10-31 15:56:57.000000 trytond_project-6.6.0/trytond_project.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:56:57.000000 trytond_project-6.6.0/trytond_project.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:56:58.224512 trytond_project-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     2346 2020-01-28 10:46:04.000000 trytond_project-6.6.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2022-04-08 16:23:26.000000 trytond_project-6.6.0/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2022-04-08 16:23:26.000000 trytond_project-6.6.0/view/work_list_children.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-04-08 16:23:26.000000 trytond_project-6.6.0/view/work_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2020-01-28 10:46:04.000000 trytond_project-6.6.0/view/work_status_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-08 16:23:26.000000 trytond_project-6.6.0/view/work_status_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2022-04-08 16:23:26.000000 trytond_project-6.6.0/view/work_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2022-04-08 16:23:26.000000 trytond_project-6.6.0/view/work_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20283 2022-10-11 19:49:58.000000 trytond_project-6.6.0/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12059 2021-04-27 07:34:40.000000 trytond_project-6.6.0/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.435983 trytond_project-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3407 2023-05-01 11:07:14.000000 trytond_project-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:07:13.000000 trytond_project-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2406 2023-05-01 11:50:52.435983 trytond_project-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_project-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.432650 trytond_project-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_project-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3201 2023-04-15 07:12:15.000000 trytond_project-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-04-15 07:12:15.000000 trytond_project-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_project-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-15 07:12:15.000000 trytond_project-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_project-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.432650 trytond_project-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_project-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-01-16 14:00:21.000000 trytond_project-6.8.0/icons/tryton-project.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_project-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.429316 trytond_project-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7126 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7477 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6169 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7909 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7467 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6240 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6437 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7513 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6143 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7522 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6409 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5965 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6337 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6676 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6218 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7426 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6385 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7106 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5936 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7382 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6720 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6157 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5961 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7055 2023-04-30 10:46:36.000000 trytond_project-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_project-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-04-15 07:12:15.000000 trytond_project-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-04-15 07:12:15.000000 trytond_project-6.8.0/project.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:50:52.435983 trytond_project-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4478 2023-04-15 07:12:15.000000 trytond_project-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.429316 trytond_project-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2201 2023-04-15 07:12:15.000000 trytond_project-6.8.0/tests/scenario_project_status.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7386 2023-04-15 07:12:15.000000 trytond_project-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1288 2023-04-15 07:12:15.000000 trytond_project-6.8.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1117 2023-04-15 07:12:15.000000 trytond_project-6.8.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_project-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-05-01 11:07:08.000000 trytond_project-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.435983 trytond_project-6.8.0/trytond_project.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2406 2023-05-01 11:50:51.000000 trytond_project-6.8.0/trytond_project.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2021 2023-05-01 11:50:52.000000 trytond_project-6.8.0/trytond_project.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:50:51.000000 trytond_project-6.8.0/trytond_project.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 11:50:51.000000 trytond_project-6.8.0/trytond_project.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_project-6.8.0/trytond_project.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-05-01 11:50:51.000000 trytond_project-6.8.0/trytond_project.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:50:51.000000 trytond_project-6.8.0/trytond_project.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:50:52.429316 trytond_project-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2346 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_list_children.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_status_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_status_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_project-6.8.0/view/work_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20486 2023-04-15 07:12:15.000000 trytond_project-6.8.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12059 2023-04-15 07:12:15.000000 trytond_project-6.8.0/work.xml
```

### Comparing `trytond_project-6.6.0/CHANGELOG` & `trytond_project-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_project-6.6.0/LICENSE` & `trytond_project-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/PKG-INFO` & `trytond_project-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_project
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with projects
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-project/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/project
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project
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
 
 ##############
 Project Module
 ##############
```

### Comparing `trytond_project-6.6.0/__init__.py` & `trytond_project-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/doc/conf.py` & `trytond_project-6.8.0/doc/conf.py`

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

### Comparing `trytond_project-6.6.0/doc/design.rst` & `trytond_project-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/doc/usage.rst` & `trytond_project-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/icons/LICENSE` & `trytond_project-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/ir.py` & `trytond_project-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/locale/bg.po` & `trytond_project-6.8.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 msgstr "Предполагаеми общо усилия за тази задача и подзадачите"
 
 #, fuzzy
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Предполагаеми общо усилия за тази задача и подзадачите"
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Предполагаеми общо усилия за тази задача и подзадачите"
 
 #, fuzzy
 msgctxt "help:project.work,total_effort:"
```

### Comparing `trytond_project-6.6.0/locale/ca.po` & `trytond_project-6.8.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr "Esforç estimat per aquest treball."
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Progrés estimat per aquest treball."
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr "Marqueu per registrar temps invertit."
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Temps total dedicat en aquest treball i els seus subtreballs."
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr "Esforç total estimat per aquest treball i els seus subtreballs."
```

### Comparing `trytond_project-6.6.0/locale/cs.po` & `trytond_project-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:project.work,effort_duration:"
 msgid "Effort"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:project.work,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:project.work,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:project.work,party:"
 msgid "Party"
@@ -83,18 +82,17 @@
 msgid "Count"
 msgstr ""
 
 msgctxt "field:project.work.status,default:"
 msgid "Default"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:project.work.status,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:project.work.status,progress:"
 msgid "Progress"
 msgstr ""
 
 msgctxt "field:project.work.status,types:"
 msgid "Types"
@@ -104,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/de.po` & `trytond_project-6.8.0/locale/de.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,children:"
 msgid "Children"
-msgstr "Untergeordnet (Projekte/Aufgaben)"
+msgstr "Untergeordnet (Projekte/Projektaufgaben)"
 
 msgctxt "field:project.work,comment:"
 msgid "Comment"
 msgstr "Kommentar"
 
 msgctxt "field:project.work,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
 msgctxt "field:project.work,effort_duration:"
 msgid "Effort"
-msgstr "Zeitaufwand"
+msgstr "Veranschlagte Zeit"
 
 msgctxt "field:project.work,name:"
 msgid "Name"
 msgstr "Name"
 
 msgctxt "field:project.work,parent:"
 msgid "Parent"
-msgstr "Übergeordnet (Projekt/Aufgabe)"
+msgstr "Übergeordnet (Projekt/Projektaufgabe)"
 
 msgctxt "field:project.work,party:"
 msgid "Party"
 msgstr "Partei"
 
 msgctxt "field:project.work,party_address:"
 msgid "Contact Address"
@@ -48,31 +48,31 @@
 
 msgctxt "field:project.work,timesheet_available:"
 msgid "Available on timesheets"
 msgstr "Verfügbar für Zeiterfassung"
 
 msgctxt "field:project.work,timesheet_duration:"
 msgid "Duration"
-msgstr "Dauer"
+msgstr "Erfasste Zeit"
 
 msgctxt "field:project.work,timesheet_end_date:"
 msgid "Timesheet End"
 msgstr "Zeiterfassung Ende"
 
 msgctxt "field:project.work,timesheet_start_date:"
 msgid "Timesheet Start"
 msgstr "Zeiterfassung Beginn"
 
 msgctxt "field:project.work,timesheet_works:"
 msgid "Timesheet Works"
-msgstr "Tätigkeiten"
+msgstr "Aufgaben"
 
 msgctxt "field:project.work,total_effort:"
 msgid "Total Effort"
-msgstr "Gesamtaufwand (Personenstunden)"
+msgstr "Veranschlagter Gesamtaufwand"
 
 msgctxt "field:project.work,total_progress:"
 msgid "Total Progress"
 msgstr "Gesamtfortschritt"
 
 msgctxt "field:project.work,type:"
 msgid "Type"
@@ -96,40 +96,46 @@
 
 msgctxt "field:project.work.status,types:"
 msgid "Types"
 msgstr "Typen"
 
 msgctxt "help:project.work,effort_duration:"
 msgid "Estimated Effort for this work."
-msgstr "Geschätzter Zeitaufwand für diese Aufgabe."
+msgstr "Geschätzter Zeitaufwand für diese Projektaufgabe."
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
-msgstr "Geschätzter Fortschritt für diese Aufgabe."
+msgstr "Geschätzter Fortschritt für diese Projektaufgabe."
+
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr "Auswählen um Zeiterfassung zu aktivieren."
 
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
-"Die gesamte Zeit, die für diese Aufgabe inkl. Unteraufgaben verwendet wurde."
+"Die gesamte Zeit, die für diese Aufgabe inkl. Unteraufgaben aufgewendet "
+"wurde."
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
-"Veranschlagter Gesamtaufwand für diese(s) Projekt/Aufgabe inkl. aller "
-"untergeordneten Projekte/Aufgaben in Stunden (Format: Personenstunden, "
-"-tage, -wochen)."
+"Geschätzter Zeitaufwand für dieses Projekt oder diese Projektaufgabe "
+"inklusive aller untergeordneten Projekte und Projektaufgaben."
 
 msgctxt "help:project.work,total_progress:"
 msgid "Estimated total progress for this work and the sub-works."
-msgstr "Geschätzter Gesamtfortschritt für diese Aufgabe inkl. Unteraufgaben."
+msgstr ""
+"Geschätzter Gesamtfortschritt für diese Projektaufgabe inkl. Unteraufgaben."
 
 msgctxt "help:project.work.status,count:"
 msgid "Check to show the number of works in this status."
 msgstr ""
-"Auswählen, um die Anzahl der Projekte/Aufgaben mit diesem Status anzuzeigen."
+"Auswählen, um die Anzahl der Projekte/Projektaufgaben mit diesem Status "
+"anzuzeigen."
 
 msgctxt "help:project.work.status,default:"
 msgid "Check to use as default status for the type."
 msgstr "Auswählen, um diesen Status für den Typ als Standard zu verwenden."
 
 msgctxt "help:project.work.status,progress:"
 msgid "The minimum progress required for this status."
@@ -137,43 +143,43 @@
 
 msgctxt "help:project.work.status,types:"
 msgid "The type of works which can use this status."
 msgstr "Die Typen, die diesen Status verwenden können."
 
 msgctxt "model:ir.action,name:act_open_child_work"
 msgid "Tasks"
-msgstr "Aufgaben"
+msgstr "Projektaufgabe"
 
 msgctxt "model:ir.action,name:act_project_form"
 msgid "Projects"
 msgstr "Projekte"
 
 msgctxt "model:ir.action,name:act_project_tree"
 msgid "Projects"
 msgstr "Projekte"
 
 msgctxt "model:ir.action,name:act_task_form"
 msgid "Tasks"
-msgstr "Aufgaben"
+msgstr "Projektaufgaben"
 
 msgctxt "model:ir.action,name:act_timesheet_line_form_work"
 msgid "Timesheet Lines"
 msgstr "Zeiterfassungspositionen"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works Efforts"
-msgstr "Aufgaben Aufwände"
+msgstr "Projekte und Projektaufgaben"
 
 msgctxt "model:ir.action,name:act_work_status"
 msgid "Work Status"
-msgstr "Aufgaben Status"
+msgstr "Projektaufgaben Status"
 
 msgctxt "model:ir.action,name:act_work_tree"
 msgid "Works Efforts"
-msgstr "Aufgaben Aufwände"
+msgstr "Projekte und Projektaufgaben"
 
 msgctxt "model:ir.message,text:msg_domain_all"
 msgid "All"
 msgstr "Alle"
 
 msgctxt "model:ir.message,text:msg_erase_party_opened_project"
 msgid ""
@@ -225,31 +231,31 @@
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Auswertungen"
 
 msgctxt "model:ir.ui.menu,name:menu_task_form"
 msgid "Tasks"
-msgstr "Aufgaben"
+msgstr "Projektaufgaben"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works Efforts"
-msgstr "Aufgaben Aufwände"
+msgstr "Projekte und Projektaufgaben"
 
 msgctxt "model:ir.ui.menu,name:menu_work_status"
 msgid "Work Status"
-msgstr "Aufgabenstatus"
+msgstr "Projektaufgabenstatus"
 
 msgctxt "model:ir.ui.menu,name:menu_work_tree"
 msgid "Works Efforts"
-msgstr "Aufgaben Aufwände"
+msgstr "Projekte und Projektaufgaben"
 
 msgctxt "model:project.work,name:"
 msgid "Work Effort"
-msgstr "Aufgabe Aufwand"
+msgstr "Projekt/Projektaufgabe"
 
 msgctxt "model:project.work.status,name:"
 msgid "Work Status"
 msgstr "Projekt Status"
 
 msgctxt "model:project.work.status,name:work_done_status"
 msgid "Done"
@@ -265,15 +271,15 @@
 
 msgctxt "selection:project.work,type:"
 msgid "Project"
 msgstr "Projekt"
 
 msgctxt "selection:project.work,type:"
 msgid "Task"
-msgstr "Aufgabe"
+msgstr "Projektaufgabe"
 
 msgctxt "view:project.work.status:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:project.work:"
 msgid "%"
```

### Comparing `trytond_project-6.6.0/locale/es.po` & `trytond_project-6.8.0/locale/es.po`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr "Esfuerzo estimado para este trabajo."
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Progreso estimado para este trabajo."
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr "Marcar para registrar el tiempo invertido."
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Tiempo total empleado en este trabajo y sus subtrabajos."
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr "Esfuerzo total estimado para este trabajo y sus subtrabajos."
@@ -282,8 +286,8 @@
 
 msgctxt "view:project.work:"
 msgid "Start:"
 msgstr "Inicio:"
 
 msgctxt "view:project.work:"
 msgid "Timesheet:"
-msgstr "Hoja de trabajo:"
+msgstr "Parte de trabajo:"
```

### Comparing `trytond_project-6.6.0/locale/es_419.po` & `trytond_project-6.8.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,18 @@
 msgstr "Esfuerzo total estimado para este trabajo y sus subtrabajos"
 
 #, fuzzy
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Esfuerzo total estimado para este trabajo y sus subtrabajos"
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Esfuerzo total estimado para este trabajo y sus subtrabajos"
 
 #, fuzzy
 msgctxt "help:project.work,total_effort:"
```

### Comparing `trytond_project-6.6.0/locale/et.po` & `trytond_project-6.8.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/fa.po` & `trytond_project-6.8.0/locale/fa.po`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 msgstr "تلاش پیش بینی شده برای این کار"
 
 #, fuzzy
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "پیشرفت پیش بینی شده برای این کار"
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "کل زمان صرف شده در این کار و زیر کارهای آن"
 
 #, fuzzy
 msgctxt "help:project.work,total_effort:"
```

### Comparing `trytond_project-6.6.0/locale/fi.po` & `trytond_project-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,children:"
 msgid "Children"
-msgstr ""
+msgstr "Alt Öge"
 
 msgctxt "field:project.work,comment:"
 msgid "Comment"
-msgstr ""
+msgstr "Açıklama"
 
 msgctxt "field:project.work,company:"
 msgid "Company"
-msgstr ""
+msgstr "Firma"
 
 msgctxt "field:project.work,effort_duration:"
 msgid "Effort"
 msgstr ""
 
 msgctxt "field:project.work,name:"
 msgid "Name"
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
@@ -265,15 +269,14 @@
 msgstr "Tasks"
 
 #, fuzzy
 msgctxt "view:project.work.status:"
 msgid "%"
 msgstr "%"
 
-#, fuzzy
 msgctxt "view:project.work:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:project.work:"
 msgid "End:"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_project-6.6.0/locale/fr.po` & `trytond_project-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr "Effort estimé pour ce travail."
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Progression estimée pour ce travail."
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr "Cochez pour enregistrer le temps passé."
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Temps total passé sur ce travail et ses sous-travaux."
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr "Effort total estimé pour ce travail et ses sous-travaux."
```

### Comparing `trytond_project-6.6.0/locale/hu.po` & `trytond_project-6.8.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/id.po` & `trytond_project-6.8.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/it.po` & `trytond_project-6.8.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/lo.po` & `trytond_project-6.8.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/lt.po` & `trytond_project-6.8.0/locale/lt.po`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/nl.po` & `trytond_project-6.8.0/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr "Geschatte inspanning voor dit werk."
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Geschatte voortgang voor dit werk."
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr "Vink aan om de bestede tijd te registreren."
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Totale tijd besteed aan dit werk en de subwerken."
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr "Geschatte totale inspanning voor dit werk en de subwerken."
```

### Comparing `trytond_project-6.6.0/locale/pl.po` & `trytond_project-6.8.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/pt.po` & `trytond_project-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 msgstr "Esforço estimado para este trabalho"
 
 #, fuzzy
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Esforço estimado para este trabalho"
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Tempo total gasto nesta tarefa e nas sub-tarefas"
 
 #, fuzzy
 msgctxt "help:project.work,total_effort:"
```

### Comparing `trytond_project-6.6.0/locale/ro.po` & `trytond_project-6.8.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/ru.po` & `trytond_project-6.8.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
 msgstr "Предположительные общие затраты для этой работы и подчиненных работ"
 
 #, fuzzy
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Предположительные общие затраты для этой работы и подчиненных работ"
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Предположительные общие затраты для этой работы и подчиненных работ"
 
 #, fuzzy
 msgctxt "help:project.work,total_effort:"
```

### Comparing `trytond_project-6.6.0/locale/sl.po` & `trytond_project-6.8.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 msgstr "Ocenjen čas za to nalogo"
 
 #, fuzzy
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "Ocenjen napredek za to nalogo"
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "Skupni čas, porabljen na tej nalogi in podnalogami."
 
 #, fuzzy
 msgctxt "help:project.work,total_effort:"
```

### Comparing `trytond_project-6.6.0/locale/tr.po` & `trytond_project-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:project.work,children:"
 msgid "Children"
-msgstr "Alt Öge"
+msgstr ""
 
 msgctxt "field:project.work,comment:"
 msgid "Comment"
-msgstr "Açıklama"
+msgstr ""
 
 msgctxt "field:project.work,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr ""
 
 msgctxt "field:project.work,effort_duration:"
 msgid "Effort"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:project.work,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:project.work,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:project.work,party:"
 msgid "Party"
@@ -82,17 +83,18 @@
 msgid "Count"
 msgstr ""
 
 msgctxt "field:project.work.status,default:"
 msgid "Default"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:project.work.status,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:project.work.status,progress:"
 msgid "Progress"
 msgstr ""
 
 msgctxt "field:project.work.status,types:"
 msgid "Types"
@@ -102,14 +104,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
@@ -265,14 +271,15 @@
 msgstr "Tasks"
 
 #, fuzzy
 msgctxt "view:project.work.status:"
 msgid "%"
 msgstr "%"
 
+#, fuzzy
 msgctxt "view:project.work:"
 msgid "%"
 msgstr "%"
 
 msgctxt "view:project.work:"
 msgid "End:"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_project-6.6.0/locale/uk.po` & `trytond_project-6.8.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr ""
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr ""
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr ""
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr ""
```

### Comparing `trytond_project-6.6.0/locale/zh_CN.po` & `trytond_project-6.8.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,18 @@
 msgid "Estimated Effort for this work."
 msgstr "这项工作的估计工作量."
 
 msgctxt "help:project.work,progress:"
 msgid "Estimated progress for this work."
 msgstr "这项工作的估计进度."
 
+msgctxt "help:project.work,timesheet_available:"
+msgid "Check to record time spent."
+msgstr ""
+
 msgctxt "help:project.work,timesheet_duration:"
 msgid "Total time spent on this work and the sub-works."
 msgstr "这项工作和其子工作的总投入时间."
 
 msgctxt "help:project.work,total_effort:"
 msgid "Estimated total effort for this work and the sub-works."
 msgstr "这项工作和其子工作的估计总工作量."
```

### Comparing `trytond_project-6.6.0/message.xml` & `trytond_project-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/party.py` & `trytond_project-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/project.xml` & `trytond_project-6.8.0/project.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/setup.py` & `trytond_project-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
@@ -37,60 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_project'
 
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
     description='Tryton module with projects',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-project/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/project',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton project',
     package_dir={'trytond.modules.project': '.'},
     packages=(
         ['trytond.modules.project']
         + ['trytond.modules.project.%s' % p for p in find_packages()]
         ),
@@ -128,27 +106,26 @@
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
     project = trytond.modules.project
     """,
     )
```

### Comparing `trytond_project-6.6.0/tests/scenario_project_status.rst` & `trytond_project-6.8.0/tests/scenario_project_status.rst`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/tests/test_module.py` & `trytond_project-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/timesheet.py` & `trytond_project-6.8.0/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/timesheet.xml` & `trytond_project-6.8.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/trytond_project.egg-info/PKG-INFO` & `trytond_project-6.8.0/trytond_project.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-project
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with projects
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-project/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/project
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton project
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
 
 ##############
 Project Module
 ##############
```

### Comparing `trytond_project-6.6.0/trytond_project.egg-info/SOURCES.txt` & `trytond_project-6.8.0/trytond_project.egg-info/SOURCES.txt`

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
```

### Comparing `trytond_project-6.6.0/view/work_form.xml` & `trytond_project-6.8.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/view/work_list.xml` & `trytond_project-6.8.0/view/work_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/view/work_status_form.xml` & `trytond_project-6.8.0/view/work_status_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/view/work_tree.xml` & `trytond_project-6.8.0/view/work_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_project-6.6.0/work.py` & `trytond_project-6.8.0/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from trytond.cache import Cache
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, fields, sequence_ordered,
     tree)
 from trytond.pool import Pool
-from trytond.pyson import Bool, Eval, If, PYSONEncoder
+from trytond.pyson import Bool, Eval, If, PYSONEncoder, TimeDelta
 from trytond.tools import grouped_slice, reduce_ids
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 from .exceptions import WorkProgressValidationError
 
 
 class WorkStatus(DeactivableMixin, sequence_ordered(), ModelSQL, ModelView):
     'Work Status'
     __name__ = 'project.work.status'
@@ -140,16 +140,17 @@
     party_address = fields.Many2One('party.address', 'Contact Address',
         domain=[('party', '=', Eval('party'))],
         states={
             'invisible': Eval('type') != 'project',
             })
     timesheet_works = fields.One2Many(
         'timesheet.work', 'origin', 'Timesheet Works', readonly=True, size=1)
-    timesheet_available = fields.Function(
-        fields.Boolean('Available on timesheets'),
+    timesheet_available = fields.Function(fields.Boolean(
+            "Available on timesheets",
+            help="Check to record time spent."),
         'get_timesheet_available', setter='set_timesheet_available')
     timesheet_start_date = fields.Function(fields.Date('Timesheet Start',
             states={
                 'invisible': ~Eval('timesheet_available'),
                 }),
         'get_timesheet_date', setter='set_timesheet_date')
     timesheet_end_date = fields.Function(fields.Date('Timesheet End',
@@ -157,15 +158,20 @@
                 'invisible': ~Eval('timesheet_available'),
                 }),
         'get_timesheet_date', setter='set_timesheet_date')
     timesheet_duration = fields.Function(fields.TimeDelta('Duration',
             'company_work_time',
             help="Total time spent on this work and the sub-works."),
         'get_total')
-    effort_duration = fields.TimeDelta('Effort', 'company_work_time',
+    effort_duration = fields.TimeDelta(
+        "Effort", 'company_work_time',
+        domain=['OR',
+            ('effort_duration', '=', None),
+            ('effort_duration', '>=', TimeDelta()),
+            ],
         help="Estimated Effort for this work.")
     total_effort = fields.Function(fields.TimeDelta('Total Effort',
             'company_work_time',
             help="Estimated total effort for this work and the sub-works."),
         'get_total')
     progress = fields.Float('Progress',
         domain=['OR',
@@ -536,15 +542,15 @@
         # Get the timesheet works linked to the project works
         timesheet_works = [
             w for pw in project_works for w in pw.timesheet_works]
 
         super(Work, cls).delete(project_works)
 
         if timesheet_works:
-            with Transaction().set_context(_check_access=False):
+            with without_check_access():
                 TimesheetWork.delete(timesheet_works)
 
     @classmethod
     def search_global(cls, text):
         for record, rec_name, icon in super(Work, cls).search_global(text):
             icon = icon or 'tryton-project'
             yield record, rec_name, icon
```

### Comparing `trytond_project-6.6.0/work.xml` & `trytond_project-6.8.0/work.xml`

 * *Files identical despite different names*

