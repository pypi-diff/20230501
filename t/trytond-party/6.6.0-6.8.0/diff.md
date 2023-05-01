# Comparing `tmp/trytond_party-6.6.0.tar.gz` & `tmp/trytond_party-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party-6.6.0.tar", last modified: Mon Oct 31 15:47:59 2022, max compression
+gzip compressed data, was "trytond_party-6.8.0.tar", last modified: Mon May  1 11:35:48 2023, max compression
```

## Comparing `trytond_party-6.6.0.tar` & `trytond_party-6.8.0.tar`

### file list

```diff
@@ -1,106 +1,103 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.356677 trytond_party-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_party-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_party-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 15:47:58.000000 trytond_party-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_party-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     5539 2022-10-31 15:47:57.000000 trytond_party-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      884 2022-10-31 15:47:56.000000 trytond_party-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:33.000000 trytond_party-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_party-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2619 2022-10-31 15:47:59.356677 trytond_party-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-10-27 11:24:44.000000 trytond_party-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1062 2022-10-11 19:49:58.000000 trytond_party-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16613 2022-10-11 19:49:58.000000 trytond_party-6.6.0/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25257 2022-04-08 16:24:27.000000 trytond_party-6.6.0/address.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1449 2022-10-11 19:49:58.000000 trytond_party-6.6.0/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3658 2021-02-27 17:17:01.000000 trytond_party-6.6.0/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4580 2022-04-11 21:24:34.000000 trytond_party-6.6.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2497 2022-04-08 16:25:27.000000 trytond_party-6.6.0/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12269 2022-10-19 08:14:45.000000 trytond_party-6.6.0/contact_mechanism.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2021-02-27 17:17:01.000000 trytond_party-6.6.0/contact_mechanism.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2022-10-11 19:49:58.000000 trytond_party-6.6.0/country.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.353343 trytond_party-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2020-12-16 10:18:43.000000 trytond_party-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6349 2022-05-31 08:05:14.000000 trytond_party-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2022-10-27 11:24:44.000000 trytond_party-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_party-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4129 2022-04-08 16:27:20.000000 trytond_party-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2019-06-04 16:49:44.000000 trytond_party-6.6.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.353343 trytond_party-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:35.000000 trytond_party-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2019-06-04 16:49:44.000000 trytond_party-6.6.0/icons/tryton-party.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     3841 2022-05-31 07:30:55.000000 trytond_party-6.6.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2020-09-17 15:18:13.000000 trytond_party-6.6.0/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    31778 2019-06-04 16:49:44.000000 trytond_party-6.6.0/label.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.350010 trytond_party-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    32197 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38457 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30842 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40098 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38857 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30645 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36222 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35713 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30627 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38379 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33249 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31368 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33657 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35025 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36909 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38166 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37167 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33648 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37614 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32710 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33435 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30627 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    45561 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37408 2022-10-29 07:50:32.000000 trytond_party-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2873 2021-10-30 15:16:00.000000 trytond_party-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    37405 2022-10-22 23:10:32.000000 trytond_party-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8099 2022-04-08 16:27:20.000000 trytond_party-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:47:59.356677 trytond_party-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5398 2022-10-29 07:39:11.000000 trytond_party-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.350010 trytond_party-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2022-04-16 16:30:56.000000 trytond_party-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1638 2020-07-09 09:37:07.000000 trytond_party-6.6.0/tests/scenario_party_erase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2020-07-09 09:37:07.000000 trytond_party-6.6.0/tests/scenario_party_phone_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2021-10-30 15:16:00.000000 trytond_party-6.6.0/tests/scenario_party_replace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    16012 2022-04-16 16:30:56.000000 trytond_party-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_party-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2022-10-31 15:10:09.000000 trytond_party-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2022-10-31 15:47:55.000000 trytond_party-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.356677 trytond_party-6.6.0/trytond_party.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2619 2022-10-31 15:47:58.000000 trytond_party-6.6.0/trytond_party.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3411 2022-10-31 15:47:59.000000 trytond_party-6.6.0/trytond_party.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:47:58.000000 trytond_party-6.6.0/trytond_party.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2022-10-31 15:47:58.000000 trytond_party-6.6.0/trytond_party.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:48.000000 trytond_party-6.6.0/trytond_party.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      176 2022-10-31 15:47:58.000000 trytond_party-6.6.0/trytond_party.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:47:58.000000 trytond_party-6.6.0/trytond_party.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:47:59.353343 trytond_party-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1556 2022-10-11 19:45:04.000000 trytond_party-6.6.0/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      999 2022-09-12 22:47:25.000000 trytond_party-6.6.0/view/address_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2019-10-11 23:09:48.000000 trytond_party-6.6.0/view/address_format_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2019-10-11 23:09:48.000000 trytond_party-6.6.0/view/address_format_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2019-10-11 23:09:48.000000 trytond_party-6.6.0/view/address_subdivision_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2019-10-11 23:09:48.000000 trytond_party-6.6.0/view/address_subdivision_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2022-04-08 16:23:26.000000 trytond_party-6.6.0/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2022-04-08 16:23:26.000000 trytond_party-6.6.0/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2019-02-13 10:09:33.000000 trytond_party-6.6.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2019-06-04 16:49:44.000000 trytond_party-6.6.0/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2022-04-08 16:23:26.000000 trytond_party-6.6.0/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2019-02-13 10:09:33.000000 trytond_party-6.6.0/view/check_vies_result.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2021-03-24 12:36:12.000000 trytond_party-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2021-04-27 07:34:40.000000 trytond_party-6.6.0/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2022-10-11 19:45:04.000000 trytond_party-6.6.0/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2022-10-11 19:45:04.000000 trytond_party-6.6.0/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2020-09-17 15:18:13.000000 trytond_party-6.6.0/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2019-06-04 16:49:44.000000 trytond_party-6.6.0/view/erase_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2022-04-08 16:24:27.000000 trytond_party-6.6.0/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-04-08 16:24:27.000000 trytond_party-6.6.0/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2022-04-08 16:24:27.000000 trytond_party-6.6.0/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2022-04-08 16:24:27.000000 trytond_party-6.6.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2022-10-24 15:39:58.000000 trytond_party-6.6.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      190 2019-02-13 10:09:33.000000 trytond_party-6.6.0/view/replace_ask_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.048093 trytond_party-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5736 2023-05-01 10:57:18.000000 trytond_party-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2023-05-01 10:57:18.000000 trytond_party-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-01 11:35:48.048093 trytond_party-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1062 2023-04-15 07:12:15.000000 trytond_party-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16613 2023-04-15 07:12:15.000000 trytond_party-6.8.0/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25257 2023-04-15 07:12:15.000000 trytond_party-6.8.0/address.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1449 2023-04-15 07:12:15.000000 trytond_party-6.8.0/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3658 2023-04-15 07:12:15.000000 trytond_party-6.8.0/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4573 2023-04-15 07:12:15.000000 trytond_party-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2497 2023-04-15 07:12:15.000000 trytond_party-6.8.0/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12269 2023-04-29 22:04:03.000000 trytond_party-6.8.0/contact_mechanism.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-04-15 07:12:15.000000 trytond_party-6.8.0/contact_mechanism.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_party-6.8.0/country.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.044760 trytond_party-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-29 22:04:03.000000 trytond_party-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.044760 trytond_party-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_party-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:20.000000 trytond_party-6.8.0/icons/tryton-party.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-04-15 07:12:15.000000 trytond_party-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-15 07:12:15.000000 trytond_party-6.8.0/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    31778 2023-01-16 14:00:20.000000 trytond_party-6.8.0/label.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.038093 trytond_party-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    32339 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38662 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30984 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40303 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39063 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30787 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36147 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35855 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30769 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38585 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33391 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31510 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33799 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35167 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37051 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38370 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37264 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33790 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37727 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32852 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33577 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30769 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    45703 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37550 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2023-04-29 22:04:03.000000 trytond_party-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    37925 2023-04-21 08:36:08.000000 trytond_party-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8099 2023-04-15 07:12:15.000000 trytond_party-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:48.048093 trytond_party-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4597 2023-04-15 07:12:15.000000 trytond_party-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.041427 trytond_party-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1638 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_erase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_identifier_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_phone_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_replace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    16012 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 10:57:12.000000 trytond_party-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.048093 trytond_party-6.8.0/trytond_party.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3475 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-14 15:56:20.000000 trytond_party-6.8.0/trytond_party.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      176 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.044760 trytond_party-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1556 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      999 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_format_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_format_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_subdivision_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_subdivision_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/check_vies_result.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/erase_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/replace_ask_form.xml
```

### Comparing `trytond_party-6.6.0/CHANGELOG` & `trytond_party-6.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Notify for duplicate identifier
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Manage dereferenced name in tax identifier clause of party
 * Add optional address to contact mechanism
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_party-6.6.0/COPYRIGHT` & `trytond_party-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2013 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 Copyright (C) 2008-2022 Udo Spallek.
 Copyright (C) 2008-2011 Korbinian Preisler.
 Copyright (C) 2008-2011 virtual things.
 Copyright (C) 2004-2008 Tiny SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
