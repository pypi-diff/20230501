# Comparing `tmp/owo_info-0.0.0.tar.gz` & `tmp/owo_info-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\owo_info-0.0.0.tar", last modified: Mon May  1 09:41:45 2023, max compression
+gzip compressed data, was "owo_info-0.0.1.tar", last modified: Mon May  1 09:52:56 2023, max compression
```

## Comparing `owo_info-0.0.0.tar` & `owo_info-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:41:45.585789 owo_info-0.0.0/
--rw-rw-rw-   0        0        0       55 2023-05-01 09:41:45.584032 owo_info-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 09:41:45.570724 owo_info-0.0.0/owo_info/
--rw-rw-rw-   0        0        0      115 2023-05-01 09:39:55.000000 owo_info-0.0.0/owo_info/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 09:41:45.581081 owo_info-0.0.0/owo_info.egg-info/
--rw-rw-rw-   0        0        0       55 2023-05-01 09:41:45.000000 owo_info-0.0.0/owo_info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-01 09:41:45.000000 owo_info-0.0.0/owo_info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:41:45.000000 owo_info-0.0.0/owo_info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 09:41:45.000000 owo_info-0.0.0/owo_info.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 09:41:45.585789 owo_info-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       79 2023-05-01 09:40:54.000000 owo_info-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:52:56.510903 owo_info-0.0.1/
+-rw-rw-rw-   0        0        0      143 2023-05-01 09:52:56.509498 owo_info-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 09:52:56.493181 owo_info-0.0.1/owo_info/
+-rw-rw-rw-   0        0        0      114 2023-05-01 09:52:15.000000 owo_info-0.0.1/owo_info/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:52:56.506420 owo_info-0.0.1/owo_info.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-05-01 09:52:56.000000 owo_info-0.0.1/owo_info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-01 09:52:56.000000 owo_info-0.0.1/owo_info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:52:56.000000 owo_info-0.0.1/owo_info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:52:56.000000 owo_info-0.0.1/owo_info.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:52:56.511405 owo_info-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      101 2023-05-01 09:52:51.000000 owo_info-0.0.1/setup.py
```

