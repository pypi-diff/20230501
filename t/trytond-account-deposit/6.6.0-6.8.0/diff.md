# Comparing `tmp/trytond_account_deposit-6.6.0.tar.gz` & `tmp/trytond_account_deposit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_deposit-6.6.0.tar", last modified: Mon Oct 31 16:00:32 2022, max compression
+gzip compressed data, was "trytond_account_deposit-6.8.0.tar", last modified: Mon May  1 11:52:37 2023, max compression
```

## Comparing `trytond_account_deposit-6.6.0.tar` & `trytond_account_deposit-6.8.0.tar`

### file list

```diff
@@ -1,83 +1,81 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:32.137622 trytond_account_deposit-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_deposit-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_deposit-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-31 16:00:30.000000 trytond_account_deposit-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_deposit-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2022-10-31 16:00:29.000000 trytond_account_deposit-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:00:29.000000 trytond_account_deposit-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_deposit-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2022-10-31 16:00:32.137622 trytond_account_deposit-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      625 2021-12-11 16:59:32.000000 trytond_account_deposit-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1727 2022-04-10 15:40:34.000000 trytond_account_deposit-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2495 2019-06-04 16:49:43.000000 trytond_account_deposit-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:32.134289 trytond_account_deposit-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2019-06-04 16:49:43.000000 trytond_account_deposit-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4997 2022-04-10 15:40:34.000000 trytond_account_deposit-6.6.0/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1567 2019-06-04 16:49:43.000000 trytond_account_deposit-6.6.0/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:32.134289 trytond_account_deposit-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1566 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1772 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1472 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1829 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1798 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1609 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1742 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1912 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1472 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1606 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1778 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1484 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1787 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1616 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1760 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1564 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1580 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1536 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1444 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2022-10-29 07:50:39.000000 trytond_account_deposit-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      626 2019-10-11 23:09:47.000000 trytond_account_deposit-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2081 2019-06-04 16:49:43.000000 trytond_account_deposit-6.6.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2020-09-19 09:11:35.000000 trytond_account_deposit-6.6.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1258 2020-09-19 09:11:43.000000 trytond_account_deposit-6.6.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2020-09-19 09:11:49.000000 trytond_account_deposit-6.6.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2020-09-19 09:11:56.000000 trytond_account_deposit-6.6.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2020-09-19 09:12:03.000000 trytond_account_deposit-6.6.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1256 2020-09-19 09:12:09.000000 trytond_account_deposit-6.6.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2020-09-19 09:12:16.000000 trytond_account_deposit-6.6.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2020-09-19 09:12:23.000000 trytond_account_deposit-6.6.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2020-09-19 09:12:29.000000 trytond_account_deposit-6.6.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2020-09-19 09:12:35.000000 trytond_account_deposit-6.6.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5553 2021-12-11 16:59:32.000000 trytond_account_deposit-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      695 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:00:32.137622 trytond_account_deposit-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5260 2022-10-29 07:39:09.000000 trytond_account_deposit-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:32.134289 trytond_account_deposit-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_deposit-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3110 2021-05-16 15:48:21.000000 trytond_account_deposit-6.6.0/tests/scenario_deposit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2022-04-16 16:30:55.000000 trytond_account_deposit-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:52.000000 trytond_account_deposit-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2021-07-12 20:56:36.000000 trytond_account_deposit-6.6.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2022-10-31 15:10:09.000000 trytond_account_deposit-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2022-10-31 16:00:28.000000 trytond_account_deposit-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:32.137622 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2022-10-31 16:00:31.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2371 2022-10-31 16:00:32.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:00:31.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2022-10-31 16:00:31.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:02.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2022-10-31 16:00:31.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:00:31.000000 trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:00:32.134289 trytond_account_deposit-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2019-06-04 16:49:43.000000 trytond_account_deposit-6.6.0/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2019-10-11 23:09:47.000000 trytond_account_deposit-6.6.0/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2019-11-01 22:06:05.000000 trytond_account_deposit-6.6.0/view/move_line_list_deposit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2018-08-18 09:54:04.000000 trytond_account_deposit-6.6.0/view/recall_deposit_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-05-01 11:08:32.000000 trytond_account_deposit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:08:32.000000 trytond_account_deposit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2559 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      625 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1762 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2495 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.290618 trytond_account_deposit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5174 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1567 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.283951 trytond_account_deposit-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1928 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1895 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1700 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1833 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2003 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1563 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1905 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1630 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1896 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1575 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1631 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1707 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1655 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1671 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1627 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1593 2023-04-30 10:46:36.000000 trytond_account_deposit-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      626 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2081 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1258 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1256 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5917 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      695 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4449 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.287284 trytond_account_deposit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2971 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/tests/scenario_deposit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3367 2023-04-21 08:36:08.000000 trytond_account_deposit-6.8.0/tests/scenario_deposit_second_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      648 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_deposit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-05-01 11:08:25.000000 trytond_account_deposit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.293951 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2559 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-05-01 11:52:37.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:52:36.000000 trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:52:37.290618 trytond_account_deposit-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:14.000000 trytond_account_deposit-6.8.0/view/move_line_list_deposit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:20.000000 trytond_account_deposit-6.8.0/view/recall_deposit_form.xml
```

### Comparing `trytond_account_deposit-6.6.0/CHANGELOG` & `trytond_account_deposit-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Support deposit in second currency
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

