# Comparing `tmp/trytond_product_attribute-6.6.0.tar.gz` & `tmp/trytond_product_attribute-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_attribute-6.6.0.tar", last modified: Mon Oct 31 15:52:51 2022, max compression
+gzip compressed data, was "trytond_product_attribute-6.8.0.tar", last modified: Mon May  1 11:42:16 2023, max compression
```

## Comparing `trytond_product_attribute-6.6.0.tar` & `trytond_product_attribute-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:51.607593 trytond_product_attribute-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_product_attribute-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_product_attribute-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      940 2022-10-31 15:52:50.000000 trytond_product_attribute-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_product_attribute-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1667 2022-10-31 15:52:49.000000 trytond_product_attribute-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 15:52:49.000000 trytond_product_attribute-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:34.000000 trytond_product_attribute-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_product_attribute-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2630 2022-10-31 15:52:51.607593 trytond_product_attribute-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2019-02-13 10:09:34.000000 trytond_product_attribute-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2021-12-11 16:59:33.000000 trytond_product_attribute-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:51.604259 trytond_product_attribute-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2019-02-13 10:09:34.000000 trytond_product_attribute-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:51.604259 trytond_product_attribute-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2652 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2351 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2673 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2708 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2293 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2923 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2338 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2721 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2153 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2661 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2737 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2635 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2683 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2428 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2368 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2404 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2022-10-29 07:50:34.000000 trytond_product_attribute-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2021-10-30 15:16:00.000000 trytond_product_attribute-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2022-10-11 19:49:58.000000 trytond_product_attribute-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6051 2021-02-27 17:17:01.000000 trytond_product_attribute-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:52:51.607593 trytond_product_attribute-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5071 2022-10-29 07:39:11.000000 trytond_product_attribute-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:51.604259 trytond_product_attribute-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_product_attribute-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2022-04-16 16:30:56.000000 trytond_product_attribute-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2022-10-31 15:10:09.000000 trytond_product_attribute-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2022-10-31 15:52:48.000000 trytond_product_attribute-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:51.607593 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2630 2022-10-31 15:52:51.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1825 2022-10-31 15:52:51.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:52:51.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2022-10-31 15:52:51.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:52.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2022-10-31 15:52:51.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:52:51.000000 trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:52:51.604259 trytond_product_attribute-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      789 2021-02-14 13:29:06.000000 trytond_product_attribute-6.6.0/view/attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2019-11-26 21:29:22.000000 trytond_product_attribute-6.6.0/view/attribute_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2020-08-21 13:12:16.000000 trytond_product_attribute-6.6.0/view/attribute_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2019-11-26 21:29:22.000000 trytond_product_attribute-6.6.0/view/attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2019-02-13 10:09:34.000000 trytond_product_attribute-6.6.0/view/attribute_set_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2021-10-30 15:16:00.000000 trytond_product_attribute-6.6.0/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2022-04-08 16:23:26.000000 trytond_product_attribute-6.6.0/view/product_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2019-02-13 10:09:34.000000 trytond_product_attribute-6.6.0/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2022-04-08 16:23:26.000000 trytond_product_attribute-6.6.0/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:16.642916 trytond_product_attribute-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1830 2023-05-01 11:01:39.000000 trytond_product_attribute-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:01:39.000000 trytond_product_attribute-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_attribute-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2620 2023-05-01 11:42:16.642916 trytond_product_attribute-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:16.639582 trytond_product_attribute-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-01-16 14:00:20.000000 trytond_product_attribute-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:16.632915 trytond_product_attribute-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2652 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2351 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2673 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2708 2023-04-29 08:02:40.000000 trytond_product_attribute-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2293 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2923 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2721 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2781 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2153 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2661 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2737 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2635 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2683 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2428 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2368 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2404 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2023-04-29 08:02:41.000000 trytond_product_attribute-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6051 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:16.642916 trytond_product_attribute-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4257 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:16.636249 trytond_product_attribute-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-05-01 11:01:34.000000 trytond_product_attribute-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:16.642916 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2620 2023-05-01 11:42:15.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1799 2023-05-01 11:42:16.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:15.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:42:15.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-05-01 11:42:15.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:15.000000 trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:16.639582 trytond_product_attribute-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      789 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/attribute_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/attribute_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_product_attribute-6.8.0/view/attribute_set_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/product_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:20.000000 trytond_product_attribute-6.8.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-04-15 07:12:15.000000 trytond_product_attribute-6.8.0/view/template_tree.xml
```

### Comparing `trytond_product_attribute-6.6.0/CHANGELOG` & `trytond_product_attribute-6.8.0/CHANGELOG`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_product_attribute-6.6.0/COPYRIGHT` & `trytond_product_attribute-6.8.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2012-2022 Cédric Krier.
-Copyright (C) 2012-2022 B2CK SPRL.
+Copyright (C) 2012-2023 Cédric Krier.
+Copyright (C) 2012-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_attribute-6.6.0/LICENSE` & `trytond_product_attribute-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/PKG-INFO` & `trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_product_attribute
-Version: 6.6.0
+Name: trytond-product-attribute
+Version: 6.8.0
 Summary: Tryton module with product attributes
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_attribute
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product attribute
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
 
 Product Attribute Module
 ########################
 
 The Product Attribute module defines the following models: Attribute and
 Attribute Set.
```

