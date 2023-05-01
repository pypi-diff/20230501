# Comparing `tmp/scrapyd-1.4.1.tar.gz` & `tmp/scrapyd-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapyd-1.4.1.tar", last modified: Fri Feb 10 07:10:03 2023, max compression
+gzip compressed data, was "scrapyd-1.4.2.tar", last modified: Mon May  1 20:19:38 2023, max compression
```

## Comparing `scrapyd-1.4.1.tar` & `scrapyd-1.4.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.245941 scrapyd-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-10 07:09:57.000000 scrapyd-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-10 07:09:57.000000 scrapyd-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-10 07:10:03.245941 scrapyd-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-10 07:09:57.000000 scrapyd-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.241941 scrapyd-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/news.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-10 07:09:57.000000 scrapyd-1.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.241941 scrapyd-1.4.1/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-10 07:09:57.000000 scrapyd-1.4.1/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-10 07:09:57.000000 scrapyd-1.4.1/integration_tests/test_webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-10 07:09:57.000000 scrapyd-1.4.1/integration_tests/test_website.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.241941 scrapyd-1.4.1/scrapyd/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/basicauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/default_scrapyd.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/eggstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/eggutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/jobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.245941 scrapyd-1.4.1/scrapyd/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/scripts/scrapyd_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/spiderqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.245941 scrapyd-1.4.1/scrapyd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/logstdout.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/mockserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/mybot.egg
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/mybot2.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/mybot3.egg
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/mybotunicode.egg
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/quotesbot.egg
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/quotesbot_asyncio.egg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/start_mock_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_dont_load_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_eggstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_jobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_spiderqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/tests/test_website.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/txapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-02-10 07:09:57.000000 scrapyd-1.4.1/scrapyd/website.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 07:10:03.245941 scrapyd-1.4.1/scrapyd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-10 07:10:03.000000 scrapyd-1.4.1/scrapyd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-10 07:10:03.249940 scrapyd-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-02-10 07:09:57.000000 scrapyd-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.398414 scrapyd-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 20:19:34.000000 scrapyd-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-01 20:19:34.000000 scrapyd-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-01 20:19:38.398414 scrapyd-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-01 20:19:34.000000 scrapyd-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.390413 scrapyd-1.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 20:19:34.000000 scrapyd-1.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.390413 scrapyd-1.4.2/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 20:19:34.000000 scrapyd-1.4.2/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 20:19:34.000000 scrapyd-1.4.2/integration_tests/test_webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 20:19:34.000000 scrapyd-1.4.2/integration_tests/test_website.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.394414 scrapyd-1.4.2/scrapyd/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/basicauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/default_scrapyd.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/eggstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/eggutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/jobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.394414 scrapyd-1.4.2/scrapyd/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/scripts/scrapyd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/spiderqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.398414 scrapyd-1.4.2/scrapyd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/logstdout.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/mybot.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/mybot2.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/mybot3.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/mybotunicode.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/quotesbot.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/quotesbot_asyncio.egg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/start_mock_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_dont_load_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_eggstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_jobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_spiderqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/tests/test_website.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/txapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-01 20:19:34.000000 scrapyd-1.4.2/scrapyd/website.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:19:38.394414 scrapyd-1.4.2/scrapyd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 20:19:38.000000 scrapyd-1.4.2/scrapyd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-01 20:19:38.398414 scrapyd-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-01 20:19:34.000000 scrapyd-1.4.2/setup.py
```

### Comparing `scrapyd-1.4.1/LICENSE` & `scrapyd-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/PKG-INFO` & `scrapyd-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapyd
-Version: 1.4.1
+Version: 1.4.2
 Summary: A service for running Scrapy spiders, with an HTTP API
 Home-page: https://github.com/scrapy/scrapyd
 Author: Scrapy developers
 Author-email: info@scrapy.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrapyd-1.4.1/README.rst` & `scrapyd-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/docs/Makefile` & `scrapyd-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/docs/api.rst` & `scrapyd-1.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/docs/conf.py` & `scrapyd-1.4.2/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,25 +18,27 @@
 # -- Project information -----------------------------------------------------
 
 project = "Scrapyd"
 copyright = "2013-2022, Scrapy group"
 author = "Scrapy group"
 
 # The short X.Y version
