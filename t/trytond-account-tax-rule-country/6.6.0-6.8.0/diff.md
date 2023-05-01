# Comparing `tmp/trytond_account_tax_rule_country-6.6.0.tar.gz` & `tmp/trytond_account_tax_rule_country-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_tax_rule_country-6.6.0.tar", last modified: Mon Oct 31 16:23:11 2022, max compression
+gzip compressed data, was "trytond_account_tax_rule_country-6.8.0.tar", last modified: Mon May  1 12:00:58 2023, max compression
```

## Comparing `trytond_account_tax_rule_country-6.6.0.tar` & `trytond_account_tax_rule_country-6.8.0.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:11.847680 trytond_account_tax_rule_country-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_tax_rule_country-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_tax_rule_country-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-31 16:23:10.000000 trytond_account_tax_rule_country-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_tax_rule_country-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1380 2022-10-31 16:23:09.000000 trytond_account_tax_rule_country-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:23:09.000000 trytond_account_tax_rule_country-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:23.000000 trytond_account_tax_rule_country-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_tax_rule_country-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3432 2022-10-31 16:23:11.847680 trytond_account_tax_rule_country-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      972 2021-12-11 16:59:32.000000 trytond_account_tax_rule_country-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5630 2022-04-10 15:40:35.000000 trytond_account_tax_rule_country-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1750 2018-08-18 09:54:23.000000 trytond_account_tax_rule_country-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:11.847680 trytond_account_tax_rule_country-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:11.844347 trytond_account_tax_rule_country-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2262 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1758 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1786 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2260 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1774 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1836 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1764 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2212 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1772 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1734 2022-10-29 07:50:43.000000 trytond_account_tax_rule_country-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1701 2022-04-10 15:40:35.000000 trytond_account_tax_rule_country-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1900 2022-04-10 15:40:35.000000 trytond_account_tax_rule_country-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:23:11.847680 trytond_account_tax_rule_country-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5378 2022-10-29 07:39:10.000000 trytond_account_tax_rule_country-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2021-12-11 16:59:32.000000 trytond_account_tax_rule_country-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:11.844347 trytond_account_tax_rule_country-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_tax_rule_country-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6344 2022-04-16 16:30:56.000000 trytond_account_tax_rule_country-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2022-10-31 15:10:09.000000 trytond_account_tax_rule_country-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2022-10-31 16:23:08.000000 trytond_account_tax_rule_country-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:11.847680 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3432 2022-10-31 16:23:11.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1788 2022-10-31 16:23:11.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:23:11.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2022-10-31 16:23:11.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:12.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2022-10-31 16:23:11.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:23:11.000000 trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:23:11.847680 trytond_account_tax_rule_country-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2019-10-11 23:09:47.000000 trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_tree_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:58.210167 trytond_account_tax_rule_country-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 11:14:19.000000 trytond_account_tax_rule_country-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:14:19.000000 trytond_account_tax_rule_country-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_tax_rule_country-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3415 2023-05-01 12:00:58.210167 trytond_account_tax_rule_country-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5621 2023-04-28 07:46:16.000000 trytond_account_tax_rule_country-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1750 2023-01-16 14:00:20.000000 trytond_account_tax_rule_country-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:58.206834 trytond_account_tax_rule_country-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:58.203500 trytond_account_tax_rule_country-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2264 2023-04-30 10:46:36.000000 trytond_account_tax_rule_country-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1758 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1786 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2260 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1774 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1836 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1764 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2212 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1772 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1734 2023-04-29 08:02:49.000000 trytond_account_tax_rule_country-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-04-28 07:46:16.000000 trytond_account_tax_rule_country-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1598 2023-04-28 07:46:16.000000 trytond_account_tax_rule_country-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:00:58.210167 trytond_account_tax_rule_country-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4543 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:58.203500 trytond_account_tax_rule_country-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6344 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-05-01 11:14:12.000000 trytond_account_tax_rule_country-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:58.210167 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3415 2023-05-01 12:00:57.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1762 2023-05-01 12:00:58.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:00:57.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2023-05-01 12:00:57.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 12:00:57.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:00:57.000000 trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:00:58.206834 trytond_account_tax_rule_country-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-04-15 07:12:15.000000 trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_tree_sequence.xml
```

### Comparing `trytond_account_tax_rule_country-6.6.0/CHANGELOG` & `trytond_account_tax_rule_country-6.8.0/CHANGELOG`

 * *Files 12% similar despite different names*

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

### Comparing `trytond_account_tax_rule_country-6.6.0/COPYRIGHT` & `trytond_account_tax_rule_country-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2014-2022 Cédric Krier.
-Copyright (C) 2014-2022 B2CK SPRL.
+Copyright (C) 2014-2023 Cédric Krier.
+Copyright (C) 2014-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_tax_rule_country-6.6.0/LICENSE` & `trytond_account_tax_rule_country-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/PKG-INFO` & `trytond_account_tax_rule_country-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_tax_rule_country
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add countries on tax rules
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_tax_rule_country
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account tax rule country
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
 
 Account Tax Rule Country
 ########################
 
 The account_tax_rule module extends the tax rule to add origin and destination
