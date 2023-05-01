# Comparing `tmp/trytond_notification_email-6.6.0.tar.gz` & `tmp/trytond_notification_email-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_notification_email-6.6.0.tar", last modified: Mon Oct 31 16:15:07 2022, max compression
+gzip compressed data, was "trytond_notification_email-6.8.0.tar", last modified: Mon May  1 11:44:48 2023, max compression
```

## Comparing `trytond_notification_email-6.6.0.tar` & `trytond_notification_email-6.8.0.tar`

### file list

```diff
@@ -1,66 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:07.677019 trytond_notification_email-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:16.000000 trytond_notification_email-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_notification_email-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2022-10-31 16:15:06.000000 trytond_notification_email-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:33.000000 trytond_notification_email-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2022-10-31 16:15:05.000000 trytond_notification_email-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2022-10-31 16:15:05.000000 trytond_notification_email-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_notification_email-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_notification_email-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2022-10-31 16:15:07.677019 trytond_notification_email-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2021-02-03 22:26:17.000000 trytond_notification_email-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2021-12-11 16:59:33.000000 trytond_notification_email-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:07.677019 trytond_notification_email-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2021-02-03 22:26:17.000000 trytond_notification_email-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2020-07-04 20:18:34.000000 trytond_notification_email-6.6.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1648 2022-04-10 15:40:35.000000 trytond_notification_email-6.6.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2019-06-04 16:49:46.000000 trytond_notification_email-6.6.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:07.673685 trytond_notification_email-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6704 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6637 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6754 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4872 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5367 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6552 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6496 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5070 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6423 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6328 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6324 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6146 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6279 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5082 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4872 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5932 2022-10-29 07:50:36.000000 trytond_notification_email-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2020-07-04 20:18:34.000000 trytond_notification_email-6.6.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16138 2022-10-11 19:49:58.000000 trytond_notification_email-6.6.0/notification.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5799 2021-02-27 17:17:01.000000 trytond_notification_email-6.6.0/notification.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:15:07.677019 trytond_notification_email-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5255 2022-10-29 07:39:11.000000 trytond_notification_email-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:07.673685 trytond_notification_email-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_notification_email-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15373 2022-04-16 16:30:56.000000 trytond_notification_email-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2022-10-31 15:10:09.000000 trytond_notification_email-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      165 2022-10-31 16:15:04.000000 trytond_notification_email-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:07.677019 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2022-10-31 16:15:07.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1650 2022-10-31 16:15:07.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:15:07.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2022-10-31 16:15:07.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:42:54.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      139 2022-10-31 16:15:07.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:15:07.000000 trytond_notification_email-6.6.0/trytond_notification_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:15:07.677019 trytond_notification_email-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1080 2021-11-24 00:06:35.000000 trytond_notification_email-6.6.0/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2019-10-11 23:09:48.000000 trytond_notification_email-6.6.0/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      672 2020-08-11 20:00:44.000000 trytond_notification_email-6.6.0/view/log_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2020-08-11 20:00:44.000000 trytond_notification_email-6.6.0/view/log_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2019-06-04 16:49:46.000000 trytond_notification_email-6.6.0/view/trigger_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:48.664802 trytond_notification_email-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-05-01 11:03:15.000000 trytond_notification_email-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2023-05-01 11:03:15.000000 trytond_notification_email-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_notification_email-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2023-05-01 11:44:48.664802 trytond_notification_email-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:48.661469 trytond_notification_email-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3458 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1961 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:48.658135 trytond_notification_email-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5948 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5835 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5986 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4218 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4636 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5737 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5735 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4404 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5669 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5565 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5576 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5372 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5654 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4218 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5197 2023-04-30 10:46:36.000000 trytond_notification_email-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14056 2023-04-29 22:04:03.000000 trytond_notification_email-6.8.0/notification.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/notification.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:44:48.664802 trytond_notification_email-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4455 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:48.658135 trytond_notification_email-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15692 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      165 2023-05-01 11:03:10.000000 trytond_notification_email-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:48.664802 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2023-05-01 11:44:47.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-05-01 11:44:48.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:44:47.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2023-05-01 11:44:47.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-05-01 11:44:47.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:44:47.000000 trytond_notification_email-6.8.0/trytond_notification_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:44:48.661469 trytond_notification_email-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1080 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_notification_email-6.8.0/view/ir_email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:20.000000 trytond_notification_email-6.8.0/view/trigger_form.xml
```

### Comparing `trytond_notification_email-6.6.0/CHANGELOG` & `trytond_notification_email-6.8.0/CHANGELOG`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Merge email logs into email archives
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

### Comparing `trytond_notification_email-6.6.0/COPYRIGHT` & `trytond_notification_email-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2016-2022 Sergi Almacellas Abellana
-Copyright (C) 2017-2022 Cédric Krier
-Copyright (C) 2017-2022 B2CK
+Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2023 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_notification_email-6.6.0/LICENSE` & `trytond_notification_email-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_notification_email-6.6.0/PKG-INFO` & `trytond_notification_email-6.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_notification_email
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sending email notifications
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
-Project-URL: Source Code, https://hg.tryton.org/modules/notification_email
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton email notification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Bulgarian
@@ -36,21 +36,21 @@
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
 
 Notification Email Module
 #########################
 
 The notification email module allows to define email templates which will be
@@ -58,11 +58,11 @@
 Extra reports from the same record can be attached to the email.
 
 Configuration
 *************
 
 The notification_email module uses parameters from the section:
 
-- `[notification_email]`:
+- ``[notification_email]``:
 
-    - `from`: The default `From` for the email.
+    - ``from``: The default ``From`` for the email.
```

### Comparing `trytond_notification_email-6.6.0/ir.py` & `trytond_notification_email-6.8.0/ir.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+
+from sql import Table
+
+from trytond import backend
 from trytond.model import fields
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
+from trytond.transaction import Transaction
 
 
 class Trigger(metaclass=PoolMeta):
     __name__ = 'ir.trigger'
 
     notification_email = fields.Many2One(
         'notification.email', "Email Notification", readonly=True,
@@ -39,7 +44,55 @@
                         ('model', '=', self.notification_email.model),
                         ])
             except ValueError:
                 pass
             else:
                 self.model = trigger_model
             self.action = 'notification.email|trigger'
+
+
+class Email(metaclass=PoolMeta):
+    __name__ = 'ir.email'
+
+    notification_email = fields.Many2One(
+        'notification.email', "Notification Email", readonly=True,
+        states={
+            'invisible': ~Eval('notification_email'),
+            })
+    notification_trigger = fields.Many2One(
+        'ir.trigger', "Notification Trigger", readonly=True,
+        states={
+            'invisible': ~Eval('notification_trigger'),
+            })
+
+    @classmethod
+    def __register__(cls, module):
+        table = cls.__table__()
+        log = Table('notification_email_log')
+
+        cursor = Transaction().connection.cursor()
+
+        super().__register__(module)
+
+        # Migration from 6.6: merge notification email log with email
+        if backend.TableHandler.table_exist('notification_email_log'):
+            query = table.insert(
+                [table.create_uid, table.create_date,
+                    table.write_uid, table.write_date,
+                    table.recipients, table.recipients_secondary,
+                    table.recipients_hidden,
+                    table.resource,
+                    table.notification_email, table.notification_trigger],
+                log.select(
+                    log.create_uid, log.create_date,
+                    log.write_uid, log.write_date,
+                    log.recipients, log.recipients_secondary,
+                    log.recipients_hidden,
+                    log.resource,
+                    log.notification, log.trigger))
+            cursor.execute(*query)
+
+    def get_user(self, name):
+        user = super().get_user(name)
+        if self.notification_email or self.notification_trigger:
+            user = None
+        return user
```

### Comparing `trytond_notification_email-6.6.0/locale/bg.po` & `trytond_notification_email-6.8.0/locale/es_419.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr ""
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr ""
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notification Emails"
+msgstr ""
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
 msgstr ""
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
@@ -75,43 +82,14 @@
 msgid "Notification"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr ""
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr ""
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -162,50 +140,34 @@
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr ""
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification Emails"
+msgstr ""
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr ""
 
