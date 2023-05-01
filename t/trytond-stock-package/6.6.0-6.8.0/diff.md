# Comparing `tmp/trytond_stock_package-6.6.0.tar.gz` & `tmp/trytond_stock_package-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package-6.6.0.tar", last modified: Mon Oct 31 16:29:13 2022, max compression
+gzip compressed data, was "trytond_stock_package-6.8.0.tar", last modified: Mon May  1 11:56:52 2023, max compression
```

## Comparing `trytond_stock_package-6.6.0.tar` & `trytond_stock_package-6.8.0.tar`

### file list

```diff
@@ -1,70 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:13.596439 trytond_stock_package-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_stock_package-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_package-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      846 2022-10-31 16:29:12.000000 trytond_stock_package-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_package-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1775 2022-10-31 16:29:11.000000 trytond_stock_package-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:29:11.000000 trytond_stock_package-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:17.000000 trytond_stock_package-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_package-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2608 2022-10-31 16:29:13.596439 trytond_stock_package-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2018-08-18 09:55:17.000000 trytond_stock_package-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2021-12-11 16:59:34.000000 trytond_stock_package-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:13.593106 trytond_stock_package-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2018-08-18 09:55:17.000000 trytond_stock_package-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2022-04-08 16:24:28.000000 trytond_stock_package-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:13.586439 trytond_stock_package-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5561 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6459 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5424 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6664 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6532 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5456 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5860 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6128 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5411 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6625 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5940 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5365 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5486 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5585 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5424 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6649 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5885 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5921 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5357 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5594 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5849 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5411 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5315 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5492 2022-10-29 07:50:42.000000 trytond_stock_package-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2022-04-08 16:24:28.000000 trytond_stock_package-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:29:13.596439 trytond_stock_package-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5157 2022-10-29 07:39:12.000000 trytond_stock_package-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18035 2022-10-11 19:49:58.000000 trytond_stock_package-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6547 2022-10-11 19:49:58.000000 trytond_stock_package-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:13.586439 trytond_stock_package-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_package-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4036 2022-04-08 16:24:28.000000 trytond_stock_package-6.6.0/tests/scenario_stock_package.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2022-04-16 16:30:57.000000 trytond_stock_package-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_package-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      704 2022-10-31 15:10:09.000000 trytond_stock_package-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2022-10-31 16:29:10.000000 trytond_stock_package-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:13.596439 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2608 2022-10-31 16:29:13.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1951 2022-10-31 16:29:13.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:29:13.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2022-10-31 16:29:13.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      131 2022-10-31 16:29:13.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:29:13.000000 trytond_stock_package-6.6.0/trytond_stock_package.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:29:13.593106 trytond_stock_package-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2022-04-08 16:23:27.000000 trytond_stock_package-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1624 2022-04-08 16:24:28.000000 trytond_stock_package-6.6.0/view/package_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2021-04-03 16:10:54.000000 trytond_stock_package-6.6.0/view/package_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2019-10-11 21:50:16.000000 trytond_stock_package-6.6.0/view/package_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1203 2022-04-08 16:25:28.000000 trytond_stock_package-6.6.0/view/package_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-10-11 21:50:16.000000 trytond_stock_package-6.6.0/view/package_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2018-08-18 09:55:17.000000 trytond_stock_package-6.6.0/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2018-08-18 09:55:17.000000 trytond_stock_package-6.6.0/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2022-10-11 19:49:58.000000 trytond_stock_package-6.6.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:52.267115 trytond_stock_package-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1980 2023-05-01 11:11:25.000000 trytond_stock_package-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:11:25.000000 trytond_stock_package-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2602 2023-05-01 11:56:52.267115 trytond_stock_package-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_stock_package-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:52.263782 trytond_stock_package-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_stock_package-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:52.257115 trytond_stock_package-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5261 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6025 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5124 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6228 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6088 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5156 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5470 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5726 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5111 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6163 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5550 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5065 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5285 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5124 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6217 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5495 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5057 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5294 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5465 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5111 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5015 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-04-30 10:46:36.000000 trytond_stock_package-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:56:52.267115 trytond_stock_package-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4348 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16902 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6547 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:52.260448 trytond_stock_package-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3880 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/tests/scenario_stock_package.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-05-01 11:11:18.000000 trytond_stock_package-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:52.267115 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2602 2023-05-01 11:56:51.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1925 2023-05-01 11:56:52.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:56:51.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2023-05-01 11:56:51.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      131 2023-05-01 11:56:51.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:56:51.000000 trytond_stock_package-6.8.0/trytond_stock_package.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:56:52.263782 trytond_stock_package-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1534 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/package_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/package_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/package_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/package_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/package_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-01-16 14:00:21.000000 trytond_stock_package-6.8.0/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:21.000000 trytond_stock_package-6.8.0/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_stock_package-6.8.0/view/stock_move_form.xml
```

### Comparing `trytond_stock_package-6.6.0/CHANGELOG` & `trytond_stock_package-6.8.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove packaging prefix from dimensions
+* Remove support for Python 3.7
+* Add support for Python 3.11
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Allow package type to be deactivated
```

### Comparing `trytond_stock_package-6.6.0/COPYRIGHT` & `trytond_stock_package-6.8.0/COPYRIGHT`

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

### Comparing `trytond_stock_package-6.6.0/LICENSE` & `trytond_stock_package-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-6.6.0/PKG-INFO` & `trytond_stock_package-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for stock packaging
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock packaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
 Classifier: Natural Language :: Romanian
 Classifier: Natural Language :: Russian
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
 
 Stock Package Module
 ####################
 
 The stock package module allows to store packaging information about customer
```

### Comparing `trytond_stock_package-6.6.0/locale/bg.po` & `trytond_stock_package-6.8.0/locale/zh_CN.po`

 * *Files 8% similar despite different names*

```diff
@@ -13,44 +13,43 @@
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Наследници"
+msgstr "子项"
 
 #, fuzzy
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Код"
+msgstr "语言编码"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Движения"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -61,61 +60,61 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 #, fuzzy
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Родител"
+msgstr "上级"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "Вид"
+msgstr "类型"
 
-#, fuzzy
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Условие за плащане"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "纳木"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -124,20 +123,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -148,51 +147,51 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
```

### Comparing `trytond_stock_package-6.6.0/locale/ca.po` & `trytond_stock_package-6.8.0/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 msgid "Code"
 msgstr "Codi"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr "Altura"
+
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "UdM de l'alçada"
+
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr "Longitud"
+
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "UdM de la longitud"
+
 msgctxt "field:stock.package,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Alçada del paquet"
