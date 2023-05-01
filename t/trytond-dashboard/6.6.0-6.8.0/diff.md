# Comparing `tmp/trytond_dashboard-6.6.0.tar.gz` & `tmp/trytond_dashboard-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_dashboard-6.6.0.tar", last modified: Mon Oct 31 15:46:35 2022, max compression
+gzip compressed data, was "trytond_dashboard-6.8.0.tar", last modified: Mon May  1 11:46:37 2023, max compression
```

## Comparing `trytond_dashboard-6.6.0.tar` & `trytond_dashboard-6.8.0.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:46:35.168786 trytond_dashboard-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_dashboard-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_dashboard-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1269 2022-10-31 15:46:33.000000 trytond_dashboard-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_dashboard-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2247 2022-10-31 15:46:33.000000 trytond_dashboard-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2022-10-31 15:46:32.000000 trytond_dashboard-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_dashboard-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2207 2022-10-31 15:46:35.168786 trytond_dashboard-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2019-06-04 16:49:44.000000 trytond_dashboard-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2021-12-11 16:59:33.000000 trytond_dashboard-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      923 2022-10-11 19:49:57.000000 trytond_dashboard-6.6.0/dashboard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1013 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/dashboard.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:46:35.165453 trytond_dashboard-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2019-06-04 16:49:44.000000 trytond_dashboard-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4742 2021-12-11 16:59:33.000000 trytond_dashboard-6.6.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2021-02-27 17:17:01.000000 trytond_dashboard-6.6.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:46:35.165453 trytond_dashboard-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1357 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1054 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1169 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1221 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1191 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1054 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1172 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1468 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1148 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1178 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1211 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1054 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1401 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1117 2022-10-29 07:50:37.000000 trytond_dashboard-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      912 2020-03-01 11:49:45.000000 trytond_dashboard-6.6.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      808 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:46:35.168786 trytond_dashboard-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4890 2022-10-29 07:39:10.000000 trytond_dashboard-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:46:35.165453 trytond_dashboard-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_dashboard-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2022-04-16 16:30:56.000000 trytond_dashboard-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2022-10-31 15:10:09.000000 trytond_dashboard-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       93 2022-10-31 15:46:31.000000 trytond_dashboard-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:46:35.168786 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2207 2022-10-31 15:46:34.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1641 2022-10-31 15:46:35.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:46:34.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2022-10-31 15:46:34.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:56.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       39 2022-10-31 15:46:34.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:46:34.000000 trytond_dashboard-6.6.0/trytond_dashboard.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:46:35.165453 trytond_dashboard-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/view/action_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/view/action_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      188 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/view/dashboard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2019-02-13 10:09:32.000000 trytond_dashboard-6.6.0/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:37.599487 trytond_dashboard-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2410 2023-05-01 11:04:28.000000 trytond_dashboard-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 11:04:28.000000 trytond_dashboard-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2205 2023-05-01 11:46:37.599487 trytond_dashboard-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      923 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/dashboard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1013 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/dashboard.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:37.596154 trytond_dashboard-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4742 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:37.592821 trytond_dashboard-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1054 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1169 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1221 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1191 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1054 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1172 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1468 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1148 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1178 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1211 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1054 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1401 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1117 2023-04-29 08:02:44.000000 trytond_dashboard-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      912 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      808 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:46:37.599487 trytond_dashboard-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4084 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:37.592821 trytond_dashboard-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_dashboard-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       93 2023-05-01 11:04:23.000000 trytond_dashboard-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:37.596154 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2205 2023-05-01 11:46:36.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1615 2023-05-01 11:46:37.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:46:36.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2023-05-01 11:46:36.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       39 2023-05-01 11:46:36.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:46:36.000000 trytond_dashboard-6.8.0/trytond_dashboard.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:37.596154 trytond_dashboard-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/view/action_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/view/action_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      188 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/view/dashboard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-01-16 14:00:20.000000 trytond_dashboard-6.8.0/view/user_form_preferences.xml
```

### Comparing `trytond_dashboard-6.6.0/CHANGELOG` & `trytond_dashboard-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_dashboard-6.6.0/COPYRIGHT` & `trytond_dashboard-6.8.0/COPYRIGHT`

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

### Comparing `trytond_dashboard-6.6.0/LICENSE` & `trytond_dashboard-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/PKG-INFO` & `trytond_dashboard-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_dashboard
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for dashboard
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
-Project-URL: Source Code, https://hg.tryton.org/modules/dashboard
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton dashboard
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,20 +37,20 @@
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
 
 Dashboard Module
 ################
 
 The dashboard module allows user to configure his dashboard.
