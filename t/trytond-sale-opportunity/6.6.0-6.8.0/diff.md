# Comparing `tmp/trytond_sale_opportunity-6.6.0.tar.gz` & `tmp/trytond_sale_opportunity-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_opportunity-6.6.0.tar", last modified: Mon Oct 31 16:11:54 2022, max compression
+gzip compressed data, was "trytond_sale_opportunity-6.8.0.tar", last modified: Mon May  1 12:02:18 2023, max compression
```

## Comparing `trytond_sale_opportunity-6.6.0.tar` & `trytond_sale_opportunity-6.8.0.tar`

### file list

```diff
@@ -1,96 +1,93 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.974217 trytond_sale_opportunity-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_sale_opportunity-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_sale_opportunity-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2022-10-31 16:11:53.000000 trytond_sale_opportunity-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_sale_opportunity-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2867 2022-10-31 16:11:52.000000 trytond_sale_opportunity-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2022-10-31 16:11:52.000000 trytond_sale_opportunity-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:04.000000 trytond_sale_opportunity-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_sale_opportunity-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4880 2022-10-31 16:11:54.974217 trytond_sale_opportunity-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2619 2020-03-28 13:26:07.000000 trytond_sale_opportunity-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2020-03-01 11:49:49.000000 trytond_sale_opportunity-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2020-03-01 11:49:49.000000 trytond_sale_opportunity-6.6.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2634 2022-04-10 15:40:35.000000 trytond_sale_opportunity-6.6.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2018-08-18 09:55:04.000000 trytond_sale_opportunity-6.6.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.970883 trytond_sale_opportunity-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2619 2020-03-28 13:26:07.000000 trytond_sale_opportunity-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.970883 trytond_sale_opportunity-6.6.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2020-06-03 15:34:41.000000 trytond_sale_opportunity-6.6.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2020-04-13 10:22:05.000000 trytond_sale_opportunity-6.6.0/icons/tryton-sale-opportunity.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.967550 trytond_sale_opportunity-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14600 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13736 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12974 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13885 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13784 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12973 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13846 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14226 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12965 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13939 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13368 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12635 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13928 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14365 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13127 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13638 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13357 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13930 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12149 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14545 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13910 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12956 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11777 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13037 2022-10-29 07:50:44.000000 trytond_sale_opportunity-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2938 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21589 2022-10-11 19:49:58.000000 trytond_sale_opportunity-6.6.0/opportunity.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11654 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/opportunity.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15459 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/opportunity_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25576 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/opportunity_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      572 2020-03-01 11:49:49.000000 trytond_sale_opportunity-6.6.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1280 2020-04-13 10:22:05.000000 trytond_sale_opportunity-6.6.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2020-03-01 11:49:49.000000 trytond_sale_opportunity-6.6.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2275 2021-12-11 16:59:34.000000 trytond_sale_opportunity-6.6.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:11:54.974217 trytond_sale_opportunity-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5235 2022-10-29 07:39:11.000000 trytond_sale_opportunity-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.967550 trytond_sale_opportunity-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_sale_opportunity-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5463 2021-03-24 12:36:50.000000 trytond_sale_opportunity-6.6.0/tests/scenario_sale_opportunity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4099 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/tests/scenario_sale_opportunity_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2022-04-16 16:30:57.000000 trytond_sale_opportunity-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_sale_opportunity-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2022-10-31 15:10:09.000000 trytond_sale_opportunity-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2022-10-31 16:11:51.000000 trytond_sale_opportunity-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.970883 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4880 2022-10-31 16:11:54.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4130 2022-10-31 16:11:54.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:11:54.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 16:11:54.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:12.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-10-31 16:11:54.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:11:54.000000 trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:11:54.970883 trytond_sale_opportunity-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2018-08-18 09:55:04.000000 trytond_sale_opportunity-6.6.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2303 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2018-08-18 09:55:04.000000 trytond_sale_opportunity-6.6.0/view/opportunity_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2020-10-09 17:09:19.000000 trytond_sale_opportunity-6.6.0/view/opportunity_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_employee_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_employee_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_employee_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      573 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      783 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2022-09-12 22:47:25.000000 trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      781 2022-04-08 16:23:26.000000 trytond_sale_opportunity-6.6.0/view/opportunity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2020-04-13 10:22:05.000000 trytond_sale_opportunity-6.6.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.461163 trytond_sale_opportunity-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2023-05-01 11:15:16.000000 trytond_sale_opportunity-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-05-01 11:15:15.000000 trytond_sale_opportunity-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_opportunity-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-05-01 12:02:18.461163 trytond_sale_opportunity-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2619 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2634 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-01-16 14:00:21.000000 trytond_sale_opportunity-6.8.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.454496 trytond_sale_opportunity-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2619 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.457830 trytond_sale_opportunity-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/icons/tryton-sale-opportunity.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.444496 trytond_sale_opportunity-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14600 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13736 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12974 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13885 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13784 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12973 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13846 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14226 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12965 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13939 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13368 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12635 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13928 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14365 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13127 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13638 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13357 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13930 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12149 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14545 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13910 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12956 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11777 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13037 2023-04-29 08:02:50.000000 trytond_sale_opportunity-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2938 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22349 2023-04-21 08:36:08.000000 trytond_sale_opportunity-6.8.0/opportunity.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11654 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/opportunity.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15574 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/opportunity_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25576 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/opportunity_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2236 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:02:18.461163 trytond_sale_opportunity-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4423 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.447830 trytond_sale_opportunity-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5463 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/tests/scenario_sale_opportunity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4099 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/tests/scenario_sale_opportunity_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-05-01 11:15:10.000000 trytond_sale_opportunity-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.457830 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-05-01 12:02:17.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4104 2023-05-01 12:02:18.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:02:17.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 12:02:17.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-05-01 12:02:17.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:02:17.000000 trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:02:18.454496 trytond_sale_opportunity-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2023-01-16 14:00:21.000000 trytond_sale_opportunity-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2303 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-01-16 14:00:21.000000 trytond_sale_opportunity-6.8.0/view/opportunity_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_employee_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_employee_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_employee_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      573 2023-04-28 07:46:16.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-28 07:46:16.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      783 2023-04-28 07:46:16.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-28 07:46:16.000000 trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      781 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/opportunity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_opportunity-6.8.0/view/party_form.xml
```

### Comparing `trytond_sale_opportunity-6.6.0/CHANGELOG` & `trytond_sale_opportunity-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Allow searching reporting by record name
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Refactor reporting
 * Use default customer payment term
 * Allow to store currency on opportunity
