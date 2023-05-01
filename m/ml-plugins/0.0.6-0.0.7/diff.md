# Comparing `tmp/ml_plugins-0.0.6.tar.gz` & `tmp/ml_plugins-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_plugins-0.0.6.tar", last modified: Mon May  1 06:31:19 2023, max compression
+gzip compressed data, was "ml_plugins-0.0.7.tar", last modified: Mon May  1 06:43:31 2023, max compression
```

## Comparing `ml_plugins-0.0.6.tar` & `ml_plugins-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:31:19.376872 ml_plugins-0.0.6/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:31:19.376438 ml_plugins-0.0.6/PKG-INFO
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:31:19.368768 ml_plugins-0.0.6/plugins/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 06:13:56.000000 ml_plugins-0.0.6/plugins/__init__.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:31:19.370978 ml_plugins-0.0.6/plugins/ml_plugins.egg-info/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:31:19.000000 ml_plugins-0.0.6/plugins/ml_plugins.egg-info/PKG-INFO
--rw-r--r--   0 grace.han   (503) staff       (20)      364 2023-05-01 06:31:19.000000 ml_plugins-0.0.6/plugins/ml_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 06:31:19.000000 ml_plugins-0.0.6/plugins/ml_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 grace.han   (503) staff       (20)       16 2023-05-01 06:31:19.000000 ml_plugins-0.0.6/plugins/ml_plugins.egg-info/requires.txt
--rw-r--r--   0 grace.han   (503) staff       (20)       20 2023-05-01 06:31:19.000000 ml_plugins-0.0.6/plugins/ml_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:31:19.372099 ml_plugins-0.0.6/plugins/pip/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.6/plugins/pip/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.6/plugins/pip/pip.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:31:19.375652 ml_plugins-0.0.6/plugins/poetry/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.6/plugins/poetry/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.6/plugins/poetry/example.py
--rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-05-01 06:11:28.000000 ml_plugins-0.0.6/plugins/poetry/plugin.py
--rw-r--r--   0 grace.han   (503) staff       (20)      220 2023-05-01 06:30:18.000000 ml_plugins-0.0.6/pyproject.toml
--rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 06:31:19.376992 ml_plugins-0.0.6/setup.cfg
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.875936 ml_plugins-0.0.7/
+-rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:43:31.875558 ml_plugins-0.0.7/PKG-INFO
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.872317 ml_plugins-0.0.7/ml_plugins.egg-info/
+-rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 grace.han   (503) staff       (20)      324 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)       23 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/requires.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)       19 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.872717 ml_plugins-0.0.7/plugins/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 06:13:56.000000 ml_plugins-0.0.7/plugins/__init__.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.873556 ml_plugins-0.0.7/plugins/pip/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.7/plugins/pip/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.7/plugins/pip/pip.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.874903 ml_plugins-0.0.7/plugins/poetry/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.7/plugins/poetry/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.7/plugins/poetry/example.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      448 2023-05-01 06:38:58.000000 ml_plugins-0.0.7/plugins/poetry/plugin.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      281 2023-05-01 06:43:22.000000 ml_plugins-0.0.7/pyproject.toml
+-rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 06:43:31.876091 ml_plugins-0.0.7/setup.cfg
```