-
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "UdM de l'alçada del paquet"
-
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Longitud del paquet"
-
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "UdM de la longitud del paquet"
-
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volum del paquet"
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "UdM del volum del paquet"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr "Pes del paquet"
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "UdM del pes del paquet"
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Amplada del paquet"
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "UdM de l'amplada del paquet"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Pare"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Albarà"
@@ -82,34 +74,42 @@
 msgid "State"
 msgstr "Estat"
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Tipus"
 
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr "Amplada"
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "UdM de l'amplada"
+
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr "Altura"
+
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "UdM de l'alçada"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr "Longitud"
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "UdM de la longitud"
+
 msgctxt "field:stock.package.type,name:"
 msgid "Name"
 msgstr "Nom"
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Alçada del paquet"
-
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "UdM de l'alçada del paquet"
-
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Longitud del paquet"
-
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "UdM de la longitud del paquet"
-
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volum del paquet"
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "UdM del volum del paquet"
@@ -118,21 +118,21 @@
 msgid "Packaging Weight"
 msgstr "Pes del paquet"
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "UdM del pes del paquet"
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Amplada del paquet"
-
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "UdM de l'amplada del paquet"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr "Amplada"
+
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "UdM de l'amplada"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Paquets"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr "Paquets"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Paquets"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr "L'alçada del paquet."
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr "La longitud del paquet."
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr "El volum del paquet."
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "El pes del paquet quan està buit."
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr "L'amplada del paquet."
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr "L'alçada del paquet."
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr "La longitud del paquet."
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr "El volum del paquet."
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "El pes del paquet quan està buit."
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr "L'amplada del paquet."
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Tipus de paquet"
```

### Comparing `trytond_stock_package-6.6.0/locale/cs.po` & `trytond_stock_package-6.8.0/locale/es_419.po`

 * *Files 10% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 msgid "Code"
 msgstr ""
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -58,57 +58,56 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr ""
+msgstr "Envío"
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Namu"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -119,20 +118,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -143,57 +142,57 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
-msgstr "Package Types"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_volume_too_small"
 msgid ""
@@ -201,47 +200,48 @@
 "volume (%(children_volume)s) of its children packages."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr "Empaquetado de stock"
 
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr "Empaquetado de stock"
 
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
-msgstr "Package Types"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr "Empaquetado de stock"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
-msgstr ""
+msgstr "Tipo de empaquetado de stock"
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Package Types"
+msgstr "Empaquetado de stock"
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
 msgstr ""
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_package-6.6.0/locale/de.po` & `trytond_stock_package-6.8.0/locale/de.po`

 * *Files 7% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 msgid "Code"
 msgstr "Code"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr "Unternehmen"
 
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr "Höhe"
+
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "Höhe Maßeinheit"
+
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr "Länge"
+
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "Längeneinheit"
+
 msgctxt "field:stock.package,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Verpackungshöhe"
-
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Maßeinheit Verpackungshöhe"
-
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Verpackungslänge"
-
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Maßeinheit Verpackungslänge"
-
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Verpackungsvolumen"
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "Maßeinheit Verpackungsvolumen"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr "Verpackungsgewicht"
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Maßeinheit Verpackungsgewicht"
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Verpackungsbreite"
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Maßeinheit Verpackungsbreite"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Übergeordnet (Paket)"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Lieferungen"
@@ -82,34 +74,42 @@
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Typ"
 
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr "Breite"
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "Breite Maßeinheit"
+
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr "Höhe"
+
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "Höhe Maßeinheit"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr "Länge"
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "Länge Maßeinheit"
+
 msgctxt "field:stock.package.type,name:"
 msgid "Name"
 msgstr "Name"
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Verpackungshöhe"
-
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Maßeinheit Verpackungshöhe"
-
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Verpackungslänge"
-
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Maßeinheit Verpackungslänge"
-
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Verpackungsvolumen"
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "Maßeinheit Verpackungsvolumen"
@@ -118,21 +118,21 @@
 msgid "Packaging Weight"
 msgstr "Verpackungsgewicht"
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Maßeinheit Verpackungsgewicht"
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Verpackungsbreite"
-
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Maßeinheit Verpackungsbreite"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr "Breite"
+
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "Breite Maßeinheit"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Pakete"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr "Pakete"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Pakete"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr "Die Höhe der Verpackung."
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr "Die Länge der Verpackung."
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr "Das Volumen der Verpackung."
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "Das Leergewicht der Verpackung."
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr "Die Breite der Verpackung."
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr "Die Höhe der Verpackung."
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr "Die Länge der Verpackung."
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr "Das Volumen der Verpackung."
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "Das Leergewicht der Verpackung."
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr "Die Breite der Verpackung."
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Packstücktypen"
```

### Comparing `trytond_stock_package-6.6.0/locale/es.po` & `trytond_stock_package-6.8.0/locale/es.po`

 * *Files 11% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 msgid "Code"
 msgstr "Código"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr "Altura"
+
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "UdM de la altura"
+
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr "Longitud"
+
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "UdM de la longitud"
+
 msgctxt "field:stock.package,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Altura del paquete"
-
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "UdM de la altura del paquete"
-
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Longitud del paquete"
-
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "UdM de la longitud del paquete"
-
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volumen del paquete"
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "UdM del volumen del paquete"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr "Peso del paquete"
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "UdM del peso del paquete"
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Ancho del paquete"
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "UdM del ancho del paquete"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Padre"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Albarán"
@@ -82,34 +74,42 @@
 msgid "State"
 msgstr "Estado"
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Tipo"
 
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr "Ancho"
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "UdM del ancho"
+
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr "Altura"
+
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "UdM de la altura"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr "Longitud"
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "UdM de la longitud"
+
 msgctxt "field:stock.package.type,name:"
 msgid "Name"
 msgstr "Nombre"
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Altura del paquete"
-
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "UdM de la altura del paquete"
-
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Longitud del paquete"
-
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "UdM de la longitud del paquete"
-
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volumen del paquete"
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "UdM del volumen del paquete"
@@ -118,21 +118,21 @@
 msgid "Packaging Weight"
 msgstr "Peso del paquete"
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "UdM del peso del paquete"
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Ancho del paquete"
-
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "UdM del ancho del paquete"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr "Ancho"
+
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "UdM del ancho"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Paquetes"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr "Paquetes"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Paquetes"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr "La altura del paquete."
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr "La longitud del paquete."
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr "El volumen del paquete."
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "El peso del paquete cuando esta vacío."
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr "El ancho del paquete."
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr "La altura del paquete."
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr "La longitud del paquete."
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr "El volumen del paquete."
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "El peso del paquete cuando esta vacío."
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr "El ancho del paquete."
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Tipos de paquete"
```

### Comparing `trytond_stock_package-6.6.0/locale/es_419.po` & `trytond_stock_package-6.8.0/locale/cs.po`

 * *Files 12% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 msgid "Code"
 msgstr ""
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -58,58 +58,59 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr "Envío"
+msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
+msgctxt "field:stock.package,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Namu"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -118,20 +119,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -142,57 +143,57 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
-msgstr ""
+msgstr "Package Types"
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_volume_too_small"
 msgid ""
