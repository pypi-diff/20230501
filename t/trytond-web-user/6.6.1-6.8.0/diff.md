# Comparing `tmp/trytond_web_user-6.6.1.tar.gz` & `tmp/trytond_web_user-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_user-6.6.1.tar", last modified: Sat Apr  1 22:01:46 2023, max compression
+gzip compressed data, was "trytond_web_user-6.8.0.tar", last modified: Mon May  1 11:36:37 2023, max compression
```

## Comparing `trytond_web_user-6.6.1.tar` & `trytond_web_user-6.8.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:01:46.931747 trytond_web_user-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1479 2023-04-01 22:01:40.000000 trytond_web_user-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-04-01 22:01:40.000000 trytond_web_user-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3309 2023-04-01 22:01:46.931747 trytond_web_user-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1119 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      677 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:01:46.925076 trytond_web_user-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1119 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1483 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/email_validation.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:01:46.921741 trytond_web_user-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4245 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4854 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4999 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4958 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3772 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4190 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5370 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4939 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4691 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4314 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4259 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6212 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4068 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4706 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3827 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4626 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3998 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4585 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:01:46.931747 trytond_web_user-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4295 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:01:46.925076 trytond_web_user-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6682 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       83 2022-12-19 12:03:07.000000 trytond_web_user-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:01:46.931747 trytond_web_user-6.6.1/trytond_web_user.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3309 2023-04-01 22:01:45.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1470 2023-04-01 22:01:46.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:01:45.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-04-01 22:01:45.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:01:45.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-01 22:01:45.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:01:45.000000 trytond_web_user-6.6.1/trytond_web_user.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    17725 2023-03-18 11:05:56.000000 trytond_web_user-6.6.1/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:01:46.925076 trytond_web_user-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      837 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2022-12-19 12:02:59.000000 trytond_web_user-6.6.1/view/user_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:37.045368 trytond_web_user-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1541 2023-05-01 10:57:52.000000 trytond_web_user-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:57:52.000000 trytond_web_user-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_web_user-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3336 2023-05-01 11:36:37.045368 trytond_web_user-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1147 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      677 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:37.042034 trytond_web_user-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1147 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1483 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/email_validation.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:37.038701 trytond_web_user-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4245 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4854 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4999 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4958 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3772 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4190 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5370 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4939 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4691 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4314 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4259 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4068 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4706 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3827 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4626 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3998 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4585 2023-04-29 08:02:39.000000 trytond_web_user-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2023-04-29 22:04:03.000000 trytond_web_user-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:36:37.045368 trytond_web_user-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4266 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:37.038701 trytond_web_user-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6682 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       83 2023-05-01 10:57:46.000000 trytond_web_user-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:37.045368 trytond_web_user-6.8.0/trytond_web_user.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3336 2023-05-01 11:36:36.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1470 2023-05-01 11:36:36.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:36:36.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-05-01 11:36:36.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 11:36:36.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:36:36.000000 trytond_web_user-6.8.0/trytond_web_user.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    17725 2023-04-29 22:04:03.000000 trytond_web_user-6.8.0/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:36:37.042034 trytond_web_user-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_web_user-6.8.0/view/user_list.xml
```

### Comparing `trytond_web_user-6.6.1/CHANGELOG` & `trytond_web_user-6.8.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-04-01
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add expire delay in reset password email
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_web_user-6.6.1/COPYRIGHT` & `trytond_web_user-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/LICENSE` & `trytond_web_user-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/PKG-INFO` & `trytond_web_user-6.8.0/trytond_web_user.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_web_user
-Version: 6.6.1
+Name: trytond-web-user
+Version: 6.8.0
 Summary: Tryton module to manage Web users
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
-Project-URL: Source Code, https://hg.tryton.org/modules/web_user
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web user
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 Provides-Extra: BCrypt
 Provides-Extra: test
 Provides-Extra: html2text
 License-File: LICENSE
 
 Web User Module
 ###############
@@ -73,26 +73,27 @@
   to set a new password.
 
 Configuration
 *************
 
 The web_user module uses parameters from different sections:
 
-- `web`:
+- ``web``:
 
-    - `reset_password_url`: the URL to reset the password to which the
-      parameters `email` and `token` will be added.
+    - ``reset_password_url``: the URL to reset the password to which the
+      parameters ``email`` and ``token`` will be added.
 
