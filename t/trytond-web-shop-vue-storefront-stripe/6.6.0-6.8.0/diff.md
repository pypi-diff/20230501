# Comparing `tmp/trytond_web_shop_vue_storefront_stripe-6.6.0.tar.gz` & `tmp/trytond_web_shop_vue_storefront_stripe-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_vue_storefront_stripe-6.6.0.tar", last modified: Mon Oct 31 16:26:02 2022, max compression
+gzip compressed data, was "trytond_web_shop_vue_storefront_stripe-6.8.0.tar", last modified: Mon May  1 11:36:28 2023, max compression
```

## Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0.tar` & `trytond_web_shop_vue_storefront_stripe-6.8.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:02.896912 trytond_web_shop_vue_storefront_stripe-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2022-10-31 16:26:01.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:35.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-10-31 16:26:00.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:26:00.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2020-10-12 16:25:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2577 2022-10-31 16:26:02.896912 trytond_web_shop_vue_storefront_stripe-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2020-10-12 16:25:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2020-10-12 16:25:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:02.893579 trytond_web_shop_vue_storefront_stripe-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2020-10-12 16:25:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:02.893579 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      149 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      161 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2022-10-29 07:50:32.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:26:02.896912 trytond_web_shop_vue_storefront_stripe-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5435 2022-10-29 07:39:12.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:02.893579 trytond_web_shop_vue_storefront_stripe-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:58.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2022-04-16 16:30:58.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2022-10-31 15:10:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-10-31 16:25:59.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:02.896912 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2577 2022-10-31 16:26:02.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1446 2022-10-31 16:26:02.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:26:02.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2022-10-31 16:26:02.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-10-13 07:23:31.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2022-10-31 16:26:02.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:26:02.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:26:02.893579 trytond_web_shop_vue_storefront_stripe-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2020-10-12 16:25:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2021-12-11 16:59:35.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2020-10-12 16:25:09.000000 trytond_web_shop_vue_storefront_stripe-6.6.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:28.548596 trytond_web_shop_vue_storefront_stripe-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-05-01 10:57:45.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:57:45.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-05-01 11:36:28.548596 trytond_web_shop_vue_storefront_stripe-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:28.545262 trytond_web_shop_vue_storefront_stripe-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:28.545262 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      149 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      161 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-29 08:02:39.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:36:28.548596 trytond_web_shop_vue_storefront_stripe-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4594 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:28.545262 trytond_web_shop_vue_storefront_stripe-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 10:57:38.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:28.548596 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-05-01 11:36:27.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-05-01 11:36:28.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:36:27.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-05-01 11:36:27.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-05-01 11:36:27.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:36:27.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:28.545262 trytond_web_shop_vue_storefront_stripe-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_web_shop_vue_storefront_stripe-6.8.0/web.xml
```

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/COPYRIGHT` & `trytond_web_shop_vue_storefront_stripe-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2022 Cédric Krier
-Copyright (C) 2020-2022 B2CK
+Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/LICENSE` & `trytond_web_shop_vue_storefront_stripe-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/PKG-INFO` & `trytond_web_shop_vue_storefront_stripe-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_vue_storefront_stripe
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to support Stripe payment with Vue Storefront
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
-Project-URL: Source Code, https://hg.tryton.org/modules/web_shop_vue_storefront_stripe
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web vue storefront PWA ecommerce Stripe
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
 
 Web Shop Vue Storefront Stripe Module
 #####################################
 
 The web_shop_vue_storefront_stripe module provides support of `Stripe payment
```

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/setup.py` & `trytond_web_shop_vue_storefront_stripe-6.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     if slice:
         content = '\n'.join(content.splitlines()[slice])
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
@@ -37,61 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_web_shop_vue_storefront_stripe'
 
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
 
 tests_require = []
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to support Stripe payment with Vue Storefront',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/web_shop_vue_storefront_stripe'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='web vue storefront PWA ecommerce Stripe',
     package_dir={'trytond.modules.web_shop_vue_storefront_stripe': '.'},
     packages=(
         ['trytond.modules.web_shop_vue_storefront_stripe']
         + ['trytond.modules.web_shop_vue_storefront_stripe.%s' % p
             for p in find_packages()]
@@ -129,27 +106,26 @@
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
     web_shop_vue_storefront_stripe = trytond.modules.web_shop_vue_storefront_stripe
     """,  # noqa: E501
     )
```

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/PKG-INFO` & `trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-web-shop-vue-storefront-stripe
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to support Stripe payment with Vue Storefront
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
-Project-URL: Source Code, https://hg.tryton.org/modules/web_shop_vue_storefront_stripe
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web vue storefront PWA ecommerce Stripe
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
 
 Web Shop Vue Storefront Stripe Module
 #####################################
 
 The web_shop_vue_storefront_stripe module provides support of `Stripe payment
```

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/trytond_web_shop_vue_storefront_stripe.egg-info/SOURCES.txt` & `trytond_web_shop_vue_storefront_stripe-6.8.0/trytond_web_shop_vue_storefront_stripe.egg-info/SOURCES.txt`

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
 setup.py
@@ -40,14 +36,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/shop_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_web_shop_vue_storefront_stripe-6.6.0/web.py` & `trytond_web_shop_vue_storefront_stripe-6.8.0/web.py`

 * *Files identical despite different names*