```

### Comparing `trytond_account_tax_rule_country-6.6.0/README.rst` & `trytond_account_tax_rule_country-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/__init__.py` & `trytond_account_tax_rule_country-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/account.py` & `trytond_account_tax_rule_country-6.8.0/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             to_subdivision = shipment_address.subdivision
         elif (PurchaseLine
                 and isinstance(self.origin, PurchaseLine)
                 and self.origin.id >= 0):
             invoice_address = self.origin.purchase.invoice_address
             from_country = invoice_address.country
             from_subdivision = invoice_address.subdivision
-            warehouse = self.origin.purchase.warehouse
+            warehouse = self.origin.warehouse
             if warehouse and warehouse.address:
                 to_country = warehouse.address.country
                 to_subdivision = warehouse.address.subdivision
 
         pattern['from_country'] = from_country.id if from_country else None
         pattern['from_subdivision'] = (
             from_subdivision.id if from_subdivision else None)
```

### Comparing `trytond_account_tax_rule_country-6.6.0/account.xml` & `trytond_account_tax_rule_country-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/doc/index.rst` & `trytond_account_tax_rule_country-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/bg.po` & `trytond_account_tax_rule_country-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/ca.po` & `trytond_account_tax_rule_country-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/cs.po` & `trytond_account_tax_rule_country-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/de.po` & `trytond_account_tax_rule_country-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/es.po` & `trytond_account_tax_rule_country-6.8.0/locale/es.po`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 msgctxt "field:account.tax.rule.line,from_subdivision:"
 msgid "From Subdivision"
 msgstr "De la subdivisión"
 
 msgctxt "field:account.tax.rule.line,to_country:"
 msgid "To Country"
-msgstr "Para el país"
+msgstr "Hacia el país"
 
 msgctxt "field:account.tax.rule.line,to_subdivision:"
 msgid "To Subdivision"
 msgstr "A la subdivisión"
 
 msgctxt "field:account.tax.rule.line.template,from_country:"
 msgid "From Country"
@@ -24,15 +24,15 @@
 
 msgctxt "field:account.tax.rule.line.template,from_subdivision:"
 msgid "From Subdivision"
 msgstr "De la subdivisión"
 
 msgctxt "field:account.tax.rule.line.template,to_country:"
 msgid "To Country"
-msgstr "Para el país"
+msgstr "Hacia el país"
 
 msgctxt "field:account.tax.rule.line.template,to_subdivision:"
 msgid "To Subdivision"
 msgstr "A la subdivisión"
 
 msgctxt "help:account.tax.rule.line,from_country:"
 msgid "Apply only to addresses of this country."
```

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/es_419.po` & `trytond_account_tax_rule_country-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/et.po` & `trytond_account_tax_rule_country-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/fa.po` & `trytond_account_tax_rule_country-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/fi.po` & `trytond_account_tax_rule_country-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/fr.po` & `trytond_account_tax_rule_country-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/hu.po` & `trytond_account_tax_rule_country-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/id.po` & `trytond_account_tax_rule_country-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/it.po` & `trytond_account_tax_rule_country-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/lo.po` & `trytond_account_tax_rule_country-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/lt.po` & `trytond_account_tax_rule_country-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/nl.po` & `trytond_account_tax_rule_country-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/pl.po` & `trytond_account_tax_rule_country-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/pt.po` & `trytond_account_tax_rule_country-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/ro.po` & `trytond_account_tax_rule_country-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/ru.po` & `trytond_account_tax_rule_country-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/sl.po` & `trytond_account_tax_rule_country-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/tr.po` & `trytond_account_tax_rule_country-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/uk.po` & `trytond_account_tax_rule_country-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/locale/zh_CN.po` & `trytond_account_tax_rule_country-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/purchase.py` & `trytond_account_tax_rule_country-6.8.0/purchase.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,28 +16,27 @@
             field.states['readonly'] |= (
                 Eval('lines', [0]) & Eval('invoice_address'))
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'purchase.line'
 