### Comparing `trytond_account_deposit-6.6.0/COPYRIGHT` & `trytond_account_deposit-6.8.0/COPYRIGHT`

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

### Comparing `trytond_account_deposit-6.6.0/LICENSE` & `trytond_account_deposit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/PKG-INFO` & `trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_deposit
-Version: 6.6.0
+Name: trytond-account-deposit
+Version: 6.8.0
 Summary: Tryton module for accounting deposit
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_deposit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account deposit
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
 
 Account Deposit Module
 ######################
 
 The account_deposit module adds support for deposit accounting.
```

### Comparing `trytond_account_deposit-6.6.0/__init__.py` & `trytond_account_deposit-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/account.py` & `trytond_account_deposit-6.8.0/account.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,11 +42,12 @@
 class AccountType(AccountTypeMixin(), metaclass=PoolMeta):
     __name__ = 'account.account.type'
 
 
 class Reconcile(metaclass=PoolMeta):
     __name__ = 'account.reconcile'
 
-    def get_parties(self, account, _balanced=False, party=None):
+    def get_currencies(self, account, party, currency=None, _balanced=False):
         if account.type.deposit:
             _balanced = True
-        return super().get_parties(account, _balanced=_balanced, party=party)
+        return super().get_parties(
+            account, party, currency=None, _balanced=_balanced)
```

### Comparing `trytond_account_deposit-6.6.0/account.xml` & `trytond_account_deposit-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/invoice.py` & `trytond_account_deposit-6.8.0/invoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,19 +33,17 @@
     @ModelView.button_action('account_deposit.wizard_recall_deposit')
     def recall_deposit(cls, invoices):
         pass
 
     def call_deposit(self, account, description, maximum=None):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
-        Currency = pool.get('currency.currency')
 
-        balance = self.party.get_deposit_balance(account)
-        balance = Currency.compute(
-            account.company.currency, balance, self.currency)
+        balance = self.party.get_deposit_balance(
+            account, currency=self.currency)
         if maximum is None:
             maximum = self.total_amount
         total_amount = min(maximum, self.total_amount, key=abs)
 
         amount = Decimal(0)
         if self.type.startswith('in'):
             if balance > 0 and total_amount > 0:
@@ -127,24 +125,30 @@
             Button('Recall', 'recall', 'tryton-ok', default=True),
             ])
     recall = StateTransition()
 
     def default_start(self, fields):
         return {
             'company': self.record.company.id,
+            'currency': self.record.currency.id,
             }
 
     def transition_recall(self):
         self.record.call_deposit(self.start.account, self.start.description)
         return 'end'
 
 
 class DepositRecallStart(ModelView):
     'Recall deposit on Invoice'
     __name__ = 'account.invoice.recall_deposit.start'
     company = fields.Many2One('company.company', 'Company', readonly=True)
+    currency = fields.Many2One('currency.currency', "Currency", readonly=True)
     account = fields.Many2One('account.account', 'Account', required=True,
         domain=[
             ('type.deposit', '=', True),
             ('company', '=', Eval('company', -1)),
+            ['OR',
+                ('currency', '=', Eval('currency', -1)),
+                ('second_currency', '=', Eval('currency', -1)),
+                ],
             ])
     description = fields.Text('Description', required=True)
```

### Comparing `trytond_account_deposit-6.6.0/invoice.xml` & `trytond_account_deposit-6.8.0/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/locale/bg.po` & `trytond_account_deposit-6.8.0/locale/bg.po`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 msgstr "Фактури"
 
 #, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "Фирма"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 #, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "Описание"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
```

### Comparing `trytond_account_deposit-6.6.0/locale/ca.po` & `trytond_account_deposit-6.8.0/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr "Moneda"
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "Descripció"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr "Bestreta"
```

### Comparing `trytond_account_deposit-6.6.0/locale/cs.po` & `trytond_account_deposit-6.8.0/locale/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr ""
```

### Comparing `trytond_account_deposit-6.6.0/locale/de.po` & `trytond_account_deposit-6.8.0/locale/ro.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Anzahlung"
+msgstr "Depozit"
 
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Anzahlung"
+msgstr "Depozit"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr "Cont"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Unternehmen"
+msgstr "Companie"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr "Valută"
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Beschreibung"
+msgstr "Descriere"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Anzahlung"
+msgstr "Depozit"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr "Anzahlung auf Rechnung verrechnen"
+msgstr "Rechemare depozit pe Factura"
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
-msgstr "Anzahlungspositionen"
+msgstr "Rânduri Depozit"
 
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Anzahlung verrechnen"
+msgstr "Rechemare Depozit"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
-"Auf Konto \"%(account)s\" ist nicht genügend Guthaben von Partei "
-"\"%(party)s\" vorhanden."
+"Contul \"%(notification)s\" nu are destul de mult depozit de la parte "
+"\"%(party)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
-"Partei \"%(party)s\" kann nicht gelöscht werden, solange Sie noch ein "
-"Guthaben bei Unternehmen \"%(company)s\" hat."
+"Nu se poate şterge parte\"%(party)s\" când au depozit la compania "
+"\"%(company)s\"."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Anzahlung verrechnen"
+msgstr "Rechemare Depozit"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Abbrechen"
+msgstr "Anulare"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr "Verrechnen"
+msgstr "Rechemare"
```

### Comparing `trytond_account_deposit-6.6.0/locale/es.po` & `trytond_account_deposit-6.8.0/locale/es.po`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr "Moneda"
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr "Anticipo"
```

### Comparing `trytond_account_deposit-6.6.0/locale/es_419.po` & `trytond_account_deposit-6.8.0/locale/es_419.po`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 msgid "Account"
 msgstr "Cuenta"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "Empresa"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "Descripción"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr "Anticipo"
```

### Comparing `trytond_account_deposit-6.6.0/locale/et.po` & `trytond_account_deposit-6.8.0/locale/sl.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Deposiit"
+msgstr "Depozit"
 
