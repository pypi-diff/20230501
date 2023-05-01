# Comparing `tmp/widgets-lib-2.7.2.tar.gz` & `tmp/widgets-lib-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgets-lib-2.7.2.tar", last modified: Thu Apr 20 16:30:29 2023, max compression
+gzip compressed data, was "widgets-lib-2.7.3.tar", last modified: Mon May  1 20:55:01 2023, max compression
```

## Comparing `widgets-lib-2.7.2.tar` & `widgets-lib-2.7.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/base/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/st_base/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/st_base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/st_base/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.834292 widgets-lib-2.7.2/src/widgets/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/expander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/files/download_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/selectstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/resource/values/textarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/streamlit/widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/streamlit/widget/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/streamlit_single.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/streamlit_single.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/src/widgets/templates/streamlit_single_ga.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.838292 widgets-lib-2.7.2/src/widgets_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 16:30:29.000000 widgets-lib-2.7.2/src/widgets_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:30:29.842292 widgets-lib-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_source_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-04-20 16:29:54.000000 widgets-lib-2.7.2/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.864685 widgets-lib-2.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/st_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/st_base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/st_base/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.872686 widgets-lib-2.7.3/src/widgets/streamlit/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/expander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.872686 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/download_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/selectstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/textarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets/streamlit/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/widget/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/streamlit_single.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/streamlit_single.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/streamlit_single_ga.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_source_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_streamlit.py
```

### Comparing `widgets-lib-2.7.2/LICENSE` & `widgets-lib-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/PKG-INFO` & `widgets-lib-2.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.2
+Version: 2.7.3
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.2/README.md` & `widgets-lib-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/pyproject.toml` & `widgets-lib-2.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/base/exceptions.py` & `widgets-lib-2.7.3/src/widgets/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/base/helpers.py` & `widgets-lib-2.7.3/src/widgets/base/helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/base/io.py` & `widgets-lib-2.7.3/src/widgets/base/io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/base/resource.py` & `widgets-lib-2.7.3/src/widgets/base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/base/widget.py` & `widgets-lib-2.7.3/src/widgets/base/widget.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/cli/main.py` & `widgets-lib-2.7.3/src/widgets/cli/main.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/st_base/resource.py` & `widgets-lib-2.7.3/src/widgets/st_base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/st_base/value.py` & `widgets-lib-2.7.3/src/widgets/st_base/value.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/__init__.py` & `widgets-lib-2.7.3/src/widgets/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/columns.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/columns.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/duplicator.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/expander.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/expander.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/files/base.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/files/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/files/dataframe.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/files/dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/files/download_dataframe.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/files/download_dataframe.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 from widgets.base.exceptions import ResourceConfigurationException
 from widgets.streamlit.resource.values.slider import StValue
 
 
 class StDownloadDataFrame(StValue):
     """Download button for an StDataFrame."""
 
+    index = None
+
     def __init__(
         self,
         target: Union[str, None] = None,
         label="",
-        sidebar=True
+        sidebar=True,
+        index=None
     ):
         """
         Args:
             target (str):   The id of the StDataFrame to be downloaded.
             label (str):    (optional) Label used for download button.
             sidebar (bool): Set up UI in the sidebar vs. the main container
 
@@ -33,29 +36,30 @@
             label = f"Download {target.title()}"
 
         # Set up the resource attributes
         super().__init__(
             id=id,
             label=label,
             help="",
-            value=None
+            value=None,
+            index=index
         )
 
         # Set up the specific attributes for this type of resource
         self.target = target
         self.sidebar = sidebar
 
     def run_self(self):
         """Give the user a button to download a DataFrame."""
 
         # Point to the target
         target = self.parent._get_child(self.target)
 
         # Get the value of the table
-        csv = target.value.to_csv(index=None)
+        csv = target.value.to_csv(index=self.index)
 
         self.ui_container().download_button(
             self.label,
             csv,
             file_name=f"{self.target}.csv",
             mime="text/csv",
             help="Download this table as a spreadsheet (csv)"
```

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/markdown.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/markdown.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/selector.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/selector.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/checkbox.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/float.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/float.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/integer.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/integer.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/multiselect.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/multiselect.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/selectstring.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/selectstring.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/slider.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/slider.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/string.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/string.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/resource/values/textarea.py` & `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/textarea.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/streamlit/widget/base.py` & `widgets-lib-2.7.3/src/widgets/streamlit/widget/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/templates/streamlit_single.html.j2` & `widgets-lib-2.7.3/src/widgets/templates/streamlit_single.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets/templates/streamlit_single_ga.html.j2` & `widgets-lib-2.7.3/src/widgets/templates/streamlit_single_ga.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/src/widgets_lib.egg-info/PKG-INFO` & `widgets-lib-2.7.3/src/widgets_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.2
+Version: 2.7.3
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.2/src/widgets_lib.egg-info/SOURCES.txt` & `widgets-lib-2.7.3/src/widgets_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_base.py` & `widgets-lib-2.7.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_cli.py` & `widgets-lib-2.7.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_duplicator.py` & `widgets-lib-2.7.3/tests/test_duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_helpers.py` & `widgets-lib-2.7.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_io.py` & `widgets-lib-2.7.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_source_parents.py` & `widgets-lib-2.7.3/tests/test_source_parents.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.2/tests/test_streamlit.py` & `widgets-lib-2.7.3/tests/test_streamlit.py`

 * *Files identical despite different names*

