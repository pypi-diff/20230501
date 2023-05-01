# Comparing `tmp/trytond_company-6.6.0.tar.gz` & `tmp/trytond_company-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_company-6.6.0.tar", last modified: Mon Oct 31 15:48:30 2022, max compression
+gzip compressed data, was "trytond_company-6.8.0.tar", last modified: Mon May  1 11:45:28 2023, max compression
```

## Comparing `trytond_company-6.6.0.tar` & `trytond_company-6.8.0.tar`

### file list

```diff
@@ -1,82 +1,78 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.440462 trytond_company-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_company-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_company-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 15:48:29.000000 trytond_company-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_company-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     3950 2022-10-31 15:48:28.000000 trytond_company-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:48:27.000000 trytond_company-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:31.000000 trytond_company-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_company-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2022-10-31 15:48:30.440462 trytond_company-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2022-10-27 11:24:44.000000 trytond_company-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1078 2021-12-11 16:59:33.000000 trytond_company-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4966 2022-10-11 19:49:57.000000 trytond_company-6.6.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9210 2022-04-08 16:27:20.000000 trytond_company-6.6.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.440462 trytond_company-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-04-27 07:34:40.000000 trytond_company-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2500 2022-05-31 08:02:36.000000 trytond_company-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2022-10-27 11:24:44.000000 trytond_company-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2406 2022-04-08 16:27:20.000000 trytond_company-6.6.0/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_company-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      949 2021-04-27 07:34:40.000000 trytond_company-6.6.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.440462 trytond_company-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:33.000000 trytond_company-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2019-06-04 16:49:44.000000 trytond_company-6.6.0/icons/tryton-company.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5012 2022-10-11 19:49:57.000000 trytond_company-6.6.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2022-04-08 16:24:27.000000 trytond_company-6.6.0/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    39274 2021-02-21 18:19:37.000000 trytond_company-6.6.0/letter.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.437129 trytond_company-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7802 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8302 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6904 2022-10-29 07:50:36.000000 trytond_company-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8593 2022-10-29 07:50:36.000000 trytond_company-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8405 2022-10-29 07:50:36.000000 trytond_company-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6632 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7967 2022-10-29 07:50:36.000000 trytond_company-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8831 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6904 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8554 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7879 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7774 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7428 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8673 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7432 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8358 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8100 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8071 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8193 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8089 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8072 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6904 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9485 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7887 2022-10-29 07:50:37.000000 trytond_company-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3172 2022-10-11 19:49:57.000000 trytond_company-6.6.0/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4096 2022-04-10 15:40:35.000000 trytond_company-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7332 2022-10-11 19:49:57.000000 trytond_company-6.6.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:48:30.440462 trytond_company-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5178 2022-10-29 07:39:10.000000 trytond_company-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.437129 trytond_company-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2022-04-16 16:30:56.000000 trytond_company-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10843 2022-04-16 16:30:56.000000 trytond_company-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1220 2021-07-12 20:56:37.000000 trytond_company-6.6.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2022-10-31 15:10:09.000000 trytond_company-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      102 2022-10-31 15:48:26.000000 trytond_company-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.440462 trytond_company-6.6.0/trytond_company.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2572 2022-10-31 15:48:29.000000 trytond_company-6.6.0/trytond_company.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2047 2022-10-31 15:48:30.000000 trytond_company-6.6.0/trytond_company.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:48:29.000000 trytond_company-6.6.0/trytond_company.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2022-10-31 15:48:29.000000 trytond_company-6.6.0/trytond_company.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:55.000000 trytond_company-6.6.0/trytond_company.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2022-10-31 15:48:29.000000 trytond_company-6.6.0/trytond_company.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:48:29.000000 trytond_company-6.6.0/trytond_company.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:30.437129 trytond_company-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2019-06-04 16:49:44.000000 trytond_company-6.6.0/view/company_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2021-03-24 12:36:50.000000 trytond_company-6.6.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2022-04-08 16:23:26.000000 trytond_company-6.6.0/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2019-06-04 16:49:44.000000 trytond_company-6.6.0/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2019-12-28 17:02:52.000000 trytond_company-6.6.0/view/employee_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2022-04-08 16:23:26.000000 trytond_company-6.6.0/view/employee_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2019-02-13 10:09:31.000000 trytond_company-6.6.0/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2022-04-08 16:23:26.000000 trytond_company-6.6.0/view/sequence_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2021-06-06 07:32:08.000000 trytond_company-6.6.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2021-04-27 07:34:40.000000 trytond_company-6.6.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.635298 trytond_company-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4113 2023-05-01 11:03:42.000000 trytond_company-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:03:41.000000 trytond_company-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_company-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_company-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2023-05-01 11:45:28.635298 trytond_company-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_company-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1078 2023-04-15 07:12:15.000000 trytond_company-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4966 2023-04-15 07:12:15.000000 trytond_company-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9210 2023-04-15 07:12:15.000000 trytond_company-6.8.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.631965 trytond_company-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_company-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2500 2023-04-15 07:12:15.000000 trytond_company-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_company-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2406 2023-04-15 07:12:15.000000 trytond_company-6.8.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_company-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      949 2023-04-15 07:12:15.000000 trytond_company-6.8.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.631965 trytond_company-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_company-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-01-16 14:00:20.000000 trytond_company-6.8.0/icons/tryton-company.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5038 2023-04-15 07:12:15.000000 trytond_company-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2023-04-15 07:12:15.000000 trytond_company-6.8.0/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    39274 2023-04-15 07:12:15.000000 trytond_company-6.8.0/letter.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.625298 trytond_company-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7802 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8302 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6904 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8593 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8405 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6632 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7967 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8831 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6904 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8554 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7879 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7774 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7428 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8673 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7432 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8358 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8100 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8071 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8304 2023-04-30 10:46:36.000000 trytond_company-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8089 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8072 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6904 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9485 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7887 2023-04-29 08:02:43.000000 trytond_company-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3172 2023-04-15 07:12:15.000000 trytond_company-6.8.0/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4096 2023-04-15 07:12:15.000000 trytond_company-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7332 2023-04-15 07:12:15.000000 trytond_company-6.8.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:45:28.635298 trytond_company-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4374 2023-04-15 07:12:15.000000 trytond_company-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.628631 trytond_company-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_company-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10843 2023-04-15 07:12:15.000000 trytond_company-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1219 2023-04-15 07:12:15.000000 trytond_company-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_company-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      102 2023-05-01 11:03:36.000000 trytond_company-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.635298 trytond_company-6.8.0/trytond_company.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2572 2023-05-01 11:45:27.000000 trytond_company-6.8.0/trytond_company.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2009 2023-05-01 11:45:28.000000 trytond_company-6.8.0/trytond_company.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:45:27.000000 trytond_company-6.8.0/trytond_company.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 11:45:27.000000 trytond_company-6.8.0/trytond_company.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_company-6.8.0/trytond_company.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2023-05-01 11:45:27.000000 trytond_company-6.8.0/trytond_company.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:45:27.000000 trytond_company-6.8.0/trytond_company.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:45:28.628631 trytond_company-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-01-16 14:00:20.000000 trytond_company-6.8.0/view/company_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/employee_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/employee_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-01-16 14:00:20.000000 trytond_company-6.8.0/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/sequence_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_company-6.8.0/view/user_form_preferences.xml
```

### Comparing `trytond_company-6.6.0/CHANGELOG` & `trytond_company-6.8.0/CHANGELOG`

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
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_company-6.6.0/COPYRIGHT` & `trytond_company-6.8.0/COPYRIGHT`

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

