# Comparing `tmp/trytond_account_fr-6.6.1.tar.gz` & `tmp/trytond_account_fr-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_fr-6.6.1.tar", last modified: Sat Mar  4 12:20:54 2023, max compression
+gzip compressed data, was "trytond_account_fr-6.8.0.tar", last modified: Mon May  1 11:59:20 2023, max compression
```

## Comparing `trytond_account_fr-6.6.1.tar` & `trytond_account_fr-6.8.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:20:54.545413 trytond_account_fr-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2666 2023-03-04 12:20:49.000000 trytond_account_fr-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-03-04 12:20:48.000000 trytond_account_fr-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2939 2023-03-04 12:20:54.542080 trytond_account_fr-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14362 2023-02-27 17:57:43.000000 trytond_account_fr-6.6.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   436015 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/account_fr.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:20:54.532080 trytond_account_fr-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:20:54.515413 trytond_account_fr-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1473 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1435 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1377 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1435 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1328 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1242 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1403 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1286 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1420 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1339 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1324 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1385 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1332 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1296 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1203 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1314 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 12:20:54.545413 trytond_account_fr-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4428 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   194518 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tax_fr.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:20:54.525413 trytond_account_fr-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/FEC-previous.csv
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/FEC.csv
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6908 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/scenario_fec.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2482 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2022-12-19 12:03:07.000000 trytond_account_fr-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:20:54.542080 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2939 2023-03-04 12:20:53.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1620 2023-03-04 12:20:54.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:20:53.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-03-04 12:20:53.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 12:20:53.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-03-04 12:20:53.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 12:20:53.000000 trytond_account_fr-6.6.1/trytond_account_fr.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 12:20:54.528747 trytond_account_fr-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/view/fec_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2022-12-19 12:02:49.000000 trytond_account_fr-6.6.1/view/fec_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:20.195618 trytond_account_fr-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2728 2023-05-01 11:13:09.000000 trytond_account_fr-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-05-01 11:13:09.000000 trytond_account_fr-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_fr-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2950 2023-05-01 11:59:20.195618 trytond_account_fr-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14362 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   435827 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/account_fr.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:20.192284 trytond_account_fr-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:20.188951 trytond_account_fr-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1269 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1473 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1435 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1269 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1377 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1269 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1435 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1328 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1242 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1403 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1286 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1339 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1324 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1385 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1332 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1296 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1203 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1314 2023-04-29 08:02:49.000000 trytond_account_fr-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:59:20.195618 trytond_account_fr-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4378 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   194518 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tax_fr.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:20.192284 trytond_account_fr-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/FEC-previous.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/FEC.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6924 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/scenario_fec.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2481 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_fr-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-05-01 11:13:04.000000 trytond_account_fr-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:20.195618 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2950 2023-05-01 11:59:19.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1620 2023-05-01 11:59:20.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:59:19.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-05-01 11:59:19.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      100 2023-05-01 11:59:19.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:59:19.000000 trytond_account_fr-6.8.0/trytond_account_fr.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:20.192284 trytond_account_fr-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2023-01-16 14:00:20.000000 trytond_account_fr-6.8.0/view/fec_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:20.000000 trytond_account_fr-6.8.0/view/fec_start_form.xml
```

### Comparing `trytond_account_fr-6.6.1/CHANGELOG` & `trytond_account_fr-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_account_fr-6.6.1/COPYRIGHT` & `trytond_account_fr-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2010-2023 Cédric Krier.
 Copyright (C) 2010-2011 Bertrand Chenal.
-Copyright (C) 2010-2022 Nicolas Évrard.
+Copyright (C) 2010-2023 Nicolas Évrard.
 Copyright (C) 2010-2023 B2CK SPRL.
 Copyright (C) 2014-2018 Raphaël Hertzog.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_account_fr-6.6.1/LICENSE` & `trytond_account_fr-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/PKG-INFO` & `trytond_account_fr-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_fr
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with French chart of accounts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_fr
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart french fec
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,38 +38,38 @@
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
 
 French Account Module
 #####################
 
 The French account module defines the standard chart of account
 
 A wizard allows to generate the FEC file for a fiscal year.
 
 Configuration
 *************
 