```

### Comparing `trytond_sale_opportunity-6.6.0/COPYRIGHT` & `trytond_sale_opportunity-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2010-2011 Open Labs Business Solutions.
-Copyright (C) 2010-2022 Cédric Krier.
-Copyright (C) 2010-2022 B2CK SPRL.
+Copyright (C) 2010-2023 Cédric Krier.
+Copyright (C) 2010-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_opportunity-6.6.0/LICENSE` & `trytond_sale_opportunity-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/PKG-INFO` & `trytond_sale_opportunity-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_sale_opportunity
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with leads and opportunities
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_opportunity
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale opportunity
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
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 Sale Opportunity Module
 #######################
```

### Comparing `trytond_sale_opportunity-6.6.0/README.rst` & `trytond_sale_opportunity-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/__init__.py` & `trytond_sale_opportunity-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/configuration.py` & `trytond_sale_opportunity-6.8.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/configuration.xml` & `trytond_sale_opportunity-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/doc/index.rst` & `trytond_sale_opportunity-6.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/icons/LICENSE` & `trytond_sale_opportunity-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/bg.po` & `trytond_sale_opportunity-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/ca.po` & `trytond_sale_opportunity-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/cs.po` & `trytond_sale_opportunity-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/de.po` & `trytond_sale_opportunity-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/es.po` & `trytond_sale_opportunity-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/es_419.po` & `trytond_sale_opportunity-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/et.po` & `trytond_sale_opportunity-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/fa.po` & `trytond_sale_opportunity-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/fi.po` & `trytond_sale_opportunity-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/fr.po` & `trytond_sale_opportunity-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/hu.po` & `trytond_sale_opportunity-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/id.po` & `trytond_sale_opportunity-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/it.po` & `trytond_sale_opportunity-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/lo.po` & `trytond_sale_opportunity-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/lt.po` & `trytond_sale_opportunity-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/nl.po` & `trytond_sale_opportunity-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/pl.po` & `trytond_sale_opportunity-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/pt.po` & `trytond_sale_opportunity-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/ro.po` & `trytond_sale_opportunity-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/ru.po` & `trytond_sale_opportunity-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/sl.po` & `trytond_sale_opportunity-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/tr.po` & `trytond_sale_opportunity-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/uk.po` & `trytond_sale_opportunity-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/locale/zh_CN.po` & `trytond_sale_opportunity-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/message.xml` & `trytond_sale_opportunity-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/opportunity.py` & `trytond_sale_opportunity-6.8.0/opportunity.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,17 @@
             ])
     currency = fields.Many2One(
         'currency.currency', "Currency", required=True, states=_states_start)
     amount = Monetary(
         "Amount", currency='currency', digits='currency',
         states=_states_stop,
         help='Estimated revenue amount.')
