# Comparing `tmp/UpyTest-3.0.3.tar.gz` & `tmp/UpyTest-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.0.3.tar", last modified: Thu Apr 20 23:22:43 2023, max compression
+gzip compressed data, was "UpyTest-3.0.5.tar", last modified: Mon May  1 00:13:11 2023, max compression
```

## Comparing `UpyTest-3.0.3.tar` & `UpyTest-3.0.5.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.269329 UpyTest-3.0.3/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 23:22:43.265329 UpyTest-3.0.3/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.257329 UpyTest-3.0.3/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2109 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-04-20 23:22:43.269329 UpyTest-3.0.3/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-04-20 23:22:40.000000 UpyTest-3.0.3/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.257329 UpyTest-3.0.3/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 UpyTest-3.0.3/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.257329 UpyTest-3.0.3/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 22:45:13.000000 UpyTest-3.0.3/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35987 2023-04-20 22:44:56.000000 UpyTest-3.0.3/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 UpyTest-3.0.3/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 UpyTest-3.0.3/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 UpyTest-3.0.3/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/EmptyTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/ExceptionTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/FailedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/PassedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/Test.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 UpyTest-3.0.3/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.3/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.265329 UpyTest-3.0.3/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15844 2023-04-20 23:20:27.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36644 2023-04-20 23:21:08.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2875 2023-04-20 19:27:21.000000 UpyTest-3.0.3/thonnycontrib/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9844 2023-04-20 19:27:15.000000 UpyTest-3.0.3/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 UpyTest-3.0.3/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.265329 UpyTest-3.0.3/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 UpyTest-3.0.3/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.164012 UpyTest-3.0.5/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-05-01 00:13:11.164012 UpyTest-3.0.5/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.152012 UpyTest-3.0.5/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-05-01 00:13:11.000000 UpyTest-3.0.5/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2192 2023-05-01 00:13:11.000000 UpyTest-3.0.5/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-05-01 00:13:11.000000 UpyTest-3.0.5/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-05-01 00:13:11.000000 UpyTest-3.0.5/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-05-01 00:13:11.000000 UpyTest-3.0.5/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-05-01 00:13:11.164012 UpyTest-3.0.5/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-05-01 00:13:08.000000 UpyTest-3.0.5/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.156012 UpyTest-3.0.5/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 UpyTest-3.0.5/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.156012 UpyTest-3.0.5/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 22:45:13.000000 UpyTest-3.0.5/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35987 2023-04-20 22:44:56.000000 UpyTest-3.0.5/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 UpyTest-3.0.5/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 UpyTest-3.0.5/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 UpyTest-3.0.5/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.156012 UpyTest-3.0.5/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/EmptyTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/ExceptionTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/FailedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/PassedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/Test.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.156012 UpyTest-3.0.5/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.160012 UpyTest-3.0.5/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.0.5/thonnycontrib/docs/res/outline-class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.0.5/thonnycontrib/docs/res/outline-method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.160012 UpyTest-3.0.5/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 UpyTest-3.0.5/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 UpyTest-3.0.5/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.160012 UpyTest-3.0.5/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.5/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.160012 UpyTest-3.0.5/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17884 2023-05-01 00:11:17.000000 UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36644 2023-04-20 23:21:08.000000 UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3328 2023-04-23 13:33:11.000000 UpyTest-3.0.5/thonnycontrib/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9776 2023-04-30 23:34:26.000000 UpyTest-3.0.5/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 UpyTest-3.0.5/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-05-01 00:13:11.160012 UpyTest-3.0.5/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.5/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.5/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.5/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 UpyTest-3.0.5/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 UpyTest-3.0.5/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 UpyTest-3.0.5/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.5/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 UpyTest-3.0.5/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 UpyTest-3.0.5/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 UpyTest-3.0.5/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.0.3/PKG-INFO` & `UpyTest-3.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.0.3
+Version: 3.0.5
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
-License: UNKNOWN
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.9
 
 A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
-
```

### Comparing `UpyTest-3.0.3/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.0.5/UpyTest.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.0.3
+Version: 3.0.5
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
-License: UNKNOWN
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.9
 
 A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
-
```

### Comparing `UpyTest-3.0.3/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.0.5/UpyTest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 thonnycontrib/backend/verdicts/PassedTest.py
 thonnycontrib/backend/verdicts/Test.py
 thonnycontrib/backend/verdicts/__init__.py
 thonnycontrib/docs/__init__.py
 thonnycontrib/docs/res/failed.png
 thonnycontrib/docs/res/l1test_icon.png
 thonnycontrib/docs/res/l1test_icon_old.png
+thonnycontrib/docs/res/outline-class.png
+thonnycontrib/docs/res/outline-method.gif
 thonnycontrib/docs/res/passed.png
 thonnycontrib/docs/res/pending_icon.png
 thonnycontrib/docs/res/test_only_btn.png
 thonnycontrib/docs/res/warning.png
 thonnycontrib/docstring_generator/__init__.py
 thonnycontrib/docstring_generator/doc_generator.py
 thonnycontrib/docstring_generator/doc_template.py
