# Comparing `tmp/trytond_account_dunning-6.6.0.tar.gz` & `tmp/trytond_account_dunning-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning-6.6.0.tar", last modified: Mon Oct 31 15:51:24 2022, max compression
+gzip compressed data, was "trytond_account_dunning-6.8.0.tar", last modified: Mon May  1 11:54:55 2023, max compression
```

## Comparing `trytond_account_dunning-6.6.0.tar` & `trytond_account_dunning-6.8.0.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:24.286323 trytond_account_dunning-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_dunning-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_dunning-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2022-10-31 15:51:22.000000 trytond_account_dunning-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_dunning-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2022-10-31 15:51:22.000000 trytond_account_dunning-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:51:21.000000 trytond_account_dunning-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_dunning-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3319 2022-10-31 15:51:24.286323 trytond_account_dunning-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2019-06-04 16:49:43.000000 trytond_account_dunning-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2021-12-11 16:59:32.000000 trytond_account_dunning-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2021-12-11 16:59:32.000000 trytond_account_dunning-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:24.286323 trytond_account_dunning-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2019-06-04 16:49:43.000000 trytond_account_dunning-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14027 2022-10-11 19:49:57.000000 trytond_account_dunning-6.6.0/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14858 2021-10-07 13:15:58.000000 trytond_account_dunning-6.6.0/dunning.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:24.282990 trytond_account_dunning-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7968 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6852 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7762 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8040 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7158 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7702 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8263 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6839 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7899 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8205 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6706 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8681 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6967 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7909 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6981 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7515 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6646 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7437 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7360 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7234 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6493 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2022-10-29 07:50:41.000000 trytond_account_dunning-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2019-10-11 23:09:47.000000 trytond_account_dunning-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1822 2022-10-11 19:49:57.000000 trytond_account_dunning-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:51:24.286323 trytond_account_dunning-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5197 2022-10-29 07:39:09.000000 trytond_account_dunning-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:24.282990 trytond_account_dunning-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_dunning-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8209 2021-10-07 13:09:31.000000 trytond_account_dunning-6.6.0/tests/scenario_account_dunning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3069 2020-07-09 09:36:49.000000 trytond_account_dunning-6.6.0/tests/scenario_account_dunning_final.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2022-04-16 16:30:55.000000 trytond_account_dunning-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_dunning-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_account_dunning-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2022-10-31 15:51:20.000000 trytond_account_dunning-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:24.286323 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3319 2022-10-31 15:51:23.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2301 2022-10-31 15:51:24.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:51:23.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 15:51:23.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:04.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      136 2022-10-31 15:51:23.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:51:23.000000 trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:24.286323 trytond_account_dunning-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2020-07-08 22:22:00.000000 trytond_account_dunning-6.6.0/view/dunning_create_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2021-10-07 13:09:31.000000 trytond_account_dunning-6.6.0/view/dunning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2019-10-11 23:09:47.000000 trytond_account_dunning-6.6.0/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/view/dunning_level_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/view/dunning_level_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2022-04-08 16:23:25.000000 trytond_account_dunning-6.6.0/view/dunning_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/view/dunning_procedure_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/view/dunning_procedure_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2020-07-08 22:22:00.000000 trytond_account_dunning-6.6.0/view/dunning_process_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2018-08-18 09:54:05.000000 trytond_account_dunning-6.6.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:55.198996 trytond_account_dunning-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1915 2023-05-01 11:10:05.000000 trytond_account_dunning-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:10:05.000000 trytond_account_dunning-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3311 2023-05-01 11:54:55.198996 trytond_account_dunning-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-04-15 07:12:14.000000 trytond_account_dunning-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:55.195662 trytond_account_dunning-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account_dunning-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14021 2023-04-28 07:46:16.000000 trytond_account_dunning-6.8.0/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14858 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/dunning.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:55.188995 trytond_account_dunning-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7436 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7968 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6852 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7762 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8040 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7158 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7702 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8263 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6839 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7899 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8205 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6706 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7417 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8681 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6967 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7909 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6981 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7515 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6646 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7437 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7360 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7234 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6493 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2023-04-29 08:02:47.000000 trytond_account_dunning-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1822 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:54:55.198996 trytond_account_dunning-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4386 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:55.188995 trytond_account_dunning-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8206 2023-04-15 07:12:14.000000 trytond_account_dunning-6.8.0/tests/scenario_account_dunning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2972 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/tests/scenario_account_dunning_final.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:14.000000 trytond_account_dunning-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2023-05-01 11:09:59.000000 trytond_account_dunning-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:55.198996 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3311 2023-05-01 11:54:54.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2275 2023-05-01 11:54:55.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:54:54.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:54:54.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      136 2023-05-01 11:54:54.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:54:54.000000 trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:54:55.195662 trytond_account_dunning-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/view/dunning_create_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/view/dunning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:14.000000 trytond_account_dunning-6.8.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/view/dunning_level_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/view/dunning_level_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/view/dunning_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/view/dunning_procedure_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/view/dunning_procedure_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_dunning-6.8.0/view/dunning_process_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-01-16 14:00:20.000000 trytond_account_dunning-6.8.0/view/party_form.xml
```

### Comparing `trytond_account_dunning-6.6.0/CHANGELOG` & `trytond_account_dunning-6.8.0/CHANGELOG`

 * *Files 24% similar despite different names*

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

### Comparing `trytond_account_dunning-6.6.0/COPYRIGHT` & `trytond_account_dunning-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_dunning-6.6.0/LICENSE` & `trytond_account_dunning-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/PKG-INFO` & `trytond_account_dunning-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_dunning
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for account dunning
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_dunning
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account dunning
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
 
 Account Dunning Module
 ######################
 
 The account_dunning module adds dunning for receivable move lines.
