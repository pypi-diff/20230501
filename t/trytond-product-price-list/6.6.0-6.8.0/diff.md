# Comparing `tmp/trytond_product_price_list-6.6.0.tar.gz` & `tmp/trytond_product_price_list-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_price_list-6.6.0.tar", last modified: Mon Oct 31 15:53:48 2022, max compression
+gzip compressed data, was "trytond_product_price_list-6.8.0.tar", last modified: Mon May  1 11:37:37 2023, max compression
```

## Comparing `trytond_product_price_list-6.6.0.tar` & `trytond_product_price_list-6.8.0.tar`

### file list

```diff
@@ -1,64 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:53:48.368418 trytond_product_price_list-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_product_price_list-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_product_price_list-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-10-31 15:53:47.000000 trytond_product_price_list-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_product_price_list-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2493 2022-10-31 15:53:46.000000 trytond_product_price_list-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:53:45.000000 trytond_product_price_list-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:36.000000 trytond_product_price_list-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_product_price_list-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2349 2022-10-31 15:53:48.365085 trytond_product_price_list-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2019-06-04 16:49:45.000000 trytond_product_price_list-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2021-12-11 16:59:33.000000 trytond_product_price_list-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:53:48.365085 trytond_product_price_list-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2019-06-04 16:49:45.000000 trytond_product_price_list-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2019-06-04 16:49:45.000000 trytond_product_price_list-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:53:48.361751 trytond_product_price_list-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3082 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3603 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3643 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2991 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3792 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3744 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3587 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2803 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2847 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2806 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3674 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2991 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3536 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3715 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3028 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3353 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2781 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2719 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2796 2022-10-29 07:50:33.000000 trytond_product_price_list-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2019-10-11 23:09:48.000000 trytond_product_price_list-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7038 2022-10-11 19:49:58.000000 trytond_product_price_list-6.6.0/price_list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3923 2021-04-27 07:34:40.000000 trytond_product_price_list-6.6.0/price_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:53:48.368418 trytond_product_price_list-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5056 2022-10-29 07:39:11.000000 trytond_product_price_list-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:53:48.365085 trytond_product_price_list-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_product_price_list-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8446 2022-04-16 16:30:56.000000 trytond_product_price_list-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2022-10-31 15:10:09.000000 trytond_product_price_list-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-31 15:53:45.000000 trytond_product_price_list-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:53:48.365085 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2349 2022-10-31 15:53:47.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1714 2022-10-31 15:53:48.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:53:47.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 15:53:47.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:49.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2022-10-31 15:53:47.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:53:47.000000 trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:53:48.365085 trytond_product_price_list-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      816 2019-10-11 23:09:48.000000 trytond_product_price_list-6.6.0/view/price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      615 2019-10-11 23:09:48.000000 trytond_product_price_list-6.6.0/view/price_list_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2022-04-08 16:23:26.000000 trytond_product_price_list-6.6.0/view/price_list_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2022-04-08 16:23:26.000000 trytond_product_price_list-6.6.0/view/price_list_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-04-08 16:23:26.000000 trytond_product_price_list-6.6.0/view/price_list_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:37.502785 trytond_product_price_list-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2656 2023-05-01 10:58:32.000000 trytond_product_price_list-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 10:58:32.000000 trytond_product_price_list-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_price_list-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-05-01 11:37:37.502785 trytond_product_price_list-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:37.499451 trytond_product_price_list-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:37.496118 trytond_product_price_list-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3121 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2833 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3802 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3119 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3030 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3840 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3839 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3635 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2842 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2886 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3110 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3768 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3030 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3584 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3799 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3067 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3401 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2758 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-04-30 10:46:36.000000 trytond_product_price_list-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7091 2023-04-22 08:56:15.000000 trytond_product_price_list-6.8.0/price_list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3923 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/price_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:37:37.502785 trytond_product_price_list-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4241 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:37.496118 trytond_product_price_list-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8446 2023-04-22 08:56:15.000000 trytond_product_price_list-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 10:58:26.000000 trytond_product_price_list-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:37.502785 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2338 2023-05-01 11:37:36.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1688 2023-05-01 11:37:37.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:37:36.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:37:36.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2023-05-01 11:37:36.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:37:36.000000 trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:37.499451 trytond_product_price_list-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      816 2023-04-22 08:56:15.000000 trytond_product_price_list-6.8.0/view/price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      615 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/view/price_list_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/view/price_list_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/view/price_list_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_product_price_list-6.8.0/view/price_list_tree.xml
```

### Comparing `trytond_product_price_list-6.6.0/CHANGELOG` & `trytond_product_price_list-6.8.0/CHANGELOG`

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

### Comparing `trytond_product_price_list-6.6.0/COPYRIGHT` & `trytond_product_price_list-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2022 Cédric Krier.
+Copyright (C) 2009-2023 Cédric Krier.
 Copyright (C) 2009-2013 Bertrand Chenal.