-The account_fr module uses the section `account_fr` to retrieve some parameters:
+The account_fr module uses the section ``account_fr`` to retrieve some parameters:
 
-- `fec_opening_code`: defines the journal code for the opening balance in the
-  FEC file. The default value is `OUV`.
+- ``fec_opening_code``: defines the journal code for the opening balance in the
+  FEC file. The default value is ``OUV``.
 
-- `fec_opening_name`: defines the journal name for the opening balance in the
-  FEC file. The default value is `Balance Initiale`.
+- ``fec_opening_name``: defines the journal name for the opening balance in the
+  FEC file. The default value is ``Balance Initiale``.
 
-- `fec_opening_number`: defines the number of the opening balance in the FEC
-  file. The default value is `0`.
+- ``fec_opening_number``: defines the number of the opening balance in the FEC
+  file. The default value is ``0``.
```

### Comparing `trytond_account_fr-6.6.1/README.rst` & `trytond_account_fr-6.8.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 The French account module defines the standard chart of account
 
 A wizard allows to generate the FEC file for a fiscal year.
 
 Configuration
 *************
 
-The account_fr module uses the section `account_fr` to retrieve some parameters:
+The account_fr module uses the section ``account_fr`` to retrieve some parameters:
 
-- `fec_opening_code`: defines the journal code for the opening balance in the
-  FEC file. The default value is `OUV`.
+- ``fec_opening_code``: defines the journal code for the opening balance in the
+  FEC file. The default value is ``OUV``.
 
-- `fec_opening_name`: defines the journal name for the opening balance in the
-  FEC file. The default value is `Balance Initiale`.
+- ``fec_opening_name``: defines the journal name for the opening balance in the
+  FEC file. The default value is ``Balance Initiale``.
 
-- `fec_opening_number`: defines the number of the opening balance in the FEC
-  file. The default value is `0`.
+- ``fec_opening_number``: defines the number of the opening balance in the FEC
+  file. The default value is ``0``.
```

### Comparing `trytond_account_fr-6.6.1/__init__.py` & `trytond_account_fr-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/account.py` & `trytond_account_fr-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/account.xml` & `trytond_account_fr-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/account_fr.xml` & `trytond_account_fr-6.8.0/account_fr.xml`

 * *Files 0% similar despite different names*

#### Comparing `trytond_account_fr-6.6.1/account_fr.xml` & `trytond_account_fr-6.8.0/account_fr.xml`

```diff
@@ -4040,16 +4040,15 @@
       <field name="code">29755</field>
       <field name="type" ref="immobilisations_financieres_autres"/>
       <field name="parent" ref="2975"/>
     </record>
     <record model="account.account.template" id="2976">
       <field name="name">Autres créances immobilisées</field>
       <field name="code">2976</field>
-      <field name="type" ref="immobilisations_financieres_autres"/>
-      <field name="closed" eval="True"/>
+      <field name="type" eval="None"/>
       <field name="parent" ref="297"/>
     </record>
     <record model="account.account.template" id="29761">
       <field name="name">Créances diverses</field>
       <field name="code">29761</field>
       <field name="type" ref="immobilisations_financieres_autres"/>
       <field name="parent" ref="2976"/>
@@ -6011,16 +6010,15 @@
       <field name="type" ref="disponibilites"/>
       <field name="closed" eval="True"/>
       <field name="parent" ref="5"/>
     </record>
     <record model="account.account.template" id="59">
       <field name="name">Dépréciation des comptes financiers</field>
       <field name="code">59</field>
-      <field name="type" ref="actions_propres"/>
-      <field name="closed" eval="True"/>
+      <field name="type" eval="None"/>
       <field name="parent" ref="5"/>
     </record>
     <record model="account.account.template" id="590">
       <field name="name">Dépréciation des valeurs mobilières de placement</field>
       <field name="code">590</field>
       <field name="parent" ref="59"/>
     </record>
@@ -6313,16 +6311,15 @@
       <field name="name">Autres charges externes</field>
       <field name="code">61/62</field>
       <field name="parent" ref="6"/>
     </record>
     <record model="account.account.template" id="61">
       <field name="name">Services extérieurs</field>
       <field name="code">61</field>
