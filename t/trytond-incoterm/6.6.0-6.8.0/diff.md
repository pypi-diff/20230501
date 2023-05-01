# Comparing `tmp/trytond_incoterm-6.6.0.tar.gz` & `tmp/trytond_incoterm-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_incoterm-6.6.0.tar", last modified: Mon Oct 31 16:31:28 2022, max compression
+gzip compressed data, was "trytond_incoterm-6.8.0.tar", last modified: Mon May  1 11:37:47 2023, max compression
```

## Comparing `trytond_incoterm-6.6.0.tar` & `trytond_incoterm-6.8.0.tar`

### file list

```diff
@@ -1,95 +1,91 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:31:28.181791 trytond_incoterm-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2199 2022-04-25 16:35:01.000000 trytond_incoterm-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2022-10-31 16:31:26.000000 trytond_incoterm-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_incoterm-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2022-10-31 16:31:26.000000 trytond_incoterm-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:31:25.000000 trytond_incoterm-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_incoterm-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2465 2022-10-31 16:31:28.178458 trytond_incoterm-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2022-10-27 11:24:44.000000 trytond_incoterm-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1735 2021-12-11 16:59:33.000000 trytond_incoterm-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1636 2021-12-11 16:59:33.000000 trytond_incoterm-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      721 2022-10-11 19:49:57.000000 trytond_incoterm-6.6.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6272 2022-07-11 20:07:22.000000 trytond_incoterm-6.6.0/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:31:28.178458 trytond_incoterm-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1847 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2022-05-31 08:02:55.000000 trytond_incoterm-6.6.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2022-10-27 11:24:44.000000 trytond_incoterm-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-27 11:24:44.000000 trytond_incoterm-6.6.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3169 2022-10-11 19:49:57.000000 trytond_incoterm-6.6.0/incoterm.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11274 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/incoterm.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:31:28.171791 trytond_incoterm-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5670 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5744 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5717 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5743 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4575 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4510 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5607 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:33.000000 trytond_incoterm-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1055 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3971 2022-10-11 19:49:57.000000 trytond_incoterm-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1866 2021-04-27 07:34:40.000000 trytond_incoterm-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2326 2022-10-15 18:57:03.000000 trytond_incoterm-6.6.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3716 2022-04-10 15:43:38.000000 trytond_incoterm-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:31:28.181791 trytond_incoterm-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5839 2022-10-29 07:39:10.000000 trytond_incoterm-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1499 2022-04-10 15:43:38.000000 trytond_incoterm-6.6.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1404 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:31:28.171791 trytond_incoterm-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_incoterm-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6212 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/tests/scenario_incoterm.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      628 2022-04-16 16:30:56.000000 trytond_incoterm-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_incoterm-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2022-10-31 15:10:09.000000 trytond_incoterm-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2022-10-31 16:31:24.000000 trytond_incoterm-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:31:28.178458 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2465 2022-10-31 16:31:27.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2782 2022-10-31 16:31:28.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:31:27.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2022-10-31 16:31:27.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-03-28 13:53:44.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2022-10-31 16:31:27.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:31:27.000000 trytond_incoterm-6.6.0/trytond_incoterm.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:31:28.175125 trytond_incoterm-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2022-10-11 19:49:57.000000 trytond_incoterm-6.6.0/view/carrier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-04-08 16:23:26.000000 trytond_incoterm-6.6.0/view/incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/party_form_purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/party_form_sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/party_incoterm_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/party_incoterm_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      467 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/purchase_request_quotation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/sale_opportunity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/stock_shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/stock_shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/stock_shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2021-04-03 16:26:39.000000 trytond_incoterm-6.6.0/view/stock_shipment_out_return_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:47.936248 trytond_incoterm-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      624 2023-05-01 10:58:39.000000 trytond_incoterm-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 10:58:38.000000 trytond_incoterm-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2464 2023-05-01 11:37:47.936248 trytond_incoterm-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1735 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1636 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      721 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6269 2023-04-21 08:36:08.000000 trytond_incoterm-6.8.0/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:47.929581 trytond_incoterm-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3169 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/incoterm.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11274 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/incoterm.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:47.919581 trytond_incoterm-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5670 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5744 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5717 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5743 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4575 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4510 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5607 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:39.000000 trytond_incoterm-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1055 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3971 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1866 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2326 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3716 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:37:47.936248 trytond_incoterm-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5026 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1499 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1404 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:47.922914 trytond_incoterm-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/tests/scenario_incoterm.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      628 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-05-01 10:58:33.000000 trytond_incoterm-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:47.932914 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2464 2023-05-01 11:37:47.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2744 2023-05-01 11:37:47.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:37:47.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-01 11:37:47.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-05-01 11:37:47.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:37:47.000000 trytond_incoterm-6.8.0/trytond_incoterm.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:37:47.929581 trytond_incoterm-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/carrier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/party_form_purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/party_form_sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/party_incoterm_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/party_incoterm_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/purchase_request_quotation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/sale_opportunity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/stock_shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/stock_shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/stock_shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_incoterm-6.8.0/view/stock_shipment_out_return_form.xml
```

### Comparing `trytond_incoterm-6.6.0/COPYRIGHT` & `trytond_incoterm-6.8.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020-2022 Cédric Krier
+Copyright (C) 2020-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_incoterm-6.6.0/LICENSE` & `trytond_incoterm-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/PKG-INFO` & `trytond_incoterm-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_incoterm
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for incoterms
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-incoterm/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/incoterm
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton incoterm
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
 
 ###############
 Incoterm Module
 ###############