```

### Comparing `trytond_account_dunning-6.6.0/README.rst` & `trytond_account_dunning-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/__init__.py` & `trytond_account_dunning-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/account.py` & `trytond_account_dunning-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/account.xml` & `trytond_account_dunning-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/doc/index.rst` & `trytond_account_dunning-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/dunning.py` & `trytond_account_dunning-6.8.0/dunning.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sql import Literal, Null
 
 from trytond.model import (
     Index, Model, ModelSQL, ModelView, Unique, fields, sequence_ordered)
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Eval
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, check_access
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 
 class Procedure(ModelSQL, ModelView):
     'Account Dunning Procedure'
     __name__ = 'account.dunning.procedure'
@@ -261,15 +261,15 @@
         Date = pool.get('ir.date')
         MoveLine = pool.get('account.move.line')
 
         if date is None:
             date = Date.today()
 
         set_level = defaultdict(list)
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             dunnings = cls.search([
                     ('state', '=', 'waiting'),
                     ('blocked', '=', False),
                     ])
         dunnings = cls.browse(dunnings)
         for dunning in dunnings:
             procedure = dunning.procedure
@@ -297,15 +297,15 @@
                 to_write.extend((dunnings, {
                             'state': 'final',
                             'date': Date.today(),
                             }))
         if to_write:
             cls.write(*to_write)
 
-        with Transaction().set_context(_check_access=True):
+        with check_access():
             lines = MoveLine.search(cls._overdue_line_domain(date))
         lines = MoveLine.browse(lines)
         dunnings = (cls._get_dunning(line, date) for line in lines)
         cls.save([d for d in dunnings if d])
 
     @classmethod
     def _get_dunning(cls, line, date):
@@ -314,14 +314,15 @@
             return
         for level in procedure.levels:
             if level.test(line, date):
                 break
         else:
             return
         return cls(
+            company=line.account.company,
             line=line,
             procedure=procedure,
             level=level,
             )
 
     @classmethod
     def process(cls, dunnings):
```

### Comparing `trytond_account_dunning-6.6.0/dunning.xml` & `trytond_account_dunning-6.8.0/dunning.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/bg.po` & `trytond_account_dunning-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/ca.po` & `trytond_account_dunning-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/cs.po` & `trytond_account_dunning-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/de.po` & `trytond_account_dunning-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/es.po` & `trytond_account_dunning-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/es_419.po` & `trytond_account_dunning-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/et.po` & `trytond_account_dunning-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/fa.po` & `trytond_account_dunning-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/fi.po` & `trytond_account_dunning-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/fr.po` & `trytond_account_dunning-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/hu.po` & `trytond_account_dunning-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/id.po` & `trytond_account_dunning-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/it.po` & `trytond_account_dunning-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/lo.po` & `trytond_account_dunning-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/lt.po` & `trytond_account_dunning-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/nl.po` & `trytond_account_dunning-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/pl.po` & `trytond_account_dunning-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/pt.po` & `trytond_account_dunning-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/ro.po` & `trytond_account_dunning-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/ru.po` & `trytond_account_dunning-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/sl.po` & `trytond_account_dunning-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/tr.po` & `trytond_account_dunning-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/uk.po` & `trytond_account_dunning-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/locale/zh_CN.po` & `trytond_account_dunning-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/party.py` & `trytond_account_dunning-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/setup.py` & `trytond_account_dunning-6.8.0/setup.py`

 * *Files 19% similar despite different names*

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
@@ -34,59 +31,40 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_dunning'
 
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
     description='Tryton module for account dunning',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_dunning',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     download_url=download_url,
     keywords='tryton account dunning',
     package_dir={'trytond.modules.account_dunning': '.'},
     packages=(
         ['trytond.modules.account_dunning']
         + ['trytond.modules.account_dunning.%s' % p for p in find_packages()]
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
     account_dunning = trytond.modules.account_dunning
     """,
     )
```

