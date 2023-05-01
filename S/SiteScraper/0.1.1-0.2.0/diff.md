# Comparing `tmp/SiteScraper-0.1.1.tar.gz` & `tmp/SiteScraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-0.1.1.tar", last modified: Mon May  1 16:57:25 2023, max compression
+gzip compressed data, was "SiteScraper-0.2.0.tar", last modified: Mon May  1 18:02:04 2023, max compression
```

## Comparing `SiteScraper-0.1.1.tar` & `SiteScraper-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 16:57:25.459073 SiteScraper-0.1.1/
--rw-rw-rw-   0        0        0      159 2023-05-01 16:57:25.458075 SiteScraper-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 16:57:25.451093 SiteScraper-0.1.1/SiteScraper/
--rw-rw-rw-   0        0        0     7864 2023-05-01 15:59:21.000000 SiteScraper-0.1.1/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       33 2023-04-30 14:41:47.000000 SiteScraper-0.1.1/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 16:57:25.457075 SiteScraper-0.1.1/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-01 16:57:25.000000 SiteScraper-0.1.1/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-01 16:57:25.000000 SiteScraper-0.1.1/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 16:57:25.000000 SiteScraper-0.1.1/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 16:57:25.000000 SiteScraper-0.1.1/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 16:57:25.000000 SiteScraper-0.1.1/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 16:57:25.459073 SiteScraper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-05-01 16:01:22.000000 SiteScraper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 18:02:04.676737 SiteScraper-0.2.0/
+-rw-rw-rw-   0        0        0      159 2023-05-01 18:02:04.675739 SiteScraper-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 18:02:04.667762 SiteScraper-0.2.0/SiteScraper/
+-rw-rw-rw-   0        0        0     7864 2023-05-01 15:59:21.000000 SiteScraper-0.2.0/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       33 2023-04-30 14:41:47.000000 SiteScraper-0.2.0/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 18:02:04.674743 SiteScraper-0.2.0/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 18:02:04.000000 SiteScraper-0.2.0/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 18:02:04.676737 SiteScraper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      341 2023-05-01 17:58:01.000000 SiteScraper-0.2.0/setup.py
```

### Comparing `SiteScraper-0.1.1/SiteScraper/SiteScraper.py` & `SiteScraper-0.2.0/SiteScraper/SiteScraper.py`

 * *Files identical despite different names*

