# Comparing `tmp/auto-iap-enviroment-0.1.tar.gz` & `tmp/auto-iap-enviroment-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-iap-enviroment-0.1.tar", last modified: Sun Apr 30 22:03:01 2023, max compression
+gzip compressed data, was "auto-iap-enviroment-0.1.1.tar", last modified: Sun Apr 30 22:06:13 2023, max compression
```

## Comparing `auto-iap-enviroment-0.1.tar` & `auto-iap-enviroment-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:03:01.505766 auto-iap-enviroment-0.1/
--rw-rw-r--   0 luis      (1000) luis      (1000)      520 2023-04-30 22:03:01.505766 auto-iap-enviroment-0.1/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)        5 2023-04-29 20:37:50.000000 auto-iap-enviroment-0.1/README.md
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:03:01.505766 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/
--rw-rw-r--   0 luis      (1000) luis      (1000)      520 2023-04-30 22:03:01.000000 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      359 2023-04-30 22:03:01.000000 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-04-30 22:03:01.000000 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)       71 2023-04-30 22:03:01.000000 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/entry_points.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        7 2023-04-30 22:03:01.000000 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        4 2023-04-30 22:03:01.000000 auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/top_level.txt
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:03:01.505766 auto-iap-enviroment-0.1/iap/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1056 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1/iap/helpers.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      471 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1/iap/iaApi.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      508 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1/iap/main.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     1168 2023-04-30 22:01:54.000000 auto-iap-enviroment-0.1/iap/scrapeMe.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      249 2023-04-30 22:01:54.000000 auto-iap-enviroment-0.1/pyproject.toml
--rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-04-30 22:03:01.505766 auto-iap-enviroment-0.1/setup.cfg
--rw-rw-r--   0 luis      (1000) luis      (1000)      878 2023-04-30 22:02:57.000000 auto-iap-enviroment-0.1/setup.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      522 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)        5 2023-04-29 20:37:50.000000 auto-iap-enviroment-0.1.1/README.md
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      522 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)      344 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)       71 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/entry_points.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        7 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        4 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/top_level.txt
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/iap/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1056 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.1/iap/helpers.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      471 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.1/iap/iaApi.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      508 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.1/iap/main.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1168 2023-04-30 22:01:54.000000 auto-iap-enviroment-0.1.1/iap/scrapeMe.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/setup.cfg
+-rw-rw-r--   0 luis      (1000) luis      (1000)      880 2023-04-30 22:05:20.000000 auto-iap-enviroment-0.1.1/setup.py
```

### Comparing `auto-iap-enviroment-0.1/PKG-INFO` & `auto-iap-enviroment-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-iap-enviroment
-Version: 0.1
+Version: 0.1.1
 Summary: Um pacote que integra o OpenAI GPT ao seu computados
 Home-page: https://github.com/seu-usuario/meu-pacote
 Author: Luis Arthur Rodrigues da Silva
 Author-email: luisarthurlards03@gmail.com
 License: UNKNOWN
 Description: # IAp
 Platform: UNKNOWN
```

### Comparing `auto-iap-enviroment-0.1/auto_iap_enviroment.egg-info/PKG-INFO` & `auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-iap-enviroment
-Version: 0.1
+Version: 0.1.1
 Summary: Um pacote que integra o OpenAI GPT ao seu computados
 Home-page: https://github.com/seu-usuario/meu-pacote
 Author: Luis Arthur Rodrigues da Silva
 Author-email: luisarthurlards03@gmail.com
 License: UNKNOWN
 Description: # IAp
 Platform: UNKNOWN
```

### Comparing `auto-iap-enviroment-0.1/iap/helpers.py` & `auto-iap-enviroment-0.1.1/iap/helpers.py`

 * *Files identical despite different names*

### Comparing `auto-iap-enviroment-0.1/iap/scrapeMe.py` & `auto-iap-enviroment-0.1.1/iap/scrapeMe.py`

 * *Files identical despite different names*

### Comparing `auto-iap-enviroment-0.1/setup.py` & `auto-iap-enviroment-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="auto-iap-enviroment",
-    version="0.1",
+    version="0.1.1",
     author="Luis Arthur Rodrigues da Silva",
     author_email="luisarthurlards03@gmail.com",
     description="Um pacote que integra o OpenAI GPT ao seu computados",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seu-usuario/meu-pacote",
     packages=['iap'],
```

