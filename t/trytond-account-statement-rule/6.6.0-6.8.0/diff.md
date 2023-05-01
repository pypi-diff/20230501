# Comparing `tmp/trytond_account_statement_rule-6.6.0.tar.gz` & `tmp/trytond_account_statement_rule-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_rule-6.6.0.tar", last modified: Mon Oct 31 16:06:00 2022, max compression
+gzip compressed data, was "trytond_account_statement_rule-6.8.0.tar", last modified: Mon May  1 12:04:38 2023, max compression
```

## Comparing `trytond_account_statement_rule-6.6.0.tar` & `trytond_account_statement_rule-6.8.0.tar`

### file list

```diff
@@ -1,69 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:00.889068 trytond_account_statement_rule-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_statement_rule-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_statement_rule-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2022-10-31 16:05:59.000000 trytond_account_statement_rule-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_statement_rule-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)      731 2022-10-31 16:05:58.000000 trytond_account_statement_rule-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2022-10-31 16:05:58.000000 trytond_account_statement_rule-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:47.000000 trytond_account_statement_rule-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4067 2022-10-31 16:06:00.889068 trytond_account_statement_rule-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2021-12-11 16:59:32.000000 trytond_account_statement_rule-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14639 2022-04-10 15:40:34.000000 trytond_account_statement_rule-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5496 2021-06-17 19:21:18.000000 trytond_account_statement_rule-6.6.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:00.885735 trytond_account_statement_rule-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1805 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:00.885735 trytond_account_statement_rule-6.6.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5079 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5181 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4268 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5249 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4157 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4088 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2022-10-29 07:50:45.000000 trytond_account_statement_rule-6.6.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:06:00.889068 trytond_account_statement_rule-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5302 2022-10-29 07:39:10.000000 trytond_account_statement_rule-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:00.885735 trytond_account_statement_rule-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_statement_rule-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2678 2022-04-08 16:23:26.000000 trytond_account_statement_rule-6.6.0/tests/scenario_account_statement_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3937 2022-04-08 16:23:26.000000 trytond_account_statement_rule-6.6.0/tests/scenario_account_statement_rule_keyword_bank_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3481 2022-04-08 16:23:26.000000 trytond_account_statement_rule-6.6.0/tests/scenario_account_statement_rule_keywords.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2022-04-16 16:30:56.000000 trytond_account_statement_rule-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:53.000000 trytond_account_statement_rule-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2022-10-31 15:10:09.000000 trytond_account_statement_rule-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2022-10-31 16:05:57.000000 trytond_account_statement_rule-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:00.889068 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4067 2022-10-31 16:06:00.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2140 2022-10-31 16:06:00.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:06:00.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2022-10-31 16:06:00.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:14.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2022-10-31 16:06:00.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:06:00.000000 trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:06:00.885735 trytond_account_statement_rule-6.6.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      998 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1031 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/view/rule_information_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2019-10-11 23:09:47.000000 trytond_account_statement_rule-6.6.0/view/rule_information_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/view/rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2019-10-11 23:09:47.000000 trytond_account_statement_rule-6.6.0/view/rule_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2022-04-08 16:23:26.000000 trytond_account_statement_rule-6.6.0/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2019-06-04 16:49:46.000000 trytond_account_statement_rule-6.6.0/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:38.169563 trytond_account_statement_rule-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      894 2023-05-01 11:16:54.000000 trytond_account_statement_rule-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-05-01 11:16:54.000000 trytond_account_statement_rule-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4068 2023-05-01 12:04:38.169563 trytond_account_statement_rule-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15926 2023-04-30 10:46:36.000000 trytond_account_statement_rule-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5496 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:38.162897 trytond_account_statement_rule-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:38.156230 trytond_account_statement_rule-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5079 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5181 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4268 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5249 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4157 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4088 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2023-04-29 08:02:51.000000 trytond_account_statement_rule-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:04:38.169563 trytond_account_statement_rule-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4484 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:38.159563 trytond_account_statement_rule-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2660 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tests/scenario_account_statement_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3944 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tests/scenario_account_statement_rule_keyword_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3489 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tests/scenario_account_statement_rule_keywords.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-05-01 11:16:48.000000 trytond_account_statement_rule-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:38.166230 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4068 2023-05-01 12:04:37.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2114 2023-05-01 12:04:38.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:04:37.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-05-01 12:04:37.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-05-01 12:04:37.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:04:37.000000 trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:04:38.162897 trytond_account_statement_rule-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1031 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/rule_information_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/rule_information_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/rule_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_statement_rule-6.8.0/view/statement_tree.xml
```

### Comparing `trytond_account_statement_rule-6.6.0/CHANGELOG` & `trytond_account_statement_rule-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_account_statement_rule-6.6.0/COPYRIGHT` & `trytond_account_statement_rule-6.8.0/COPYRIGHT`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2018-2022 Cédric Krier
+Copyright (C) 2018-2023 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_statement_rule-6.6.0/LICENSE` & `trytond_account_statement_rule-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/PKG-INFO` & `trytond_account_statement_rule-6.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_rule
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to automate statement import with rules
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement_rule
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton statement import rule
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
 
 Account Statement Rule Module
 #############################
 
 The account_statement_rule module allows rules to be defined to complete
@@ -84,25 +84,25 @@
         * The matching value depending of the type of the key:
 
             * Boolean
             * Numeric: A range of value.
             * Char: A regular expression.
             * Selection
 
-The regular expression can register the group names `party`, `bank_account` and
-`invoice` which are later used to search for a party and an invoice.
+The regular expression can register the group names ``party``, ``bank_account``
+and ``invoice`` which are later used to search for a party and an invoice.
 
 Lines
 -----
 
 They define how to create the statement lines from the matching origin:
 
     * Amount: A Python expression evaluated with:
-        * `amount`: the amount of the origin.
-        * `pending`: the amount from which previous lines have been deducted.
+        * ``amount``: the amount of the origin.
+        * ``pending``: the amount from which previous lines have been deducted.
     * Party
     * Account
 
 If the party is not filled in, one will be searched for using the
-`bank_account` or the `party` group names from the regular expressions.
-If the `invoice` group name appears in a regular expression, it will be used to
-find an invoice to link with.
+``bank_account`` or the ``party`` group names from the regular expressions.
+If the ``invoice`` group name appears in a regular expression, it will be used
+to find an invoice to link with.
```