@@ -200,48 +201,47 @@
 "volume (%(children_volume)s) of its children packages."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
-msgstr "Empaquetado de stock"
+msgstr "Stock Package"
 
-#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
-msgstr "Empaquetado de stock"
+msgstr "Stock Package"
 
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
-msgstr ""
+msgstr "Package Types"
 
+#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Empaquetado de stock"
+msgstr "Stock Package"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
-msgstr "Tipo de empaquetado de stock"
+msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Empaquetado de stock"
+msgstr "Package Types"
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
 msgstr ""
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_package-6.6.0/locale/et.po` & `trytond_stock_package-6.8.0/locale/et.po`

 * *Files 6% similar despite different names*

```diff
@@ -22,37 +22,35 @@
 msgid "Code"
 msgstr "Kood"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Kanded"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr "Pakend"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Pakend"
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr "Pakend"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Pakend"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Kanded"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Pakend"
 
 #, fuzzy
@@ -66,24 +64,14 @@
 msgstr "Pakend"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Pakend"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Pakend"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Pakend"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Ülemjaotus"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Tarne"
@@ -92,38 +80,45 @@
 msgid "State"
 msgstr "Olek"
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Tüüp"
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Nimi"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr "Pakend"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Pakend"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr "Pakend"
 
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
+
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr "Pakend"
 
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Nimi"
+
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Pakend"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -136,22 +131,21 @@
 msgstr "Pakend"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Pakend"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Pakend"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr "Pakend"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Pakendid"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -162,51 +156,51 @@
 msgid "Packages"
 msgstr "Pakendid"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Pakendid"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Pakendi tüüp"
```

### Comparing `trytond_stock_package-6.6.0/locale/fa.po` & `trytond_stock_package-6.8.0/locale/fa.po`

 * *Files 4% similar despite different names*

```diff
@@ -22,37 +22,35 @@
 msgid "Code"
 msgstr "کد"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "جابجایی ها"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr "بسته"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "بسته"
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr "بسته"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "بسته"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "جابجایی ها"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "بسته"
 
 #, fuzzy
@@ -66,24 +64,14 @@
 msgstr "بسته"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "بسته"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "بسته"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "بسته"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "منبع"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "محموله"
@@ -92,38 +80,45 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "نوع"
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "نام"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr "بسته"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "بسته"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr "بسته"
 
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
+
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr "بسته"
 
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "نام"
+
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "بسته"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -136,22 +131,21 @@
 msgstr "بسته"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "بسته"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "بسته"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr "بسته"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "بسته ها"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -162,51 +156,51 @@
 msgid "Packages"
 msgstr "بسته ها"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "بسته ها"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "انواع بسته"
```

### Comparing `trytond_stock_package-6.6.0/locale/fi.po` & `trytond_stock_package-6.8.0/locale/uk.po`

 * *Files 12% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 msgid "Code"
 msgstr ""
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr ""
@@ -82,32 +74,40 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr ""
+
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -118,20 +118,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -142,57 +142,57 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
-msgstr "Package Types"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_volume_too_small"
 msgid ""
@@ -202,45 +202,43 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr ""
 
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
-msgstr "Package Types"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr ""
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Package Types"
+msgstr ""
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
 msgstr ""
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
```

### Comparing `trytond_stock_package-6.6.0/locale/fr.po` & `trytond_stock_package-6.8.0/locale/fr.po`

 * *Files 8% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 msgid "Code"
 msgstr "Code"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr "Société"
 
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr "Hauteur"
+
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "UDM de hauteur"
+
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr "Longueur"
+
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "UDM de longueur"
+
 msgctxt "field:stock.package,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Hauteur de l'emballage"
-
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Hauteur de l'emballage UDM"
-
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Longueur de l'emballage"
-
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Longueur de l'emballage UDM"
-
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volume de l'emballage"
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "Volume de l'emballage UDM"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr "Poids de l'emballage"
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Poids de l'emballage UDM"
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Largeur de l'emballage"
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Largeur de l'emballage UDM"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Parent"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Expédition"
@@ -82,34 +74,42 @@
 msgid "State"
 msgstr "État"
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Type"
 
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr "Largeur"
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "UDM de largeur"
+
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr "Hauteur"
+
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "UDM de hauteur"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr "Longueur"
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "UDM de longueur"
+
 msgctxt "field:stock.package.type,name:"
 msgid "Name"
 msgstr "Nom"
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Hauteur de l'emballage"
-
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Hauteur de l'emballage UDM"
-
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Longueur de l'emballage"
-
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Longueur de l'emballage UDM"
-
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volume de l'emballage"
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "Volume de l'emballage UDM"
@@ -118,21 +118,21 @@
 msgid "Packaging Weight"
 msgstr "Poids de l'emballage"
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Poids de l'emballage UDM"
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Largeur de l'emballage"
-
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Largeur de l'emballage UDM"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr "Largeur"
+
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "UDM de largeur"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Emballages"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr "Emballages"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Emballages"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr "La hauteur de l'emballage."
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr "La longueur de l'emballage."
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr "Le volume de l'emballage."
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "Le poids du colis vide."
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr "La largeur de l'emballage."
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr "La hauteur de l'emballage."
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr "La longueur de l'emballage."
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr "Le volume de l'emballage."
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "Le poids du colis vide."
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr "La largeur de l'emballage."
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Types d'emballage"
```

### Comparing `trytond_stock_package-6.6.0/locale/hu.po` & `trytond_stock_package-6.8.0/locale/pl.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,213 +1,206 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.configuration,package_sequence:"
 msgid "Package Sequence"
-msgstr "Csomag számkör"
+msgstr "Sekwencja paczki"
 
-#, fuzzy
 msgctxt "field:stock.configuration.sequence,package_sequence:"
 msgid "Package Sequence"
-msgstr "Csomag számkör"
+msgstr "Sekwencja paczki"
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
-msgstr "Csomag"
+msgstr "Paczka"
 
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Gyermek (csomag)"
+msgstr "Podrzędne paczki"
 
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Kód"
+msgstr "Kod"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Raktár mozgatás"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Csomag"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "Paczka"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Csomag"
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Csomag"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "Paczka"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Csomag"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Ruchy"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight:"
 msgid "Packaging Weight"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
-msgstr "Csomag"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Csomag"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Csomag"
+msgstr "Paczka"
 
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Szülő (csomag)"
+msgstr "Paczka nadrzędna"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr "Szállítási tétel"
+msgstr "Wysyłka"
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "Típus"
+msgstr "Typ"
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Név"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Csomag"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "Paczka"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Csomag"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Csomag"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "Paczka"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Csomag"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "Paczka"
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Nazwa"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight:"
 msgid "Packaging Weight"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