+#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Deposiit"
+msgstr "Depozit"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Ettevõte"
+msgstr "Družba"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Kirjeldus"
+msgstr "Opis"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Deposiit"
+msgstr "Depozit"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr "Tagasta arve deposiit"
+msgstr "Odpoklic depozita za račun"
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
-msgstr "Deposiidi read"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Tagasta deposiit"
+msgstr "Recall Deposit"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
-msgstr "Kontol \"%(account)s\" pole piisavalt osapoole \"%(party)s\" deposiiti."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
-"Ei saa kustutada osapoolt \"%(party)s\" kui neil on ettevõttes "
-"\"%(company)s\" deposiit."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Tühista deposiit."
+msgstr "Recall Deposit"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Tühista"
+msgstr "Prekliči"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr "Tühista"
+msgstr "Odpoklic"
```

### Comparing `trytond_account_deposit-6.6.0/locale/fa.po` & `trytond_account_deposit-6.8.0/locale/fa.po`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 msgid "Account"
 msgstr "حساب"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "شرکت"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "شرح"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr "سپرده"
```

### Comparing `trytond_account_deposit-6.6.0/locale/fi.po` & `trytond_account_deposit-6.8.0/locale/fi.po`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr ""
```

### Comparing `trytond_account_deposit-6.6.0/locale/fr.po` & `trytond_account_deposit-6.8.0/locale/fr.po`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 msgid "Account"
 msgstr "Compte"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "Société"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr "Devise"
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "Description"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr "Dépôt"
```

### Comparing `trytond_account_deposit-6.6.0/locale/hu.po` & `trytond_account_deposit-6.8.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 msgid "Deposit"
 msgstr ""
 
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Számla"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Társaság"
+msgstr ""
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Leírás"
+msgstr "描述"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr ""
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
@@ -54,12 +56,12 @@
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
 msgstr "Recall Deposit"
 
 #, fuzzy
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Mégse"
+msgstr "取消"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
 msgstr ""
```

### Comparing `trytond_account_deposit-6.6.0/locale/id.po` & `trytond_account_deposit-6.8.0/locale/pl.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Setoran"
+msgstr "Wpłata"
 
+#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Setoran"
+msgstr "Wpłata"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Akun"
+msgstr "Konto"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Perusahaan"
+msgstr "Firma"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Deskripsi"
+msgstr "Opis"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Simpanan"
+msgstr "Wpłata"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr ""
+msgstr "Recall Deposit"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
-"Anda tidak dapat menghapus pihak \"%(party)s\" saat mereka memiliki setoran "
-"di perusahaan \"%(company)s\"."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr ""
+msgstr "Recall Deposit"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Batal"
+msgstr "Anuluj"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_deposit-6.6.0/locale/it.po` & `trytond_account_deposit-6.8.0/locale/nl.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Deposito"
+msgstr "Storting"
 
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Deposito"
+msgstr "Storting"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Conto"
+msgstr "Rekening"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Azienda"
+msgstr "Bedrijf"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr "Valuta"
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Descrizione"
+msgstr "Specificatie"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Deposito"
+msgstr "storting"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr "Richiama il deposito sulla fattura"
+msgstr "herinnering ??( Recall deposit on Invoice)"
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
-msgstr "Linee di deposito"
+msgstr "Stortingsregels"
 
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Richiama deposito"
+msgstr "Stort terug"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
-"L'account \"%(account)s\" non ha abbastanza deposito dalla controparte "
+"De rekening \"%(account)s\" heeft niet voldoende krediet van relatie "
 "\"%(party)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
-"Non è possibile cancellare la controparte \"%(party)s\" mentre hanno un "
-"deposito presso la società \"%(company)s\"."
+"U kunt relatie \"%(party)s\" niet wissen terwijl ze een tegoed hebben bij "
+"bedrijf \"%(company)s\"."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Richiama Deposito"
+msgstr "Stort terug"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Annuleren"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr "Richiama"
+msgstr "Terugroepen"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_deposit-6.6.0/locale/lo.po` & `trytond_account_deposit-6.8.0/locale/lo.po`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 msgid "Account"
 msgstr "ບັນຊີ"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr "ບໍລິສັດ"
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr "ເນື້ອໃນລາຍການ"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr "ເງິນມັດຈໍາ"
```