-      <field name="type" ref="autres_achats"/>
-      <field name="closed" eval="True"/>
+      <field name="type" eval="None"/>
       <field name="parent" ref="61_62"/>
     </record>
     <record model="account.account.template" id="611">
       <field name="name">Sous-traitance générale</field>
       <field name="code">611</field>
       <field name="type" ref="autres_achats"/>
       <field name="parent" ref="61"/>
```

### Comparing `trytond_account_fr-6.6.1/doc/conf.py` & `trytond_account_fr-6.8.0/doc/conf.py`

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

### Comparing `trytond_account_fr-6.6.1/doc/index.rst` & `trytond_account_fr-6.8.0/doc/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 The French account module defines the standard chart of account
 
 A wizard allows to generate the FEC file for a fiscal year.
 
 Configuration
 *************
 
-The account_fr module uses the section `account_fr` to retrieve some parameters:
+The account_fr module uses the section ``account_fr`` to retrieve some parameters:
 
-- `fec_opening_code`: defines the journal code for the opening balance in the
-  FEC file. The default value is `OUV`.
+- ``fec_opening_code``: defines the journal code for the opening balance in the
+  FEC file. The default value is ``OUV``.
 
-- `fec_opening_name`: defines the journal name for the opening balance in the
-  FEC file. The default value is `Balance Initiale`.
+- ``fec_opening_name``: defines the journal name for the opening balance in the
+  FEC file. The default value is ``Balance Initiale``.
 
-- `fec_opening_number`: defines the number of the opening balance in the FEC
-  file. The default value is `0`.
+- ``fec_opening_number``: defines the number of the opening balance in the FEC
+  file. The default value is ``0``.
```

### Comparing `trytond_account_fr-6.6.1/locale/bg.po` & `trytond_account_fr-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/ca.po` & `trytond_account_fr-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/cs.po` & `trytond_account_fr-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/de.po` & `trytond_account_fr-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/es.po` & `trytond_account_fr-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/es_419.po` & `trytond_account_fr-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/et.po` & `trytond_account_fr-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/fa.po` & `trytond_account_fr-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/fi.po` & `trytond_account_fr-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/fr.po` & `trytond_account_fr-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/hu.po` & `trytond_account_fr-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/id.po` & `trytond_account_fr-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/it.po` & `trytond_account_fr-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/lo.po` & `trytond_account_fr-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/lt.po` & `trytond_account_fr-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/nl.po` & `trytond_account_fr-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/pl.po` & `trytond_account_fr-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/pt.po` & `trytond_account_fr-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/ro.po` & `trytond_account_fr-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/ru.po` & `trytond_account_fr-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/sl.po` & `trytond_account_fr-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/tr.po` & `trytond_account_fr-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/uk.po` & `trytond_account_fr-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/locale/zh_CN.po` & `trytond_account_fr-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/setup.py` & `trytond_account_fr-6.8.0/setup.py`

 * *Files 5% similar despite different names*

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
 name = 'trytond_account_fr'
 
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
 
-tests_require = [get_require_version('proteus'), 'python-dateutil']
+tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module with French chart of accounts',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_fr',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account chart french fec',
     package_dir={'trytond.modules.account_fr': '.'},
     packages=(
         ['trytond.modules.account_fr']
         + ['trytond.modules.account_fr.%s' % p for p in find_packages()]
         ),
@@ -102,24 +102,24 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_account_fr-6.6.1/tax_fr.xml` & `trytond_account_fr-6.8.0/tax_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/tests/FEC.csv` & `trytond_account_fr-6.8.0/tests/FEC.csv`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/tests/scenario_fec.rst` & `trytond_account_fr-6.8.0/tests/scenario_fec.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 ============
 FEC Scenario
 ============
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> import os
     >>> import io
     >>> from decimal import Decimal
-    >>> from dateutil.relativedelta import relativedelta
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear
     >>> from trytond.modules.account_fr.tests.tools import create_chart, \
     ...     get_accounts
 
-    >>> today = datetime.date(2018, 1, 1)
-
 Activate modules::
 
     >>> config = activate_modules('account_fr')
 
 Create company::
 
     >>> _ = create_company()
