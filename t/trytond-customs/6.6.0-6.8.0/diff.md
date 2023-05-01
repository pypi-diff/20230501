# Comparing `tmp/trytond_customs-6.6.0.tar.gz` & `tmp/trytond_customs-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_customs-6.6.0.tar", last modified: Mon Oct 31 15:52:22 2022, max compression
+gzip compressed data, was "trytond_customs-6.8.0.tar", last modified: Mon May  1 12:04:47 2023, max compression
```

## Comparing `trytond_customs-6.6.0.tar` & `trytond_customs-6.8.0.tar`

### file list

```diff
@@ -1,68 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:22.483836 trytond_customs-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_customs-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_customs-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      705 2022-10-31 15:52:21.000000 trytond_customs-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_customs-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2022-10-31 15:52:20.000000 trytond_customs-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:52:20.000000 trytond_customs-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_customs-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2022-10-31 15:52:22.483836 trytond_customs-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      774 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2021-12-11 16:59:33.000000 trytond_customs-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6673 2022-10-11 19:49:57.000000 trytond_customs-6.6.0/customs.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4350 2021-02-27 17:17:01.000000 trytond_customs-6.6.0/customs.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:22.483836 trytond_customs-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      774 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:22.480502 trytond_customs-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7343 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7496 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6878 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7450 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7603 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6972 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7211 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8019 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6810 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7516 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7169 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6776 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7510 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7416 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7200 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7487 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7218 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7592 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6797 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7400 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7607 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6810 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6483 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6954 2022-10-29 07:50:45.000000 trytond_customs-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6878 2022-10-11 19:49:57.000000 trytond_customs-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1638 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:52:22.483836 trytond_customs-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5031 2022-10-29 07:39:10.000000 trytond_customs-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:22.480502 trytond_customs-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_customs-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7306 2022-04-16 16:30:56.000000 trytond_customs-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2022-10-31 15:10:09.000000 trytond_customs-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      121 2022-10-31 15:52:19.000000 trytond_customs-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:22.483836 trytond_customs-6.6.0/trytond_customs.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2022-10-31 15:52:21.000000 trytond_customs-6.6.0/trytond_customs.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2022-10-31 15:52:22.000000 trytond_customs-6.6.0/trytond_customs.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:52:21.000000 trytond_customs-6.6.0/trytond_customs.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2022-10-31 15:52:21.000000 trytond_customs-6.6.0/trytond_customs.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:14.000000 trytond_customs-6.6.0/trytond_customs.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      124 2022-10-31 15:52:21.000000 trytond_customs-6.6.0/trytond_customs.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:52:21.000000 trytond_customs-6.6.0/trytond_customs.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:22.483836 trytond_customs-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      869 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/view/duty_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2019-10-11 23:09:47.000000 trytond_customs-6.6.0/view/duty_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/view/product-tariff_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2019-10-11 23:09:47.000000 trytond_customs-6.6.0/view/product-tariff_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2019-10-11 23:09:47.000000 trytond_customs-6.6.0/view/product-tariff_code_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2018-08-18 09:54:37.000000 trytond_customs-6.6.0/view/tariff_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2019-10-11 23:09:47.000000 trytond_customs-6.6.0/view/tariff_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2021-10-30 15:32:31.000000 trytond_customs-6.6.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:47.109674 trytond_customs-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-05-01 11:17:01.000000 trytond_customs-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:17:01.000000 trytond_customs-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_customs-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3124 2023-05-01 12:04:47.109674 trytond_customs-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8774 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/customs.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4350 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/customs.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:47.106341 trytond_customs-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:47.103008 trytond_customs-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6467 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6507 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5902 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6451 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6606 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5979 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6150 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6911 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5817 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6519 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6192 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5712 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6449 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6570 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6138 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6493 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6133 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6535 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5647 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6533 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6568 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5817 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5490 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5982 2023-04-30 10:46:36.000000 trytond_customs-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7927 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1638 2023-01-16 14:00:20.000000 trytond_customs-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:04:47.109674 trytond_customs-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4227 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:47.103008 trytond_customs-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9525 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      121 2023-05-01 11:16:55.000000 trytond_customs-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:47.109674 trytond_customs-6.8.0/trytond_customs.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3124 2023-05-01 12:04:46.000000 trytond_customs-6.8.0/trytond_customs.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-05-01 12:04:47.000000 trytond_customs-6.8.0/trytond_customs.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:04:46.000000 trytond_customs-6.8.0/trytond_customs.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2023-05-01 12:04:46.000000 trytond_customs-6.8.0/trytond_customs.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_customs-6.8.0/trytond_customs.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      124 2023-05-01 12:04:46.000000 trytond_customs-6.8.0/trytond_customs.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:04:46.000000 trytond_customs-6.8.0/trytond_customs.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:47.106341 trytond_customs-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-01-16 14:00:20.000000 trytond_customs-6.8.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      890 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/duty_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/duty_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_customs-6.8.0/view/product-tariff_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/product-tariff_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/product-tariff_code_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/tariff_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/tariff_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_customs-6.8.0/view/template_form.xml
```

### Comparing `trytond_customs-6.6.0/COPYRIGHT` & `trytond_customs-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2015-2022 Cédric Krier.
-Copyright (C) 2015-2022 B2CK SPRL.
+Copyright (C) 2015-2023 Cédric Krier.
+Copyright (C) 2015-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_customs-6.6.0/LICENSE` & `trytond_customs-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_customs-6.6.0/PKG-INFO` & `trytond_customs-6.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_customs
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for customs
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
-Project-URL: Source Code, https://hg.tryton.org/modules/customs
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton customs tariff duty
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
 License-File: LICENSE
 
 Customs Module
 ##############
 
 The customs module allows to define customs duty based on the tariff code.
 
@@ -61,23 +61,25 @@
 Tarif Code
 **********
 
 It stores the `Harmonized System`_ that can be set on *Product*.
 
 - The *Code* from the HS.
 - The *Country* in case of a country specific code.
+- The *Organization* in case of a country organization code.
 - The *Start* / *End* period of the year for which the code is valid.
 
 .. _`Harmonized System`: http://en.wikipedia.org/wiki/Harmonized_System
 
 Duty Rate
 *********
 
 It stores the rate of a *Tarif Code* for a country over a period.
 
 - The *Tariff Code*.
 - The *Country* for which the rate is.
+- The *Organization* for which the rate is.
 - The *Type*: *Import* or *Export*
 - The *Start* and *End* date of validity.
 - The *Computation Type*:
     - *Amount*: fixed amount with currency.
     - *Quantity*: amount (in currency) per unit of measure.
```

### Comparing `trytond_customs-6.6.0/README.rst` & `trytond_customs-6.8.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 Tarif Code
 **********
 
 It stores the `Harmonized System`_ that can be set on *Product*.
 
 - The *Code* from the HS.
 - The *Country* in case of a country specific code.
+- The *Organization* in case of a country organization code.
 - The *Start* / *End* period of the year for which the code is valid.
 
 .. _`Harmonized System`: http://en.wikipedia.org/wiki/Harmonized_System
 
 Duty Rate
 *********
 
 It stores the rate of a *Tarif Code* for a country over a period.
 
 - The *Tariff Code*.
 - The *Country* for which the rate is.
+- The *Organization* for which the rate is.
 - The *Type*: *Import* or *Export*
 - The *Start* and *End* date of validity.
 - The *Computation Type*:
     - *Amount*: fixed amount with currency.
     - *Quantity*: amount (in currency) per unit of measure.
```

### Comparing `trytond_customs-6.6.0/customs.py` & `trytond_customs-6.8.0/customs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,158 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 from decimal import Decimal
 
 from sql import Null
 
+from trytond import backend
 from trytond.model import (
     DeactivableMixin, MatchMixin, ModelSQL, ModelView, fields)
 from trytond.modules.product import price_digits
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
+from trytond.transaction import Transaction
 
-# Use 2 chars numbering to allow string comparison
-MONTHS = [
-    (None, ''),
-    ('01', 'January'),
-    ('02', 'February'),
-    ('03', 'March'),
-    ('04', 'April'),
-    ('05', 'May'),
-    ('06', 'June'),
-    ('07', 'July'),
-    ('08', 'August'),
-    ('09', 'September'),
-    ('10', 'October'),
-    ('11', 'November'),
-    ('12', 'December'),
-    ]
 
+class CountryMatchMixin(MatchMixin):
+    country = fields.Many2One(
+        'country.country', "Country",
+        states={
+            'invisible': Bool(Eval('organization')),
+            })
+    organization = fields.Many2One(
+        'country.organization', "Organization",
+        states={
+            'invisible': Bool(Eval('country')),
+            })
+
+    def match(self, pattern, match_none=False):
+        if 'country' in pattern:
+            pattern = pattern.copy()
+            country = pattern.pop('country')
+            if country is not None or match_none:
+                if self.country and self.country.id != country:
+                    return False
+                if (self.organization
+                        and country not in [
+                            c.id for c in self.organization.countries]):
+                    return False
+        return super().match(pattern, match_none=match_none)
 
-class TariffCode(DeactivableMixin, ModelSQL, ModelView, MatchMixin):
+
+class TariffCode(DeactivableMixin, CountryMatchMixin, ModelSQL, ModelView):
     'Tariff Code'
     __name__ = 'customs.tariff.code'
     _rec_name = 'code'
     code = fields.Char('Code', required=True,
         help='The code from Harmonized System of Nomenclature.')
     description = fields.Char('Description', translate=True)
     country = fields.Many2One('country.country', 'Country')
     # TODO country group
