# Comparing `tmp/trytond_country-6.6.1.tar.gz` & `tmp/trytond_country-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_country-6.6.1.tar", last modified: Sun Feb  5 21:21:24 2023, max compression
+gzip compressed data, was "trytond_country-6.8.0.tar", last modified: Mon May  1 12:06:07 2023, max compression
```

## Comparing `trytond_country-6.6.1.tar` & `trytond_country-6.8.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.473002 trytond_country-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     3665 2023-02-05 21:21:21.000000 trytond_country-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-02-05 21:21:20.000000 trytond_country-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_country-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_country-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-02-05 21:21:24.469669 trytond_country-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-12-19 12:02:49.000000 trytond_country-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2022-12-19 12:02:49.000000 trytond_country-6.6.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20860 2022-12-19 12:02:49.000000 trytond_country-6.6.1/country.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13472 2022-12-19 12:02:49.000000 trytond_country-6.6.1/country.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.469669 trytond_country-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_country-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2738 2022-12-19 12:02:49.000000 trytond_country-6.6.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2022-12-19 12:02:49.000000 trytond_country-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:49.000000 trytond_country-6.6.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2022-12-19 12:02:49.000000 trytond_country-6.6.1/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2022-12-19 12:02:49.000000 trytond_country-6.6.1/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.469669 trytond_country-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:49.000000 trytond_country-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2022-12-19 12:02:49.000000 trytond_country-6.6.1/icons/tryton-country.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.459668 trytond_country-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    25666 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25651 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22688 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25659 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25807 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22530 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24628 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25889 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22571 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25743 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23696 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21710 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22889 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25695 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25164 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25471 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25421 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    25039 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23473 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    26709 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    24811 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    22475 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    27230 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    23084 2022-12-19 12:02:49.000000 trytond_country-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4126 2022-12-19 12:02:49.000000 trytond_country-6.6.1/organization.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8410 2022-12-19 12:02:49.000000 trytond_country-6.6.1/region.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.463002 trytond_country-6.6.1/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_country-6.6.1/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)    19990 2022-12-19 12:02:49.000000 trytond_country-6.6.1/scripts/import_countries.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4050 2023-02-05 20:48:28.000000 trytond_country-6.6.1/scripts/import_postal_codes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-02-05 21:21:24.473002 trytond_country-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4887 2022-12-19 12:02:49.000000 trytond_country-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.463002 trytond_country-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_country-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2022-12-19 12:02:49.000000 trytond_country-6.6.1/tests/scenario_country_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3259 2022-12-19 12:02:49.000000 trytond_country-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:49.000000 trytond_country-6.6.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2022-12-19 12:02:49.000000 trytond_country-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2022-12-19 12:03:07.000000 trytond_country-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.469669 trytond_country-6.6.1/trytond_country.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-02-05 21:21:23.000000 trytond_country-6.6.1/trytond_country.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2395 2023-02-05 21:21:24.000000 trytond_country-6.6.1/trytond_country.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:21:23.000000 trytond_country-6.6.1/trytond_country.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-02-05 21:21:23.000000 trytond_country-6.6.1/trytond_country.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-05 21:21:23.000000 trytond_country-6.6.1/trytond_country.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-02-05 21:21:23.000000 trytond_country-6.6.1/trytond_country.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-02-05 21:21:23.000000 trytond_country-6.6.1/trytond_country.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-02-05 21:21:24.466335 trytond_country-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/country_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/organization_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/organization_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/organization_member_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/organization_member_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/postal_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/postal_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/region_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/region_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/subdivision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2022-12-19 12:02:49.000000 trytond_country-6.6.1/view/subdivision_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.547339 trytond_country-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3728 2023-05-01 11:17:57.000000 trytond_country-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2023-05-01 11:17:57.000000 trytond_country-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_country-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_country-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-05-01 12:06:07.544006 trytond_country-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_country-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20860 2023-04-15 07:12:15.000000 trytond_country-6.8.0/country.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13472 2023-04-15 07:12:15.000000 trytond_country-6.8.0/country.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.540672 trytond_country-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_country-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2738 2023-04-15 07:12:15.000000 trytond_country-6.8.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_country-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_country-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1114 2023-04-21 08:36:08.000000 trytond_country-6.8.0/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_country-6.8.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.544006 trytond_country-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_country-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-01-16 14:00:20.000000 trytond_country-6.8.0/icons/tryton-country.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.537339 trytond_country-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    25666 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25651 2023-04-29 08:02:54.000000 trytond_country-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22688 2023-04-29 08:02:51.000000 trytond_country-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25659 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25807 2023-04-29 08:02:51.000000 trytond_country-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22530 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24628 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25889 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22571 2023-04-29 08:02:54.000000 trytond_country-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25743 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23696 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21710 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22889 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25695 2023-04-29 08:02:54.000000 trytond_country-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25164 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25471 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25421 2023-04-29 08:02:54.000000 trytond_country-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    25039 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23473 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    26709 2023-04-29 08:02:54.000000 trytond_country-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    24811 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    22475 2023-04-29 08:02:52.000000 trytond_country-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    27230 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    23084 2023-04-29 08:02:53.000000 trytond_country-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-04-15 07:12:15.000000 trytond_country-6.8.0/organization.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8410 2023-04-15 07:12:15.000000 trytond_country-6.8.0/region.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.537339 trytond_country-6.8.0/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-6.8.0/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)    19990 2023-04-15 07:12:15.000000 trytond_country-6.8.0/scripts/import_countries.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4050 2023-04-15 07:12:15.000000 trytond_country-6.8.0/scripts/import_postal_codes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:06:07.547339 trytond_country-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4859 2023-04-15 07:12:15.000000 trytond_country-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.537339 trytond_country-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_country-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_country-6.8.0/tests/scenario_country_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3259 2023-04-15 07:12:15.000000 trytond_country-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_country-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_country-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-05-01 11:17:51.000000 trytond_country-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.544006 trytond_country-6.8.0/trytond_country.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-05-01 12:06:06.000000 trytond_country-6.8.0/trytond_country.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2395 2023-05-01 12:06:07.000000 trytond_country-6.8.0/trytond_country.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:06:06.000000 trytond_country-6.8.0/trytond_country.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-05-01 12:06:06.000000 trytond_country-6.8.0/trytond_country.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_country-6.8.0/trytond_country.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-05-01 12:06:06.000000 trytond_country-6.8.0/trytond_country.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:06:06.000000 trytond_country-6.8.0/trytond_country.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:06:07.540672 trytond_country-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/country_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/organization_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/organization_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/organization_member_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/organization_member_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/postal_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/postal_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/region_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/region_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/subdivision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2023-04-15 07:12:15.000000 trytond_country-6.8.0/view/subdivision_tree.xml
```

### Comparing `trytond_country-6.6.1/CHANGELOG` & `trytond_country-6.8.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-Version 6.6.1 - 2023-02-05
+
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add country organizations
 * Add UN M49 regions
 * Add flag symbol for country and subdivision
