# Comparing `tmp/trytond_marketing_email-6.6.1.tar.gz` & `tmp/trytond_marketing_email-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_email-6.6.1.tar", last modified: Sat Apr  1 22:18:37 2023, max compression
+gzip compressed data, was "trytond_marketing_email-6.8.0.tar", last modified: Mon May  1 11:58:01 2023, max compression
```

## Comparing `trytond_marketing_email-6.6.1.tar` & `trytond_marketing_email-6.8.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.758808 trytond_marketing_email-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2023-04-01 22:18:33.000000 trytond_marketing_email-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-04-01 22:18:32.000000 trytond_marketing_email-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3628 2023-04-01 22:18:37.758808 trytond_marketing_email-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1430 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      729 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.748808 trytond_marketing_email-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1430 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1785 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/email_subscribe.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/email_unsubscribe.html
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/empty.gif
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.748808 trytond_marketing_email-6.6.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/icons/tryton-marketing-mail.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.742141 trytond_marketing_email-6.6.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6184 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6124 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6249 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6061 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5373 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5205 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18704 2023-03-18 10:58:52.000000 trytond_marketing_email-6.6.1/marketing.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10433 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      603 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:18:37.758808 trytond_marketing_email-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4347 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.742141 trytond_marketing_email-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5631 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2022-12-19 12:03:07.000000 trytond_marketing_email-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.755475 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3628 2023-04-01 22:18:36.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1955 2023-04-01 22:18:37.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:18:36.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-04-01 22:18:36.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:18:36.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-04-01 22:18:36.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:18:36.000000 trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:18:37.748808 trytond_marketing_email-6.6.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/email_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/email_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/email_message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/email_message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/view/send_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2022-12-19 12:02:49.000000 trytond_marketing_email-6.6.1/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.051302 trytond_marketing_email-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      660 2023-05-01 11:12:18.000000 trytond_marketing_email-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-05-01 11:12:17.000000 trytond_marketing_email-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3636 2023-05-01 11:58:01.051302 trytond_marketing_email-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.047969 trytond_marketing_email-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/email_subscribe.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/email_unsubscribe.html
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/empty.gif
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-29 22:04:03.000000 trytond_marketing_email-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.047969 trytond_marketing_email-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/icons/tryton-marketing-mail.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.041302 trytond_marketing_email-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6184 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6124 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6249 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6061 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5373 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5205 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18644 2023-04-29 22:04:03.000000 trytond_marketing_email-6.8.0/marketing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10433 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      603 2023-04-29 22:04:03.000000 trytond_marketing_email-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:01.051302 trytond_marketing_email-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4311 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.041302 trytond_marketing_email-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5610 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 11:12:12.000000 trytond_marketing_email-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.047969 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3636 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1955 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.044635 trytond_marketing_email-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-28 07:46:16.000000 trytond_marketing_email-6.8.0/view/email_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/send_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/web.py
```

### Comparing `trytond_marketing_email-6.6.1/CHANGELOG` & `trytond_marketing_email-6.8.0/CHANGELOG`

 * *Files 25% similar despite different names*

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
 * Count subscribed emails per list
 
 Version 6.4.0 - 2022-05-02
```

### Comparing `trytond_marketing_email-6.6.1/COPYRIGHT` & `trytond_marketing_email-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/LICENSE` & `trytond_marketing_email-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/PKG-INFO` & `trytond_marketing_email-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_email
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to manage marketing mailing lists
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
-Project-URL: Source Code, https://hg.tryton.org/modules/marketing_email
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing email list
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
 Provides-Extra: test
 License-File: LICENSE
 
 Marketing Email Module
 ######################
 
 The marketing_email module manages mailing lists.
@@ -95,18 +95,18 @@
 list for test purposes.
 
 Configuration
 *************
 
 The marketing_email module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the e-mails that get sent.
+    - ``email_from``: The default ``From`` for the e-mails that get sent.
 
-    - `email_subscribe_url`: the URL to confirm the subscription to which the
-      parameter `token` will be added.
+    - ``email_subscribe_url``: the URL to confirm the subscription to which the
+      parameter ``token`` will be added.
 
-    - `email_unsubscribe_url`: the URL to unsubscribe an e-mail address to
-      which the parameter `token` will be added.
+    - ``email_unsubscribe_url``: the URL to unsubscribe an e-mail address to
+      which the parameter ``token`` will be added.
 
-    - `email_spy_pixel`: A boolean to activate spy pixel. Disable by default.
+    - ``email_spy_pixel``: A boolean to activate spy pixel. Disable by default.
```

### Comparing `trytond_marketing_email-6.6.1/README.rst` & `trytond_marketing_email-6.8.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 list for test purposes.
 
 Configuration
 *************
 
 The marketing_email module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the e-mails that get sent.
