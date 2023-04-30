# Comparing `tmp/suap_scraper-0.0.2.tar.gz` & `tmp/suap_scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suap_scraper-0.0.2.tar", last modified: Sun Apr 30 19:39:22 2023, max compression
+gzip compressed data, was "suap_scraper-0.0.3.tar", last modified: Sun Apr 30 22:50:42 2023, max compression
```

## Comparing `suap_scraper-0.0.2.tar` & `suap_scraper-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 19:39:22.071488 suap_scraper-0.0.2/
--rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.2/LICENSE.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-04-30 19:39:22.067488 suap_scraper-0.0.2/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.2/README.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      586 2023-04-30 19:34:33.000000 suap_scraper-0.0.2/pyproject.toml
--rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-04-30 19:39:22.071488 suap_scraper-0.0.2/setup.cfg
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 19:39:22.051488 suap_scraper-0.0.2/suap_scraper/
--rw-rw-r--   0 dom       (1000) dom       (1000)     3872 2023-04-30 18:34:44.000000 suap_scraper-0.0.2/suap_scraper/SUAP.py
--rw-rw-r--   0 dom       (1000) dom       (1000)        0 2023-04-30 18:35:47.000000 suap_scraper-0.0.2/suap_scraper/__init__.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-04-30 18:34:44.000000 suap_scraper-0.0.2/suap_scraper/config.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     2276 2023-04-30 18:34:44.000000 suap_scraper-0.0.2/suap_scraper/utils.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 19:39:22.067488 suap_scraper-0.0.2/suap_scraper.egg-info/
--rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-04-30 19:39:21.000000 suap_scraper-0.0.2/suap_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)      270 2023-04-30 19:39:21.000000 suap_scraper-0.0.2/suap_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-04-30 19:39:21.000000 suap_scraper-0.0.2/suap_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-04-30 19:39:21.000000 suap_scraper-0.0.2/suap_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 22:50:42.104246 suap_scraper-0.0.3/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.3/LICENSE.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-04-30 22:50:42.104246 suap_scraper-0.0.3/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.3/README.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      631 2023-04-30 22:49:43.000000 suap_scraper-0.0.3/pyproject.toml
+-rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-04-30 22:50:42.104246 suap_scraper-0.0.3/setup.cfg
+-rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.3/setup.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 22:50:42.100246 suap_scraper-0.0.3/suap_scraper/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     3872 2023-04-30 18:34:44.000000 suap_scraper-0.0.3/suap_scraper/SUAP.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)        0 2023-04-30 18:35:47.000000 suap_scraper-0.0.3/suap_scraper/__init__.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-04-30 18:34:44.000000 suap_scraper-0.0.3/suap_scraper/config.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     2276 2023-04-30 18:34:44.000000 suap_scraper-0.0.3/suap_scraper/utils.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-04-30 22:50:42.104246 suap_scraper-0.0.3/suap_scraper.egg-info/
+-rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-04-30 22:50:42.000000 suap_scraper-0.0.3/suap_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)      279 2023-04-30 22:50:42.000000 suap_scraper-0.0.3/suap_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-04-30 22:50:42.000000 suap_scraper-0.0.3/suap_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-04-30 22:50:42.000000 suap_scraper-0.0.3/suap_scraper.egg-info/top_level.txt
```

### Comparing `suap_scraper-0.0.2/LICENSE.md` & `suap_scraper-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.2/PKG-INFO` & `suap_scraper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap_scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `suap_scraper-0.0.2/pyproject.toml` & `suap_scraper-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "requests>=2.26.0", "beautifulsoup4==4.9.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "suap_scraper"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jao42", email="cavalcante.joao@protonmail.ch" },
 ]
 description = "Um scraper para o SUAP do IFPB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `suap_scraper-0.0.2/suap_scraper/SUAP.py` & `suap_scraper-0.0.3/suap_scraper/SUAP.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.2/suap_scraper/config.py` & `suap_scraper-0.0.3/suap_scraper/config.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.2/suap_scraper/utils.py` & `suap_scraper-0.0.3/suap_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.2/suap_scraper.egg-info/PKG-INFO` & `suap_scraper-0.0.3/suap_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