### Comparing `trytond_account_deposit-6.6.0/locale/lt.po` & `trytond_account_deposit-6.8.0/locale/tr.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr ""
+msgstr "Depozit"
 
+#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr ""
+msgstr "Depozit"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr ""
+msgstr "Hesap"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Organizacija"
+msgstr "Şirket"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr ""
+msgstr "Tanım"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr ""
+msgstr "Depozit"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
@@ -50,12 +56,12 @@
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
 msgstr "Recall Deposit"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Vazgeç"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_deposit-6.6.0/locale/nl.po` & `trytond_account_deposit-6.8.0/locale/de.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Storting"
+msgstr "Anzahlung"
 
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Storting"
+msgstr "Anzahlung"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Rekening"
+msgstr "Konto"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Bedrijf"
+msgstr "Unternehmen"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr "Währung"
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Specificatie"
+msgstr "Beschreibung"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "storting"
+msgstr "Anzahlung"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr "herinnering ??( Recall deposit on Invoice)"
+msgstr "Anzahlung auf Rechnung verrechnen"
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
-msgstr "Stortingsregels"
+msgstr "Anzahlungspositionen"
 
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Stort terug"
+msgstr "Anzahlung verrechnen"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
-"De rekening \"%(account)s\" heeft niet voldoende krediet van relatie "
-"\"%(party)s\"."
+"Auf Konto \"%(account)s\" ist nicht genügend Guthaben von Partei "
+"\"%(party)s\" vorhanden."
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
-"U kunt relatie \"%(party)s\" niet wissen terwijl ze een tegoed hebben bij "
-"bedrijf \"%(company)s\"."
+"Partei \"%(party)s\" kann nicht gelöscht werden, solange Sie noch ein "
+"Guthaben bei Unternehmen \"%(company)s\" hat."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Stort terug"
+msgstr "Anzahlung verrechnen"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Annuleren"
+msgstr "Abbrechen"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr "Terugroepen"
+msgstr "Verrechnen"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_deposit-6.6.0/locale/pl.po` & `trytond_account_deposit-6.8.0/locale/ru.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Wpłata"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Wpłata"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr "Счет"
 
+#, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Firma"
+msgstr "Учет.орг."
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
+#, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "Описание"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Wpłata"
+msgstr ""
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
 msgstr "Recall Deposit"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
@@ -51,14 +55,15 @@
 "\"%(company)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
 msgstr "Recall Deposit"
 
+#, fuzzy
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Anuluj"
+msgstr "Отменить"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
 msgstr ""
```

### Comparing `trytond_account_deposit-6.6.0/locale/pt.po` & `trytond_account_deposit-6.8.0/locale/et.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Depósito"
+msgstr "Deposiit"
 
-#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Depósito"
+msgstr "Deposiit"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Conta"
+msgstr "Konto"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Empresa"
+msgstr "Ettevõte"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Descrição"
+msgstr "Kirjeldus"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Depósito"
+msgstr "Deposiit"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr "Recuperar o depósito na fatura"
+msgstr "Tagasta arve deposiit"
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
-msgstr "Linhas de Depósito"
+msgstr "Deposiidi read"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Recall Deposit"
+msgstr "Tagasta deposiit"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
-msgstr ""
+msgstr "Kontol \"%(account)s\" pole piisavalt osapoole \"%(party)s\" deposiiti."
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
+"Ei saa kustutada osapoolt \"%(party)s\" kui neil on ettevõttes "
+"\"%(company)s\" deposiit."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Recall Deposit"
+msgstr "Tühista deposiit."
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Tühista"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr "Recuperar"
+msgstr "Tühista"
```

### Comparing `trytond_account_deposit-6.6.0/locale/ru.po` & `trytond_account_deposit-6.8.0/locale/hu.po`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Счет"
+msgstr "Számla"
 
 #, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Учет.орг."
+msgstr "Társaság"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Описание"
+msgstr "Leírás"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr ""
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
@@ -54,12 +58,12 @@
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
 msgstr "Recall Deposit"
 
 #, fuzzy
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Mégse"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
 msgstr ""
```