-#, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
 msgstr ""
```

### Comparing `trytond_notification_email-6.6.0/locale/ca.po` & `trytond_notification_email-6.8.0/locale/fr.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,220 +1,182 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "E-mail de notification"
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Déclencheur de notification"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr "Notificació per correu electrònic"
+msgstr "Notification par e-mail"
 
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notificacions per correu electrònic obligatòria"
+msgstr "E-mail de notification requis"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr "Adjunts"
+msgstr "Attachements"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr "Mitjà de contacte"
+msgstr "Moyen de contact"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr "Contingut"
+msgstr "Contenu"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr "Usuari enviament fallada destinataris"
+msgstr "Destinataire de secours"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr "Usuari enviament fallada destinataris ocults"
+msgstr "Destinataire caché de secours"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr "Usuari enviament fallada destinataris secundaris"
+msgstr "Destinataire secondaire de secours"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
 msgstr "De"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr "Model"
+msgstr "Modèle"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr "Destinataris"
+msgstr "Destinataires"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr "Destinataris ocults"
+msgstr "Destinataires cachés"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr "Destinataris secundaris"
+msgstr "Destinataires secondaires"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
-msgstr "Enviar després de"
+msgstr "Envoyer après"
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr "Asumpte"
+msgstr "Objet"
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr "Disparadors"
+msgstr "Déclencheurs"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr "Model"
+msgstr "Modèle"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr "Notificació"
+msgstr "Notification"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr "Informe"
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "Data"
-
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notificació"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr "Destinataris"
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr "Destinataris ocults"
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr "Destinataris secundaris"
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr "Recurs"
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr "Disparador"
+msgstr "Rapport"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr "El informes que s'utilitzaran com a adjunts."
+msgstr "Les rapports utilisés comme attachements."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
-msgstr ""
-"Defineix quin correu electrònic dels mitjans de contacte del tercer "
-"s'utilitzarà"
+msgstr "Définit quel e-mail utiliser des mécanismes de contact du tiers"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr "El informes utilitzat com a plantilla del correu electrònic."
+msgstr "Le rapport utilisé comme modèle d'e-mail."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
-msgstr ""
-"El usuari que es notificarà quan no es trobi un correu electrònic pels "
-"destinataris"
+msgstr "Utilisateur notifié quand l'e-mail du destinataire n'est pas trouvé"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
 msgstr ""
-"El usuari que es notificarà quan no es trobi un correu electrònic pels "
-"destinataris ocults"
+"Utilisateur notifié quand l'e-mail du destinataire caché ne peut être trouvé"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
-"El usuari que es notificarà quan no es trobi un correu electrònic pels "
-"destinataris secundaris"
+"Utilisateur notifié quand l'e-mail du destinataire secondaire ne peut être "
+"trouvé"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
-msgstr ""
-"Deixeu en blanc per a utilitzar el valor definit al fitxer de configuració."
+msgstr "Laissez vide pour la valeur définie dans le fichier de configuration."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr "El camp que conté el recipient(s)."
+msgstr "Le champ qui contient le(s) destinataire(s)."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr "El camp que conté el recipient(s) ocults."
+msgstr "Le champ qui contient le(s) destinataire(s) caché(s)."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr "El camp que conté el recipient(s) secundaris."
+msgstr "Le champ qui contient le(s) destinataire(s) secondaire(s)."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
-"El retard després del qual s'ha d'enviar el correu electrònic.\n"
-"S'aplica si la cua de treballs està activada."
+"Le délai après lequel l'e-mail doit être envoyé.\n"
+"Appliqué si une file de travail est activée."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
-"Es pot utilitzar la sintàxis Gensih amb 'record' al context d'evaluació.\n"
-"En blanc s'utiltizarà el nom de l'informe."
+"La syntaxe Genshi peut être utilisée avec « record » dans le contexte d'évaluation.\n"
+"S'il est vide, le nom du rapport sera utilisé."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr "Afegir un disparador per la notificació."
+msgstr "Ajouter un déclencheur pour la notification."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notificacions per correu electrònic"
+msgstr "E-mails de notification"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Registres"
-
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notificacions per correu electrònic"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr "E-mails"
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"El asumpte del correu electrónic de la notificació \"%(notification)s\" és "
-"invàlid amb l'excepció: \"%(exception)s\"."
+"Objet de l'e-mail non valide dans la notification « %(notification)s » avec "
+"l'exception « %(exception)s »."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notificacions per correu electrònic"
+msgstr "E-mails de notification"
 
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notificació per correu electrònic"
+msgstr "Notification par e-mail"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr "Adjunts notificacions per correu electrònic"
-
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Registre notificacions per correu electrònic"
+msgstr "Attachement d'e-mail de notification"
 
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notificació per correu electrònic"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "Hora"
+msgstr "Notification par e-mail"
```

### Comparing `trytond_notification_email-6.6.0/locale/cs.po` & `trytond_notification_email-6.8.0/locale/uk.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr ""
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr ""
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notification Emails"
+msgstr ""
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
 msgstr ""
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
@@ -75,43 +82,14 @@
 msgid "Notification"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr ""
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr ""
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -162,50 +140,34 @@
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr ""
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification Emails"
+msgstr ""
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr ""
 
-#, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
 msgstr ""
```

### Comparing `trytond_notification_email-6.6.0/locale/de.po` & `trytond_notification_email-6.8.0/locale/it.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,219 +1,188 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Email di notifica"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Notifica"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr "E-Mail-Benachrichtigung"
+msgstr "Notifica email"
 
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "E-Mail Benachrichtigung Erforderlich"
+msgstr "Email di notifica obbligatoria"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr "Anhänge"
+msgstr "Allegati"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr "Kontaktinformation"
+msgstr "Meccanismi di contatto"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr "Inhalt"
+msgstr "Contenuto"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr "Empfänger im Ausweichfall"
+msgstr "Utenti destinatari di ripiego"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr "Versteckte Emfänger im Ausweichfall"
+msgstr "Utenti destinatari di ripiego nascosti"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr "Sekundäre Empfänger im Ausweichfall"
+msgstr "Utenti destinatari secondari di ripiego"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr "Von"
+msgstr "Da"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr "Modell"
+msgstr "Modello"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr "Empfänger"
+msgstr "Destinatari"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr "Versteckte Empfänger"
+msgstr "Destinatari nascosti"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr "Sekundäre Empfänger"
+msgstr "Destinatari secondari"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
-msgstr "Versenden nach"
+msgstr "Invia dopo"
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr "Betreff"
+msgstr "Oggetto"
 
-# https://de.wikipedia.org/wiki/Datenbanktrigger
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
 msgstr "Trigger"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr "Modell"
+msgstr "Modello"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr "Benachrichtigung"
+msgstr "Notifica"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr "Bericht"
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "Datum"
-
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Benachrichtigung"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr "Empfänger"
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr "Versteckte Empfänger"
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr "Sekundäre Empfänger"
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr "Ressource"
-
-# https://de.wikipedia.org/wiki/Datenbanktrigger
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr "Trigger"
+msgstr "Segnala"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr "Der als Anhang genutzte Bericht."
+msgstr "I report utilizzati da usare come allegati."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
-msgstr "Auswahl der E-Mail-Adresse aus den Kontaktinformationen der Partei"
+msgstr ""
+"Definire quale e-mail utilizzare fra i meccanismi di contatto della "
+"controparte"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr "Der als E-Mail-Vorlage genutzte Bericht."
+msgstr "Il report utilizzato come template della E-mail."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
 msgstr ""
-"Zu benachrichtigender Benutzer wenn keine E-Mail-Adresse vorhanden ist"
+"Utente notificato quando nessun destinatario nella E-mail viene trovato"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
 msgstr ""