```

### Comparing `trytond_party-6.6.0/LICENSE` & `trytond_party-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/PKG-INFO` & `trytond_party-6.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_party
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-party/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/party
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party
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
 Provides-Extra: test
 Provides-Extra: VIES
 Provides-Extra: phonenumbers
 License-File: LICENSE
 
 ############
 Party Module
```

### Comparing `trytond_party-6.6.0/__init__.py` & `trytond_party-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/address.py` & `trytond_party-6.8.0/address.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/address.xml` & `trytond_party-6.8.0/address.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/category.py` & `trytond_party-6.8.0/category.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/category.xml` & `trytond_party-6.8.0/category.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/configuration.py` & `trytond_party-6.8.0/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     'Party Configuration Sequence'
     __name__ = 'party.configuration.party_sequence'
     party_sequence = party_sequence
     _configuration_value_field = 'party_sequence'
 
     @classmethod
     def check_xml_record(cls, records, values):
-        return True
+        pass
 
 
 class ConfigurationLang(_ConfigurationValue, ModelSQL, ValueMixin):
     'Party Configuration Lang'
     __name__ = 'party.configuration.party_lang'
     party_lang = party_lang
     _configuration_value_field = 'party_lang'
```

### Comparing `trytond_party-6.6.0/configuration.xml` & `trytond_party-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/contact_mechanism.py` & `trytond_party-6.8.0/contact_mechanism.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/contact_mechanism.xml` & `trytond_party-6.8.0/contact_mechanism.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/country.py` & `trytond_party-6.8.0/country.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/doc/conf.py` & `trytond_party-6.8.0/doc/conf.py`

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

### Comparing `trytond_party-6.6.0/doc/design.rst` & `trytond_party-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/doc/usage.rst` & `trytond_party-6.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/exceptions.py` & `trytond_party-6.8.0/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/icons/LICENSE` & `trytond_party-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/ir.py` & `trytond_party-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/label.fodt` & `trytond_party-6.8.0/label.fodt`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/locale/bg.po` & `trytond_party-6.8.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -551,14 +551,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 #, fuzzy
```

### Comparing `trytond_party-6.6.0/locale/ca.po` & `trytond_party-6.8.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -541,14 +541,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "El número de telèfon \"%(phone)s\" del tercer \"%(party)s\" no és vàlid."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "El codi del tercer ha de ser únic."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr "El tercer \"%(party)\" té el mateix \"%(type)s\" \"%(code)s\"."
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Per canviar el \"%(field)s\" del tercer \"%(party)s\", heu d'editar els seus"
 " mètodes de contacte."
@@ -951,15 +955,15 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Income Tax Identifier"
 msgstr "Identificador fiscal Indi"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indonesian VAT Number"
-msgstr "Identificador fiscal Estonià"
+msgstr "Identificador fiscal Indonesi"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish Personal Number"
 msgstr "Número personal Irlandès"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish VAT Number"
```

### Comparing `trytond_party-6.6.0/locale/cs.po` & `trytond_party-6.8.0/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
```

### Comparing `trytond_party-6.6.0/locale/de.po` & `trytond_party-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 msgctxt "field:party.address,party:"
 msgid "Party"
 msgstr "Partei"
 
 msgctxt "field:party.address,party_name:"
 msgid "Party Name"
-msgstr "Parteiname"
+msgstr "Zustellzusatz"
 
 msgctxt "field:party.address,postal_code:"
 msgid "Postal Code"
 msgstr "Postleitzahl"
 
 msgctxt "field:party.address,street:"
 msgid "Street"
@@ -548,14 +548,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "Die Telefonnummer \"%(phone)s\" von Partei \"%(party)s\" ist nicht gültig."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Der Code für eine Partei kann nur einmal vergeben werden."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr "Die Partei \"%(party)s\" hat dieselbe %(type)s \"%(code)s\"."
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Das Feld \"%(field)s\" für die Partei \"%(party)s\" muss bei den "
 "Kontaktinformationen geändert werden."
```

### Comparing `trytond_party-6.6.0/locale/es.po` & `trytond_party-6.8.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -542,14 +542,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "El número de teléfono \"%(phone)s\" del tercero \"%(party)s\" no es válido."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "El código del tercero debe ser único."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr "El tercero \"%(party)s\" tiene el mismo %(type)s \"%(code)s\"."
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Para cambiar el \"%(field)s\" del tercer \"%(party)s\", debe editar sus "
 "metodos de contacto."
@@ -952,15 +956,15 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indian Income Tax Identifier"
 msgstr "Identificador fiscal Indio"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Indonesian VAT Number"
-msgstr "Identificador fiscal Estonio"
+msgstr "Identificador fiscal Indonesio"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish Personal Number"
 msgstr "Número personal Irlandés"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Irish VAT Number"
