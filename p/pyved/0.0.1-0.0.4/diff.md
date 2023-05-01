# Comparing `tmp/pyved-0.0.1.tar.gz` & `tmp/pyved-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyved-0.0.1.tar", last modified: Thu Apr 27 15:45:36 2023, max compression
+gzip compressed data, was "pyved-0.0.4.tar", last modified: Mon May  1 12:49:40 2023, max compression
```

## Comparing `pyved-0.0.1.tar` & `pyved-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:45:36.431776 pyved-0.0.1/
--rw-rw-rw-   0        0        0      236 2023-04-27 15:45:36.431776 pyved-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-04-27 15:35:58.000000 pyved-0.0.1/README.md
--rw-rw-rw-   0        0        0      383 2023-04-27 15:34:09.000000 pyved-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 15:45:36.431776 pyved-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      444 2023-04-27 15:45:30.000000 pyved-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:45:36.415792 pyved-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 15:45:36.415792 pyved-0.0.1/src/pyved/
--rw-rw-rw-   0        0        0        0 2023-04-02 10:28:27.000000 pyved-0.0.1/src/pyved/__init__.py
--rw-rw-rw-   0        0        0       24 2023-04-02 10:28:27.000000 pyved-0.0.1/src/pyved/test.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:45:36.431776 pyved-0.0.1/src/pyved.egg-info/
--rw-rw-rw-   0        0        0      236 2023-04-27 15:45:36.000000 pyved-0.0.1/src/pyved.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-27 15:45:36.000000 pyved-0.0.1/src/pyved.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:45:36.000000 pyved-0.0.1/src/pyved.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 15:45:36.000000 pyved-0.0.1/src/pyved.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.162005 pyved-0.0.4/
+-rw-rw-rw-   0        0        0      700 2023-05-01 12:49:40.162005 pyved-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-04-27 15:35:58.000000 pyved-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 12:49:40.162005 pyved-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-05-01 12:12:44.000000 pyved-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.130622 pyved-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.146348 pyved-0.0.4/src/pyved/
+-rw-rw-rw-   0        0        0        0 2023-04-02 10:28:27.000000 pyved-0.0.4/src/pyved/__init__.py
+-rw-rw-rw-   0        0        0     3096 2023-05-01 12:18:11.000000 pyved-0.0.4/src/pyved/__main__.py
+-rw-rw-rw-   0        0        0     1981 2023-05-01 11:45:38.000000 pyved-0.0.4/src/pyved/editor.py
+-rw-rw-rw-   0        0        0      526 2023-04-27 16:07:20.000000 pyved-0.0.4/src/pyved/test.py
+-rw-rw-rw-   0        0        0       23 2023-05-01 11:24:01.000000 pyved-0.0.4/src/pyved/ver_info.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:49:40.162005 pyved-0.0.4/src/pyved.egg-info/
+-rw-rw-rw-   0        0        0      700 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 12:49:40.000000 pyved-0.0.4/src/pyved.egg-info/top_level.txt
```

