# Comparing `tmp/trytond_account_dunning_fee-6.6.1.tar.gz` & `tmp/trytond_account_dunning_fee-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_dunning_fee-6.6.1.tar", last modified: Sat Mar  4 12:28:05 2023, max compression
+gzip compressed data, was "trytond_account_dunning_fee-6.8.0.tar", last modified: Mon May  1 11:48:47 2023, max compression
```

## Comparing `trytond_account_dunning_fee-6.6.1.tar` & `trytond_account_dunning_fee-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:28:05.870077 trytond_account_dunning_fee-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-03-04 12:28:02.000000 trytond_account_dunning_fee-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-03-04 12:28:02.000000 trytond_account_dunning_fee-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2903 2023-03-04 12:28:05.870077 trytond_account_dunning_fee-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:28:05.866743 trytond_account_dunning_fee-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6682 2023-02-27 17:46:08.000000 trytond_account_dunning_fee-6.6.1/dunning.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6128 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/dunning.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:28:05.860077 trytond_account_dunning_fee-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1929 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2059 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1793 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1947 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1846 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2687 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1813 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2113 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1917 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2081 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2071 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2117 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1859 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 12:28:05.870077 trytond_account_dunning_fee-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4433 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:28:05.863410 trytond_account_dunning_fee-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5011 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/tests/scenario_account_dunning_fee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      546 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2022-12-19 12:03:07.000000 trytond_account_dunning_fee-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:28:05.870077 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2903 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1931 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 12:28:05.000000 trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:28:05.866743 trytond_account_dunning_fee-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_fee_dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_fee_dunning_level_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_fee_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_fee_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_level_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2022-12-19 12:02:49.000000 trytond_account_dunning_fee-6.6.1/view/dunning_level_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:47.757769 trytond_account_dunning_fee-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1237 2023-05-01 11:05:51.000000 trytond_account_dunning_fee-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:05:51.000000 trytond_account_dunning_fee-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2891 2023-05-01 11:48:47.757769 trytond_account_dunning_fee-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-04-15 07:12:14.000000 trytond_account_dunning_fee-6.8.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:47.757769 trytond_account_dunning_fee-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6783 2023-04-21 08:36:08.000000 trytond_account_dunning_fee-6.8.0/dunning.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6128 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/dunning.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:47.751102 trytond_account_dunning_fee-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2082 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1929 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2059 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1793 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1947 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1846 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2687 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1813 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2113 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1805 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2081 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2071 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2117 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1859 2023-04-29 08:02:45.000000 trytond_account_dunning_fee-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:48:47.757769 trytond_account_dunning_fee-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4393 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:47.754436 trytond_account_dunning_fee-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4956 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/tests/scenario_account_dunning_fee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:14.000000 trytond_account_dunning_fee-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-05-01 11:05:46.000000 trytond_account_dunning_fee-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:47.757769 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2891 2023-05-01 11:48:46.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1931 2023-05-01 11:48:47.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:48:46.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-05-01 11:48:46.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2023-05-01 11:48:46.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:48:46.000000 trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:47.754436 trytond_account_dunning_fee-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/view/dunning_fee_dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/view/dunning_fee_dunning_level_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/view/dunning_fee_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_account_dunning_fee-6.8.0/view/dunning_fee_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/view/dunning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/view/dunning_level_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-01-16 14:00:20.000000 trytond_account_dunning_fee-6.8.0/view/dunning_level_list.xml
```

### Comparing `trytond_account_dunning_fee-6.6.1/CHANGELOG` & `trytond_account_dunning_fee-6.8.0/CHANGELOG`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-03-04
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

### Comparing `trytond_account_dunning_fee-6.6.1/COPYRIGHT` & `trytond_account_dunning_fee-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/LICENSE` & `trytond_account_dunning_fee-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/PKG-INFO` & `trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_dunning_fee
-Version: 6.6.1
+Name: trytond-account-dunning-fee
+Version: 6.8.0
 Summary: Tryton module for account dunning fee
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_dunning_fee
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: account dunning fee
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
 
 Account Dunning Fee Module
 ##########################
 
 The account_dunning_fee module allows to generate accounting moves as fees when
```

### Comparing `trytond_account_dunning_fee-6.6.1/README.rst` & `trytond_account_dunning_fee-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/__init__.py` & `trytond_account_dunning_fee-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/doc/conf.py` & `trytond_account_dunning_fee-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_dunning_fee-6.6.1/doc/index.rst` & `trytond_account_dunning_fee-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/dunning.py` & `trytond_account_dunning_fee-6.8.0/dunning.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,24 @@
         help='Method to compute the fee amount')
     percentage = fields.Numeric('Percentage', digits=(16, 8),
         states={
             'invisible': Eval('compute_method') != 'percentage',
             'required': Eval('compute_method') == 'percentage',
             })
 
+    def get_list_price(self, dunning, **pattern):
+        pattern.setdefault('company', dunning.company.id)
+        return self.product.get_multivalue('list_price', **pattern)
+
     def get_amount(self, dunning):
         'Return fee amount and currency'
         amount, currency = None, None
         if self.compute_method == 'list_price':
-            assert Transaction().context.get('company') == dunning.company.id
             currency = dunning.company.currency
-            amount = currency.round(self.product.list_price)
+            amount = currency.round(self.get_list_price(dunning))
         elif self.compute_method == 'percentage':
             if dunning.second_currency:
                 amount = dunning.amount_second_currency
                 currency = dunning.second_currency
             else:
                 amount = dunning.amount
                 currency = dunning.company.currency
@@ -136,15 +139,15 @@
 
         with Transaction().set_context(company=self.dunning.company.id):
             today = Date.today()
         move = Move()
         move.company = self.dunning.company
         move.journal = self.level.fee.journal
         move.date = today