```

### Comparing `trytond_party-6.6.0/locale/es_419.po` & `trytond_party-6.8.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -527,14 +527,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
```

### Comparing `trytond_party-6.6.0/locale/et.po` & `trytond_party-6.8.0/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:ir.email.template,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
 msgctxt "field:party.address,city:"
 msgid "City"
 msgstr "Linn"
 
-#, fuzzy
 msgctxt "field:party.address,contact_mechanisms:"
 msgid "Contact Mechanisms"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
 msgctxt "field:party.address,country:"
 msgid "Country"
 msgstr "Riik"
 
 msgctxt "field:party.address,full_address:"
 msgid "Full Address"
@@ -31,66 +29,60 @@
 
 msgctxt "field:party.address,name:"
 msgid "Building Name"
 msgstr "Hoone"
 
 msgctxt "field:party.address,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.address,party_name:"
 msgid "Party Name"
-msgstr "Osapoole nimi"
+msgstr "Partneri nimi"
 
-#, fuzzy
 msgctxt "field:party.address,postal_code:"
 msgid "Postal Code"
-msgstr "Riik"
+msgstr "Sihtnumber"
 
 msgctxt "field:party.address,street:"
 msgid "Street"
 msgstr "Tänav"
 
-#, fuzzy
 msgctxt "field:party.address,street_single_line:"
 msgid "Street"
 msgstr "Tänav"
 
 msgctxt "field:party.address,subdivision:"
 msgid "Subdivision"
 msgstr "Alajaotus"
 
 #, fuzzy
 msgctxt "field:party.address,subdivision_types:"
 msgid "Subdivision Types"
-msgstr "Alajaotus"
+msgstr "Maakond"
 
-#, fuzzy
 msgctxt "field:party.address.format,country_code:"
 msgid "Country Code"
-msgstr "Riik"
+msgstr "Riigi kood"
 
 msgctxt "field:party.address.format,format_:"
 msgid "Format"
 msgstr "Formaat"
 
-#, fuzzy
 msgctxt "field:party.address.format,language_code:"
 msgid "Language Code"
-msgstr "Keel"
+msgstr "Keele kood"
 
-#, fuzzy
 msgctxt "field:party.address.subdivision_type,country_code:"
 msgid "Country Code"
-msgstr "Riik"
+msgstr "Riigi kood"
 
-#, fuzzy
 msgctxt "field:party.address.subdivision_type,types:"
 msgid "Subdivision Types"
-msgstr "Alajaotus"
+msgstr "Maakond"
 
 msgctxt "field:party.category,childs:"
 msgid "Children"
 msgstr "Alamjaotus"
 
 msgctxt "field:party.category,name:"
 msgid "Name"
@@ -111,62 +103,59 @@
 #, fuzzy
 msgctxt "field:party.configuration,identifier_types:"
 msgid "Identifier Types"
 msgstr "Identifikaatorid"
 
 msgctxt "field:party.configuration,party_lang:"
 msgid "Party Language"
-msgstr "Osapoole keel"
+msgstr "Partneri keel"
 
 msgctxt "field:party.configuration,party_sequence:"
 msgid "Party Sequence"
-msgstr "Osapoole jada"
+msgstr "Partneri jada"
 
 msgctxt "field:party.configuration.party_lang,party_lang:"
 msgid "Party Language"
-msgstr "Osapoole keel"
+msgstr "Partneri keel"
 
 msgctxt "field:party.configuration.party_sequence,party_sequence:"
 msgid "Party Sequence"
-msgstr "Osapoole jada"
+msgstr "Partneri jada"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism,address:"
 msgid "Address"
-msgstr "Aadressid"
+msgstr "Aadress"
 
 msgctxt "field:party.contact_mechanism,comment:"
 msgid "Comment"
 msgstr "Kommentaar"
 
 msgctxt "field:party.contact_mechanism,email:"
 msgid "E-Mail"
 msgstr "E-Kiri"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism,language:"
 msgid "Language"
 msgstr "Keel"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism,languages:"
 msgid "Languages"
 msgstr "Keeled"
 
 msgctxt "field:party.contact_mechanism,name:"
 msgid "Name"
 msgstr "Nimi"
 
 msgctxt "field:party.contact_mechanism,other_value:"
 msgid "Value"
 msgstr "Väärtus"
 
 msgctxt "field:party.contact_mechanism,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.contact_mechanism,sip:"
 msgid "SIP"
 msgstr "SIP"
 
 msgctxt "field:party.contact_mechanism,skype:"
 msgid "Skype"
@@ -188,49 +177,45 @@
 msgid "Value Compact"
 msgstr ""
 
 msgctxt "field:party.contact_mechanism,website:"
 msgid "Website"
 msgstr "Koduleht"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism.language,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism.language,language:"
 msgid "Language"
 msgstr "Keel"
 
 msgctxt "field:party.erase.ask,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
-#, fuzzy
 msgctxt "field:party.identifier,address:"
 msgid "Address"
-msgstr "Aadressid"
+msgstr "Aadress"
 
 msgctxt "field:party.identifier,code:"
 msgid "Code"
 msgstr "Kood"
 
 msgctxt "field:party.identifier,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.identifier,type:"
 msgid "Type"
 msgstr "Tüüp"
 
-#, fuzzy
 msgctxt "field:party.identifier,type_address:"
 msgid "Type of Address"
-msgstr "Aadressid"
+msgstr "Aadressi tüüp"
 
 msgctxt "field:party.party,addresses:"
 msgid "Addresses"
 msgstr "Aadressid"
 
 msgctxt "field:party.party,categories:"
 msgid "Categories"
@@ -242,19 +227,19 @@
 
 msgctxt "field:party.party,code_readonly:"
 msgid "Code Readonly"
 msgstr ""
 
 msgctxt "field:party.party,contact_mechanisms:"
 msgid "Contact Mechanisms"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
 msgctxt "field:party.party,distance:"
 msgid "Distance"
-msgstr ""
+msgstr "Kaugus"
 
 msgctxt "field:party.party,email:"
 msgid "E-Mail"
 msgstr "E-Kiri"
 
 msgctxt "field:party.party,fax:"
 msgid "Fax"
@@ -302,23 +287,23 @@
 
 msgctxt "field:party.party-party.category,category:"
 msgid "Category"
 msgstr "Kategooria"
 
 msgctxt "field:party.party-party.category,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.party.lang,lang:"
 msgid "Language"
 msgstr "Keel"
 
 msgctxt "field:party.party.lang,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.replace.ask,destination:"
 msgid "Destination"
 msgstr "Sihtkoht"
 
 msgctxt "field:party.replace.ask,source:"
 msgid "Source"
@@ -367,79 +352,77 @@
 
 msgctxt "help:party.configuration,party_lang:"
 msgid "The default language for new parties."
 msgstr "Uute osapoolte vaikimisi keel"
 
 msgctxt "help:party.configuration,party_sequence:"
 msgid "Used to generate the party code."