+    - ``email_from``: The default ``From`` for the e-mails that get sent.
 
-    - `email_subscribe_url`: the URL to confirm the subscription to which the
-      parameter `token` will be added.
+    - ``email_subscribe_url``: the URL to confirm the subscription to which the
+      parameter ``token`` will be added.
 
-    - `email_unsubscribe_url`: the URL to unsubscribe an e-mail address to
-      which the parameter `token` will be added.
+    - ``email_unsubscribe_url``: the URL to unsubscribe an e-mail address to
+      which the parameter ``token`` will be added.
 
-    - `email_spy_pixel`: A boolean to activate spy pixel. Disable by default.
+    - ``email_spy_pixel``: A boolean to activate spy pixel. Disable by default.
```

### Comparing `trytond_marketing_email-6.6.1/__init__.py` & `trytond_marketing_email-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/doc/conf.py` & `trytond_marketing_email-6.8.0/doc/conf.py`

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

### Comparing `trytond_marketing_email-6.6.1/doc/index.rst` & `trytond_marketing_email-6.8.0/doc/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 list for test purposes.
 
 Configuration
 *************
 
 The marketing_email module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the e-mails that get sent.
+    - ``email_from``: The default ``From`` for the e-mails that get sent.
 
-    - `email_subscribe_url`: the URL to confirm the subscription to which the
-      parameter `token` will be added.
+    - ``email_subscribe_url``: the URL to confirm the subscription to which the
+      parameter ``token`` will be added.
 
-    - `email_unsubscribe_url`: the URL to unsubscribe an e-mail address to
-      which the parameter `token` will be added.
+    - ``email_unsubscribe_url``: the URL to unsubscribe an e-mail address to
+      which the parameter ``token`` will be added.
 
-    - `email_spy_pixel`: A boolean to activate spy pixel. Disable by default.
+    - ``email_spy_pixel``: A boolean to activate spy pixel. Disable by default.
```

### Comparing `trytond_marketing_email-6.6.1/email_subscribe.html` & `trytond_marketing_email-6.8.0/email_subscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/email_unsubscribe.html` & `trytond_marketing_email-6.8.0/email_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/icons/LICENSE` & `trytond_marketing_email-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/bg.po` & `trytond_marketing_email-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/ca.po` & `trytond_marketing_email-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/cs.po` & `trytond_marketing_email-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/de.po` & `trytond_marketing_email-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/es.po` & `trytond_marketing_email-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/es_419.po` & `trytond_marketing_email-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/et.po` & `trytond_marketing_email-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/fa.po` & `trytond_marketing_email-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/fi.po` & `trytond_marketing_email-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/fr.po` & `trytond_marketing_email-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/hu.po` & `trytond_marketing_email-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/id.po` & `trytond_marketing_email-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/it.po` & `trytond_marketing_email-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/lo.po` & `trytond_marketing_email-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/lt.po` & `trytond_marketing_email-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/nl.po` & `trytond_marketing_email-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/pl.po` & `trytond_marketing_email-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/pt.po` & `trytond_marketing_email-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/ro.po` & `trytond_marketing_email-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/ru.po` & `trytond_marketing_email-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/sl.po` & `trytond_marketing_email-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/tr.po` & `trytond_marketing_email-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/uk.po` & `trytond_marketing_email-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/locale/zh_CN.po` & `trytond_marketing_email-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/marketing.py` & `trytond_marketing_email-6.8.0/marketing.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     DeactivableMixin, Index, ModelSQL, ModelView, Unique, Workflow, fields)
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.report import Report, get_email
 from trytond.sendmail import SMTPDataManager, sendmail_transactional
 from trytond.tools import grouped_slice, reduce_ids
 from trytond.tools.email_ import set_from_header
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 from trytond.url import http_host
 from trytond.wizard import Button, StateTransition, StateView, Wizard
 
 from .exceptions import TemplateError
 
 if not config.get(
         'html', 'plugins-marketing.email.message-content'):
@@ -166,15 +166,15 @@
         return cls.subscribe(list(tokens))
 
     @classmethod
     def subscribe(cls, tokens):
         # Make it slow to prevent brute force attacks
         delay = config.getint('marketing', 'subscribe_delay', default=1)
         Transaction().atexit(time.sleep, delay)
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             records = cls.search([
                     ('email_token', 'in', tokens),
                     ])
         cls.write(records, {'active': True})
         return bool(records)
 
     def get_email_unsubscribe(self, report_name='marketing.email.unsubscribe'):
