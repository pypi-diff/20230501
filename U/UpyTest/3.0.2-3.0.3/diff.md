# Comparing `tmp/UpyTest-3.0.2.tar.gz` & `tmp/UpyTest-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.0.2.tar", last modified: Thu Apr 20 22:48:29 2023, max compression
+gzip compressed data, was "UpyTest-3.0.3.tar", last modified: Thu Apr 20 23:22:43 2023, max compression
```

## Comparing `UpyTest-3.0.2.tar` & `UpyTest-3.0.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.313171 UpyTest-3.0.2/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 22:48:29.313171 UpyTest-3.0.2/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.289171 UpyTest-3.0.2/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2109 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-04-20 22:48:29.313171 UpyTest-3.0.2/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-04-20 22:47:14.000000 UpyTest-3.0.2/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.297170 UpyTest-3.0.2/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 UpyTest-3.0.2/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.305171 UpyTest-3.0.2/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 20:40:22.000000 UpyTest-3.0.2/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35987 2023-04-20 22:46:44.000000 UpyTest-3.0.2/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 UpyTest-3.0.2/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 UpyTest-3.0.2/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 UpyTest-3.0.2/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.305171 UpyTest-3.0.2/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/EmptyTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/ExceptionTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/FailedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/PassedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/Test.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 UpyTest-3.0.2/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.2/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15610 2023-03-25 14:55:16.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36655 2023-04-07 14:49:23.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2875 2023-04-20 19:27:21.000000 UpyTest-3.0.2/thonnycontrib/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9844 2023-04-20 19:27:15.000000 UpyTest-3.0.2/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 UpyTest-3.0.2/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.313171 UpyTest-3.0.2/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 UpyTest-3.0.2/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.269329 UpyTest-3.0.3/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 23:22:43.265329 UpyTest-3.0.3/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.257329 UpyTest-3.0.3/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2109 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 23:22:43.000000 UpyTest-3.0.3/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-04-20 23:22:43.269329 UpyTest-3.0.3/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-04-20 23:22:40.000000 UpyTest-3.0.3/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.257329 UpyTest-3.0.3/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 UpyTest-3.0.3/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.257329 UpyTest-3.0.3/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 22:45:13.000000 UpyTest-3.0.3/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35987 2023-04-20 22:44:56.000000 UpyTest-3.0.3/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 UpyTest-3.0.3/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 UpyTest-3.0.3/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 UpyTest-3.0.3/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/EmptyTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/ExceptionTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/FailedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/PassedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/Test.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 UpyTest-3.0.3/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.261329 UpyTest-3.0.3/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.3/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.265329 UpyTest-3.0.3/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15844 2023-04-20 23:20:27.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36644 2023-04-20 23:21:08.000000 UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2875 2023-04-20 19:27:21.000000 UpyTest-3.0.3/thonnycontrib/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9844 2023-04-20 19:27:15.000000 UpyTest-3.0.3/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 UpyTest-3.0.3/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 23:22:43.265329 UpyTest-3.0.3/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 UpyTest-3.0.3/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 UpyTest-3.0.3/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.0.2/PKG-INFO` & `UpyTest-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.0.2
+Version: 3.0.3
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 License: UNKNOWN
 Platform: Windows
 Platform: macOS
 Platform: Linux
```

### Comparing `UpyTest-3.0.2/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.0.3/UpyTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.0.2
+Version: 3.0.3
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 License: UNKNOWN
 Platform: Windows
 Platform: macOS
 Platform: Linux
```

### Comparing `UpyTest-3.0.2/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.0.3/UpyTest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/setup.py` & `UpyTest-3.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.0.2",
+    version="3.0.3",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.0.2/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.0.3/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.0.3/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.0.3/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/evaluator.py` & `UpyTest-3.0.3/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.0.3/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/test_finder.py` & `UpyTest-3.0.3/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/verdicts/ExceptionTest.py` & `UpyTest-3.0.3/thonnycontrib/backend/verdicts/ExceptionTest.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/verdicts/FailedTest.py` & `UpyTest-3.0.3/thonnycontrib/backend/verdicts/FailedTest.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/backend/verdicts/Test.py` & `UpyTest-3.0.3/thonnycontrib/backend/verdicts/Test.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/failed.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/passed.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docs/res/warning.png` & `UpyTest-3.0.3/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.0.3/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/environement_vars.py` & `UpyTest-3.0.3/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/exceptions.py` & `UpyTest-3.0.3/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.0.3/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,18 +240,20 @@
             if event.get("full"):
                 self.terminate_running()
                 self.clean_treeview()          
             else:       
                 # on vérifie si le l1test a été invoqué
                 if self.is_running(): 
                     self.clean_treeview()
+                    l1test_treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
+                    l1test_treeview.insert_in_header("Starting executing tests ...", clear=True, tags="blue", image=l1test_treeview.pending_img)
                 else: # probablement une autre commande a déclenché le Restart du backend -> on fait rien
                     pass
         self.show_right_view()
-      
+     
     def show_right_view(self, event:WorkbenchEvent=None, verdicts=None, error_msg:str=None, error_title:str=None, both=False):
         """
             Displays either the L1TestTreeView or the L1TestErrorView. 
             It depends on the execution state of the l1test plugin. 
             
             If an error was raised by the plugin then only the Error view will be displayed.
         """
```

### Comparing `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.0.3/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,15 +765,15 @@
         """
         Insert in the header of the treeview a text. 
         If image is not None so the image will be added before the texte.
         """
         if clear:
             self.header_bar.direct_delete("1.0", tk.END)
         if image:
-            self.header_bar.image_create(tk.END, image=self.pending_img)
+            self.header_bar.image_create(tk.END, image=image)
             text = " " + text
         self.header_bar.direct_insert(tk.END, text, tags=tags)
         self.resize_header_bar()
            
     def is_treeview_cleared(self):
         return len(self.treeview.get_children()) == 0
```

### Comparing `UpyTest-3.0.2/thonnycontrib/outlines.py` & `UpyTest-3.0.3/thonnycontrib/outlines.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/plugin_loader.py` & `UpyTest-3.0.3/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/properties.py` & `UpyTest-3.0.3/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.0.3/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.0.3/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.0.3/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.0.3/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.0.3/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/tests/tests_view.py` & `UpyTest-3.0.3/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.0.2/thonnycontrib/utils.py` & `UpyTest-3.0.3/thonnycontrib/utils.py`

 * *Files identical despite different names*