-msgstr "Kasutatakse osapoole koodi loomiseks"
+msgstr "Kasutatakse partneri koodi loomiseks"
 
 msgctxt "help:party.configuration.party_lang,party_lang:"
 msgid "The default language for new parties."
 msgstr "Vaikimisi keel uutele osapooltele."
 
 msgctxt "help:party.configuration.party_sequence,party_sequence:"
 msgid "Used to generate the party code."
-msgstr "Kasutatakse osapoole koodi loomiseks"
+msgstr "Kasutatakse partneri koodi loomiseks"
 
-#, fuzzy
 msgctxt "help:party.contact_mechanism,language:"
 msgid ""
 "Used to translate communication made using the contact mechanism.\n"
 "Leave empty for the party language."
-msgstr "Kasutatakse osapoolega suhtluse tõlkimisel"
+msgstr "Kasutatakse partneriga suhtluse tõlkimisel"
 
 msgctxt "help:party.erase.ask,party:"
 msgid "The party to be erased."
-msgstr "Kustutatav osapool."
+msgstr "Kustutatav partner."
 
-#, fuzzy
 msgctxt "help:party.identifier,address:"
 msgid "The address identified by this record."
-msgstr "Kirje poolt identifitseeritud osapool"
+msgstr "Kirje poolt identifitseeritud aadress."
 
 msgctxt "help:party.identifier,party:"
 msgid "The party identified by this record."
-msgstr "Kirje poolt identifitseeritud osapool"
+msgstr "Kirje põhjal identifitseeritud partner"
 
 msgctxt "help:party.party,categories:"
 msgid "The categories the party belongs to."
-msgstr "Kategooriad kuhu osapool kuulub"
+msgstr "Kategooriad kuhu partner kuulub"
 
 msgctxt "help:party.party,code:"
 msgid "The unique identifier of the party."
-msgstr "Osapoole unikaalne tunnus"
+msgstr "Partneri unikaalne tunnus"
 
 msgctxt "help:party.party,identifiers:"
 msgid "Add other identifiers of the party."
-msgstr "Lisa osapoolele muid tunnuseid"
+msgstr "Lisa partnerile muid tunnuseid"
 
 msgctxt "help:party.party,lang:"
 msgid "Used to translate communications with the party."
-msgstr "Kasutatakse osapoolega suhtluse tõlkimisel"
+msgstr "Kasutatakse partneriga suhtluse tõlkimisel"
 
 msgctxt "help:party.party,name:"
 msgid "The main identifier of the party."
-msgstr "Osapoole peamine tunnus"
+msgstr "Partneri identifikaator"
 
 msgctxt "help:party.party,replaced_by:"
 msgid "The party replacing this one."
-msgstr "Osapoolt asendav osapool"
+msgstr "Asendav partner"
 
 msgctxt "help:party.party,tax_identifier:"
 msgid "The identifier used for tax report."
 msgstr "Maksuaruandes kasutatav tunnus"
 
 msgctxt "help:party.replace.ask,destination:"
 msgid "The party that replaces."
-msgstr "Osapool, kes asendab"
+msgstr "Partner, kes asendab"
 
 msgctxt "help:party.replace.ask,source:"
 msgid "The party to be replaced."
-msgstr "Osapool, keda asendatakse"
+msgstr "Partner, keda asendatakse"
 
 msgctxt "model:ir.action,name:act_address_form"
 msgid "Addresses"
 msgstr "Aadressid"
 
 msgctxt "model:ir.action,name:act_address_format_form"
 msgid "Address Formats"
@@ -456,28 +439,27 @@
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
 msgstr "Kategooriad"
 
 msgctxt "model:ir.action,name:act_contact_mechanism_form"
 msgid "Contact Mechanisms"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
 msgctxt "model:ir.action,name:act_party_by_category"
 msgid "Parties by Category"
 msgstr "Kategooriatepõhised osapooled"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_party_configuration_form"
 msgid "Configuration"
 msgstr "Seadistus"
 
 msgctxt "model:ir.action,name:act_party_form"
 msgid "Parties"
-msgstr "Osapooled"
+msgstr "Partnerid"
 
 msgctxt "model:ir.action,name:report_label"
 msgid "Labels"
 msgstr "Etiketid"
 
 msgctxt "model:ir.action,name:wizard_check_vies"
 msgid "Check VIES"
@@ -491,18 +473,17 @@
 msgid "Replace"
 msgstr "Asenda"
 
 msgctxt "model:ir.message,text:msg_address_change_party"
 msgid "You cannot change the party of address \"%(address)s\"."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_address_subdivision_country_code_unique"
 msgid "The country code on subdivision type must be unique."
-msgstr "Osapoole kood peab olema unikaalne."
+msgstr "Riigi kood peab olema unikaalne."
 
 msgctxt "model:ir.message,text:msg_category_name_unique"
 msgid "The name of party category must be unique by parent."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_contact_mechanism_change_party"
 msgid "You cannot change the party of contact mechanism \"%(contact)s\"."
@@ -538,33 +519,37 @@
 
 msgctxt "model:ir.message,text:msg_invalid_phone_number"
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
-msgstr "Osapoole kood peab olema unikaalne."
+msgstr "Partneri kood peab olema unikaalne."
+
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
 msgid "The VIES service is unavailable, try again later."
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_party"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_party"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "model:ir.ui.menu,name:menu_address_form"
 msgid "Addresses"
 msgstr "Aadressid"
 
 msgctxt "model:ir.ui.menu,name:menu_address_format_form"
 msgid "Address Formats"
@@ -585,29 +570,28 @@
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Seadistus"
 
 msgctxt "model:ir.ui.menu,name:menu_contact_mechanism_form"
 msgid "Contact Mechanisms"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_party"
 msgid "Parties"
-msgstr "Osapooled"
+msgstr "Partnerid"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_party_configuration"
 msgid "Configuration"
 msgstr "Seadistus"
 
 msgctxt "model:ir.ui.menu,name:menu_party_form"
 msgid "Parties"
-msgstr "Osapooled"
+msgstr "Partnerid"
 
 msgctxt "model:party.address,name:"
 msgid "Address"
 msgstr "Aadressid"
 
 msgctxt "model:party.address.format,name:"
 msgid "Address Format"
@@ -625,60 +609,59 @@
 #, fuzzy
 msgctxt "model:party.check_vies.result,name:"
 msgid "Check VIES"
 msgstr "Kontrolli VIES"
 
 msgctxt "model:party.configuration,name:"
 msgid "Party Configuration"
-msgstr "Osapoole seadistus"
+msgstr "Partneri seadistus"
 
 msgctxt "model:party.configuration.party_lang,name:"
 msgid "Party Configuration Lang"
-msgstr "Osapoole seadistuse keel"
+msgstr "Partneri seadistuse keel"
 
 msgctxt "model:party.configuration.party_sequence,name:"
 msgid "Party Configuration Sequence"