-Copyright (C) 2009-2022 B2CK SPRL.
+Copyright (C) 2009-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_product_price_list-6.6.0/LICENSE` & `trytond_product_price_list-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-6.6.0/PKG-INFO` & `trytond_product_price_list-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_product_price_list
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with price list
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_price_list
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product price list
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
 License-File: LICENSE
 
 Product Price List Module
 #########################
 
 The product price list module provides formula to compute prices per product or
 category.
```

### Comparing `trytond_product_price_list-6.6.0/locale/bg.po` & `trytond_product_price_list-6.8.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/ca.po` & `trytond_product_price_list-6.8.0/locale/ca.po`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Fes que la tarifa pertanyi a l'empresa.\n"
 "Defineix la moneda de la tarifa."
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
-msgstr "Afegiu formules de preu per diferents criteris."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
+msgstr ""
+"Afegiu formules de preu per diferents criteris.\n"
+"S'utilitza la primera linia que coincideix."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "El identificador principal de la tarifa."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
```

### Comparing `trytond_product_price_list-6.6.0/locale/cs.po` & `trytond_product_price_list-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/de.po` & `trytond_product_price_list-6.8.0/locale/de.po`

 * *Files 3% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Die Preisliste dem Unternehmen zuordnen.\n"
 "Dies definiert die Währung der Preisliste."
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
-msgstr "Preisformeln für verschiedene Kriterien hinzufügen."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
+msgstr ""
+"Erlaubt die Erfassung von Preisformeln für unterschiedliche Kriterien.\n"
+"Die erste Zeile mit übereinstimmenden Kriterien wird verwendet."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "Das Hauptidentifizierungsmerkmal der Preisliste."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
```

### Comparing `trytond_product_price_list-6.6.0/locale/es.po` & `trytond_product_price_list-6.8.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Hacer que la tarifa pertenezca a la empresa.\n"
 "Define la moneda de la tarifa."
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
-msgstr "Añadir formulas de precio por distintos criterios."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
+msgstr ""
+"Añadir formulas de precio por distintos criterios.\n"
+"Se utiliza la primera línea que coincide."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "El identificador principal de la tarifa."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
```

### Comparing `trytond_product_price_list-6.6.0/locale/es_419.po` & `trytond_product_price_list-6.8.0/locale/lt.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.price_list,company:"
 msgid "Company"
-msgstr ""
+msgstr "Organizacija"
 
 msgctxt "field:product.price_list,lines:"
 msgid "Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.price_list,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:product.price_list,tax_included:"
 msgid "Tax Included"
-msgstr "Impuesto incluido"
+msgstr ""
 
 msgctxt "field:product.price_list,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:product.price_list.line,category:"
 msgid "Category"
 msgstr ""
 
 msgctxt "field:product.price_list.line,formula:"
 msgid "Formula"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:product.price_list.line,price_list:"
 msgid "Price List"
-msgstr "Lista de precios"
+msgstr "Price Lists"
 
 msgctxt "field:product.price_list.line,product:"
 msgid "Product"
 msgstr ""
 
 msgctxt "field:product.price_list.line,quantity:"
 msgid "Quantity"