```

### Comparing `trytond_dashboard-6.6.0/dashboard.py` & `trytond_dashboard-6.8.0/dashboard.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/dashboard.xml` & `trytond_dashboard-6.8.0/dashboard.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/ir.py` & `trytond_dashboard-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/ir.xml` & `trytond_dashboard-6.8.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/bg.po` & `trytond_dashboard-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/ca.po` & `trytond_dashboard-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/cs.po` & `trytond_dashboard-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/de.po` & `trytond_dashboard-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/es.po` & `trytond_dashboard-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/es_419.po` & `trytond_dashboard-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/et.po` & `trytond_dashboard-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/fa.po` & `trytond_dashboard-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/fi.po` & `trytond_dashboard-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/fr.po` & `trytond_dashboard-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/hu.po` & `trytond_dashboard-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/id.po` & `trytond_dashboard-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/it.po` & `trytond_dashboard-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/lo.po` & `trytond_dashboard-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/lt.po` & `trytond_dashboard-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/nl.po` & `trytond_dashboard-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/pl.po` & `trytond_dashboard-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/pt.po` & `trytond_dashboard-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/ro.po` & `trytond_dashboard-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/ru.po` & `trytond_dashboard-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/sl.po` & `trytond_dashboard-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/tr.po` & `trytond_dashboard-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/uk.po` & `trytond_dashboard-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/locale/zh_CN.po` & `trytond_dashboard-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/res.py` & `trytond_dashboard-6.8.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/res.xml` & `trytond_dashboard-6.8.0/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/setup.py` & `trytond_dashboard-6.8.0/setup.py`

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
 name = 'trytond_dashboard'
 
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
 
 requires = ['lxml', 'python-sql >= 0.4']
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
     description='Tryton module for dashboard',
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
-        "Source Code": 'https://hg.tryton.org/modules/dashboard',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton dashboard',
     package_dir={'trytond.modules.dashboard': '.'},
     packages=(
         ['trytond.modules.dashboard']
         + ['trytond.modules.dashboard.%s' % p for p in find_packages()]
         ),
@@ -121,24 +98,23 @@
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
     dashboard = trytond.modules.dashboard
     """,
     )
```

### Comparing `trytond_dashboard-6.6.0/tests/test_module.py` & `trytond_dashboard-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/trytond_dashboard.egg-info/PKG-INFO` & `trytond_dashboard-6.8.0/trytond_dashboard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-dashboard
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for dashboard
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
-Project-URL: Source Code, https://hg.tryton.org/modules/dashboard
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton dashboard
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,20 +37,20 @@
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
 
 Dashboard Module
 ################
 
 The dashboard module allows user to configure his dashboard.
```

### Comparing `trytond_dashboard-6.6.0/trytond_dashboard.egg-info/SOURCES.txt` & `trytond_dashboard-6.8.0/trytond_dashboard.egg-info/SOURCES.txt`

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
 dashboard.py
@@ -53,14 +49,15 @@
 ./tests/test_module.py
 ./view/action_form.xml
 ./view/action_tree.xml
 ./view/action_tree_sequence.xml
 ./view/dashboard.xml
 ./view/user_form.xml
 ./view/user_form_preferences.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_dashboard-6.6.0/view/user_form.xml` & `trytond_dashboard-6.8.0/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_dashboard-6.6.0/view/user_form_preferences.xml` & `trytond_dashboard-6.8.0/view/user_form_preferences.xml`

 * *Files identical despite different names*