-"Zu benachrichtigender Benutzer wenn keine versteckte E-Mail-Adresse "
-"vorhanden ist"
+"Utente notificato quando nessun destinatario nascosto nella E-mail viene "
+"trovato"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
-"Zu benachrichtigender Benutzer wenn keine sekundäre E-Mail-Adresse vorhanden"
-" ist"
+"Utente notificato quando nessun destinatario secondario nella E-mail viene "
+"trovato"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
-msgstr "Leer lassen, um den Wert aus der Konfigurationsdatei zu verwenden."
+msgstr "Lasciare vuoto per il valore definito nel file di configurazione."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr "Das Feld das den/die Empfänger enthält."
+msgstr "Il campo che contiene il destinatario o i destinatari."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr "Das Feld das den/die versteckten Empfänger enthält."
+msgstr "Il campo che contiene i destinatari nascosti."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr "Das Feld das den/die sekundären Empfänger enthält."
+msgstr "Campo che contiene i destinatari secondari."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
-"Die Verzögerung nach der die E-Mail versandt werden soll.\n"
-"Wird nur angewendet wenn die Queue aktiviert ist."
+"Il ritardo dopo il quale l'e-mail deve essere inviata.\n"
+"Valido se viene attivata una coda di lavoro."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
-"Die Genshi Syntax kann mit 'record' im Evaluierungskontext verwendet werden.\n"
-"Sofern nicht angegeben wird die Bezeichnung des Datensatzes verwendet."
+"La sintassi di Genshi può essere utilizzata con il 'record' nel contesto di valutazione.\n"
+"Se vuoto verrà utilizzato il nome del rapporto."
 
-# https://de.wikipedia.org/wiki/Datenbanktrigger
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr "Einen Trigger für die Benachrichtigung hinzufügen."
+msgstr "Aggiungi un trigger per la notifica."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "E-Mail Benachrichtigungen"
+msgstr "Email di notifica"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "E-Mail Benachrichtigungen"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Ungültiger E-Mail-Betreff in Benachrichtigung \"%(notification)s\" mit "
-"Fehler \"%(exception)s\"."
+"Oggetto dell'e-mail non valido nella notifica \"%(notification)s\" con "
+"eccezione \"%(exception)s\"."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "E-Mail Benachrichtigungen"
+msgstr "Email di notifica"
 
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "E-Mail-Benachrichtigung"
+msgstr "Notifica Email"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr "Anhang für die E-Mail-Benachrichtigung"
-
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Log der E-Mail-Benachrichtigung"
+msgstr "Allegato E-mail di notifica"
 
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "E-Mail-Benachrichtigung"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "Zeit"
+msgstr "Notifica email"
```

### Comparing `trytond_notification_email-6.6.0/locale/es.po` & `trytond_notification_email-6.8.0/locale/es.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Notificacion por correo electrónico"
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Disparador notificación"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr "Notificación por correo electrónico"
 
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
 msgstr "Notificaciones por correo electrónico obligatoria"
@@ -74,42 +82,14 @@
 msgid "Notification"
 msgstr "Notificación"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr "Informe"
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "Fecha"
-
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notificación"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr "Destinatarios"
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr "Destinatarios ocultos"
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr "Destinatarios secundarios"
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr "Recurso"
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr "Disparador"
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr "Los informes que se van a utilizar como adjuntos."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -176,21 +156,17 @@
 msgid "Add a trigger for the notification."
 msgstr "Añade un disparador para la notificación."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
 msgstr "Notificaciones por correo electrónico"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Registros"
-
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notificaciones por correo electrónico"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr "Correos electrónicos"
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 "Asunto de correo electrónico inválido en la notificación "
@@ -204,18 +180,10 @@
 msgid "Email Notification"
 msgstr "Notificación por correo electrónico"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr "Adjuntos de notificaciones por correo electrónico"
 
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Registro de notificaciones por correo electrónico"
-
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
 msgstr "Notificación por correo electrónico"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "Hora"
```

### Comparing `trytond_notification_email-6.6.0/locale/es_419.po` & `trytond_notification_email-6.8.0/locale/pl.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,205 +1,184 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "E-maile z powiadomieniami"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Powiadomienie"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr ""
+msgstr "Powiadomienie e-mailowe"
 
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr ""
+msgstr "E-maile z powiadomieniami"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr ""
+msgstr "Załączniki"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr ""
+msgstr "Sposób kontaktu"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr ""
+msgstr "Treść"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr ""
+msgstr "Zastępczy użytkownik odbiorców"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr ""
+msgstr "Ukryty zastępczy użytkownik odbiorców"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr ""
+msgstr "Dodatkowy zastępczy użytkownik odbiorców"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr ""
+msgstr "Od"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "Odbiorcy"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Ukryci odbiorcy"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Dodatkowi odbiorcy"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
 msgstr ""
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "Temat"
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr ""
+msgstr "Wyzwalacze"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr ""
+msgstr "Powiadomienie"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr ""
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
+msgstr "Raport"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr ""
+msgstr "Raporty użyte jako załączniki."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
-msgstr ""
+msgstr "Określ, którego e-maila ze sposobów kontaktu użyć dla strony"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr ""
+msgstr "Raport użyty jako szablon wiadomości."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
 msgstr ""
+"Użytkownik zostanie powiadomiony, jeśli adres e-mail nie jest dostępny"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
 msgstr ""
+"Użytkownik zostanie powiadomiony, jeśli żaden ukryty adres e-mail nie jest "
+"dostępny"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
+"Użytkownik zostanie powiadomiony, jeśli żaden dodatkowy adres e-mail nie "
+"jest dostępny"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
-msgstr ""
+msgstr "Pozostaw puste dla wartości zdefiniowanej w pliku konfiguracyjnym."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr ""
+msgstr "Pole zawierające odbiorcę(ów)."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr ""
+msgstr "Pole zawierające ukrytego odbiorcę(ów)."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "Pole zawierające dodatkowego odbiorcę(ów)."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
+"Składnia Genshi może być używana z „rekordem” w kontekście oceny.\n"
+"Jeśli jest pusta, zostanie użyta nazwa raportu."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr ""
+msgstr "Dodaj wyzwalacz powiadomienia."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr ""
+msgstr "E-maile z powiadomieniami"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr ""
-
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"Nieprawidłowy temat wiadomości e-mail w powiadomieniu „% (notification) s” "
+"generujący wyjątek „% (exception) s”."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr ""
+msgstr "E-maile z powiadomieniami"
 
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr ""
+msgstr "E-mail z powiadomieniami"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr ""
-
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr ""
+msgstr "Załącznik z powiadomieniem e-mailowym"
 
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr ""
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
+msgstr "Powiadomienie e-mailowe"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_notification_email-6.6.0/locale/et.po` & `trytond_notification_email-6.8.0/locale/et.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "E-kirja teavitused"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Teavitus"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr "E-kirja teatis"
 
 #, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
@@ -75,43 +85,14 @@
 msgid "Notification"
 msgstr "Teavitus"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr "Aruanne"
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "Kuupäev"
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Teavitus"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr "Saajad"
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr "Peidetud saajad"
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr "Teised saajad"
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr "Aruanded, mida kasutatakse manusena."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -164,22 +145,17 @@
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
 msgstr "E-kirja teavitused"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logid"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "E-kirja teavitused"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
@@ -193,19 +169,10 @@
 msgstr "E-kirja teatis"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr "E-kirja teavituse manus"
 
 #, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Teavituskirja logi"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
 msgstr "E-kirja teatis"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "Aeg"
```

### Comparing `trytond_notification_email-6.6.0/locale/fa.po` & `trytond_notification_email-6.8.0/locale/fa.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "ایمیل‌های اطلاعیه"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "اطلاعیه"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr "ایمیل اطلاعیه"
 
 #, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
@@ -75,43 +85,14 @@
 msgid "Notification"
 msgstr "اطلاعیه"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr "گزارش"
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "تاریخ"
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "اطلاعیه"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr "گیرندگان"
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr "گیرنده گان پنهان"
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr "گیرندگان ثانویه"
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr "ماشه"
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr "استفاده از گزارش ها بعنوان پیوست ها."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -166,22 +147,17 @@
 msgid "Add a trigger for the notification."
 msgstr "یک ماشه برای اعلان اضافه کنید."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
 msgstr "ایمیل‌های اطلاعیه"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "گزارش ها"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "ایمیل‌های اطلاعیه"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