### Comparing `trytond_account_statement_rule-6.6.0/README.rst` & `trytond_account_statement_rule-6.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,25 +30,25 @@
         * The matching value depending of the type of the key:
 
             * Boolean
             * Numeric: A range of value.
             * Char: A regular expression.
             * Selection
 
-The regular expression can register the group names `party`, `bank_account` and
-`invoice` which are later used to search for a party and an invoice.
+The regular expression can register the group names ``party``, ``bank_account``
+and ``invoice`` which are later used to search for a party and an invoice.
 
 Lines
 -----
 
 They define how to create the statement lines from the matching origin:
 
     * Amount: A Python expression evaluated with:
-        * `amount`: the amount of the origin.
-        * `pending`: the amount from which previous lines have been deducted.
+        * ``amount``: the amount of the origin.
+        * ``pending``: the amount from which previous lines have been deducted.
     * Party
     * Account
 
 If the party is not filled in, one will be searched for using the
-`bank_account` or the `party` group names from the regular expressions.
-If the `invoice` group name appears in a regular expression, it will be used to
-find an invoice to link with.
+``bank_account`` or the ``party`` group names from the regular expressions.
+If the ``invoice`` group name appears in a regular expression, it will be used
+to find an invoice to link with.
```

### Comparing `trytond_account_statement_rule-6.6.0/__init__.py` & `trytond_account_statement_rule-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/account.py` & `trytond_account_statement_rule-6.8.0/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,16 +103,15 @@
 
     currency = fields.Function(fields.Many2One(
             'currency.currency', "Currency"),
         'on_change_with_currency')
 
     @fields.depends('journal')
     def on_change_with_currency(self, name=None):
-        if self.journal:
-            return self.journal.currency.id
+        return self.journal.currency if self.journal else None
 
     def match(self, origin):
         keywords = {}
         if self.company and self.company != origin.company:
             return False
         if self.journal and self.journal != origin.statement.journal:
             return False
@@ -309,37 +308,44 @@
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('rule')
 
     @fields.depends('rule', '_parent_rule.company')
     def on_change_with_company(self, name=None):
-        if self.rule and self.rule.company:
-            return self.rule.company.id
+        return self.rule.company if self.rule else None
 
     def get_line(self, origin, keywords, **context):
         pool = Pool()
         Line = pool.get('account.statement.line')
         context.setdefault('functions', {})['Decimal'] = Decimal
         context.setdefault('names', {}).update(keywords)
 
         currency = origin.statement.journal.currency
         amount = currency.round(simple_eval(decistmt(self.amount), **context))
         party = self._get_party(origin, keywords)
-        invoice = self._get_invoice(origin, keywords)
+        related_to = list(
+            filter(None, self._get_related_to(
+                    origin, keywords, party=party, amount=amount)))
+        if len(related_to) == 1:
+            related_to, = related_to
+        else:
+            related_to = None
+        related_to_party = self._get_party_from(related_to)
 
-        if invoice and party and invoice.party != party:
+        if related_to_party and party and related_to_party != party:
             return
-        if invoice and not party:
-            party = invoice.party
+        if related_to_party and not party:
+            party = related_to_party
 
         account = self.account
         if not account:
-            if invoice:
-                account = invoice.account
+            related_to_account = self._get_account_from(related_to)
+            if related_to_account:
+                account = related_to_account
             elif party:
                 with Transaction().set_context(date=origin.date):
                     if amount > Decimal('0.0'):
                         account = party.account_receivable_used
                     else:
                         account = party.account_payable_used
 
@@ -357,15 +363,15 @@
         line.number = origin.number
         line.description = origin.description
         line.origin = origin
         line.amount = amount
         line.date = origin.date
         line.party = party
         line.account = account
-        line.related_to = invoice
+        line.related_to = related_to
         return line
 
     def _get_party(self, origin, keywords):
         pool = Pool()
         Party = pool.get('party.party')
         Line = pool.get('account.statement.line')
         try:
@@ -409,15 +415,41 @@
                             ],
                         order=[('date', 'DESC')], limit=1)
                     if lines:
                         line, = lines
                         party = line.party
         return party
 
-    def _get_invoice(self, origin, keywords):
+    def _get_related_to(self, origin, keywords, party=None, amount=0):
+        return {self._get_invoice(origin, keywords, party=party)}
+
+    def _get_party_from(self, related_to):
+        pool = Pool()
+        Invoice = pool.get('account.invoice')
+        if isinstance(related_to, Invoice):
+            return related_to.party
+
+    def _get_account_from(self, related_to):
+        pool = Pool()
+        Invoice = pool.get('account.invoice')
+        if isinstance(related_to, Invoice):
+            return related_to.account
+
+    def _get_invoice(self, origin, keywords, party=None):
         pool = Pool()
         Invoice = pool.get('account.invoice')
         if keywords.get('invoice'):
-            invoices = Invoice.search([('rec_name', '=', keywords['invoice'])])
+            domain = [
+                ('rec_name', '=', keywords['invoice']),
+                ('company', '=', origin.company.id),
+                ('currency', '=', origin.currency.id),
+                ('state', '=', 'posted'),
+                ]
+            if party:
+                domain.append(['OR',
+                        ('party', '=', party.id),
+                        ('alternative_payees', '=', party.id),
+                        ])
+            invoices = Invoice.search(domain)
             if len(invoices) == 1:
                 invoice, = invoices
                 return invoice
```

### Comparing `trytond_account_statement_rule-6.6.0/account.xml` & `trytond_account_statement_rule-6.8.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/doc/index.rst` & `trytond_account_statement_rule-6.8.0/doc/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,25 +30,25 @@
         * The matching value depending of the type of the key:
 
             * Boolean
             * Numeric: A range of value.
             * Char: A regular expression.
             * Selection
 
-The regular expression can register the group names `party`, `bank_account` and
-`invoice` which are later used to search for a party and an invoice.
+The regular expression can register the group names ``party``, ``bank_account``
+and ``invoice`` which are later used to search for a party and an invoice.
 
 Lines
 -----
 
 They define how to create the statement lines from the matching origin:
 
     * Amount: A Python expression evaluated with:
-        * `amount`: the amount of the origin.
-        * `pending`: the amount from which previous lines have been deducted.
+        * ``amount``: the amount of the origin.
+        * ``pending``: the amount from which previous lines have been deducted.
     * Party
     * Account
 
 If the party is not filled in, one will be searched for using the
-`bank_account` or the `party` group names from the regular expressions.
-If the `invoice` group name appears in a regular expression, it will be used to
-find an invoice to link with.
+``bank_account`` or the ``party`` group names from the regular expressions.
+If the ``invoice`` group name appears in a regular expression, it will be used
+to find an invoice to link with.
```

### Comparing `trytond_account_statement_rule-6.6.0/locale/bg.po` & `trytond_account_statement_rule-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/ca.po` & `trytond_account_statement_rule-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/cs.po` & `trytond_account_statement_rule-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/de.po` & `trytond_account_statement_rule-6.8.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/es.po` & `trytond_account_statement_rule-6.8.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/es_419.po` & `trytond_account_statement_rule-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/et.po` & `trytond_account_statement_rule-6.8.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/fa.po` & `trytond_account_statement_rule-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/fi.po` & `trytond_account_statement_rule-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/fr.po` & `trytond_account_statement_rule-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/hu.po` & `trytond_account_statement_rule-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/id.po` & `trytond_account_statement_rule-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/it.po` & `trytond_account_statement_rule-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/lo.po` & `trytond_account_statement_rule-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/lt.po` & `trytond_account_statement_rule-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/nl.po` & `trytond_account_statement_rule-6.8.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/pl.po` & `trytond_account_statement_rule-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/pt.po` & `trytond_account_statement_rule-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/ro.po` & `trytond_account_statement_rule-6.8.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/ru.po` & `trytond_account_statement_rule-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/sl.po` & `trytond_account_statement_rule-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/tr.po` & `trytond_account_statement_rule-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/uk.po` & `trytond_account_statement_rule-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/locale/zh_CN.po` & `trytond_account_statement_rule-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/setup.py` & `trytond_account_statement_rule-6.8.0/setup.py`

 * *Files 25% similar despite different names*

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
@@ -34,63 +31,44 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_statement_rule'
 
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
 
 tests_require = [
     get_require_version('proteus'),
     get_require_version('trytond_bank'),
     ]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to automate statement import with rules',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_statement_rule',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton statement import rule',
     package_dir={'trytond.modules.account_statement_rule': '.'},
     packages=(
         ['trytond.modules.account_statement_rule']
         + ['trytond.modules.account_statement_rule.%s' % p
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
     account_statement_rule = trytond.modules.account_statement_rule
     """,
     )
```