### Comparing `trytond_account_deposit-6.6.0/locale/sl.po` & `trytond_account_deposit-6.8.0/locale/id.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Depozit"
+msgstr "Setoran"
 
-#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Depozit"
+msgstr "Setoran"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Konto"
+msgstr "Akun"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Družba"
+msgstr "Perusahaan"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Opis"
+msgstr "Deskripsi"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Depozit"
+msgstr "Simpanan"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr "Odpoklic depozita za račun"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Recall Deposit"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
+"Anda tidak dapat menghapus pihak \"%(party)s\" saat mereka memiliki setoran "
+"di perusahaan \"%(company)s\"."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Recall Deposit"
+msgstr ""
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Batal"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr "Odpoklic"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_deposit-6.6.0/locale/tr.po` & `trytond_account_deposit-6.8.0/locale/lt.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#, fuzzy
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr "Depozit"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr "Depozit"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr "Hesap"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
-msgstr "Şirket"
+msgstr "Organizacija"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "Tanım"
+msgstr ""
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr "Depozit"
+msgstr ""
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
@@ -52,12 +54,12 @@
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
 msgstr "Recall Deposit"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "Vazgeç"
+msgstr ""
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_deposit-6.6.0/locale/uk.po` & `trytond_account_deposit-6.8.0/locale/uk.po`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
 msgstr ""
 
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
+msgstr ""
+
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
 msgstr ""
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
 msgstr ""
```

### Comparing `trytond_account_deposit-6.6.0/locale/zh_CN.po` & `trytond_account_deposit-6.8.0/locale/it.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.account.type,deposit:"
 msgid "Deposit"
-msgstr ""
+msgstr "Deposito"
 
 msgctxt "field:account.account.type.template,deposit:"
 msgid "Deposit"
-msgstr ""
+msgstr "Deposito"
 
 msgctxt "field:account.invoice.recall_deposit.start,account:"
 msgid "Account"
-msgstr ""
+msgstr "Conto"
 
 msgctxt "field:account.invoice.recall_deposit.start,company:"
 msgid "Company"
+msgstr "Azienda"
+
+msgctxt "field:account.invoice.recall_deposit.start,currency:"
+msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.recall_deposit.start,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descrizione"
 
 msgctxt "field:party.party,deposit:"
 msgid "Deposit"
-msgstr ""
+msgstr "Deposito"
 
 msgctxt "model:account.invoice.recall_deposit.start,name:"
 msgid "Recall deposit on Invoice"
-msgstr ""
+msgstr "Richiama il deposito sulla fattura"
 
 msgctxt "model:ir.action,name:act_move_line_deposit"
 msgid "Deposit Lines"
-msgstr ""
+msgstr "Linee di deposito"
 
 msgctxt "model:ir.action,name:wizard_recall_deposit"
 msgid "Recall Deposit"
-msgstr "Recall Deposit"
+msgstr "Richiama deposito"
 
 msgctxt "model:ir.message,text:msg_deposit_not_enough"
 msgid "The account \"%(account)s\" has not enough deposit from party \"%(party)s\"."
 msgstr ""
+"L'account \"%(account)s\" non ha abbastanza deposito dalla controparte "
+"\"%(party)s\"."
 
 msgctxt "model:ir.message,text:msg_erase_party_deposit"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have deposit at company "
 "\"%(company)s\"."
 msgstr ""
+"Non è possibile cancellare la controparte \"%(party)s\" mentre hanno un "
+"deposito presso la società \"%(company)s\"."
 
 msgctxt "model:ir.model.button,string:invoice_recall_deposit_button"
 msgid "Recall Deposit"
-msgstr "Recall Deposit"
+msgstr "Richiama Deposito"
 
