# Comparing `tmp/trytond_account_dunning_letter-6.6.0.tar.gz` & `tmp/trytond_account_dunning_letter-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning_letter-6.6.0.tar", last modified: Mon Oct 31 15:54:47 2022, max compression
+gzip compressed data, was "trytond_account_dunning_letter-6.8.0.tar", last modified: Mon May  1 11:54:18 2023, max compression
```

## Comparing `trytond_account_dunning_letter-6.6.0.tar` & `trytond_account_dunning_letter-6.8.0.tar`

### file list

```diff
@@ -1,62 +1,59 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:47.879283 trytond_account_dunning_letter-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_dunning_letter-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_dunning_letter-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2022-10-31 15:54:46.000000 trytond_account_dunning_letter-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_dunning_letter-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1555 2022-10-31 15:54:45.000000 trytond_account_dunning_letter-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:54:45.000000 trytond_account_dunning_letter-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:06.000000 trytond_account_dunning_letter-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_dunning_letter-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2527 2022-10-31 15:54:47.879283 trytond_account_dunning_letter-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2018-08-18 09:54:06.000000 trytond_account_dunning_letter-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2021-12-11 16:59:32.000000 trytond_account_dunning_letter-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:47.875950 trytond_account_dunning_letter-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2018-08-18 09:54:06.000000 trytond_account_dunning_letter-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5286 2022-04-08 16:23:26.000000 trytond_account_dunning_letter-6.6.0/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1469 2019-06-04 16:49:43.000000 trytond_account_dunning_letter-6.6.0/dunning.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    60409 2021-10-31 09:17:58.000000 trytond_account_dunning_letter-6.6.0/letter.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:47.875950 trytond_account_dunning_letter-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1029 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1018 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      882 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1018 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      888 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1065 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      882 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      882 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1000 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      895 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1003 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1004 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1010 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      978 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      989 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      939 2022-10-29 07:50:41.000000 trytond_account_dunning_letter-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:54:47.879283 trytond_account_dunning_letter-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5291 2022-10-29 07:39:10.000000 trytond_account_dunning_letter-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:47.875950 trytond_account_dunning_letter-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_dunning_letter-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5652 2020-07-09 09:36:50.000000 trytond_account_dunning_letter-6.6.0/tests/scenario_account_dunning_letter.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2022-04-16 16:30:55.000000 trytond_account_dunning_letter-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_dunning_letter-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_account_dunning_letter-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      114 2022-10-31 15:54:44.000000 trytond_account_dunning_letter-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:47.879283 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2527 2022-10-31 15:54:47.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1642 2022-10-31 15:54:47.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:54:47.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 15:54:47.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:04.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2022-10-31 15:54:47.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:54:47.000000 trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:54:47.875950 trytond_account_dunning_letter-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2018-08-18 09:54:06.000000 trytond_account_dunning_letter-6.6.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2018-08-18 09:54:06.000000 trytond_account_dunning_letter-6.6.0/view/dunning_level_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:18.595208 trytond_account_dunning_letter-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-05-01 11:09:39.000000 trytond_account_dunning_letter-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:09:39.000000 trytond_account_dunning_letter-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-05-01 11:54:18.595208 trytond_account_dunning_letter-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:18.595208 trytond_account_dunning_letter-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5286 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-6.8.0/dunning.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    60409 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/letter.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:18.591875 trytond_account_dunning_letter-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1029 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1018 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      882 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1018 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      888 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1065 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      882 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      882 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1000 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1003 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1004 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1010 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      978 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      989 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      939 2023-04-29 08:02:47.000000 trytond_account_dunning_letter-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:54:18.595208 trytond_account_dunning_letter-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4473 2023-04-15 07:12:14.000000 trytond_account_dunning_letter-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:18.591875 trytond_account_dunning_letter-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5556 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/tests/scenario_account_dunning_letter.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_dunning_letter-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      114 2023-05-01 11:09:33.000000 trytond_account_dunning_letter-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:18.595208 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2512 2023-05-01 11:54:17.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1616 2023-05-01 11:54:18.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:54:17.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:54:17.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-05-01 11:54:17.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:54:17.000000 trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:18.595208 trytond_account_dunning_letter-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-6.8.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-16 14:00:20.000000 trytond_account_dunning_letter-6.8.0/view/dunning_level_list.xml
```

### Comparing `trytond_account_dunning_letter-6.6.0/CHANGELOG` & `trytond_account_dunning_letter-6.8.0/CHANGELOG`

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

### Comparing `trytond_account_dunning_letter-6.6.0/COPYRIGHT` & `trytond_account_dunning_letter-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_dunning_letter-6.6.0/LICENSE` & `trytond_account_dunning_letter-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/PKG-INFO` & `trytond_account_dunning_letter-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning_letter
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for account dunning letter
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_dunning_letter
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account dunning letter
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
 
 Account Dunning Letter Module
 #############################
 
 The account_dunning_letter module generates a dunning letter after the process