@@ -195,19 +171,10 @@
 msgstr "ایمیل اطلاعیه"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr "پیوست ایمیل اطلاعیه"
 
 #, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "گزارش ایمیل اطلاعیه"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
 msgstr "ایمیل اطلاعیه"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "زمان"
```

### Comparing `trytond_notification_email-6.6.0/locale/fi.po` & `trytond_notification_email-6.8.0/locale/zh_CN.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,211 +1,179 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "电子邮件通知"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "通知"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr ""
+msgstr "电子邮件通知"
 
 #, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notification Emails"
+msgstr "电子邮件通知"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr ""
+msgstr "附件"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr ""
+msgstr "联系方式"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr ""
+msgstr "内容"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr ""
+msgstr "收件人回退用户"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr ""
+msgstr "隐藏的收件人回退用户"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr ""
+msgstr "第二收件人回退用户"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr ""
+msgstr "发件人"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr ""
+msgstr "模型"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "收件人"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "隐藏的收件人"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "第二收件人"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
 msgstr ""
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "主题"
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr ""
+msgstr "触发器"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr ""
+msgstr "模型"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr ""
+msgstr "通知"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr ""
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
+msgstr "报告"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr ""
+msgstr "作为附件的报告."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
-msgstr ""
+msgstr "定义从参与者联系方式中使用哪个电子邮件"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr ""
+msgstr "作为电子邮件模板的报告."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
-msgstr ""
+msgstr "当找不到收件人电子邮件时通知用户"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
-msgstr ""
+msgstr "当找不到隐藏的收件人电子邮件时通知用户"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
-msgstr ""
+msgstr "当找不到第二收件人电子邮件时通知用户"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
-msgstr ""
+msgstr "配置文件中取值留空。"
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr ""
+msgstr "包含收件人的字段."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr ""
+msgstr "包含隐藏收件人的字段."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "包含次要收件人的字段."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
+"Genshi 语法可以与 'record' 一起使用.\n"
+"如果为空，则使用报告名称。"
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr ""
+msgstr "为通知添加触发器。"
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
-
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
+msgstr "电子邮件通知"
 
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
-msgstr ""
+msgstr "通知 \"%(notification)s\" 中电子邮件主题无效，异常为: \"%(exception)s\"."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr "电子邮件通知"
 
 #, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification Emails"
+msgstr "电子邮件通知"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr ""
-
-#, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
+msgstr "电子邮件通知附件"
 
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
+msgstr "电子邮件通知"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_notification_email-6.6.0/locale/fr.po` & `trytond_notification_email-6.8.0/locale/pt.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,214 +1,183 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Emails de Notificação"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Notificação"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr "Notification par e-mail"
+msgstr "Email de Notificação"
 
+#, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "E-mail de notification requis"
+msgstr "Emails de Notificação"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr "Attachements"
+msgstr "Anexos"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr "Moyen de contact"
+msgstr "Formas de Contato"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr "Contenu"
+msgstr "Conteúdo"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr "Destinataire de secours"
+msgstr "Usuário Substituto de Destinatários"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr "Destinataire caché de secours"
+msgstr "Usuário Substituto de Destinatários Ocultos"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr "Destinataire secondaire de secours"
+msgstr "Segundo Usuário Substituto de Destinatários Ocultos"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
 msgstr "De"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr "Modèle"
+msgstr "Modelo"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr "Destinataires"
+msgstr "Destinatários"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr "Destinataires cachés"
+msgstr "Destinatários Ocultos"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr "Destinataires secondaires"
+msgstr "Destinatários Secundários"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
-msgstr "Envoyer après"
+msgstr ""
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr "Objet"
+msgstr ""
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr "Déclencheurs"
+msgstr "Gatilhos"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr "Modèle"
+msgstr "Modelo"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr "Notification"
+msgstr "Notificação"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr "Rapport"
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "Date"
-
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr "Destinataires"
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr "Destinataires cachés"
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr "Destinataires secondaires"
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr "Ressource"
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr "Déclencheur"
+msgstr "Relatório"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr "Les rapports utilisés comme attachements."
+msgstr "Os relatórios usados como anexos."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
-msgstr "Définit quel e-mail utiliser des mécanismes de contact du tiers"
+msgstr "Escolha qual email da pessoa será usado"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr "Le rapport utilisé comme modèle d'e-mail."
+msgstr "O relatório utilizado como modelo para o email."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
-msgstr "Utilisateur notifié quand l'e-mail du destinataire n'est pas trouvé"
+msgstr ""
+"Usuário a ser notificado quando o email de nenhum destinatário for "
+"encontrado"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
 msgstr ""
-"Utilisateur notifié quand l'e-mail du destinataire caché ne peut être trouvé"
+"Usuário a ser notificado quando nenhum destinatário oculto for encontrado"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
-"Utilisateur notifié quand l'e-mail du destinataire secondaire ne peut être "
-"trouvé"
+"Usuário a ser notificado quando nenhum destinatário secundário for "
+"encontrado"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
-msgstr "Laissez vide pour la valeur définie dans le fichier de configuration."
+msgstr "Deixe vazio para usar o valor definido no arquivo de configuração."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr "Le champ qui contient le(s) destinataire(s)."
+msgstr "O campo que contém o(s) destinatário(s)."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr "Le champ qui contient le(s) destinataire(s) caché(s)."
+msgstr "O campo que contém o(s) destinatário(s) oculto(s)."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr "Le champ qui contient le(s) destinataire(s) secondaire(s)."
+msgstr "O campo que contém o(s) destinatário(s) secundário(s)."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
-"Le délai après lequel l'e-mail doit être envoyé.\n"
-"Appliqué si une file de travail est activée."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
-"La syntaxe Genshi peut être utilisée avec « record » dans le contexte d'évaluation.\n"
-"S'il est vide, le nom du rapport sera utilisé."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr "Ajouter un déclencheur pour la notification."
+msgstr "Adicionar um gatilho para a notificação."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "E-mails de notification"
+msgstr "Emails de Notificação"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Journaux"
-
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "E-mails de notification"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
-"Objet de l'e-mail non valide dans la notification « %(notification)s » avec "
-"l'exception « %(exception)s »."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "E-mails de notification"
+msgstr "Emails de Notificação"
 
+#, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification par e-mail"
+msgstr "Email de Notificação"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr "Attachement d'e-mail de notification"
-
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Journal d'e-mail de notification"
+msgstr "Anexo do Email de Notificação"
 
+#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification par e-mail"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "Heure"
+msgstr "Email de Notificação"
```

### Comparing `trytond_notification_email-6.6.0/locale/hu.po` & `trytond_notification_email-6.8.0/locale/id.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Pemberitahuan Email"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Pemberitahuan Email"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr ""
+msgstr "Pemberitahuan Email"
 
-#, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notification Emails"
+msgstr ""
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr ""
+msgstr "Lampiran-Lampiran"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
 msgstr ""
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr ""
+msgstr "Kandungan"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
 msgstr ""
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
@@ -33,23 +42,23 @@
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
 msgstr ""
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr ""
+msgstr "Dari"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "Penerima"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
 msgstr ""
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
@@ -65,52 +74,23 @@
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr ""
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
+msgstr "Laporan"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr ""
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
@@ -162,50 +142,36 @@
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
-
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
+msgstr ""
 
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification Emails"
+msgstr "Pemberitahuan Email"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr ""
 
 #, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
