# Comparing `tmp/catnapmodule-0.21.tar.gz` & `tmp/catnapmodule-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnapmodule-0.21.tar", last modified: Sat Apr 29 14:31:31 2023, max compression
+gzip compressed data, was "catnapmodule-1.1.tar", last modified: Mon May  1 10:03:58 2023, max compression
```

## Comparing `catnapmodule-0.21.tar` & `catnapmodule-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 14:31:31.813988 catnapmodule-0.21/
--rw-rw-rw-   0        0        0      202 2023-04-29 14:31:31.812986 catnapmodule-0.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 14:31:31.782946 catnapmodule-0.21/catnapmodule/
--rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-0.21/catnapmodule/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-0.21/catnapmodule/chat.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:31:31.809986 catnapmodule-0.21/catnapmodule.egg-info/
--rw-rw-rw-   0        0        0      202 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-29 14:31:31.000000 catnapmodule-0.21/catnapmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 14:31:31.814989 catnapmodule-0.21/setup.cfg
--rw-rw-rw-   0        0        0      238 2023-04-29 14:31:27.000000 catnapmodule-0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:03:58.602135 catnapmodule-1.1/
+-rw-rw-rw-   0        0        0      527 2023-05-01 10:03:58.603135 catnapmodule-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-01 09:59:23.000000 catnapmodule-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 10:03:58.575296 catnapmodule-1.1/catnapmodule/
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-1.1/catnapmodule/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-1.1/catnapmodule/chat.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:03:58.600134 catnapmodule-1.1/catnapmodule.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:03:58.606138 catnapmodule-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      288 2023-05-01 10:03:56.000000 catnapmodule-1.1/setup.py
```