-    - `email_validation_url`: the URL for email validation to which the
-      parameter `token` will be added.
+    - ``email_validation_url``: the URL for email validation to which the
+      parameter ``token`` will be added.
 
-- `email`:
+- ``email``:
 
-    - `from`: the origin address to send emails.
+    - ``from``: the origin address to send emails.
 
-- `session`:
+- ``session``:
 
-    - `web_timeout`: defines in seconds the validity of the web session.
+    - ``web_timeout``: defines in seconds the validity of the web session.
       Default: 30 days.
 
-    - `web_timeout_reset`: in seconds the validity of the reset password token.
+    - ``web_timeout_reset``: in seconds the validity of the reset password
+      token.
       Default: 1 day.
```

### Comparing `trytond_web_user-6.6.1/README.rst` & `trytond_web_user-6.8.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -18,26 +18,27 @@
   to set a new password.
 
 Configuration
 *************
 
 The web_user module uses parameters from different sections:
 
-- `web`:
+- ``web``:
 
-    - `reset_password_url`: the URL to reset the password to which the
-      parameters `email` and `token` will be added.
+    - ``reset_password_url``: the URL to reset the password to which the
+      parameters ``email`` and ``token`` will be added.
 
-    - `email_validation_url`: the URL for email validation to which the
-      parameter `token` will be added.
+    - ``email_validation_url``: the URL for email validation to which the
+      parameter ``token`` will be added.
 
-- `email`:
+- ``email``:
 
-    - `from`: the origin address to send emails.
+    - ``from``: the origin address to send emails.
 
-- `session`:
+- ``session``:
 
-    - `web_timeout`: defines in seconds the validity of the web session.
+    - ``web_timeout``: defines in seconds the validity of the web session.
       Default: 30 days.
 
-    - `web_timeout_reset`: in seconds the validity of the reset password token.
+    - ``web_timeout_reset``: in seconds the validity of the reset password
+      token.
       Default: 1 day.
```

### Comparing `trytond_web_user-6.6.1/__init__.py` & `trytond_web_user-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/doc/conf.py` & `trytond_web_user-6.8.0/doc/conf.py`

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

### Comparing `trytond_web_user-6.6.1/doc/index.rst` & `trytond_web_user-6.8.0/doc/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -18,26 +18,27 @@
   to set a new password.
 
 Configuration
 *************
 
 The web_user module uses parameters from different sections:
 
-- `web`:
+- ``web``:
 
-    - `reset_password_url`: the URL to reset the password to which the
-      parameters `email` and `token` will be added.
+    - ``reset_password_url``: the URL to reset the password to which the
+      parameters ``email`` and ``token`` will be added.
 
-    - `email_validation_url`: the URL for email validation to which the
-      parameter `token` will be added.
+    - ``email_validation_url``: the URL for email validation to which the
+      parameter ``token`` will be added.
 
-- `email`:
+- ``email``:
 
-    - `from`: the origin address to send emails.
+    - ``from``: the origin address to send emails.
 
-- `session`:
+- ``session``:
 
-    - `web_timeout`: defines in seconds the validity of the web session.
+    - ``web_timeout``: defines in seconds the validity of the web session.
       Default: 30 days.
 
-    - `web_timeout_reset`: in seconds the validity of the reset password token.
+    - ``web_timeout_reset``: in seconds the validity of the reset password
+      token.
       Default: 1 day.
