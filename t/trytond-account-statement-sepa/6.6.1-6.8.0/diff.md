# Comparing `tmp/trytond_account_statement_sepa-6.6.1.tar.gz` & `tmp/trytond_account_statement_sepa-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_sepa-6.6.1.tar", last modified: Thu Nov 17 17:52:09 2022, max compression
+gzip compressed data, was "trytond_account_statement_sepa-6.8.0.tar", last modified: Mon May  1 11:40:43 2023, max compression
```

## Comparing `trytond_account_statement_sepa-6.6.1.tar` & `trytond_account_statement_sepa-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-11-17 17:52:09.839274 trytond_account_statement_sepa-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)       94 2022-11-17 17:52:08.000000 trytond_account_statement_sepa-6.6.1/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2022-11-17 17:52:07.000000 trytond_account_statement_sepa-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2022-11-17 17:52:07.000000 trytond_account_statement_sepa-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2560 2022-11-17 17:52:09.839274 trytond_account_statement_sepa-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9507 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6603 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-11-17 17:52:09.835940 trytond_account_statement_sepa-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-11-17 17:52:09.832607 trytond_account_statement_sepa-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3751 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3638 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3782 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3775 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3569 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3118 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-11-17 17:52:09.839274 trytond_account_statement_sepa-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5475 2022-11-14 22:42:28.000000 trytond_account_statement_sepa-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-11-17 17:52:09.835940 trytond_account_statement_sepa-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4737 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/tests/camt.053.001.02.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3592 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/tests/scenario_account_statement_sepa.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 16:31:01.000000 trytond_account_statement_sepa-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2022-10-31 16:33:28.000000 trytond_account_statement_sepa-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-11-17 17:52:09.839274 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2560 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1583 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-11-17 17:52:09.000000 trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:43.475093 trytond_account_statement_sepa-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-05-01 11:00:36.000000 trytond_account_statement_sepa-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 11:00:35.000000 trytond_account_statement_sepa-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2023-05-01 11:40:43.475093 trytond_account_statement_sepa-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9507 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6603 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:43.471759 trytond_account_statement_sepa-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:43.468426 trytond_account_statement_sepa-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3751 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3638 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3782 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3775 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3569 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3118 2023-04-29 08:02:40.000000 trytond_account_statement_sepa-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:40:43.475093 trytond_account_statement_sepa-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4648 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:43.471759 trytond_account_statement_sepa-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4737 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/tests/camt.053.001.02.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/tests/scenario_account_statement_sepa.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_statement_sepa-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2023-05-01 11:00:30.000000 trytond_account_statement_sepa-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:40:43.475093 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2023-05-01 11:40:42.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1545 2023-05-01 11:40:43.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:40:42.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 11:40:42.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-05-01 11:40:42.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:40:42.000000 trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/top_level.txt
```

### Comparing `trytond_account_statement_sepa-6.6.1/COPYRIGHT` & `trytond_account_statement_sepa-6.8.0/COPYRIGHT`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2015-2022 B2CK
-Copyright (C) 2022 Cédric Krier
-Copyright (C) 2015 Nicolas Évrard
+Copyright (C) 2015-2023 B2CK
+Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2015-2023 Nicolas Évrard
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_statement_sepa-6.6.1/LICENSE` & `trytond_account_statement_sepa-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/PKG-INFO` & `trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_statement_sepa
-Version: 6.6.1
+Name: trytond-account-statement-sepa
+Version: 6.8.0
 Summary: Tryton module to import SEPA statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-statement-sepa
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement_sepa
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement SEPA CAMT.052 CAMT.053 CAMT.054
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 #############################
 Account Statement SEPA Module
 #############################
```

### Comparing `trytond_account_statement_sepa-6.6.1/account.py` & `trytond_account_statement_sepa-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/account.xml` & `trytond_account_statement_sepa-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/doc/conf.py` & `trytond_account_statement_sepa-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_statement_sepa-6.6.1/locale/bg.po` & `trytond_account_statement_sepa-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/ca.po` & `trytond_account_statement_sepa-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/cs.po` & `trytond_account_statement_sepa-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/de.po` & `trytond_account_statement_sepa-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/es.po` & `trytond_account_statement_sepa-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/es_419.po` & `trytond_account_statement_sepa-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/et.po` & `trytond_account_statement_sepa-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/fa.po` & `trytond_account_statement_sepa-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/fi.po` & `trytond_account_statement_sepa-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/fr.po` & `trytond_account_statement_sepa-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/hu.po` & `trytond_account_statement_sepa-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/id.po` & `trytond_account_statement_sepa-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/it.po` & `trytond_account_statement_sepa-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/lo.po` & `trytond_account_statement_sepa-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/lt.po` & `trytond_account_statement_sepa-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/nl.po` & `trytond_account_statement_sepa-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/pl.po` & `trytond_account_statement_sepa-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/pt.po` & `trytond_account_statement_sepa-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/ro.po` & `trytond_account_statement_sepa-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/ru.po` & `trytond_account_statement_sepa-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/sl.po` & `trytond_account_statement_sepa-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/tr.po` & `trytond_account_statement_sepa-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/uk.po` & `trytond_account_statement_sepa-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/locale/zh_CN.po` & `trytond_account_statement_sepa-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/setup.py` & `trytond_account_statement_sepa-6.8.0/setup.py`

 * *Files 11% similar despite different names*

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
@@ -37,62 +34,42 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_statement_sepa'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-
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
+
 requires = ['lxml']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module to import SEPA statements',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
             'https://docs.tryton.org/projects/modules-account-statement-sepa'),
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/account_statement_sepa',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account statement SEPA CAMT.052 CAMT.053 CAMT.054',
     package_dir={'trytond.modules.account_statement_sepa': '.'},
     packages=(
         ['trytond.modules.account_statement_sepa']
         + ['trytond.modules.account_statement_sepa.%s' % p
             for p in find_packages()]
@@ -130,27 +107,26 @@
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
     account_statement_sepa = trytond.modules.account_statement_sepa
     """,  # noqa: E501
     )
```

### Comparing `trytond_account_statement_sepa-6.6.1/tests/camt.053.001.02.xml` & `trytond_account_statement_sepa-6.8.0/tests/camt.053.001.02.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/tests/scenario_account_statement_sepa.rst` & `trytond_account_statement_sepa-6.8.0/tests/scenario_account_statement_sepa.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/PKG-INFO` & `trytond_account_statement_sepa-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-statement-sepa
-Version: 6.6.1
+Name: trytond_account_statement_sepa
+Version: 6.8.0
 Summary: Tryton module to import SEPA statements
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-statement-sepa
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement_sepa
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account statement SEPA CAMT.052 CAMT.053 CAMT.054
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
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
 
 #############################
 Account Statement SEPA Module
 #############################
```

### Comparing `trytond_account_statement_sepa-6.6.1/trytond_account_statement_sepa.egg-info/SOURCES.txt` & `trytond_account_statement_sepa-6.8.0/trytond_account_statement_sepa.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
```