-#, fuzzy
 msgctxt "wizard_button:account.invoice.recall_deposit,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Annulla"
 
 msgctxt "wizard_button:account.invoice.recall_deposit,start,recall:"
 msgid "Recall"
-msgstr ""
+msgstr "Richiama"
```

### Comparing `trytond_account_deposit-6.6.0/message.xml` & `trytond_account_deposit-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart.xml` & `trytond_account_deposit-6.8.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_bg.xml` & `trytond_account_deposit-6.8.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_ca.xml` & `trytond_account_deposit-6.8.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_de.xml` & `trytond_account_deposit-6.8.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_en.xml` & `trytond_account_deposit-6.8.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_es.xml` & `trytond_account_deposit-6.8.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_fr.xml` & `trytond_account_deposit-6.8.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_nl.xml` & `trytond_account_deposit-6.8.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_pt.xml` & `trytond_account_deposit-6.8.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_ru.xml` & `trytond_account_deposit-6.8.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/minimal_chart_sl.xml` & `trytond_account_deposit-6.8.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/party.py` & `trytond_account_deposit-6.8.0/party.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from decimal import Decimal
 
 from sql import For, Literal, Null
 from sql.aggregate import Sum
-from sql.conditionals import Coalesce
+from sql.conditionals import Case, Coalesce
 
 from trytond.i18n import gettext
 from trytond.model import fields
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.party.exceptions import EraseError
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import grouped_slice, reduce_ids
@@ -96,48 +96,59 @@
                 & line_clause,
                 group_by=line.party,
                 having=Operator(
                     Sum(Coalesce(line.debit, 0) - Coalesce(line.credit, 0)),
                     Decimal(clause[2] or 0))))
         return [('id', 'in', query)]
 
-    def get_deposit_balance(self, deposit_account):
+    def get_deposit_balance(self, deposit_account, currency=None):
         'Return the deposit account balance (debit - credit) for the party'
         pool = Pool()
         MoveLine = pool.get('account.move.line')
         transaction = Transaction()
         cursor = transaction.connection.cursor()
 
         line = MoveLine.__table__()
+        if currency is None:
+            currency = deposit_account.currency
         assert deposit_account.type.deposit
 
         where = ((line.account == deposit_account.id)
             & (line.party == self.id)
             & (line.reconciliation == Null))
         if transaction.database.has_select_for():
             cursor.execute(*line.select(
                     Literal(1),
                     where=where,
                     for_=For('UPDATE', nowait=True)))
         else:
             MoveLine.lock()
-        cursor.execute(*line.select(
-                Sum(Coalesce(line.debit, 0) - Coalesce(line.credit, 0)),
-                where=where))
+
+        if currency == deposit_account.currency:
+            amount = Sum(Coalesce(line.debit, 0) - Coalesce(line.credit, 0))
+        else:
+            amount = Sum(Case(
+                    (line.second_currency == currency.id,
+                        line.amount_second_currency),
+                    else_=0))
+
+        cursor.execute(*line.select(amount, where=where))
         amount, = cursor.fetchone()
-        if amount and not isinstance(amount, Decimal):
-            currency = deposit_account.company.currency
-            amount = currency.round(Decimal(str(amount)))
-        return amount or Decimal(0)
+        if amount is None:
+            amount = Decimal(0)
+        if not isinstance(amount, Decimal):
+            amount = Decimal(str(amount))
+        return currency.round(amount)
 
     def check_deposit(self, deposit_account, sign=1):
         '''Check if the deposit account balance (debit - credit) has the same
         sign for the party'''
         assert sign in (1, -1)
-        amount = self.get_deposit_balance(deposit_account)
+        amount = self.get_deposit_balance(
+            deposit_account, currency=deposit_account.second_currency)
         return not amount or ((amount < 0) == (sign < 0))
 
 
 class Erase(metaclass=PoolMeta):
     __name__ = 'party.erase'
 
     def check_erase_company(self, party, company):