-msgstr "Csomag"
+msgstr "Paczka"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Csomag"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Csomag"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "Paczka"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
-msgstr "Csomagok"
+msgstr "Paczki"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
-msgstr "Csomagok"
+msgstr "Paczki"
 
 msgctxt "field:stock.shipment.out,packages:"
 msgid "Packages"
-msgstr "Csomagok"
+msgstr "Paczki"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
-msgstr "Csomagok"
+msgstr "Paczki"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
@@ -237,39 +230,40 @@
 msgstr "Stock Package"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
 msgstr "Package Types"
 
+#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Raktár csomag"
+msgstr "Stock Package"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
-msgstr "Raktár csomag típus"
+msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Csomag"
+msgstr "Paczka"
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
-msgstr "Csomag számkör"
+msgstr "Sekwencja paczki"
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
 msgstr ""
 
 msgctxt "view:stock.package:"
 msgid "Measurements"
```

### Comparing `trytond_stock_package-6.6.0/locale/id.po` & `trytond_stock_package-6.8.0/locale/lt.po`

 * *Files 18% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Cabang"
+msgstr ""
 
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Kode"
+msgstr ""
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
-msgstr "Perusahaan"
+msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Perpindahan"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -58,58 +58,59 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Induk"
+msgstr ""
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Nama"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Namu"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -118,20 +119,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -142,57 +143,57 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
-msgstr ""
+msgstr "Package Types"
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_volume_too_small"
 msgid ""
@@ -202,47 +203,49 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
-msgstr ""
+msgstr "Stock Package"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
-msgstr ""
+msgstr "Stock Package"
 
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
-msgstr ""
+msgstr "Package Types"
 
+#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr ""
+msgstr "Stock Package"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
-msgstr "Buka"
+msgstr ""
 
+#, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr ""
+msgstr "Package Types"
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
-msgstr "Urutan"
+msgstr ""
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
 msgstr ""
 
 msgctxt "view:stock.package:"
 msgid "Measurements"
```

### Comparing `trytond_stock_package-6.6.0/locale/it.po` & `trytond_stock_package-6.8.0/locale/ro.po`

 * *Files 16% similar despite different names*

```diff
@@ -10,47 +10,44 @@
 msgid "Package Sequence"
 msgstr ""
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Figlio"
+msgstr "Copii"
 
-#, fuzzy
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Codice"
+msgstr "Cod"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Movimenti"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -61,57 +58,56 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Padre"
+msgstr "Părinte"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr ""
+msgstr "Expediere"
 
 msgctxt "field:stock.package,state:"
 msgid "State"
-msgstr "Stato"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Nome"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -122,20 +118,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -146,57 +142,57 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
-msgstr "Package Types"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_volume_too_small"
 msgid ""
@@ -206,49 +202,47 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr ""
 
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
-msgstr "Package Types"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr ""
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
-msgstr ""
+msgstr "Închis"
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Package Types"
+msgstr ""
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
-msgstr ""
+msgstr "Secvenţă"
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
 msgstr ""
 
 msgctxt "view:stock.package:"
 msgid "Measurements"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_package-6.6.0/locale/lo.po` & `trytond_stock_package-6.8.0/locale/it.po`

 * *Files 10% similar despite different names*

```diff
@@ -13,46 +13,46 @@
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "ໝວດຍ່ອຍ"
+msgstr "Figlio"
 
 #, fuzzy
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "ລະຫັດແຂວງ"
+msgstr "Codice"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "ຕັດບັນຊີສາງ"
-
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Movimenti"
+
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -61,61 +61,59 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
-#, fuzzy
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "ຮ່ວງ"
+msgstr "Padre"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
-msgstr ""
+msgstr "Stato"
 
 #, fuzzy
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "ຮູບແບບ"
+msgstr "Tipo"
 
-#, fuzzy
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "ຊື່"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Nome"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -124,20 +122,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -148,51 +146,51 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_package-6.6.0/locale/lt.po` & `trytond_stock_package-6.8.0/locale/fi.po`

 * *Files 15% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 msgid "Code"
 msgstr ""
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr ""
@@ -82,33 +74,40 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Namu"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -119,20 +118,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -143,51 +142,51 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
```

### Comparing `trytond_stock_package-6.6.0/locale/nl.po` & `trytond_stock_package-6.8.0/locale/nl.po`

 * *Files 22% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 msgid "Code"
 msgstr "Code"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr "Bedrijf"
 
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr "Hoogte"
+
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "Hoogte maateenheid"
+
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr "Lengte"
+
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "Lengte maateenheid"
+
 msgctxt "field:stock.package,moves:"
 msgid "Moves"
 msgstr "Mutaties"
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Hoogte verpakking"
-
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Maateenheid hoogte verpakking"
-
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Lengte verpakking"
-
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Maateenheid lengte verpakking"
-
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volume verpakking"
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "Maateenheid volume verpakking"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr "Gewicht verpakking"
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Maateenheid gewicht verpakking"
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Breedte verpakking"
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Maateenheid breedte verpakking"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Bovenliggend niveau"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Levering"
@@ -82,34 +74,42 @@
 msgid "State"
 msgstr "Status"
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Type"
 
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr "Breedte"
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "Breedte maateenheid"
+
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr "Hoogte"
+
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "Hoogte maateenheid"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr "Lengte"
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "Lengte maateenheid"
+
 msgctxt "field:stock.package.type,name:"
 msgid "Name"
 msgstr "Naam"
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Hoogte verpakking"
-
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Maateenheid hoogte verpakking"
-
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Lengte verpakking"
-
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Maateenheid lengte verpakking"
-
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Volume verpakking"
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr "Maateenheid volume verpakking"
@@ -118,21 +118,21 @@
 msgid "Packaging Weight"
 msgstr "Gewicht verpakking"
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Maateenheid gewicht verpakking"
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Breedte verpakking"
-
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Maateenheid breedte verpakking"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr "Breedte"
+
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "Breedte maateenheid"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Pakketten"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr "Pakketten"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Pakketten"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr "De hoogte van de verpakking."
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr "De lengte van de verpakking."
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr "Het volume van de verpakking."
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "Het gewicht van de lege verpakking."
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr "De breedte van de verpakking."
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr "De hoogte van de verpakking."
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr "De lengte van de verpakking."
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr "Het volume van de verpakking."
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr "Het gewicht van de lege verpakking."
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr "De breedte van de verpakking."
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Pakket Soorten"
```

### Comparing `trytond_stock_package-6.6.0/locale/pl.po` & `trytond_stock_package-6.8.0/locale/pt.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,212 +1,206 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.configuration,package_sequence:"
 msgid "Package Sequence"
-msgstr "Sekwencja paczki"
+msgstr "Sequência das Embalagens"
 
 msgctxt "field:stock.configuration.sequence,package_sequence:"
 msgid "Package Sequence"