-    @fields.depends('purchase', '_parent_purchase.warehouse',
-        '_parent_purchase.invoice_address')
+    @fields.depends(
+        'purchase', 'warehouse', '_parent_purchase.invoice_address')
     def _get_tax_rule_pattern(self):
         pattern = super()._get_tax_rule_pattern()
 
         from_country = from_subdivision = to_country = to_subdivision = None
         if self.purchase:
             if self.purchase.invoice_address:
                 from_country = self.purchase.invoice_address.country
                 from_subdivision = self.purchase.invoice_address.subdivision
-            warehouse = self.purchase.warehouse
-            if warehouse and warehouse.address:
-                to_country = warehouse.address.country
-                to_subdivision = warehouse.address.subdivision
+            if self.warehouse and self.warehouse.address:
+                to_country = self.warehouse.address.country
+                to_subdivision = self.warehouse.address.subdivision
 
         pattern['from_country'] = from_country.id if from_country else None
         pattern['from_subdivision'] = (
             from_subdivision.id if from_subdivision else None)
         pattern['to_country'] = to_country.id if to_country else None
         pattern['to_subdivision'] = (
             to_subdivision.id if to_subdivision else None)
```

### Comparing `trytond_account_tax_rule_country-6.6.0/sale.py` & `trytond_account_tax_rule_country-6.8.0/sale.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.model import fields
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 from trytond.pyson import Eval
 
 
 class Sale(metaclass=PoolMeta):
     __name__ = 'sale.sale'
 
     @classmethod
@@ -16,32 +16,22 @@
             field.states['readonly'] |= (
                 Eval('lines', [0]) & Eval('shipment_address'))
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'sale.line'
 
-    @fields.depends('sale', '_parent_sale.warehouse',
-        '_parent_sale.shipment_address')
+    @fields.depends('sale', 'warehouse', '_parent_sale.shipment_address')
     def _get_tax_rule_pattern(self):
-        pool = Pool()
-        Location = pool.get('stock.location')
-
         pattern = super()._get_tax_rule_pattern()
 
         from_country = from_subdivision = to_country = to_subdivision = None
-        if self.id is None or self.id < 0:
-            warehouse = self.get_warehouse('warehouse')
-            if warehouse:
-                warehouse = Location(warehouse)
-        else:
-            warehouse = self.warehouse
-        if warehouse and warehouse.address:
-            from_country = warehouse.address.country
-            from_subdivision = warehouse.address.subdivision
+        if self.warehouse and self.warehouse.address:
+            from_country = self.warehouse.address.country
+            from_subdivision = self.warehouse.address.subdivision
         if self.sale and self.sale.shipment_address:
             to_country = self.sale.shipment_address.country
             to_subdivision = self.sale.shipment_address.subdivision
 
         pattern['from_country'] = from_country.id if from_country else None
         pattern['from_subdivision'] = (
             from_subdivision.id if from_subdivision else None)
```

### Comparing `trytond_account_tax_rule_country-6.6.0/setup.py` & `trytond_account_tax_rule_country-6.8.0/setup.py`

 * *Files 17% similar despite different names*

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
@@ -34,63 +31,43 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_tax_rule_country'
 
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
 for dep in ['account_invoice', 'sale', 'purchase', 'stock']:
     tests_require.append(get_require_version('trytond_%s' % dep))
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add countries on tax rules',
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
-            'https://hg.tryton.org/modules/account_tax_rule_country'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account tax rule country',
     package_dir={'trytond.modules.account_tax_rule_country': '.'},
     packages=(
         ['trytond.modules.account_tax_rule_country']
         + ['trytond.modules.account_tax_rule_country.%s' % p
             for p in find_packages()]
@@ -127,28 +104,27 @@
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
     account_tax_rule_country = trytond.modules.account_tax_rule_country
     """,
     )
```

### Comparing `trytond_account_tax_rule_country-6.6.0/stock.py` & `trytond_account_tax_rule_country-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/tests/test_module.py` & `trytond_account_tax_rule_country-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/PKG-INFO` & `trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-tax-rule-country
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to add countries on tax rules
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_tax_rule_country
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account tax rule country
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
 
 Account Tax Rule Country
 ########################
 
 The account_tax_rule module extends the tax rule to add origin and destination
```

### Comparing `trytond_account_tax_rule_country-6.6.0/trytond_account_tax_rule_country.egg-info/SOURCES.txt` & `trytond_account_tax_rule_country-6.8.0/trytond_account_tax_rule_country.egg-info/SOURCES.txt`

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
@@ -50,14 +46,15 @@
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/tax_rule_line_form.xml
 ./view/tax_rule_line_template_form.xml
 ./view/tax_rule_line_template_tree.xml
 ./view/tax_rule_line_tree.xml
 ./view/tax_rule_line_tree_sequence.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_form.xml` & `trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_tax_rule_country-6.6.0/view/tax_rule_line_template_form.xml` & `trytond_account_tax_rule_country-6.8.0/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