@@ -276,15 +276,15 @@
         Email = pool.get('marketing.email')
 
         # Randomize processing time to prevent guessing whether the email
         # address is already subscribed to the list or not.
         Transaction().atexit(time.sleep, random.random())
 
         email = email.lower()
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             records = Email.search([
                     ('email', '=', email),
                     ('list_', '=', self.id),
                     ])
         if not records:
             record = Email(email=email, list_=self.id, active=False)
             record.save()
@@ -304,15 +304,15 @@
         Email = pool.get('marketing.email')
 
         # Randomize processing time to prevent guessing whether the email
         # address was subscribed to the list or not.
         Transaction().atexit(time.sleep, random.random())
 
         email = email.lower()
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             records = Email.search([
                     ('email', '=', email),
                     ('list_', '=', self.id),
                     ])
         if records:
             record, = records
             if record.active:
```

### Comparing `trytond_marketing_email-6.6.1/marketing.xml` & `trytond_marketing_email-6.8.0/marketing.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/message.xml` & `trytond_marketing_email-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/setup.py` & `trytond_marketing_email-6.8.0/setup.py`

 * *Files 2% similar despite different names*

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
 name = 'trytond_marketing_email'
 
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
     description='Tryton module to manage marketing mailing lists',
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
-        "Source Code": 'https://hg.tryton.org/modules/marketing_email',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton marketing email list',
     package_dir={'trytond.modules.marketing_email': '.'},
     packages=(
         ['trytond.modules.marketing_email']
         + ['trytond.modules.marketing_email.%s' % p for p in find_packages()]
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
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
     [trytond.modules]
```

### Comparing `trytond_marketing_email-6.6.1/tests/test_module.py` & `trytond_marketing_email-6.8.0/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from unittest.mock import ANY, Mock, patch
 
 from trytond.config import config
 from trytond.modules.marketing_email import marketing as marketing_module
 from trytond.pool import Pool
 from trytond.tests.test_tryton import ModuleTestCase, with_transaction
-from trytond.transaction import Transaction
+from trytond.transaction import inactive_records
 
 SUBSCRIBE_URL = 'http://www.example.com/subscribe'
 UNSUBSCRIBE_URL = 'http://www.example.com/unsubscribe'
 FROM = 'marketing@example.com'
 
 
 class MarketingEmailTestCase(ModuleTestCase):
@@ -53,15 +53,15 @@
         email_list.save()
 
         with patch.object(
                 marketing_module, 'sendmail_transactional') as sendmail:
             email_list.request_subscribe('user@example.com')
             sendmail.assert_called_once_with(FROM, ['user@example.com'], ANY)
 
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             email, = Email.search([
                     ('list_', '=', email_list.id),
                     ])
         token = email.email_token
         self.assertTrue(token)
         self.assertFalse(email.active)
         self.assertEqual(email_list.subscribed, 0)
```

### Comparing `trytond_marketing_email-6.6.1/tox.ini` & `trytond_marketing_email-6.8.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 extras = test
 commands =
-    coverage run --include=./**/marketing_email/* -m unittest discover -s tests
-    coverage report --include=./**/marketing_email/* --omit=*/tests/*
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

### Comparing `trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/PKG-INFO` & `trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-marketing-email
-Version: 6.6.1
+Version: 6.8.0
 Summary: Tryton module to manage marketing mailing lists
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
-Project-URL: Source Code, https://hg.tryton.org/modules/marketing_email
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton marketing email list
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
 Provides-Extra: test
 License-File: LICENSE
 
 Marketing Email Module
 ######################
 
 The marketing_email module manages mailing lists.
@@ -95,18 +95,18 @@
 list for test purposes.
 
 Configuration
 *************
 
 The marketing_email module uses parameters from the section:
 
-- `[marketing]`:
+- ``[marketing]``:
 
-    - `email_from`: The default `From` for the e-mails that get sent.
+    - ``email_from``: The default ``From`` for the e-mails that get sent.
 
-    - `email_subscribe_url`: the URL to confirm the subscription to which the
-      parameter `token` will be added.
+    - ``email_subscribe_url``: the URL to confirm the subscription to which the
+      parameter ``token`` will be added.
 
-    - `email_unsubscribe_url`: the URL to unsubscribe an e-mail address to
-      which the parameter `token` will be added.
+    - ``email_unsubscribe_url``: the URL to unsubscribe an e-mail address to
+      which the parameter ``token`` will be added.
 
-    - `email_spy_pixel`: A boolean to activate spy pixel. Disable by default.
+    - ``email_spy_pixel``: A boolean to activate spy pixel. Disable by default.
```

### Comparing `trytond_marketing_email-6.6.1/trytond_marketing_email.egg-info/SOURCES.txt` & `trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.6.1/view/email_message_form.xml` & `trytond_marketing_email-6.8.0/view/email_message_form.xml`

 * *Files identical despite different names*