### Comparing `trytond_company-6.6.0/LICENSE` & `trytond_company-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/PKG-INFO` & `trytond_company-6.8.0/trytond_company.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_company
-Version: 6.6.0
+Name: trytond-company
+Version: 6.8.0
 Summary: Tryton module with companies and employees
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-company/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/company
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton company employee
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
 
 ##############
 Company Module
 ##############
 
 The *Company Module* allows the business that is using Tryton to be
```

### Comparing `trytond_company-6.6.0/__init__.py` & `trytond_company-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/company.py` & `trytond_company-6.8.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/company.xml` & `trytond_company-6.8.0/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/doc/conf.py` & `trytond_company-6.8.0/doc/conf.py`

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

### Comparing `trytond_company-6.6.0/doc/design.rst` & `trytond_company-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/doc/reference.rst` & `trytond_company-6.8.0/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/doc/usage.rst` & `trytond_company-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/icons/LICENSE` & `trytond_company-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/ir.py` & `trytond_company-6.8.0/ir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.model import (
     EvalEnvironment, ModelSQL, ModelView, dualmethod, fields)
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import timezone as tz
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 
 class Sequence(metaclass=PoolMeta):
     __name__ = 'ir.sequence'
     company = fields.Many2One(
         'company.company', "Company",
         help="Restricts the sequence usage to the company.")
@@ -72,16 +72,16 @@
         Employee = pool.get('company.employee')
         context = super()._get_context()
         # Use root to avoid infinite loop when accessing user attributes
         user_id = Transaction().user
         with Transaction().set_user(0):
             user = User(user_id)
         if user.employee:
-            with Transaction().set_context(
-                    _check_access=False, _datetime=None):
+            with without_check_access(), \
+                    Transaction().set_context(_datetime=None):
                 context['employee'] = EvalEnvironment(
                     Employee(user.employee.id), Employee)
         if user.company_filter == 'one':
             context['companies'] = [user.company.id] if user.company else []
             context['employees'] = [user.employee.id] if user.employee else []
         elif user.company_filter == 'all':
             context['companies'] = [c.id for c in user.companies]
```

### Comparing `trytond_company-6.6.0/ir.xml` & `trytond_company-6.8.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/letter.fodt` & `trytond_company-6.8.0/letter.fodt`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/bg.po` & `trytond_company-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/ca.po` & `trytond_company-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/cs.po` & `trytond_company-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/de.po` & `trytond_company-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/es.po` & `trytond_company-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/es_419.po` & `trytond_company-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/et.po` & `trytond_company-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/fa.po` & `trytond_company-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/fi.po` & `trytond_company-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/fr.po` & `trytond_company-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/hu.po` & `trytond_company-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/id.po` & `trytond_company-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/it.po` & `trytond_company-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/lo.po` & `trytond_company-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/lt.po` & `trytond_company-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/nl.po` & `trytond_company-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/pl.po` & `trytond_company-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/pt.po` & `trytond_company-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/ro.po` & `trytond_company-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -162,24 +162,25 @@
 msgid "The employee who oversees this employee."
 msgstr "Angajatul care supraveghează acest angajat."
 
 msgctxt "help:ir.cron,companies:"
 msgid "Companies registered for this cron."
 msgstr "Companii înregistrate pentru acest cron."
 
-#, fuzzy
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "\n"
 "- \"employee\" from the current user\n"
 "- \"employees\" as list of ids from the current user\n"
 "- \"companies\" as list of ids from the current user"
 msgstr ""
 "\n"
-"- \"angajatul\" de la utilizatorul curent"
+"- \"angajatul\" de la utilizatorul curent\n"
+"- \"angajați\" ca lista de ID-uri de la utilizatorul curent\n"
+"- \"companii\" ca lista de ID-uri de la utilizatorul curent"
 
 msgctxt "help:ir.sequence,company:"
 msgid "Restricts the sequence usage to the company."
 msgstr "Restricționează utilizarea secvenței la companie."
 
 msgctxt "help:ir.sequence.strict,company:"
 msgid "Restricts the sequence usage to the company."
@@ -245,15 +246,14 @@
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_sequence_strict_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_company"
 msgid "Companies"
 msgstr "Companii"
 
 msgctxt "model:ir.ui.menu,name:menu_company_list"
 msgid "Companies"
 msgstr "Companii"
```

### Comparing `trytond_company-6.6.0/locale/ru.po` & `trytond_company-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/sl.po` & `trytond_company-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/tr.po` & `trytond_company-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/uk.po` & `trytond_company-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/locale/zh_CN.po` & `trytond_company-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/model.py` & `trytond_company-6.8.0/model.py`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/party.py` & `trytond_company-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/res.py` & `trytond_company-6.8.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/setup.py` & `trytond_company-6.8.0/setup.py`

 * *Files 15% similar despite different names*

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
@@ -37,59 +34,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_company'
 
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
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module with companies and employees',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-company/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/company',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton company employee',
     package_dir={'trytond.modules.company': '.'},
     packages=(
         ['trytond.modules.company']
         + ['trytond.modules.company.%s' % p for p in find_packages()]
         ),
@@ -127,24 +104,23 @@
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
     company = trytond.modules.company
     """,
     )
```

### Comparing `trytond_company-6.6.0/tests/test_module.py` & `trytond_company-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/tests/tools.py` & `trytond_company-6.8.0/tests/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model, Wizard
 from proteus.config import get_config
-
 from trytond.modules.currency.tests.tools import get_currency
 
 __all__ = ['create_company', 'get_company']
 
 
 def create_company(party=None, currency=None, config=None):
     "Create the company using the proteus config"
```

### Comparing `trytond_company-6.6.0/trytond_company.egg-info/PKG-INFO` & `trytond_company-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-company
-Version: 6.6.0
+Name: trytond_company
+Version: 6.8.0
 Summary: Tryton module with companies and employees
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-company/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/company
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton company employee
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
 
 ##############
 Company Module
 ##############
 
 The *Company Module* allows the business that is using Tryton to be
```

### Comparing `trytond_company-6.6.0/trytond_company.egg-info/SOURCES.txt` & `trytond_company-6.8.0/trytond_company.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

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
 company.py
```

### Comparing `trytond_company-6.6.0/view/company_form.xml` & `trytond_company-6.8.0/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/view/user_form.xml` & `trytond_company-6.8.0/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_company-6.6.0/view/user_form_preferences.xml` & `trytond_company-6.8.0/view/user_form_preferences.xml`

 * *Files identical despite different names*