```

### Comparing `UpyTest-3.0.3/setup.py` & `UpyTest-3.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.0.3",
+    version="3.0.5",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.0.3/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.0.5/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.0.5/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.0.5/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/evaluator.py` & `UpyTest-3.0.5/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.0.5/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/test_finder.py` & `UpyTest-3.0.5/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/verdicts/ExceptionTest.py` & `UpyTest-3.0.5/thonnycontrib/backend/verdicts/ExceptionTest.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/verdicts/FailedTest.py` & `UpyTest-3.0.5/thonnycontrib/backend/verdicts/FailedTest.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/backend/verdicts/Test.py` & `UpyTest-3.0.5/thonnycontrib/backend/verdicts/Test.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/failed.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/passed.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docs/res/warning.png` & `UpyTest-3.0.5/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.0.5/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.0.5/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/environement_vars.py` & `UpyTest-3.0.5/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/exceptions.py` & `UpyTest-3.0.5/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.0.5/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections import namedtuple
 from thonny.workbench import WorkbenchEvent
+from ..utils import send_to_backend
 from ..backend.verdicts.Test import Test
 from ..environement_vars import IS_SELECTED_VAR
 from ..exceptions import *
 from .l1test_reporter import *
 from ..properties import *
 from thonny.common import ToplevelResponse, InlineResponse
 from thonnycontrib import l1test_frontend 
 from ..ThonnyLogsGenerator import log_in_thonny
-import pickle, inspect, thonny, ast
+import pickle, inspect, thonny, ast, time
 
 # ErrorMsg déclare deux champs : le préfixe et le message d'erreur
 # le préfix est juste le titre qui précède le message d'erreur sur la Error view
 ErrorMsg = namedtuple("ErrorMsg", "title msg")
 
 # Le nom de l'event qui lance le redémarrage du backend thonny
 BACKEND_RESTART_EVENT = "BackendRestart"
@@ -141,14 +142,54 @@
         Report the verdicts on the view.
 
         Args:
             test_results (dict): The recieved verdicts from the backend.
         """
         self._reporter.display_tests_results(test_results) 
     
+    def send_to_backend(self, is_selected, selected_line):
+        """Allows to execute the `L1test` magic command. 
+        
+        There's two cases : 
+        1. if the `L1test` is invoked for the first so the command is sent to 
+        backend to be executed by the thonny's runner. 
+        2. if the `L1test` is invoked while it's always running, so the L1TestRunner
+        will force to stop the backend before resending the command to the thonny's 
+        runner. Note: there's a delay of 0.3 second after the backend is restarted to allow 
+        the proxy to be initialized.
+
+        Args:
+            is_selected (bool): Set as True if only one method is selected to run
+                            it's tests.
+            selected_line (int): The number of the selected line.
+        """
+        if not self.is_running(): # si le plugin n'est pas en execution 
+            self.__send_to_backend(is_selected, selected_line)
+        else: # si le plugin est en cours d'execution et pas encore terminé
+            thonny.get_runner().cmd_stop_restart() # invoke le restart backend
+            
+            # on affiche sur la treeview comme quoi un restart backend forcé est en cours
+            self.get_reporter() \
+                .get_l1test_treeview() \
+                .insert_in_header("/!\ Force to restart backand ...", clear=True, tags=("red"))
+            
+            # on indique que l'état du plugin n'est plus en execution
+            self.set_is_running(False)
+            
+            # On donne un peu du temps au proxy pour se réinitialiser.
+            # La valeur choisit n'affecte pas le temps d'execution du plugin.
+            time.sleep(0.5) 
+            
+            # On invoque la commande magique L1test
+            self.__send_to_backend(is_selected, selected_line)
+    
+    def __send_to_backend(self, is_selected, selected_line):
+        self.set_is_running()
+        send_to_backend(is_selected=is_selected, selected_line=selected_line)
+        
     def __handle_raised_exception(self, exception: dict) -> ErrorMsg:
         """
         This function handles the raised exception by returning a tuple containing
         a prefix message and the exception message.
 
         The prefix refers to the title shown on the ErrorView. If you want to remove 
         the title, you should specify the prefix as an empty string. If you don't
```

### Comparing `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.0.5/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/outlines.py` & `UpyTest-3.0.5/thonnycontrib/outlines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from typing import List
 import re
 from thonny import get_workbench
 from functools import partial
 from .properties import PLUGIN_NAME
-import tkinter as tk
+import tkinter as tk, os
 
 _OUTLINE_REGEX = r"\s*(?P<type>def|class)[ ]+(?P<name>[\w]+)"
 
 # Ceci est une implémentation de création d'un singleton pour OutlineParser
 _outliner = None
 
 class OutlinedNode():
     def __init__(self, type:str, name:str, lineno:int) -> None:
         self.__type = type
         self.__name = name
         self.__lineno = lineno