```

### Comparing `trytond_country-6.6.1/COPYRIGHT` & `trytond_country-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/LICENSE` & `trytond_country-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/PKG-INFO` & `trytond_country-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_country
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with countries
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-country/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/country
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton country
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
 Provides-Extra: data
 Provides-Extra: test
 Provides-Extra: GeoNames
 Provides-Extra: completion
 License-File: LICENSE
 
 ##############
```

### Comparing `trytond_country-6.6.1/country.py` & `trytond_country-6.8.0/country.py`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/country.xml` & `trytond_country-6.8.0/country.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/doc/conf.py` & `trytond_country-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
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
```

### Comparing `trytond_country-6.6.1/doc/design.rst` & `trytond_country-6.8.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/doc/setup.rst` & `trytond_country-6.8.0/doc/setup.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 =================================
 
 You can use the :command:`trytond_import_postal_codes` script to load and update
 the `Postal Codes <model-country.postal_code>` in Tryton from the `GeoNames
 Database`_.
 It is run with:
 
-.. code-block:: bash
+.. code-block:: console
 
-   trytond_import_postal_codes -c trytond.conf -d <database> <two_letter_country_code>
+   $ trytond_import_postal_codes -c trytond.conf -d <database> <two_letter_country_code>
 
 .. _GeoNames Database: https://www.geonames.org/
```

### Comparing `trytond_country-6.6.1/icons/LICENSE` & `trytond_country-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/bg.po` & `trytond_country-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/ca.po` & `trytond_country-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/cs.po` & `trytond_country-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/de.po` & `trytond_country-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/es.po` & `trytond_country-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/es_419.po` & `trytond_country-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/et.po` & `trytond_country-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/fa.po` & `trytond_country-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/fi.po` & `trytond_country-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/fr.po` & `trytond_country-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/hu.po` & `trytond_country-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/id.po` & `trytond_country-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/it.po` & `trytond_country-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/lo.po` & `trytond_country-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/lt.po` & `trytond_country-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/nl.po` & `trytond_country-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/pl.po` & `trytond_country-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/pt.po` & `trytond_country-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/ro.po` & `trytond_country-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/ru.po` & `trytond_country-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/sl.po` & `trytond_country-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/tr.po` & `trytond_country-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/uk.po` & `trytond_country-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/locale/zh_CN.po` & `trytond_country-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/organization.xml` & `trytond_country-6.8.0/organization.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/region.xml` & `trytond_country-6.8.0/region.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/scripts/import_countries.py` & `trytond_country-6.8.0/scripts/import_countries.py`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/scripts/import_postal_codes.py` & `trytond_country-6.8.0/scripts/import_postal_codes.py`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/setup.py` & `trytond_country-6.8.0/setup.py`

 * *Files 4% similar despite different names*

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
@@ -37,38 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_country'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus'), 'pycountry']
 
 setup(name=name,
     version=version,
     description='Tryton module with countries',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-country/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/country',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton country',
     package_dir={'trytond.modules.country': '.'},
     packages=(
         ['trytond.modules.country']
         + ['trytond.modules.country.%s' % p for p in find_packages()]
         ),
@@ -106,23 +106,23 @@
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
         'data': ['pycountry', get_require_version('proteus')],
         'test': tests_require,
         'GeoNames': [get_require_version('proteus')],
         'completion': ['argcomplete'],
         },
```

### Comparing `trytond_country-6.6.1/tests/scenario_country_import.rst` & `trytond_country-6.8.0/tests/scenario_country_import.rst`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/tests/test_module.py` & `trytond_country-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/tox.ini` & `trytond_country-6.8.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/country/* -m unittest discover -s tests
-    coverage report --include=./**/country/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_country-6.6.1/trytond_country.egg-info/PKG-INFO` & `trytond_country-6.8.0/trytond_country.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-country
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module with countries
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-country/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/country
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton country
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
 Provides-Extra: data
 Provides-Extra: test
 Provides-Extra: GeoNames
 Provides-Extra: completion
 License-File: LICENSE
 
 ##############
```

### Comparing `trytond_country-6.6.1/trytond_country.egg-info/SOURCES.txt` & `trytond_country-6.8.0/trytond_country.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/view/country_form.xml` & `trytond_country-6.8.0/view/country_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_country-6.6.1/view/subdivision_form.xml` & `trytond_country-6.8.0/view/subdivision_form.xml`

 * *Files identical despite different names*

