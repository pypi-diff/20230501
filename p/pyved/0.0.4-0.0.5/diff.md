# Comparing `tmp/pyved-0.0.4.tar.gz` & `tmp/pyved-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-0.0.4.tar", last modified: Mon May  1 12:49:40 2023, max compression
+gzip compressed data, was "pyved-0.0.5.tar", last modified: Mon May  1 19:29:00 2023, max compression
```

## Comparing `pyved-0.0.4.tar` & `pyved-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.162005 pyved-0.0.4/
--rw-rw-rw-   0        0        0      700 2023-05-01 12:49:40.162005 pyved-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-04-27 15:35:58.000000 pyved-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 12:49:40.162005 pyved-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-05-01 12:12:44.000000 pyved-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.130622 pyved-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.146348 pyved-0.0.4/src/pyved/
--rw-rw-rw-   0        0        0        0 2023-04-02 10:28:27.000000 pyved-0.0.4/src/pyved/__init__.py
--rw-rw-rw-   0        0        0     3096 2023-05-01 12:18:11.000000 pyved-0.0.4/src/pyved/__main__.py
--rw-rw-rw-   0        0        0     1981 2023-05-01 11:45:38.000000 pyved-0.0.4/src/pyved/editor.py
--rw-rw-rw-   0        0        0      526 2023-04-27 16:07:20.000000 pyved-0.0.4/src/pyved/test.py
--rw-rw-rw-   0        0        0       23 2023-05-01 11:24:01.000000 pyved-0.0.4/src/pyved/ver_info.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.162005 pyved-0.0.4/src/pyved.egg-info/
--rw-rw-rw-   0        0        0      700 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.052037 pyved-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-01 19:28:48.000000 pyved-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-01 19:29:00.052037 pyved-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 19:28:48.000000 pyved-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:29:00.052037 pyved-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-01 19:28:48.000000 pyved-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.048037 pyved-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.052037 pyved-0.0.5/src/pyved/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/menu_bar_ev_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/menu_bar_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 19:28:48.000000 pyved-0.0.5/src/pyved/ver_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:29:00.052037 pyved-0.0.5/src/pyved.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 19:29:00.000000 pyved-0.0.5/src/pyved.egg-info/top_level.txt
```

### Comparing `pyved-0.0.4/setup.py` & `pyved-0.0.5/setup.py`

 * *Files identical despite different names*