### Comparing `trytond_account_dunning-6.6.0/tests/scenario_account_dunning.rst` & `trytond_account_dunning-6.8.0/tests/scenario_account_dunning.rst`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     >>> process_dunning = Wizard('account.dunning.process',
     ...     [dunning])
     >>> process_dunning.execute('process')
     >>> dunning.reload()
     >>> dunning.state
     'waiting'
-    >>> dunning.date == today
+    >>> bool(dunning.date)
     True
 
 Create dunnings on 30 days with blocked dunning::
 
     >>> dunning.blocked = True
     >>> dunning.save()
     >>> create_dunning = Wizard('account.dunning.create')
```

### Comparing `trytond_account_dunning-6.6.0/tests/scenario_account_dunning_final.rst` & `trytond_account_dunning-6.8.0/tests/scenario_account_dunning_final.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 ==============================
 Account Dunning Final Scenario
 ==============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning')
 
 Create company::
 
@@ -40,15 +38,15 @@
 
 Create dunning procedure::
 
     >>> Procedure = Model.get('account.dunning.procedure')
     >>> procedure = Procedure(name='Procedure')
     >>> level = procedure.levels.new()
     >>> level.sequence = 1
-    >>> level.overdue = datetime.timedelta(0)
+    >>> level.overdue = dt.timedelta(0)
     >>> procedure.save()
 
 Create parties::
 
     >>> Party = Model.get('party.party')
     >>> customer = Party(name='Customer')
     >>> customer.dunning_procedure = procedure
@@ -78,15 +76,15 @@
     >>> line.maturity_date = period.start_date
     >>> move.save()
 
 Create dunning::
 
     >>> Dunning = Model.get('account.dunning')
     >>> create_dunning = Wizard('account.dunning.create')
-    >>> create_dunning.form.date = period.start_date + relativedelta(days=1)
+    >>> create_dunning.form.date = period.start_date + dt.timedelta(days=1)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
     >>> dunning.state
     'draft'
 
 Process dunning::
 
@@ -96,12 +94,12 @@
     >>> dunning.reload()
     >>> dunning.state
     'waiting'
 
 Refresh dunning::
 
     >>> create_dunning = Wizard('account.dunning.create')
-    >>> create_dunning.form.date = period.start_date + relativedelta(days=2)
+    >>> create_dunning.form.date = period.start_date + dt.timedelta(days=2)
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
     >>> dunning.state
     'final'
```

### Comparing `trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/PKG-INFO` & `trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-dunning
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for account dunning
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_dunning
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account dunning
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
 
 Account Dunning Module
 ######################
 
 The account_dunning module adds dunning for receivable move lines.
```

### Comparing `trytond_account_dunning-6.6.0/trytond_account_dunning.egg-info/SOURCES.txt` & `trytond_account_dunning-6.8.0/trytond_account_dunning.egg-info/SOURCES.txt`

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
 account.py
@@ -63,14 +59,15 @@
 ./view/dunning_level_list.xml
 ./view/dunning_level_list_sequence.xml
 ./view/dunning_list.xml
 ./view/dunning_procedure_form.xml
 ./view/dunning_procedure_list.xml
 ./view/dunning_process_start_form.xml
 ./view/party_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_dunning-6.6.0/view/dunning_form.xml` & `trytond_account_dunning-6.8.0/view/dunning_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning-6.6.0/view/dunning_list.xml` & `trytond_account_dunning-6.8.0/view/dunning_list.xml`

 * *Files identical despite different names*

