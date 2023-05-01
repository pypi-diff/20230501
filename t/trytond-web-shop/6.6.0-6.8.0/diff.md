# Comparing `tmp/trytond_web_shop-6.6.0.tar.gz` & `tmp/trytond_web_shop-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop-6.6.0.tar", last modified: Mon Oct 31 16:13:55 2022, max compression
+gzip compressed data, was "trytond_web_shop-6.8.0.tar", last modified: Mon May  1 11:48:36 2023, max compression
```

## Comparing `trytond_web_shop-6.6.0.tar` & `trytond_web_shop-6.8.0.tar`

### file list

```diff
@@ -1,73 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:13:55.532636 trytond_web_shop-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_web_shop-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_web_shop-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2022-10-31 16:13:54.000000 trytond_web_shop-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:35.000000 trytond_web_shop-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2022-10-31 16:13:53.000000 trytond_web_shop-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2022-10-31 16:13:53.000000 trytond_web_shop-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_web_shop-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2257 2022-10-31 16:13:55.532636 trytond_web_shop-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      817 2021-12-11 16:59:35.000000 trytond_web_shop-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:13:55.532636 trytond_web_shop-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:13:55.529303 trytond_web_shop-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5535 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5712 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5583 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5795 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4812 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4565 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4556 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5690 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6492 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2022-10-29 07:50:38.000000 trytond_web_shop-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1536 2022-04-10 15:40:36.000000 trytond_web_shop-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2021-10-30 15:32:33.000000 trytond_web_shop-6.6.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2022-09-19 19:26:12.000000 trytond_web_shop-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:13:55.532636 trytond_web_shop-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5219 2022-10-29 07:39:12.000000 trytond_web_shop-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:13:55.529303 trytond_web_shop-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:58.000000 trytond_web_shop-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2022-04-16 16:30:58.000000 trytond_web_shop-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2022-10-31 15:10:09.000000 trytond_web_shop-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2022-10-31 16:13:52.000000 trytond_web_shop-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:13:55.532636 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2257 2022-10-31 16:13:54.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1958 2022-10-31 16:13:55.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:13:54.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2022-10-31 16:13:54.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-10-13 07:23:31.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      273 2022-10-31 16:13:54.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:13:54.000000 trytond_web_shop-6.6.0/trytond_web_shop.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:13:55.532636 trytond_web_shop-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/product_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/product_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2021-10-07 13:08:07.000000 trytond_web_shop-6.6.0/view/product_image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2021-10-07 13:08:07.000000 trytond_web_shop-6.6.0/view/product_image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/product_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2021-10-30 15:32:33.000000 trytond_web_shop-6.6.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/shop_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-04-08 16:23:27.000000 trytond_web_shop-6.6.0/view/shop_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2020-10-12 16:25:09.000000 trytond_web_shop-6.6.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    10812 2022-10-11 19:49:59.000000 trytond_web_shop-6.6.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3395 2021-04-27 07:34:41.000000 trytond_web_shop-6.6.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:36.217626 trytond_web_shop-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-05-01 11:05:45.000000 trytond_web_shop-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 11:05:45.000000 trytond_web_shop-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2023-05-01 11:48:36.217626 trytond_web_shop-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      817 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:36.214293 trytond_web_shop-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:36.207626 trytond_web_shop-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5535 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5712 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5583 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5795 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4812 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4565 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4556 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5690 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6492 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-04-29 08:02:45.000000 trytond_web_shop-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1536 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:48:36.217626 trytond_web_shop-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4415 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:36.210959 trytond_web_shop-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-05-01 11:05:39.000000 trytond_web_shop-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:36.217626 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2023-05-01 11:48:35.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1932 2023-05-01 11:48:36.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:48:35.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-01 11:48:35.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      273 2023-05-01 11:48:35.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:48:35.000000 trytond_web_shop-6.8.0/trytond_web_shop.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:48:36.214293 trytond_web_shop-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/product_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/product_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/product_image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/product_image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/product_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/shop_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/shop_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10812 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3395 2023-04-15 07:12:15.000000 trytond_web_shop-6.8.0/web.xml
```

### Comparing `trytond_web_shop-6.6.0/COPYRIGHT` & `trytond_web_shop-6.8.0/COPYRIGHT`

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

### Comparing `trytond_web_shop-6.6.0/LICENSE` & `trytond_web_shop-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/PKG-INFO` & `trytond_web_shop-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module that provides a common base for webshops
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
-Project-URL: Source Code, https://hg.tryton.org/modules/web_shop
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: webshop ecommerce
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Web Shop Module
 ###############
 
 The web_shop module provides facilities to store configuration of online web
