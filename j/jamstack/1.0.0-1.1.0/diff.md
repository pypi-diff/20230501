# Comparing `tmp/jamstack-1.0.0.tar.gz` & `tmp/jamstack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamstack-1.0.0.tar", last modified: Sat Feb 26 16:39:39 2022, max compression
+gzip compressed data, was "jamstack-1.1.0.tar", last modified: Mon May  1 12:09:39 2023, max compression
```

## Comparing `jamstack-1.0.0.tar` & `jamstack-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.981547 jamstack-1.0.0/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)    11357 2022-02-26 14:17:47.000000 jamstack-1.0.0/LICENSE
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)       54 2022-02-26 14:17:47.000000 jamstack-1.0.0/MANIFEST.in
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2591 2022-02-26 16:39:39.981547 jamstack-1.0.0/PKG-INFO
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1774 2022-02-26 15:43:08.000000 jamstack-1.0.0/README.md
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)       80 2022-02-26 16:24:41.000000 jamstack-1.0.0/jamstack/__init__.py
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1306 2022-02-26 14:46:51.000000 jamstack-1.0.0/jamstack/__main__.py
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/__pycache__/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      339 2022-02-26 16:27:33.000000 jamstack-1.0.0/jamstack/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1475 2022-02-26 15:21:49.000000 jamstack-1.0.0/jamstack/__pycache__/__main__.cpython-39.pyc
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/api/
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/api/__pycache__/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     3122 2022-02-26 15:21:49.000000 jamstack-1.0.0/jamstack/api/__pycache__/file.cpython-39.pyc
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1671 2022-02-26 15:22:03.000000 jamstack-1.0.0/jamstack/api/__pycache__/template.cpython-39.pyc
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2525 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/api/file.py
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1359 2022-02-26 14:52:13.000000 jamstack-1.0.0/jamstack/api/template.py
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/jamdo/
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/jamdo/__pycache__/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1941 2022-02-26 15:26:10.000000 jamstack-1.0.0/jamstack/jamdo/__pycache__/jamdo.cpython-39.pyc
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2023 2022-02-26 15:26:07.000000 jamstack-1.0.0/jamstack/jamdo/jamdo.py
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.973548 jamstack-1.0.0/jamstack/sites/
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.973548 jamstack-1.0.0/jamstack/sites/html5up/
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/sites/html5up/massively/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)       88 2022-02-26 15:04:40.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/info.json
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      338 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/settings.py
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1434 2022-02-26 15:05:30.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/static.py
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      882 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/index.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      882 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/index2.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      882 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/index3.html
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      363 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/bottom_scripts.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1570 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/footer.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      296 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/head_content.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2040 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/main.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      738 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/nav.html
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack/sites/html5up/phantom/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1945 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/info.json
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     3318 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/posts.json
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      172 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/settings.py
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1735 2022-02-26 15:06:22.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/static.py
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.981547 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)    18073 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/elements.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2994 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/generic.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2337 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/index.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2617 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/post_template.html
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.981547 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/sections/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      233 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/sections/bottom_scripts.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1102 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/sections/footer.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      471 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/sections/head_content.html
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.981547 jamstack-1.0.0/jamstack/sites/plain/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      137 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/plain/info.json
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      103 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/plain/settings.py
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1073 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/plain/static.py
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.981547 jamstack-1.0.0/jamstack/sites/plain/templates/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      157 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/plain/templates/index.html
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.981547 jamstack-1.0.0/jamstack/sites/plain/templates/sections/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      134 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/plain/templates/sections/body.html
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      543 2022-02-26 14:17:47.000000 jamstack-1.0.0/jamstack/sites/plain/templates/sections/head.html
-drwxrwxr-x   0 jalkhov   (1000) jalkhov   (1000)        0 2022-02-26 16:39:39.977547 jamstack-1.0.0/jamstack.egg-info/
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2591 2022-02-26 16:39:39.000000 jamstack-1.0.0/jamstack.egg-info/PKG-INFO
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     2052 2022-02-26 16:39:39.000000 jamstack-1.0.0/jamstack.egg-info/SOURCES.txt
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)        1 2022-02-26 16:39:39.000000 jamstack-1.0.0/jamstack.egg-info/dependency_links.txt
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)       53 2022-02-26 16:39:39.000000 jamstack-1.0.0/jamstack.egg-info/entry_points.txt
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      168 2022-02-26 16:39:39.000000 jamstack-1.0.0/jamstack.egg-info/requires.txt
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)        9 2022-02-26 16:39:39.000000 jamstack-1.0.0/jamstack.egg-info/top_level.txt
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)      168 2022-02-26 14:43:53.000000 jamstack-1.0.0/requirements.txt
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)       79 2022-02-26 16:39:39.981547 jamstack-1.0.0/setup.cfg
--rw-rw-r--   0 jalkhov   (1000) jalkhov   (1000)     1524 2022-02-26 16:34:24.000000 jamstack-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.703364 jamstack-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-10 03:39:52.000000 jamstack-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-04-10 03:39:52.000000 jamstack-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3623 2023-05-01 12:09:39.703364 jamstack-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2719 2023-04-18 11:35:59.000000 jamstack-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.640465 jamstack-1.1.0/jamstack/
+-rw-rw-rw-   0        0        0       72 2023-04-18 03:05:47.000000 jamstack-1.1.0/jamstack/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-04-10 22:29:48.000000 jamstack-1.1.0/jamstack/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.656096 jamstack-1.1.0/jamstack/__pycache__/
+-rw-rw-rw-   0        0        0      249 2023-04-18 03:07:13.000000 jamstack-1.1.0/jamstack/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1423 2023-04-10 22:36:36.000000 jamstack-1.1.0/jamstack/__pycache__/__main__.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.656096 jamstack-1.1.0/jamstack/api/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.656096 jamstack-1.1.0/jamstack/api/__pycache__/
+-rw-rw-rw-   0        0        0     3925 2023-04-17 02:13:26.000000 jamstack-1.1.0/jamstack/api/__pycache__/file.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2100 2023-04-17 02:28:12.000000 jamstack-1.1.0/jamstack/api/__pycache__/template.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3306 2023-04-17 02:01:15.000000 jamstack-1.1.0/jamstack/api/file.py
+-rw-rw-rw-   0        0        0     1870 2023-04-17 02:27:56.000000 jamstack-1.1.0/jamstack/api/template.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.656096 jamstack-1.1.0/jamstack/jamdo/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.656096 jamstack-1.1.0/jamstack/jamdo/__pycache__/
+-rw-rw-rw-   0        0        0     1755 2023-04-18 02:17:08.000000 jamstack-1.1.0/jamstack/jamdo/__pycache__/jamdo.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1587 2023-04-18 02:17:05.000000 jamstack-1.1.0/jamstack/jamdo/jamdo.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.640465 jamstack-1.1.0/jamstack/sites/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.624841 jamstack-1.1.0/jamstack/sites/html5up/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.671713 jamstack-1.1.0/jamstack/sites/html5up/massively/
+-rw-rw-rw-   0        0        0       96 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/info.json
+-rw-rw-rw-   0        0        0      307 2023-04-12 11:20:30.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/settings.py
+-rw-rw-rw-   0        0        0     1486 2023-04-17 02:36:16.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/static.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.671713 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/
+-rw-rw-rw-   0        0        0      914 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/index.html
+-rw-rw-rw-   0        0        0      914 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/index2.html
+-rw-rw-rw-   0        0        0      914 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/index3.html
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.682225 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/
+-rw-rw-rw-   0        0        0      370 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/bottom_scripts.html
+-rw-rw-rw-   0        0        0     1617 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/footer.html
+-rw-rw-rw-   0        0        0      300 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/head_content.html
+-rw-rw-rw-   0        0        0     2056 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/main.html
+-rw-rw-rw-   0        0        0      751 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/nav.html
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.687733 jamstack-1.1.0/jamstack/sites/html5up/phantom/
+-rw-rw-rw-   0        0        0     2077 2023-04-12 11:12:08.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/info.json
+-rw-rw-rw-   0        0        0     3393 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/posts.json
+-rw-rw-rw-   0        0        0      132 2023-04-17 02:04:43.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/settings.py
+-rw-rw-rw-   0        0        0     1731 2023-04-18 01:26:31.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/static.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.687733 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/
+-rw-rw-rw-   0        0        0    18469 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/elements.html
+-rw-rw-rw-   0        0        0     3051 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/generic.html
+-rw-rw-rw-   0        0        0     2414 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/index.html
+-rw-rw-rw-   0        0        0     2673 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/post_template.html
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.687733 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/sections/
+-rw-rw-rw-   0        0        0      237 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/sections/bottom_scripts.html
+-rw-rw-rw-   0        0        0     1135 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/sections/footer.html
+-rw-rw-rw-   0        0        0      480 2023-04-10 03:39:52.000000 jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/sections/head_content.html
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.687733 jamstack-1.1.0/jamstack/sites/plain/
+-rw-rw-rw-   0        0        0      247 2023-04-12 11:12:04.000000 jamstack-1.1.0/jamstack/sites/plain/info.json
+-rw-rw-rw-   0        0        0      100 2023-04-12 10:43:13.000000 jamstack-1.1.0/jamstack/sites/plain/settings.py
+-rw-rw-rw-   0        0        0     1073 2023-04-17 02:34:14.000000 jamstack-1.1.0/jamstack/sites/plain/static.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.703364 jamstack-1.1.0/jamstack/sites/plain/templates/
+-rw-rw-rw-   0        0        0      170 2023-04-18 02:28:20.000000 jamstack-1.1.0/jamstack/sites/plain/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.703364 jamstack-1.1.0/jamstack/sites/plain/templates/sections/
+-rw-rw-rw-   0        0        0      113 2023-04-12 10:46:01.000000 jamstack-1.1.0/jamstack/sites/plain/templates/sections/body.html
+-rw-rw-rw-   0        0        0      664 2023-04-12 10:40:27.000000 jamstack-1.1.0/jamstack/sites/plain/templates/sections/head.html
+drwxrwxrwx   0        0        0        0 2023-05-01 12:09:39.656096 jamstack-1.1.0/jamstack.egg-info/
+-rw-rw-rw-   0        0        0     3623 2023-05-01 12:09:39.000000 jamstack-1.1.0/jamstack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2052 2023-05-01 12:09:39.000000 jamstack-1.1.0/jamstack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 12:09:39.000000 jamstack-1.1.0/jamstack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-01 12:09:39.000000 jamstack-1.1.0/jamstack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-05-01 12:09:39.000000 jamstack-1.1.0/jamstack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 12:09:39.000000 jamstack-1.1.0/jamstack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-04-18 11:27:33.000000 jamstack-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-01 12:09:39.703364 jamstack-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1587 2023-04-18 11:26:51.000000 jamstack-1.1.0/setup.py
```

### Comparing `jamstack-1.0.0/LICENSE` & `jamstack-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `jamstack-1.0.0/README.md` & `jamstack-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <div align="center">
   <img alt="Jamstack logo" src="https://i.imgur.com/sXUAdYJ.png" height="217" />
 </div>
 
-
 ![](https://img.shields.io/pypi/v/jamstack)
 
-Also known as Jamstackpy
+Also known as Jamstackpy, is a tool that allows you to create static websites using the power of **Python** hand in hand
+with the [Flask](https://github.com/pallets/flask) library. Its operation is based on templates which are rendered with
+the powerful Jinja engine generating your website with all its dependencies.
 
 ## Installation
 
 ```bash
 python -m pip install jamstack
 ```
 
@@ -19,43 +20,56 @@
 jamstack plain <foldername>
 ```
 
 ## Templates
 
 Jamstack has templates available courtesy of [html5up](https://html5up.net).
 
-| Template                                   | Command           | Tutorial                                                     |
-| ------------------------------------------ | ----------------- | ------------------------------------------------------------ |
-| [Massively](https://html5up.net/massively) | html5up/massively |                                                              |
+| Template                                   | Command           | Tutorial                                                                 |
+|--------------------------------------------|-------------------|--------------------------------------------------------------------------|
+| [Massively](https://html5up.net/massively) | html5up/massively |                                                                          |
 | [Phantom](https://html5up.net/phantom)     | html5up/phantom   | [**HERE**](https://github.com/jamstackpy/jamstack/wiki/Phantom-template) |
 
 The syntax is as follows:
 
 ```bash
-jamstack t <template> <foldername>
+jamstack t <template_command> <project_folder_name>
 ```
 
 Use the `--existing` flag if you want the project to be created in an existing folder
 
 ```bash
 jamstack t html5up/massively myproject --existing
 ```
 
-By default, projects are created without the assets (stylesheets, images, etc...) to download them, you must pass the `--jamdo` option to the `static.py` file of the respective project.
+By default, projects based in templates are created without the assets (stylesheets, images, etc...) to download them,
+you must pass
+the `--jamdo` option to the `static.py` file of the respective project.
 
 ## Build
 
 To build the site run the file `static.py`.
 
 ```bash
 python static.py
 ```
 
 Your site will be generated in the **dist/** folder.
 
-Alternatively you can use the `--server` flag if you want to start livewatch.
+## Other project command-line options
+
+| Argument  | Description                                                               |
+|-----------|---------------------------------------------------------------------------|
+| `--serve` | Optional. Start project livewatch (autoreload when files change).         |
+| `--watch` | Optional. Specify files and folders to watch. Must be separated by comma. |
+| `--port`  | Optional. Specify server port.                                            |
 
 ## Sites using jamstack
 
 - [DeliciousPy Telegram Channel](https://deliciouspy.github.io/)
 - [The Flask Community Work Group](https://flaskcwg.github.io/)
-- [A Personal Site](https://compileralchemy.github.io/)
+- [Abdur-Rahmaan Janhangeer](https://compileralchemy.github.io/)
+
+# TODO
+
+- [ ] Replace `python static.py --serve/--jamdo` by something like `jamstack --serve/--jamdo`
+- [ ] Remove Flask as Main requirement and just use Jinja
```

### Comparing `jamstack-1.0.0/jamstack/__pycache__/__main__.cpython-39.pyc` & `jamstack-1.1.0/jamstack/__pycache__/__main__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Feb 26 14:46:51 2022 UTC, .py size: 1306 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5b3d 1a62 1a05 0000  a.......[=.b....
+00000000: 550d 0d0a 0000 0000 dc8d 3464 5e04 0000  U.........4d^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6502 6506 8301 6a07 a008  m.Z...e.e...j...
 00000060: a100 5a09 6500 6a0a a00b 6509 6404 a102  ..Z.e.j...e.d...
 00000070: 5a0c 6503 6a0d 6405 6406 8d01 6407 6408  Z.e.j.d.d...d.d.
@@ -13,81 +13,77 @@
 000000c0: 6411 a101 6503 a010 640a a101 6503 6a11  d...e...d...e.j.
 000000d0: 640b 640c 640d 8d02 6412 6413 8400 8301  d.d.d...d.d.....
 000000e0: 8301 8301 8301 5a13 650e a014 6512 a101  ......Z.e...e...
 000000f0: 0100 650e a014 6513 a101 0100 6414 6415  ..e...e.....d.d.
 00000100: 8400 5a15 6516 6416 6b02 72e4 650e 8300  ..Z.e.d.k.r.e...
 00000110: 0100 6401 5300 2917 e900 0000 004e 2901  ..d.S.)......N).
 00000120: da04 5061 7468 2901 da0b 7472 7963 6f70  ..Path)...trycop
-00000130: 7974 7265 655a 0573 6974 6573 7a0f 3c4a  ytreeZ.sitesz.<J
-00000140: 616d 7374 6163 6b20 636c 692f 3e29 01da  amstack cli/>)..
-00000150: 0468 656c 7063 0000 0000 0000 0000 0000  .helpc..........
-00000160: 0000 0000 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000170: 0000 0064 0053 00a9 014e a900 7206 0000  ...d.S...N..r...
-00000180: 0072 0600 0000 7206 0000 00fa 3c2f 686f  .r....r.....</ho
-00000190: 6d65 2f6a 616c 6b68 6f76 2f72 6570 6f73  me/jalkhov/repos
-000001a0: 2f4a 616d 7374 6163 6b70 792f 6a61 6d73  /Jamstackpy/jams
-000001b0: 7461 636b 2f6a 616d 7374 6163 6b2f 5f5f  tack/jamstack/__
-000001c0: 6d61 696e 5f5f 2e70 79da 0363 6c69 0b00  main__.py..cli..
-000001d0: 0000 7302 0000 0000 0272 0800 0000 7a15  ..s......r....z.
-000001e0: 3c45 6d70 7479 2c20 706c 6169 6e20 7265  <Empty, plain re
-000001f0: 706f 202f 3eda 0c70 726f 6a65 6374 5f6e  po />..project_n
-00000200: 616d 657a 192d 2d65 7869 7374 696e 672f  amez.--existing/
-00000210: 2d2d 6e6f 742d 6578 6973 7469 6e67 4629  --not-existingF)
-00000220: 01da 0764 6566 6175 6c74 6302 0000 0000  ...defaultc.....
-00000230: 0000 0000 0000 0004 0000 0006 0000 0043  ...............C
-00000240: 0000 0073 3a00 0000 6401 7d02 6402 7d03  ...s:...d.}.d.}.
-00000250: 7c01 6403 7500 7214 6403 7d03 7400 7401  |.d.u.r.d.}.t.t.
-00000260: 6a02 a003 7404 6404 a102 7401 6a02 a003  j...t.d...t.j...
-00000270: 7c02 7c00 a102 7c03 6405 8d03 0100 6400  |.|...|.d.....d.
-00000280: 5300 2906 4eda 012e 4654 da05 706c 6169  S.).N...FT..plai
-00000290: 6ea9 01da 0d64 6972 735f 6578 6973 745f  n....dirs_exist_
-000002a0: 6f6b 2905 7203 0000 00da 026f 73da 0470  ok).r......os..p
-000002b0: 6174 68da 046a 6f69 6eda 0a73 6974 6573  ath..join..sites
-000002c0: 5f70 6174 6829 0472 0900 0000 da08 6578  _path).r......ex
-000002d0: 6973 7469 6e67 7210 0000 0072 0e00 0000  istingr....r....
-000002e0: 7206 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-000002f0: 0c00 0000 1000 0000 7312 0000 0000 0404  ........s.......
-00000300: 0204 0108 0104 0102 010c 010c 0102 fd72  ...............r
-00000310: 0c00 0000 7a15 3c52 6570 6f20 6279 2074  ....z.<Repo by t
-00000320: 656d 706c 6174 6573 202f 3eda 0874 656d  emplates />..tem
-00000330: 706c 6174 6563 0300 0000 0000 0000 0000  platec..........
-00000340: 0000 0700 0000 0600 0000 4300 0000 7358  ..........C...sX
-00000350: 0000 0064 017d 037c 00a0 0064 02a1 0164  ...d.}.|...d...d
-00000360: 0319 007d 047c 00a0 0064 02a1 0164 0419  ...}.|...d...d..
-00000370: 007d 0564 057d 067c 0264 0675 0072 3064  .}.d.}.|.d.u.r0d
-00000380: 067d 0674 0174 026a 03a0 0474 057c 047c  .}.t.t.j...t.|.|
-00000390: 05a1 0374 026a 03a0 047c 037c 01a1 027c  ...t.j...|.|...|
-000003a0: 0664 078d 0301 0064 0053 0029 084e 720b  .d.....d.S.).Nr.
-000003b0: 0000 00fa 012f 7201 0000 00e9 0100 0000  ...../r.........
-000003c0: 4654 720d 0000 0029 06da 0573 706c 6974  FTr....)...split
-000003d0: 7203 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000003e0: 1100 0000 7212 0000 0029 0772 1400 0000  ....r....).r....
-000003f0: 7209 0000 0072 1300 0000 7210 0000 00da  r....r....r.....
-00000400: 096e 616d 6573 7061 6365 5a07 7072 6f6a  .namespaceZ.proj
-00000410: 6563 7472 0e00 0000 7206 0000 0072 0600  ectr....r....r..
-00000420: 0000 7207 0000 00da 0174 2000 0000 7316  ..r......t ...s.
-00000430: 0000 0000 0504 020e 010e 0204 0108 0104  ................
-00000440: 0202 010e 010c 0102 fd72 1900 0000 6300  .........r....c.
-00000450: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00000460: 0000 0043 0000 0073 0a00 0000 7400 8300  ...C...s....t...
-00000470: 0100 6400 5300 7205 0000 0029 0172 0800  ..d.S.r....).r..
-00000480: 0000 7206 0000 0072 0600 0000 7206 0000  ..r....r....r...
-00000490: 0072 0700 0000 da04 6d61 696e 3900 0000  .r......main9...
-000004a0: 7302 0000 0000 0172 1a00 0000 da08 5f5f  s......r......__
-000004b0: 6d61 696e 5f5f 2917 720f 0000 00da 0770  main__).r......p
-000004c0: 6174 686c 6962 7202 0000 005a 0563 6c69  athlibr....Z.cli
-000004d0: 636b 5a11 6a61 6d73 7461 636b 2e61 7069  ckZ.jamstack.api
-000004e0: 2e66 696c 6572 0300 0000 da08 5f5f 6669  .filer......__fi
-000004f0: 6c65 5f5f da06 7061 7265 6e74 da08 6162  le__..parent..ab
-00000500: 736f 6c75 7465 5a0e 7061 636b 6167 655f  soluteZ.package_
-00000510: 666f 6c64 6572 7210 0000 0072 1100 0000  folderr....r....
-00000520: 7212 0000 00da 0567 726f 7570 7208 0000  r......groupr...
-00000530: 005a 0763 6f6d 6d61 6e64 5a08 6172 6775  .Z.commandZ.argu
-00000540: 6d65 6e74 da06 6f70 7469 6f6e 720c 0000  ment..optionr...
-00000550: 0072 1900 0000 5a0b 6164 645f 636f 6d6d  .r....Z.add_comm
-00000560: 616e 6472 1a00 0000 da08 5f5f 6e61 6d65  andr......__name
-00000570: 5f5f 7206 0000 0072 0600 0000 7206 0000  __r....r....r...
-00000580: 0072 0700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000590: 0100 0000 732a 0000 0008 010c 0208 010c  ....s*..........
-000005a0: 020e 010e 030a 010a 040a 0108 010c 010e  ................
-000005b0: 0d0a 0108 0108 010c 0110 110a 010a 0308  ................
-000005c0: 0408 01                                  ...
+00000130: 7974 7265 655a 0573 6974 6573 7a1f 4a61  ytreeZ.sitesz.Ja
+00000140: 6d73 7461 636b 2063 6f6d 6d61 6e64 206c  mstack command l
+00000150: 696e 6520 696e 7465 7266 6163 6529 01da  ine interface)..
+00000160: 0468 656c 7063 0000 0000 0000 0000 0000  .helpc..........
+00000170: 0000 0000 0000 0100 0000 4300 0000 7304  ..........C...s.
+00000180: 0000 0064 0053 00a9 014e a900 7206 0000  ...d.S...N..r...
+00000190: 0072 0600 0000 7206 0000 00fa 4c63 3a5c  .r....r.....Lc:\
+000001a0: 7573 6572 735c 6a61 6c6b 686f 765c 646f  users\jalkhov\do
+000001b0: 6375 6d65 6e74 735c 6769 7468 7562 5c6a  cuments\github\j
+000001c0: 616d 7374 6163 6b2e 6f72 675c 6a61 6d73  amstack.org\jams
+000001d0: 7461 636b 5c6a 616d 7374 6163 6b5c 5f5f  tack\jamstack\__
+000001e0: 6d61 696e 5f5f 2e70 79da 0363 6c69 0c00  main__.py..cli..
+000001f0: 0000 7302 0000 0000 0272 0800 0000 7a21  ..s......r....z!
+00000200: 4372 6561 7465 2061 6e20 656d 7074 792c  Create an empty,
+00000210: 2070 6c61 696e 2072 6570 6f73 6974 6f72   plain repositor
+00000220: 79da 0c70 726f 6a65 6374 5f6e 616d 657a  y..project_namez
+00000230: 192d 2d65 7869 7374 696e 672f 2d2d 6e6f  .--existing/--no
+00000240: 742d 6578 6973 7469 6e67 4629 01da 0764  t-existingF)...d
+00000250: 6566 6175 6c74 6302 0000 0000 0000 0000  efaultc.........
+00000260: 0000 0003 0000 0006 0000 0043 0000 0073  ...........C...s
+00000270: 2800 0000 6401 7d02 7400 7401 6a02 a003  (...d.}.t.t.j...
+00000280: 7404 6402 a102 7401 6a02 a003 7c02 7c00  t.d...t.j...|.|.
+00000290: a102 7c01 8303 0100 6400 5300 2903 4eda  ..|.....d.S.).N.
+000002a0: 012e da05 706c 6169 6e29 0572 0300 0000  ....plain).r....
+000002b0: da02 6f73 da04 7061 7468 da04 6a6f 696e  ..os..path..join
+000002c0: da0a 7369 7465 735f 7061 7468 2903 7209  ..sites_path).r.
+000002d0: 0000 00da 0865 7869 7374 696e 6772 0e00  .....existingr..
+000002e0: 0000 7206 0000 0072 0600 0000 7207 0000  ..r....r....r...
+000002f0: 0072 0c00 0000 1100 0000 730c 0000 0000  .r........s.....
+00000300: 0404 0202 010c 010c 0102 fd72 0c00 0000  ...........r....
+00000310: 7a23 4372 6561 7465 2061 2072 6570 6f73  z#Create a repos
+00000320: 6974 6f72 7920 6672 6f6d 2061 2074 656d  itory from a tem
+00000330: 706c 6174 65da 0874 656d 706c 6174 6563  plate..templatec
+00000340: 0300 0000 0000 0000 0000 0000 0600 0000  ................
+00000350: 0600 0000 4300 0000 7338 0000 0064 017d  ....C...s8...d.}
+00000360: 037c 00a0 0064 02a1 015c 027d 047d 0574  .|...d...\.}.}.t
+00000370: 0174 026a 03a0 0474 057c 047c 05a1 0374  .t.j...t.|.|...t
+00000380: 026a 03a0 047c 037c 01a1 027c 0283 0301  .j...|.|...|....
+00000390: 0064 0053 0029 034e 720b 0000 00fa 012f  .d.S.).Nr....../
+000003a0: 2906 da05 7370 6c69 7472 0300 0000 720d  )...splitr....r.
+000003b0: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
+000003c0: 0000 2906 7212 0000 0072 0900 0000 7211  ..).r....r....r.
+000003d0: 0000 0072 0e00 0000 da09 6e61 6d65 7370  ...r......namesp
+000003e0: 6163 655a 0770 726f 6a65 6374 7206 0000  aceZ.projectr...
+000003f0: 0072 0600 0000 7207 0000 00da 0174 1e00  .r....r......t..
+00000400: 0000 730e 0000 0000 0504 010e 0202 010e  ..s.............
+00000410: 010c 0102 fd72 1600 0000 6300 0000 0000  .....r....c.....
+00000420: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
+00000430: 0000 0073 0a00 0000 7400 8300 0100 6400  ...s....t.....d.
+00000440: 5300 7205 0000 0029 0172 0800 0000 7206  S.r....).r....r.
+00000450: 0000 0072 0600 0000 7206 0000 0072 0700  ...r....r....r..
+00000460: 0000 da04 6d61 696e 3100 0000 7302 0000  ....main1...s...
+00000470: 0000 0172 1700 0000 da08 5f5f 6d61 696e  ...r......__main
+00000480: 5f5f 2917 720d 0000 00da 0770 6174 686c  __).r......pathl
+00000490: 6962 7202 0000 005a 0563 6c69 636b 5a11  ibr....Z.clickZ.
+000004a0: 6a61 6d73 7461 636b 2e61 7069 2e66 696c  jamstack.api.fil
+000004b0: 6572 0300 0000 da08 5f5f 6669 6c65 5f5f  er......__file__
+000004c0: da06 7061 7265 6e74 da08 6162 736f 6c75  ..parent..absolu
+000004d0: 7465 5a0e 7061 636b 6167 655f 666f 6c64  teZ.package_fold
+000004e0: 6572 720e 0000 0072 0f00 0000 7210 0000  err....r....r...
+000004f0: 00da 0567 726f 7570 7208 0000 005a 0763  ...groupr....Z.c
+00000500: 6f6d 6d61 6e64 5a08 6172 6775 6d65 6e74  ommandZ.argument
+00000510: da06 6f70 7469 6f6e 720c 0000 0072 1600  ..optionr....r..
+00000520: 0000 5a0b 6164 645f 636f 6d6d 616e 6472  ..Z.add_commandr
+00000530: 1700 0000 da08 5f5f 6e61 6d65 5f5f 7206  ......__name__r.
+00000540: 0000 0072 0600 0000 7206 0000 0072 0700  ...r....r....r..
+00000550: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000560: 732a 0000 0008 010c 0208 020c 020e 010e  s*..............
+00000570: 030a 010a 040a 0108 010c 010e 0a0a 0108  ................
+00000580: 0108 010c 0110 0b0a 010a 0308 0408 01    ...............
```

### Comparing `jamstack-1.0.0/jamstack/api/file.py` & `jamstack-1.1.0/jamstack/api/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,88 @@
+import logging
 import os
 import shutil
 import uuid
 
-# from werkzeug.utils import secure_filename
 
-
-def trycopytree(source, dest, verbose=False, dirs_exist_ok=False):
+def trycopytree(source, dest, dirs_exist_ok):
     """
-    Recursive copy of folder
+    Copy a file or directory from source to dest.
 
     Parameters
     ----------
     source: str
-        source folder path
+        source file or directory path
     dest: str
-        destination folder path
-
+        destination file or directory path
+    dirs_exist_ok:
+        especifies if the project folder already exist
     Returns
     -------
     None
     """
     try:
         shutil.copytree(source, dest, dirs_exist_ok=dirs_exist_ok)
-        if verbose:
-            print("done copying {} to {}".format(source, dest))
-    except Exception as e:
-        print(e)
-
-
-def trycopy(source, dest, verbose=False):
-    """
-    Non-ecursive copy of folder
-
-    Parameters
-    ----------
-    source: str
-        source folder path
-    dest: str
-        destination folder path
-
-    Returns
-    -------
-    None
-    """
-    try:
-        shutil.copy(source, dest)
-        if verbose:
-            print("done copying {} to {}".format(source, dest))
+        os.mkdir(os.path.join(dest, 'dist'))  # Maybe place in static.py?
+        print('Project created successfully! :)')
+    except FileExistsError:
+        print('Project folder already exist! Use --existing if you want to override it.')
     except Exception as e:
-        print(e)
+        logging.exception(e)
 
 
 def trymkdir(path, verbose=False):
     """
     Creates dir at destination
 
     Parameters
     ----------
     path: str
         path with folder already in
+    verbose: bool, optional
+        If True, print debug information. Default is False.
 
     Returns
     -------
     None
     """
     try:
         os.mkdir(path)
         if verbose:
             print("created dir at", path)
     except Exception as e:
-        print(e)
+        logging.exception(e)
 
 
 def trymkfile(path, content, verbose=False):
     """
     Creates file
 
     Parameters
     ----------
     path: str
         path to create file with filename included
     content: str
         file content
+    verbose: bool, optional
+        If True, print debug information. Default is False.
 
     Returns
     -------
     None
     """
     try:
-        with open(path, "w+") as f:
+        with open(path, "x") as f:
             f.write(content)
         if verbose:
             print("file created at {}".format(path))
             print("with content:")
             print(content)
     except Exception as e:
-        print(e)
+        logging.exception(e)
 
 
 def absdiroffile(filepath):
     """
     Gives absolute directory of file, normally expects __file__ as
     param
 
@@ -113,23 +96,64 @@
     str
         Absolute dir path of file
     """
     return os.path.dirname(os.path.abspath(filepath))
 
 
 def get_folders(path):
+    """
+    Get a list of directories in the given path.
+
+    Parameters
+    ----------
+    path: str
+        Path to search for directories.
+
+    Returns
+    -------
+    list
+        List of directories in the given path.
+    """
     dirs = [d for d in os.listdir(
         path) if os.path.isdir(os.path.join(path, d))]
     return dirs
 
 
 def unique_filename(fname):
+    """
+    Generate a unique filename by prepending a UUID to the given filename.
+
+    Parameters
+    ----------
+    fname: str
+        Original filename.
+
+    Returns
+    -------
+    str
+        Unique filename with prepended UUID.
+    """
     prepended = str(uuid.uuid4()).replace("-", "_")[:10]
     return "{}_{}".format(prepended, fname)
 
 
 def delete_file(path):
-    os.remove(path)
+    """
+    Delete the file at the given path.
+
+    Parameters
+    ----------
+    path: str
+        Path of the file to delete.
 
+    Returns
+    -------
+    None
+    """
+    try:
+        os.remove(path)
+        logging.info("File deleted: {}".format(path))
+    except Exception as e:
+        logging.exception(e)
 
 # def unique_sec_filename(filename):
 #     return unique_filename(secure_filename(filename))
```

### Comparing `jamstack-1.0.0/jamstack/jamdo/jamdo.py` & `jamstack-1.1.0/jamstack/jamdo/jamdo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,54 @@
-import json
 import os
 import urllib.request
 
 import requests
 from tqdm import tqdm
 
-templates_url = ("https://api.github.com/repos/jamstackpy/"
-                 "jamstack-templates/git/trees/main?recursive=1")
+TEMPLATES_URL = "https://api.github.com/repos/jamstackpy/jamstack-templates/git/trees/main?recursive=1"
+
+
+def mkdirs(path):
+    if not os.path.isdir(path):
+        os.makedirs(path)
 
 
 def get_raw_url(file_path, url):
-    tmp_url = url.replace(
+    raw_url = url.replace(
         'https://api.github.com/repos/',
         'https://raw.githubusercontent.com/')
-    tmp_url = tmp_url.split('/git/blobs/')[0]
-    tmp_url = tmp_url + '/master/' + file_path
-    return tmp_url
+    raw_url = raw_url.split('/git/blobs/')[0]
+    raw_url = raw_url + '/master/' + file_path
+    return raw_url
 
 
 def get_download_links(template):
-    api = requests.get(templates_url).text
-    print(templates_url)
-    files = json.loads(api)
+    api = requests.get(TEMPLATES_URL).json()
+    files = api['tree']
     output = []
-    location = dict()
-    for (k, i) in enumerate(files['tree']):
-        if template in i['path']:
-            if i['type'] == 'blob':
-                tmp = [i['path']]
-                tmp += [get_raw_url(tmp[0], i['url'])]
-                output.append(tmp)
+    location = {}
+    for i, file in enumerate(files):
+        if template in file['path']:
+            if file['type'] == 'blob':
+                output.append([file['path'], get_raw_url(file['path'], file['url'])])
             else:
-                location[i['path']] = k
-    files = output
-    location = location
-
-    return (files, location)
-
-
-def mkdirs(path):
-    if not os.path.isdir(path):
-        os.makedirs(path)
+                location[file['path']] = i
+    return output, location
 
 
 def download(template, target_folder='*', recursive=True):
     data = get_download_links(template)
     files = data[0]
     location = data[1]
 
-    # mkdirs(".")
-
     if target_folder == '*':
         start = 0
     else:
-        tmp_target = target_folder.replace('./', '')
-        tmp_target = tmp_target.replace('../', '')
-
-        # Remove "/"
-        tmp_target = (tmp_target if tmp_target[-1] != '/'
-                      else tmp_target[:-1])
         start = location[target_folder]
 
-    # Start download
     with tqdm(total=len(files), desc="Downloading assets...") as pbar:
         for i in files[start:]:
             ndir = i[0].replace('templates/' + template, 'dist/assets/')
-            if recursive or ndir.split(target_folder)[1].count('/') \
-                    <= 1:
+            if recursive or ndir.split(target_folder)[1].count('/') <= 1:
                 mkdirs('.' + '/' + os.path.dirname(ndir))
                 urllib.request.urlretrieve(i[1], '.' + '/' + ndir)
             pbar.update(1)
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/footer.html` & `jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/footer.html`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-<!-- Footer -->
-<footer id="footer">
-	<section>
-		<form method="post" action="#">
-			<div class="fields">
-				<div class="field">
-					<label for="name">Name</label>
-					<input type="text" name="name" id="name" />
-				</div>
-				<div class="field">
-					<label for="email">Email</label>
-					<input type="text" name="email" id="email" />
-				</div>
-				<div class="field">
-					<label for="message">Message</label>
-					<textarea name="message" id="message" rows="3"></textarea>
-				</div>
-			</div>
-			<ul class="actions">
-				<li><input type="submit" value="Send Message" /></li>
-			</ul>
-		</form>
-	</section>
-	<section class="split contact">
-		<section class="alt">
-			<h3>Address</h3>
-			<p>1234 Somewhere Road #87257<br />
-			Nashville, TN 00000-0000</p>
-		</section>
-		<section>
-			<h3>Phone</h3>
-			<p><a href="#">(000) 000-0000</a></p>
-		</section>
-		<section>
-			<h3>Email</h3>
-			<p><a href="#">info@untitled.tld</a></p>
-		</section>
-		<section>
-			<h3>Social</h3>
-			<ul class="icons alt">
-				<li><a href="{{ info['social']['twitter'] }}" class="icon brands alt fa-twitter"><span class="label">Twitter</span></a></li>
-				<li><a href="{{ info['social']['facebook'] }}" class="icon brands alt fa-facebook-f"><span class="label">Facebook</span></a></li>
-				<li><a href="{{ info['social']['instagram'] }}" class="icon brands alt fa-instagram"><span class="label">Instagram</span></a></li>
-				<li><a href="{{ info['social']['github'] }}" class="icon brands alt fa-github"><span class="label">GitHub</span></a></li>
-			</ul>
-		</section>
-	</section>
+<!-- Footer -->
+<footer id="footer">
+	<section>
+		<form method="post" action="#">
+			<div class="fields">
+				<div class="field">
+					<label for="name">Name</label>
+					<input type="text" name="name" id="name" />
+				</div>
+				<div class="field">
+					<label for="email">Email</label>
+					<input type="text" name="email" id="email" />
+				</div>
+				<div class="field">
+					<label for="message">Message</label>
+					<textarea name="message" id="message" rows="3"></textarea>
+				</div>
+			</div>
+			<ul class="actions">
+				<li><input type="submit" value="Send Message" /></li>
+			</ul>
+		</form>
+	</section>
+	<section class="split contact">
+		<section class="alt">
+			<h3>Address</h3>
+			<p>1234 Somewhere Road #87257<br />
+			Nashville, TN 00000-0000</p>
+		</section>
+		<section>
+			<h3>Phone</h3>
+			<p><a href="#">(000) 000-0000</a></p>
+		</section>
+		<section>
+			<h3>Email</h3>
+			<p><a href="#">info@untitled.tld</a></p>
+		</section>
+		<section>
+			<h3>Social</h3>
+			<ul class="icons alt">
+				<li><a href="{{ info['social']['twitter'] }}" class="icon brands alt fa-twitter"><span class="label">Twitter</span></a></li>
+				<li><a href="{{ info['social']['facebook'] }}" class="icon brands alt fa-facebook-f"><span class="label">Facebook</span></a></li>
+				<li><a href="{{ info['social']['instagram'] }}" class="icon brands alt fa-instagram"><span class="label">Instagram</span></a></li>
+				<li><a href="{{ info['social']['github'] }}" class="icon brands alt fa-github"><span class="label">GitHub</span></a></li>
+			</ul>
+		</section>
+	</section>
 </footer>
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/main.html` & `jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/main.html`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-<!-- Main -->
-<div id="main">
-	<!-- Post -->
-	<section class="post">
-		<header class="major">
-			<span class="date">April 25, 2017</span>
-			<h1>This is a<br />
-			Generic Page</h1>
-			<p>Aenean ornare velit lacus varius enim ullamcorper proin aliquam<br />
-				facilisis ante sed etiam magna interdum congue. Lorem ipsum dolor<br />
-			amet nullam sed etiam veroeros.</p>
-		</header>
-		<div class="image main"><img src="images/pic01.jpg" alt="" /></div>
-		<p>Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Curabitur sapien risus, commodo eget turpis at, elementum convallis enim turpis, lorem ipsum dolor sit amet nullam.</p>
-		<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis dapibus rutrum facilisis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam tristique libero eu nibh porttitor fermentum. Nullam venenatis erat id vehicula viverra. Nunc ultrices eros ut ultricies condimentum. Mauris risus lacus, blandit sit amet venenatis non, bibendum vitae dolor. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In non lorem sit amet elit placerat maximus. Pellentesque aliquam maximus risus. Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum.</p>
-	</section>
+<!-- Main -->
+<div id="main">
+	<!-- Post -->
+	<section class="post">
+		<header class="major">
+			<span class="date">April 25, 2017</span>
+			<h1>This is a<br />
+			Generic Page</h1>
+			<p>Aenean ornare velit lacus varius enim ullamcorper proin aliquam<br />
+				facilisis ante sed etiam magna interdum congue. Lorem ipsum dolor<br />
+			amet nullam sed etiam veroeros.</p>
+		</header>
+		<div class="image main"><img src="images/pic01.jpg" alt="" /></div>
+		<p>Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Curabitur sapien risus, commodo eget turpis at, elementum convallis enim turpis, lorem ipsum dolor sit amet nullam.</p>
+		<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis dapibus rutrum facilisis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam tristique libero eu nibh porttitor fermentum. Nullam venenatis erat id vehicula viverra. Nunc ultrices eros ut ultricies condimentum. Mauris risus lacus, blandit sit amet venenatis non, bibendum vitae dolor. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In non lorem sit amet elit placerat maximus. Pellentesque aliquam maximus risus. Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum.</p>
+	</section>
 </div>
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/massively/templates/sections/nav.html` & `jamstack-1.1.0/jamstack/sites/html5up/massively/templates/sections/nav.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-<!-- Nav -->
-<nav id="nav">
-	<ul class="links">
-		{% for elem in info['nav'] %}
-			<li class="{{ 'active' if active_page == elem[2] }}"><a href="{{ elem[1] }}">{{ elem[0] }}</a></li>
-		{% endfor %}
-	</ul>
-	<ul class="icons">
-		<li><a href="{{ info['social']['twitter'] }}" class="icon brands fa-twitter"><span class="label">Twitter</span></a></li>
-		<li><a href="{{ info['social']['facebook'] }}" class="icon brands fa-facebook-f"><span class="label">Facebook</span></a></li>
-		<li><a href="{{ info['social']['instagram'] }}" class="icon brands fa-instagram"><span class="label">Instagram</span></a></li>
-		<li><a href="{{ info['social']['github'] }}" class="icon brands fa-github"><span class="label">GitHub</span></a></li>
-	</ul>
+<!-- Nav -->
+<nav id="nav">
+	<ul class="links">
+		{% for elem in info['nav'] %}
+			<li class="{{ 'active' if active_page == elem[2] }}"><a href="{{ elem[1] }}">{{ elem[0] }}</a></li>
+		{% endfor %}
+	</ul>
+	<ul class="icons">
+		<li><a href="{{ info['social']['twitter'] }}" class="icon brands fa-twitter"><span class="label">Twitter</span></a></li>
+		<li><a href="{{ info['social']['facebook'] }}" class="icon brands fa-facebook-f"><span class="label">Facebook</span></a></li>
+		<li><a href="{{ info['social']['instagram'] }}" class="icon brands fa-instagram"><span class="label">Instagram</span></a></li>
+		<li><a href="{{ info['social']['github'] }}" class="icon brands fa-github"><span class="label">GitHub</span></a></li>
+	</ul>
 </nav>
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/phantom/posts.json` & `jamstack-1.1.0/jamstack/sites/html5up/phantom/posts.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,208 +1,213 @@
-00000000: 7b0a 2020 2020 2270 6f73 7473 223a 207b  {.    "posts": {
-00000010: 0a20 2020 2020 2020 2022 706f 7374 3122  .        "post1"
-00000020: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000030: 2274 6974 6c65 223a 2022 4d41 474e 4122  "title": "MAGNA"
-00000040: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-00000050: 6875 6d62 6e61 696c 223a 2022 6874 7470  humbnail": "http
-00000060: 733a 2f2f 7069 6373 756d 2e70 686f 746f  s://picsum.photo
-00000070: 732f 3335 302f 3335 303f 7261 6e64 6f6d  s/350/350?random
-00000080: 3d32 222c 0a20 2020 2020 2020 2020 2020  =2",.           
-00000090: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000000a0: 2253 6564 206e 6973 6c20 6172 6375 2065  "Sed nisl arcu e
-000000b0: 7569 736d 6f64 2073 6974 2061 6d65 7420  uismod sit amet 
-000000c0: 6e69 7369 206c 6f72 656d 2065 7469 616d  nisi lorem etiam
-000000d0: 2064 6f6c 6f72 2076 6572 6f65 726f 7320   dolor veroeros 
-000000e0: 6574 2066 6575 6769 6174 2e22 2c0a 2020  et feugiat.",.  
-000000f0: 2020 2020 2020 2020 2020 2270 6167 6522            "page"
-00000100: 3a20 2270 6f73 745f 7465 6d70 6c61 7465  : "post_template
-00000110: 2e68 746d 6c22 0a20 2020 2020 2020 207d  .html".        }
-00000120: 2c0a 2020 2020 2020 2020 2270 6f73 7432  ,.        "post2
-00000130: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000140: 2022 7469 746c 6522 3a20 224c 4f52 454d   "title": "LOREM
-00000150: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000160: 7468 756d 626e 6169 6c22 3a20 2268 7474  thumbnail": "htt
-00000170: 7073 3a2f 2f70 6963 7375 6d2e 7068 6f74  ps://picsum.phot
-00000180: 6f73 2f33 3530 2f33 3530 3f72 616e 646f  os/350/350?rando
-00000190: 6d3d 3222 2c0a 2020 2020 2020 2020 2020  m=2",.          
-000001a0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000001b0: 2022 5365 6420 6e69 736c 2061 7263 7520   "Sed nisl arcu 
-000001c0: 6575 6973 6d6f 6420 7369 7420 616d 6574  euismod sit amet
-000001d0: 206e 6973 6920 6c6f 7265 6d20 6574 6961   nisi lorem etia
-000001e0: 6d20 646f 6c6f 7220 7665 726f 6572 6f73  m dolor veroeros
-000001f0: 2065 7420 6665 7567 6961 742e 222c 0a20   et feugiat.",. 
-00000200: 2020 2020 2020 2020 2020 2022 7061 6765             "page
-00000210: 223a 2022 706f 7374 5f74 656d 706c 6174  ": "post_templat
-00000220: 652e 6874 6d6c 220a 2020 2020 2020 2020  e.html".        
-00000230: 7d2c 0a20 2020 2020 2020 2022 706f 7374  },.        "post
-00000240: 3322 3a20 7b0a 2020 2020 2020 2020 2020  3": {.          
-00000250: 2020 2274 6974 6c65 223a 2022 4645 5547    "title": "FEUG
-00000260: 4941 5422 2c0a 2020 2020 2020 2020 2020  IAT",.          
-00000270: 2020 2274 6875 6d62 6e61 696c 223a 2022    "thumbnail": "
-00000280: 6874 7470 733a 2f2f 7069 6373 756d 2e70  https://picsum.p
-00000290: 686f 746f 732f 3335 302f 3335 303f 7261  hotos/350/350?ra
-000002a0: 6e64 6f6d 3d32 222c 0a20 2020 2020 2020  ndom=2",.       
-000002b0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000002c0: 6e22 3a20 2253 6564 206e 6973 6c20 6172  n": "Sed nisl ar
-000002d0: 6375 2065 7569 736d 6f64 2073 6974 2061  cu euismod sit a
-000002e0: 6d65 7420 6e69 7369 206c 6f72 656d 2065  met nisi lorem e
-000002f0: 7469 616d 2064 6f6c 6f72 2076 6572 6f65  tiam dolor veroe
-00000300: 726f 7320 6574 2066 6575 6769 6174 2e22  ros et feugiat."
-00000310: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
-00000320: 6167 6522 3a20 2270 6f73 745f 7465 6d70  age": "post_temp
-00000330: 6c61 7465 2e68 746d 6c22 0a20 2020 2020  late.html".     
-00000340: 2020 207d 2c0a 2020 2020 2020 2020 2270     },.        "p
-00000350: 6f73 7434 223a 207b 0a20 2020 2020 2020  ost4": {.       
-00000360: 2020 2020 2022 7469 746c 6522 3a20 2254       "title": "T
-00000370: 454d 5055 5322 2c0a 2020 2020 2020 2020  EMPUS",.        
-00000380: 2020 2020 2274 6875 6d62 6e61 696c 223a      "thumbnail":
-00000390: 2022 6874 7470 733a 2f2f 7069 6373 756d   "https://picsum
-000003a0: 2e70 686f 746f 732f 3335 302f 3335 303f  .photos/350/350?
-000003b0: 7261 6e64 6f6d 3d32 222c 0a20 2020 2020  random=2",.     
-000003c0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000003d0: 696f 6e22 3a20 2253 6564 206e 6973 6c20  ion": "Sed nisl 
-000003e0: 6172 6375 2065 7569 736d 6f64 2073 6974  arcu euismod sit
-000003f0: 2061 6d65 7420 6e69 7369 206c 6f72 656d   amet nisi lorem
-00000400: 2065 7469 616d 2064 6f6c 6f72 2076 6572   etiam dolor ver
-00000410: 6f65 726f 7320 6574 2066 6575 6769 6174  oeros et feugiat
-00000420: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00000430: 2270 6167 6522 3a20 2270 6f73 745f 7465  "page": "post_te
-00000440: 6d70 6c61 7465 2e68 746d 6c22 0a20 2020  mplate.html".   
-00000450: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00000460: 2270 6f73 7435 223a 207b 0a20 2020 2020  "post5": {.     
-00000470: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
-00000480: 2241 4c49 5155 414d 222c 0a20 2020 2020  "ALIQUAM",.     
-00000490: 2020 2020 2020 2022 7468 756d 626e 6169         "thumbnai
-000004a0: 6c22 3a20 2268 7474 7073 3a2f 2f70 6963  l": "https://pic
-000004b0: 7375 6d2e 7068 6f74 6f73 2f33 3530 2f33  sum.photos/350/3
-000004c0: 3530 3f72 616e 646f 6d3d 3222 2c0a 2020  50?random=2",.  
-000004d0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-000004e0: 6970 7469 6f6e 223a 2022 5365 6420 6e69  iption": "Sed ni
-000004f0: 736c 2061 7263 7520 6575 6973 6d6f 6420  sl arcu euismod 
-00000500: 7369 7420 616d 6574 206e 6973 6920 6c6f  sit amet nisi lo
-00000510: 7265 6d20 6574 6961 6d20 646f 6c6f 7220  rem etiam dolor 
-00000520: 7665 726f 6572 6f73 2065 7420 6665 7567  veroeros et feug
-00000530: 6961 742e 222c 0a20 2020 2020 2020 2020  iat.",.         
-00000540: 2020 2022 7061 6765 223a 2022 706f 7374     "page": "post
-00000550: 5f74 656d 706c 6174 652e 6874 6d6c 220a  _template.html".
-00000560: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000570: 2020 2022 706f 7374 3622 3a20 7b0a 2020     "post6": {.  
-00000580: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
-00000590: 223a 2022 5645 524f 4552 4f53 222c 0a20  ": "VEROEROS",. 
-000005a0: 2020 2020 2020 2020 2020 2022 7468 756d             "thum
-000005b0: 626e 6169 6c22 3a20 2268 7474 7073 3a2f  bnail": "https:/
-000005c0: 2f70 6963 7375 6d2e 7068 6f74 6f73 2f33  /picsum.photos/3
-000005d0: 3530 2f33 3530 3f72 616e 646f 6d3d 3222  50/350?random=2"
-000005e0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-000005f0: 6573 6372 6970 7469 6f6e 223a 2022 5365  escription": "Se
-00000600: 6420 6e69 736c 2061 7263 7520 6575 6973  d nisl arcu euis
-00000610: 6d6f 6420 7369 7420 616d 6574 206e 6973  mod sit amet nis
-00000620: 6920 6c6f 7265 6d20 6574 6961 6d20 646f  i lorem etiam do
-00000630: 6c6f 7220 7665 726f 6572 6f73 2065 7420  lor veroeros et 
-00000640: 6665 7567 6961 742e 222c 0a20 2020 2020  feugiat.",.     
-00000650: 2020 2020 2020 2022 7061 6765 223a 2022         "page": "
-00000660: 706f 7374 5f74 656d 706c 6174 652e 6874  post_template.ht
-00000670: 6d6c 220a 2020 2020 2020 2020 7d2c 0a20  ml".        },. 
-00000680: 2020 2020 2020 2022 706f 7374 3722 3a20         "post7": 
-00000690: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
-000006a0: 6974 6c65 223a 2022 4950 5355 4d22 2c0a  itle": "IPSUM",.
-000006b0: 2020 2020 2020 2020 2020 2020 2274 6875              "thu
-000006c0: 6d62 6e61 696c 223a 2022 6874 7470 733a  mbnail": "https:
-000006d0: 2f2f 7069 6373 756d 2e70 686f 746f 732f  //picsum.photos/
-000006e0: 3335 302f 3335 303f 7261 6e64 6f6d 3d32  350/350?random=2
-000006f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000700: 6465 7363 7269 7074 696f 6e22 3a20 2253  description": "S
-00000710: 6564 206e 6973 6c20 6172 6375 2065 7569  ed nisl arcu eui
-00000720: 736d 6f64 2073 6974 2061 6d65 7420 6e69  smod sit amet ni
-00000730: 7369 206c 6f72 656d 2065 7469 616d 2064  si lorem etiam d
-00000740: 6f6c 6f72 2076 6572 6f65 726f 7320 6574  olor veroeros et
-00000750: 2066 6575 6769 6174 2e22 2c0a 2020 2020   feugiat.",.    
-00000760: 2020 2020 2020 2020 2270 6167 6522 3a20          "page": 
-00000770: 2270 6f73 745f 7465 6d70 6c61 7465 2e68  "post_template.h
-00000780: 746d 6c22 0a20 2020 2020 2020 207d 2c0a  tml".        },.
-00000790: 2020 2020 2020 2020 2270 6f73 7438 223a          "post8":
-000007a0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-000007b0: 7469 746c 6522 3a20 2244 4f4c 4f52 222c  title": "DOLOR",
-000007c0: 0a20 2020 2020 2020 2020 2020 2022 7468  .            "th
-000007d0: 756d 626e 6169 6c22 3a20 2268 7474 7073  umbnail": "https
-000007e0: 3a2f 2f70 6963 7375 6d2e 7068 6f74 6f73  ://picsum.photos
-000007f0: 2f33 3530 2f33 3530 3f72 616e 646f 6d3d  /350/350?random=
-00000800: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
-00000810: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00000820: 5365 6420 6e69 736c 2061 7263 7520 6575  Sed nisl arcu eu
-00000830: 6973 6d6f 6420 7369 7420 616d 6574 206e  ismod sit amet n
-00000840: 6973 6920 6c6f 7265 6d20 6574 6961 6d20  isi lorem etiam 
-00000850: 646f 6c6f 7220 7665 726f 6572 6f73 2065  dolor veroeros e
-00000860: 7420 6665 7567 6961 742e 222c 0a20 2020  t feugiat.",.   
-00000870: 2020 2020 2020 2020 2022 7061 6765 223a           "page":
-00000880: 2022 706f 7374 5f74 656d 706c 6174 652e   "post_template.
-00000890: 6874 6d6c 220a 2020 2020 2020 2020 7d2c  html".        },
-000008a0: 0a20 2020 2020 2020 2022 706f 7374 3922  .        "post9"
-000008b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000008c0: 2274 6974 6c65 223a 2022 4e55 4c4c 414d  "title": "NULLAM
-000008d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000008e0: 7468 756d 626e 6169 6c22 3a20 2268 7474  thumbnail": "htt
-000008f0: 7073 3a2f 2f70 6963 7375 6d2e 7068 6f74  ps://picsum.phot
-00000900: 6f73 2f33 3530 2f33 3530 3f72 616e 646f  os/350/350?rando
-00000910: 6d3d 3222 2c0a 2020 2020 2020 2020 2020  m=2",.          
-00000920: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00000930: 2022 5365 6420 6e69 736c 2061 7263 7520   "Sed nisl arcu 
-00000940: 6575 6973 6d6f 6420 7369 7420 616d 6574  euismod sit amet
-00000950: 206e 6973 6920 6c6f 7265 6d20 6574 6961   nisi lorem etia
-00000960: 6d20 646f 6c6f 7220 7665 726f 6572 6f73  m dolor veroeros
-00000970: 2065 7420 6665 7567 6961 742e 222c 0a20   et feugiat.",. 
-00000980: 2020 2020 2020 2020 2020 2022 7061 6765             "page
-00000990: 223a 2022 706f 7374 5f74 656d 706c 6174  ": "post_templat
-000009a0: 652e 6874 6d6c 220a 2020 2020 2020 2020  e.html".        
-000009b0: 7d2c 0a20 2020 2020 2020 2022 706f 7374  },.        "post
-000009c0: 3130 223a 207b 0a20 2020 2020 2020 2020  10": {.         
-000009d0: 2020 2022 7469 746c 6522 3a20 2255 4c54     "title": "ULT
-000009e0: 5249 4349 4553 222c 0a20 2020 2020 2020  RICIES",.       
-000009f0: 2020 2020 2022 7468 756d 626e 6169 6c22       "thumbnail"
-00000a00: 3a20 2268 7474 7073 3a2f 2f70 6963 7375  : "https://picsu
-00000a10: 6d2e 7068 6f74 6f73 2f33 3530 2f33 3530  m.photos/350/350
-00000a20: 3f72 616e 646f 6d3d 3222 2c0a 2020 2020  ?random=2",.    
-00000a30: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00000a40: 7469 6f6e 223a 2022 5365 6420 6e69 736c  tion": "Sed nisl
-00000a50: 2061 7263 7520 6575 6973 6d6f 6420 7369   arcu euismod si
-00000a60: 7420 616d 6574 206e 6973 6920 6c6f 7265  t amet nisi lore
-00000a70: 6d20 6574 6961 6d20 646f 6c6f 7220 7665  m etiam dolor ve
-00000a80: 726f 6572 6f73 2065 7420 6665 7567 6961  roeros et feugia
-00000a90: 742e 222c 0a20 2020 2020 2020 2020 2020  t.",.           
-00000aa0: 2022 7061 6765 223a 2022 706f 7374 5f74   "page": "post_t
-00000ab0: 656d 706c 6174 652e 6874 6d6c 220a 2020  emplate.html".  
-00000ac0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000ad0: 2022 706f 7374 3131 223a 207b 0a20 2020   "post11": {.   
-00000ae0: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-00000af0: 3a20 2244 4943 5455 4d22 2c0a 2020 2020  : "DICTUM",.    
-00000b00: 2020 2020 2020 2020 2274 6875 6d62 6e61          "thumbna
-00000b10: 696c 223a 2022 6874 7470 733a 2f2f 7069  il": "https://pi
-00000b20: 6373 756d 2e70 686f 746f 732f 3335 302f  csum.photos/350/
-00000b30: 3335 303f 7261 6e64 6f6d 3d32 222c 0a20  350?random=2",. 
-00000b40: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00000b50: 7269 7074 696f 6e22 3a20 2253 6564 206e  ription": "Sed n
-00000b60: 6973 6c20 6172 6375 2065 7569 736d 6f64  isl arcu euismod
-00000b70: 2073 6974 2061 6d65 7420 6e69 7369 206c   sit amet nisi l
-00000b80: 6f72 656d 2065 7469 616d 2064 6f6c 6f72  orem etiam dolor
-00000b90: 2076 6572 6f65 726f 7320 6574 2066 6575   veroeros et feu
-00000ba0: 6769 6174 2e22 2c0a 2020 2020 2020 2020  giat.",.        
-00000bb0: 2020 2020 2270 6167 6522 3a20 2270 6f73      "page": "pos
-00000bc0: 745f 7465 6d70 6c61 7465 2e68 746d 6c22  t_template.html"
-00000bd0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00000be0: 2020 2020 2270 6f73 7431 3222 3a20 7b0a      "post12": {.
-00000bf0: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
-00000c00: 6c65 223a 2022 5052 4554 4955 4d22 2c0a  le": "PRETIUM",.
-00000c10: 2020 2020 2020 2020 2020 2020 2274 6875              "thu
-00000c20: 6d62 6e61 696c 223a 2022 6874 7470 733a  mbnail": "https:
-00000c30: 2f2f 7069 6373 756d 2e70 686f 746f 732f  //picsum.photos/
-00000c40: 3335 302f 3335 303f 7261 6e64 6f6d 3d32  350/350?random=2
-00000c50: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000c60: 6465 7363 7269 7074 696f 6e22 3a20 2253  description": "S
-00000c70: 6564 206e 6973 6c20 6172 6375 2065 7569  ed nisl arcu eui
-00000c80: 736d 6f64 2073 6974 2061 6d65 7420 6e69  smod sit amet ni
-00000c90: 7369 206c 6f72 656d 2065 7469 616d 2064  si lorem etiam d
-00000ca0: 6f6c 6f72 2076 6572 6f65 726f 7320 6574  olor veroeros et
-00000cb0: 2066 6575 6769 6174 2e22 2c0a 2020 2020   feugiat.",.    
-00000cc0: 2020 2020 2020 2020 2270 6167 6522 3a20          "page": 
-00000cd0: 2270 6f73 745f 7465 6d70 6c61 7465 2e68  "post_template.h
-00000ce0: 746d 6c22 0a20 2020 2020 2020 207d 0a20  tml".        }. 
-00000cf0: 2020 207d 0a7d                              }.}
+00000000: 7b0d 0a20 2020 2022 706f 7374 7322 3a20  {..    "posts": 
+00000010: 7b0d 0a20 2020 2020 2020 2022 706f 7374  {..        "post
+00000020: 3122 3a20 7b0d 0a20 2020 2020 2020 2020  1": {..         
+00000030: 2020 2022 7469 746c 6522 3a20 224d 4147     "title": "MAG
+00000040: 4e41 222c 0d0a 2020 2020 2020 2020 2020  NA",..          
+00000050: 2020 2274 6875 6d62 6e61 696c 223a 2022    "thumbnail": "
+00000060: 6874 7470 733a 2f2f 7069 6373 756d 2e70  https://picsum.p
+00000070: 686f 746f 732f 3335 302f 3335 303f 7261  hotos/350/350?ra
+00000080: 6e64 6f6d 3d32 222c 0d0a 2020 2020 2020  ndom=2",..      
+00000090: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000000a0: 6f6e 223a 2022 5365 6420 6e69 736c 2061  on": "Sed nisl a
+000000b0: 7263 7520 6575 6973 6d6f 6420 7369 7420  rcu euismod sit 
+000000c0: 616d 6574 206e 6973 6920 6c6f 7265 6d20  amet nisi lorem 
+000000d0: 6574 6961 6d20 646f 6c6f 7220 7665 726f  etiam dolor vero
+000000e0: 6572 6f73 2065 7420 6665 7567 6961 742e  eros et feugiat.
+000000f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000100: 2270 6167 6522 3a20 2270 6f73 745f 7465  "page": "post_te
+00000110: 6d70 6c61 7465 2e68 746d 6c22 0d0a 2020  mplate.html"..  
+00000120: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00000130: 2020 2270 6f73 7432 223a 207b 0d0a 2020    "post2": {..  
+00000140: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+00000150: 223a 2022 4c4f 5245 4d22 2c0d 0a20 2020  ": "LOREM",..   
+00000160: 2020 2020 2020 2020 2022 7468 756d 626e           "thumbn
+00000170: 6169 6c22 3a20 2268 7474 7073 3a2f 2f70  ail": "https://p
+00000180: 6963 7375 6d2e 7068 6f74 6f73 2f33 3530  icsum.photos/350
+00000190: 2f33 3530 3f72 616e 646f 6d3d 3222 2c0d  /350?random=2",.
+000001a0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+000001b0: 7363 7269 7074 696f 6e22 3a20 2253 6564  scription": "Sed
+000001c0: 206e 6973 6c20 6172 6375 2065 7569 736d   nisl arcu euism
+000001d0: 6f64 2073 6974 2061 6d65 7420 6e69 7369  od sit amet nisi
+000001e0: 206c 6f72 656d 2065 7469 616d 2064 6f6c   lorem etiam dol
+000001f0: 6f72 2076 6572 6f65 726f 7320 6574 2066  or veroeros et f
+00000200: 6575 6769 6174 2e22 2c0d 0a20 2020 2020  eugiat.",..     
+00000210: 2020 2020 2020 2022 7061 6765 223a 2022         "page": "
+00000220: 706f 7374 5f74 656d 706c 6174 652e 6874  post_template.ht
+00000230: 6d6c 220d 0a20 2020 2020 2020 207d 2c0d  ml"..        },.
+00000240: 0a20 2020 2020 2020 2022 706f 7374 3322  .        "post3"
+00000250: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00000260: 2022 7469 746c 6522 3a20 2246 4555 4749   "title": "FEUGI
+00000270: 4154 222c 0d0a 2020 2020 2020 2020 2020  AT",..          
+00000280: 2020 2274 6875 6d62 6e61 696c 223a 2022    "thumbnail": "
+00000290: 6874 7470 733a 2f2f 7069 6373 756d 2e70  https://picsum.p
+000002a0: 686f 746f 732f 3335 302f 3335 303f 7261  hotos/350/350?ra
+000002b0: 6e64 6f6d 3d32 222c 0d0a 2020 2020 2020  ndom=2",..      
+000002c0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000002d0: 6f6e 223a 2022 5365 6420 6e69 736c 2061  on": "Sed nisl a
+000002e0: 7263 7520 6575 6973 6d6f 6420 7369 7420  rcu euismod sit 
+000002f0: 616d 6574 206e 6973 6920 6c6f 7265 6d20  amet nisi lorem 
+00000300: 6574 6961 6d20 646f 6c6f 7220 7665 726f  etiam dolor vero
+00000310: 6572 6f73 2065 7420 6665 7567 6961 742e  eros et feugiat.
+00000320: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000330: 2270 6167 6522 3a20 2270 6f73 745f 7465  "page": "post_te
+00000340: 6d70 6c61 7465 2e68 746d 6c22 0d0a 2020  mplate.html"..  
+00000350: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00000360: 2020 2270 6f73 7434 223a 207b 0d0a 2020    "post4": {..  
+00000370: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
+00000380: 223a 2022 5445 4d50 5553 222c 0d0a 2020  ": "TEMPUS",..  
+00000390: 2020 2020 2020 2020 2020 2274 6875 6d62            "thumb
+000003a0: 6e61 696c 223a 2022 6874 7470 733a 2f2f  nail": "https://
+000003b0: 7069 6373 756d 2e70 686f 746f 732f 3335  picsum.photos/35
+000003c0: 302f 3335 303f 7261 6e64 6f6d 3d32 222c  0/350?random=2",
+000003d0: 0d0a 2020 2020 2020 2020 2020 2020 2264  ..            "d
+000003e0: 6573 6372 6970 7469 6f6e 223a 2022 5365  escription": "Se
+000003f0: 6420 6e69 736c 2061 7263 7520 6575 6973  d nisl arcu euis
+00000400: 6d6f 6420 7369 7420 616d 6574 206e 6973  mod sit amet nis
+00000410: 6920 6c6f 7265 6d20 6574 6961 6d20 646f  i lorem etiam do
+00000420: 6c6f 7220 7665 726f 6572 6f73 2065 7420  lor veroeros et 
+00000430: 6665 7567 6961 742e 222c 0d0a 2020 2020  feugiat.",..    
+00000440: 2020 2020 2020 2020 2270 6167 6522 3a20          "page": 
+00000450: 2270 6f73 745f 7465 6d70 6c61 7465 2e68  "post_template.h
+00000460: 746d 6c22 0d0a 2020 2020 2020 2020 7d2c  tml"..        },
+00000470: 0d0a 2020 2020 2020 2020 2270 6f73 7435  ..        "post5
+00000480: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
+00000490: 2020 2274 6974 6c65 223a 2022 414c 4951    "title": "ALIQ
+000004a0: 5541 4d22 2c0d 0a20 2020 2020 2020 2020  UAM",..         
+000004b0: 2020 2022 7468 756d 626e 6169 6c22 3a20     "thumbnail": 
+000004c0: 2268 7474 7073 3a2f 2f70 6963 7375 6d2e  "https://picsum.
+000004d0: 7068 6f74 6f73 2f33 3530 2f33 3530 3f72  photos/350/350?r
+000004e0: 616e 646f 6d3d 3222 2c0d 0a20 2020 2020  andom=2",..     
+000004f0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00000500: 696f 6e22 3a20 2253 6564 206e 6973 6c20  ion": "Sed nisl 
+00000510: 6172 6375 2065 7569 736d 6f64 2073 6974  arcu euismod sit
+00000520: 2061 6d65 7420 6e69 7369 206c 6f72 656d   amet nisi lorem
+00000530: 2065 7469 616d 2064 6f6c 6f72 2076 6572   etiam dolor ver
+00000540: 6f65 726f 7320 6574 2066 6575 6769 6174  oeros et feugiat
+00000550: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00000560: 2022 7061 6765 223a 2022 706f 7374 5f74   "page": "post_t
+00000570: 656d 706c 6174 652e 6874 6d6c 220d 0a20  emplate.html".. 
+00000580: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+00000590: 2020 2022 706f 7374 3622 3a20 7b0d 0a20     "post6": {.. 
+000005a0: 2020 2020 2020 2020 2020 2022 7469 746c             "titl
+000005b0: 6522 3a20 2256 4552 4f45 524f 5322 2c0d  e": "VEROEROS",.
+000005c0: 0a20 2020 2020 2020 2020 2020 2022 7468  .            "th
+000005d0: 756d 626e 6169 6c22 3a20 2268 7474 7073  umbnail": "https
+000005e0: 3a2f 2f70 6963 7375 6d2e 7068 6f74 6f73  ://picsum.photos
+000005f0: 2f33 3530 2f33 3530 3f72 616e 646f 6d3d  /350/350?random=
+00000600: 3222 2c0d 0a20 2020 2020 2020 2020 2020  2",..           
+00000610: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00000620: 2253 6564 206e 6973 6c20 6172 6375 2065  "Sed nisl arcu e
+00000630: 7569 736d 6f64 2073 6974 2061 6d65 7420  uismod sit amet 
+00000640: 6e69 7369 206c 6f72 656d 2065 7469 616d  nisi lorem etiam
+00000650: 2064 6f6c 6f72 2076 6572 6f65 726f 7320   dolor veroeros 
+00000660: 6574 2066 6575 6769 6174 2e22 2c0d 0a20  et feugiat.",.. 
+00000670: 2020 2020 2020 2020 2020 2022 7061 6765             "page
+00000680: 223a 2022 706f 7374 5f74 656d 706c 6174  ": "post_templat
+00000690: 652e 6874 6d6c 220d 0a20 2020 2020 2020  e.html"..       
+000006a0: 207d 2c0d 0a20 2020 2020 2020 2022 706f   },..        "po
+000006b0: 7374 3722 3a20 7b0d 0a20 2020 2020 2020  st7": {..       
+000006c0: 2020 2020 2022 7469 746c 6522 3a20 2249       "title": "I
+000006d0: 5053 554d 222c 0d0a 2020 2020 2020 2020  PSUM",..        
+000006e0: 2020 2020 2274 6875 6d62 6e61 696c 223a      "thumbnail":
+000006f0: 2022 6874 7470 733a 2f2f 7069 6373 756d   "https://picsum
+00000700: 2e70 686f 746f 732f 3335 302f 3335 303f  .photos/350/350?
+00000710: 7261 6e64 6f6d 3d32 222c 0d0a 2020 2020  random=2",..    
+00000720: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00000730: 7469 6f6e 223a 2022 5365 6420 6e69 736c  tion": "Sed nisl
+00000740: 2061 7263 7520 6575 6973 6d6f 6420 7369   arcu euismod si
+00000750: 7420 616d 6574 206e 6973 6920 6c6f 7265  t amet nisi lore
+00000760: 6d20 6574 6961 6d20 646f 6c6f 7220 7665  m etiam dolor ve
+00000770: 726f 6572 6f73 2065 7420 6665 7567 6961  roeros et feugia
+00000780: 742e 222c 0d0a 2020 2020 2020 2020 2020  t.",..          
+00000790: 2020 2270 6167 6522 3a20 2270 6f73 745f    "page": "post_
+000007a0: 7465 6d70 6c61 7465 2e68 746d 6c22 0d0a  template.html"..
+000007b0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
+000007c0: 2020 2020 2270 6f73 7438 223a 207b 0d0a      "post8": {..
+000007d0: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
+000007e0: 6c65 223a 2022 444f 4c4f 5222 2c0d 0a20  le": "DOLOR",.. 
+000007f0: 2020 2020 2020 2020 2020 2022 7468 756d             "thum
+00000800: 626e 6169 6c22 3a20 2268 7474 7073 3a2f  bnail": "https:/
+00000810: 2f70 6963 7375 6d2e 7068 6f74 6f73 2f33  /picsum.photos/3
+00000820: 3530 2f33 3530 3f72 616e 646f 6d3d 3222  50/350?random=2"
+00000830: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000840: 6465 7363 7269 7074 696f 6e22 3a20 2253  description": "S
+00000850: 6564 206e 6973 6c20 6172 6375 2065 7569  ed nisl arcu eui
+00000860: 736d 6f64 2073 6974 2061 6d65 7420 6e69  smod sit amet ni
+00000870: 7369 206c 6f72 656d 2065 7469 616d 2064  si lorem etiam d
+00000880: 6f6c 6f72 2076 6572 6f65 726f 7320 6574  olor veroeros et
+00000890: 2066 6575 6769 6174 2e22 2c0d 0a20 2020   feugiat.",..   
+000008a0: 2020 2020 2020 2020 2022 7061 6765 223a           "page":
+000008b0: 2022 706f 7374 5f74 656d 706c 6174 652e   "post_template.
+000008c0: 6874 6d6c 220d 0a20 2020 2020 2020 207d  html"..        }
+000008d0: 2c0d 0a20 2020 2020 2020 2022 706f 7374  ,..        "post
+000008e0: 3922 3a20 7b0d 0a20 2020 2020 2020 2020  9": {..         
+000008f0: 2020 2022 7469 746c 6522 3a20 224e 554c     "title": "NUL
+00000900: 4c41 4d22 2c0d 0a20 2020 2020 2020 2020  LAM",..         
+00000910: 2020 2022 7468 756d 626e 6169 6c22 3a20     "thumbnail": 
+00000920: 2268 7474 7073 3a2f 2f70 6963 7375 6d2e  "https://picsum.
+00000930: 7068 6f74 6f73 2f33 3530 2f33 3530 3f72  photos/350/350?r
+00000940: 616e 646f 6d3d 3222 2c0d 0a20 2020 2020  andom=2",..     
+00000950: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00000960: 696f 6e22 3a20 2253 6564 206e 6973 6c20  ion": "Sed nisl 
+00000970: 6172 6375 2065 7569 736d 6f64 2073 6974  arcu euismod sit
+00000980: 2061 6d65 7420 6e69 7369 206c 6f72 656d   amet nisi lorem
+00000990: 2065 7469 616d 2064 6f6c 6f72 2076 6572   etiam dolor ver
+000009a0: 6f65 726f 7320 6574 2066 6575 6769 6174  oeros et feugiat
+000009b0: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+000009c0: 2022 7061 6765 223a 2022 706f 7374 5f74   "page": "post_t
+000009d0: 656d 706c 6174 652e 6874 6d6c 220d 0a20  emplate.html".. 
+000009e0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+000009f0: 2020 2022 706f 7374 3130 223a 207b 0d0a     "post10": {..
+00000a00: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
+00000a10: 6c65 223a 2022 554c 5452 4943 4945 5322  le": "ULTRICIES"
+00000a20: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000a30: 7468 756d 626e 6169 6c22 3a20 2268 7474  thumbnail": "htt
+00000a40: 7073 3a2f 2f70 6963 7375 6d2e 7068 6f74  ps://picsum.phot
+00000a50: 6f73 2f33 3530 2f33 3530 3f72 616e 646f  os/350/350?rando
+00000a60: 6d3d 3222 2c0d 0a20 2020 2020 2020 2020  m=2",..         
+00000a70: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000a80: 3a20 2253 6564 206e 6973 6c20 6172 6375  : "Sed nisl arcu
+00000a90: 2065 7569 736d 6f64 2073 6974 2061 6d65   euismod sit ame
+00000aa0: 7420 6e69 7369 206c 6f72 656d 2065 7469  t nisi lorem eti
+00000ab0: 616d 2064 6f6c 6f72 2076 6572 6f65 726f  am dolor veroero
+00000ac0: 7320 6574 2066 6575 6769 6174 2e22 2c0d  s et feugiat.",.
+00000ad0: 0a20 2020 2020 2020 2020 2020 2022 7061  .            "pa
+00000ae0: 6765 223a 2022 706f 7374 5f74 656d 706c  ge": "post_templ
+00000af0: 6174 652e 6874 6d6c 220d 0a20 2020 2020  ate.html"..     
+00000b00: 2020 207d 2c0d 0a20 2020 2020 2020 2022     },..        "
+00000b10: 706f 7374 3131 223a 207b 0d0a 2020 2020  post11": {..    
+00000b20: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
+00000b30: 2022 4449 4354 554d 222c 0d0a 2020 2020   "DICTUM",..    
+00000b40: 2020 2020 2020 2020 2274 6875 6d62 6e61          "thumbna
+00000b50: 696c 223a 2022 6874 7470 733a 2f2f 7069  il": "https://pi
+00000b60: 6373 756d 2e70 686f 746f 732f 3335 302f  csum.photos/350/
+00000b70: 3335 303f 7261 6e64 6f6d 3d32 222c 0d0a  350?random=2",..
+00000b80: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00000b90: 6372 6970 7469 6f6e 223a 2022 5365 6420  cription": "Sed 
+00000ba0: 6e69 736c 2061 7263 7520 6575 6973 6d6f  nisl arcu euismo
+00000bb0: 6420 7369 7420 616d 6574 206e 6973 6920  d sit amet nisi 
+00000bc0: 6c6f 7265 6d20 6574 6961 6d20 646f 6c6f  lorem etiam dolo
+00000bd0: 7220 7665 726f 6572 6f73 2065 7420 6665  r veroeros et fe
+00000be0: 7567 6961 742e 222c 0d0a 2020 2020 2020  ugiat.",..      
+00000bf0: 2020 2020 2020 2270 6167 6522 3a20 2270        "page": "p
+00000c00: 6f73 745f 7465 6d70 6c61 7465 2e68 746d  ost_template.htm
+00000c10: 6c22 0d0a 2020 2020 2020 2020 7d2c 0d0a  l"..        },..
+00000c20: 2020 2020 2020 2020 2270 6f73 7431 3222          "post12"
+00000c30: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00000c40: 2022 7469 746c 6522 3a20 2250 5245 5449   "title": "PRETI
+00000c50: 554d 222c 0d0a 2020 2020 2020 2020 2020  UM",..          
+00000c60: 2020 2274 6875 6d62 6e61 696c 223a 2022    "thumbnail": "
+00000c70: 6874 7470 733a 2f2f 7069 6373 756d 2e70  https://picsum.p
+00000c80: 686f 746f 732f 3335 302f 3335 303f 7261  hotos/350/350?ra
+00000c90: 6e64 6f6d 3d32 222c 0d0a 2020 2020 2020  ndom=2",..      
+00000ca0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000cb0: 6f6e 223a 2022 5365 6420 6e69 736c 2061  on": "Sed nisl a
+00000cc0: 7263 7520 6575 6973 6d6f 6420 7369 7420  rcu euismod sit 
+00000cd0: 616d 6574 206e 6973 6920 6c6f 7265 6d20  amet nisi lorem 
+00000ce0: 6574 6961 6d20 646f 6c6f 7220 7665 726f  etiam dolor vero
+00000cf0: 6572 6f73 2065 7420 6665 7567 6961 742e  eros et feugiat.
+00000d00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000d10: 2270 6167 6522 3a20 2270 6f73 745f 7465  "page": "post_te
+00000d20: 6d70 6c61 7465 2e68 746d 6c22 0d0a 2020  mplate.html"..  
+00000d30: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
+00000d40: 7d                                       }
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/phantom/static.py` & `jamstack-1.1.0/jamstack/sites/html5up/massively/static.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,42 @@
-# https://github.com/pymug/website-AV19-AV20
-
-import sys
+import argparse
 from os.path import join
 
+from livereload import Server
+
 import settings
-from flask import Flask
-from jamstack.api.template import base_context, generate
+from jamstack.api.template import generate
 from jamstack.jamdo.jamdo import download as download_template
-from livereload import Server
 
-context = base_context()
-context.update({
-    "info": settings.info,
-    "posts": settings.posts
-})
-
-
-def main(args):
-    def gen():
-        generate('index.html', join(
-            settings.OUTPUT_FOLDER, 'index.html'), **context)
-
-        # Generate pages based in sidebar items
-        sidebar = settings.info['sidebar']
-        for item in sidebar:
-            page = sidebar[item]['page']
-            generate(page, join(settings.OUTPUT_FOLDER, page), **context)
-
-        # Generate posts pages
-        posts = settings.posts['posts']
-        for post in posts:
-            page = posts[post]['page']
-            generate(page, join(
-                settings.OUTPUT_FOLDER, page), **context)
-
-    if len(args) > 1 and args[1] == '--server':
-        app = Flask(__name__)
-
-        # remember to use DEBUG mode for templates auto reload
-        # https://github.com/lepture/python-livereload/issues/144
-        app.debug = True
-        server = Server(app.wsgi_app)
-
-        # run a shell command
-        # server.watch('.', 'make static')
-
-        # run a function
-
-        server.watch('.', gen, delay=5)
-        server.watch('*.py')
-
-        # output stdout into a file
-        # server.watch('style.less', shell('lessc style.less',\
-        # output='style.css'))
-
-        server.serve()
-    elif len(args) > 1 and args[1] == '--jamdo':
-        download_template('html5up/phantom')
-    else:
-        gen()
+
+def generate_site():
+    extra_context = {"info": settings.info}
+
+    generate('index.html', join(settings.OUTPUT_FOLDER, 'index.html'), context=extra_context)
+    generate('index2.html', join(settings.OUTPUT_FOLDER, 'index2.html'), context=extra_context)
+    generate('index3.html', join(settings.OUTPUT_FOLDER, 'index3.html'), context=extra_context)
+
+
+def serve_files(port, watch):
+    server = Server()
+    for x in watch.split('|'):
+        server.watch(x, func=generate_site)
+    try:
+        server.serve(root=settings.OUTPUT_FOLDER, port=port)
+    except KeyboardInterrupt:
+        print("Shutting down...")
 
 
 if __name__ == '__main__':
-    main(sys.argv)
+    parser = argparse.ArgumentParser(description='Project manager.')
+    parser.add_argument('--serve', action='store_true', help='Serve files for livewatch')
+    parser.add_argument('--jamdo', action='store_true', help='Download template assets')
+    parser.add_argument('--watch', type=str, default='*.py|templates|templates/sections', help='Files/Folders to watch')
+    parser.add_argument('--port', type=int, default=8000, help='Port to serve')
+    args = parser.parse_args()
+
+    if args.serve:
+        serve_files(args.port, args.watch)
+    elif args.jamdo:
+        download_template('html5up/massively')
+    else:
+        generate_site()
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/elements.html` & `jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/elements.html`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-<!DOCTYPE HTML>
-<!--
-	Phantom by HTML5 UP
-	html5up.net | @ajlkn
-	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
--->
-<html>
-	<head>
-		<title>Elements - Phantom by HTML5 UP</title>
-		<meta charset="utf-8" />
-		<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
-		<link rel="stylesheet" href="assets/css/main.css" />
-		<noscript><link rel="stylesheet" href="assets/css/noscript.css" /></noscript>
-	</head>
-	<body class="is-preload">
-		<!-- Wrapper -->
-		<div id="wrapper">
-			<!-- Header -->
-			<header id="header">
-				<div class="inner">
-					<!-- Logo -->
-					<a href="index.html" class="logo">
-						<span class="symbol"><img src="{{ info['logo'] }}" alt="" /></span><span class="title">Phantom</span>
-					</a>
-					<!-- Nav -->
-					<nav>
-						<ul>
-							<li><a href="#menu">Menu</a></li>
-						</ul>
-					</nav>
-				</div>
-			</header>
-			<!-- Menu -->
-			<nav id="menu">
-				<h2>Menu</h2>
-				<ul>
-					<li><a href="index.html">Home</a></li>
-					<li><a href="generic.html">Ipsum veroeros</a></li>
-					<li><a href="generic.html">Tempus etiam</a></li>
-					<li><a href="generic.html">Consequat dolor</a></li>
-					<li><a href="elements.html">Elements</a></li>
-				</ul>
-			</nav>
-			<!-- Main -->
-			<div id="main">
-				<div class="inner">
-					<h1>Elements</h1>
-					<!-- Text -->
-					<section>
-						<h2>Text</h2>
-						<p>This is <b>bold</b> and this is <strong>strong</strong>. This is <i>italic</i> and this is <em>emphasized</em>.
-							This is <sup>superscript</sup> text and this is <sub>subscript</sub> text.
-							This is <u>underlined</u> and this is code: <code>for (;;) { ... }</code>. Finally, <a href="#">this is a link</a>.</p>
-							<hr />
-							<p>Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit tempus accumsan.</p>
-							<hr />
-							<h2>Heading Level 2</h2>
-							<h3>Heading Level 3</h3>
-							<h4>Heading Level 4</h4>
-							<hr />
-							<h3>Blockquote</h3>
-						<blockquote>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan faucibus. Vestibulum ante ipsum primis in faucibus lorem ipsum dolor sit amet nullam adipiscing eu felis.</blockquote>
-						<h3>Preformatted</h3>
-						<pre><code>i = 0;
-							while (!deck.isInOrder()) {
-							    print 'Iteration ' + i;
-							    deck.shuffle();
-							    i++;
-							}
-						print 'It took ' + i + ' iterations to sort the deck.';</code></pre>
-					</section>
-					<!-- Lists -->
-					<section>
-						<h2>Lists</h2>
-						<div class="row">
-							<div class="col-6 col-12-medium">
-								<h3>Unordered</h3>
-								<ul>
-									<li>Dolor pulvinar etiam.</li>
-									<li>Sagittis adipiscing.</li>
-									<li>Felis enim feugiat.</li>
-								</ul>
-								<h3>Alternate</h3>
-								<ul class="alt">
-									<li>Dolor pulvinar etiam.</li>
-									<li>Sagittis adipiscing.</li>
-									<li>Felis enim feugiat.</li>
-								</ul>
-							</div>
-							<div class="col-6 col-12-medium">
-								<h3>Ordered</h3>
-								<ol>
-									<li>Dolor pulvinar etiam.</li>
-									<li>Etiam vel felis viverra.</li>
-									<li>Felis enim feugiat.</li>
-									<li>Dolor pulvinar etiam.</li>
-									<li>Etiam vel felis lorem.</li>
-									<li>Felis enim et feugiat.</li>
-								</ol>
-								<h3>Icons</h3>
-								<ul class="icons">
-									<li><a href="#" class="icon brands style1 fa-twitter"><span class="label">Twitter</span></a></li>
-									<li><a href="#" class="icon brands style1 fa-facebook-f"><span class="label">Facebook</span></a></li>
-									<li><a href="#" class="icon brands style1 fa-instagram"><span class="label">Instagram</span></a></li>
-									<li><a href="#" class="icon brands style1 fa-github"><span class="label">Github</span></a></li>
-								</ul>
-								<ul class="icons">
-									<li><a href="#" class="icon brands style2 fa-twitter"><span class="label">Twitter</span></a></li>
-									<li><a href="#" class="icon brands style2 fa-facebook-f"><span class="label">Facebook</span></a></li>
-									<li><a href="#" class="icon brands style2 fa-instagram"><span class="label">Instagram</span></a></li>
-									<li><a href="#" class="icon brands style2 fa-github"><span class="label">Github</span></a></li>
-								</ul>
-							</div>
-						</div>
-						<h2>Actions</h2>
-						<div class="row">
-							<div class="col-6 col-12-medium">
-								<ul class="actions">
-									<li><a href="#" class="button primary">Default</a></li>
-									<li><a href="#" class="button">Default</a></li>
-								</ul>
-								<ul class="actions small">
-									<li><a href="#" class="button primary small">Small</a></li>
-									<li><a href="#" class="button small">Small</a></li>
-								</ul>
-								<ul class="actions stacked">
-									<li><a href="#" class="button primary">Default</a></li>
-									<li><a href="#" class="button">Default</a></li>
-								</ul>
-								<ul class="actions stacked">
-									<li><a href="#" class="button primary small">Small</a></li>
-									<li><a href="#" class="button small">Small</a></li>
-								</ul>
-							</div>
-							<div class="col-6 col-12-medium">
-								<ul class="actions stacked">
-									<li><a href="#" class="button primary fit">Default</a></li>
-									<li><a href="#" class="button fit">Default</a></li>
-								</ul>
-								<ul class="actions stacked">
-									<li><a href="#" class="button primary small fit">Small</a></li>
-									<li><a href="#" class="button small fit">Small</a></li>
-								</ul>
-							</div>
-						</div>
-					</section>
-					<!-- Table -->
-					<section>
-						<h2>Table</h2>
-						<h3>Default</h3>
-						<div class="table-wrapper">
-							<table>
-								<thead>
-									<tr>
-										<th>Name</th>
-										<th>Description</th>
-										<th>Price</th>
-									</tr>
-								</thead>
-								<tbody>
-									<tr>
-										<td>Item One</td>
-										<td>Ante turpis integer aliquet porttitor.</td>
-										<td>29.99</td>
-									</tr>
-									<tr>
-										<td>Item Two</td>
-										<td>Vis ac commodo adipiscing arcu aliquet.</td>
-										<td>19.99</td>
-									</tr>
-									<tr>
-										<td>Item Three</td>
-										<td> Morbi faucibus arcu accumsan lorem.</td>
-										<td>29.99</td>
-									</tr>
-									<tr>
-										<td>Item Four</td>
-										<td>Vitae integer tempus condimentum.</td>
-										<td>19.99</td>
-									</tr>
-									<tr>
-										<td>Item Five</td>
-										<td>Ante turpis integer aliquet porttitor.</td>
-										<td>29.99</td>
-									</tr>
-								</tbody>
-								<tfoot>
-								<tr>
-									<td colspan="2"></td>
-									<td>100.00</td>
-								</tr>
-								</tfoot>
-							</table>
-						</div>
-						<h3>Alternate</h3>
-						<div class="table-wrapper">
-							<table class="alt">
-								<thead>
-									<tr>
-										<th>Name</th>
-										<th>Description</th>
-										<th>Price</th>
-									</tr>
-								</thead>
-								<tbody>
-									<tr>
-										<td>Item One</td>
-										<td>Ante turpis integer aliquet porttitor.</td>
-										<td>29.99</td>
-									</tr>
-									<tr>
-										<td>Item Two</td>
-										<td>Vis ac commodo adipiscing arcu aliquet.</td>
-										<td>19.99</td>
-									</tr>
-									<tr>
-										<td>Item Three</td>
-										<td> Morbi faucibus arcu accumsan lorem.</td>
-										<td>29.99</td>
-									</tr>
-									<tr>
-										<td>Item Four</td>
-										<td>Vitae integer tempus condimentum.</td>
-										<td>19.99</td>
-									</tr>
-									<tr>
-										<td>Item Five</td>
-										<td>Ante turpis integer aliquet porttitor.</td>
-										<td>29.99</td>
-									</tr>
-								</tbody>
-								<tfoot>
-								<tr>
-									<td colspan="2"></td>
-									<td>100.00</td>
-								</tr>
-								</tfoot>
-							</table>
-						</div>
-					</section>
-					<!-- Buttons -->
-					<section>
-						<h3>Buttons</h3>
-						<ul class="actions">
-							<li><a href="#" class="button primary">Primary</a></li>
-							<li><a href="#" class="button">Default</a></li>
-						</ul>
-						<ul class="actions">
-							<li><a href="#" class="button large">Large</a></li>
-							<li><a href="#" class="button">Default</a></li>
-							<li><a href="#" class="button small">Small</a></li>
-						</ul>
-						<ul class="actions fit">
-							<li><a href="#" class="button primary fit">Fit</a></li>
-							<li><a href="#" class="button fit">Fit</a></li>
-							<li><a href="#" class="button fit">Fit</a></li>
-						</ul>
-						<ul class="actions fit small">
-							<li><a href="#" class="button primary fit small">Fit + Small</a></li>
-							<li><a href="#" class="button fit small">Fit + Small</a></li>
-							<li><a href="#" class="button fit small">Fit + Small</a></li>
-						</ul>
-						<ul class="actions">
-							<li><a href="#" class="button primary icon solid fa-download">Icon</a></li>
-							<li><a href="#" class="button icon solid fa-upload">Icon</a></li>
-							<li><a href="#" class="button icon solid fa-save">Icon</a></li>
-						</ul>
-						<ul class="actions">
-							<li><span class="button primary disabled">Disabled</span></li>
-							<li><span class="button disabled">Disabled</span></li>
-						</ul>
-					</section>
-					<!-- Form -->
-					<section>
-						<h2>Form</h2>
-						<form method="post" action="#">
-							<div class="row gtr-uniform">
-								<div class="col-6 col-12-xsmall">
-									<input type="text" name="demo-name" id="demo-name" value="" placeholder="Name" />
-								</div>
-								<div class="col-6 col-12-xsmall">
-									<input type="email" name="demo-email" id="demo-email" value="" placeholder="Email" />
-								</div>
-								<div class="col-12">
-									<select name="demo-category" id="demo-category">
-										<option value="">- Category -</option>
-										<option value="1">Manufacturing</option>
-										<option value="1">Shipping</option>
-										<option value="1">Administration</option>
-										<option value="1">Human Resources</option>
-									</select>
-								</div>
-								<div class="col-4 col-12-small">
-									<input type="radio" id="demo-priority-low" name="demo-priority" checked>
-									<label for="demo-priority-low">Low</label>
-								</div>
-								<div class="col-4 col-12-small">
-									<input type="radio" id="demo-priority-normal" name="demo-priority">
-									<label for="demo-priority-normal">Normal</label>
-								</div>
-								<div class="col-4 col-12-small">
-									<input type="radio" id="demo-priority-high" name="demo-priority">
-									<label for="demo-priority-high">High</label>
-								</div>
-								<div class="col-6 col-12-small">
-									<input type="checkbox" id="demo-copy" name="demo-copy">
-									<label for="demo-copy">Email me a copy</label>
-								</div>
-								<div class="col-6 col-12-small">
-									<input type="checkbox" id="demo-human" name="demo-human" checked>
-									<label for="demo-human">Not a robot</label>
-								</div>
-								<div class="col-12">
-									<textarea name="demo-message" id="demo-message" placeholder="Enter your message" rows="6"></textarea>
-								</div>
-								<div class="col-12">
-									<ul class="actions">
-										<li><input type="submit" value="Send Message" class="primary" /></li>
-										<li><input type="reset" value="Reset" /></li>
-									</ul>
-								</div>
-							</div>
-						</form>
-					</section>
-					<!-- Image -->
-					<section>
-						<h2>Image</h2>
-						<h3>Fit</h3>
-						<div class="box alt">
-							<div class="row gtr-uniform">
-								<div class="col-12"><span class="image fit"><img src="https://picsum.photos/1132/326?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
-							</div>
-						</div>
-						<h3>Left &amp; Right</h3>
-						<p><span class="image left"><img src="https://picsum.photos/177/163/?blur=2?random=2" alt="" /></span>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.</p>
-						<p><span class="image right"><img src="https://picsum.photos/177/163/?blur=2?random=2" alt="" /></span>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.</p>
-					</section>
-				</div>
-			</div>
-			<!-- Footer -->
-			<footer id="footer">
-				<div class="inner">
-					<section>
-						<h2>Get in touch</h2>
-						<form method="post" action="#">
-							<div class="fields">
-								<div class="field half">
-									<input type="text" name="name" id="name" placeholder="Name" />
-								</div>
-								<div class="field half">
-									<input type="email" name="email" id="email" placeholder="Email" />
-								</div>
-								<div class="field">
-									<textarea name="message" id="message" placeholder="Message"></textarea>
-								</div>
-							</div>
-							<ul class="actions">
-								<li><input type="submit" value="Send" class="primary" /></li>
-							</ul>
-						</form>
-					</section>
-					<section>
-						<h2>Follow</h2>
-						<ul class="icons">
-							<li><a href="#" class="icon brands style2 fa-twitter"><span class="label">Twitter</span></a></li>
-							<li><a href="#" class="icon brands style2 fa-facebook-f"><span class="label">Facebook</span></a></li>
-							<li><a href="#" class="icon brands style2 fa-instagram"><span class="label">Instagram</span></a></li>
-							<li><a href="#" class="icon brands style2 fa-dribbble"><span class="label">Dribbble</span></a></li>
-							<li><a href="#" class="icon brands style2 fa-github"><span class="label">GitHub</span></a></li>
-							<li><a href="#" class="icon brands style2 fa-500px"><span class="label">500px</span></a></li>
-							<li><a href="#" class="icon solid style2 fa-phone"><span class="label">Phone</span></a></li>
-							<li><a href="#" class="icon solid style2 fa-envelope"><span class="label">Email</span></a></li>
-						</ul>
-					</section>
-					<ul class="copyright">
-						<li>&copy; Untitled. All rights reserved</li><li>Design: <a href="http://html5up.net">HTML5 UP</a></li>
-					</ul>
-				</div>
-			</footer>
-		</div>
-		<!-- Scripts -->
-		<script src="assets/js/jquery.min.js"></script>
-		<script src="assets/js/browser.min.js"></script>
-		<script src="assets/js/breakpoints.min.js"></script>
-		<script src="assets/js/util.js"></script>
-		<script src="assets/js/main.js"></script>
-	</body>
+<!DOCTYPE HTML>
+<!--
+	Phantom by HTML5 UP
+	html5up.net | @ajlkn
+	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
+-->
+<html>
+	<head>
+		<title>Elements - Phantom by HTML5 UP</title>
+		<meta charset="utf-8" />
+		<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
+		<link rel="stylesheet" href="assets/css/main.css" />
+		<noscript><link rel="stylesheet" href="assets/css/noscript.css" /></noscript>
+	</head>
+	<body class="is-preload">
+		<!-- Wrapper -->
+		<div id="wrapper">
+			<!-- Header -->
+			<header id="header">
+				<div class="inner">
+					<!-- Logo -->
+					<a href="index.html" class="logo">
+						<span class="symbol"><img src="{{ info['logo'] }}" alt="" /></span><span class="title">Phantom</span>
+					</a>
+					<!-- Nav -->
+					<nav>
+						<ul>
+							<li><a href="#menu">Menu</a></li>
+						</ul>
+					</nav>
+				</div>
+			</header>
+			<!-- Menu -->
+			<nav id="menu">
+				<h2>Menu</h2>
+				<ul>
+					<li><a href="index.html">Home</a></li>
+					<li><a href="generic.html">Ipsum veroeros</a></li>
+					<li><a href="generic.html">Tempus etiam</a></li>
+					<li><a href="generic.html">Consequat dolor</a></li>
+					<li><a href="elements.html">Elements</a></li>
+				</ul>
+			</nav>
+			<!-- Main -->
+			<div id="main">
+				<div class="inner">
+					<h1>Elements</h1>
+					<!-- Text -->
+					<section>
+						<h2>Text</h2>
+						<p>This is <b>bold</b> and this is <strong>strong</strong>. This is <i>italic</i> and this is <em>emphasized</em>.
+							This is <sup>superscript</sup> text and this is <sub>subscript</sub> text.
+							This is <u>underlined</u> and this is code: <code>for (;;) { ... }</code>. Finally, <a href="#">this is a link</a>.</p>
+							<hr />
+							<p>Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit tempus accumsan.</p>
+							<hr />
+							<h2>Heading Level 2</h2>
+							<h3>Heading Level 3</h3>
+							<h4>Heading Level 4</h4>
+							<hr />
+							<h3>Blockquote</h3>
+						<blockquote>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan faucibus. Vestibulum ante ipsum primis in faucibus lorem ipsum dolor sit amet nullam adipiscing eu felis.</blockquote>
+						<h3>Preformatted</h3>
+						<pre><code>i = 0;
+							while (!deck.isInOrder()) {
+							    print 'Iteration ' + i;
+							    deck.shuffle();
+							    i++;
+							}
+						print 'It took ' + i + ' iterations to sort the deck.';</code></pre>
+					</section>
+					<!-- Lists -->
+					<section>
+						<h2>Lists</h2>
+						<div class="row">
+							<div class="col-6 col-12-medium">
+								<h3>Unordered</h3>
+								<ul>
+									<li>Dolor pulvinar etiam.</li>
+									<li>Sagittis adipiscing.</li>
+									<li>Felis enim feugiat.</li>
+								</ul>
+								<h3>Alternate</h3>
+								<ul class="alt">
+									<li>Dolor pulvinar etiam.</li>
+									<li>Sagittis adipiscing.</li>
+									<li>Felis enim feugiat.</li>
+								</ul>
+							</div>
+							<div class="col-6 col-12-medium">
+								<h3>Ordered</h3>
+								<ol>
+									<li>Dolor pulvinar etiam.</li>
+									<li>Etiam vel felis viverra.</li>
+									<li>Felis enim feugiat.</li>
+									<li>Dolor pulvinar etiam.</li>
+									<li>Etiam vel felis lorem.</li>
+									<li>Felis enim et feugiat.</li>
+								</ol>
+								<h3>Icons</h3>
+								<ul class="icons">
+									<li><a href="#" class="icon brands style1 fa-twitter"><span class="label">Twitter</span></a></li>
+									<li><a href="#" class="icon brands style1 fa-facebook-f"><span class="label">Facebook</span></a></li>
+									<li><a href="#" class="icon brands style1 fa-instagram"><span class="label">Instagram</span></a></li>
+									<li><a href="#" class="icon brands style1 fa-github"><span class="label">Github</span></a></li>
+								</ul>
+								<ul class="icons">
+									<li><a href="#" class="icon brands style2 fa-twitter"><span class="label">Twitter</span></a></li>
+									<li><a href="#" class="icon brands style2 fa-facebook-f"><span class="label">Facebook</span></a></li>
+									<li><a href="#" class="icon brands style2 fa-instagram"><span class="label">Instagram</span></a></li>
+									<li><a href="#" class="icon brands style2 fa-github"><span class="label">Github</span></a></li>
+								</ul>
+							</div>
+						</div>
+						<h2>Actions</h2>
+						<div class="row">
+							<div class="col-6 col-12-medium">
+								<ul class="actions">
+									<li><a href="#" class="button primary">Default</a></li>
+									<li><a href="#" class="button">Default</a></li>
+								</ul>
+								<ul class="actions small">
+									<li><a href="#" class="button primary small">Small</a></li>
+									<li><a href="#" class="button small">Small</a></li>
+								</ul>
+								<ul class="actions stacked">
+									<li><a href="#" class="button primary">Default</a></li>
+									<li><a href="#" class="button">Default</a></li>
+								</ul>
+								<ul class="actions stacked">
+									<li><a href="#" class="button primary small">Small</a></li>
+									<li><a href="#" class="button small">Small</a></li>
+								</ul>
+							</div>
+							<div class="col-6 col-12-medium">
+								<ul class="actions stacked">
+									<li><a href="#" class="button primary fit">Default</a></li>
+									<li><a href="#" class="button fit">Default</a></li>
+								</ul>
+								<ul class="actions stacked">
+									<li><a href="#" class="button primary small fit">Small</a></li>
+									<li><a href="#" class="button small fit">Small</a></li>
+								</ul>
+							</div>
+						</div>
+					</section>
+					<!-- Table -->
+					<section>
+						<h2>Table</h2>
+						<h3>Default</h3>
+						<div class="table-wrapper">
+							<table>
+								<thead>
+									<tr>
+										<th>Name</th>
+										<th>Description</th>
+										<th>Price</th>
+									</tr>
+								</thead>
+								<tbody>
+									<tr>
+										<td>Item One</td>
+										<td>Ante turpis integer aliquet porttitor.</td>
+										<td>29.99</td>
+									</tr>
+									<tr>
+										<td>Item Two</td>
+										<td>Vis ac commodo adipiscing arcu aliquet.</td>
+										<td>19.99</td>
+									</tr>
+									<tr>
+										<td>Item Three</td>
+										<td> Morbi faucibus arcu accumsan lorem.</td>
+										<td>29.99</td>
+									</tr>
+									<tr>
+										<td>Item Four</td>
+										<td>Vitae integer tempus condimentum.</td>
+										<td>19.99</td>
+									</tr>
+									<tr>
+										<td>Item Five</td>
+										<td>Ante turpis integer aliquet porttitor.</td>
+										<td>29.99</td>
+									</tr>
+								</tbody>
+								<tfoot>
+								<tr>
+									<td colspan="2"></td>
+									<td>100.00</td>
+								</tr>
+								</tfoot>
+							</table>
+						</div>
+						<h3>Alternate</h3>
+						<div class="table-wrapper">
+							<table class="alt">
+								<thead>
+									<tr>
+										<th>Name</th>
+										<th>Description</th>
+										<th>Price</th>
+									</tr>
+								</thead>
+								<tbody>
+									<tr>
+										<td>Item One</td>
+										<td>Ante turpis integer aliquet porttitor.</td>
+										<td>29.99</td>
+									</tr>
+									<tr>
+										<td>Item Two</td>
+										<td>Vis ac commodo adipiscing arcu aliquet.</td>
+										<td>19.99</td>
+									</tr>
+									<tr>
+										<td>Item Three</td>
+										<td> Morbi faucibus arcu accumsan lorem.</td>
+										<td>29.99</td>
+									</tr>
+									<tr>
+										<td>Item Four</td>
+										<td>Vitae integer tempus condimentum.</td>
+										<td>19.99</td>
+									</tr>
+									<tr>
+										<td>Item Five</td>
+										<td>Ante turpis integer aliquet porttitor.</td>
+										<td>29.99</td>
+									</tr>
+								</tbody>
+								<tfoot>
+								<tr>
+									<td colspan="2"></td>
+									<td>100.00</td>
+								</tr>
+								</tfoot>
+							</table>
+						</div>
+					</section>
+					<!-- Buttons -->
+					<section>
+						<h3>Buttons</h3>
+						<ul class="actions">
+							<li><a href="#" class="button primary">Primary</a></li>
+							<li><a href="#" class="button">Default</a></li>
+						</ul>
+						<ul class="actions">
+							<li><a href="#" class="button large">Large</a></li>
+							<li><a href="#" class="button">Default</a></li>
+							<li><a href="#" class="button small">Small</a></li>
+						</ul>
+						<ul class="actions fit">
+							<li><a href="#" class="button primary fit">Fit</a></li>
+							<li><a href="#" class="button fit">Fit</a></li>
+							<li><a href="#" class="button fit">Fit</a></li>
+						</ul>
+						<ul class="actions fit small">
+							<li><a href="#" class="button primary fit small">Fit + Small</a></li>
+							<li><a href="#" class="button fit small">Fit + Small</a></li>
+							<li><a href="#" class="button fit small">Fit + Small</a></li>
+						</ul>
+						<ul class="actions">
+							<li><a href="#" class="button primary icon solid fa-download">Icon</a></li>
+							<li><a href="#" class="button icon solid fa-upload">Icon</a></li>
+							<li><a href="#" class="button icon solid fa-save">Icon</a></li>
+						</ul>
+						<ul class="actions">
+							<li><span class="button primary disabled">Disabled</span></li>
+							<li><span class="button disabled">Disabled</span></li>
+						</ul>
+					</section>
+					<!-- Form -->
+					<section>
+						<h2>Form</h2>
+						<form method="post" action="#">
+							<div class="row gtr-uniform">
+								<div class="col-6 col-12-xsmall">
+									<input type="text" name="demo-name" id="demo-name" value="" placeholder="Name" />
+								</div>
+								<div class="col-6 col-12-xsmall">
+									<input type="email" name="demo-email" id="demo-email" value="" placeholder="Email" />
+								</div>
+								<div class="col-12">
+									<select name="demo-category" id="demo-category">
+										<option value="">- Category -</option>
+										<option value="1">Manufacturing</option>
+										<option value="1">Shipping</option>
+										<option value="1">Administration</option>
+										<option value="1">Human Resources</option>
+									</select>
+								</div>
+								<div class="col-4 col-12-small">
+									<input type="radio" id="demo-priority-low" name="demo-priority" checked>
+									<label for="demo-priority-low">Low</label>
+								</div>
+								<div class="col-4 col-12-small">
+									<input type="radio" id="demo-priority-normal" name="demo-priority">
+									<label for="demo-priority-normal">Normal</label>
+								</div>
+								<div class="col-4 col-12-small">
+									<input type="radio" id="demo-priority-high" name="demo-priority">
+									<label for="demo-priority-high">High</label>
+								</div>
+								<div class="col-6 col-12-small">
+									<input type="checkbox" id="demo-copy" name="demo-copy">
+									<label for="demo-copy">Email me a copy</label>
+								</div>
+								<div class="col-6 col-12-small">
+									<input type="checkbox" id="demo-human" name="demo-human" checked>
+									<label for="demo-human">Not a robot</label>
+								</div>
+								<div class="col-12">
+									<textarea name="demo-message" id="demo-message" placeholder="Enter your message" rows="6"></textarea>
+								</div>
+								<div class="col-12">
+									<ul class="actions">
+										<li><input type="submit" value="Send Message" class="primary" /></li>
+										<li><input type="reset" value="Reset" /></li>
+									</ul>
+								</div>
+							</div>
+						</form>
+					</section>
+					<!-- Image -->
+					<section>
+						<h2>Image</h2>
+						<h3>Fit</h3>
+						<div class="box alt">
+							<div class="row gtr-uniform">
+								<div class="col-12"><span class="image fit"><img src="https://picsum.photos/1132/326?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+								<div class="col-4"><span class="image fit"><img src="https://picsum.photos/353/326/?blur=2?random=2" alt="" /></span></div>
+							</div>
+						</div>
+						<h3>Left &amp; Right</h3>
+						<p><span class="image left"><img src="https://picsum.photos/177/163/?blur=2?random=2" alt="" /></span>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.</p>
+						<p><span class="image right"><img src="https://picsum.photos/177/163/?blur=2?random=2" alt="" /></span>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.</p>
+					</section>
+				</div>
+			</div>
+			<!-- Footer -->
+			<footer id="footer">
+				<div class="inner">
+					<section>
+						<h2>Get in touch</h2>
+						<form method="post" action="#">
+							<div class="fields">
+								<div class="field half">
+									<input type="text" name="name" id="name" placeholder="Name" />
+								</div>
+								<div class="field half">
+									<input type="email" name="email" id="email" placeholder="Email" />
+								</div>
+								<div class="field">
+									<textarea name="message" id="message" placeholder="Message"></textarea>
+								</div>
+							</div>
+							<ul class="actions">
+								<li><input type="submit" value="Send" class="primary" /></li>
+							</ul>
+						</form>
+					</section>
+					<section>
+						<h2>Follow</h2>
+						<ul class="icons">
+							<li><a href="#" class="icon brands style2 fa-twitter"><span class="label">Twitter</span></a></li>
+							<li><a href="#" class="icon brands style2 fa-facebook-f"><span class="label">Facebook</span></a></li>
+							<li><a href="#" class="icon brands style2 fa-instagram"><span class="label">Instagram</span></a></li>
+							<li><a href="#" class="icon brands style2 fa-dribbble"><span class="label">Dribbble</span></a></li>
+							<li><a href="#" class="icon brands style2 fa-github"><span class="label">GitHub</span></a></li>
+							<li><a href="#" class="icon brands style2 fa-500px"><span class="label">500px</span></a></li>
+							<li><a href="#" class="icon solid style2 fa-phone"><span class="label">Phone</span></a></li>
+							<li><a href="#" class="icon solid style2 fa-envelope"><span class="label">Email</span></a></li>
+						</ul>
+					</section>
+					<ul class="copyright">
+						<li>&copy; Untitled. All rights reserved</li><li>Design: <a href="http://html5up.net">HTML5 UP</a></li>
+					</ul>
+				</div>
+			</footer>
+		</div>
+		<!-- Scripts -->
+		<script src="assets/js/jquery.min.js"></script>
+		<script src="assets/js/browser.min.js"></script>
+		<script src="assets/js/breakpoints.min.js"></script>
+		<script src="assets/js/util.js"></script>
+		<script src="assets/js/main.js"></script>
+	</body>
 </html>
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/generic.html` & `jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/generic.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-<!DOCTYPE HTML>
-<!--
-	Phantom by HTML5 UP
-	html5up.net | @ajlkn
-	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
--->
-<html>
-	<head>
-		{% include 'sections/head_content.html' %}
-		{% block head %}
-			<title>{{ info['pagename'] }} - Generic page</title>
-		{% endblock %}
-	</head>
-	<body class="is-preload">
-		<!-- Wrapper -->
-		<div id="wrapper">
-			<!-- Header -->
-			<header id="header">
-				<div class="inner">
-					<!-- Logo -->
-					<a href="index.html" class="logo">
-						<span class="symbol"><img src="{{ info['logo'] }}" alt="" /></span><span class="title">Phantom</span>
-					</a>
-					<!-- Nav -->
-					<nav>
-						<ul>
-							<li><a href="#menu">Menu</a></li>
-						</ul>
-					</nav>
-				</div>
-			</header>
-			<!-- Menu -->
-			<nav id="menu">
-				<h2>Menu</h2>
-				<ul>
-					{% for item in info['sidebar'] %}
-						{% set items = info['sidebar'] %}
-						{% set title = items[item]['title'] %}
-						{% set page = items[item]['page'] %}
-						<li><a href="{{ page }}">{{ title }}</a></li>
-					{% endfor %}
-				</ul>
-			</nav>
-			<!-- Main -->
-			<div id="main">
-				<div class="inner">
-					<h1>Generic Page</h1>
-					<span class="image main"><img src="https://picsum.photos/1132/326?blur=2?random=2" alt="" /></span>
-					<p>Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Curabitur sapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique.</p>
-					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis dapibus rutrum facilisis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam tristique libero eu nibh porttitor fermentum. Nullam venenatis erat id vehicula viverra. Nunc ultrices eros ut ultricies condimentum. Mauris risus lacus, blandit sit amet venenatis non, bibendum vitae dolor. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In non lorem sit amet elit placerat maximus. Pellentesque aliquam maximus risus, vel venenatis mauris vehicula hendrerit.</p>
-					<p>Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fersapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique lorem ipsum dolor.</p>
-				</div>
-			</div>
-			{% include 'sections/footer.html' %}
-		</div>
-		{% include 'sections/bottom_scripts.html' %}
-	</body>
+<!DOCTYPE HTML>
+<!--
+	Phantom by HTML5 UP
+	html5up.net | @ajlkn
+	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
+-->
+<html>
+	<head>
+		{% include 'sections/head_content.html' %}
+		{% block head %}
+			<title>{{ info['pagename'] }} - Generic page</title>
+		{% endblock %}
+	</head>
+	<body class="is-preload">
+		<!-- Wrapper -->
+		<div id="wrapper">
+			<!-- Header -->
+			<header id="header">
+				<div class="inner">
+					<!-- Logo -->
+					<a href="index.html" class="logo">
+						<span class="symbol"><img src="{{ info['logo'] }}" alt="" /></span><span class="title">Phantom</span>
+					</a>
+					<!-- Nav -->
+					<nav>
+						<ul>
+							<li><a href="#menu">Menu</a></li>
+						</ul>
+					</nav>
+				</div>
+			</header>
+			<!-- Menu -->
+			<nav id="menu">
+				<h2>Menu</h2>
+				<ul>
+					{% for item in info['sidebar'] %}
+						{% set items = info['sidebar'] %}
+						{% set title = items[item]['title'] %}
+						{% set page = items[item]['page'] %}
+						<li><a href="{{ page }}">{{ title }}</a></li>
+					{% endfor %}
+				</ul>
+			</nav>
+			<!-- Main -->
+			<div id="main">
+				<div class="inner">
+					<h1>Generic Page</h1>
+					<span class="image main"><img src="https://picsum.photos/1132/326?blur=2?random=2" alt="" /></span>
+					<p>Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Curabitur sapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique.</p>
+					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis dapibus rutrum facilisis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam tristique libero eu nibh porttitor fermentum. Nullam venenatis erat id vehicula viverra. Nunc ultrices eros ut ultricies condimentum. Mauris risus lacus, blandit sit amet venenatis non, bibendum vitae dolor. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In non lorem sit amet elit placerat maximus. Pellentesque aliquam maximus risus, vel venenatis mauris vehicula hendrerit.</p>
+					<p>Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fersapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique lorem ipsum dolor.</p>
+				</div>
+			</div>
+			{% include 'sections/footer.html' %}
+		</div>
+		{% include 'sections/bottom_scripts.html' %}
+	</body>
 </html>
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/post_template.html` & `jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/post_template.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-<!DOCTYPE HTML>
-<!--
-	Phantom by HTML5 UP
-	html5up.net | @ajlkn
-	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
--->
-<html>
-	<head>
-		{% include 'sections/head_content.html' %}
-		{% block head %}
-			<title>{{ info['pagename'] }} POST</title>
-		{% endblock %}
-	</head>
-	<body class="is-preload">
-		<!-- Wrapper -->
-		<div id="wrapper">
-			<!-- Header -->
-			<header id="header">
-				<div class="inner">
-					<!-- Logo -->
-					<a href="index.html" class="logo">
-						<span class="symbol"><img src="{{ info['logo'] }}" alt="" /></span><span class="title">{{ info['pagename'] }}</span>
-					</a>
-					<!-- Nav -->
-					<nav>
-						<ul>
-							<li><a href="#menu">Menu</a></li>
-						</ul>
-					</nav>
-				</div>
-			</header>
-			<!-- Menu -->
-			<nav id="menu">
-				<h2>Menu</h2>
-				<ul>
-					{% for item in info['sidebar'] %}
-						{% set items = info['sidebar'] %}
-						{% set title = items[item]['title'] %}
-						{% set page = items[item]['page'] %}
-						<li><a href="{{ page }}">{{ title }}</a></li>
-					{% endfor %}
-				</ul>
-			</nav>
-			<!-- Main -->
-			<div id="main">
-				<div class="inner">
-					<h1>LOREM IPSUM POST</h1>
-					<span class="image main"><img src="https://picsum.photos/1132/326?blur=2?random=2" alt="" /></span>
-					<p>Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Curabitur sapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique.</p>
-					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis dapibus rutrum facilisis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam tristique libero eu nibh porttitor fermentum. Nullam venenatis erat id vehicula viverra. Nunc ultrices eros ut ultricies condimentum. Mauris risus lacus, blandit sit amet venenatis non, bibendum vitae dolor. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In non lorem sit amet elit placerat maximus. Pellentesque aliquam maximus risus, vel venenatis mauris vehicula hendrerit.</p>
-				</div>
-			</div>
-			{% include 'sections/footer.html' %}
-		</div>
-		{% include 'sections/bottom_scripts.html' %}
-	</body>
+<!DOCTYPE HTML>
+<!--
+	Phantom by HTML5 UP
+	html5up.net | @ajlkn
+	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
+-->
+<html>
+	<head>
+		{% include 'sections/head_content.html' %}
+		{% block head %}
+			<title>{{ info['pagename'] }} POST</title>
+		{% endblock %}
+	</head>
+	<body class="is-preload">
+		<!-- Wrapper -->
+		<div id="wrapper">
+			<!-- Header -->
+			<header id="header">
+				<div class="inner">
+					<!-- Logo -->
+					<a href="index.html" class="logo">
+						<span class="symbol"><img src="{{ info['logo'] }}" alt="" /></span><span class="title">{{ info['pagename'] }}</span>
+					</a>
+					<!-- Nav -->
+					<nav>
+						<ul>
+							<li><a href="#menu">Menu</a></li>
+						</ul>
+					</nav>
+				</div>
+			</header>
+			<!-- Menu -->
+			<nav id="menu">
+				<h2>Menu</h2>
+				<ul>
+					{% for item in info['sidebar'] %}
+						{% set items = info['sidebar'] %}
+						{% set title = items[item]['title'] %}
+						{% set page = items[item]['page'] %}
+						<li><a href="{{ page }}">{{ title }}</a></li>
+					{% endfor %}
+				</ul>
+			</nav>
+			<!-- Main -->
+			<div id="main">
+				<div class="inner">
+					<h1>LOREM IPSUM POST</h1>
+					<span class="image main"><img src="https://picsum.photos/1132/326?blur=2?random=2" alt="" /></span>
+					<p>Donec eget ex magna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Pellentesque venenatis dolor imperdiet dolor mattis sagittis. Praesent rutrum sem diam, vitae egestas enim auctor sit amet. Pellentesque leo mauris, consectetur id ipsum sit amet, fergiat. Pellentesque in mi eu massa lacinia malesuada et a elit. Donec urna ex, lacinia in purus ac, pretium pulvinar mauris. Curabitur sapien risus, commodo eget turpis at, elementum convallis elit. Pellentesque enim turpis, hendrerit tristique.</p>
+					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis dapibus rutrum facilisis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Etiam tristique libero eu nibh porttitor fermentum. Nullam venenatis erat id vehicula viverra. Nunc ultrices eros ut ultricies condimentum. Mauris risus lacus, blandit sit amet venenatis non, bibendum vitae dolor. Nunc lorem mauris, fringilla in aliquam at, euismod in lectus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In non lorem sit amet elit placerat maximus. Pellentesque aliquam maximus risus, vel venenatis mauris vehicula hendrerit.</p>
+				</div>
+			</div>
+			{% include 'sections/footer.html' %}
+		</div>
+		{% include 'sections/bottom_scripts.html' %}
+	</body>
 </html>
```

### Comparing `jamstack-1.0.0/jamstack/sites/html5up/phantom/templates/sections/footer.html` & `jamstack-1.1.0/jamstack/sites/html5up/phantom/templates/sections/footer.html`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-<footer id="footer">
-	<div class="inner">
-		<section>
-			<h2>Get in touch</h2>
-			<form method="post" action="#">
-				<div class="fields">
-					<div class="field half">
-						<input type="text" name="name" id="name" placeholder="Name" />
-					</div>
-					<div class="field half">
-						<input type="email" name="email" id="email" placeholder="Email" />
-					</div>
-					<div class="field">
-						<textarea name="message" id="message" placeholder="Message"></textarea>
-					</div>
-				</div>
-				<ul class="actions">
-					<li><input type="submit" value="Send" class="primary" /></li>
-				</ul>
-			</form>
-		</section>
-		<section>
-			<h2>Follow</h2>
-			<ul class="icons">
-				{% for item in info['social'] %}
-					<li><a href="{{ info['social'][item]['url'] }}" class="icon {{ info['social'][item]['icon-type'] }} style2 fa-{{ item }}"><span class="label">{{ info['social'][item]['title'] }}</span></a></li>
-				{% endfor %}
-			</ul>
-		</section>
-		<ul class="copyright">
-			<li>&copy; Untitled. All rights reserved</li><li>Design: <a href="http://html5up.net">HTML5 UP</a></li>
-		</ul>
-	</div>
+<footer id="footer">
+	<div class="inner">
+		<section>
+			<h2>Get in touch</h2>
+			<form method="post" action="#">
+				<div class="fields">
+					<div class="field half">
+						<input type="text" name="name" id="name" placeholder="Name" />
+					</div>
+					<div class="field half">
+						<input type="email" name="email" id="email" placeholder="Email" />
+					</div>
+					<div class="field">
+						<textarea name="message" id="message" placeholder="Message"></textarea>
+					</div>
+				</div>
+				<ul class="actions">
+					<li><input type="submit" value="Send" class="primary" /></li>
+				</ul>
+			</form>
+		</section>
+		<section>
+			<h2>Follow</h2>
+			<ul class="icons">
+				{% for item in info['social'] %}
+					<li><a href="{{ info['social'][item]['url'] }}" class="icon {{ info['social'][item]['icon-type'] }} style2 fa-{{ item }}"><span class="label">{{ info['social'][item]['title'] }}</span></a></li>
+				{% endfor %}
+			</ul>
+		</section>
+		<ul class="copyright">
+			<li>&copy; Untitled. All rights reserved</li><li>Design: <a href="http://html5up.net">HTML5 UP</a></li>
+		</ul>
+	</div>
 </footer>
```

### Comparing `jamstack-1.0.0/jamstack/sites/plain/templates/sections/head.html` & `jamstack-1.1.0/jamstack/sites/plain/templates/sections/head.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-<title>web and software dev</title>
-<meta name="viewport" content="width=device-width, initial-scale=1.0">
-<meta charset="utf-8">
-<meta name="description" content="{{ info['head']['description'] }}">
-<meta name="keywords" content="{{ info['head']['keywords'] }}">
-<meta name="author" content="{{ info['head']['author'] }}">
-<meta name="theme-color" content="{{ info['head']['theme-color'] }}" />
-<link rel="icon" href="">
-<script type="text/javascript" src="js/script.js"></script>
-<link rel="stylesheet" type="text/css" href="css/styles.css">
+<title>Jamstack Plain Site</title>
+<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
+<meta http-equiv="X-UA-Compatible" content="ie=edge">
+<meta charset="utf-8">
+<meta name="description" content="{{ info['head']['description'] }}">
+<meta name="keywords" content="{{ info['head']['keywords'] }}">
+<meta name="author" content="{{ info['head']['author'] }}">
+<meta name="theme-color" content="{{ info['head']['theme-color'] }}" />
+<link rel="icon" href="">
+<script type="text/javascript" src="js/script.js"></script>
+<link rel="stylesheet" type="text/css" href="css/styles.css">
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
 
 
 
 
 
 
 
+
+
```

### Comparing `jamstack-1.0.0/jamstack.egg-info/SOURCES.txt` & `jamstack-1.1.0/jamstack.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 jamstack/__main__.py
 jamstack.egg-info/PKG-INFO
 jamstack.egg-info/SOURCES.txt
 jamstack.egg-info/dependency_links.txt
 jamstack.egg-info/entry_points.txt
 jamstack.egg-info/requires.txt
 jamstack.egg-info/top_level.txt
-jamstack/__pycache__/__init__.cpython-39.pyc
-jamstack/__pycache__/__main__.cpython-39.pyc
+jamstack/__pycache__/__init__.cpython-38.pyc
+jamstack/__pycache__/__main__.cpython-38.pyc
 jamstack/api/file.py
 jamstack/api/template.py
-jamstack/api/__pycache__/file.cpython-39.pyc
-jamstack/api/__pycache__/template.cpython-39.pyc
+jamstack/api/__pycache__/file.cpython-38.pyc
+jamstack/api/__pycache__/template.cpython-38.pyc
 jamstack/jamdo/jamdo.py
-jamstack/jamdo/__pycache__/jamdo.cpython-39.pyc
+jamstack/jamdo/__pycache__/jamdo.cpython-38.pyc
 jamstack/sites/html5up/massively/info.json
 jamstack/sites/html5up/massively/settings.py
 jamstack/sites/html5up/massively/static.py
 jamstack/sites/html5up/massively/templates/index.html
 jamstack/sites/html5up/massively/templates/index2.html
 jamstack/sites/html5up/massively/templates/index3.html
 jamstack/sites/html5up/massively/templates/sections/bottom_scripts.html
```

### Comparing `jamstack-1.0.0/setup.py` & `jamstack-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import os
 import sys
 
-from jamstack import __version__
 from setuptools import setup
 
+from jamstack import __version__
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 if sys.argv[-1] == "publish":
-    os.system("python3 setup.py sdist")
+    os.system("python setup.py sdist")
     os.system("twine upload dist/* --skip-existing")
     sys.exit()
 
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
+
+with open(os.path.join(here, "requirements.txt"), encoding="utf-8") as f:
+    install_requires = f.read().split("\n")
+
 setup(
     name="jamstack",
-    version=__version__,
+    version=f'{__version__}',
     description="Jamstack in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jamstackpy/jamstack",
     author="Abdur-Rahmaan Janhangeer",
     author_email="arj.python@gmail.com",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
-    keywords="jamstack static",
+    keywords="jamstack static website jinja2",
     packages=["jamstack"],
     include_package_data=True,
     python_requires=">=3.6",
-    install_requires=open(
-        os.path.join(here, "requirements.txt"), encoding="utf-8"
-    )
-    .read()
-    .split("\n"),
+    install_requires=install_requires,
     project_urls={
         "Bug Reports": "https://github.com/jamstackpy/jamstack/issues",
         "Source": "https://github.com/jamstackpy/jamstack",
     },
     entry_points={"console_scripts": ["jamstack=jamstack.__main__:main"]},
 )
```