### Comparing `trytond_product_attribute-6.6.0/locale/bg.po` & `trytond_product_attribute-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/ca.po` & `trytond_product_attribute-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/cs.po` & `trytond_product_attribute-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/de.po` & `trytond_product_attribute-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/es.po` & `trytond_product_attribute-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/es_419.po` & `trytond_product_attribute-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/et.po` & `trytond_product_attribute-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/fa.po` & `trytond_product_attribute-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/fi.po` & `trytond_product_attribute-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/fr.po` & `trytond_product_attribute-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/hu.po` & `trytond_product_attribute-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/id.po` & `trytond_product_attribute-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/it.po` & `trytond_product_attribute-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/lo.po` & `trytond_product_attribute-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/lt.po` & `trytond_product_attribute-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/nl.po` & `trytond_product_attribute-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/pl.po` & `trytond_product_attribute-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/pt.po` & `trytond_product_attribute-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/ro.po` & `trytond_product_attribute-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/ru.po` & `trytond_product_attribute-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/sl.po` & `trytond_product_attribute-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/tr.po` & `trytond_product_attribute-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/uk.po` & `trytond_product_attribute-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/locale/zh_CN.po` & `trytond_product_attribute-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/product.py` & `trytond_product_attribute-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/product.xml` & `trytond_product_attribute-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/setup.py` & `trytond_product_attribute-6.8.0/setup.py`

 * *Files 6% similar despite different names*

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
 name = 'trytond_product_attribute'
 
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
     description='Tryton module with product attributes',
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
-        "Source Code": 'https://hg.tryton.org/modules/product_attribute',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product attribute',
     package_dir={'trytond.modules.product_attribute': '.'},
     packages=(
         ['trytond.modules.product_attribute']
         + ['trytond.modules.product_attribute.%s' % p for p in find_packages()]
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
     product_attribute = trytond.modules.product_attribute
     """,
     )
```

### Comparing `trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/PKG-INFO` & `trytond_product_attribute-6.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-product-attribute
-Version: 6.6.0
+Name: trytond_product_attribute
+Version: 6.8.0
 Summary: Tryton module with product attributes
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_attribute
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product attribute
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
 
 Product Attribute Module
 ########################
 
 The Product Attribute module defines the following models: Attribute and
 Attribute Set.
```

### Comparing `trytond_product_attribute-6.6.0/trytond_product_attribute.egg-info/SOURCES.txt` & `trytond_product_attribute-6.8.0/trytond_product_attribute.egg-info/SOURCES.txt`

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
 message.xml
@@ -50,14 +46,15 @@
 ./view/attribute_list_simple.xml
 ./view/attribute_set_form.xml
 ./view/attribute_set_list.xml
 ./view/product_form.xml
 ./view/product_tree.xml
 ./view/template_form.xml
 ./view/template_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_product_attribute-6.6.0/view/attribute_form.xml` & `trytond_product_attribute-6.8.0/view/attribute_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_attribute-6.6.0/view/product_form.xml` & `trytond_product_attribute-6.8.0/view/product_form.xml`

 * *Files identical despite different names*

