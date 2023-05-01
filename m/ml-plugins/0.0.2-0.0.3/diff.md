# Comparing `tmp/ml_plugins-0.0.2.tar.gz` & `tmp/ml_plugins-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/grace.han/Documents/ml-plugins/dist/.tmp-lioclp9g/ml_plugins-0.0.2.tar", last modified: Mon May  1 05:50:52 2023, max compression
+gzip compressed data, was "/Users/grace.han/Documents/ml-plugins/dist/.tmp-q2rbl2n0/ml_plugins-0.0.3.tar", last modified: Mon May  1 05:55:17 2023, max compression
```

## Comparing `ml_plugins-0.0.2.tar` & `ml_plugins-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.707499 ml_plugins-0.0.2/
--rw-r--r--   0 grace.han   (503) staff       (20)       77 2023-05-01 05:50:52.707090 ml_plugins-0.0.2/PKG-INFO
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.703969 ml_plugins-0.0.2/ml_plugins.egg-info/
--rw-r--r--   0 grace.han   (503) staff       (20)       77 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/PKG-INFO
--rw-r--r--   0 grace.han   (503) staff       (20)      324 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        9 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/requires.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        8 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.704380 ml_plugins-0.0.2/plugins/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:32:14.000000 ml_plugins-0.0.2/plugins/__init__.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.705147 ml_plugins-0.0.2/plugins/pip/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.2/plugins/pip/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.2/plugins/pip/pip.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.706550 ml_plugins-0.0.2/plugins/poetry/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.2/plugins/poetry/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.2/plugins/poetry/example.py
--rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-04-27 03:25:00.000000 ml_plugins-0.0.2/plugins/poetry/plugin.py
--rw-r--r--   0 grace.han   (503) staff       (20)      109 2023-05-01 05:50:47.000000 ml_plugins-0.0.2/pyproject.toml
--rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 05:50:52.707633 ml_plugins-0.0.2/setup.cfg
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:55:17.376682 ml_plugins-0.0.3/
+-rw-r--r--   0 grace.han   (503) staff       (20)       77 2023-05-01 05:55:17.376124 ml_plugins-0.0.3/PKG-INFO
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:55:17.369356 ml_plugins-0.0.3/plugins/
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:55:17.372338 ml_plugins-0.0.3/plugins/ml_plugins.egg-info/
+-rw-r--r--   0 grace.han   (503) staff       (20)       77 2023-05-01 05:55:17.000000 ml_plugins-0.0.3/plugins/ml_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 grace.han   (503) staff       (20)      344 2023-05-01 05:55:17.000000 ml_plugins-0.0.3/plugins/ml_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 05:55:17.000000 ml_plugins-0.0.3/plugins/ml_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        9 2023-05-01 05:55:17.000000 ml_plugins-0.0.3/plugins/ml_plugins.egg-info/requires.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)       11 2023-05-01 05:55:17.000000 ml_plugins-0.0.3/plugins/ml_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:55:17.373216 ml_plugins-0.0.3/plugins/pip/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.3/plugins/pip/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.3/plugins/pip/pip.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:55:17.374885 ml_plugins-0.0.3/plugins/poetry/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.3/plugins/poetry/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.3/plugins/poetry/example.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-04-27 03:25:00.000000 ml_plugins-0.0.3/plugins/poetry/plugin.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      162 2023-05-01 05:55:09.000000 ml_plugins-0.0.3/pyproject.toml
+-rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 05:55:17.376873 ml_plugins-0.0.3/setup.cfg
```

### Comparing `ml_plugins-0.0.2/plugins/poetry/plugin.py` & `ml_plugins-0.0.3/plugins/poetry/plugin.py`

 * *Files identical despite different names*