```

### Comparing `trytond_web_shop-6.6.0/__init__.py` & `trytond_web_shop-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/bg.po` & `trytond_web_shop-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/ca.po` & `trytond_web_shop-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/cs.po` & `trytond_web_shop-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/de.po` & `trytond_web_shop-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/es.po` & `trytond_web_shop-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/es_419.po` & `trytond_web_shop-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/et.po` & `trytond_web_shop-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/fa.po` & `trytond_web_shop-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/fi.po` & `trytond_web_shop-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/fr.po` & `trytond_web_shop-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/hu.po` & `trytond_web_shop-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/id.po` & `trytond_web_shop-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/it.po` & `trytond_web_shop-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/lo.po` & `trytond_web_shop-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/lt.po` & `trytond_web_shop-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/nl.po` & `trytond_web_shop-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/pl.po` & `trytond_web_shop-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/pt.po` & `trytond_web_shop-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/ro.po` & `trytond_web_shop-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/ru.po` & `trytond_web_shop-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/sl.po` & `trytond_web_shop-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/tr.po` & `trytond_web_shop-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/uk.po` & `trytond_web_shop-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/locale/zh_CN.po` & `trytond_web_shop-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/message.xml` & `trytond_web_shop-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/product.py` & `trytond_web_shop-6.8.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/product.xml` & `trytond_web_shop-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/sale.py` & `trytond_web_shop-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/setup.py` & `trytond_web_shop-6.8.0/setup.py`

 * *Files 16% similar despite different names*

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
@@ -37,63 +34,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_web_shop'
 
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
 
 tests_require = [
     get_require_version('trytond_product_attribute'),
     get_require_version('trytond_product_image'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module that provides a common base for webshops',
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
-        "Source Code": 'https://hg.tryton.org/modules/web_shop',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='webshop ecommerce',
     package_dir={'trytond.modules.web_shop': '.'},
     packages=(
         ['trytond.modules.web_shop']
         + ['trytond.modules.web_shop.%s' % p for p in find_packages()]
         ),
@@ -128,27 +106,26 @@
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
     web_shop = trytond.modules.web_shop
     """,
     )
```

### Comparing `trytond_web_shop-6.6.0/trytond_web_shop.egg-info/PKG-INFO` & `trytond_web_shop-6.8.0/trytond_web_shop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-web-shop
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module that provides a common base for webshops
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
-Project-URL: Source Code, https://hg.tryton.org/modules/web_shop
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: webshop ecommerce
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -36,21 +36,21 @@
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
 
 Web Shop Module
 ###############
 
 The web_shop module provides facilities to store configuration of online web
```

### Comparing `trytond_web_shop-6.6.0/trytond_web_shop.egg-info/SOURCES.txt` & `trytond_web_shop-6.8.0/trytond_web_shop.egg-info/SOURCES.txt`

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
@@ -60,14 +56,15 @@
 ./view/product_product_form.xml
 ./view/product_template_form.xml
 ./view/sale_form.xml
 ./view/shop_attribute_form.xml
 ./view/shop_form.xml
 ./view/shop_list.xml
 ./view/user_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_web_shop-6.6.0/view/shop_form.xml` & `trytond_web_shop-6.8.0/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/web.py` & `trytond_web_shop-6.8.0/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-6.6.0/web.xml` & `trytond_web_shop-6.8.0/web.xml`

 * *Files identical despite different names*