-msgstr "Sekwencja paczki"
+msgstr "Sequência dos Pacotes"
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
-msgstr "Paczka"
+msgstr "Pacote"
 
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Podrzędne paczki"
+msgstr "Filhos"
 
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Kod"
+msgstr "Código"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Ruchy"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Paczka"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr "Pacote"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Paczka"
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Paczka"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr "Pacote"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Paczka"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Movimentações"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight:"
 msgid "Packaging Weight"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
-msgstr "Paczka"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Paczka"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Paczka"
+msgstr "Pacote"
 
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Paczka nadrzędna"
+msgstr "Pai"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr "Wysyłka"
+msgstr "Remessa"
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "Typ"
+msgstr "Tipo"
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Nazwa"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Paczka"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr "Pacote"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Paczka"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Paczka"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr "Pacote"
+
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Paczka"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr "Pacote"
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Nome"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight:"
 msgid "Packaging Weight"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
-msgstr "Paczka"
+msgstr "Pacote"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Paczka"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Paczka"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr "Pacote"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
-msgstr "Paczki"
+msgstr "Pacotes"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
-msgstr "Paczki"
+msgstr "Pacotes"
 
 msgctxt "field:stock.shipment.out,packages:"
 msgid "Packages"
-msgstr "Paczki"
+msgstr "Pacotes"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
-msgstr "Paczki"
+msgstr "Pacotes"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
@@ -236,40 +230,39 @@
 msgstr "Stock Package"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
 msgstr "Package Types"
 
-#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Stock Package"
+msgstr "Estoque de Pacote"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
-msgstr ""
+msgstr "Tipo de Estoque de Pacote"
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Paczka"
+msgstr "Pacote"
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
-msgstr "Sekwencja paczki"
+msgstr "Sequência das Embalagens"
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
 msgstr ""
 
 msgctxt "view:stock.package:"
 msgid "Measurements"
```

### Comparing `trytond_stock_package-6.6.0/locale/pt.po` & `trytond_stock_package-6.8.0/locale/bg.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,216 +1,201 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:stock.configuration,package_sequence:"
 msgid "Package Sequence"
-msgstr "Sequência das Embalagens"
+msgstr ""
 
 msgctxt "field:stock.configuration.sequence,package_sequence:"
 msgid "Package Sequence"
-msgstr "Sequência dos Pacotes"
+msgstr ""
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
-msgstr "Pacote"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Filhos"
+msgstr "Наследници"
 
+#, fuzzy
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Código"
+msgstr "Код"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Movimentações"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
-msgstr "Pacote"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Pacote"
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
-msgstr "Pacote"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Pacote"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Движения"
 
-#, fuzzy
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package,packaging_weight:"
 msgid "Packaging Weight"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
-msgstr "Pacote"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Pacote"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Pacote"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Pai"
+msgstr "Родител"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr "Remessa"
+msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "Tipo"
+msgstr "Вид"
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Nome"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
-msgstr "Pacote"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Pacote"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
-msgstr "Pacote"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Pacote"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
+
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
 
 #, fuzzy
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Условие за плащане"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package.type,packaging_weight:"
 msgid "Packaging Weight"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
-msgstr "Pacote"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Pacote"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Pacote"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
+msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
-msgstr "Pacotes"
+msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
 msgid "Packages"
-msgstr "Pacotes"
+msgstr ""
 
 msgctxt "field:stock.shipment.out,packages:"
 msgid "Packages"
-msgstr "Pacotes"
+msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
-msgstr "Pacotes"
+msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
@@ -221,54 +206,51 @@
 "volume (%(children_volume)s) of its children packages."
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
 msgstr "Stock Package"
 
-#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
 msgstr "Stock Package"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
 msgstr "Package Types"
 
+#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr "Estoque de Pacote"
+msgstr "Stock Package"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
-msgstr "Tipo de Estoque de Pacote"
+msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr "Pacote"
+msgstr "Package Types"
 
-#, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
-msgstr "Sequência das Embalagens"
+msgstr ""
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
 msgstr ""
 
 msgctxt "view:stock.package:"
 msgid "Measurements"
```

### Comparing `trytond_stock_package-6.6.0/locale/ro.po` & `trytond_stock_package-6.8.0/locale/id.po`

 * *Files 21% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Copii"
+msgstr "Cabang"
 
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr "Kode"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
-msgstr ""
+msgstr "Perusahaan"
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr ""
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Perpindahan"
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
@@ -58,58 +58,58 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Părinte"
+msgstr "Induk"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr "Expediere"
+msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Nama"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -118,20 +118,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr ""
 
@@ -222,27 +222,27 @@
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
-msgstr "Închis"
+msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
-msgstr ""
+msgstr "Buka"
 
 msgctxt "view:stock.configuration:"
 msgid "Package"
 msgstr ""
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
-msgstr "Secvenţă"
+msgstr "Urutan"
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
 msgstr ""
 
 msgctxt "view:stock.package:"
 msgid "Measurements"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_package-6.6.0/locale/ru.po` & `trytond_stock_package-6.8.0/locale/lo.po`

 * *Files 8% similar despite different names*

```diff
@@ -13,46 +13,46 @@
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr "Подчиненый"
+msgstr "ໝວດຍ່ອຍ"
 
 #, fuzzy
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr "Код языка"
+msgstr "ລະຫັດແຂວງ"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Перемещения"
-
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "ຕັດບັນຊີສາງ"
+
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -61,62 +61,61 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 #, fuzzy
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr "Предок"
+msgstr "ຮ່ວງ"
 
-#, fuzzy
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr "Доставка"
+msgstr ""
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:stock.package,type:"
 msgid "Type"
-msgstr "Тип"
+msgstr "ຮູບແບບ"
 
-#, fuzzy
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Правило оплаты"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+#, fuzzy
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "ຊື່"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -125,20 +124,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -149,51 +148,51 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
```

### Comparing `trytond_stock_package-6.6.0/locale/sl.po` & `trytond_stock_package-6.8.0/locale/sl.po`

 * *Files 13% similar despite different names*

```diff
@@ -22,37 +22,35 @@
 msgid "Code"
 msgstr "Šifra"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
-msgstr "Promet"
+msgctxt "field:stock.package,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr "Paket"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Paket"
+msgctxt "field:stock.package,length:"
+msgid "Length"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr "Paket"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr "Paket"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Promet"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Paket"
 
 #, fuzzy
@@ -66,24 +64,14 @@
 msgstr "Paket"
 
 #, fuzzy
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Paket"
 
-#, fuzzy
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr "Paket"
-
-#, fuzzy
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr "Paket"
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr "Matični paket"
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr "Pošiljka"
@@ -92,38 +80,45 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr "Tip"
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
-msgstr "Naziv"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr "Paket"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
-msgstr "Paket"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr "Paket"
 
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
+msgstr ""
+
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr "Paket"
 
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Naziv"
+
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr "Paket"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -136,22 +131,21 @@
 msgstr "Paket"
 
 #, fuzzy
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr "Paket"
 
-#, fuzzy
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
-msgstr "Paket"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
+msgstr ""
 
 #, fuzzy
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr "Paket"
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr "Paketi"
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -162,51 +156,51 @@
 msgid "Packages"
 msgstr "Paketi"
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr "Paketi"
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
```