```

### Comparing `trytond_account_deposit-6.6.0/party.xml` & `trytond_account_deposit-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_deposit-6.6.0/setup.py` & `trytond_account_deposit-6.8.0/setup.py`

 * *Files 12% similar despite different names*

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
 name = 'trytond_account_deposit'
 
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
 
 requires = ['python-dateutil', 'python-sql >= 0.4']
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
     description='Tryton module for accounting deposit',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_deposit',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account deposit',
     package_dir={'trytond.modules.account_deposit': '.'},
     packages=(
         ['trytond.modules.account_deposit']
         + ['trytond.modules.account_deposit.%s' % p for p in find_packages()]
         ),
@@ -124,28 +102,27 @@
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
     account_deposit = trytond.modules.account_deposit
     """,
     )
```

### Comparing `trytond_account_deposit-6.6.0/tests/scenario_deposit.rst` & `trytond_account_deposit-6.8.0/tests/scenario_deposit.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 ================
 Deposit Scenario
 ================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
     ...     create_chart, get_accounts
     >>> from trytond.modules.account_invoice.tests.tools import \
     ...     set_fiscalyear_invoice_sequences, create_payment_term
     >>> from trytond.modules.account_deposit.tests.tools import \
     ...     add_deposit_accounts
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_deposit')
 
 Create company::
 
@@ -79,15 +76,15 @@
     >>> line.unit_price = Decimal(500)
     >>> invoice.save()
     >>> invoice.untaxed_amount
     Decimal('500.00')
 
 Recall deposit::
 
-    >>> recall_deposit = Wizard('account.invoice.recall_deposit', [invoice])
+    >>> recall_deposit = invoice.click('recall_deposit')
     >>> recall_deposit.form.account = accounts['deposit']
     >>> recall_deposit.form.description = 'Recall Deposit'
     >>> recall_deposit.execute('recall')
     >>> invoice.reload()
     >>> deposit_line, = [l for l in invoice.lines
     ...     if l.account == accounts['deposit']]
     >>> deposit_line.amount
```

### Comparing `trytond_account_deposit-6.6.0/tests/tools.py` & `trytond_account_deposit-6.8.0/tests/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from proteus import Model
-
 from trytond.modules.company.tests.tools import get_company
 
 
 def add_deposit_accounts(accounts, company=None, config=None):
     'Add deposit to accounts'
     Account = Model.get('account.account', config=config)
```

### Comparing `trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/PKG-INFO` & `trytond_account_deposit-6.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-deposit
-Version: 6.6.0
+Name: trytond_account_deposit
+Version: 6.8.0
 Summary: Tryton module for accounting deposit
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_deposit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account deposit
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
 
 Account Deposit Module
 ######################
 
 The account_deposit module adds support for deposit accounting.
```

### Comparing `trytond_account_deposit-6.6.0/trytond_account_deposit.egg-info/SOURCES.txt` & `trytond_account_deposit-6.8.0/trytond_account_deposit.egg-info/SOURCES.txt`

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
 account.py
@@ -72,23 +68,25 @@
 ./locale/ru.po
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_deposit.rst
+./tests/scenario_deposit_second_currency.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./tests/tools.py
 ./view/account_type_form.xml
 ./view/invoice_form.xml
 ./view/move_line_list_deposit.xml
 ./view/party_form.xml
 ./view/party_tree.xml
 ./view/recall_deposit_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -108,14 +106,15 @@
 locale/ru.po
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_deposit.rst
+tests/scenario_deposit_second_currency.rst
 tests/test_module.py
 tests/test_scenario.py
 tests/tools.py
 trytond_account_deposit.egg-info/PKG-INFO
 trytond_account_deposit.egg-info/SOURCES.txt
 trytond_account_deposit.egg-info/dependency_links.txt
 trytond_account_deposit.egg-info/entry_points.txt
```