### Comparing `trytond_account_statement_rule-6.6.0/tests/scenario_account_statement_rule.rst` & `trytond_account_statement_rule-6.8.0/tests/scenario_account_statement_rule.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ===============================
 Account Statement Rule Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> today = datetime.date.today()
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, get_accounts)
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_rule')
 
 Create company::
```

### Comparing `trytond_account_statement_rule-6.6.0/tests/scenario_account_statement_rule_keyword_bank_account.rst` & `trytond_account_statement_rule-6.8.0/tests/scenario_account_statement_rule_keyword_bank_account.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ====================================================
 Account Statement Rule Keyword Bank Account Scenario
 ====================================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> today = datetime.date.today()
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_statement_rule', 'bank'])
 
     >>> AccountJournal = Model.get('account.journal')
     >>> Bank = Model.get('bank')
@@ -32,15 +32,15 @@
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
```

### Comparing `trytond_account_statement_rule-6.6.0/tests/scenario_account_statement_rule_keywords.rst` & `trytond_account_statement_rule-6.8.0/tests/scenario_account_statement_rule_keywords.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 =======================================
 Account Statement Rule Keyword Scenario
 =======================================
 
 Imports::
 
-    >>> import datetime
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
     ...     create_fiscalyear, create_chart, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_statement_rule')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create fiscal year::
 
     >>> fiscalyear = set_fiscalyear_invoice_sequences(
-    ...     create_fiscalyear(company))
+    ...     create_fiscalyear(company, today))
     >>> fiscalyear.click('create_period')
 
 Create chart of accounts::
 
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
     >>> receivable = accounts['receivable']
```

### Comparing `trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/PKG-INFO` & `trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-account-statement-rule
-Version: 6.6.0
+Version: 6.8.0
 Summary: Tryton module to automate statement import with rules
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_statement_rule
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton statement import rule
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
 
 Account Statement Rule Module
 #############################
 
 The account_statement_rule module allows rules to be defined to complete
@@ -84,25 +84,25 @@
         * The matching value depending of the type of the key:
 
             * Boolean
             * Numeric: A range of value.
             * Char: A regular expression.
             * Selection
 
-The regular expression can register the group names `party`, `bank_account` and
-`invoice` which are later used to search for a party and an invoice.
+The regular expression can register the group names ``party``, ``bank_account``
+and ``invoice`` which are later used to search for a party and an invoice.
 
 Lines
 -----
 
 They define how to create the statement lines from the matching origin:
 
     * Amount: A Python expression evaluated with:
-        * `amount`: the amount of the origin.
-        * `pending`: the amount from which previous lines have been deducted.
+        * ``amount``: the amount of the origin.
+        * ``pending``: the amount from which previous lines have been deducted.
     * Party
     * Account
 
 If the party is not filled in, one will be searched for using the
-`bank_account` or the `party` group names from the regular expressions.
-If the `invoice` group name appears in a regular expression, it will be used to
-find an invoice to link with.
+``bank_account`` or the ``party`` group names from the regular expressions.
+If the ``invoice`` group name appears in a regular expression, it will be used
+to find an invoice to link with.
```

### Comparing `trytond_account_statement_rule-6.6.0/trytond_account_statement_rule.egg-info/SOURCES.txt` & `trytond_account_statement_rule-6.8.0/trytond_account_statement_rule.egg-info/SOURCES.txt`

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
 account.py
@@ -51,14 +47,15 @@
 ./view/rule_information_form.xml
 ./view/rule_information_list.xml
 ./view/rule_line_form.xml
 ./view/rule_line_list.xml
 ./view/rule_list.xml
 ./view/statement_form.xml
 ./view/statement_tree.xml
+doc/conf.py
 doc/index.rst
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
 locale/es_419.po
```

### Comparing `trytond_account_statement_rule-6.6.0/view/rule_form.xml` & `trytond_account_statement_rule-6.8.0/view/rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-6.6.0/view/rule_information_form.xml` & `trytond_account_statement_rule-6.8.0/view/rule_information_form.xml`

 * *Files identical despite different names*