```

### Comparing `trytond_account_dunning_letter-6.6.0/__init__.py` & `trytond_account_dunning_letter-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/dunning.py` & `trytond_account_dunning_letter-6.8.0/dunning.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/dunning.xml` & `trytond_account_dunning_letter-6.8.0/dunning.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/letter.fodt` & `trytond_account_dunning_letter-6.8.0/letter.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/bg.po` & `trytond_account_dunning_letter-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/ca.po` & `trytond_account_dunning_letter-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/cs.po` & `trytond_account_dunning_letter-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/de.po` & `trytond_account_dunning_letter-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/es.po` & `trytond_account_dunning_letter-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/es_419.po` & `trytond_account_dunning_letter-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/et.po` & `trytond_account_dunning_letter-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/fa.po` & `trytond_account_dunning_letter-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/fi.po` & `trytond_account_dunning_letter-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/fr.po` & `trytond_account_dunning_letter-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/hu.po` & `trytond_account_dunning_letter-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/id.po` & `trytond_account_dunning_letter-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/it.po` & `trytond_account_dunning_letter-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/lo.po` & `trytond_account_dunning_letter-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/lt.po` & `trytond_account_dunning_letter-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/nl.po` & `trytond_account_dunning_letter-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/pl.po` & `trytond_account_dunning_letter-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/pt.po` & `trytond_account_dunning_letter-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/ro.po` & `trytond_account_dunning_letter-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/ru.po` & `trytond_account_dunning_letter-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/sl.po` & `trytond_account_dunning_letter-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/tr.po` & `trytond_account_dunning_letter-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/uk.po` & `trytond_account_dunning_letter-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/locale/zh_CN.po` & `trytond_account_dunning_letter-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_letter-6.6.0/setup.py` & `trytond_account_dunning_letter-6.8.0/setup.py`

 * *Files 22% similar despite different names*

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
 name = 'trytond_account_dunning_letter'
 
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
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for account dunning letter',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_dunning_letter',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account dunning letter',
     package_dir={'trytond.modules.account_dunning_letter': '.'},
     packages=(
         ['trytond.modules.account_dunning_letter']
         + ['trytond.modules.account_dunning_letter.%s' % p
             for p in find_packages()]
@@ -125,28 +103,27 @@
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
     account_dunning_letter = trytond.modules.account_dunning_letter
     """,
     )
```

### Comparing `trytond_account_dunning_letter-6.6.0/tests/scenario_account_dunning_letter.rst` & `trytond_account_dunning_letter-6.8.0/tests/scenario_account_dunning_letter.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 ========================
 Account Dunning Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import config, Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning_letter')
 
 Create company::
 
@@ -78,15 +76,15 @@
 Create dunning procedure::
 
     >>> set_user(account_admin_user)
     >>> Procedure = Model.get('account.dunning.procedure')
     >>> procedure = Procedure(name='Procedure')
     >>> level = procedure.levels.new()
     >>> level.sequence = 1
-    >>> level.overdue = datetime.timedelta(5)
+    >>> level.overdue = dt.timedelta(5)
     >>> level.print_on_letter = True
     >>> procedure.save()
 
 Create parties::
 
     >>> Party = Model.get('party.party')
     >>> customer = Party(name='Customer')
@@ -170,15 +168,15 @@
     >>> move.save()
 
 Create dunnings::
 
     >>> set_user(dunning_user)
     >>> Dunning = Model.get('account.dunning')
     >>> create_dunning = Wizard('account.dunning.create')
-    >>> create_dunning.form.date = period.start_date + relativedelta(days=5)
+    >>> create_dunning.form.date = period.start_date + dt.timedelta(days=5)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
 
 Process dunning::
 
     >>> process_dunning = Wizard('account.dunning.process',
     ...     [dunning])
```

### Comparing `trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/PKG-INFO` & `trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-dunning-letter
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for account dunning letter
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_dunning_letter
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account dunning letter
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
 
 Account Dunning Letter Module
 #############################
 
 The account_dunning_letter module generates a dunning letter after the process
```

### Comparing `trytond_account_dunning_letter-6.6.0/trytond_account_dunning_letter.egg-info/SOURCES.txt` & `trytond_account_dunning_letter-6.8.0/trytond_account_dunning_letter.egg-info/SOURCES.txt`

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
 dunning.py
@@ -45,14 +41,15 @@
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_account_dunning_letter.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/dunning_level_form.xml
 ./view/dunning_level_list.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

