# Comparing `tmp/trytond_google_maps-6.6.0.tar.gz` & `tmp/trytond_google_maps-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_google_maps-6.6.0.tar", last modified: Mon Oct 31 15:48:45 2022, max compression
+gzip compressed data, was "trytond_google_maps-6.8.0.tar", last modified: Mon May  1 11:57:01 2023, max compression
```

## Comparing `trytond_google_maps-6.6.0.tar` & `trytond_google_maps-6.8.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:45.354012 trytond_google_maps-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_google_maps-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_google_maps-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1363 2022-10-31 15:48:43.000000 trytond_google_maps-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_google_maps-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2311 2022-10-31 15:48:43.000000 trytond_google_maps-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:48:42.000000 trytond_google_maps-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:38.000000 trytond_google_maps-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_google_maps-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2461 2022-10-31 15:48:45.350679 trytond_google_maps-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      212 2019-06-04 16:49:44.000000 trytond_google_maps-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2021-12-11 16:59:33.000000 trytond_google_maps-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2021-12-11 16:59:33.000000 trytond_google_maps-6.6.0/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2022-06-03 22:25:03.000000 trytond_google_maps-6.6.0/address.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:45.350679 trytond_google_maps-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      212 2019-06-04 16:49:44.000000 trytond_google_maps-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:45.350679 trytond_google_maps-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      140 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2022-10-29 07:50:42.000000 trytond_google_maps-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:48:45.354012 trytond_google_maps-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5011 2022-10-29 07:39:10.000000 trytond_google_maps-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:45.350679 trytond_google_maps-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_google_maps-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1405 2022-04-16 16:30:56.000000 trytond_google_maps-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2022-10-31 15:10:09.000000 trytond_google_maps-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 15:48:41.000000 trytond_google_maps-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:45.350679 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2461 2022-10-31 15:48:44.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1335 2022-10-31 15:48:45.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:48:44.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2022-10-31 15:48:44.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:06.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       42 2022-10-31 15:48:44.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:48:44.000000 trytond_google_maps-6.6.0/trytond_google_maps.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:48:45.350679 trytond_google_maps-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2022-06-03 22:25:03.000000 trytond_google_maps-6.6.0/view/address_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:01.720566 trytond_google_maps-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2474 2023-05-01 11:11:33.000000 trytond_google_maps-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:11:33.000000 trytond_google_maps-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_google_maps-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2457 2023-05-01 11:57:01.720566 trytond_google_maps-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      212 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/address.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:01.717232 trytond_google_maps-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      212 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:01.717232 trytond_google_maps-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      140 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-04-29 08:02:48.000000 trytond_google_maps-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:57:01.720566 trytond_google_maps-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4203 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:01.717232 trytond_google_maps-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1405 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 11:11:26.000000 trytond_google_maps-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:01.720566 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2457 2023-05-01 11:57:00.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-05-01 11:57:01.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:57:00.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-05-01 11:57:00.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-05-01 11:57:00.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:57:00.000000 trytond_google_maps-6.8.0/trytond_google_maps.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:57:01.717232 trytond_google_maps-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_google_maps-6.8.0/view/address_form.xml
```

### Comparing `trytond_google_maps-6.6.0/CHANGELOG` & `trytond_google_maps-6.8.0/CHANGELOG`

 * *Files 14% similar despite different names*

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

### Comparing `trytond_google_maps-6.6.0/COPYRIGHT` & `trytond_google_maps-6.8.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2008-2022 Cédric Krier.
+Copyright (C) 2008-2023 Cédric Krier.
 Copyright (C) 2008-2012 Bertrand Chenal.
-Copyright (C) 2008-2022 B2CK SPRL.
+Copyright (C) 2008-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_google_maps-6.6.0/LICENSE` & `trytond_google_maps-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-6.6.0/PKG-INFO` & `trytond_google_maps-6.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_google_maps
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to link addresses to Google Maps
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
-Project-URL: Source Code, https://hg.tryton.org/modules/google_maps
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton google maps
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
 
 Google Maps Module
 ##################
 
 The Google Maps module add a new URL field on the party
 addresses. This link open the Google Maps page on the default browser
```

### Comparing `trytond_google_maps-6.6.0/address.py` & `trytond_google_maps-6.8.0/address.py`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-6.6.0/address.xml` & `trytond_google_maps-6.8.0/address.xml`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-6.6.0/setup.py` & `trytond_google_maps-6.8.0/setup.py`

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
@@ -34,59 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_google_maps'
 
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
     description='Tryton module to link addresses to Google Maps',
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
-        "Source Code": 'https://hg.tryton.org/modules/google_maps',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton google maps',
     package_dir={'trytond.modules.google_maps': '.'},
     packages=(
         ['trytond.modules.google_maps']
         + ['trytond.modules.google_maps.%s' % p for p in find_packages()]
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
     google_maps = trytond.modules.google_maps
     """,
     )
```

### Comparing `trytond_google_maps-6.6.0/tests/test_module.py` & `trytond_google_maps-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_google_maps-6.6.0/trytond_google_maps.egg-info/PKG-INFO` & `trytond_google_maps-6.8.0/trytond_google_maps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-google-maps
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to link addresses to Google Maps
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
-Project-URL: Source Code, https://hg.tryton.org/modules/google_maps
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton google maps
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
 
 Google Maps Module
 ##################
 
 The Google Maps module add a new URL field on the party
 addresses. This link open the Google Maps page on the default browser
```

### Comparing `trytond_google_maps-6.6.0/trytond_google_maps.egg-info/SOURCES.txt` & `trytond_google_maps-6.8.0/trytond_google_maps.egg-info/SOURCES.txt`

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
@@ -40,14 +36,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/address_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