-    start_month = fields.Selection(MONTHS, 'Start Month', sort=False,
+    start_month = fields.Many2One('ir.calendar.month', "Start Month",
         states={
             'required': Eval('end_month') | Eval('start_day'),
             })
     start_day = fields.Integer('Start Day',
         domain=['OR',
-            ('start_day', '<=', If(Eval('start_month').in_(
-                        ['01', '03', '05', '07', '08', '10', '12']), 31,
-                    If(Eval('start_month') == '02', 29, 30))),
             ('start_day', '=', None),
+            [('start_day', '>=', 1), ('start_day', '<=', 31)],
             ],
         states={
             'required': Bool(Eval('start_month')),
             })
-    end_month = fields.Selection(MONTHS, 'End Month', sort=False,
+    end_month = fields.Many2One('ir.calendar.month', "End Month",
         states={
             'required': Eval('start_month') | Eval('end_day'),
             })
     end_day = fields.Integer('End Day',
         domain=['OR',
-            ('end_day', '<=', If(Eval('end_month').in_(
-                        ['01', '03', '05', '07', '08', '10', '12']), 31,
-                    If(Eval('end_month') == '02', 29, 30))),
             ('end_day', '=', None),
+            [('end_day', '>=', 1), ('end_day', '<=', 31)],
             ],
         states={
             'required': Bool(Eval('end_month')),
             })
     duty_rates = fields.One2Many('customs.duty.rate', 'tariff_code',
         'Duty Rates')
 
     @classmethod
     def __setup__(cls):
         super(TariffCode, cls).__setup__()
         cls._order.insert(0, ('code', 'ASC'))
 
-    def match(self, pattern):
+    @classmethod
+    def __register__(cls, module_name):
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
+        pool = Pool()
+        Month = pool.get('ir.calendar.month')
+        sql_table = cls.__table__()
+        month = Month.__table__()
+        table_h = cls.__table_handler__(module_name)
+
+        # Migration from 6.6: use ir.calendar
+        migrate_calendar = False
+        if (backend.TableHandler.table_exist(cls._table)
+                and table_h.column_exist('start_month')
+                and table_h.column_exist('end_month')):
+            migrate_calendar = (
+                table_h.column_is_type('start_month', 'VARCHAR')
+                or table_h.column_is_type('end_month', 'VARCHAR'))
+            if migrate_calendar:
+                table_h.column_rename('start_month', '_temp_start_month')
+                table_h.column_rename('end_month', '_temp_end_month')
+
+        super().__register__(module_name)
+
+        table_h = cls.__table_handler__(module_name)
+
+        # Migration from 6.6: use ir.calendar
+        if migrate_calendar:
+            update = transaction.connection.cursor()
+            cursor.execute(*month.select(month.id, month.index))
+            for month_id, index in cursor:
+                str_index = f'{index:02d}'
+                update.execute(*sql_table.update(
+                        [sql_table.start_month], [month_id],
+                        where=sql_table._temp_start_month == str_index))
+                update.execute(*sql_table.update(
+                        [sql_table.end_month], [month_id],
+                        where=sql_table._temp_end_month == str_index))
+            table_h.drop_column('_temp_start_month')
+            table_h.drop_column('_temp_end_month')
+
+    def match(self, pattern, match_none=False):
         if 'date' in pattern:
             pattern = pattern.copy()
             date = pattern.pop('date')
             if self.start_month and self.end_month:
-                start = (int(self.start_month), self.start_day)
-                end = (int(self.end_month), self.end_day)
+                start = (self.start_month.index, self.start_day)
+                end = (self.end_month.index, self.end_day)
                 date = (date.month, date.day)
                 if start <= end:
                     if not (start <= date <= end):
                         return False
                 else:
                     if end <= date <= start:
                         return False
-        return super(TariffCode, self).match(pattern)
+        return super().match(pattern, match_none=match_none)
 
     def get_duty_rate(self, pattern):
         for rate in self.duty_rates:
             if rate.match(pattern):
                 return rate
 
 
-class DutyRate(ModelSQL, ModelView, MatchMixin):
+class DutyRate(CountryMatchMixin, ModelSQL, ModelView):
     'Duty Rate'
     __name__ = 'customs.duty.rate'
     tariff_code = fields.Many2One(
         'customs.tariff.code', "Tariff Code", required=True)
-    country = fields.Many2One('country.country', 'Country')
-    # TODO country group
     type = fields.Selection([
             ('import', 'Import'),
             ('export', 'Export'),
             ], 'Type')
     start_date = fields.Date('Start Date',
         domain=['OR',
             ('start_date', '<=', If(Bool(Eval('end_date')),
```

### Comparing `trytond_customs-6.6.0/customs.xml` & `trytond_customs-6.8.0/customs.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-6.6.0/doc/index.rst` & `trytond_customs-6.8.0/doc/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 Tarif Code
 **********
 
 It stores the `Harmonized System`_ that can be set on *Product*.
 
 - The *Code* from the HS.
 - The *Country* in case of a country specific code.
+- The *Organization* in case of a country organization code.
 - The *Start* / *End* period of the year for which the code is valid.
 
 .. _`Harmonized System`: http://en.wikipedia.org/wiki/Harmonized_System
 
 Duty Rate
 *********
 
 It stores the rate of a *Tarif Code* for a country over a period.
 
 - The *Tariff Code*.
 - The *Country* for which the rate is.
+- The *Organization* for which the rate is.
 - The *Type*: *Import* or *Export*
 - The *Start* and *End* date of validity.
 - The *Computation Type*:
     - *Amount*: fixed amount with currency.
     - *Quantity*: amount (in currency) per unit of measure.
```

### Comparing `trytond_customs-6.6.0/locale/bg.po` & `trytond_customs-6.8.0/locale/ro.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,356 +1,270 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Сума"
+msgstr "Suma"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Държава"
+msgstr "Țară"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Управление на валути"
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Крайна дата"
+msgstr ""
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Начална дата"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Вид"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Мерни единици"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Код"
+msgstr "Cod"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Държава"
+msgstr "Țară"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Описание"
+msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Крайна дата"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Начална дата"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Țară"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Продукт"
+msgstr "Produs"
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Customs"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Държава"
+msgstr "Țară"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Държава"
+msgstr "Țară"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Duty Rates"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Извличане"
+msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
 msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Customs Administration"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Сума"
+msgstr "Suma"
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Количество"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Извличане"
+msgstr "Export"
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr ""
-
-#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Категория мер. ед."
+msgstr "Categorie"
 
-#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Шаблон"
+msgstr "Șablon"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr ""
+msgstr "Calcul"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr ""
+msgstr "De la"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr ""
+msgstr "La"
 
-#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
 
-#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Customs"
+msgstr "Vamă"
```

### Comparing `trytond_customs-6.6.0/locale/ca.po` & `trytond_customs-6.8.0/locale/id.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,323 +1,273 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Jumlah"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Tipus de càlcul"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Negara"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Mata uang"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Data final"
+msgstr "Tanggal Akhir"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Data inicial"
+msgstr "Tanggal Awal"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Codi aranzelari"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Tipus"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "UdM"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Codi"
+msgstr "Kode"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Negara"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Descripció"
+msgstr "Deskripsi"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Tarifa aranzelaria"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Dia final"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Mes final"
+msgstr ""
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Data inicial"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Mes inicial"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Negara"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Tanggal Akhir"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Producte"
+msgstr "Produk"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Tanggal Awal"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Tanggal Awal"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Codi aranzelari"
+msgstr ""
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Duanes"
+msgstr ""
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codis aranzelaris"
+msgstr ""
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Usa els codis aranzelaris del pare"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "País"
+msgstr "Negara"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Categoria de duanes"
+msgstr ""
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codis aranzelaris"
+msgstr ""
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Usa els codis aranzelaris de la categoria"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "País"
+msgstr "Negara"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Categoria de duanes"
+msgstr ""
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codis aranzelaris"
+msgstr ""
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Usa els codis aranzelaris de la categoria"
+msgstr ""
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr "El codi del Sistema Harmonitzat de designació."
+msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Utilitza els codis aranzelaris definits a la categoria pare."
+msgstr ""
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilitza els codis aranzelaris definits a la categoria."
+msgstr ""
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilitza els codis aranzelaris definits a la categoria."
+msgstr ""
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Taxa d'aranzel"
+msgstr ""
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Codi aranzelari"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Taxes d'aranzel"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Codis d'aranzel"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Exportacions"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Importacions"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Duanes"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Taxes d'aranzel"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Codis d'aranzel"
+msgstr ""
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Producte - Codi aranzelari"
+msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Administració de duanes"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Import"
+msgstr "Jumlah"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Quantitat"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exportació"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importació"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Abril"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Agost"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Desembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Febrer"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Gener"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Juliol"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Juny"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Març"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Maig"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Novembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Octubre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Setembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Abril"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Agost"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Desembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Febrer"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Gener"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Juliol"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Juny"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Març"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Maig"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Novembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Octubre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Setembre"
+msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Categoria"
+msgstr "Kategori"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Plantilla"
+msgstr "Templat"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Càlcul"
+msgstr "Perhitungan"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Des de"
+msgstr "Dari"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Fins"
+msgstr "Kepada"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Duanes"
+msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Duanes"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-6.6.0/locale/de.po` & `trytond_customs-6.8.0/locale/hu.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,325 +1,294 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Betrag"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Berechnungstyp"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Land"
+msgstr "Ország"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Währung"
+msgstr "Pénznem"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Enddatum"
+msgstr ""
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Startdatum"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Zolltarifnummer"
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "Típus"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Maßeinheit"
+msgstr "Egység"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Code"
+msgstr "Partner kód"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Land"
+msgstr "Ország"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Beschreibung"
+msgstr "Leírás"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Zolltarife"
+msgstr "Duty Rates"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Endtag"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Endmonat"
+msgstr ""
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Anfangstag"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Anfangsmonat"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Ország"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Artikel"
+msgstr "Termék"
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
 
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Zolltarifnummer"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Zoll"
+msgstr "Külkereskedelmi"
 
+#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Zolltarifnummern"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Zolltarifnummern der übergeordneten Kategorie anwenden"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Land"
+msgstr "Ország"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Zollkategorie"
+msgstr "Külkereskedelmi kategória"
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Zolltarifnummern"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Zolltarifnummern der Kategorie anwenden"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Land"
+msgstr "Ország"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Zollkategorie"
+msgstr "Külkereskedelmi kategória"
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Zolltarifnummern"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Zolltarifnummern der Kategorie anwenden"
+msgstr ""
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
-"Code des Harmonisierten Systems zur Bezeichnung und Codierung von Waren (HS "
-"Nomenklatur)."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Zolltarifnummern der übergeordneten Kategorie anwenden."
+msgstr ""
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Zolltarifnummern der Kategorie anwenden."
+msgstr ""
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Zolltarifnummern der Kategorie anwenden."
+msgstr ""
 
+#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Zolltarif"
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Zolltarifnummer"
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Zolltarife"
+msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Zolltarifnummern"
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Export"
+msgstr "Exportálás"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Zoll"
+msgstr "Külkereskedelem"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Zolltarife"
+msgstr "Duty Rates"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Zolltarifnummern"
+msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Artikel - Zolltarifnummer"
+msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Zoll Administration"
+msgstr "Customs Administration"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Betrag"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Menge"
+msgstr "Mennyiség"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Export"
+msgstr "Exportálás"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "August"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Dezember"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Februar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Januar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Juli"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Juni"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "März"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Mai"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "September"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "August"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Dezember"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Februar"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Januar"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Juli"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Juni"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "März"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Mai"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "September"
-
+#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategorie"
+msgstr "Kategória"
 
+#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Artikelvorlage"
+msgstr "Űrlap adószámlához"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Berechnung"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Von"
+msgstr "-tól; től"
 
+#, fuzzy
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Bis"
+msgstr "-hoz; -höz"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Zoll"
+msgstr "Külkereskedelem"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Zoll"
+msgstr "Külkereskedelem"
```

### Comparing `trytond_customs-6.6.0/locale/es.po` & `trytond_customs-6.8.0/locale/it.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,323 +1,272 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Importo"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Tipo de cálculo"
+msgstr "tipo calcolo"
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Paese"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Valuta"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Fecha final"
+msgstr "Data finale"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Fecha inicial"
+msgstr "Data iniziale"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Código arancelario"
+msgstr "Codice dazio"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
 msgstr "Tipo"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
 msgstr "UdM"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Codice"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Paese"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Descripción"
+msgstr "Descrizione"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Tasas de arancel"
+msgstr "aliquote dazio"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Día final"
+msgstr "Data finale"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Mes final"
+msgstr "fine mese"
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Día inicial"
+msgstr "Data iniziale"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Mes inicial"
+msgstr "mese iniziale"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Paese"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Data finale"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "fine mese"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Producto"
+msgstr "Prodotto"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Data iniziale"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "mese iniziale"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Código arancelario"
+msgstr "Codice doganale"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Aduanas"
+msgstr "Dogane"
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Códigos arancelarios"
+msgstr "Codici doganali"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Usar los códigos arancelarios del padre"
+msgstr "usare il codice tariffario del padre"
 
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "País"
+msgstr "Paese"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Categoría de aduanas"
+msgstr "categoria doganale"
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Códigos arancelarios"
+msgstr "Codici doganali"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Usar los códigos arancelarios de la categoría"
+msgstr "usare i codici tariffari della categoria"
 
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "País"
+msgstr "Paese"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Categoría de aduanas"
+msgstr "categoria doganale"
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Códigos arancelarios"
+msgstr "Codici doganali"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Usar los códigos arancelarios de la categoría"
+msgstr "usare i codici tariffari della categoria"
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr "El código del sistema armonizado de nomenclatura."
+msgstr "Il codice del sistema di nomenclatura armonizzato."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Usar los códigos arancelarios definidos en la categoría padre."
+msgstr "Utilizzare i codici doganali definiti nella categoria del padre."
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Usar los códigos arancelarios definidos en la categoría."
+msgstr "Utilizzare i codici diganali definiti nella categoria."
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Usar los códigos arancelarios definidos en la categoría."
+msgstr "Utilizzare i codici doganali definiti nella categoria del padre."
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Tasa de arancel"
+msgstr "aliquota dazio"
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Código arancelario"
+msgstr "Codice dazio"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Tasas de arancel"
+msgstr "Aliquote dazi"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Códigos arancelarios"
+msgstr "Codici doganali"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Exportaciones"
+msgstr "Esportazione"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Importaciones"
+msgstr "Importazione"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Aduanas"
+msgstr "Dogane"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Tasas de arancel"
+msgstr "Aliquote dazi"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Códigos arancelarios"
+msgstr "Codici doganali"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Producto - Código arancelario"
+msgstr "prodotto - codice tariffario"
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Administración de aduanas"
+msgstr "Amministrazione dogane"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Importe"
+msgstr "Importo"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Cantidad"
+msgstr "Quantità"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exportación"
+msgstr "Esportazione"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importación"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Abril"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Agosto"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Diciembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Febrero"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Enero"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Julio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Junio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Marzo"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Mayo"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Noviembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Octubre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Septiembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Abril"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Agosto"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Diciembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Febrero"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Enero"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Julio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Junio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Marzo"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Mayo"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Noviembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Octubre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Septiembre"
+msgstr "Importazione"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Categoría"
+msgstr "Categoria"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Plantilla"
+msgstr "esempio"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Cálculo"
+msgstr "calcolo"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Desde"
+msgstr "Da"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Hasta"
+msgstr "a"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Aduanas"
+msgstr "dogane"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Aduanas"
+msgstr "dogane"
```

### Comparing `trytond_customs-6.6.0/locale/es_419.po` & `trytond_customs-6.8.0/locale/uk.po`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
 msgstr ""
 
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
 msgstr ""
@@ -48,51 +52,79 @@
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Tasas de aduana"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
 msgstr ""
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
 msgstr ""
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
 msgstr ""
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Utilizar los códigos arancelarios del padre"
+msgstr ""
 
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
 msgstr ""
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
@@ -100,15 +132,15 @@
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
 msgstr ""
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Utilizar los códigos arancelarios de la categoría"
+msgstr ""
 
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
 msgstr ""
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
@@ -116,70 +148,71 @@
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
 msgstr ""
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Utilizar los códigos arancelarios de la categoría"
+msgstr ""
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Utilizar los códigos arancelarios definidos en la categoría padre"
+msgstr ""
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilizar los códigos arancelarios definidos en la categoría"
+msgstr ""
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilizar los códigos arancelarios definidos en la categoría"
+msgstr ""
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Tasa de aduana"
+msgstr ""
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Tasas de aduana"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Exportar"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Importar"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Tasas de aduana"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
 msgstr ""
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
@@ -195,114 +228,18 @@
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exportar"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
 msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
 msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-6.6.0/locale/et.po` & `trytond_customs-6.8.0/locale/cs.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,325 +1,285 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Väärtus"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Arvutuse tüüp"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Riik"
+msgstr "Coventry"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Valuuta"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Lõppkuupäev"
+msgstr ""
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Alguskuupäev"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariifi kood"
+msgstr "Tariff Codes"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Tüüp"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Mõõtühik"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Kood"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Riik"
+msgstr "Coventry"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Selgitus"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Maksumäär"
+msgstr "Duty Rates"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Lõppkuupäev"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Lõppkuu"
+msgstr ""
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Alguskuupäev"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Alguskuu"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Coventry"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Toode"
+msgstr ""
 
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariifi kood"
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Toll"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariifi koodid"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Kasuta ülema jaotuse tariifi koodi"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Riik"
+msgstr "Coventry"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Tolli kategooria"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariifi koodid"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Kasuta kategooria tariifi koode"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Riik"
+msgstr "Coventry"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Tolli kategooria"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariifi koodid"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Kasuta kategooria tariifi koode"
+msgstr ""
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Tasu määr"
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tariifi kood"
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Tasu määr"
+msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariifi kood"
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Eksport"
+msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Toll"
+msgstr "Customs"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Maksumäär"
+msgstr "Duty Rates"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariifi kood"
+msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Toode - tariifi kood"
+msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Tolli administreerimine"
+msgstr "Customs Administration"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Väärtus"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Kogus"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Eksport"
+msgstr "Export"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Aprill"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "August"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Detsember"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Veebruar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Jaanuar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Juuli"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Juuni"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Märts"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Mai"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Oktoober"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "September"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "aprill"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "August"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Detsember"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Veebruar"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Jaanuar"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Juuli"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Juuni"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Märts"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Mai"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Noveber"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Oktoober"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "September"
-
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategooria"
+msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Mall"
+msgstr ""
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
 msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Kellelt"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Kellele"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Toll"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Toll"
+msgstr "Customs"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-6.6.0/locale/fa.po` & `trytond_customs-6.8.0/locale/fa.po`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 msgid "Currency"
 msgstr "واحد پول"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
 msgstr "تاریخ پایان"
 
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
 msgstr "تاریخ شروع"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
 msgstr "کد تعرفه"
@@ -58,26 +62,59 @@
 msgid "End Day"
 msgstr "پایان روز"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr "پایان ماه"
 
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr "شروع روز"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr "شروع ماه"
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "کشور"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "پایان روز"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "پایان ماه"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
 msgstr "محصول"
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "شروع روز"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "شروع ماه"
+
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
 msgstr "کد تعرفه"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
 msgstr "گمرک"
@@ -130,19 +167,27 @@
 msgstr "کد از سیستم هماهنگ نامگذاری،فهرست و اضطلاحات"
 
 #, fuzzy
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr "استفاده از کدهای تعرفه تعریف شده در رده مرجع"
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr "استفاده از کدهای تعرفه تعریف شده در دسته بندی"
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 #, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr "استفاده از کدهای تعرفه تعریف شده در دسته بندی"
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
@@ -200,110 +245,14 @@
 msgid "Export"
 msgstr "صادرات"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "واردات"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "آوریل"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "اوت"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "دسامبر"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "فوریه"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "ژانویه"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "جولای"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "ژوئن"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "مارس"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "می"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "نوامبر"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "اکتبر"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "سپتامبر"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "آوریل"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "اوت"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "دسامبر"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "فوریه"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "ژانویه"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "جولای"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "ژوئن"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "مارس"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "می"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "نوامبر"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "اکتبر"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "سپتامبر"
-
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
 msgstr "دسته‌بندی‌"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
 msgstr "الگو"
```

### Comparing `trytond_customs-6.6.0/locale/fr.po` & `trytond_customs-6.8.0/locale/ca.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,323 +1,267 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Import"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Type de calcul"
+msgstr "Tipus de càlcul"
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Pays"
+msgstr "País"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Devise"
+msgstr "Moneda"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Date de fin"
+msgstr "Data final"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr "Organització"
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Date de début"
+msgstr "Data inicial"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Code tarifaire"
+msgstr "Codi aranzelari"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Type"
+msgstr "Tipus"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "UDM"
+msgstr "UdM"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Code"
+msgstr "Codi"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Pays"
+msgstr "País"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Description"
+msgstr "Descripció"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Taux de douane"
+msgstr "Tarifa aranzelaria"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Jour final"
+msgstr "Dia final"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Mois final"
+msgstr "Mes final"
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr "Organització"
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Jour initial"
+msgstr "Data inicial"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Mois initial"
+msgstr "Mes inicial"
+
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "País"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Dia final"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "Mes final"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr "Organització"
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Produit"
+msgstr "Producte"
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Dia inicial"
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Mes inicial"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Code tarifaire"
+msgstr "Codi aranzelari"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Douanes"
+msgstr "Duanes"
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codes tarifaires"
+msgstr "Codis aranzelaris"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Utiliser les codes tarifaires du parent"
+msgstr "Usa els codis aranzelaris del pare"
 
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Pays"
+msgstr "País"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Catégorie douanière"
+msgstr "Categoria de duanes"
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codes tarifaires"
+msgstr "Codis aranzelaris"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Utiliser les codes tarifaires de la catégorie"
+msgstr "Usa els codis aranzelaris de la categoria"
 
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Pays"
+msgstr "País"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Catégorie douanière"
+msgstr "Categoria de duanes"
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codes tarifaires"
+msgstr "Codis aranzelaris"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Utiliser les codes tarifaires de la catégorie"
+msgstr "Usa els codis aranzelaris de la categoria"
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr "Le code du système harmonisé de nomenclature."
+msgstr "El codi del Sistema Harmonitzat de designació."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Utilisez les codes tarifaires définis sur la catégorie parente."
+msgstr "Utilitza els codis aranzelaris definits a la categoria pare."
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr "El país d'origen del producte."
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilisez les codes tarifaires définis sur la catégorie."
+msgstr "Utilitza els codis aranzelaris definits a la categoria."
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr "El país d'origen del producte."
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilisez les codes tarifaires définis sur la catégorie."
+msgstr "Utilitza els codis aranzelaris definits a la categoria."
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Taux de douane"
+msgstr "Taxa d'aranzel"
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Code tarifaire"
+msgstr "Codi aranzelari"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Taux de douane"
+msgstr "Taxes d'aranzel"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Codes tarifaires"
+msgstr "Codis d'aranzel"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Exportation"
+msgstr "Exportacions"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Importation"
+msgstr "Importacions"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Douanes"
+msgstr "Duanes"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Taux de douane"
+msgstr "Taxes d'aranzel"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Codes tarifaires"
+msgstr "Codis d'aranzel"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Produit - Code tarifaire"
+msgstr "Producte - Codi aranzelari"
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Administration des douanes"
+msgstr "Administració de duanes"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Montant"
+msgstr "Import"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Quantité"
+msgstr "Quantitat"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exporter"
+msgstr "Exportació"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importation"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Avril"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Août"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Décembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Février"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Janvier"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Juillet"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Juin"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Mars"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Mai"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Novembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Octobre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Septembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Avril"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Août"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Décembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Février"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Janvier"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Juillet"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Juin"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Mars"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Mai"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Novembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Octobre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Septembre"
+msgstr "Importació"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Catégorie"
+msgstr "Categoria"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Modèle"
+msgstr "Plantilla"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Calcule"
+msgstr "Càlcul"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "De"
+msgstr "Des de"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "À"
+msgstr "Fins"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Douanes"
+msgstr "Duanes"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Douanes"
+msgstr "Duanes"
```

### Comparing `trytond_customs-6.6.0/locale/hu.po` & `trytond_customs-6.8.0/locale/fi.po`

 * *Files 25% similar despite different names*

```diff
@@ -6,132 +6,155 @@
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Ország"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Pénznem"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
 msgstr ""
 
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Típus"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Egység"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Partner kód"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Ország"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Leírás"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Termék"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Külkereskedelmi"
+msgstr "Customs"
 
 #, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Ország"
+msgstr ""
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Külkereskedelmi kategória"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Ország"
+msgstr ""
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Külkereskedelmi kategória"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
@@ -142,18 +165,26 @@
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
@@ -168,26 +199,25 @@
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Exportálás"
+msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Külkereskedelem"
+msgstr "Customs"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
@@ -201,149 +231,50 @@
 msgid "Customs Administration"
 msgstr "Customs Administration"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Mennyiség"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exportálás"
+msgstr "Export"
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr ""
-
-#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategória"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Űrlap adószámlához"
+msgstr ""
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "-tól; től"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "-hoz; -höz"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Külkereskedelem"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Külkereskedelem"
+msgstr "Customs"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-6.6.0/locale/id.po` & `trytond_customs-6.8.0/locale/lo.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,325 +1,303 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Jumlah"
+msgstr "ມູນຄ່າ"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Negara"
+msgstr "ປະເທດ"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Mata uang"
+msgstr "ສະກຸນເງິນ"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Tanggal Akhir"
+msgstr "ວັນທີສິ້ນສຸດ"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Tanggal Awal"
+msgstr "ວັນທີເລີ່ມ"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr ""
+msgstr "ຮູບແບບ"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr ""
+msgstr "ຫົວໜ່ວຍ"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Kode"
+msgstr "ລະຫັດແຂວງ"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Negara"
+msgstr "ປະເທດ"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Deskripsi"
+msgstr "ເນື້ອໃນລາຍການ"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr ""
+msgstr "ວັນທີສິ້ນສຸດ"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr ""
+msgstr "ວັນທີເລີ່ມ"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "ປະເທດ"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "ວັນທີສິ້ນສຸດ"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Produk"
+msgstr "ຜະລິດຕະພັນ"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "ວັນທີເລີ່ມ"
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "ວັນທີເລີ່ມ"
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr ""
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Negara"
+msgstr "ປະເທດ"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Negara"
+msgstr "ປະເທດ"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr ""
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr ""
+msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr ""
+msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr ""
+msgstr "Customs"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
 msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr ""
+msgstr "Customs Administration"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Jumlah"
+msgstr "ມູນຄ່າ"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr ""
+msgstr "ຈຳນວນ"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr ""
+msgstr "Export"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Agustus"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Desember"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Februari"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Januari"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Juli"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Juni"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Maret"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Mei"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "September"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Agustus"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Desember"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Februari"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Januari"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Juli"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Juni"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Maret"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Mei"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "September"
+msgstr "Import"
 
+#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategori"
+msgstr "ໝວດ"
 
+#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Templat"
+msgstr "ຮ່າງແບບ"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Perhitungan"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Dari"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Kepada"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr ""
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr ""
+msgstr "Customs"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_customs-6.6.0/locale/it.po` & `trytond_customs-6.8.0/locale/nl.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,323 +1,269 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Bedrag"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "tipo calcolo"
+msgstr "Type berekening"
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Paese"
+msgstr "Land"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
 msgstr "Valuta"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Data finale"
+msgstr "Eind datum"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr "Organisatie"
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Data iniziale"
+msgstr "Start datum"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Codice dazio"
+msgstr "Tariefcodes"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr "Type"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "UdM"
+msgstr "Eenheid"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Codice"
+msgstr "Code"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Paese"
+msgstr "Land"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Omschrijving"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "aliquote dazio"
+msgstr "Invoerrechten"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Data finale"
+msgstr "Eind datum"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "fine mese"
+msgstr "Eindmaand"
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr "Organisatie"
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Data iniziale"
+msgstr "Start dag"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "mese iniziale"
+msgstr "Begin maand"
+
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Land"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Eind Dag"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "Eind Maand"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr "Organisatie"
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Prodotto"
+msgstr "Product"
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Start Dag"
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Start Maand"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Codice doganale"
+msgstr "Tariefcode"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Dogane"
+msgstr "Douane"
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codici doganali"
+msgstr "Tariefcodes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "usare il codice tariffario del padre"
+msgstr "Gebruik tariefcode van bovenliggend niveau"
 
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Paese"
+msgstr "Land"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "categoria doganale"
+msgstr "Douanecategorie"
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codici doganali"
+msgstr "Tariefcodes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "usare i codici tariffari della categoria"
+msgstr "Gebruik de tariefcodes van de categorie"
 
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Paese"
+msgstr "Land"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "categoria doganale"
+msgstr "Douanecategorie"
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Codici doganali"
+msgstr "Tariefcodes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "usare i codici tariffari della categoria"
+msgstr "Gebruik de tariefcodes van de categorie"
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr "Il codice del sistema di nomenclatura armonizzato."
+msgstr ""
+"De code van het geharmonizeerd syteem van Nomenclatuur (HS Nomenclatruur)."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Utilizzare i codici doganali definiti nella categoria del padre."
+msgstr ""
+"Gebruik de tariefcodes die zijn gedefinieerd in de bovenliggende categorie."
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr "Het land van herkomst van het product."
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilizzare i codici diganali definiti nella categoria."
+msgstr "Gebruik de tariefcodes die in de categorie zijn gedefinieerd."
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr "Het land van herkomst van het product."
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Utilizzare i codici doganali definiti nella categoria del padre."
+msgstr "Gebruik de tariefcodes die in de categorie zijn gedefinieerd."
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "aliquota dazio"
+msgstr "Invoerrechten"
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Codice dazio"
+msgstr "Tariefcodes"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Aliquote dazi"
+msgstr "Invoerrechten"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Codici doganali"
+msgstr "Tariefcodes"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Esportazione"
+msgstr "Exporteren"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Importazione"
+msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Dogane"
+msgstr "Douane"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Aliquote dazi"
+msgstr "Invoerrechten"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Codici doganali"
+msgstr "Tariefcodes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "prodotto - codice tariffario"
+msgstr "Product - Tariefcode"
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Amministrazione dogane"
+msgstr "Douane administratie"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Importo"
+msgstr "Bedrag"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Quantità"
+msgstr "Hoeveelheid"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Esportazione"
+msgstr "Exporteren"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importazione"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Aprile"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Agosto"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Dicembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Febbraio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Gennaio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Luglio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Giugno"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Marzo"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Maggio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Novembre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Ottobre"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Settembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Aprile"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Agosto"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Dicembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Febbraio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Gennaio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Luglio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Giugno"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Marzo"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Maggio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Novembre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Ottobre"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Settembre"
+msgstr "Importeren"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Categoria"
+msgstr "Categorie"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "esempio"
+msgstr "Sjabloon"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "calcolo"
+msgstr "Berekenen"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Da"
+msgstr "Van"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "a"
+msgstr "tot"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "dogane"
+msgstr "Douane"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "dogane"
+msgstr "Douane"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-6.6.0/locale/lo.po` & `trytond_customs-6.8.0/locale/zh_CN.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,122 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "ມູນຄ່າ"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "ປະເທດ"
+msgstr "考文垂郡"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "ສະກຸນເງິນ"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "ວັນທີສິ້ນສຸດ"
+msgstr ""
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "ວັນທີເລີ່ມ"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "ຮູບແບບ"
+msgstr "类型"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "ຫົວໜ່ວຍ"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "ລະຫັດແຂວງ"
+msgstr "语言编码"
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "ປະເທດ"
+msgstr "考文垂郡"
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "ເນື້ອໃນລາຍການ"
+msgstr "描述"
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "ວັນທີສິ້ນສຸດ"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "ວັນທີເລີ່ມ"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "考文垂郡"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "ຜະລິດຕະພັນ"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
 #, fuzzy
@@ -107,15 +132,15 @@
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "ປະເທດ"
+msgstr "考文垂郡"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,tariff_codes:"
@@ -125,15 +150,15 @@
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "ປະເທດ"
+msgstr "考文垂郡"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,tariff_codes:"
@@ -148,18 +173,26 @@
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
@@ -174,17 +207,18 @@
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Export"
+msgstr "导出"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
@@ -202,139 +236,39 @@
 msgid "Product - Tariff Code"
 msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
 msgstr "Customs Administration"
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "ມູນຄ່າ"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "ຈຳນວນ"
+msgstr ""
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Export"
+msgstr "导出"
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr ""
-
-#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "ໝວດ"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "ຮ່າງແບບ"
+msgstr ""
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
 msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
```

### Comparing `trytond_customs-6.6.0/locale/lt.po` & `trytond_customs-6.8.0/locale/fr.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,325 +1,267 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Montant"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Skaičiavimo būdas"
+msgstr "Type de calcul"
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Šalis"
+msgstr "Pays"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Valiuta"
+msgstr "Devise"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Pabaigos data"
+msgstr "Date de fin"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr "Organisation"
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Pradžios data"
+msgstr "Date de début"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tarifo kodas"
+msgstr "Code tarifaire"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Tipas"
+msgstr "Type"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Mato vienetas"
+msgstr "UDM"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Kodas"
+msgstr "Code"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Šalis"
+msgstr "Pays"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Aprašymas"
+msgstr "Description"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Muito tarifai"
+msgstr "Taux de douane"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Pabaigos data"
+msgstr "Jour final"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Pabaigos mėnuo"
+msgstr "Mois final"
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr "Organisation"
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Pradžios data"
+msgstr "Jour initial"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Pradžios mėnuo"
+msgstr "Mois initial"
+
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Pays"
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Jour de fin"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "Mois de fin"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr "Organisation"
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Prekė"
+msgstr "Produit"
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Jour de début"
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Mois de début"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tarifo kodas"
+msgstr "Code tarifaire"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Muitai"
+msgstr "Douanes"
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tarifų kodai"
+msgstr "Codes tarifaires"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr ""
+msgstr "Utiliser les codes tarifaires du parent"
 
-#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Šalis"
+msgstr "Pays"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Muitinės kategorija"
+msgstr "Catégorie douanière"
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tarifų kodai"
+msgstr "Codes tarifaires"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Utiliser les codes tarifaires de la catégorie"
 
-#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Šalis"
+msgstr "Pays"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Muitinės kategorija"
+msgstr "Catégorie douanière"
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tarifų kodai"
+msgstr "Codes tarifaires"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Utiliser les codes tarifaires de la catégorie"
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr ""
+msgstr "Le code du système harmonisé de nomenclature."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr ""
+msgstr "Utilisez les codes tarifaires définis sur la catégorie parente."
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr "Le pays d'origine du produit."
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr ""
+msgstr "Utilisez les codes tarifaires définis sur la catégorie."
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr "Le pays d'origine du produit."
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr ""
+msgstr "Utilisez les codes tarifaires définis sur la catégorie."
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Muito tarifas"
+msgstr "Taux de douane"
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tarifo kodas"
+msgstr "Code tarifaire"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Muito tarifai"
+msgstr "Taux de douane"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tarifų kodai"
+msgstr "Codes tarifaires"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Eksportas"
+msgstr "Exportation"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Importas"
+msgstr "Importation"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Muitai"
+msgstr "Douanes"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Muito tarifai"
+msgstr "Taux de douane"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tarifų kodai"
+msgstr "Codes tarifaires"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Prekė - tarifo kodas"
+msgstr "Produit - Code tarifaire"
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Muitų valdymas"
+msgstr "Administration des douanes"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Suma"
+msgstr "Montant"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Kiekis"
+msgstr "Quantité"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Eksportas"
+msgstr "Exporter"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importas"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Balandis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Rugpjūtis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Gruodis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Vasaris"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Sausis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Liepa"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Birželis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Kovas"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Gegužė"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Lapkritis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Spalis"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Rugsėjis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Balandis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Rugpjūtis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Gruodis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Vasaris"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Sausis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Liepa"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Birželis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Kovas"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Gegužė"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Lapkritis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Spalis"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Rugsėjis"
+msgstr "Importation"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategorija"
+msgstr "Catégorie"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Prekės šablonas"
+msgstr "Modèle"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Skaičiavimas"
+msgstr "Calcule"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Nuo"
+msgstr "De"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Iki"
+msgstr "À"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Muitai"
+msgstr "Douanes"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Muitai"
+msgstr "Douanes"
```

### Comparing `trytond_customs-6.6.0/locale/nl.po` & `trytond_customs-6.8.0/locale/et.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,325 +1,274 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Bedrag"
+msgstr "Väärtus"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Type berekening"
+msgstr "Arvutuse tüüp"
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Land"
+msgstr "Riik"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Valuuta"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Eind datum"
+msgstr "Lõppkuupäev"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Start datum"
+msgstr "Alguskuupäev"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariefcodes"
+msgstr "Tariifi kood"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Type"
+msgstr "Tüüp"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Eenheid"
+msgstr "Mõõtühik"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Code"
+msgstr "Kood"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Land"
+msgstr "Riik"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Omschrijving"
+msgstr "Selgitus"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Invoerrechten"
+msgstr "Maksumäär"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Eind datum"
+msgstr "Lõppkuupäev"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Eindmaand"
+msgstr "Lõppkuu"
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Start dag"
+msgstr "Alguskuupäev"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Begin maand"
+msgstr "Alguskuu"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Riik"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Lõppkuupäev"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "Lõppkuu"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Product"
+msgstr "Toode"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Alguskuupäev"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Alguskuu"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariefcode"
+msgstr "Tariifi kood"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Douane"
+msgstr "Toll"
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariefcodes"
+msgstr "Tariifi koodid"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Gebruik tariefcode van bovenliggend niveau"
+msgstr "Kasuta ülema jaotuse tariifi koodi"
 
+#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Land"
+msgstr "Riik"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Douanecategorie"
+msgstr "Tolli kategooria"
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariefcodes"
+msgstr "Tariifi koodid"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Gebruik de tariefcodes van de categorie"
+msgstr "Kasuta kategooria tariifi koode"
 
+#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Land"
+msgstr "Riik"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Douanecategorie"
+msgstr "Tolli kategooria"
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariefcodes"
+msgstr "Tariifi koodid"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Gebruik de tariefcodes van de categorie"
+msgstr "Kasuta kategooria tariifi koode"
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
-"De code van het geharmonizeerd syteem van Nomenclatuur (HS Nomenclatruur)."
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
-"Gebruik de tariefcodes die zijn gedefinieerd in de bovenliggende categorie."
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Gebruik de tariefcodes die in de categorie zijn gedefinieerd."
+msgstr ""
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Gebruik de tariefcodes die in de categorie zijn gedefinieerd."
+msgstr ""
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Invoerrechten"
+msgstr "Tasu määr"
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tariefcodes"
+msgstr "Tariifi kood"
 
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Invoerrechten"
+msgstr "Tasu määr"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariefcodes"
+msgstr "Tariifi kood"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Exporteren"
+msgstr "Eksport"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Douane"
+msgstr "Toll"
 
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Invoerrechten"
+msgstr "Maksumäär"
 
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariefcodes"
+msgstr "Tariifi kood"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Product - Tariefcode"
+msgstr "Toode - tariifi kood"
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Douane administratie"
+msgstr "Tolli administreerimine"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Bedrag"
+msgstr "Väärtus"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Hoeveelheid"
+msgstr "Kogus"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exporteren"
+msgstr "Eksport"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importeren"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Augustus"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "December"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Februari"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Januari"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Juli"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Juni"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Maart"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "mei"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "September"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Augustus"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "December"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Februari"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Januari"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Juli"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Juni"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Maart"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "mei"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "September"
+msgstr "Import"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Categorie"
+msgstr "Kategooria"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Sjabloon"
+msgstr "Mall"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Berekenen"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Van"
+msgstr "Kellelt"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "tot"
+msgstr "Kellele"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Douane"
+msgstr "Toll"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Douane"
+msgstr "Toll"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_customs-6.6.0/locale/pl.po` & `trytond_customs-6.8.0/locale/es_419.po`

 * *Files 27% similar despite different names*

```diff
@@ -8,340 +8,267 @@
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Kraj"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Waluta"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Data ukończenia"
+msgstr ""
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Data rozpoczęcia"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "Jm"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Kraj"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr "Tasas de aduana"
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Data ukończenia"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
-#, fuzzy
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Data rozpoczęcia"
+msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Produkt"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Customs"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr ""
+msgstr "Utilizar los códigos arancelarios del padre"
 
-#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Kraj"
+msgstr ""
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Utilizar los códigos arancelarios de la categoría"
 
-#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Kraj"
+msgstr ""
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Utilizar los códigos arancelarios de la categoría"
 
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
+msgstr "Utilizar los códigos arancelarios definidos en la categoría padre"
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
+msgstr "Utilizar los códigos arancelarios definidos en la categoría"
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr ""
+msgstr "Utilizar los códigos arancelarios definidos en la categoría"
 
-#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Duty Rates"
+msgstr "Tasa de aduana"
 
-#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tariff Codes"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr "Tasas de aduana"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Export"
+msgstr "Exportar"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr "Import"
+msgstr "Importar"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr "Customs"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr "Duty Rates"
+msgstr "Tasas de aduana"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr "Tariff Codes"
+msgstr ""
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
 msgstr ""
 
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr "Customs Administration"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Export"
+msgstr "Exportar"
 
-#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Import"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Kwiecień"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Sierpień"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Grudzień"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Luty"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Styczeń"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Lipiec"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Czerwiec"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Marzec"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Maj"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Listopad"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Październik"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Wrzesień"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Kwiecień"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Sierpień"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Grudzień"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Luty"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Styczeń"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Lipiec"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Czerwiec"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Marzec"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Maj"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Listopad"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Październik"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Wrzesień"
+msgstr "Importar"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategoria"
+msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Szablon"
+msgstr ""
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
 msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "Od"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Do"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Customs"
+msgstr ""
 
-#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Customs"
+msgstr ""
```

### Comparing `trytond_customs-6.6.0/locale/pt.po` & `trytond_customs-6.8.0/locale/bg.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,337 +1,304 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Montante"
+msgstr "Сума"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Tipo de Cálculo"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Държава"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Moeda"
+msgstr "Управление на валути"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Data Final"
+msgstr "Крайна дата"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Data de início"
+msgstr "Начална дата"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Código Tarifário"
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr "Вид"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "UDM"
+msgstr "Мерни единици"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Код"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "País"
+msgstr "Държава"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "Descrição"
+msgstr "Описание"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Taxa de Aduana"
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Dia Final"
+msgstr "Крайна дата"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Mês Final"
+msgstr ""
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Dia Inicial"
+msgstr "Начална дата"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Mês Inicial"
+msgstr ""
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Държава"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Крайна дата"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Produto"
+msgstr "Продукт"
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Начална дата"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Начална дата"
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Código da Tarifa"
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Aduana"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Códigos de Aduana"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Usar Códigos de Aduana do Pai"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "País"
+msgstr "Държава"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Categoria Aduana"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Códigos de Aduana"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Utilizar os Códigos da Categoria de Tarifa"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "País"
+msgstr "Държава"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Categoria Aduana"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Códigos de Tarifa"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Utilizar os Códigos da Categoria de Tarifa"
+msgstr ""
 
-#, fuzzy
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr "O Código da Nomenclatura do Sistema Harmonizado"
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Utilizar os códigos de aduana definidos na categoria pai"
+msgstr ""
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Usar os códifos de tarifa definidos na categoria"
+msgstr ""
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Usar dos códifos de tarifa definidos na categoria"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Taxa de Aduana"
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Código da Tarifa"
+msgstr "Tariff Codes"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 #, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "Export"
+msgstr "Извличане"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
 msgstr "Customs"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Produto - Código de Tarifa"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
 msgstr "Customs Administration"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Montante"
+msgstr "Сума"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Quantidade"
+msgstr "Количество"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Exportar"
+msgstr "Извличане"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Importar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "Abril"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Agosto"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "Dezembro"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Fevereiro"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Janeiro"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Julho"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Junho"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Março"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Maio"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "Novembro"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Outubro"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "Setembro"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "Abril"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Agosto"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "Dezembro"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Fevereiro"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Janeiro"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Julho"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Junho"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Março"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Maio"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "Novembro"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Outubro"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "Setembro"
+msgstr "Import"
 
+#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Categoria"
+msgstr "Категория мер. ед."
 
+#, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Modelo"
+msgstr "Шаблон"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Cálculo"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr "De"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr "Para"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Aduana"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Aduana"
+msgstr "Customs"
```

### Comparing `trytond_customs-6.6.0/locale/ru.po` & `trytond_customs-6.8.0/locale/ru.po`

 * *Files 27% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 msgstr "Валюты"
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
 msgstr "Дата окончания"
 
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
 msgstr "Дата начала"
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
@@ -71,29 +75,61 @@
 msgid "End Day"
 msgstr "Дата окончания"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr "Дата начала"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
 #, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Страны мира"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Дата окончания"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
 msgstr "Товарно материальные ценности (ТМЦ)"
 
 #, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Дата начала"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Дата начала"
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
 #, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
@@ -148,18 +184,26 @@
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
@@ -223,110 +267,14 @@
 msgstr "Экспорт"
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr ""
-
 #, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
 msgstr "Категория ед. измерения"
 
 #, fuzzy
 msgctxt "selection:product-customs.tariff.code,product:"
```

### Comparing `trytond_customs-6.6.0/locale/sl.po` & `trytond_customs-6.8.0/locale/pl.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,211 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr "Tip obračuna"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "Država"
+msgstr "Kraj"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Waluta"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
-msgstr "Končni datum"
+msgstr "Data ukończenia"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr "Začetni datum"
+msgstr "Data rozpoczęcia"
 
+#, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tarifna številka"
+msgstr "Tariff Codes"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "Vrsta"
+msgstr "Typ"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr "ME"
+msgstr "Jm"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "Šifra"
+msgstr "Kod"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "Država"
+msgstr "Kraj"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
 msgstr "Opis"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr "Stopnje dajatev"
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr "Končni dan"
+msgstr "Data ukończenia"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
-msgstr "Končni mesec"
+msgstr ""
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr "Začetni dan"
+msgstr "Data rozpoczęcia"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
-msgstr "Začetni mesec"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Kraj"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Data ukończenia"
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr "Izdelek"
+msgstr "Produkt"
 
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Data rozpoczęcia"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Data rozpoczęcia"
+
+#, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr "Tarifna številka"
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr "Carinjenje"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tarfine številke"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr "Uporabi nadtarifne številke"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "Država"
+msgstr "Kraj"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr "Kategorija carinjenja"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tarfine številke"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Uporabi tarifne številke iz kategorije"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "Država"
+msgstr "Kraj"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr "Kategorija carinjenja"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr "Tarifne številke"
+msgstr "Tariff Codes"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr "Uporabi tarifne številke iz kategorije"
+msgstr ""
 
-#, fuzzy
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr "Številka iz nomenklature harmoniziranega sistema"
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
-msgstr "Uporabi tarfine številke, ki so definirane v nadkategoriji"
+msgstr ""
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Uporabi tarifne številke, ki so definirane v kategoriji"
+msgstr ""
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
 
-#, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr "Uporabi tarifne številke, ki so definirane v kategoriji"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr "Stopnja dajatve"
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr "Tarifna številka"
+msgstr "Tariff Codes"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 #, fuzzy
@@ -185,153 +236,60 @@
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr "Izdelek - Tarifna številka"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
 msgstr "Customs Administration"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr "Znesek"
+msgstr ""
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr "Količina"
+msgstr ""
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "Izvoz"
+msgstr "Export"
 
+#, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr "Uvoz"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr "Avgust"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr "December"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr "Februar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr "Januar"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr "Julij"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr "Junij"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr "Marec"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr "Maj"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr "September"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr "April"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr "Avgust"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr "December"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr "Februar"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr "Januar"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr "Julij"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr "Junij"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr "Marec"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr "Maj"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr "November"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr "Oktober"
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr "September"
+msgstr "Import"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr "Kategorija"
+msgstr "Kategoria"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr "Predloga"
+msgstr "Szablon"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr "Izračun"
+msgstr ""
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
 msgstr "Od"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
 msgstr "Do"
 
+#, fuzzy
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr "Carinjenje"
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr "Carinjenje"
+msgstr "Customs"
```

### Comparing `trytond_customs-6.6.0/locale/uk.po` & `trytond_customs-6.8.0/locale/sl.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,323 +1,286 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:customs.duty.rate,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Znesek"
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
-msgstr ""
+msgstr "Tip obračuna"
 
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr ""
+msgstr "Država"
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
+msgstr "Končni datum"
+
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
-msgstr ""
+msgstr "Začetni datum"
 
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tarifna številka"
 
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr ""
+msgstr "Vrsta"
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
-msgstr ""
+msgstr "ME"
 
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr ""
+msgstr "Šifra"
 
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr ""
+msgstr "Država"
 
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr ""
+msgstr "Opis"
 
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Stopnje dajatev"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
-msgstr ""
+msgstr "Končni dan"
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
+msgstr "Končni mesec"
+
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
-msgstr ""
+msgstr "Začetni dan"
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
+msgstr "Začetni mesec"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr "Država"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr "Končni dan"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr "Končni mesec"
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
 msgstr ""
 
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
-msgstr ""
+msgstr "Izdelek"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr "Začetni dan"
+
+#, fuzzy
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr "Začetni mesec"
 
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tarifna številka"
 
 msgctxt "field:product.category,customs:"
 msgid "Customs"
-msgstr ""
+msgstr "Carinjenje"
 
 msgctxt "field:product.category,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tarfine številke"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
-msgstr ""
+msgstr "Uporabi nadtarifne številke"
 
+#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr ""
+msgstr "Država"
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
-msgstr ""
+msgstr "Kategorija carinjenja"
 
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tarfine številke"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Uporabi tarifne številke iz kategorije"
 
+#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr ""
+msgstr "Država"
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
-msgstr ""
+msgstr "Kategorija carinjenja"
 
 msgctxt "field:product.template,tariff_codes:"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tarifne številke"
 
 msgctxt "field:product.template,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
-msgstr ""
+msgstr "Uporabi tarifne številke iz kategorije"
 
+#, fuzzy
 msgctxt "help:customs.tariff.code,code:"
 msgid "The code from Harmonized System of Nomenclature."
-msgstr ""
+msgstr "Številka iz nomenklature harmoniziranega sistema"
 
+#, fuzzy
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
+msgstr "Uporabi tarfine številke, ki so definirane v nadkategoriji"
+
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
+msgstr "Uporabi tarifne številke, ki so definirane v kategoriji"
+
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
-msgstr ""
+msgstr "Uporabi tarifne številke, ki so definirane v kategoriji"
 
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
-msgstr ""
+msgstr "Stopnja dajatve"
 
 msgctxt "model:customs.tariff.code,name:"
 msgid "Tariff Code"
-msgstr ""
+msgstr "Tarifna številka"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_duty_rate_form"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr ""
+msgstr "Export"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
-msgstr ""
+msgstr "Import"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
-msgstr ""
+msgstr "Customs"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_duty_rate_form"
 msgid "Duty Rates"
-msgstr ""
+msgstr "Duty Rates"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_tariff_code_form"
 msgid "Tariff Codes"
-msgstr ""
+msgstr "Tariff Codes"
 
 msgctxt "model:product-customs.tariff.code,name:"
 msgid "Product - Tariff Code"
-msgstr ""
+msgstr "Izdelek - Tarifna številka"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_customs_admin"
 msgid "Customs Administration"
-msgstr ""
+msgstr "Customs Administration"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Amount"
-msgstr ""
+msgstr "Znesek"
 
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
-msgstr ""
+msgstr "Količina"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr ""
+msgstr "Izvoz"
 
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr ""
+msgstr "Uvoz"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
-msgstr ""
+msgstr "Kategorija"
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
-msgstr ""
+msgstr "Predloga"
 
 msgctxt "view:customs.duty.rate:"
 msgid "Computation"
-msgstr ""
+msgstr "Izračun"
 
 msgctxt "view:customs.tariff.code:"
 msgid "From"
-msgstr ""
+msgstr "Od"
 
 msgctxt "view:customs.tariff.code:"
 msgid "To"
-msgstr ""
+msgstr "Do"
 
 msgctxt "view:product.category:"
 msgid "Customs"
-msgstr ""
+msgstr "Carinjenje"
 
 msgctxt "view:product.template:"
 msgid "Customs"
-msgstr ""
+msgstr "Carinjenje"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_customs-6.6.0/locale/zh_CN.po` & `trytond_customs-6.8.0/locale/tr.po`

 * *Files 27% similar despite different names*

```diff
@@ -6,85 +6,112 @@
 msgid "Amount"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,computation_type:"
 msgid "Computation Type"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,country:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:customs.duty.rate,end_date:"
 msgid "End Date"
 msgstr ""
 
+msgctxt "field:customs.duty.rate,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.duty.rate,start_date:"
 msgid "Start Date"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.duty.rate,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
-#, fuzzy
 msgctxt "field:customs.duty.rate,type:"
 msgid "Type"
-msgstr "类型"
+msgstr ""
 
 msgctxt "field:customs.duty.rate,uom:"
 msgid "Uom"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,code:"
 msgid "Code"
-msgstr "语言编码"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,country:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:customs.tariff.code,description:"
 msgid "Description"
-msgstr "描述"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:customs.tariff.code,duty_rates:"
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "field:customs.tariff.code,end_day:"
 msgid "End Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,end_month:"
 msgid "End Month"
 msgstr ""
 
+msgctxt "field:customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:customs.tariff.code,start_day:"
 msgid "Start Day"
 msgstr ""
 
 msgctxt "field:customs.tariff.code,start_month:"
 msgid "Start Month"
 msgstr ""
 
+msgctxt "field:product-customs.tariff.code,country:"
+msgid "Country"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_day:"
+msgid "End Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,end_month:"
+msgid "End Month"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,organization:"
+msgid "Organization"
+msgstr ""
+
 msgctxt "field:product-customs.tariff.code,product:"
 msgid "Product"
 msgstr ""
 
+msgctxt "field:product-customs.tariff.code,start_day:"
+msgid "Start Day"
+msgstr ""
+
+msgctxt "field:product-customs.tariff.code,start_month:"
+msgid "Start Month"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:product-customs.tariff.code,tariff_code:"
 msgid "Tariff Code"
 msgstr "Tariff Codes"
 
 #, fuzzy
 msgctxt "field:product.category,customs:"
@@ -96,36 +123,34 @@
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.category,tariff_codes_parent:"
 msgid "Use Parent's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.product,country_of_origin:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr ""
 
 msgctxt "field:product.product,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,tariff_codes:"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
 msgctxt "field:product.product,tariff_codes_category:"
 msgid "Use Category's Tariff Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.template,country_of_origin:"
 msgid "Country"
-msgstr "考文垂郡"
+msgstr ""
 
 msgctxt "field:product.template,customs_category:"
 msgid "Customs Category"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,tariff_codes:"
@@ -140,18 +165,26 @@
 msgid "The code from Harmonized System of Nomenclature."
 msgstr ""
 
 msgctxt "help:product.category,tariff_codes_parent:"
 msgid "Use the tariff codes defined on the parent category."
 msgstr ""
 
+msgctxt "help:product.product,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.product,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
+msgctxt "help:product.template,country_of_origin:"
+msgid "The country of origin of the product."
+msgstr ""
+
 msgctxt "help:product.template,tariff_codes_category:"
 msgid "Use the tariff codes defined on the category."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:customs.duty.rate,name:"
 msgid "Duty Rate"
@@ -166,18 +199,17 @@
 msgid "Duty Rates"
 msgstr "Duty Rates"
 
 msgctxt "model:ir.action,name:act_tariff_code_form"
 msgid "Tariff Codes"
 msgstr "Tariff Codes"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_export"
 msgid "Export"
-msgstr "导出"
+msgstr "Export"
 
 msgctxt "model:ir.action.act_window.domain,name:act_duty_rate_domain_import"
 msgid "Import"
 msgstr "Import"
 
 msgctxt "model:ir.ui.menu,name:menu_customs"
 msgid "Customs"
@@ -206,117 +238,21 @@
 msgctxt "selection:customs.duty.rate,computation_type:"
 msgid "Quantity"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Export"
-msgstr "导出"
+msgstr "Export"
 
 #, fuzzy
 msgctxt "selection:customs.duty.rate,type:"
 msgid "Import"
 msgstr "Import"
 
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,end_month:"
-msgid "September"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "April"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "August"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "December"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "February"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "January"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "July"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "June"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "March"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "May"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "November"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "October"
-msgstr ""
-
-msgctxt "selection:customs.tariff.code,start_month:"
-msgid "September"
-msgstr ""
-
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Category"
 msgstr ""
 
 msgctxt "selection:product-customs.tariff.code,product:"
 msgid "Template"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_customs-6.6.0/product.py` & `trytond_customs-6.8.0/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,15 +104,16 @@
             'invisible': ((Eval('type') == 'service')
                 | Eval('tariff_codes_category', False)),
             })
     country_of_origin = fields.Many2One(
         'country.country', "Country",
         states={
             'invisible': Eval('type') == 'service',
-            })
+            },
+        help="The country of origin of the product.")
 
     @classmethod
     def __register__(cls, module_name):
         cursor = Transaction().connection.cursor()
         pool = Pool()
         Category = pool.get('product.category')
         sql_table = cls.__table__()
@@ -177,14 +178,38 @@
     __name__ = 'product-customs.tariff.code'
     product = fields.Reference('Product', selection=[
             ('product.template', 'Template'),
             ('product.category', 'Category'),
             ], required=True)
     tariff_code = fields.Many2One('customs.tariff.code', 'Tariff Code',
         required=True, ondelete='CASCADE')
+    country = fields.Function(
+        fields.Many2One('country.country', "Country"), 'get_tariff_code_field')
+    organization = fields.Function(
+        fields.Many2One('country.organization', "Organization"),
+        'get_tariff_code_field')
+    start_day = fields.Function(
+        fields.Integer("Start Day"), 'get_tariff_code_field')
+    start_month = fields.Function(
+        fields.Many2One('ir.calendar.month', "Start Month"),
+        'get_tariff_code_field')
+    end_day = fields.Function(
+        fields.Integer("End Day"), 'get_tariff_code_field')
+    end_month = fields.Function(
+        fields.Many2One('ir.calendar.month', "End Month"),
+        'get_tariff_code_field')
+
+    def get_tariff_code_field(self, name):
+        field = getattr(self.__class__, name)
+        value = getattr(self.tariff_code, name, None)
+        if isinstance(value, ModelSQL):
+            if field._type == 'reference':
+                return str(value)
+            return value.id
+        return value
 
     def get_rec_name(self, name):
         return self.tariff_code.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         return [('tariff_code.rec_name',) + tuple(clause[1:])]
```

### Comparing `trytond_customs-6.6.0/product.xml` & `trytond_customs-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-6.6.0/setup.py` & `trytond_customs-6.8.0/setup.py`

 * *Files 7% similar despite different names*

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
 name = 'trytond_customs'
 
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
 
 requires = ['simpleeval', 'python-sql >= 0.4']
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
     description='Tryton module for customs',
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
-        "Source Code": 'https://hg.tryton.org/modules/customs',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton customs tariff duty',
     package_dir={'trytond.modules.customs': '.'},
     packages=(
         ['trytond.modules.customs']
         + ['trytond.modules.customs.%s' % p for p in find_packages()]
         ),
@@ -122,25 +99,24 @@
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     customs = trytond.modules.customs
     """,
     )
```

### Comparing `trytond_customs-6.6.0/tests/test_module.py` & `trytond_customs-6.8.0/tests/test_module.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,53 +9,109 @@
 
 
 class CustomsTestCase(ModuleTestCase):
     'Test Customs module'
     module = 'customs'
 
     @with_transaction()
-    def test_tariff_code_match(self):
-        'Test tariff code match'
+    def test_tariff_code_match_date(self):
+        "Test tariff code match date"
         pool = Pool()
         Tariff = pool.get('customs.tariff.code')
         Template = pool.get('product.template')
         Product_TariffCode = pool.get(
             'product-customs.tariff.code')
+        Month = pool.get('ir.calendar.month')
+
+        june, = Month.search([('index', '=', 6)])
+        august, = Month.search([('index', '=', 8)])
 
         # Test start <= end
         tariff1 = Tariff(code='170390')
         tariff2 = Tariff(code='17039099',
-                start_month='06', start_day=20,
-                end_month='08', end_day=20)
+                start_month=june, start_day=20,
+                end_month=august, end_day=20)
         Tariff.save([tariff1, tariff2])
         template = Template(tariff_codes=[
                 Product_TariffCode(tariff_code=tariff2),
                 Product_TariffCode(tariff_code=tariff1),
                 ], tariff_codes_category=False)
 
         for pattern, result in [
                 ({'date': date(2015, 1, 1)}, tariff1),
                 ({'date': date(2015, 7, 1)}, tariff2),
                 ({'date': date(2016, 9, 1)}, tariff1),
                 ]:
             self.assertEqual(template.get_tariff_code(pattern), result)
 
         # Test start > end
-        tariff2.start_month = '08'
-        tariff2.end_month = '06'
+        tariff2.start_month = august
+        tariff2.end_month = june
         tariff2.save()
 
         for pattern, result in [
                 ({'date': date(2015, 1, 1)}, tariff2),
                 ({'date': date(2015, 7, 1)}, tariff1),
                 ({'date': date(2016, 9, 1)}, tariff2),
                 ]:
             self.assertEqual(template.get_tariff_code(pattern), result)
 
     @with_transaction()
+    def test_tariff_code_match_country(self):
+        "Test tariff code match country"
+        pool = Pool()
+        Tariff = pool.get('customs.tariff.code')
+        Country = pool.get('country.country')
+
+        country1 = Country(name="Country 1")
+        country1.save()
+        country2 = Country(name="Country 2")
+        country2.save()
+        tariff1 = Tariff(code='170390')
+        tariff1.save()
+        tariff2 = Tariff(code='17039099', country=country1)
+        tariff2.save()
+
+        self.assertTrue(tariff1.match({}))
+        self.assertTrue(tariff1.match({'country': None}))
+        self.assertTrue(tariff1.match({'country': country1.id}))
+        self.assertTrue(tariff2.match({}))
+        self.assertTrue(tariff2.match({'country': None}))
+        self.assertTrue(tariff2.match({'country': country1.id}))
+        self.assertFalse(tariff2.match({'country': country2.id}))
+
+    @with_transaction()
+    def test_tariff_code_match_country_organization(self):
+        "Test Tariff code match country with organization"
+        pool = Pool()
+        Tariff = pool.get('customs.tariff.code')
+        Country = pool.get('country.country')
+        Organization = pool.get('country.organization')
+
+        country1 = Country(name="Country 1")
+        country1.save()
+        country2 = Country(name="Country 2")
+        country2.save()
+        organization = Organization(
+            name="Organization", members=[{'country': country1.id}])
+        organization.save()
+        tariff1 = Tariff(code='170390')
+        tariff1.save()
+        tariff2 = Tariff(code='17039099', organization=organization)
+        tariff2.save()
+
+        self.assertTrue(tariff1.match({}))
+        self.assertTrue(tariff1.match({'country': None}))
+        self.assertTrue(tariff1.match({'country': country1.id}))
+        self.assertTrue(tariff2.match({}))
+        self.assertTrue(tariff2.match({'country': None}))
+        self.assertTrue(tariff2.match({'country': country1.id}))
+        self.assertFalse(tariff2.match({'country': country2.id}))
+
+    @with_transaction()
     def test_get_tariff_code(self):
         'Test get_tariff_code'
         pool = Pool()
         Tariff = pool.get('customs.tariff.code')
         Template = pool.get('product.template')
         Category = pool.get('product.category')
         Product_TariffCode = pool.get(
```

### Comparing `trytond_customs-6.6.0/trytond_customs.egg-info/PKG-INFO` & `trytond_customs-6.8.0/trytond_customs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-customs
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for customs
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
-Project-URL: Source Code, https://hg.tryton.org/modules/customs
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton customs tariff duty
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
 License-File: LICENSE
 
 Customs Module
 ##############
 
 The customs module allows to define customs duty based on the tariff code.
 
@@ -61,23 +61,25 @@
 Tarif Code
 **********
 
 It stores the `Harmonized System`_ that can be set on *Product*.
 
 - The *Code* from the HS.
 - The *Country* in case of a country specific code.
+- The *Organization* in case of a country organization code.
 - The *Start* / *End* period of the year for which the code is valid.
 
 .. _`Harmonized System`: http://en.wikipedia.org/wiki/Harmonized_System
 
 Duty Rate
 *********
 
 It stores the rate of a *Tarif Code* for a country over a period.
 
 - The *Tariff Code*.
 - The *Country* for which the rate is.
+- The *Organization* for which the rate is.
 - The *Type*: *Import* or *Export*
 - The *Start* and *End* date of validity.
 - The *Computation Type*:
     - *Amount*: fixed amount with currency.
     - *Quantity*: amount (in currency) per unit of measure.
```

### Comparing `trytond_customs-6.6.0/trytond_customs.egg-info/SOURCES.txt` & `trytond_customs-6.8.0/trytond_customs.egg-info/SOURCES.txt`

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
 customs.py
@@ -52,14 +48,15 @@
 ./view/duty_rate_list.xml
 ./view/product-tariff_code_form.xml
 ./view/product-tariff_code_list.xml
 ./view/product-tariff_code_list_sequence.xml
 ./view/tariff_code_form.xml
 ./view/tariff_code_list.xml
 ./view/template_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_customs-6.6.0/view/category_form.xml` & `trytond_customs-6.8.0/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_customs-6.6.0/view/duty_rate_form.xml` & `trytond_customs-6.8.0/view/duty_rate_form.xml`

 * *Files 23% similar despite different names*

#### Comparing `trytond_customs-6.6.0/view/duty_rate_form.xml` & `trytond_customs-6.8.0/view/duty_rate_form.xml`

```diff
@@ -4,16 +4,16 @@
 <form>
   <label name="tariff_code"/>
   <field name="tariff_code"/>
   <label name="type"/>
   <field name="type"/>
   <label name="country"/>
   <field name="country"/>
-  <!-- TODO country group -->
-  <newline/>
+  <label name="organization"/>
+  <field name="organization"/>
   <label name="start_date"/>
   <field name="start_date"/>
   <label name="end_date"/>
   <field name="end_date"/>
   <separator string="Computation" id="computation" colspan="4"/>
   <label name="computation_type"/>
   <field name="computation_type"/>
```

### Comparing `trytond_customs-6.6.0/view/tariff_code_form.xml` & `trytond_customs-6.8.0/view/tariff_code_form.xml`

 * *Files 24% similar despite different names*

#### Comparing `trytond_customs-6.6.0/view/tariff_code_form.xml` & `trytond_customs-6.8.0/view/tariff_code_form.xml`

```diff
@@ -6,20 +6,20 @@
   <field name="code"/>
   <label name="active"/>
   <field name="active"/>
   <label name="description"/>
   <field name="description" colspan="3"/>
   <label name="country"/>
   <field name="country"/>
-  <!-- TODO country group -->
-  <newline/>
+  <label name="organization"/>
+  <field name="organization"/>
   <label id="from" string="From"/>
   <group id="start" col="2">
     <field name="start_day"/>
-    <field name="start_month"/>
+    <field name="start_month" widget="selection"/>
   </group>
   <label id="to" string="To"/>
   <group id="end" col="2">
     <field name="end_day"/>
-    <field name="end_month"/>
+    <field name="end_month" widget="selection"/>
   </group>
 </form>
```

### Comparing `trytond_customs-6.6.0/view/template_form.xml` & `trytond_customs-6.8.0/view/template_form.xml`

 * *Files identical despite different names*