### Comparing `trytond_stock_package-6.6.0/locale/tr.po` & `trytond_stock_package-6.8.0/locale/tr.po`

 * *Files 16% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 msgid "Code"
 msgstr ""
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
@@ -58,22 +58,14 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
 msgstr ""
@@ -82,32 +74,40 @@
 msgid "State"
 msgstr ""
 
 msgctxt "field:stock.package,type:"
 msgid "Type"
 msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
+msgctxt "field:stock.package,width:"
+msgid "Width"
+msgstr ""
+
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
+msgstr ""
+
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
@@ -118,20 +118,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -142,51 +142,51 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
 msgstr "Package Types"
```

### Comparing `trytond_stock_package-6.6.0/locale/uk.po` & `trytond_stock_package-6.8.0/locale/ru.po`

 * *Files 24% similar despite different names*

```diff
@@ -10,45 +10,48 @@
 msgid "Package Sequence"
 msgstr ""
 
 msgctxt "field:stock.move,package:"
 msgid "Package"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.package,children:"
 msgid "Children"
-msgstr ""
+msgstr "Подчиненый"
 
+#, fuzzy
 msgctxt "field:stock.package,code:"
 msgid "Code"
-msgstr ""
+msgstr "Код языка"
 
 msgctxt "field:stock.package,company:"
 msgid "Company"
 msgstr ""
 
-msgctxt "field:stock.package,moves:"
-msgid "Moves"
+msgctxt "field:stock.package,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_length_uom:"
-msgid "Packaging Length UOM"
-msgstr ""
+#, fuzzy
+msgctxt "field:stock.package,moves:"
+msgid "Moves"
+msgstr "Перемещения"
 
 msgctxt "field:stock.package,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
@@ -58,58 +61,62 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package,packaging_width:"
-msgid "Packaging Width"
-msgstr ""
-
-msgctxt "field:stock.package,packaging_width_uom:"
-msgid "Packaging Width UOM"
-msgstr ""
-
+#, fuzzy
 msgctxt "field:stock.package,parent:"
 msgid "Parent"
-msgstr ""
+msgstr "Предок"
 
+#, fuzzy
 msgctxt "field:stock.package,shipment:"
 msgid "Shipment"
-msgstr ""
+msgstr "Доставка"
 
 msgctxt "field:stock.package,state:"
 msgid "State"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.package,type:"
 msgid "Type"
+msgstr "Тип"
+
+msgctxt "field:stock.package,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,name:"
-msgid "Name"
+msgctxt "field:stock.package,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height:"
-msgid "Packaging Height"
+msgctxt "field:stock.package.type,height:"
+msgid "Height"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_height_uom:"
-msgid "Packaging Height UOM"
+msgctxt "field:stock.package.type,height_uom:"
+msgid "Height UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length:"
-msgid "Packaging Length"
+msgctxt "field:stock.package.type,length:"
+msgid "Length"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_length_uom:"
-msgid "Packaging Length UOM"
+msgctxt "field:stock.package.type,length_uom:"
+msgid "Length UOM"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:stock.package.type,name:"
+msgid "Name"
+msgstr "Правило оплаты"
+
 msgctxt "field:stock.package.type,packaging_volume:"
 msgid "Packaging Volume"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_volume_uom:"
 msgid "Packaging Volume UOM"
 msgstr ""
@@ -118,20 +125,20 @@
 msgid "Packaging Weight"
 msgstr ""
 
 msgctxt "field:stock.package.type,packaging_weight_uom:"
 msgid "Packaging Weight UOM"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width:"
-msgid "Packaging Width"
+msgctxt "field:stock.package.type,width:"
+msgid "Width"
 msgstr ""
 
-msgctxt "field:stock.package.type,packaging_width_uom:"
-msgid "Packaging Width UOM"
+msgctxt "field:stock.package.type,width_uom:"
+msgid "Width UOM"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,packages:"
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.in.return,root_packages:"
@@ -142,57 +149,57 @@
 msgid "Packages"
 msgstr ""
 
 msgctxt "field:stock.shipment.out,root_packages:"
 msgid "Packages"
 msgstr ""
 
-msgctxt "help:stock.package,packaging_height:"
+msgctxt "help:stock.package,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_length:"
+msgctxt "help:stock.package,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package,packaging_width:"
+msgctxt "help:stock.package,width:"
 msgid "The width of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_height:"
+msgctxt "help:stock.package.type,height:"
 msgid "The height of the package."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_length:"
+msgctxt "help:stock.package.type,length:"
 msgid "The length of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_volume:"
 msgid "The volume of the package."
 msgstr ""
 
 msgctxt "help:stock.package.type,packaging_weight:"
 msgid "The weight of the package when empty."
 msgstr ""
 
-msgctxt "help:stock.package.type,packaging_width:"
+msgctxt "help:stock.package.type,width:"
 msgid "The width of the package."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_package_type_form"
 msgid "Package Types"
-msgstr ""
+msgstr "Package Types"
 
 msgctxt "model:ir.message,text:msg_package_mismatch"
 msgid "To process shipment \"%(shipment)s\", you must pack all its moves."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_package_volume_too_small"
 msgid ""
@@ -202,43 +209,45 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_package_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_package"
 msgid "Stock Package"
-msgstr ""
+msgstr "Stock Package"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_package"
 msgid "Stock Package"
-msgstr ""
+msgstr "Stock Package"
 
 msgctxt "model:ir.ui.menu,name:menu_package_form"
 msgid "Package Types"
-msgstr ""
+msgstr "Package Types"
 
+#, fuzzy
 msgctxt "model:stock.package,name:"
 msgid "Stock Package"
-msgstr ""
+msgstr "Stock Package"
 
 msgctxt "model:stock.package.type,name:"
 msgid "Stock Package Type"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Closed"
 msgstr ""
 
 msgctxt "selection:stock.package,state:"
 msgid "Open"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:stock.configuration:"
 msgid "Package"
