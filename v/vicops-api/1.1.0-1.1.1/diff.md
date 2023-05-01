# Comparing `tmp/vicops_api-1.1.0.tar.gz` & `tmp/vicops_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicops_api-1.1.0.tar", last modified: Sat Apr 22 07:33:21 2023, max compression
+gzip compressed data, was "vicops_api-1.1.1.tar", max compression
```

## Comparing `vicops_api-1.1.0.tar` & `vicops_api-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 07:33:21.952947 vicops_api-1.1.0/
--rw-rw-rw-   0        0        0     1083 2023-03-04 14:34:18.000000 vicops_api-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      527 2023-04-22 07:33:21.952947 vicops_api-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-03-04 15:36:21.000000 vicops_api-1.1.0/README.md
--rw-rw-rw-   0        0        0       99 2023-03-04 15:18:20.000000 vicops_api-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 07:33:21.952947 vicops_api-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-04-22 07:32:47.000000 vicops_api-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 07:33:21.945948 vicops_api-1.1.0/vicops_api/
--rw-rw-rw-   0        0        0      126 2023-04-22 07:32:40.000000 vicops_api-1.1.0/vicops_api/__init__.py
--rw-rw-rw-   0        0        0     4948 2023-04-22 07:32:04.000000 vicops_api-1.1.0/vicops_api/main.py
-drwxrwxrwx   0        0        0        0 2023-04-22 07:33:21.951948 vicops_api-1.1.0/vicops_api.egg-info/
--rw-rw-rw-   0        0        0      527 2023-04-22 07:33:21.000000 vicops_api-1.1.0/vicops_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-22 07:33:21.000000 vicops_api-1.1.0/vicops_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:33:21.000000 vicops_api-1.1.0/vicops_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 07:33:21.000000 vicops_api-1.1.0/vicops_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 07:33:21.000000 vicops_api-1.1.0/vicops_api.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1083 2023-03-04 14:34:18.067932 vicops_api-1.1.1/LICENSE
+-rw-r--r--   0        0        0      473 2023-05-01 10:41:19.382156 vicops_api-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-03-04 15:36:21.112213 vicops_api-1.1.1/README.md
+-rw-r--r--   0        0        0      126 2023-04-22 07:32:40.143497 vicops_api-1.1.1/vicops_api/__init__.py
+-rw-r--r--   0        0        0     4948 2023-04-22 07:32:04.216209 vicops_api-1.1.1/vicops_api/main.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 vicops_api-1.1.1/PKG-INFO
```

### Comparing `vicops_api-1.1.0/LICENSE` & `vicops_api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vicops_api-1.1.0/vicops_api/main.py` & `vicops_api-1.1.1/vicops_api/main.py`

 * *Files identical despite different names*