-msgstr "Osapoole seadistuse järjestus"
+msgstr "Partneri seadistuse järjestus"
 
 msgctxt "model:party.contact_mechanism,name:"
 msgid "Contact Mechanism"
-msgstr "Kontakteerumisviis"
+msgstr "Kontaktid"
 
-#, fuzzy
 msgctxt "model:party.contact_mechanism.language,name:"
 msgid "Contact Mechanism Language"
-msgstr "Kontakteerumisviis"
+msgstr "Kontakti keel"
 
 msgctxt "model:party.erase.ask,name:"
 msgid "Erase Party"
-msgstr "Kustuta osapool"
+msgstr "Kustuta partner"
 
 msgctxt "model:party.identifier,name:"
 msgid "Party Identifier"
-msgstr "Osapoole tunnus"
+msgstr "Partneri identifikaator"
 
 msgctxt "model:party.party,name:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "model:party.party-party.category,name:"
 msgid "Party - Category"
-msgstr "Osapool - Kategooria"
+msgstr "Partner - Kategooria"
 
 msgctxt "model:party.party.lang,name:"
 msgid "Party Lang"
-msgstr ""
+msgstr "Partneri keel"
 
 msgctxt "model:party.replace.ask,name:"
 msgid "Replace Party"
-msgstr "Asenda osapool"
+msgstr "Asenda partner"
 
 msgctxt "model:res.group,name:group_party_admin"
 msgid "Party Administration"
-msgstr "Osapoole administreerimine"
+msgstr "Partneri administreerimine"
 
 #, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Albanian VAT Number"
 msgstr "Albaania KMKR"
 
 #, fuzzy
@@ -1405,15 +1388,15 @@
 
 msgctxt "view:party.party:"
 msgid "General"
 msgstr "Üldine"
 
 msgctxt "view:party.replace.ask:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "view:party.replace.ask:"
 msgid "Replace By"
 msgstr "Asendatud"
 
 msgctxt "wizard_button:party.check_vies,result,end:"
 msgid "OK"
```

### Comparing `trytond_party-6.6.0/locale/fa.po` & `trytond_party-6.8.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -554,14 +554,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "شماره تلفن \"%s\" نهاد/سازمان \"%s\" معتبر نیست."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "کد نهاد/سازمان باید منحصربفرد یاشد."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr "کد پیش شماره تلفن \"%s\" نهاد/سازمان \"%s\" معتبر نیست."
```

### Comparing `trytond_party-6.6.0/locale/fi.po` & `trytond_party-6.8.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -533,14 +533,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
```

### Comparing `trytond_party-6.6.0/locale/fr.po` & `trytond_party-6.8.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -543,14 +543,18 @@
 "Le numéro de téléphone « %(phone)s » du tiers « %(party)s » n'est pas "
 "valide."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Le code du tiers doit être unique."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr "Le tiers « %(party)s » a le même %(type)s « %(code)s »."
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Pour modifier le « %(field)s » pour le tiers «%(party)s », vous devez "
 "modifier ces moyens de contact."
```

### Comparing `trytond_party-6.6.0/locale/hu.po` & `trytond_party-6.8.0/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -548,14 +548,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Egy partner kódja csak egyszer adható ki"
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 #, fuzzy
```

### Comparing `trytond_party-6.6.0/locale/id.po` & `trytond_party-6.8.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -536,14 +536,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
```

### Comparing `trytond_party-6.6.0/locale/it.po` & `trytond_party-6.8.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -568,14 +568,18 @@
 "Il numero telefonico \"%(phone)s\" della controparte \"%(party)s\" non è "
 "valido."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Il codice della controparte deve essere univoco."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Il numero di partita IVA \"%(code)s\" della controparte \"%(party)s\" non è "
```

### Comparing `trytond_party-6.6.0/locale/lo.po` & `trytond_party-6.8.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -572,14 +572,18 @@
 msgstr "ເລກໂທລະສັບ \"%(phone)s\" ຂອງພາກສ່ວນ \"%(party)s\" ບໍ່ຖືກຕ້ອງ ."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "ລະຫັດຂອງພາກສ່ວນຕ້ອງບໍ່ຊໍ້າກັນ"
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr "ເລກໂທລະສັບ \"%(phone)s\" ຂອງພາກສ່ວນ \"%(party)s\" ບໍ່ຖືກຕ້ອງ ."
```

### Comparing `trytond_party-6.6.0/locale/lt.po` & `trytond_party-6.8.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -535,14 +535,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
```

### Comparing `trytond_party-6.6.0/locale/nl.po` & `trytond_party-6.8.0/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -543,14 +543,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "Het telefoonnummer \"%(phone)s\" voor relatie \"%(party)s\" is niet geldig."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "De code voor relatie moet uniek zijn."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr "De relatie \"%(party)s\" heeft dezelfde %(type)s \"%(code)s\"."
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Om \"%(field)s\" voor relatie \"%(party)s\" te wijzigen, moet de contact "
 "mogelijkheid bewerkt worden."
```

### Comparing `trytond_party-6.6.0/locale/pl.po` & `trytond_party-6.8.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,26 @@
 msgid "Contact Mechanism"
 msgstr "Sposób kontaktu"
 
 msgctxt "field:party.address,city:"
 msgid "City"
 msgstr "Miejscowość"
 
-#, fuzzy
 msgctxt "field:party.address,contact_mechanisms:"
 msgid "Contact Mechanisms"
 msgstr "Sposoby kontaktu"
 
 msgctxt "field:party.address,country:"
 msgid "Country"
 msgstr "Kraj"
 
 msgctxt "field:party.address,full_address:"
 msgid "Full Address"
 msgstr "Pełny adres"
 
-#, fuzzy
 msgctxt "field:party.address,identifiers:"
 msgid "Identifiers"
 msgstr "Identyfikatory"
 
 msgctxt "field:party.address,name:"
 msgid "Building Name"
 msgstr "Nazwa budynku"
@@ -44,15 +42,14 @@
 msgid "Postal Code"
 msgstr "Kod pocztowy"
 
 msgctxt "field:party.address,street:"
 msgid "Street"
 msgstr "Ulica"
 
-#, fuzzy
 msgctxt "field:party.address,street_single_line:"
 msgid "Street"
 msgstr "Ulica"
 
 msgctxt "field:party.address,subdivision:"
 msgid "Subdivision"
 msgstr "Region"
@@ -117,15 +114,14 @@
 msgid "Party Language"
 msgstr "Język strony"
 
 msgctxt "field:party.configuration.party_sequence,party_sequence:"
 msgid "Party Sequence"
 msgstr "Numeracja strony"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism,address:"
 msgid "Address"
 msgstr "Adres"
 
 msgctxt "field:party.contact_mechanism,comment:"
 msgid "Comment"
 msgstr "Komentarz"