-        move.period = Period.find(move.company.id, date=today)
+        move.period = Period.find(move.company, date=today)
         move.origin = self
         move.description = self.level.fee.name
 
         line = Line()
         if self.currency == move.company.currency:
             line.debit = self.amount
         else:
```

### Comparing `trytond_account_dunning_fee-6.6.1/dunning.xml` & `trytond_account_dunning_fee-6.8.0/dunning.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/bg.po` & `trytond_account_dunning_fee-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/ca.po` & `trytond_account_dunning_fee-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/cs.po` & `trytond_account_dunning_fee-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/de.po` & `trytond_account_dunning_fee-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/es.po` & `trytond_account_dunning_fee-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/es_419.po` & `trytond_account_dunning_fee-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/et.po` & `trytond_account_dunning_fee-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/fa.po` & `trytond_account_dunning_fee-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/fi.po` & `trytond_account_dunning_fee-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/fr.po` & `trytond_account_dunning_fee-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/hu.po` & `trytond_account_dunning_fee-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/id.po` & `trytond_account_dunning_fee-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/it.po` & `trytond_account_dunning_fee-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/lo.po` & `trytond_account_dunning_fee-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/lt.po` & `trytond_account_dunning_fee-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/nl.po` & `trytond_account_dunning_fee-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/pl.po` & `trytond_account_dunning_fee-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/pt.po` & `trytond_account_dunning_fee-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/ro.po` & `trytond_account_dunning_fee-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/ru.po` & `trytond_account_dunning_fee-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/sl.po` & `trytond_account_dunning_fee-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/tr.po` & `trytond_account_dunning_fee-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/uk.po` & `trytond_account_dunning_fee-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/locale/zh_CN.po` & `trytond_account_dunning_fee-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/setup.py` & `trytond_account_dunning_fee-6.8.0/setup.py`

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
@@ -34,16 +31,19 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_dunning_fee'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
@@ -51,22 +51,22 @@
     get_require_version('trytond_account_dunning_letter')]
 
 setup(name=name,
     version=version,
     description='Tryton module for account dunning fee',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_dunning_fee',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='account dunning fee',
     package_dir={'trytond.modules.account_dunning_fee': '.'},
     packages=(
         ['trytond.modules.account_dunning_fee']
         + ['trytond.modules.account_dunning_fee.%s' % p
             for p in find_packages()]
@@ -103,23 +103,23 @@
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

### Comparing `trytond_account_dunning_fee-6.6.1/tests/scenario_account_dunning_fee.rst` & `trytond_account_dunning_fee-6.8.0/tests/scenario_account_dunning_fee.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 ============================
 Account Dunning Fee Scenario
 ============================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import config, Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_dunning_fee')
 
 Create company::
 
@@ -83,18 +82,18 @@
     >>> fee_pc.save()
 
 Create dunning procedure::
 
     >>> Procedure = Model.get('account.dunning.procedure')
     >>> procedure = Procedure(name='Procedure Fee')
     >>> level = procedure.levels.new()
-    >>> level.overdue = datetime.timedelta(5)
+    >>> level.overdue = dt.timedelta(5)
     >>> level.fee = fee
     >>> level = procedure.levels.new()
-    >>> level.overdue = datetime.timedelta(10)
+    >>> level.overdue = dt.timedelta(10)
     >>> level.fee = fee_pc
     >>> procedure.save()
 
 Create parties::
 
     >>> Party = Model.get('party.party')
     >>> customer = Party(name='Customer')
@@ -127,16 +126,16 @@
     >>> revenue.balance
     Decimal('-100.00')
 
 Create dunning on 5 days::
 
     >>> Dunning = Model.get('account.dunning')
     >>> create_dunning = Wizard('account.dunning.create')
-    >>> create_dunning.form.date = (period.start_date
-    ...     + datetime.timedelta(days=5))
+    >>> create_dunning.form.date = (
+    ...     period.start_date + dt.timedelta(days=5))
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
 
 Process dunning::
 
     >>> process_dunning = Wizard('account.dunning.process',
     ...     [dunning])
@@ -152,15 +151,15 @@
     Decimal('-110.00')
 
 Create dunning on 10 days::
 
     >>> Dunning = Model.get('account.dunning')
     >>> create_dunning = Wizard('account.dunning.create')
     >>> create_dunning.form.date = (period.start_date
-    ...     + datetime.timedelta(days=10))
+    ...     + dt.timedelta(days=10))
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
 
 Process dunning::
 
     >>> process_dunning = Wizard('account.dunning.process',
     ...     [dunning])
```

### Comparing `trytond_account_dunning_fee-6.6.1/tox.ini` & `trytond_account_dunning_fee-6.8.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/account_dunning_fee/* -m unittest discover -s tests
-    coverage report --include=./**/account_dunning_fee/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/PKG-INFO` & `trytond_account_dunning_fee-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-dunning-fee
-Version: 6.6.1
+Name: trytond_account_dunning_fee
+Version: 6.8.0
 Summary: Tryton module for account dunning fee
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_dunning_fee
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: account dunning fee
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
 
 Account Dunning Fee Module
 ##########################
 
 The account_dunning_fee module allows to generate accounting moves as fees when
```

### Comparing `trytond_account_dunning_fee-6.6.1/trytond_account_dunning_fee.egg-info/SOURCES.txt` & `trytond_account_dunning_fee-6.8.0/trytond_account_dunning_fee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_dunning_fee-6.6.1/view/dunning_fee_form.xml` & `trytond_account_dunning_fee-6.8.0/view/dunning_fee_form.xml`

 * *Files identical despite different names*