+msgstr "Pemberitahuan Email"
```

### Comparing `trytond_notification_email-6.6.0/locale/id.po` & `trytond_notification_email-6.8.0/locale/ca.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,188 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Notificació per correu electrònic"
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Disparador notificació"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr "Pemberitahuan Email"
+msgstr "Notificació per correu electrònic"
 
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr ""
+msgstr "Notificacions per correu electrònic obligatòria"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr "Lampiran-Lampiran"
+msgstr "Adjunts"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr ""
+msgstr "Mitjà de contacte"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr "Kandungan"
+msgstr "Contingut"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr ""
+msgstr "Usuari enviament fallada destinataris"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr ""
+msgstr "Usuari enviament fallada destinataris ocults"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr ""
+msgstr "Usuari enviament fallada destinataris secundaris"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr "Dari"
+msgstr "De"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr "Penerima"
+msgstr "Destinataris"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Destinataris ocults"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Destinataris secundaris"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
-msgstr ""
+msgstr "Enviar després de"
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "Asumpte"
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr ""
+msgstr "Disparadors"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr ""
+msgstr "Notificació"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr "Laporan"
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr "Tanggal"
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Pemberitahuan Email"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
+msgstr "Informe"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr ""
+msgstr "El informes que s'utilitzaran com a adjunts."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
+"Defineix quin correu electrònic dels mitjans de contacte del tercer "
+"s'utilitzarà"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr ""
+msgstr "El informes utilitzat com a plantilla del correu electrònic."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
 msgstr ""
+"El usuari que es notificarà quan no es trobi un correu electrònic pels "
+"destinataris"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
 msgstr ""
+"El usuari que es notificarà quan no es trobi un correu electrònic pels "
+"destinataris ocults"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
+"El usuari que es notificarà quan no es trobi un correu electrònic pels "
+"destinataris secundaris"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
 msgstr ""
+"Deixeu en blanc per a utilitzar el valor definit al fitxer de configuració."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr ""
+msgstr "El camp que conté el recipient(s)."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr ""
+msgstr "El camp que conté el recipient(s) ocults."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "El camp que conté el recipient(s) secundaris."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
+"El retard després del qual s'ha d'enviar el correu electrònic.\n"
+"S'aplica si la cua de treballs està activada."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
+"Es pot utilitzar la sintàxis Gensih amb 'record' al context d'evaluació.\n"
+"En blanc s'utiltizarà el nom de l'informe."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr ""
+msgstr "Afegir un disparador per la notificació."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr ""
-
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr ""
+msgstr "Notificacions per correu electrònic"
 
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Pemberitahuan Email"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr "Correus electrònics"
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"El asumpte del correu electrónic de la notificació \"%(notification)s\" és "
+"invàlid amb l'excepció: \"%(exception)s\"."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr ""
+msgstr "Notificacions per correu electrònic"
 
-#, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Pemberitahuan Email"
+msgstr "Notificació per correu electrònic"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr ""
+msgstr "Adjunts notificacions per correu electrònic"
 
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr ""
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Pemberitahuan Email"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr "Waktu"
+msgstr "Notificació per correu electrònic"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_notification_email-6.6.0/locale/lo.po` & `trytond_notification_email-6.8.0/locale/nl.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,211 +1,183 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "E-mailmeldingen"
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Melding Trigger"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr ""
+msgstr "E-mail notificatie"
 
-#, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notification Emails"
+msgstr "E-mailmelding vereist"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr ""
+msgstr "Bijlagen"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr ""
+msgstr "Contactmogelijkheid"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr ""
+msgstr "Inhoud"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr ""
+msgstr "Ontvanger in geval van nood"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr ""
+msgstr "Verborgen ontvangers in geval van nood"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr ""
+msgstr "Secundaire ontvanger in geval van nood"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr ""
+msgstr "Van"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "ontvangers"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Verborgen ontvangers"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Secundaire ontvangers"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
-msgstr ""
+msgstr "Verstuur over"
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "Onderwerp"
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr ""
+msgstr "triggers"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr ""
+msgstr "Kennisgeving"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr ""
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
+msgstr "Verslag"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr ""
+msgstr "De rapporten die als bijlagen worden gebruikt."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
+"Bepaal welke e-mail u wilt gebruiken van de contactmechanismen van de "
+"relatie"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr ""
+msgstr "Het rapport gebruikt als e-mailsjabloon."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
-msgstr ""
+msgstr "Te verwittigen gebruiker als er geen e-mail adres is"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
-msgstr ""
+msgstr "Gebruiker op de hoogte stellen als er geen verborgen e-mailadres is"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
+"Gebruiker wordt op de hoogte gesteld als er geen secundair e-mailadres is"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
 msgstr ""
+"Laat leeg voor de waarde die is gedefinieerd in het configuratiebestand."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr ""
+msgstr "Het veld dat de ontvanger (s) bevat."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr ""
+msgstr "Het veld dat de verborgen ontvanger (s) bevat."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "Het veld dat de secundaire ontvanger (s) bevat."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
+"De vertraging voordat de email verstuurd wordt\n"
+"Wordt toegepast wanneer workers geactiveerd zijn."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
+"De Genshi-syntaxis kan worden gebruikt met 'record' in de evaluatiecontext.\n"
+"Indien leeg wordt de rapportnaam gebruikt."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr ""
+msgstr "Voeg een trigger toe voor de melding."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr "E-mailmeldingen"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr "E-mails"
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"Ongeldig e-mailonderwerp in melding \"%(notification)s\" met uitzondering "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr "E-mailmeldingen"
 
-#, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification Emails"
+msgstr "E-mail notificatie"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr ""
+msgstr "Bijlage bij e-mailmelding"
 
-#, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
+msgstr "E-mail notificatie"
```

### Comparing `trytond_notification_email-6.6.0/locale/lt.po` & `trytond_notification_email-6.8.0/locale/ro.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,182 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Email pentru Notificări"
+
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Declanșator Notificare"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
-msgstr ""
+msgstr "Notificare Email"
 
-#, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
-msgstr "Notification Emails"
+msgstr "Notificare Email Obligatorie"
 
 msgctxt "field:notification.email,attachments:"
 msgid "Attachments"
-msgstr ""
+msgstr "Atașament"
 
 msgctxt "field:notification.email,contact_mechanism:"
 msgid "Contact Mechanism"
-msgstr ""
+msgstr "Mecanism de contact"
 
 msgctxt "field:notification.email,content:"
 msgid "Content"
-msgstr ""
+msgstr "Conţinut"
 
 msgctxt "field:notification.email,fallback_recipients:"
 msgid "Recipients Fallback User"
-msgstr ""
+msgstr "Destinatari Utilizator Alternativ"
 
 msgctxt "field:notification.email,fallback_recipients_hidden:"
 msgid "Hidden Recipients Fallback User"
-msgstr ""
+msgstr "Destinatari Ascunși Utilizator Alternativ"
 
 msgctxt "field:notification.email,fallback_recipients_secondary:"
 msgid "Secondary Recipients Fallback User"
-msgstr ""
+msgstr "Destinatari secundari Utilizator alternativ"
 
 msgctxt "field:notification.email,from_:"
 msgid "From"
-msgstr ""
+msgstr "Din"
 
 msgctxt "field:notification.email,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email,recipients:"
 msgid "Recipients"
-msgstr ""
+msgstr "Destinatari"
 
 msgctxt "field:notification.email,recipients_hidden:"
 msgid "Hidden Recipients"
-msgstr ""
+msgstr "Destinatari Ascunși"
 
 msgctxt "field:notification.email,recipients_secondary:"
 msgid "Secondary Recipients"
-msgstr ""
+msgstr "Destinatari Secundari"
 
 msgctxt "field:notification.email,send_after:"
 msgid "Send After"
-msgstr ""
+msgstr "Trimite După"
 
 msgctxt "field:notification.email,subject:"
 msgid "Subject"
-msgstr ""
+msgstr "Subiect"
 
 msgctxt "field:notification.email,triggers:"
 msgid "Triggers"
-msgstr ""
+msgstr "Declanșatoare"
 
 msgctxt "field:notification.email.attachment,model:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "field:notification.email.attachment,notification:"
 msgid "Notification"
-msgstr ""
+msgstr "Notificare"
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
-msgstr ""
-
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
+msgstr "Raport"
 
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
-msgstr ""
+msgstr "Rapoartele utilizate că atașamente."
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
-msgstr ""
+msgstr "Definire email de folosit din mecanismele de contact al parții"
 
 msgctxt "help:notification.email,content:"
 msgid "The report used as email template."
-msgstr ""
+msgstr "Raportul utilizat ca șablon pentru email."
 
 msgctxt "help:notification.email,fallback_recipients:"
 msgid "User notified when no recipients e-mail is found"