@@ -190,15 +186,14 @@
 msgid "Language"
 msgstr "Język"
 
 msgctxt "field:party.erase.ask,party:"
 msgid "Party"
 msgstr "Strona"
 
-#, fuzzy
 msgctxt "field:party.identifier,address:"
 msgid "Address"
 msgstr "Adres"
 
 msgctxt "field:party.identifier,code:"
 msgid "Code"
 msgstr "Kod"
@@ -207,18 +202,17 @@
 msgid "Party"
 msgstr "Strona"
 
 msgctxt "field:party.identifier,type:"
 msgid "Type"
 msgstr "Typ"
 
-#, fuzzy
 msgctxt "field:party.identifier,type_address:"
 msgid "Type of Address"
-msgstr "Adres"
+msgstr "Typ adresu"
 
 msgctxt "field:party.party,addresses:"
 msgid "Addresses"
 msgstr "Adresy"
 
 msgctxt "field:party.party,categories:"
 msgid "Categories"
@@ -391,15 +385,14 @@
 "Służy do tłumaczenia komunikacji realizowanej za pomocą sposobu kontaktu.\n"
 "Pozostaw puste, aby użyć języka strony."
 
 msgctxt "help:party.erase.ask,party:"
 msgid "The party to be erased."
 msgstr "Strona przeznaczona do usunięcia."
 
-#, fuzzy
 msgctxt "help:party.identifier,address:"
 msgid "The address identified by this record."
 msgstr "Strona identyfikowana przez ten rekord."
 
 msgctxt "help:party.identifier,party:"
 msgid "The party identified by this record."
 msgstr "Strona identyfikowana przez ten rekord."
@@ -548,20 +541,25 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "Numer telefonu \"%(phone)s\" strony \"%(party)s\" jest niewłaściwy."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Kod strony musi być unikatowy."
 
-#, fuzzy
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
-msgstr "Typ %(type)s \"%(code)s\" strony \"%(party)s\" jest niepoprawny."
+msgstr ""
+"Aby zmienić pole \"%(field)s\" strony \"%(party)s\" należy zmodyfikować "
+"sposoby kontaktu."
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
 msgid "The VIES service is unavailable, try again later."
 msgstr "Usługa VIES jest niedostępna. Spróbuj później."
 
 msgctxt "model:ir.sequence,name:sequence_party"
 msgid "Party"
@@ -595,15 +593,14 @@
 msgid "Configuration"
 msgstr "Konfiguracja"
 
 msgctxt "model:ir.ui.menu,name:menu_contact_mechanism_form"
 msgid "Contact Mechanisms"
 msgstr "Sposoby kontaktu"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_party"
 msgid "Parties"
 msgstr "Strony"
 
 msgctxt "model:ir.ui.menu,name:menu_party_configuration"
 msgid "Configuration"
 msgstr "Konfiguracja"
@@ -634,15 +631,15 @@
 
 msgctxt "model:party.configuration,name:"
 msgid "Party Configuration"
 msgstr "Ustawienia strony"
 
 msgctxt "model:party.configuration.party_lang,name:"
 msgid "Party Configuration Lang"
-msgstr "Język konfiguracji strony"
+msgstr "Język ustawień strony"
 
 msgctxt "model:party.configuration.party_sequence,name:"
 msgid "Party Configuration Sequence"
 msgstr "Ustawienia numeracji strony"
 
 msgctxt "model:party.contact_mechanism,name:"
 msgid "Contact Mechanism"
@@ -686,15 +683,15 @@
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Andorra Tax Number"
 msgstr "Numer podatkowy w Andorze"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Argentinian National Identity Number"
-msgstr "Argentyński numer identyfikacji narodowej"
+msgstr "Argentyński krajowy numer identyfikacyjny"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Argentinian Tax Number"
 msgstr "Argentyński numer podatkowy"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Australian Business Number"
```

### Comparing `trytond_party-6.6.0/locale/pt.po` & `trytond_party-6.8.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -556,14 +556,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "O número de telefone \"%(phone)s\" da pessoa \"%(party)s\" é inválido."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "O código da pessoa deve ser único."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr "O número de IVA \"%(code)s\" da pessoa \"%(party)s\" é inválido."
```

### Comparing `trytond_party-6.6.0/locale/ro.po` & `trytond_party-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 msgid "Contact Mechanism"
 msgstr "Mecanism de contact"
 
 msgctxt "field:party.address,city:"
 msgid "City"
 msgstr "Oraș"
 
-#, fuzzy
 msgctxt "field:party.address,contact_mechanisms:"
 msgid "Contact Mechanisms"
-msgstr "Mecanisme de contact"
+msgstr "Date de Contact"
 
 msgctxt "field:party.address,country:"
 msgid "Country"
 msgstr "Țară"
 
 msgctxt "field:party.address,full_address:"
 msgid "Full Address"
 msgstr "Adresa completa"
 
-#, fuzzy
 msgctxt "field:party.address,identifiers:"
 msgid "Identifiers"
-msgstr "Identificatorii"
+msgstr "Identificatori"
 
 msgctxt "field:party.address,name:"
 msgid "Building Name"
 msgstr "Numele Cladirii"
 
 msgctxt "field:party.address,party:"
 msgid "Party"
@@ -116,15 +114,14 @@
 msgid "Party Language"
 msgstr "Limba Părții"
 
 msgctxt "field:party.configuration.party_sequence,party_sequence:"
 msgid "Party Sequence"
 msgstr "Secvență Părții"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism,address:"
 msgid "Address"
 msgstr "Adresa"
 
 msgctxt "field:party.contact_mechanism,comment:"
 msgid "Comment"
 msgstr "Cometariu"
@@ -189,15 +186,14 @@
 msgid "Language"
 msgstr "Limba"
 
 msgctxt "field:party.erase.ask,party:"
 msgid "Party"
 msgstr "Parte"
 
-#, fuzzy
 msgctxt "field:party.identifier,address:"
 msgid "Address"
 msgstr "Adresa"
 
 msgctxt "field:party.identifier,code:"
 msgid "Code"
 msgstr "Cod"
@@ -206,18 +202,17 @@
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:party.identifier,type:"
 msgid "Type"
 msgstr "Tip"
 
-#, fuzzy
 msgctxt "field:party.identifier,type_address:"
 msgid "Type of Address"
-msgstr "Adresa"
+msgstr "Tip de Adresa"
 
 msgctxt "field:party.party,addresses:"
 msgid "Addresses"
 msgstr "Adrese"
 
 msgctxt "field:party.party,categories:"
 msgid "Categories"
@@ -229,15 +224,15 @@
 
 msgctxt "field:party.party,code_readonly:"
 msgid "Code Readonly"
 msgstr "Cod numai pentru citit"
 
 msgctxt "field:party.party,contact_mechanisms:"
 msgid "Contact Mechanisms"
-msgstr "Mecanisme de contact"
+msgstr "Date de Contact"
 
 msgctxt "field:party.party,distance:"
 msgid "Distance"
 msgstr "Distanţă"
 
 msgctxt "field:party.party,email:"
 msgid "E-Mail"
