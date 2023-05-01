# Comparing `tmp/catnapmodule-1.1.tar.gz` & `tmp/catnapmodule-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnapmodule-1.1.tar", last modified: Mon May  1 10:03:58 2023, max compression
+gzip compressed data, was "catnapmodule-1.2.tar", last modified: Mon May  1 10:42:51 2023, max compression
```

## Comparing `catnapmodule-1.1.tar` & `catnapmodule-1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:03:58.602135 catnapmodule-1.1/
--rw-rw-rw-   0        0        0      527 2023-05-01 10:03:58.603135 catnapmodule-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-01 09:59:23.000000 catnapmodule-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 10:03:58.575296 catnapmodule-1.1/catnapmodule/
--rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-1.1/catnapmodule/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-1.1/catnapmodule/chat.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:03:58.600134 catnapmodule-1.1/catnapmodule.egg-info/
--rw-rw-rw-   0        0        0      527 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 10:03:58.000000 catnapmodule-1.1/catnapmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 10:03:58.606138 catnapmodule-1.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2023-05-01 10:03:56.000000 catnapmodule-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:42:51.411156 catnapmodule-1.2/
+-rw-rw-rw-   0        0        0      921 2023-05-01 10:42:51.412155 catnapmodule-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-05-01 10:42:40.000000 catnapmodule-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 10:42:51.395144 catnapmodule-1.2/catnapmodule/
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-1.2/catnapmodule/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-1.2/catnapmodule/chat.py
+-rw-rw-rw-   0        0        0      306 2023-05-01 10:40:51.000000 catnapmodule-1.2/catnapmodule/queq.py
+drwxrwxrwx   0        0        0        0 2023-05-01 10:42:51.409153 catnapmodule-1.2/catnapmodule.egg-info/
+-rw-rw-rw-   0        0        0      921 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 10:42:51.415158 catnapmodule-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      287 2023-05-01 10:40:51.000000 catnapmodule-1.2/setup.py
```