```

### Comparing `trytond_incoterm-6.6.0/__init__.py` & `trytond_incoterm-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/account.py` & `trytond_incoterm-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/carrier.xml` & `trytond_incoterm-6.8.0/carrier.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/common.py` & `trytond_incoterm-6.8.0/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         pattern = self._get_incoterm_pattern()
         incoterms = Incoterm.get_incoterms(self.company, pattern)
         if self.party:
             party_incoterms = {r.incoterm for r in self._party_incoterms}
         else:
             party_incoterms = set()
         return [
-            i.id for i in incoterms
+            i for i in incoterms
             if not party_incoterms or i in party_incoterms]
 
     @fields.depends()
     def _get_incoterm_pattern(self):
         return {}
 
     @fields.depends('incoterm')
```

### Comparing `trytond_incoterm-6.6.0/doc/conf.py` & `trytond_incoterm-6.8.0/doc/conf.py`

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

### Comparing `trytond_incoterm-6.6.0/incoterm.py` & `trytond_incoterm-6.8.0/incoterm.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/incoterm.xml` & `trytond_incoterm-6.8.0/incoterm.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/bg.po` & `trytond_incoterm-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/ca.po` & `trytond_incoterm-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/cs.po` & `trytond_incoterm-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/de.po` & `trytond_incoterm-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/es.po` & `trytond_incoterm-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/es_419.po` & `trytond_incoterm-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/et.po` & `trytond_incoterm-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/fa.po` & `trytond_incoterm-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/fi.po` & `trytond_incoterm-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/fr.po` & `trytond_incoterm-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/hu.po` & `trytond_incoterm-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/id.po` & `trytond_incoterm-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/it.po` & `trytond_incoterm-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/lo.po` & `trytond_incoterm-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/lt.po` & `trytond_incoterm-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/nl.po` & `trytond_incoterm-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/pl.po` & `trytond_incoterm-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/pt.po` & `trytond_incoterm-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/ro.po` & `trytond_incoterm-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/ru.po` & `trytond_incoterm-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/sl.po` & `trytond_incoterm-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/tr.po` & `trytond_incoterm-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/uk.po` & `trytond_incoterm-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/locale/zh_CN.po` & `trytond_incoterm-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/message.xml` & `trytond_incoterm-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/party.py` & `trytond_incoterm-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/party.xml` & `trytond_incoterm-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/purchase.py` & `trytond_incoterm-6.8.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/purchase.xml` & `trytond_incoterm-6.8.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/sale.py` & `trytond_incoterm-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/sale.xml` & `trytond_incoterm-6.8.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/setup.py` & `trytond_incoterm-6.8.0/setup.py`

 * *Files 16% similar despite different names*

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
@@ -37,34 +34,20 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_incoterm'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-
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
+
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
@@ -77,34 +60,28 @@
     get_require_version('trytond_purchase_request_quotation'),
     get_require_version('trytond_sale'),
     get_require_version('trytond_sale_shipment_cost'),
     get_require_version('trytond_sale_opportunity'),
     get_require_version('trytond_sale_invoice_grouping'),
     get_require_version('trytond_stock'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version)
-        )
 
 setup(name=name,
     version=version,
     description='Tryton module for incoterms',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-incoterm/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/incoterm',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton incoterm',
     package_dir={'trytond.modules.incoterm': '.'},
     packages=(
         ['trytond.modules.incoterm']
         + ['trytond.modules.incoterm.%s' % p
             for p in find_packages()]
@@ -142,27 +119,26 @@
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
     incoterm = trytond.modules.incoterm
     """,  # noqa: E501
     )
```

### Comparing `trytond_incoterm-6.6.0/stock.py` & `trytond_incoterm-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/stock.xml` & `trytond_incoterm-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/tests/scenario_incoterm.rst` & `trytond_incoterm-6.8.0/tests/scenario_incoterm.rst`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/tests/test_module.py` & `trytond_incoterm-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/trytond_incoterm.egg-info/PKG-INFO` & `trytond_incoterm-6.8.0/trytond_incoterm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-incoterm
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for incoterms
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-incoterm/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/incoterm
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton incoterm
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
 
 ###############
 Incoterm Module
 ###############
```

### Comparing `trytond_incoterm-6.6.0/trytond_incoterm.egg-info/SOURCES.txt` & `trytond_incoterm-6.8.0/trytond_incoterm.egg-info/SOURCES.txt`

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
```

### Comparing `trytond_incoterm-6.6.0/view/incoterm_form.xml` & `trytond_incoterm-6.8.0/view/incoterm_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_incoterm-6.6.0/view/party_incoterm_form.xml` & `trytond_incoterm-6.8.0/view/party_incoterm_form.xml`

 * *Files identical despite different names*