-msgstr ""
+msgstr "Package Types"
 
 msgctxt "view:stock.configuration:"
 msgid "Sequence"
 msgstr ""
 
 msgctxt "view:stock.package.type:"
 msgid "Measurements"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_stock_package-6.6.0/message.xml` & `trytond_stock_package-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-6.6.0/setup.py` & `trytond_stock_package-6.8.0/setup.py`

 * *Files 18% similar despite different names*

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
 name = 'trytond_stock_package'
 
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
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for stock packaging',
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
-        "Source Code": 'https://hg.tryton.org/modules/stock_package',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock packaging',
     package_dir={'trytond.modules.stock_package': '.'},
     packages=(
         ['trytond.modules.stock_package']
         + ['trytond.modules.stock_package.%s' % p for p in find_packages()]
         ),
@@ -124,27 +102,26 @@
         'Natural Language :: Romanian',
         'Natural Language :: Russian',
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
     stock_package = trytond.modules.stock_package
     """,
     )
```

### Comparing `trytond_stock_package-6.6.0/stock.py` & `trytond_stock_package-6.8.0/stock.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,106 +76,98 @@
         except KeyError:
             return None
 
 
 class MeasurementsMixin:
     __slots__ = ()
 
-    packaging_length = fields.Float(
-        "Packaging Length", digits='packaging_length_uom',
+    length = fields.Float(
+        "Length", digits='length_uom',
         help="The length of the package.")
-    packaging_length_uom = fields.Many2One(
-        'product.uom', "Packaging Length UOM",
+    length_uom = fields.Many2One(
+        'product.uom', "Length UOM",
         domain=[('category', '=', Id('product', 'uom_cat_length'))],
         states={
-            'required': Bool(Eval('packaging_length')),
-            },
-        depends=['packaging_length'])
-    packaging_height = fields.Float(
-        "Packaging Height", digits='packaging_height_uom',
+            'required': Bool(Eval('length')),
+            })
+    height = fields.Float(
+        "Height", digits='height_uom',
         help="The height of the package.")
-    packaging_height_uom = fields.Many2One(
-        'product.uom', "Packaging Height UOM",
+    height_uom = fields.Many2One(
+        'product.uom', "Height UOM",
         domain=[('category', '=', Id('product', 'uom_cat_length'))],
         states={
-            'required': Bool(Eval('packaging_height')),
-            },
-        depends=['packaging_height'])
-    packaging_width = fields.Float(
-        "Packaging Width", digits='packaging_width_uom',
+            'required': Bool(Eval('height')),
+            })
+    width = fields.Float(
+        "Width", digits='width_uom',
         help="The width of the package.")
-    packaging_width_uom = fields.Many2One(
-        'product.uom', "Packaging Width UOM",
+    width_uom = fields.Many2One(
+        'product.uom', "Width UOM",
         domain=[('category', '=', Id('product', 'uom_cat_length'))],
         states={
-            'required': Bool(Eval('packaging_width')),
-            },
-        depends=['packaging_width'])
+            'required': Bool(Eval('width')),
+            })
 
     packaging_volume = fields.Float(
         "Packaging Volume", digits='packaging_volume_uom',
         states={
             'readonly': (
-                Bool(Eval('packaging_length'))
-                & Bool(Eval('packaging_height'))
-                & Bool(Eval('packaging_width'))),
+                Bool(Eval('length'))
+                & Bool(Eval('height'))
+                & Bool(Eval('width'))),
             },
-        depends=['packaging_length', 'packaging_height', 'packaging_width'],
         help="The volume of the package.")
     packaging_volume_uom = fields.Many2One(
         'product.uom', "Packaging Volume UOM",
         domain=[('category', '=', Id('product', 'uom_cat_volume'))],
         states={
             'required': Bool(Eval('packaging_volume')),
-            },
-        depends=['packaging_volume'])
+            })
 
     packaging_weight = fields.Float(
         "Packaging Weight", digits='packaging_weight_uom',
         help="The weight of the package when empty.")
     packaging_weight_uom = fields.Many2One(
         'product.uom', "Packaging Weight UOM",
         domain=[('category', '=', Id('product', 'uom_cat_weight'))],
         states={
             'required': Bool(Eval('packaging_weight')),
             })
 
     @fields.depends(
         'packaging_volume', 'packaging_volume_uom',
-        'packaging_length', 'packaging_length_uom',
-        'packaging_height', 'packaging_height_uom',
-        'packaging_width', 'packaging_width_uom')
+        'length', 'length_uom',
+        'height', 'height_uom',
+        'width', 'width_uom')
     def on_change_with_packaging_volume(self):
         pool = Pool()
         ModelData = pool.get('ir.model.data')
         Uom = pool.get('product.uom')
 
         if not all([self.packaging_volume_uom,
-                    self.packaging_length, self.packaging_length_uom,
-                    self.packaging_height, self.packaging_height_uom,
-                    self.packaging_width, self.packaging_width_uom]):
+                    self.length, self.length_uom,
+                    self.height, self.height_uom,
+                    self.width, self.width_uom]):
             if all([
-                        self.packaging_length,
-                        self.packaging_height,
-                        self.packaging_width]):
+                        self.length,
+                        self.height,
+                        self.width]):
                 return
             return self.packaging_volume
 
         meter = Uom(ModelData.get_id('product', 'uom_meter'))
         cubic_meter = Uom(ModelData.get_id('product', 'uom_cubic_meter'))
 
         length = Uom.compute_qty(
-            self.packaging_length_uom, self.packaging_length, meter,
-            round=False)
+            self.length_uom, self.length, meter, round=False)
         height = Uom.compute_qty(
-            self.packaging_height_uom, self.packaging_height, meter,
-            round=False)
+            self.height_uom, self.height, meter, round=False)
         width = Uom.compute_qty(
-            self.packaging_width_uom, self.packaging_width, meter,
-            round=False)
+            self.width_uom, self.width, meter, round=False)
 
         return Uom.compute_qty(
             cubic_meter, length * height * width, self.packaging_volume_uom)
 
 
 class Package(tree(), MeasurementsMixin, ModelSQL, ModelView):
     'Stock Package'
@@ -370,18 +362,15 @@
 
 class Move(metaclass=PoolMeta):
     __name__ = 'stock.move'
     package = fields.Many2One(
         'stock.package', "Package", readonly=True,
         domain=[
             ('company', '=', Eval('company', -1)),
-            ],
-        states={
-            'readonly': Eval('state') == 'cancelled',
-            })
+            ])
 
     @property
     def package_path(self):
         path = []
         package = self.package
         while package:
             path.append(package)
@@ -408,32 +397,22 @@
 
 class PackageMixin(object):
     __slots__ = ()
     packages = fields.One2Many('stock.package', 'shipment', 'Packages',
         domain=[
             ('company', '=', Eval('company', -1)),
             ])