```

### Comparing `trytond_web_user-6.6.1/email_reset_password.html` & `trytond_web_user-6.8.0/email_reset_password.html`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/email_validation.html` & `trytond_web_user-6.8.0/email_validation.html`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/ir.py` & `trytond_web_user-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/bg.po` & `trytond_web_user-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/ca.po` & `trytond_web_user-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/cs.po` & `trytond_web_user-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/de.po` & `trytond_web_user-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/es.po` & `trytond_web_user-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/es_419.po` & `trytond_web_user-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/et.po` & `trytond_web_user-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/fa.po` & `trytond_web_user-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/fi.po` & `trytond_web_user-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/fr.po` & `trytond_web_user-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/hu.po` & `trytond_web_user-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/id.po` & `trytond_web_user-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/it.po` & `trytond_web_user-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/lo.po` & `trytond_web_user-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/lt.po` & `trytond_web_user-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/nl.po` & `trytond_web_user-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/pl.po` & `trytond_web_user-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/pt.po` & `trytond_web_user-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/ro.po` & `trytond_web_user-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/ru.po` & `trytond_web_user-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/sl.po` & `trytond_web_user-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/tr.po` & `trytond_web_user-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/uk.po` & `trytond_web_user-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/locale/zh_CN.po` & `trytond_web_user-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/message.xml` & `trytond_web_user-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/party.py` & `trytond_web_user-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/setup.py` & `trytond_web_user-6.8.0/setup.py`

 * *Files 9% similar despite different names*

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
@@ -34,38 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_web_user'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = []
 
 setup(name=name,
     version=version,
     description='Tryton module to manage Web users',
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
-        "Source Code": 'https://hg.tryton.org/modules/web_user',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='web user',
     package_dir={'trytond.modules.web_user': '.'},
     packages=(
         ['trytond.modules.web_user']
         + ['trytond.modules.web_user.%s' % p for p in find_packages()]
         ),
@@ -101,23 +101,23 @@
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
         'BCrypt': ['bcrypt'],
         'test': tests_require,
         'html2text': ['html2text'],
         },
     zip_safe=False,
```

### Comparing `trytond_web_user-6.6.1/tests/test_module.py` & `trytond_web_user-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/trytond_web_user.egg-info/PKG-INFO` & `trytond_web_user-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-web-user
-Version: 6.6.1
+Name: trytond_web_user
+Version: 6.8.0
 Summary: Tryton module to manage Web users
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
-Project-URL: Source Code, https://hg.tryton.org/modules/web_user
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web user
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -37,21 +37,21 @@
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
 Provides-Extra: BCrypt
 Provides-Extra: test
 Provides-Extra: html2text
 License-File: LICENSE
 
 Web User Module
 ###############
@@ -73,26 +73,27 @@
   to set a new password.
 
 Configuration
 *************
 
 The web_user module uses parameters from different sections:
 
-- `web`:
+- ``web``:
 
-    - `reset_password_url`: the URL to reset the password to which the
-      parameters `email` and `token` will be added.
+    - ``reset_password_url``: the URL to reset the password to which the
+      parameters ``email`` and ``token`` will be added.
 
-    - `email_validation_url`: the URL for email validation to which the
-      parameter `token` will be added.
+    - ``email_validation_url``: the URL for email validation to which the
+      parameter ``token`` will be added.
 
-- `email`:
+- ``email``:
 
-    - `from`: the origin address to send emails.
+    - ``from``: the origin address to send emails.
 
-- `session`:
+- ``session``:
 
-    - `web_timeout`: defines in seconds the validity of the web session.
+    - ``web_timeout``: defines in seconds the validity of the web session.
       Default: 30 days.
 
-    - `web_timeout_reset`: in seconds the validity of the reset password token.
+    - ``web_timeout_reset``: in seconds the validity of the reset password
+      token.
       Default: 1 day.
```

### Comparing `trytond_web_user-6.6.1/trytond_web_user.egg-info/SOURCES.txt` & `trytond_web_user-6.8.0/trytond_web_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/user.py` & `trytond_web_user-6.8.0/user.py`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/user.xml` & `trytond_web_user-6.8.0/user.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_user-6.6.1/view/user_form.xml` & `trytond_web_user-6.8.0/view/user_form.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_web_user-6.6.1/view/user_form.xml` & `trytond_web_user-6.8.0/view/user_form.xml`

```diff
@@ -7,15 +7,15 @@
     <field name="party"/>
     <label name="active"/>
     <field name="active"/>
     <label name="email"/>
     <field name="email" widget="email"/>
     <newline/>
   </group>
-  <field name="avatar" widget="image" height="100" width="100" xexpand="0"/>
+  <field name="avatar" widget="image" height="100" width="100" xexpand="0" border="circle"/>
   <label name="password"/>
   <field name="password" widget="password"/>
   <button name="reset_password" colspan="2"/>
   <label name="email_valid"/>
   <field name="email_valid"/>
   <button name="validate_email" colspan="2"/>
   <field name="secondary_parties" colspan="4"/>
```

