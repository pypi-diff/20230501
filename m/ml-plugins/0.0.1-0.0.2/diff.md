# Comparing `tmp/ml_plugins-0.0.1.tar.gz` & `tmp/ml_plugins-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/grace.han/Documents/ml-plugins/dist/.tmp-d7erf23f/ml_plugins-0.0.1.tar", last modified: Mon May  1 05:20:49 2023, max compression
+gzip compressed data, was "/Users/grace.han/Documents/ml-plugins/dist/.tmp-lioclp9g/ml_plugins-0.0.2.tar", last modified: Mon May  1 05:50:52 2023, max compression
```

## Comparing `ml_plugins-0.0.1.tar` & `ml_plugins-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:20:49.175960 ml_plugins-0.0.1/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 05:20:49.175638 ml_plugins-0.0.1/PKG-INFO
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:20:49.173580 ml_plugins-0.0.1/ml_plugins.egg-info/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 05:20:49.000000 ml_plugins-0.0.1/ml_plugins.egg-info/PKG-INFO
--rw-r--r--   0 grace.han   (503) staff       (20)      281 2023-05-01 05:20:49.000000 ml_plugins-0.0.1/ml_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 05:20:49.000000 ml_plugins-0.0.1/ml_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        9 2023-05-01 05:20:49.000000 ml_plugins-0.0.1/ml_plugins.egg-info/requires.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        8 2023-05-01 05:20:49.000000 ml_plugins-0.0.1/ml_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:20:49.174031 ml_plugins-0.0.1/plugins/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:32:14.000000 ml_plugins-0.0.1/plugins/__init__.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:20:49.175179 ml_plugins-0.0.1/plugins/poetry/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.1/plugins/poetry/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.1/plugins/poetry/example.py
--rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-04-27 03:25:00.000000 ml_plugins-0.0.1/plugins/poetry/plugin.py
--rw-r--r--   0 grace.han   (503) staff       (20)       81 2023-05-01 05:14:46.000000 ml_plugins-0.0.1/pyproject.toml
--rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 05:20:49.176076 ml_plugins-0.0.1/setup.cfg
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.707499 ml_plugins-0.0.2/
+-rw-r--r--   0 grace.han   (503) staff       (20)       77 2023-05-01 05:50:52.707090 ml_plugins-0.0.2/PKG-INFO
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.703969 ml_plugins-0.0.2/ml_plugins.egg-info/
+-rw-r--r--   0 grace.han   (503) staff       (20)       77 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 grace.han   (503) staff       (20)      324 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        9 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/requires.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        8 2023-05-01 05:50:52.000000 ml_plugins-0.0.2/ml_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.704380 ml_plugins-0.0.2/plugins/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:32:14.000000 ml_plugins-0.0.2/plugins/__init__.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.705147 ml_plugins-0.0.2/plugins/pip/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.2/plugins/pip/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.2/plugins/pip/pip.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 05:50:52.706550 ml_plugins-0.0.2/plugins/poetry/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.2/plugins/poetry/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.2/plugins/poetry/example.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      593 2023-04-27 03:25:00.000000 ml_plugins-0.0.2/plugins/poetry/plugin.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      109 2023-05-01 05:50:47.000000 ml_plugins-0.0.2/pyproject.toml
+-rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 05:50:52.707633 ml_plugins-0.0.2/setup.cfg
```

### Comparing `ml_plugins-0.0.1/plugins/poetry/plugin.py` & `ml_plugins-0.0.2/plugins/poetry/plugin.py`

 * *Files identical despite different names*