@@ -45,15 +47,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
@@ -64,64 +68,57 @@
 msgid "The unit in which the quantity is expressed."
 msgstr ""
 
 msgctxt "help:product.price_list.line,category:"
 msgid "Apply only to products of this category."
 msgstr ""
 
-#, fuzzy
 msgctxt "help:product.price_list.line,formula:"
 msgid ""
 "Python expression that will be evaluated with:\n"
 "- unit_price: the original unit_price\n"
 "- cost_price: the cost price of the product\n"
 "- list_price: the list price of the product"
 msgstr ""
-"Expresión de Python que se evaluará con:\n"
-"- unit_price: el precio unitario original"
 
 msgctxt "help:product.price_list.line,price_list:"
 msgid "The price list to which the line belongs."
 msgstr ""
 
 msgctxt "help:product.price_list.line,product:"
 msgid "Apply only to this product."
 msgstr ""
 
 msgctxt "help:product.price_list.line,quantity:"
 msgid "Apply only when quantity is greater."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_price_list_form"
 msgid "Price Lists"
-msgstr "Lista de precios"
+msgstr "Price Lists"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in price list line \"%(line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
-"La fórmula \"%(formula)s\" en la línea de lista de precios \"%(line)s\" con "
-"excepción \"%(exception)s\" no es válida."
 
 msgctxt "model:ir.rule.group,name:rule_group_price_list_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_price_list"
 msgid "Price Lists"
-msgstr "Lista de precios"
+msgstr "Price Lists"
 
+#, fuzzy
 msgctxt "model:product.price_list,name:"
 msgid "Price List"
-msgstr "Lista de precios"
+msgstr "Price Lists"
 
 msgctxt "model:product.price_list.line,name:"
 msgid "Price List Line"
-msgstr "Línea de lista de precios"
+msgstr ""
 
 msgctxt "selection:product.price_list,unit:"
 msgid "Product Default"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_product_price_list-6.6.0/locale/et.po` & `trytond_product_price_list-6.8.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/fa.po` & `trytond_product_price_list-6.8.0/locale/fa.po`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,19 @@
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "ساختن لیست قیمت متعلق به شرکت.\n"
 "این ارز از لیست قیمت تعریف می کند."
 
+#, fuzzy
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr "فرمول قیمت را برای معیارهای مختلف اضافه کنید."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "شناسه اصلی لیست قیمت."
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/fi.po` & `trytond_product_price_list-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/fr.po` & `trytond_product_price_list-6.8.0/locale/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Faire appartenir la liste de prix à la société.\n"
 "Ça définit la devise de la liste de prix."
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
-msgstr "Ajouter des formules de prix pour différents critères."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
+msgstr ""
+"Ajouter des formules de prix pour différents critères.\n"
+"La première ligne correspondante est utilisée."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "L'identifiant principal de la liste de prix."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
```

### Comparing `trytond_product_price_list-6.6.0/locale/hu.po` & `trytond_product_price_list-6.8.0/locale/hu.po`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,19 @@
 
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 "Az árszámításhoz használt képleteket adhatja itt meg, különböző "
 "feltételekkel."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "Az árlista megnevezése."