+        
+        icon_filename = "outline-class.png" if self.__type == "class" else "outline-method.gif"
+        icon_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "docs/res", icon_filename)
+        self.__image = tk.PhotoImage(name=icon_path, file=icon_path)
     
     def get_type(self):
         return self.__type  
     
     def get_name(self):
         return self.__name  
     
     def get_lineno(self):
-        return self.__lineno    
+        return self.__lineno  
+    
+    def get_image(self):
+        return self.__image    
 
 class Outliner():   
     def __init__(self, workbench=get_workbench()) -> None:
         super().__init__()
         global _outliner
         _outliner = self
         
@@ -49,23 +56,25 @@
             lineno += 1
             match = re.match(_OUTLINE_REGEX,line) 
             if match:
                 outlined = OutlinedNode(match.group("type"), match.group("name"), lineno)
                 outlines.append(outlined)
         return outlines
     
-    def from_outlines_post_menu(self, source):
+    def from_source_post_menu(self, source):
         self.menu.delete(0, tk.END)
         outlines = self.__parse(source)
         for outline in outlines: 
             label = "%s %s" % (outline.get_type(), outline.get_name())
             self.menu.add_command(label=label, 
+                                  image=outline.get_image(),
                                   command=partial(run_outlined_test, outline.get_lineno()),
                                   activebackground="white",
-                                  activeforeground="darkblue")
+                                  activeforeground="darkblue",
+                                  compound=tk.LEFT)
     
     def get_menu(self):
         return self.menu
     
     
 def run_outlined_test(lineno:int):
     """
```

### Comparing `UpyTest-3.0.3/thonnycontrib/plugin_loader.py` & `UpyTest-3.0.5/thonnycontrib/plugin_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os, os.path
-from thonny import get_workbench
+from thonny import get_workbench, get_runner
 from thonny.editors import  EditorNotebook
 from thonny import editors
 from thonny.ui_utils import select_sequence
 from thonnycontrib.outlines import get_outliner, run_outlined_test
 from .docstring_generator.doc_generator import DocGenerator
 from .l1test_frontend.l1test_reporter import L1TestErrorView, L1TestTreeView
 from .exceptions import *
@@ -29,15 +29,15 @@
 def update_test_for_one_menu(event):
     editor = get_workbench().get_editor_notebook().get_current_editor()
     if editor is None:
         return
     source = editor.get_code_view().get_content()
     
     outliner = get_outliner()
-    outliner.from_outlines_post_menu(source)
+    outliner.from_source_post_menu(source)
 
 def run_selected_test():
     """
     Cette fonction est invoquée quand le button `Run test for selected function`
     suite à un clique droit sur une ligne du fichier.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test avec en argument
     is_selected=True.
@@ -57,15 +57,15 @@
 
 def _send_to_l1test_backend(is_selected: bool=False, selected_line: int=0):
     """
         Send a command to the l1test_backend.
         Args:
             is_selected (bool): Set as True if only one method is selected to run
                             it's tests.
-            test_only (bool): Set as True to run only the decorated(with @test_only) methods.
+            selected_line (int): The number of the selected line.
     """
     l1test_runner = get_l1test_runner()
     try:
         editor: EditorNotebook = get_workbench().get_editor_notebook()
         # si aucun editeur n'est ouvert sur le workbench
         if not editor.get_current_editor():
             raise NoEditorFoundException("No editor found !\n\nPlease open an editor before running the tests.")
@@ -82,18 +82,17 @@
             raise NotSavedFileException(msg)
 
         if not editor.get_current_editor_content().strip():  # L'éditeur est vide. 
             # on a pas envie d'envoyer une commande au backend si le fichier est vide.
             # Dans tous les cas y a rien à tester.
             raise EmptyEditorException("The editor is empty!\n")
         
-        # si on est là alors le fichier est bien sauvegardé et contient quelque chose.
-        l1test_runner.set_is_running()
+         # si on est là alors le fichier est bien sauvegardé et contient quelque chose.
+        l1test_runner.send_to_backend(is_selected, selected_line)
         
-        send_to_backend(is_selected=is_selected, selected_line=selected_line)
     except FrontendException as e: # on catche que les exception coté view
         l1test_runner.terminate_running()
         l1test_runner.set_has_exception(True) 
         l1test_runner.clean_error_view()
         l1test_runner.show_right_view(error_msg=str(e))
        
 def generate_auto_docstring(event):
```

### Comparing `UpyTest-3.0.3/thonnycontrib/properties.py` & `UpyTest-3.0.5/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.0.5/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.0.5/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.0.5/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.0.5/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.0.5/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.0.5/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/tests/tests_view.py` & `UpyTest-3.0.5/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.3/thonnycontrib/utils.py` & `UpyTest-3.0.5/thonnycontrib/utils.py`

 * *Files identical despite different names*