@@ -30,21 +27,22 @@
     >>> siren = company.party.identifiers.new(type='fr_siren')
     >>> siren.code = '820043784'
     >>> company.party.save()
 
 Create last year fiscal year::
 
     >>> fiscalyear_previous = create_fiscalyear(
-    ...     company, today=today - relativedelta(years=1))
+    ...     company, (dt.date(2017, 1, 1), dt.date(2017, 12, 31)))
     >>> fiscalyear_previous.click('create_period')
     >>> period_previous = fiscalyear_previous.periods[0]
 
 Create fiscal year::
 
-    >>> fiscalyear = create_fiscalyear(company, today=today)
+    >>> fiscalyear = create_fiscalyear(
+    ...     company, (dt.date(2018, 1, 1), dt.date(2018, 12, 31)))
     >>> fiscalyear.click('create_period')
     >>> period = fiscalyear.periods[0]
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
@@ -149,14 +147,15 @@
     ...         }, config.context)
     >>> move.click('post')
     >>> reconcile2, = [l for l in move.lines if l.account == receivable]
     >>> reconcile_lines = Wizard('account.move.reconcile_lines',
     ...     [reconcile1, reconcile2])
     >>> reconcile_lines.state == 'end'
     True
+    >>> reconcile_date = reconcile1.reconciliation.create_date
 
 Balance non-deferral::
 
     >>> Sequence = Model.get('ir.sequence')
     >>> Period = Model.get('account.period')
     >>> Account = Model.get('account.account')
 
@@ -193,15 +192,15 @@
     >>> FEC.form.fiscalyear = fiscalyear
     >>> FEC.form.deferral_period = period_closing
     >>> FEC.execute('generate')
     >>> FEC.form.filename
     >>> file = os.path.join(os.path.dirname(__file__), 'FEC.csv')
     >>> with io.open(file, mode='rb') as fp:
     ...     template = fp.read().decode('utf-8')
-    >>> current_date = datetime.date.today().strftime('%Y%m%d')
+    >>> current_date = reconcile_date.strftime('%Y%m%d')
     >>> template = template.format(
     ...         current_date=current_date,
     ...         )
     >>> FEC.form.file.decode('utf-8') == template
     True
 
 Generate FEC for previous fiscal year::
```

### Comparing `trytond_account_fr-6.6.1/tests/test_module.py` & `trytond_account_fr-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_fr-6.6.1/tests/tools.py` & `trytond_account_fr-6.8.0/tests/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model, Wizard
-
 from trytond.modules.company.tests.tools import get_company
 
 __all__ = ['create_chart', 'get_accounts']
 
 
 def create_chart(company=None, config=None):
     "Create chart of accounts"
```

### Comparing `trytond_account_fr-6.6.1/trytond_account_fr.egg-info/PKG-INFO` & `trytond_account_fr-6.8.0/trytond_account_fr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-fr
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with French chart of accounts
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_fr
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart french fec
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,38 +38,38 @@
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
 
 French Account Module
 #####################
 
 The French account module defines the standard chart of account
 
 A wizard allows to generate the FEC file for a fiscal year.
 
 Configuration
 *************
 
-The account_fr module uses the section `account_fr` to retrieve some parameters:
+The account_fr module uses the section ``account_fr`` to retrieve some parameters:
 
-- `fec_opening_code`: defines the journal code for the opening balance in the
-  FEC file. The default value is `OUV`.
+- ``fec_opening_code``: defines the journal code for the opening balance in the
+  FEC file. The default value is ``OUV``.
 
-- `fec_opening_name`: defines the journal name for the opening balance in the
-  FEC file. The default value is `Balance Initiale`.
+- ``fec_opening_name``: defines the journal name for the opening balance in the
+  FEC file. The default value is ``Balance Initiale``.
 
-- `fec_opening_number`: defines the number of the opening balance in the FEC
-  file. The default value is `0`.
+- ``fec_opening_number``: defines the number of the opening balance in the FEC
+  file. The default value is ``0``.
```

### Comparing `trytond_account_fr-6.6.1/trytond_account_fr.egg-info/SOURCES.txt` & `trytond_account_fr-6.8.0/trytond_account_fr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

