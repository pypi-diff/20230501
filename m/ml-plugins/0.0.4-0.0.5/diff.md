# Comparing `tmp/ml_plugins-0.0.4.tar.gz` & `tmp/ml_plugins-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_plugins-0.0.4.tar", last modified: Mon May  1 06:10:59 2023, max compression
+gzip compressed data, was "ml_plugins-0.0.5.tar", last modified: Mon May  1 06:16:40 2023, max compression
```

## Comparing `ml_plugins-0.0.4.tar` & `ml_plugins-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:10:59.315413 ml_plugins-0.0.4/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:10:59.314803 ml_plugins-0.0.4/PKG-INFO
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:10:59.309555 ml_plugins-0.0.4/plugins/
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:10:59.312214 ml_plugins-0.0.4/plugins/ml_plugins.egg-info/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:10:59.000000 ml_plugins-0.0.4/plugins/ml_plugins.egg-info/PKG-INFO
--rw-r--r--   0 grace.han   (503) staff       (20)      344 2023-05-01 06:10:59.000000 ml_plugins-0.0.4/plugins/ml_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 06:10:59.000000 ml_plugins-0.0.4/plugins/ml_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        9 2023-05-01 06:10:59.000000 ml_plugins-0.0.4/plugins/ml_plugins.egg-info/requires.txt
--rw-r--r--   0 grace.han   (503) staff       (20)       11 2023-05-01 06:10:59.000000 ml_plugins-0.0.4/plugins/ml_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:10:59.312974 ml_plugins-0.0.4/plugins/pip/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.4/plugins/pip/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.4/plugins/pip/pip.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:10:59.314305 ml_plugins-0.0.4/plugins/poetry/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.4/plugins/poetry/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.4/plugins/poetry/example.py
--rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-04-27 03:25:00.000000 ml_plugins-0.0.4/plugins/poetry/plugin.py
--rw-r--r--   0 grace.han   (503) staff       (20)      218 2023-05-01 06:10:50.000000 ml_plugins-0.0.4/pyproject.toml
--rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 06:10:59.315604 ml_plugins-0.0.4/setup.cfg
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:16:40.612671 ml_plugins-0.0.5/
+-rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:16:40.612323 ml_plugins-0.0.5/PKG-INFO
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:16:40.609301 ml_plugins-0.0.5/ml_plugins.egg-info/
+-rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:16:40.000000 ml_plugins-0.0.5/ml_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 grace.han   (503) staff       (20)      324 2023-05-01 06:16:40.000000 ml_plugins-0.0.5/ml_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 06:16:40.000000 ml_plugins-0.0.5/ml_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        9 2023-05-01 06:16:40.000000 ml_plugins-0.0.5/ml_plugins.egg-info/requires.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)       19 2023-05-01 06:16:40.000000 ml_plugins-0.0.5/ml_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:16:40.609690 ml_plugins-0.0.5/plugins/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 06:13:56.000000 ml_plugins-0.0.5/plugins/__init__.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:16:40.610577 ml_plugins-0.0.5/plugins/pip/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.5/plugins/pip/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.5/plugins/pip/pip.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:16:40.611866 ml_plugins-0.0.5/plugins/poetry/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.5/plugins/poetry/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.5/plugins/poetry/example.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-05-01 06:11:28.000000 ml_plugins-0.0.5/plugins/poetry/plugin.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      260 2023-05-01 06:15:19.000000 ml_plugins-0.0.5/pyproject.toml
+-rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 06:16:40.612777 ml_plugins-0.0.5/setup.cfg
```

### Comparing `ml_plugins-0.0.4/plugins/poetry/plugin.py` & `ml_plugins-0.0.5/plugins/poetry/plugin.py`

 * *Files identical despite different names*