@@ -392,18 +387,17 @@
 "Folosit pentru a traduce comunicarea făcută utilizând mecanismul de contact.\n"
 "Lăsați gol pentru limba părţii."
 
 msgctxt "help:party.erase.ask,party:"
 msgid "The party to be erased."
 msgstr "Partea care urmează să fie ștearsă."
 
-#, fuzzy
 msgctxt "help:party.identifier,address:"
 msgid "The address identified by this record."
-msgstr "Partea identificată prin această înregistrare."
+msgstr "Adresa identificată prin această înregistrare."
 
 msgctxt "help:party.identifier,party:"
 msgid "The party identified by this record."
 msgstr "Partea identificată prin această înregistrare."
 
 msgctxt "help:party.party,categories:"
 msgid "The categories the party belongs to."
@@ -459,19 +453,19 @@
 
 msgctxt "model:ir.action,name:act_category_tree"
 msgid "Categories"
 msgstr "Categorii"
 
 msgctxt "model:ir.action,name:act_contact_mechanism_form"
 msgid "Contact Mechanisms"
-msgstr "Mecanisme de contact"
+msgstr "Date de Contact"
 
 msgctxt "model:ir.action,name:act_party_by_category"
 msgid "Parties by Category"
-msgstr "Părți pe categorii"
+msgstr "Părți pe Categorii"
 
 msgctxt "model:ir.action,name:act_party_configuration_form"
 msgid "Configuration"
 msgstr "Configurare"
 
 msgctxt "model:ir.action,name:act_party_form"
 msgid "Parties"
@@ -545,14 +539,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "Numărul de telefon \"%(phone)s\" al parti \"%(party)s\" nu este valid."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Codul parții trebuie să fie unic."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr "Partea \"%(party)s\" are acelaş %(type)s \"%(code)s\"."
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Pentru a schimba \"%(field)s\" pentru parte \"%(party)s\" trebuie editate "
 "mecanismele lor de contact."
@@ -591,17 +589,16 @@
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Configurare"
 
 msgctxt "model:ir.ui.menu,name:menu_contact_mechanism_form"
 msgid "Contact Mechanisms"
-msgstr "Mecanisme de contact"
+msgstr "Date de Contact"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_party"
 msgid "Parties"
 msgstr "Părți"
 
 msgctxt "model:ir.ui.menu,name:menu_party_configuration"
 msgid "Configuration"
 msgstr "Configurare"
@@ -886,23 +883,21 @@
 msgid "Finnish Personal Identity Code"
 msgstr "Finlanda, Cod numeric Personal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "Finnish VAT Number"
 msgstr "Finlanda, Număr TVA"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Company Establishment Identification Number"
-msgstr "Franţa, Cod Numeric Personal"
+msgstr "Franţa, Cod Identificare Companie"
 
-#, fuzzy
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Company Identification Number"
-msgstr "Franţa, Cod Fiscal"
+msgstr "Franţa, Cod Identificare Companie"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Personal Identification Number"
 msgstr "Franţa, Cod Numeric Personal"
 
 msgctxt "selection:party.configuration,identifier_types:"
 msgid "French Tax Identification Number"
@@ -1264,15 +1259,14 @@
 msgid "Skype"
 msgstr "Skype"
 
 msgctxt "selection:party.contact_mechanism,type:"
 msgid "Website"
 msgstr "Site web"
 
-#, fuzzy
 msgctxt "view:party.address:"
 msgid "General"
 msgstr "General"
 
 msgctxt "view:party.party:"
 msgid "General"
 msgstr "General"
```

### Comparing `trytond_party-6.6.0/locale/ru.po` & `trytond_party-6.8.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -555,14 +555,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Код контрагента должен быть уникальным"
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 #, fuzzy
```

### Comparing `trytond_party-6.6.0/locale/sl.po` & `trytond_party-6.8.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -573,14 +573,18 @@
 msgstr "Telefonska številka \"%(phone)s\" partnerja \"%(party)s\" je neveljavna."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Šifra partnerja mora biti edinstvena."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr "Telefonska številka \"%(phone)s\" partnerja \"%(party)s\" je neveljavna."
```

### Comparing `trytond_party-6.6.0/locale/tr.po` & `trytond_party-6.8.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -533,14 +533,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr ""
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_vies_unavailable"
```

### Comparing `trytond_party-6.6.0/locale/uk.po` & `trytond_party-6.8.0/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -541,14 +541,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "Номер телефону \"%(phone)s\" для особи \"%(party)s\" не є коректним."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "Код особи має бути унікальним."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr ""
 "Щоб змінити \"%(field)s\" для особи \"%(party)s\", вам слід змінити її "
 "контактні механізми."
```

### Comparing `trytond_party-6.6.0/locale/zh_CN.po` & `trytond_party-6.8.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,18 @@
 msgid "The phone number \"%(phone)s\" for party \"%(party)s\" is not valid."
 msgstr "参与者 \"%(party)s\" 的电话号码 \"%(phone)s\" 设置无效."
 
 msgctxt "model:ir.message,text:msg_party_code_unique"
 msgid "The code on party must be unique."
 msgstr "参与者代码不能重复."
 
+msgctxt "model:ir.message,text:msg_party_identifier_duplicate"
+msgid "The party \"%(party)s\" has the same %(type)s \"%(code)s\"."
+msgstr ""
+
 #, fuzzy
 msgctxt "model:ir.message,text:msg_party_set_contact_mechanism"
 msgid ""
 "To change the \"%(field)s\" for party \"%(party)s\", you must edit their "
 "contact mechanisms."
 msgstr "参与者 \"%(party)s\" 的 %(type)s \"%(code)s\" 设置无效."
```

### Comparing `trytond_party-6.6.0/message.xml` & `trytond_party-6.8.0/message.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_party-6.6.0/message.xml` & `trytond_party-6.8.0/message.xml`

```diff
@@ -14,14 +14,17 @@
     </record>
     <record model="ir.message" id="msg_invalid_phone_number">
       <field name="text">The phone number &quot;%(phone)s&quot; for party &quot;%(party)s&quot; is not valid.</field>
     </record>
     <record model="ir.message" id="msg_invalid_code">
       <field name="text">The %(type)s &quot;%(code)s&quot; for party &quot;%(party)s&quot; is not valid.</field>
     </record>
+    <record model="ir.message" id="msg_party_identifier_duplicate">
+      <field name="text">The party &quot;%(party)s&quot; has the same %(type)s &quot;%(code)s&quot;.</field>
+    </record>
     <record model="ir.message" id="msg_vies_unavailable">
       <field name="text">The VIES service is unavailable, try again later.</field>
     </record>
     <record model="ir.message" id="msg_different_name">
       <field name="text">Parties have different names: &quot;%(source_name)s&quot; vs &quot;%(destination_name)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_different_tax_identifier">