-    root_packages = fields.Function(fields.One2Many('stock.package',
-            'shipment', 'Packages',
-            domain=[
-                ('company', '=', Eval('company', -1)),
-                ('parent', '=', None),
-                ]),
-        'get_root_packages', setter='set_root_packages')
-
-    def get_root_packages(self, name):
-        return [p.id for p in self.packages if not p.parent]
-
-    @classmethod
-    def set_root_packages(cls, shipments, name, value):
-        if not value:
-            return
-        cls.write(shipments, {
-                'packages': value,
-                })
+    root_packages = fields.One2Many('stock.package',
+        'shipment', 'Packages',
+        domain=[
+            ('company', '=', Eval('company', -1)),
+            ],
+        filter=[
+            ('parent', '=', None),
+            ])
 
     @classmethod
     def check_packages(cls, shipments):
         for shipment in shipments:
             if not shipment.packages:
                 continue
             length = sum(len(p.moves) for p in shipment.packages)
```

### Comparing `trytond_stock_package-6.6.0/stock.xml` & `trytond_stock_package-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package-6.6.0/tests/scenario_stock_package.rst` & `trytond_stock_package-6.8.0/tests/scenario_stock_package.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ======================
 Stock Package Scenario
 ======================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.exceptions import UserError
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_package')
 
 Create company::
 
@@ -82,41 +82,41 @@
     >>> shipment_out.click('assign_force')
     >>> shipment_out.click('pick')
 
 Package products::
 
     >>> PackageType = Model.get('stock.package.type')
     >>> box = PackageType(name='box')
-    >>> box.packaging_length = 80
-    >>> box.packaging_length_uom, = ProductUom.find([('name', '=', "Centimeter")])
-    >>> box.packaging_width = 1
-    >>> box.packaging_width_uom, = ProductUom.find([('name', '=', "Meter")])
-    >>> box.packaging_height_uom = box.packaging_length_uom
+    >>> box.length = 80
+    >>> box.length_uom, = ProductUom.find([('name', '=', "Centimeter")])
+    >>> box.width = 1
+    >>> box.width_uom, = ProductUom.find([('name', '=', "Meter")])
+    >>> box.height_uom = box.length_uom
     >>> box.packaging_volume
     >>> box.packaging_volume_uom, = ProductUom.find([('name', '=', "Cubic meter")])
     >>> box.save()
     >>> package1 = shipment_out.packages.new(type=box)
-    >>> package1.packaging_length
+    >>> package1.length
     80.0
-    >>> package1.packaging_height = 50
+    >>> package1.height = 50
     >>> package1.packaging_volume
     0.4
     >>> package_child = package1.children.new(shipment=shipment_out, type=box)
-    >>> package_child.packaging_height = 100
+    >>> package_child.height = 100
     >>> moves = package_child.moves.find()
     >>> len(moves)
     2
     >>> package_child.moves.append(moves[0])
 
     >>> shipment_out.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     PackageValidationError: ...
 
-    >>> package1.packaging_height = 120
+    >>> package1.height = 120
     >>> package1.packaging_volume
     0.96
 
     >>> shipment_out.click('pack')  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     PackageError: ...
```

### Comparing `trytond_stock_package-6.6.0/trytond_stock_package.egg-info/PKG-INFO` & `trytond_stock_package-6.8.0/trytond_stock_package.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock-package
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for stock packaging
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
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_package
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock packaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,21 +38,21 @@
 Classifier: Natural Language :: Romanian
 Classifier: Natural Language :: Russian
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
 
 Stock Package Module
 ####################
 
 The stock package module allows to store packaging information about customer
```

### Comparing `trytond_stock_package-6.6.0/trytond_stock_package.egg-info/SOURCES.txt` & `trytond_stock_package-6.8.0/trytond_stock_package.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

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
@@ -54,14 +50,15 @@
 ./view/package_list.xml
 ./view/package_tree.xml
 ./view/package_type_form.xml
 ./view/package_type_list.xml
 ./view/shipment_in_return_form.xml
 ./view/shipment_out_form.xml
 ./view/stock_move_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_stock_package-6.6.0/view/package_form.xml` & `trytond_stock_package-6.8.0/view/package_form.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_stock_package-6.6.0/view/package_form.xml` & `trytond_stock_package-6.8.0/view/package_form.xml`

```diff
@@ -16,23 +16,23 @@
     <page name="moves">
       <field name="moves" colspan="4" widget="many2many"/>
     </page>
     <page name="children">
       <field name="children" colspan="4"/>
     </page>
     <page string="Measurements" col="3" id="measurements">
-      <label name="packaging_length"/>
-      <field name="packaging_length"/>
-      <field name="packaging_length_uom" widget="selection"/>
-      <label name="packaging_height"/>
-      <field name="packaging_height"/>
-      <field name="packaging_height_uom" widget="selection"/>
-      <label name="packaging_width"/>
-      <field name="packaging_width"/>
-      <field name="packaging_width_uom" widget="selection"/>
+      <label name="length"/>
+      <field name="length"/>
+      <field name="length_uom" widget="selection"/>
+      <label name="height"/>
+      <field name="height"/>
+      <field name="height_uom" widget="selection"/>
+      <label name="width"/>
+      <field name="width"/>
+      <field name="width_uom" widget="selection"/>
       <label name="packaging_volume"/>
       <field name="packaging_volume"/>
       <field name="packaging_volume_uom" widget="selection"/>
       <label name="packaging_weight"/>
       <field name="packaging_weight"/>
       <field name="packaging_weight_uom"/>
     </page>
```

### Comparing `trytond_stock_package-6.6.0/view/package_type_form.xml` & `trytond_stock_package-6.8.0/view/package_type_form.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_stock_package-6.6.0/view/package_type_form.xml` & `trytond_stock_package-6.8.0/view/package_type_form.xml`

```diff
@@ -4,23 +4,23 @@
 <form>
   <label name="name"/>
   <field name="name"/>
   <label name="active"/>
   <field name="active"/>
   <notebook colspan="4">
     <page string="Measurements" col="3" id="measurements">
-      <label name="packaging_length"/>
-      <field name="packaging_length"/>
-      <field name="packaging_length_uom" widget="selection"/>
-      <label name="packaging_height"/>
-      <field name="packaging_height"/>
-      <field name="packaging_height_uom" widget="selection"/>
-      <label name="packaging_width"/>
-      <field name="packaging_width"/>
-      <field name="packaging_width_uom" widget="selection"/>
+      <label name="length"/>
+      <field name="length"/>
+      <field name="length_uom" widget="selection"/>
+      <label name="height"/>
+      <field name="height"/>
+      <field name="height_uom" widget="selection"/>
+      <label name="width"/>
+      <field name="width"/>
+      <field name="width_uom" widget="selection"/>
       <label name="packaging_volume"/>
       <field name="packaging_volume"/>
       <field name="packaging_volume_uom" widget="selection"/>
       <label name="packaging_weight"/>
       <field name="packaging_weight"/>
       <field name="packaging_weight_uom" widget="selection"/>
     </page>
```

