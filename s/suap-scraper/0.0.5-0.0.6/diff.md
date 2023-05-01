# Comparing `tmp/suap_scraper-0.0.5.tar.gz` & `tmp/suap_scraper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suap_scraper-0.0.5.tar", last modified: Sun Apr 30 23:50:26 2023, max compression
+gzip compressed data, was "suap_scraper-0.0.6.tar", last modified: Mon May  1 00:12:05 2023, max compression
```

## Comparing `suap_scraper-0.0.5.tar` & `suap_scraper-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 23:50:26.114509 suap_scraper-0.0.5/
--rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.5/LICENSE.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-04-30 23:50:26.114509 suap_scraper-0.0.5/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.5/README.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      643 2023-04-30 23:49:32.000000 suap_scraper-0.0.5/pyproject.toml
--rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-04-30 23:50:26.114509 suap_scraper-0.0.5/setup.cfg
--rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.5/setup.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 23:50:26.106509 suap_scraper-0.0.5/suap_scraper/
--rw-rw-r--   0 dom       (1000) dom       (1000)     3898 2023-04-30 23:47:13.000000 suap_scraper-0.0.5/suap_scraper/SUAP.py
--rw-rw-r--   0 dom       (1000) dom       (1000)        0 2023-04-30 18:35:47.000000 suap_scraper-0.0.5/suap_scraper/__init__.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-04-30 18:34:44.000000 suap_scraper-0.0.5/suap_scraper/config.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     2289 2023-04-30 23:48:10.000000 suap_scraper-0.0.5/suap_scraper/utils.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 23:50:26.114509 suap_scraper-0.0.5/suap_scraper.egg-info/
--rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-04-30 23:50:26.000000 suap_scraper-0.0.5/suap_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)      314 2023-04-30 23:50:26.000000 suap_scraper-0.0.5/suap_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-04-30 23:50:26.000000 suap_scraper-0.0.5/suap_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       24 2023-04-30 23:50:26.000000 suap_scraper-0.0.5/suap_scraper.egg-info/requires.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-04-30 23:50:26.000000 suap_scraper-0.0.5/suap_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-01 00:12:05.838954 suap_scraper-0.0.6/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6/LICENSE.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-05-01 00:12:05.834954 suap_scraper-0.0.6/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6/README.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      643 2023-05-01 00:10:46.000000 suap_scraper-0.0.6/pyproject.toml
+-rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-01 00:12:05.838954 suap_scraper-0.0.6/setup.cfg
+-rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6/setup.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-01 00:12:05.822954 suap_scraper-0.0.6/suap_scraper/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     3898 2023-04-30 23:47:13.000000 suap_scraper-0.0.6/suap_scraper/SUAP.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6/suap_scraper/__init__.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-04-30 18:34:44.000000 suap_scraper-0.0.6/suap_scraper/config.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     2289 2023-04-30 23:48:10.000000 suap_scraper-0.0.6/suap_scraper/utils.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-01 00:12:05.834954 suap_scraper-0.0.6/suap_scraper.egg-info/
+-rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)      314 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       24 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/requires.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/top_level.txt
```

### Comparing `suap_scraper-0.0.5/LICENSE.md` & `suap_scraper-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.5/PKG-INFO` & `suap_scraper-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap_scraper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `suap_scraper-0.0.5/suap_scraper/SUAP.py` & `suap_scraper-0.0.6/suap_scraper/SUAP.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.5/suap_scraper/config.py` & `suap_scraper-0.0.6/suap_scraper/config.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.5/suap_scraper/utils.py` & `suap_scraper-0.0.6/suap_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.5/suap_scraper.egg-info/PKG-INFO` & `suap_scraper-0.0.6/suap_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap-scraper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

