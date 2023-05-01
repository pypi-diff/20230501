# Comparing `tmp/autoLinker-1.0.1.tar.gz` & `tmp/autoLinker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\autoLinker-1.0.1.tar", last modified: Sun Apr 30 10:24:24 2023, max compression
+gzip compressed data, was "dist\autoLinker-1.0.2.tar", last modified: Mon May  1 10:14:45 2023, max compression
```

## Comparing `autoLinker-1.0.1.tar` & `autoLinker-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:24:24.000000 autoLinker-1.0.1/
--rw-rw-rw-   0        0        0      202 2023-04-30 10:24:24.000000 autoLinker-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 10:24:24.000000 autoLinker-1.0.1/autoLinker.egg-info/
--rw-rw-rw-   0        0        0      202 2023-04-30 10:24:24.000000 autoLinker-1.0.1/autoLinker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-30 10:24:24.000000 autoLinker-1.0.1/autoLinker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:24:24.000000 autoLinker-1.0.1/autoLinker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-30 10:24:24.000000 autoLinker-1.0.1/autoLinker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-30 10:24:24.000000 autoLinker-1.0.1/autoLinker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 10:24:24.000000 autoLinker-1.0.1/main/
--rw-rw-rw-   0        0        0       47 2023-04-30 06:40:47.000000 autoLinker-1.0.1/main/__init__.py
--rw-rw-rw-   0        0        0      434 2023-04-30 09:40:42.000000 autoLinker-1.0.1/main/file.py
--rw-rw-rw-   0        0        0       42 2023-04-30 10:24:24.000000 autoLinker-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-04-30 10:23:40.000000 autoLinker-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:45.000000 autoLinker-1.0.2/
+-rw-rw-rw-   0        0        0      229 2023-05-01 10:14:45.000000 autoLinker-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:45.000000 autoLinker-1.0.2/autoLinker/
+-rw-rw-rw-   0        0        0       96 2023-04-30 11:06:14.000000 autoLinker-1.0.2/autoLinker/__init__.py
+-rw-rw-rw-   0        0        0      434 2023-04-30 09:40:42.000000 autoLinker-1.0.2/autoLinker/file.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:14:45.000000 autoLinker-1.0.2/autoLinker.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      587 2023-05-01 10:07:25.000000 autoLinker-1.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:14:45.000000 autoLinker-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      469 2023-05-01 10:10:31.000000 autoLinker-1.0.2/setup.py
```