```

### Comparing `trytond_product_price_list-6.6.0/locale/id.po` & `trytond_product_price_list-6.8.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/it.po` & `trytond_product_price_list-6.8.0/locale/it.po`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/lo.po` & `trytond_product_price_list-6.8.0/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/lt.po` & `trytond_product_price_list-6.8.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.price_list,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr ""
 
 msgctxt "field:product.price_list,lines:"
 msgid "Lines"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.price_list,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr "纳木"
 
 msgctxt "field:product.price_list,tax_included:"
 msgid "Tax Included"
 msgstr ""
 
 msgctxt "field:product.price_list,unit:"
 msgid "Unit"
@@ -47,15 +47,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_product_price_list-6.6.0/locale/nl.po` & `trytond_product_price_list-6.8.0/locale/nl.po`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Koppel de prijslijst aan het bedrijf.\n"
 "Dit definieert de valuta van de prijslijst."
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
-msgstr "Voeg prijs formules toe voor verschillende criteria."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
+msgstr ""
+"Voeg prijs formules toe voor verschillende criteria.\n"
+"De eerste regel die overeenkomt wordt gebruikt."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "De hoofdidentificatie van de prijslijst."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
```

### Comparing `trytond_product_price_list-6.6.0/locale/pl.po` & `trytond_product_price_list-6.8.0/locale/pl.po`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "Główny identyfikator cennika."
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/pt.po` & `trytond_product_price_list-6.8.0/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,19 @@
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Faça com que o preço de tabela pertença à empresa.\n"
 "Isto define a moeda do preço de tabela."
 
+#, fuzzy
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr "Adiciona fórmulas de preço para diversos critérios."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "O identificador principal do preço de tabela."
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/ro.po` & `trytond_product_price_list-6.8.0/locale/ro.po`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 "Faceți ca lista de prețuri să aparțină companiei.\n"
 "Acesta definește moneda listei de prețuri."
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
-msgstr "Adăugați formule de preț pentru diferite criterii."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
+msgstr ""
+"Adăugați formule preţuri pentru diferite criterii.\n"
+"Primul rând potrivit va fi utilizat."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "Identificatorul principal al listei de prețuri."
 
 msgctxt "help:product.price_list,tax_included:"
 msgid "Check if result's formula includes taxes."
```

### Comparing `trytond_product_price_list-6.6.0/locale/ru.po` & `trytond_product_price_list-6.8.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/sl.po` & `trytond_product_price_list-6.8.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,19 @@
 
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr "Poveži cenik z družbo, ki s tem določa tudi valuto cenika."
 
+#, fuzzy
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr "Dodaj formule cen za različne kriterije."
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr "Glavni identifikator cenika."
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/tr.po` & `trytond_product_price_list-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/uk.po` & `trytond_product_price_list-6.8.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
```

### Comparing `trytond_product_price_list-6.6.0/locale/zh_CN.po` & `trytond_product_price_list-6.8.0/locale/es_419.po`

 * *Files 7% similar despite different names*

```diff
@@ -6,39 +6,37 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:product.price_list,lines:"
 msgid "Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.price_list,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr ""
 
 msgctxt "field:product.price_list,tax_included:"
 msgid "Tax Included"
-msgstr ""
+msgstr "Impuesto incluido"
 
 msgctxt "field:product.price_list,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:product.price_list.line,category:"
 msgid "Category"
 msgstr ""
 
 msgctxt "field:product.price_list.line,formula:"
 msgid "Formula"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:product.price_list.line,price_list:"
 msgid "Price List"
-msgstr "Price Lists"
+msgstr "Lista de precios"
 
 msgctxt "field:product.price_list.line,product:"
 msgid "Product"
 msgstr ""
 
 msgctxt "field:product.price_list.line,quantity:"
 msgid "Quantity"
@@ -47,15 +45,17 @@
 msgctxt "help:product.price_list,company:"
 msgid ""
 "Make the price list belong to the company.\n"
 "It defines the currency of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,lines:"
-msgid "Add price formulas for different criterias."
+msgid ""
+"Add price formulas for different criteria.\n"
+"The first matching line is used."
 msgstr ""
 
 msgctxt "help:product.price_list,name:"
 msgid "The main identifier of the price list."
 msgstr ""
 
 msgctxt "help:product.price_list,tax_included:"
@@ -66,57 +66,64 @@
 msgid "The unit in which the quantity is expressed."
 msgstr ""
 
 msgctxt "help:product.price_list.line,category:"
 msgid "Apply only to products of this category."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:product.price_list.line,formula:"
 msgid ""
 "Python expression that will be evaluated with:\n"
 "- unit_price: the original unit_price\n"
 "- cost_price: the cost price of the product\n"
 "- list_price: the list price of the product"
 msgstr ""