-version = "1.4.1"
+version = "1.4.2"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = []
+extensions = [
+    "sphinx.ext.extlinks",
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -50,7 +52,15 @@
 #
 html_theme = "furo"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = []
+
+
+# -- Extension configuration -------------------------------------------------
+
+extlinks = {
+    "issue": ("https://github.com/open-contracting/pelican-frontend/issues/%s", "#%s"),
+    "commit": ("https://github.com/open-contracting/pelican-frontend/commit/%s", "%s"),
+}
```

### Comparing `scrapyd-1.4.1/docs/config.rst` & `scrapyd-1.4.2/docs/config.rst`

 * *Files 23% similar despite different names*

```diff
@@ -60,45 +60,72 @@
 debug
 -----
 
 Whether debug mode is enabled. Defaults to ``off``. When debug mode is enabled
 the full Python traceback will be returned (as plain text responses) when there
 is an error processing a JSON API call.
 
+.. _eggs_dir:
+
 eggs_dir
 --------
 
 The directory where the project eggs will be stored.
 
+.. seealso::
+
+   :ref:`eggstorage`
+
 dbs_dir
 -------
 
 The directory where the project databases will be stored (this includes the
 spider queues).
 
 logs_dir
 --------
 
-The directory where the Scrapy logs will be stored. If you want to disable
-storing logs set this option empty, like this::
+The directory where the Scrapy logs will be stored.
+
+To disable log storage, set this option to empty:
+
+.. code-block:: ini
+
+   logs_dir =
+
+To log messages to a remote service, you can, for example, reconfigure Scrapy's logger from your Scrapy project:
 
-    logs_dir =
+.. code-block:: python
+
+   import logging
+   import logstash
+
+   logger = logging.getLogger("scrapy")
+   logger.handlers.clear()
+   logger.addHandler(logstash.LogstashHandler("https://user:pass@id.us-east-1.aws.found.io", 5959, version=1))
 
 .. _items_dir:
 
 items_dir
 ---------
 
 .. versionadded:: 0.15
 
 The directory where the Scrapy items will be stored.
-This option is disabled by default
-because you are expected to use a database or a feed exporter.
-Setting it to non-empty results in storing scraped item feeds
-to the specified directory by overriding the scrapy setting ``FEEDS``.
+
+This option is disabled by default. It is recommended to either:
+
+-  Use `feed exports <https://docs.scrapy.org/en/latest/topics/feed-exports.html>`__, by setting the ``FEEDS`` Scrapy setting in your Scrapy project. See the full list of `storage backends <https://docs.scrapy.org/en/latest/topics/feed-exports.html#storages>`__.
+-  Use the `item pipeline <https://docs.scrapy.org/en/latest/topics/item-pipeline.html>`__, to store the scraped items in a database. See the `MongoDB example <https://docs.scrapy.org/en/latest/topics/item-pipeline.html#write-items-to-mongodb>`__, which can be adapted to another database.
+
+If this option is non-empty, the `FEEDS <https://docs.scrapy.org/en/latest/topics/feed-exports.html#std-setting-FEEDS>`__ Scrapy setting is set as follows, resulting in feeds being stored in the specified directory as JSON lines.
+
+.. code-block:: json
+
+   {"value from items_dir": {"format": "jsonlines"}}
 
 .. _jobs_to_keep:
 
 jobs_to_keep
 ------------
 
 .. versionadded:: 0.15
@@ -123,14 +150,26 @@
 poll_interval
 -------------
 
 The interval used to poll queues, in seconds.
 Defaults to ``5.0``.
 Can be a float, such as ``0.2``
 
+.. _prefix_header:
+
+prefix_header
+-------------
+
+.. versionadded:: 1.4.2
+
+The header for the base path of the original request.
+A base path must have a leading slash and no trailing slash, e.g. ``/base/path``.
+The header is relevant only if Scrapyd is running behind a reverse proxy, and if the public URL contains a base path, before the Scrapyd API path components.
+Defaults to ``x-forwarded-prefix``.
+
 runner
 ------
 
 The module that will be used for launching sub-processes. You can customize the
 Scrapy processes launched from Scrapyd by using your own module.
 
 application
@@ -138,14 +177,24 @@
 
 A function that returns the (Twisted) Application object to use. This can be
 used if you want to extend Scrapyd by adding and removing your own components
 and services.
 
 For more info see `Twisted Application Framework`_
 
+.. _spiderqueue:
+
+spiderqueue
+-----------
+
+The scheduler enqueues crawls in per-project spider queues, for the poller to pick.
+You can define a custom spider queue class that implements the ISpiderQueue interface.
+
+Defaults to ``scrapyd.spiderqueue.SqliteSpiderQueue``.
+
 .. _webroot:
 
 webroot
 -------
 
 A twisted web resource that represents the interface to scrapyd.
 Scrapyd includes an interface with a website to provide simple monitoring
@@ -156,25 +205,28 @@
 ----------
 
 A class that stores finished jobs. There are 2 implementations provided:
 
 * ``scrapyd.jobstorage.MemoryJobStorage`` (default) jobs are stored in memory and lost when the daemon is restarted
 * ``scrapyd.jobstorage.SqliteJobStorage`` jobs are persisted in a Sqlite database in ``dbs_dir``
 
-If another backend is needed, one can implement its own class by implementing the IJobStorage 
+If another backend is needed, one can implement its own class by implementing the IJobStorage
 interface.
 
+.. _eggstorage:
+
 eggstorage
 ----------
 
-A class that stores and retrieves eggs for running spiders. 
-The default implementation is FilesystemEggStorage and stores eggs on the file system based on
-``eggs_dir`` configuration.
+A class that stores project eggs, implementing the ``IEggStorage`` interface.
+
+The default value is ``scrapyd.eggstorage.FilesystemEggStorage``.
+This implementation stores eggs in the directory specified by the :ref:`eggs_dir` setting.
 
-One can customize the storage by implementing the IEggStorage interface.
+You can implement your own egg storage: for example, to store eggs remotely.
 
 node_name
 ---------
 
 .. versionadded:: 1.1
 
 The node name for each node to something like the display hostname. Defaults to ``${socket.gethostname()}``.
```

### Comparing `scrapyd-1.4.1/docs/contributing.rst` & `scrapyd-1.4.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/docs/install.rst` & `scrapyd-1.4.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/docs/news.rst` & `scrapyd-1.4.2/docs/news.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 .. _news:
 
 Release notes
 =============
 
+1.4.2 (2023-05-01)
+------------------
+
+Added
+~~~~~
+
+- Add ``spiderqueue`` configuration option for custom spider queue.
+- Add support for the X-Forwarded-Prefix HTTP header. Rename this header using the :ref:`prefix_header` configuration option.
+
+Changed
+~~~~~~~
+
+- ``scrapyd.spiderqueue.SqliteSpiderQueue`` is initialized with a ``scrapyd.config.Config`` object and a project name, rather than a SQLite connection string (i.e. database file path).
+- If ``dbs_dir`` is set to ``:memory`` or to a URL, it is passed through without modification and without creating a directory to ``scrapyd.jobstorage.SqliteJobStorage`` and ``scrapyd.spiderqueue.SqliteSpiderQueue``.
+- ``scrapyd.utils.get_spider_queues`` defers the creation of the ``dbs_dir`` directory to the spider queue implementation.
+
 1.4.1 (2023-02-10)
 ------------------
 
 Fixed
 ~~~~~
 
 - Encode the ``FEEDS`` command-line argument as JSON.
 
 1.4.0 (2023-02-07)
 ------------------
 
 Added
 ~~~~~
 
-- Add ``item_url`` and ``log_url`` to the response from the listjobs.json webservice. (@mxdev88)
+- Add ``items_url`` and ``log_url`` to the response from the listjobs.json webservice. (@mxdev88)
 - Scrapy 2.8 support. Scrapyd sets ``LOG_FILE`` and ``FEEDS`` command-line arguments, instead of ``SCRAPY_LOG_FILE`` and ``SCRAPY_FEED_URI`` environment variables.
 - Python 3.11 support.
 - Python 3.12 support. Use ``packaging.version.Version`` instead of ``distutils.LooseVersion``. (@pawelmhm)
 
 Changed
 ~~~~~~~
 
@@ -164,71 +180,49 @@
 - ``FEED_URI`` was always overridden by Scrapyd.
 - Specify maximum versions for requirements that became incompatible.
 - Mark package as zip-unsafe because Twistd requires a plain ``txapp.py``.
 
 1.1.0 (2015-06-29)
 ------------------
 
-Features & Enhancements
-~~~~~~~~~~~~~~~~~~~~~~~
+Added
+~~~~~
+
+- Add ``node_name`` (hostname) to webservice responses. (:commit:`fac3a5c`, :commit:`4aebe1c`)
+- Add ``start_time`` to the response from the listjobs.json webservice. (:commit:`6712af9`, :commit:`acd460b`)
+
+Changed
+~~~~~~~
 
-- Outsource scrapyd-deploy command to scrapyd-client (c1358dc, c9d66ca..191353e)
-  **If you rely on this command, install the scrapyd-client package from pypi.**
-- Look for a ``~/.scrapyd.conf`` file in the users home (1fce99b)
-- Adding the nodename to identify the process that is working on the job (fac3a5c..4aebe1c)
-- Allow remote items store (e261591..35a21db)
-- Debian sysvinit script (a54193a, ff457a9)
-- Add 'start_time' field in webservice for running jobs (6712af9, acd460b)
-- Check if a spider exists before schedule it (with sqlite cache) (#8, 288afef..a185ff2)
-
-Bugfixes
-~~~~~~~~
-
-- F̶i̶x̶ ̶s̶c̶r̶a̶p̶y̶d̶-̶d̶e̶p̶l̶o̶y̶ ̶-̶-̶l̶i̶s̶t̶-̶p̶r̶o̶j̶e̶c̶t̶s̶ ̶(̶9̶4̶2̶a̶1̶b̶2̶)̶ → moved to scrapyd-client
-- Sanitize version names when creating egg paths (8023720)
-- Copy txweb/JsonResource from scrapy which no longer provides it (99ea920)
-- Use w3lib to generate correct feed uris (9a88ea5)
-- Fix GIT versioning for projects without annotated tags (e91dcf4 #34)
-- Correcting HTML tags in scrapyd website monitor (da5664f, 26089cd)
-- Fix FEED_URI path on windows (4f0060a)
-
-Setup script and Tests/CI
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-- Restore integration test script (66de25d)
-- Changed scripts to be installed using entry_points (b670f5e)
-- Renovate scrapy upstart job (d130770)
-- Travis.yml: remove deprecated ``--use-mirros`` pip option (b3cdc61)
-- Mark package as zip unsafe because twistd requires a plain ``txapp.py`` (f27c054)
-- Removed python 2.6/lucid env from travis (5277755)
-- Made Scrapyd package name lowercase (1adfc31)
-
-Documentation
-~~~~~~~~~~~~~
-
-- Spiders should allow for arbitrary keyword arguments (696154)
-- Various typos (51f1d69, 0a4a77a)
-- Fix release notes: 1.0 is already released (6c8dcfb)
-- Point website module's links to readthedocs (215c700)
-- Remove reference to 'scrapy server' command (f599b60)
+- Move scrapyd-deploy command to `scrapyd-client <https://pypi.org/project/scrapyd-client/>`__ package. (:commit:`c1358dc`, :commit:`c9d66ca`, :commit:`191353e`)
+- Allow remote ``items_dir`` configuration. (:commit:`e261591`, :commit:`35a21db`)
+- Look for a ``~/.scrapyd.conf`` file in the user's home directory. (:commit:`1fce99b`)
 
-1.0.2 (2016-03-28)
-------------------
+Fixed
+~~~~~
 
-setup script
-~~~~~~~~~~~~
+- Check if a spider exists before scheduling it. (:issue:`8`, :commit:`288afef`, :commit:`a185ff2`)
+- Sanitize version names when creating egg paths. (:commit:`8023720`)
+- Generate correct feed URIs, using w3lib. (:commit:`9a88ea5`)
+- Fix git versioning for projects without annotated tags. (:issue:`34`, :commit:`e91dcf4`)
+- Use valid HTML markup on website pages. (:commit:`da5664f`, :commit:`26089cd`)
+- Use ``file`` protocol for ``SCRAPY_FEED_URI`` environment variable on Windows. (:commit:`4f0060a`)
+- Copy ``JsonResource`` class from Scrapy, which no longer provides it. (:commit:`99ea920`)
+- Lowercase ``scrapyd`` package name. (:commit:`1adfc31`).
+- Mark package as zip-unsafe, because Twisted requires a plain ``txapp.py``. (:commit:`f27c054`)
+- Install scripts using ``entry_points`` instead of ``scripts``. (:commit:`b670f5e`)
 
-- Specified maximum versions for requirements that became incompatible.
-- Marked package as zip-unsafe because twistd requires a plain ``txapp.py``
+1.0.2 (2016-03-28)
+------------------
 
-documentation
-~~~~~~~~~~~~~
+Fixed
+~~~~~
 
-- Updated broken links, references to wrong versions and scrapy
-- Warn that scrapyd 1.0 felling out of support
+- Mark package as zip-unsafe, because Twisted requires a plain ``txapp.py``.
+- Specify maximum versions for compatible requirements.
 
 1.0.1 (2013-09-02)
 ------------------
 
 *Trivial update*
 
 1.0.0 (2013-09-02)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrapyd-1.4.1/docs/overview.rst` & `scrapyd-1.4.2/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/integration_tests/__init__.py` & `scrapyd-1.4.2/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/integration_tests/test_webservice.py` & `scrapyd-1.4.2/integration_tests/test_webservice.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/_deprecate.py` & `scrapyd-1.4.2/scrapyd/_deprecate.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/app.py` & `scrapyd-1.4.2/scrapyd/app.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/basicauth.py` & `scrapyd-1.4.2/scrapyd/basicauth.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/config.py` & `scrapyd-1.4.2/scrapyd/config.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/default_scrapyd.conf` & `scrapyd-1.4.2/scrapyd/default_scrapyd.conf`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 max_proc_per_cpu = 4
 finished_to_keep = 100
 poll_interval = 5.0
 bind_address = 127.0.0.1
 http_port   = 6800
 username    =
 password    =
+prefix_header = x-forwarded-prefix
 debug       = off
 runner      = scrapyd.runner
 jobstorage  = scrapyd.jobstorage.MemoryJobStorage
 application = scrapyd.app.application
 launcher    = scrapyd.launcher.Launcher
+spiderqueue = scrapyd.spiderqueue.SqliteSpiderQueue
 webroot     = scrapyd.website.Root
 eggstorage  = scrapyd.eggstorage.FilesystemEggStorage
 
 [services]
 schedule.json     = scrapyd.webservice.Schedule
 cancel.json       = scrapyd.webservice.Cancel
 addversion.json   = scrapyd.webservice.AddVersion
```

### Comparing `scrapyd-1.4.1/scrapyd/eggstorage.py` & `scrapyd-1.4.2/scrapyd/eggstorage.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/eggutils.py` & `scrapyd-1.4.2/scrapyd/eggutils.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/environ.py` & `scrapyd-1.4.2/scrapyd/environ.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/interfaces.py` & `scrapyd-1.4.2/scrapyd/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,18 +101,24 @@
         """Called when projects may have changed, to refresh the available
         projects"""
 
 
 class IEnvironment(Interface):
     """A component to generate the environment of crawler processes"""
 
+    def get_settings(message):
+        """Return the Scrapy settings to use for running the process.
+
+        `message` is the message received from the IPoller.next() method.
+        """
+
     def get_environment(message, slot):
         """Return the environment variables to use for running the process.
 
-        `message` is the message received from the IPoller.next() method
+        `message` is the message received from the IPoller.next() method.
         `slot` is the Launcher slot where the process will be running.
         """
 
 
 class IJobStorage(Interface):
     """A component that handles storing and retrieving finished jobs. """
```

### Comparing `scrapyd-1.4.1/scrapyd/jobstorage.py` & `scrapyd-1.4.2/scrapyd/jobstorage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
 from datetime import datetime
 
 from zope.interface import implementer
 
 from scrapyd.interfaces import IJobStorage
 from scrapyd.sqlite import SqliteFinishedJobs
+from scrapyd.utils import sqlite_connection_string
 
 
 def job_log_url(job):
     return f"/logs/{job.project}/{job.spider}/{job.job}.log"
 
 
 def job_items_url(job):
@@ -46,19 +46,15 @@
             yield j
 
 
 @implementer(IJobStorage)
 class SqliteJobStorage(object):
 
     def __init__(self, config):
-        dbsdir = config.get('dbs_dir', 'dbs')
-        if not os.path.exists(dbsdir):
-            os.makedirs(dbsdir)
-        dbpath = os.path.join(dbsdir, 'jobs.db')
-        self.jstorage = SqliteFinishedJobs(dbpath, "finished_jobs")
+        self.jstorage = SqliteFinishedJobs(sqlite_connection_string(config, 'jobs'), "finished_jobs")
         self.finished_to_keep = config.getint('finished_to_keep', 100)
 
     def add(self, job):
         self.jstorage.add(job)
         self.jstorage.clear(self.finished_to_keep)
 
     def list(self):
```

### Comparing `scrapyd-1.4.1/scrapyd/launcher.py` & `scrapyd-1.4.2/scrapyd/launcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         message['settings'].update(e.get_settings(message))
         msg = native_stringify_dict(message, keys_only=False)
         project = msg['_project']
         args = [sys.executable, '-m', self.runner, 'crawl']
         args += get_crawl_args(msg)
         env = e.get_environment(msg, slot)
         env = native_stringify_dict(env, keys_only=False)
-        pp = ScrapyProcessProtocol(slot, project, msg['_spider'],
-                                   msg['_job'], env)
+        pp = ScrapyProcessProtocol(project, msg['_spider'], msg['_job'], env, args)
         pp.deferred.addBoth(self._process_finished, slot)
         reactor.spawnProcess(pp, sys.executable, args=args, env=env)
         self.processes[slot] = pp
 
     def _process_finished(self, _, slot):
         process = self.processes.pop(slot)
         process.end_time = datetime.now()
@@ -64,25 +63,23 @@
                 cpus = 1
             max_proc = cpus * config.getint('max_proc_per_cpu', 4)
         return max_proc
 
 
 class ScrapyProcessProtocol(protocol.ProcessProtocol):
 
-    def __init__(self, slot, project, spider, job, env):
-        self.slot = slot
+    def __init__(self, project, spider, job, env, args):
         self.pid = None
         self.project = project
         self.spider = spider
         self.job = job
         self.start_time = datetime.now()
         self.end_time = None
         self.env = env
-        self.logfile = env.get('SCRAPYD_LOG_FILE')
-        self.itemsfile = env.get('SCRAPYD_FEED_URI')
+        self.args = args
         self.deferred = defer.Deferred()
 
     def outReceived(self, data):
         log.msg(data.rstrip(), system="Launcher,%d/stdout" % self.pid)
 
     def errReceived(self, data):
         log.msg(data.rstrip(), system="Launcher,%d/stderr" % self.pid)
@@ -95,10 +92,10 @@
         if isinstance(status.value, error.ProcessDone):
             self.log("Process finished: ")
         else:
             self.log("Process died: exitstatus=%r " % status.value.exitCode)
         self.deferred.callback(self)
 
     def log(self, action):
-        fmt = '%(action)s project=%(project)r spider=%(spider)r job=%(job)r pid=%(pid)r log=%(log)r items=%(items)r'
+        fmt = '%(action)s project=%(project)r spider=%(spider)r job=%(job)r pid=%(pid)r args=%(args)r'
         log.msg(format=fmt, action=action, project=self.project, spider=self.spider,
-                job=self.job, pid=self.pid, log=self.logfile, items=self.itemsfile)
+                job=self.job, pid=self.pid, args=self.args)
```

### Comparing `scrapyd-1.4.1/scrapyd/poller.py` & `scrapyd-1.4.2/scrapyd/poller.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/runner.py` & `scrapyd-1.4.2/scrapyd/runner.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/scheduler.py` & `scrapyd-1.4.2/scrapyd/scheduler.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/sqlite.py` & `scrapyd-1.4.2/scrapyd/sqlite.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/conftest.py` & `scrapyd-1.4.2/scrapyd/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/logstdout.egg` & `scrapyd-1.4.2/scrapyd/tests/logstdout.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/mockserver.py` & `scrapyd-1.4.2/scrapyd/tests/mockserver.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/mybot.egg` & `scrapyd-1.4.2/scrapyd/tests/mybot.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/mybot2.egg` & `scrapyd-1.4.2/scrapyd/tests/mybot2.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/mybot3.egg` & `scrapyd-1.4.2/scrapyd/tests/mybot3.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/mybotunicode.egg` & `scrapyd-1.4.2/scrapyd/tests/mybotunicode.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/quotesbot.egg` & `scrapyd-1.4.2/scrapyd/tests/quotesbot.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/quotesbot_asyncio.egg` & `scrapyd-1.4.2/scrapyd/tests/quotesbot_asyncio.egg`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/start_mock_app.py` & `scrapyd-1.4.2/scrapyd/tests/start_mock_app.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_dont_load_settings.py` & `scrapyd-1.4.2/scrapyd/tests/test_dont_load_settings.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_eggstorage.py` & `scrapyd-1.4.2/scrapyd/tests/test_eggstorage.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_endpoints.py` & `scrapyd-1.4.2/scrapyd/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_environ.py` & `scrapyd-1.4.2/scrapyd/tests/test_environ.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_jobstorage.py` & `scrapyd-1.4.2/scrapyd/tests/test_jobstorage.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_poller.py` & `scrapyd-1.4.2/scrapyd/tests/test_poller.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_scheduler.py` & `scrapyd-1.4.2/scrapyd/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_scripts.py` & `scrapyd-1.4.2/scrapyd/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_spiderqueue.py` & `scrapyd-1.4.2/scrapyd/tests/test_spiderqueue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from twisted.internet.defer import inlineCallbacks, maybeDeferred
 from twisted.trial import unittest
 from zope.interface.verify import verifyObject
 
 from scrapyd import spiderqueue
+from scrapyd.config import Config
 from scrapyd.interfaces import ISpiderQueue
 
 
 class SpiderQueueTest(unittest.TestCase):
     """This test case also supports queues with deferred methods.
     """
 
     def setUp(self):
-        self.q = spiderqueue.SqliteSpiderQueue(':memory:')
+        self.q = spiderqueue.SqliteSpiderQueue(Config(values={'dbs_dir': ':memory:'}), 'quotesbot')
         self.name = 'spider1'
         self.priority = 5
         self.args = {
             'arg1': 'val1',
             'arg2': 2,
             'arg3': u'\N{SNOWMAN}',
         }
```

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_sqlite.py` & `scrapyd-1.4.2/scrapyd/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_utils.py` & `scrapyd-1.4.2/scrapyd/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_webservice.py` & `scrapyd-1.4.2/scrapyd/tests/test_webservice.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/tests/test_website.py` & `scrapyd-1.4.2/scrapyd/tests/test_website.py`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/scrapyd/utils.py` & `scrapyd-1.4.2/scrapyd/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 import sys
 from subprocess import PIPE, Popen
+from urllib.parse import urlsplit
 
 from packaging.version import InvalidVersion, Version
 from scrapy.utils.misc import load_object
 from twisted.web import resource
 
 from scrapyd.config import Config
-from scrapyd.spiderqueue import SqliteSpiderQueue
 from scrapyd.sqlite import JsonSqliteDict
 
 
 class JsonResource(resource.Resource):
 
     json_encoder = json.JSONEncoder()
 
@@ -51,22 +51,25 @@
 
     def __setitem__(self, key, value):
         self.cache_manager[key] = value
 
 
 def get_spider_queues(config):
     """Return a dict of Spider Queues keyed by project name"""
-    dbsdir = config.get('dbs_dir', 'dbs')
-    if not os.path.exists(dbsdir):
-        os.makedirs(dbsdir)
-    d = {}
-    for project in get_project_list(config):
-        dbpath = os.path.join(dbsdir, '%s.db' % project)
-        d[project] = SqliteSpiderQueue(dbpath)
-    return d
+    spiderqueue = load_object(config.get('spiderqueue', 'scrapyd.spiderqueue.SqliteSpiderQueue'))
+    return {project: spiderqueue(config, project) for project in get_project_list(config)}
+
+
+def sqlite_connection_string(config, database):
+    dbs_dir = config.get('dbs_dir', 'dbs')
+    if dbs_dir == ':memory:' or urlsplit(dbs_dir).scheme:
+        return dbs_dir
+    if not os.path.exists(dbs_dir):
+        os.makedirs(dbs_dir)
+    return os.path.join(dbs_dir, f'{database}.db')
 
 
 def get_project_list(config):
     """Get list of projects by inspecting the eggs storage and the ones defined in
     the scrapyd.conf [settings] section
     """
     eggstorage = config.get('eggstorage', 'scrapyd.eggstorage.FilesystemEggStorage')
```

### Comparing `scrapyd-1.4.1/scrapyd/webservice.py` & `scrapyd-1.4.2/scrapyd/webservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,22 +136,24 @@
             for qname in (queues if project is None else [project])
             for x in queues[qname].list()
         ]
         running = [
             {
                 "project": s.project,
                 "spider": s.spider,
-                "id": s.job, "pid": s.pid,
+                "id": s.job,
+                "pid": s.pid,
                 "start_time": str(s.start_time),
             } for s in spiders if project is None or s.project == project
         ]
         finished = [
             {
                 "project": s.project,
-                "spider": s.spider, "id": s.job,
+                "spider": s.spider,
+                "id": s.job,
                 "start_time": str(s.start_time),
                 "end_time": str(s.end_time),
                 "log_url": job_log_url(s),
                 "items_url": job_items_url(s),
             } for s in self.root.launcher.finished
             if project is None or s.project == project
         ]
```

### Comparing `scrapyd-1.4.1/scrapyd/website.py` & `scrapyd-1.4.2/scrapyd/website.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 from twisted.application.service import IServiceCollection
 from twisted.web import resource, static
 
 from scrapyd.interfaces import IEggStorage, IPoller, ISpiderScheduler
 from scrapyd.jobstorage import job_items_url, job_log_url
 
 
+class PrefixHeaderMixin:
+    def get_base_path(self, txrequest):
+        return txrequest.getHeader(self.prefix_header) or ''
+
+
 class Root(resource.Resource):
 
     def __init__(self, config, app):
         resource.Resource.__init__(self)
         self.debug = config.getboolean('debug', False)
         self.runner = config.get('runner')
+        self.prefix_header = config.get('prefix_header')
         logsdir = config.get('logs_dir')
         itemsdir = config.get('items_dir')
         self.local_items = itemsdir and (urlparse(itemsdir).scheme.lower() in ['', 'file'])
         self.app = app
         self.nodename = config.get('node_name', socket.gethostname())
         self.putChild(b'', Home(self, self.local_items))
         if logsdir:
@@ -51,38 +57,40 @@
         return self.app.getComponent(IEggStorage)
 
     @property
     def poller(self):
         return self.app.getComponent(IPoller)
 
 
-class Home(resource.Resource):
+class Home(PrefixHeaderMixin, resource.Resource):
 
     def __init__(self, root, local_items):
         resource.Resource.__init__(self)
         self.root = root
         self.local_items = local_items
+        self.prefix_header = root.prefix_header
 
     def render_GET(self, txrequest):
         vars = {
-            'projects': ', '.join(self.root.scheduler.list_projects())
+            'projects': ', '.join(self.root.scheduler.list_projects()),
+            'base_path': self.get_base_path(txrequest),
         }
         s = """
 <html>
 <head><title>Scrapyd</title></head>
 <body>
 <h1>Scrapyd</h1>
 <p>Available projects: <b>%(projects)s</b></p>
 <ul>
-<li><a href="/jobs">Jobs</a></li>
-""" % vars
+<li><a href="%(base_path)s/jobs">Jobs</a></li>
+"""
         if self.local_items:
-            s += '<li><a href="/items/">Items</a></li>'
+            s += '<li><a href="%(base_path)s/items/">Items</a></li>'
         s += """
-<li><a href="/logs/">Logs</a></li>
+<li><a href="%(base_path)s/logs/">Logs</a></li>
 <li><a href="http://scrapyd.readthedocs.org/en/latest/">Documentation</a></li>
 </ul>
 
 <h2>How to schedule a spider?</h2>
 
 <p>To schedule a spider you need to use the API (this web UI is only for
 monitoring)</p>
@@ -90,38 +98,39 @@
 <p>Example using <a href="http://curl.haxx.se/">curl</a>:</p>
 <p><code>curl http://localhost:6800/schedule.json -d project=default -d spider=somespider</code></p>
 
 <p>For more information about the API, see the
 <a href="http://scrapyd.readthedocs.org/en/latest/">Scrapyd documentation</a></p>
 </body>
 </html>
-""" % vars
+"""
         txrequest.setHeader('Content-Type', 'text/html; charset=utf-8')
-        s = s.encode('utf8')
+        s = (s % vars).encode('utf8')
         txrequest.setHeader('Content-Length', str(len(s)))
         return s
 
 
 def microsec_trunc(timelike):
     if hasattr(timelike, 'microsecond'):
         ms = timelike.microsecond
     else:
         ms = timelike.microseconds
     return timelike - timedelta(microseconds=ms)
 
 
-class Jobs(resource.Resource):
+class Jobs(PrefixHeaderMixin, resource.Resource):
 
     def __init__(self, root, local_items):
         resource.Resource.__init__(self)
         self.root = root
         self.local_items = local_items
+        self.prefix_header = root.prefix_header
 
     cancel_button = """
-    <form method="post" action="/cancel.json">
+    <form method="post" action="{base_path}/cancel.json">
     <input type="hidden" name="project" value="{project}"/>
     <input type="hidden" name="job" value="{jobid}"/>
     <input type="submit" style="float: left;" value="Cancel"/>
     </form>
     """.format
 
     header_cols = [
@@ -157,15 +166,15 @@
         return (
             '<html>'
             '<head>'
             '<title>Scrapyd</title>'
             '<style type="text/css">' + self.gen_css() + '</style>'
             '</head>'
             '<body><h1>Jobs</h1>'
-            '<p><a href="..">Go up</a></p>'
+            '<p><a href="./">Go up</a></p>'
             + self.prep_table() +
             '</body>'
             '</html>'
         )
 
     def prep_table(self):
         return (
@@ -188,50 +197,51 @@
 
     def prep_tab_pending(self):
         return '\n'.join(
             self.prep_row({
                 "Project": project,
                 "Spider": m['name'],
                 "Job": m['_job'],
-                "Cancel": self.cancel_button(project=project, jobid=m['_job']),
+                "Cancel": self.cancel_button(project=project, jobid=m['_job'], base_path=self.base_path),
             })
             for project, queue in self.root.poller.queues.items()
             for m in queue.list()
         )
 
     def prep_tab_running(self):
         return '\n'.join(
             self.prep_row({
                 "Project": p.project,
                 "Spider": p.spider,
                 "Job": p.job,
                 "PID": p.pid,
                 "Start": microsec_trunc(p.start_time),
                 "Runtime": microsec_trunc(datetime.now() - p.start_time),
-                "Log": f'<a href="{job_log_url(p)}">Log</a>',
-                "Items": f'<a href="{job_items_url(p)}">Items</a>',
-                "Cancel": self.cancel_button(project=p.project, jobid=p.job),
+                "Log": f'<a href="{self.base_path}{job_log_url(p)}">Log</a>',
+                "Items": f'<a href="{self.base_path}{job_items_url(p)}">Items</a>',
+                "Cancel": self.cancel_button(project=p.project, jobid=p.job, base_path=self.base_path),
             })
             for p in self.root.launcher.processes.values()
         )
 
     def prep_tab_finished(self):
         return '\n'.join(
             self.prep_row({
                 "Project": p.project,
                 "Spider": p.spider,
                 "Job": p.job,
                 "Start": microsec_trunc(p.start_time),
                 "Runtime": microsec_trunc(p.end_time - p.start_time),
                 "Finish": microsec_trunc(p.end_time),
-                "Log": f'<a href="{job_log_url(p)}">Log</a>',
-                "Items": f'<a href="{job_items_url(p)}">Items</a>',
+                "Log": f'<a href="{self.base_path}{job_log_url(p)}">Log</a>',
+                "Items": f'<a href="{self.base_path}{job_items_url(p)}">Items</a>',
             })
             for p in self.root.launcher.finished
         )
 
     def render(self, txrequest):
+        self.base_path = self.get_base_path(txrequest)
         doc = self.prep_doc()
         txrequest.setHeader('Content-Type', 'text/html; charset=utf-8')
         doc = doc.encode('utf-8')
         txrequest.setHeader('Content-Length', str(len(doc)))
         return doc
```

### Comparing `scrapyd-1.4.1/scrapyd.egg-info/PKG-INFO` & `scrapyd-1.4.2/scrapyd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapyd
-Version: 1.4.1
+Version: 1.4.2
 Summary: A service for running Scrapy spiders, with an HTTP API
 Home-page: https://github.com/scrapy/scrapyd
 Author: Scrapy developers
 Author-email: info@scrapy.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrapyd-1.4.1/scrapyd.egg-info/SOURCES.txt` & `scrapyd-1.4.2/scrapyd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapyd-1.4.1/setup.py` & `scrapyd-1.4.2/setup.py`

 * *Files identical despite different names*

