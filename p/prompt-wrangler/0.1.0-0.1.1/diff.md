# Comparing `tmp/prompt_wrangler-0.1.0.tar.gz` & `tmp/prompt_wrangler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_wrangler-0.1.0.tar", last modified: Mon May  1 14:19:19 2023, max compression
+gzip compressed data, was "prompt_wrangler-0.1.1.tar", last modified: Mon May  1 14:25:51 2023, max compression
```

## Comparing `prompt_wrangler-0.1.0.tar` & `prompt_wrangler-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:19:19.480783 prompt_wrangler-0.1.0/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1924 2023-05-01 14:19:19.480643 prompt_wrangler-0.1.0/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)     1218 2023-05-01 14:17:19.000000 prompt_wrangler-0.1.0/README.md
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:19:19.479812 prompt_wrangler-0.1.0/prompt_wrangler/
--rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 14:12:42.000000 prompt_wrangler-0.1.0/prompt_wrangler/__init__.py
--rw-r--r--   0 maxshaw    (501) staff       (20)     2366 2023-05-01 14:15:16.000000 prompt_wrangler-0.1.0/prompt_wrangler/client.py
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:19:19.480441 prompt_wrangler-0.1.0/prompt_wrangler.egg-info/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1924 2023-05-01 14:19:19.000000 prompt_wrangler-0.1.0/prompt_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)      266 2023-05-01 14:19:19.000000 prompt_wrangler-0.1.0/prompt_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 14:19:19.000000 prompt_wrangler-0.1.0/prompt_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 14:19:19.000000 prompt_wrangler-0.1.0/prompt_wrangler.egg-info/requires.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 14:19:19.000000 prompt_wrangler-0.1.0/prompt_wrangler.egg-info/top_level.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 14:19:19.480841 prompt_wrangler-0.1.0/setup.cfg
--rw-r--r--   0 maxshaw    (501) staff       (20)      959 2023-05-01 14:18:57.000000 prompt_wrangler-0.1.0/setup.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:25:51.728212 prompt_wrangler-0.1.1/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1924 2023-05-01 14:25:51.728066 prompt_wrangler-0.1.1/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1218 2023-05-01 14:17:19.000000 prompt_wrangler-0.1.1/README.md
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:25:51.727151 prompt_wrangler-0.1.1/prompt_wrangler/
+-rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 14:12:42.000000 prompt_wrangler-0.1.1/prompt_wrangler/__init__.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)     2366 2023-05-01 14:15:16.000000 prompt_wrangler-0.1.1/prompt_wrangler/client.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 14:25:51.727876 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1924 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)      266 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/requires.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/prompt_wrangler.egg-info/top_level.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 14:25:51.728272 prompt_wrangler-0.1.1/setup.cfg
+-rw-r--r--   0 maxshaw    (501) staff       (20)      959 2023-05-01 14:25:51.000000 prompt_wrangler-0.1.1/setup.py
```

### Comparing `prompt_wrangler-0.1.0/PKG-INFO` & `prompt_wrangler-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt_wrangler
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: https://github.com/exit38/prompt_wrangler
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prompt_wrangler-0.1.0/README.md` & `prompt_wrangler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.1.0/prompt_wrangler/client.py` & `prompt_wrangler-0.1.1/prompt_wrangler/client.py`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.1.0/prompt_wrangler.egg-info/PKG-INFO` & `prompt_wrangler-0.1.1/prompt_wrangler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-wrangler
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: https://github.com/exit38/prompt_wrangler
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prompt_wrangler-0.1.0/setup.py` & `prompt_wrangler-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="prompt_wrangler",
-    version="0.1.0",
+    version="0.1.1",
     author="Max Shaw",
     author_email="max@exit38.org",
     description="A Python wrapper for the Prompt Wrangler REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/exit38/prompt_wrangler",
     packages=find_packages(),
```