-    payment_term = fields.Many2One('account.invoice.payment_term',
-        'Payment Term', states={
+    payment_term = fields.Many2One(
+        'account.invoice.payment_term', "Payment Term", ondelete='RESTRICT',
+        states={
             'readonly': In(Eval('state'),
                 ['converted', 'lost', 'cancelled']),
             })
     employee = fields.Many2One('company.employee', 'Employee',
         states={
             'readonly': _states_stop['readonly'],
             'required': ~Eval('state').in_(['lead', 'lost', 'cancelled']),
@@ -298,14 +299,33 @@
         pool = Pool()
         Configuration = pool.get('account.configuration')
         config = Configuration(1)
         payment_term = config.get_multivalue(
             'default_customer_payment_term', **pattern)
         return payment_term.id if payment_term else None
 
+    def get_rec_name(self, name):
+        items = [self.number]
+        if self.reference:
+            items.append(f'[{self.reference}]')
+        return ' '.join(items)
+
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        _, operator, value = clause
+        if operator.startswith('!') or operator.startswith('not '):
+            bool_op = 'AND'
+        else:
+            bool_op = 'OR'
+        domain = [bool_op,
+            ('number', operator, value),
+            ('reference', operator, value),
+            ]
+        return domain
+
     @classmethod
     def view_attributes(cls):
         return super().view_attributes() + [
             ('/tree', 'visual', If(Eval('state') == 'cancelled', 'muted', '')),
             ]
 
     @classmethod
@@ -545,15 +565,21 @@
         states={
             'readonly': _states['readonly'] & Bool(Eval('opportunity')),
             })
     opportunity_state = fields.Function(
         fields.Selection('get_opportunity_states', "Opportunity State"),
         'on_change_with_opportunity_state')
     product = fields.Many2One('product.product', 'Product', required=True,
-        domain=[('salable', '=', True)], states=_states)
+        domain=[
+            If(Eval('opportunity_state').in_(['lead', 'opportunity'])
+                & ~(Eval('quantity', 0) < 0),
+                ('salable', '=', True),
+                ()),
+            ],
+        states=_states)
     quantity = fields.Float(
         "Quantity", digits='unit', required=True, states=_states)
     unit = fields.Many2One('product.uom', 'Unit', required=True,
         states=_states)
 
     del _states
```

### Comparing `trytond_sale_opportunity-6.6.0/opportunity.xml` & `trytond_sale_opportunity-6.8.0/opportunity.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/opportunity_reporting.py` & `trytond_sale_opportunity-6.8.0/opportunity_reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from itertools import tee, zip_longest
 
 from dateutil.relativedelta import relativedelta
 from sql import Literal, Null, With
 from sql.aggregate import Count, Min, Sum
 from sql.conditionals import Case
 from sql.functions import CurrentTimestamp
+
 try:
     import pygal
 except ImportError:
     pygal = None
 
 from trytond.i18n import lazy_gettext
 from trytond.model import ModelSQL, ModelView, fields
@@ -428,14 +429,18 @@
         opportunity = tables['opportunity']
         return super()._group_by(tables, withs) + [
             opportunity.employee]
 
     def get_rec_name(self, name):
         return self.employee.rec_name
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('employee.rec_name', *clause[1:])]
+
 
 class ConversionEmployee(EmployeeMixin, AbstractConversion, ModelView):
     "Sale Opportunity Reporting Conversion per Employee"
     __name__ = 'sale.opportunity.reporting.conversion.employee'
 
     time_series = fields.One2Many(
         'sale.opportunity.reporting.conversion.employee.time_series',
```

### Comparing `trytond_sale_opportunity-6.6.0/opportunity_reporting.xml` & `trytond_sale_opportunity-6.8.0/opportunity_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/party.py` & `trytond_sale_opportunity-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/party.xml` & `trytond_sale_opportunity-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/sale.py` & `trytond_sale_opportunity-6.8.0/sale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
-from trytond.transaction import Transaction
+from trytond.transaction import without_check_access
 
 
 def process_opportunity(func):
     @wraps(func)
     def wrapper(cls, sales):
         pool = Pool()
         Opportunity = pool.get('sale.opportunity')
-        with Transaction().set_context(_check_access=False):
+        with without_check_access():
             opportunities = Opportunity.browse(
                 set(s.origin for s in cls.browse(sales)
                     if isinstance(s.origin, Opportunity)))
         func(cls, sales)
-        with Transaction().set_context(_check_access=False):
+        with without_check_access():
             Opportunity.process(opportunities)
     return wrapper
 
 
 class Sale(metaclass=PoolMeta):
     __name__ = 'sale.sale'
```

### Comparing `trytond_sale_opportunity-6.6.0/setup.py` & `trytond_sale_opportunity-6.8.0/setup.py`

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
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_opportunity'
 
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
 
 requires = ['python-sql >= 0.4', 'python-dateutil']
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
     description='Tryton module with leads and opportunities',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_opportunity',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale opportunity',
     package_dir={'trytond.modules.sale_opportunity': '.'},
     packages=(
         ['trytond.modules.sale_opportunity']
         + ['trytond.modules.sale_opportunity.%s' % p for p in find_packages()]
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
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'sparklines': ['pygal'],
         'test': tests_require,
         },
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     sale_opportunity = trytond.modules.sale_opportunity
     """,
     )
```

### Comparing `trytond_sale_opportunity-6.6.0/tests/scenario_sale_opportunity.rst` & `trytond_sale_opportunity-6.8.0/tests/scenario_sale_opportunity.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/tests/scenario_sale_opportunity_reporting.rst` & `trytond_sale_opportunity-6.8.0/tests/scenario_sale_opportunity_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/PKG-INFO` & `trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-sale-opportunity
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module with leads and opportunities
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_opportunity
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale opportunity
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
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 Sale Opportunity Module
 #######################
```

### Comparing `trytond_sale_opportunity-6.6.0/trytond_sale_opportunity.egg-info/SOURCES.txt` & `trytond_sale_opportunity-6.8.0/trytond_sale_opportunity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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
@@ -87,14 +83,15 @@
 ./view/opportunity_reporting_main_graph_number.xml
 ./view/opportunity_reporting_main_list.xml
 ./view/opportunity_reporting_main_time_series_graph_amount.xml
 ./view/opportunity_reporting_main_time_series_graph_number.xml
 ./view/opportunity_reporting_main_time_series_list.xml
 ./view/opportunity_tree.xml
 ./view/party_form.xml
+doc/conf.py
 doc/index.rst
 icons/LICENSE
 icons/tryton-sale-opportunity.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
```

### Comparing `trytond_sale_opportunity-6.6.0/view/opportunity_form.xml` & `trytond_sale_opportunity-6.8.0/view/opportunity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/view/opportunity_reporting_conversion_list.xml` & `trytond_sale_opportunity-6.8.0/view/opportunity_reporting_conversion_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/view/opportunity_reporting_main_list.xml` & `trytond_sale_opportunity-6.8.0/view/opportunity_reporting_main_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_opportunity-6.6.0/view/opportunity_tree.xml` & `trytond_sale_opportunity-6.8.0/view/opportunity_tree.xml`

 * *Files identical despite different names*