-msgstr ""
+msgstr "Utilizator notificat când nu se găsesc destinatari e-mail"
 
 msgctxt "help:notification.email,fallback_recipients_hidden:"
 msgid "User notified when no hidden recipients e-mail is found"
-msgstr ""
+msgstr "Utilizator notificat când nu sunt destinatari ascunși în e-mail"
 
 msgctxt "help:notification.email,fallback_recipients_secondary:"
 msgid "User notified when no secondary recipients e-mail is found"
 msgstr ""
+"Utilizatorul este notificat când nu este găsit niciun e-mail al "
+"destinatarilor secundari"
 
 msgctxt "help:notification.email,from_:"
 msgid "Leave empty for the value defined in the configuration file."
 msgstr ""
+"Lăsați necompletat pentru valoarea definită în fișierul de configurare."
 
 msgctxt "help:notification.email,recipients:"
 msgid "The field that contains the recipient(s)."
-msgstr ""
+msgstr "Câmpul care conține destinatarii."
 
 msgctxt "help:notification.email,recipients_hidden:"
 msgid "The field that contains the hidden recipient(s)."
-msgstr ""
+msgstr "Câmpul care conține destinatarii ascunși."
 
 msgctxt "help:notification.email,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "Câmpul care conține destinatarii secundari."
 
 msgctxt "help:notification.email,send_after:"
 msgid ""
 "The delay after which the email must be sent.\n"
 "Applied if a worker queue is activated."
 msgstr ""
+"Întârzierea după care trebuie trimis e-mailul.\n"
+"Se aplică dacă este activată o coadă de lucrători."
 
 msgctxt "help:notification.email,subject:"
 msgid ""
 "The Genshi syntax can be used with 'record' in the evaluation context.\n"
 "If empty the report name will be used."
 msgstr ""
+"Sintaxa Genshi poate fi folosită cu „înregistrare” în contextul evaluării.\n"
+"Dacă este gol, va fi folosit numele raportului."
 
 msgctxt "help:notification.email,triggers:"
 msgid "Add a trigger for the notification."
-msgstr ""
+msgstr "Adăugați un declanșator pentru notificare."
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr "E-mailuri de notificare"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr "E-mailuri"
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"Subiect invalid în e-mail notificare \"%(notification)s\" cu excepția "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "Notification Emails"
-msgstr "Notification Emails"
+msgstr "E-mailuri de notificare"
 
-#, fuzzy
 msgctxt "model:notification.email,name:"
 msgid "Email Notification"
-msgstr "Notification Emails"
+msgstr "Notificare Email"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
-msgstr ""
+msgstr "Atașament Email de Notificare"
 
-#, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
-msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
+msgstr "Notificare Email"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_notification_email-6.6.0/locale/ru.po` & `trytond_notification_email-6.8.0/locale/bg.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Notification Emails"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Notification Emails"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
@@ -75,43 +85,14 @@
 msgid "Notification"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr ""
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr ""
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -164,22 +145,17 @@
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
 msgstr "Notification Emails"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
@@ -193,19 +169,10 @@
 msgstr "Notification Emails"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr ""
 
 #, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
 msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
```

### Comparing `trytond_notification_email-6.6.0/locale/sl.po` & `trytond_notification_email-6.8.0/locale/cs.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Notification Emails"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Notification Emails"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
@@ -75,43 +85,14 @@
 msgid "Notification"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr ""
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr ""
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -164,22 +145,17 @@
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
 msgstr "Notification Emails"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
@@ -193,19 +169,10 @@
 msgstr "Notification Emails"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr ""
 
 #, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
 msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
```

### Comparing `trytond_notification_email-6.6.0/locale/tr.po` & `trytond_notification_email-6.8.0/locale/fi.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
+msgctxt "field:ir.email,notification_email:"
+msgid "Notification Email"
+msgstr "Notification Emails"
+
+#, fuzzy
+msgctxt "field:ir.email,notification_trigger:"
+msgid "Notification Trigger"
+msgstr "Notification Emails"
+
 msgctxt "field:ir.trigger,notification_email:"
 msgid "Email Notification"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:ir.trigger,notification_email_required:"
 msgid "Notification Email Required"
@@ -75,43 +85,14 @@
 msgid "Notification"
 msgstr ""
 
 msgctxt "field:notification.email.attachment,report:"
 msgid "Report"
 msgstr ""
 
-msgctxt "field:notification.email.log,date:"
-msgid "Date"
-msgstr ""
-
-#, fuzzy
-msgctxt "field:notification.email.log,notification:"
-msgid "Notification"
-msgstr "Notification Emails"
-
-msgctxt "field:notification.email.log,recipients:"
-msgid "Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_hidden:"
-msgid "Hidden Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,recipients_secondary:"
-msgid "Secondary Recipients"
-msgstr ""
-
-msgctxt "field:notification.email.log,resource:"
-msgid "Resource"
-msgstr ""
-
-msgctxt "field:notification.email.log,trigger:"
-msgid "Trigger"
-msgstr ""
-
 msgctxt "help:notification.email,attachments:"
 msgid "The reports used as attachments."
 msgstr ""
 
 msgctxt "help:notification.email,contact_mechanism:"
 msgid "Define which email to use from the party's contact mechanisms"
 msgstr ""
@@ -164,22 +145,17 @@
 msgid "Add a trigger for the notification."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_email_form"
 msgid "Notification Emails"
 msgstr "Notification Emails"
 
-msgctxt "model:ir.action,name:act_notification_email_log"
-msgid "Logs"
-msgstr "Logs"
-
-#, fuzzy
-msgctxt "model:ir.action,name:act_notification_email_log_relate"
-msgid "Notification E-Mails"
-msgstr "Notification Emails"
+msgctxt "model:ir.action,name:act_ir_email_form_relate_notification"
+msgid "E-mails"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_notification_invalid_subject"
 msgid ""
 "Invalid e-mail subject in notification \"%(notification)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
 
@@ -193,19 +169,10 @@
 msgstr "Notification Emails"
 
 msgctxt "model:notification.email.attachment,name:"
 msgid "Email Notification Attachment"
 msgstr ""
 
 #, fuzzy
-msgctxt "model:notification.email.log,name:"
-msgid "Notification Email Log"
-msgstr "Notification Emails"
-
-#, fuzzy
 msgctxt "selection:ir.trigger,action:"
 msgid "Email Notification"
 msgstr "Notification Emails"
-
-msgctxt "view:notification.email.log:"
-msgid "Time"
-msgstr ""
```

### Comparing `trytond_notification_email-6.6.0/notification.py` & `trytond_notification_email-6.8.0/notification.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,20 @@
 from email.header import Header
 from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
 from email.mime.nonmultipart import MIMENonMultipart
 from email.utils import formataddr, getaddresses, parseaddr
 
 from genshi.template import TextTemplate
-from sql import Null
-from sql.operators import Concat
 
 from trytond.config import config
 from trytond.i18n import gettext
-from trytond.ir.resource import ResourceAccessMixin
 from trytond.model import ModelSQL, ModelView, fields
 from trytond.pool import Pool
-from trytond.pyson import Eval
+from trytond.pyson import Eval, TimeDelta
 from trytond.report import get_email
 from trytond.sendmail import SMTPDataManager, sendmail_transactional
 from trytond.tools.email_ import set_from_header
 from trytond.transaction import Transaction
 
 from .exceptions import TemplateError
 
@@ -102,14 +99,18 @@
 
     triggers = fields.One2Many(
         'ir.trigger', 'notification_email', "Triggers",
         domain=[('model.model', '=', Eval('model'))],
         help="Add a trigger for the notification.")
     send_after = fields.TimeDelta(
         "Send After",
+        domain=['OR',
+            ('send_after', '=', None),
+            ('send_after', '>=', TimeDelta()),
+            ],
         help="The delay after which the email must be sent.\n"
         "Applied if a worker queue is activated.")
 
     model = fields.Function(
         fields.Char("Model"), 'on_change_with_model', searcher='search_model')
 
     @classmethod