+"Expresión de Python que se evaluará con:\n"
+"- unit_price: el precio unitario original"
 
 msgctxt "help:product.price_list.line,price_list:"
 msgid "The price list to which the line belongs."
 msgstr ""
 
 msgctxt "help:product.price_list.line,product:"
 msgid "Apply only to this product."
 msgstr ""
 
 msgctxt "help:product.price_list.line,quantity:"
 msgid "Apply only when quantity is greater."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_price_list_form"
 msgid "Price Lists"
-msgstr "Price Lists"
+msgstr "Lista de precios"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_invalid_formula"
 msgid ""
 "Invalid formula \"%(formula)s\" in price list line \"%(line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
+"La fórmula \"%(formula)s\" en la línea de lista de precios \"%(line)s\" con "
+"excepción \"%(exception)s\" no es válida."
 
 msgctxt "model:ir.rule.group,name:rule_group_price_list_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_price_list"
 msgid "Price Lists"
-msgstr "Price Lists"
+msgstr "Lista de precios"
 
-#, fuzzy
 msgctxt "model:product.price_list,name:"
 msgid "Price List"
-msgstr "Price Lists"
+msgstr "Lista de precios"
 
 msgctxt "model:product.price_list.line,name:"
 msgid "Price List Line"
-msgstr ""
+msgstr "Línea de lista de precios"
 
 msgctxt "selection:product.price_list,unit:"
 msgid "Product Default"
 msgstr ""
```

### Comparing `trytond_product_price_list-6.6.0/price_list.py` & `trytond_product_price_list-6.8.0/price_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,18 @@
         "It defines the currency of the price list.")
     tax_included = fields.Boolean('Tax Included',
         help="Check if result's formula includes taxes.")
     unit = fields.Selection([
             ('product_default', "Product Default"),
             ], "Unit", required=True,
         help="The unit in which the quantity is expressed.")
-    lines = fields.One2Many('product.price_list.line', 'price_list', 'Lines',
-        help="Add price formulas for different criterias.")
+    lines = fields.One2Many(
+        'product.price_list.line', 'price_list', "Lines",
+        help="Add price formulas for different criteria.\n"
+        "The first matching line is used.")
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @staticmethod
     def default_tax_included():
```

### Comparing `trytond_product_price_list-6.6.0/price_list.xml` & `trytond_product_price_list-6.8.0/price_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-6.6.0/setup.py` & `trytond_product_price_list-6.8.0/setup.py`

 * *Files 13% similar despite different names*

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
 name = 'trytond_product_price_list'
 
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
     description='Tryton module with price list',
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
-        "Source Code": 'https://hg.tryton.org/modules/product_price_list',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product price list',
     package_dir={'trytond.modules.product_price_list': '.'},
     packages=(
         ['trytond.modules.product_price_list']
         + ['trytond.modules.product_price_list.%s' % p
             for p in find_packages()]
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
     product_price_list = trytond.modules.product_price_list
     """,
     )
```

### Comparing `trytond_product_price_list-6.6.0/tests/test_module.py` & `trytond_product_price_list-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/PKG-INFO` & `trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-product-price-list
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with price list
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
-Project-URL: Source Code, https://hg.tryton.org/modules/product_price_list
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product price list
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
 License-File: LICENSE
 
 Product Price List Module
 #########################
 
 The product price list module provides formula to compute prices per product or
 category.
```

### Comparing `trytond_product_price_list-6.6.0/trytond_product_price_list.egg-info/SOURCES.txt` & `trytond_product_price_list-6.8.0/trytond_product_price_list.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
@@ -48,14 +44,15 @@
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/price_list_form.xml
 ./view/price_list_line_form.xml
 ./view/price_list_line_tree.xml
 ./view/price_list_line_tree_sequence.xml
 ./view/price_list_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_product_price_list-6.6.0/view/price_list_form.xml` & `trytond_product_price_list-6.8.0/view/price_list_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_price_list-6.6.0/view/price_list_line_form.xml` & `trytond_product_price_list-6.8.0/view/price_list_line_form.xml`

 * *Files identical despite different names*