```

### Comparing `trytond_party-6.6.0/party.py` & `trytond_party-6.8.0/party.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from sql.functions import CharLength
 from stdnum import get_cc_module
 
 from trytond import backend
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, MultiValueMixin, Unique,
-    ValueMixin, fields, sequence_ordered)
+    ValueMixin, convert_from, fields, sequence_ordered)
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval
 from trytond.tools import is_full_text, lstrip_wildcard
 from trytond.tools.multivalue import migrate_property
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 from trytond.wizard import Button, StateTransition, StateView, Wizard
 
 from .contact_mechanism import _PHONE_TYPES, _ContactMechanismMixin
 from .exceptions import (
     EraseError, InvalidIdentifierCode, SimilarityWarning, VIESUnavailable)
 
 
@@ -706,14 +706,38 @@
                         party = ''
                     raise InvalidIdentifierCode(
                         gettext('party.msg_invalid_code',
                             type=self.type_string,
                             code=self.code,
                             party=party))
 
+    @fields.depends(methods=['_notify_duplicate'])
+    def on_change_notify(self):
+        notifications = super().on_change_notify()
+        notifications.extend(self._notify_duplicate())
+        return notifications
+
+    @fields.depends('code', methods=['on_change_with_code'])
+    def _notify_duplicate(self):
+        cls = self.__class__
+        if self.code:
+            code = self.on_change_with_code()
+            others = cls.search([
+                    ('id', '!=', self.id),
+                    ('type', '!=', None),
+                    ('code', '=', code),
+                    ], limit=1)
+            if others:
+                other, = others
+                yield ('warning', gettext(
+                        'party.msg_party_identifier_duplicate',
+                        party=other.party.rec_name,
+                        type=other.type_string,
+                        code=other.code))
+
 
 class CheckVIESResult(ModelView):
     'Check VIES'
     __name__ = 'party.check_vies.result'
     parties_succeed = fields.Many2Many('party.party', None, None,
         'Parties Succeed', readonly=True, states={
             'invisible': ~Eval('parties_succeed'),
@@ -909,29 +933,17 @@
     erase = StateTransition()
 
     def transition_erase(self):
         pool = Pool()
         Party = pool.get('party.party')
         cursor = Transaction().connection.cursor()
 
-        def convert_from(table, tables):
-            right, condition = tables[None]
-            if table:
-                table = table.join(right, condition=condition)
-            else:
-                table = right
-            for k, sub_tables in tables.items():
-                if k is None:
-                    continue
-                table = convert_from(table, sub_tables)
-            return table
-
         resources = self.get_resources()
         parties = replacing = [self.ask.party]
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             while replacing:
                 replacing = Party.search([
                         ('replaced_by', 'in', list(map(int, replacing))),
                         ])
                 parties += replacing
         for party in parties:
             self.check_erase(party)
@@ -940,15 +952,15 @@
                 assert issubclass(Model, ModelSQL)
                 assert len(columns) == len(values)
                 if 'active' in Model._fields:
                     records = Model.search(domain)
                     Model.write(records, {'active': False})
 
                 tables, where = Model.search_domain(domain, active_test=False)
-                from_ = convert_from(None, tables)
+                from_ = convert_from(None, tables, type_='INNER')
                 table, _ = tables[None]
                 query = from_.select(table.id, where=where)
 
                 if columns:
                     model_tables = [Model.__table__()]
                     if Model._history:
                         model_tables.append(Model.__table_history__())
```

### Comparing `trytond_party-6.6.0/party.xml` & `trytond_party-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/setup.py` & `trytond_party-6.8.0/setup.py`

 * *Files 14% similar despite different names*

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
@@ -37,60 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_party'
 
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
 
 requires = ['python-sql >= 0.4', 'python-stdnum >= 1.15']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus'), 'phonenumbers']
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module with parties and addresses',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-party/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/party',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton party',
     package_dir={'trytond.modules.party': '.'},
     packages=(
         ['trytond.modules.party']
         + ['trytond.modules.party.%s' % p for p in find_packages()]
         ),
@@ -128,29 +106,28 @@
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
         'VIES': ['python-stdnum[SOAP]'],
         'phonenumbers': ['phonenumbers'],
         },
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     party = trytond.modules.party
     """,
     )
```

### Comparing `trytond_party-6.6.0/tests/scenario_party_erase.rst` & `trytond_party-6.8.0/tests/scenario_party_erase.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/tests/scenario_party_phone_number.rst` & `trytond_party-6.8.0/tests/scenario_party_phone_number.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/tests/scenario_party_replace.rst` & `trytond_party-6.8.0/tests/scenario_party_replace.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/tests/test_module.py` & `trytond_party-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/trytond_party.egg-info/PKG-INFO` & `trytond_party-6.8.0/trytond_party.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-party
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-party/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/party
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton party
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
 Provides-Extra: test
 Provides-Extra: VIES
 Provides-Extra: phonenumbers
 License-File: LICENSE
 
 ############
 Party Module
```

### Comparing `trytond_party-6.6.0/trytond_party.egg-info/SOURCES.txt` & `trytond_party-6.8.0/trytond_party.egg-info/SOURCES.txt`

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
 address.py
@@ -68,14 +64,15 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_party_erase.rst
+./tests/scenario_party_identifier_notifications.rst
 ./tests/scenario_party_phone_number.rst
 ./tests/scenario_party_replace.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/address_form.xml
 ./view/address_form_simple.xml
 ./view/address_format_form.xml
@@ -129,14 +126,15 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_party_erase.rst
+tests/scenario_party_identifier_notifications.rst
 tests/scenario_party_phone_number.rst
 tests/scenario_party_replace.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_party.egg-info/PKG-INFO
 trytond_party.egg-info/SOURCES.txt
 trytond_party.egg-info/dependency_links.txt
```

### Comparing `trytond_party-6.6.0/view/address_form.xml` & `trytond_party-6.8.0/view/address_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/view/address_form_simple.xml` & `trytond_party-6.8.0/view/address_form_simple.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/view/address_tree_sequence.xml` & `trytond_party-6.8.0/view/address_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/view/contact_mechanism_form.xml` & `trytond_party-6.8.0/view/contact_mechanism_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/view/contact_mechanism_tree_sequence.xml` & `trytond_party-6.8.0/view/contact_mechanism_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.6.0/view/identifier_form.xml` & `trytond_party-6.8.0/view/identifier_form.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_party-6.6.0/view/identifier_form.xml` & `trytond_party-6.8.0/view/identifier_form.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form>
+<form cursor="type">
   <label name="party"/>
   <field name="party"/>
   <group colspan="2" col="-1" id="checkboxes">
     <label name="active"/>
     <field name="active"/>
     <label name="sequence"/>
     <field name="sequence"/>
```

### Comparing `trytond_party-6.6.0/view/party_form.xml` & `trytond_party-6.8.0/view/party_form.xml`

 * *Files identical despite different names*