@@ -194,25 +195,15 @@
             msg = content
 
         set_from_header(msg, sender, from_)
         msg['To'] = ', '.join(formataddr(parseaddr(a)) for a in to)
         msg['Cc'] = ', '.join(formataddr(parseaddr(a)) for a in cc)
         msg['Subject'] = Header(title, 'utf-8')
         msg['Auto-Submitted'] = 'auto-generated'
-        return msg
-
-    def get_log(self, record, trigger, msg, bcc=None):
-        return {
-            'recipients': msg['To'],
-            'recipients_secondary': msg['Cc'],
-            'recipients_hidden': bcc,
-            'resource': str(record),
-            'notification': trigger.notification_email.id,
-            'trigger': trigger.id,
-            }
+        return msg, title
 
     @classmethod
     def trigger(cls, records, trigger):
         "Action function for the triggers"
         notification_email = trigger.notification_email
         if not notification_email:
             raise ValueError(
@@ -232,85 +223,92 @@
         Trigger = pool.get('ir.trigger')
         records = Model.browse(ids)
         trigger = Trigger(trigger_id)
         self.send_email(records, trigger)
 
     def send_email(self, records, trigger):
         pool = Pool()
-        Log = pool.get('notification.email.log')
+        Email = pool.get('ir.email')
         datamanager = SMTPDataManager()
         Transaction().join(datamanager)
         from_ = (config.get('notification_email', 'from')
             or config.get('email', 'from'))
-        logs = []
+        emails = []
         for record in records:
             to, to_languages = self._get_to(record)
             cc, cc_languages = self._get_cc(record)
             bcc, bcc_languages = self._get_bcc(record)
-            languagues = to_languages | cc_languages | bcc_languages
+            languages = to_languages | cc_languages | bcc_languages
             to_addrs = [e for _, e in getaddresses(to + cc + bcc)]
             if to_addrs:
-                msg = self.get_email(record, from_, to, cc, bcc, languagues)
+                msg, title = self.get_email(
+                    record, from_, to, cc, bcc, languages)
                 sendmail_transactional(
                     from_, to_addrs, msg, datamanager=datamanager)
-                logs.append(self.get_log(
-                        record, trigger, msg, bcc=', '.join(bcc)))
-        if logs:
-            Log.create(logs)
+                emails.append(Email(
+                        recipients=', '.join(to),
+                        recipients_secondary=', '.join(cc),
+                        recipients_hidden=', '.join(bcc),
+                        addresses=[{'address': a} for a in to_addrs],
+                        subject=title,
+                        resource=record,
+                        notification_email=trigger.notification_email,
+                        notification_trigger=trigger))
+        Email.save(emails)
 
     def _get_recipients(self, record, name):
         if name == 'id':
             return record
         else:
             return getattr(record, name, None)
 
     def _get_to(self, record):
         to = []
-        languagues = set()
+        languages = set()
         if self.recipients:
             recipients = self._get_recipients(record, self.recipients.name)
             if recipients:
-                languagues.update(self._get_languages(recipients))
+                languages.update(self._get_languages(recipients))
                 to = self._get_addresses(recipients)
         if not to and self.fallback_recipients:
-            languagues.update(
+            languages.update(
                 self._get_languages(self.fallback_recipients))
             to = self._get_addresses(self.fallback_recipients)
-        return to, languagues
+        return to, languages
 
     def _get_cc(self, record):
         cc = []
-        languagues = set()
+        languages = set()
         if self.recipients_secondary:
             recipients_secondary = self._get_recipients(
                 record, self.recipients_secondary.name)
             if recipients_secondary:
-                languagues.update(
+                languages.update(
                     self._get_languages(recipients_secondary))
                 cc = self._get_addresses(recipients_secondary)
         if not cc and self.fallback_recipients_secondary:
-            languagues.update(
+            languages.update(
                 self._get_languages(self.fallback_recipients_secondary))
             cc = self._get_addresses(self.fallback_recipients_secondary)
-        return cc, languagues
+        return cc, languages
 
     def _get_bcc(self, record):
         bcc = []
-        languagues = set()
+        languages = set()
         if self.recipients_hidden:
             recipients_hidden = self._get_recipients(
                 record, self.recipients_hidden.name)
             if recipients_hidden:
-                languagues.update(self._get_languages(recipients_hidden))
+                languages.update(self._get_languages(recipients_hidden))
                 bcc = self._get_addresses(recipients_hidden)
         if not bcc and self.fallback_recipients_hidden:
-            languagues.update(
+            languages.update(
                 self._get_languages(self.fallback_recipients_hidden))
             bcc = self._get_addresses(self.fallback_recipients_hidden)
-        return bcc, languagues
+        return bcc, languages
 
     @classmethod
     def validate_fields(cls, notifications, field_names):
         super().validate_fields(notifications, field_names)
         cls.check_subject(notifications, field_names)
 
     @classmethod
@@ -368,70 +366,7 @@
             name = name.encode('utf-8')
         if not isinstance(language, str):
             language = language.encode('utf-8')
         msg.add_header(
             'Content-Disposition', 'attachment',
             filename=('utf-8', language, name))
         return msg
-
-
-class EmailLog(ResourceAccessMixin, ModelSQL, ModelView):
-    "Notification Email Log"
-    __name__ = 'notification.email.log'
-    date = fields.Function(fields.DateTime('Date'), 'get_date')
-    recipients = fields.Char("Recipients")
-    recipients_secondary = fields.Char("Secondary Recipients")
-    recipients_hidden = fields.Char("Hidden Recipients")
-    notification = fields.Many2One(
-        'notification.email', "Notification",
-        required=True, ondelete='RESTRICT')
-    trigger = fields.Many2One('ir.trigger', "Trigger")
-
-    @classmethod
-    def __setup__(cls):
-        super().__setup__()
-        cls._order = [
-            ('create_date', 'DESC'),
-            ('id', 'DESC'),
-            ]
-
-    @classmethod
-    def __register__(cls, module_name):
-        pool = Pool()
-        Model = pool.get('ir.model')
-        Trigger = pool.get('ir.trigger')
-        model = Model.__table__()
-        trigger = Trigger.__table__()
-        table = cls.__table__()
-        super().__register__(module_name)
-
-        table_h = cls.__table_handler__(module_name)
-        cursor = Transaction().connection.cursor()
-
-        # Migration from 5.6:
-        # fill notification and resource
-        # remove required on trigger
-        notification = trigger.select(
-            trigger.notification_email,
-            where=trigger.id == table.trigger)
-        resource = (trigger
-            .join(model, condition=trigger.model == model.id)
-            .select(
-                Concat(model.model, ',-1'),
-                where=trigger.id == table.trigger))
-        cursor.execute(*table.update(
-                [table.notification, table.resource],
-                [notification, resource],
-                where=(table.trigger != Null) & (table.resource == Null)))
-        table_h.not_null_action('trigger', 'remove')
-
-    def get_date(self, name):
-        return self.create_date.replace(microsecond=0)
-
-    @classmethod
-    def search_date(cls, name, clause):
-        return [('create_date',) + tuple(clause[1:])]
-
-    @staticmethod
-    def order_date(tables):
-        table, _ = tables[None]
-        return [table.create_date]
```

### Comparing `trytond_notification_email-6.6.0/setup.py` & `trytond_notification_email-6.8.0/setup.py`

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
@@ -34,65 +31,46 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_notification_email'
 
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
 
-requires = ['Genshi']
+requires = ['Genshi', 'python-sql']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('trytond_company'),
     get_require_version('trytond_commission'),
     get_require_version('trytond_party'),
     get_require_version('trytond_web_user'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for sending email notifications',
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
-        "Source Code": 'https://hg.tryton.org/modules/notification_email',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton email notification',
     package_dir={'trytond.modules.notification_email': '.'},
     packages=(
         ['trytond.modules.notification_email']
         + ['trytond.modules.notification_email.%s' % p
             for p in find_packages()]
@@ -128,27 +106,26 @@
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
     notification_email = trytond.modules.notification_email
     """,
     )
```

### Comparing `trytond_notification_email-6.6.0/tests/test_module.py` & `trytond_notification_email-6.8.0/tests/test_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,96 +87,101 @@
     def test_notification_email(self):
         "Test email notificiation is sent on trigger"
         pool = Pool()
         User = pool.get('res.user')
         Trigger = pool.get('ir.trigger')
         Model = pool.get('ir.model')
         NotificationEmail = pool.get('notification.email')
-        Log = pool.get('notification.email.log')
+        Email = pool.get('ir.email')
 
         self._setup_notification()
         notification_email, = NotificationEmail.search([])
 
         model, = Model.search([
                 ('model', '=', User.__name__),
                 ])
-        Trigger.create([{
+        trigger, = Trigger.create([{
                     'name': 'Test creation',
                     'model': model.id,
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
                 notification_module, 'sendmail_transactional') as sendmail, \
                 patch.object(notification_module, 'SMTPDataManager'):
-            User.create([{'name': "Michael Scott", 'login': "msc"}])
+            user, = User.create([{'name': "Michael Scott", 'login': "msc"}])
             self.run_tasks()
             sendmail.assert_called_once_with(
                 FROM, ['user@example.com'], ANY,
                 datamanager=ANY)
             _, _, msg = sendmail.call_args[0]
             self.assertEqual(msg['From'], FROM)
             self.assertEqual(msg['Subject'], 'Notification Email')
             self.assertEqual(msg['To'], 'Administrator <user@example.com>')
             self.assertEqual(msg['Auto-Submitted'], 'auto-generated')
             self.assertEqual(msg.get_content_type(), 'multipart/alternative')
             self.assertEqual(
                 msg.get_payload(0).get_payload(), 'Hello Michael Scott')
 
-        log, = Log.search([])
-        self.assertEqual(log.trigger.notification_email, notification_email)
-        self.assertEqual(log.recipients, 'Administrator <user@example.com>')
-        self.assertEqual(log.recipients_secondary, '')
-        self.assertEqual(log.recipients_hidden, '')
+        email, = Email.search([])
+        self.assertEqual(email.recipients, 'Administrator <user@example.com>')
+        self.assertEqual(email.recipients_secondary, '')
+        self.assertEqual(email.recipients_hidden, '')
+        self.assertEqual(email.subject, 'Notification Email')
+        self.assertEqual(email.resource, user)
+        self.assertEqual(email.notification_email, notification_email)
+        self.assertEqual(email.notification_trigger, trigger)
 
     @unittest.skipIf(
         (3, 5, 0) <= sys.version_info < (3, 5, 2), "python bug #25195")
     @with_transaction()
     def test_notification_email_id_recipient(self):
         "Test email notificiation is sent when using id as recipient"
         pool = Pool()
         User = pool.get('res.user')
         Trigger = pool.get('ir.trigger')
         Model = pool.get('ir.model')
         NotificationEmail = pool.get('notification.email')
-        Log = pool.get('notification.email.log')
+        Email = pool.get('ir.email')
 
         self._setup_notification(recipient_field='id')
         notification_email, = NotificationEmail.search([])
 
         model, = Model.search([
                 ('model', '=', User.__name__),
                 ])
-        Trigger.create([{
+        trigger, = Trigger.create([{
                     'name': 'Test creation',
                     'model': model.id,
                     'on_create': True,
                     'condition': 'true',
                     'notification_email': notification_email.id,
                     'action': 'notification.email|trigger',
                     }])
 
         with patch.object(
                 notification_module, 'sendmail_transactional') as sendmail, \
                 patch.object(notification_module, 'SMTPDataManager'):
-            User.create([{
+            user, = User.create([{
                         'name': "Michael Scott",
                         'login': "msc",
                         'email': 'msc@example.com'}])
             self.run_tasks()
             sendmail.assert_called_once_with(
                 FROM, ['msc@example.com'], ANY,
                 datamanager=ANY)
 
-        log, = Log.search([])
-        self.assertEqual(log.trigger.notification_email, notification_email)
-        self.assertEqual(log.recipients, 'Michael Scott <msc@example.com>')
+        email, = Email.search([])
+        self.assertEqual(email.recipients, 'Michael Scott <msc@example.com>')
+        self.assertEqual(email.resource, user)
+        self.assertEqual(email.notification_email, notification_email)
+        self.assertEqual(email.notification_trigger, trigger)
 
     @with_transaction()
     def test_notification_email_delay(self):
         "Test email notification is sent with delay"
         pool = Pool()
         User = pool.get('res.user')
         Trigger = pool.get('ir.trigger')
@@ -236,15 +241,15 @@
 
         notification_email, = NotificationEmail.search([])
         notification_email.attachments = [attachment]
         notification_email.save()
 
         user, = User.create([{'name': "Michael Scott", 'login': "msc"}])
 
-        msg = notification_email.get_email(
+        msg, title = notification_email.get_email(
             user, FROM, ['Administrator <user@example.com>'], [], [], [en])
 
         self.assertEqual(msg['From'], FROM)
         self.assertEqual(msg['Subject'], 'Notification Email')
         self.assertEqual(msg['To'], 'Administrator <user@example.com>')
         self.assertEqual(msg.get_content_type(), 'multipart/mixed')
         self.assertEqual(
@@ -276,15 +281,15 @@
 
         notification_email, = NotificationEmail.search([])
         notification_email.subject = 'Notification for ${record.name}'
         notification_email.save()
 
         user, = User.create([{'name': "Michael Scott", 'login': "msc"}])
 
-        msg = notification_email.get_email(
+        msg, title = notification_email.get_email(
             user, FROM, ['Administrator <user@example.com>'], [], [], [en])
 
         self.assertEqual(msg['Subject'], 'Notification for Michael Scott')
 
     @with_transaction()
     def test_notification_email_translated_subject(self):
         "Test email notificiation with translated subject"
@@ -312,15 +317,15 @@
 
         user, = User.create([{
                     'name': "Michael Scott",
                     'login': "msc",
                     'language': es.id,
                     }])
 
-        msg = notification_email.get_email(
+        msg, title = notification_email.get_email(
             user, FROM, ['Administrator <user@example.com>'], [], [], [es])
 
         self.assertEqual(msg['Subject'], 'Notificación para Michael Scott')
 
     @unittest.skipIf(
         (3, 5, 0) <= sys.version_info < (3, 5, 2), "python bug #25195")
     @with_transaction()
```

### Comparing `trytond_notification_email-6.6.0/trytond_notification_email.egg-info/PKG-INFO` & `trytond_notification_email-6.8.0/trytond_notification_email.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-notification-email
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module for sending email notifications
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
-Project-URL: Source Code, https://hg.tryton.org/modules/notification_email
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton email notification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Bulgarian
@@ -36,21 +36,21 @@
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
 
 Notification Email Module
 #########################
 
 The notification email module allows to define email templates which will be
@@ -58,11 +58,11 @@
 Extra reports from the same record can be attached to the email.
 
 Configuration
 *************
 
 The notification_email module uses parameters from the section:
 
-- `[notification_email]`:
+- ``[notification_email]``:
 
-    - `from`: The default `From` for the email.
+    - ``from``: The default ``From`` for the email.
```

### Comparing `trytond_notification_email-6.6.0/trytond_notification_email.egg-info/SOURCES.txt` & `trytond_notification_email-6.8.0/trytond_notification_email.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

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
@@ -49,17 +45,17 @@
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/test_module.py
 ./view/email_form.xml
 ./view/email_list.xml
-./view/log_form.xml
-./view/log_list.xml
+./view/ir_email_form.xml
 ./view/trigger_form.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
@@ -88,10 +84,9 @@
 trytond_notification_email.egg-info/dependency_links.txt
 trytond_notification_email.egg-info/entry_points.txt
 trytond_notification_email.egg-info/not-zip-safe
 trytond_notification_email.egg-info/requires.txt
 trytond_notification_email.egg-info/top_level.txt
 view/email_form.xml
 view/email_list.xml
-view/log_form.xml
-view/log_list.xml
+view/ir_email_form.xml
 view/trigger_form.xml
```

### Comparing `trytond_notification_email-6.6.0/view/email_form.xml` & `trytond_notification_email-6.8.0/view/email_form.xml`

 * *Files identical despite different names*

