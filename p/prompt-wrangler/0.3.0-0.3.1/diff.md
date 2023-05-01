# Comparing `tmp/prompt_wrangler-0.3.0.tar.gz` & `tmp/prompt_wrangler-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_wrangler-0.3.0.tar", last modified: Mon May  1 21:40:30 2023, max compression
+gzip compressed data, was "prompt_wrangler-0.3.1.tar", last modified: Mon May  1 21:44:35 2023, max compression
```

## Comparing `prompt_wrangler-0.3.0.tar` & `prompt_wrangler-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:40:30.641003 prompt_wrangler-0.3.0/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1882 2023-05-01 21:40:30.640837 prompt_wrangler-0.3.0/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)     1210 2023-05-01 14:39:54.000000 prompt_wrangler-0.3.0/README.md
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:40:30.638690 prompt_wrangler-0.3.0/__pycache__/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1883 2023-05-01 20:47:14.000000 prompt_wrangler-0.3.0/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:40:30.639113 prompt_wrangler-0.3.0/prompt_wrangler/
--rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 14:12:42.000000 prompt_wrangler-0.3.0/prompt_wrangler/__init__.py
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:40:30.640584 prompt_wrangler-0.3.0/prompt_wrangler/__pycache__/
--rw-r--r--   0 maxshaw    (501) staff       (20)      286 2023-05-01 14:12:45.000000 prompt_wrangler-0.3.0/prompt_wrangler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     4111 2023-05-01 21:03:40.000000 prompt_wrangler-0.3.0/prompt_wrangler/__pycache__/client.cpython-310.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     3786 2023-05-01 21:03:28.000000 prompt_wrangler-0.3.0/prompt_wrangler/client.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      552 2023-05-01 20:51:29.000000 prompt_wrangler-0.3.0/prompt_wrangler/client.pyi
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:40:30.640219 prompt_wrangler-0.3.0/prompt_wrangler.egg-info/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1882 2023-05-01 21:40:30.000000 prompt_wrangler-0.3.0/prompt_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)      510 2023-05-01 21:40:30.000000 prompt_wrangler-0.3.0/prompt_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 21:40:30.000000 prompt_wrangler-0.3.0/prompt_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 21:40:30.000000 prompt_wrangler-0.3.0/prompt_wrangler.egg-info/requires.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 21:40:30.000000 prompt_wrangler-0.3.0/prompt_wrangler.egg-info/top_level.txt
--rwxr-xr-x   0 maxshaw    (501) staff       (20)      866 2023-05-01 14:35:01.000000 prompt_wrangler-0.3.0/publish.sh
--rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-01 20:47:41.000000 prompt_wrangler-0.3.0/run_prompt.py
--rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 21:40:30.641109 prompt_wrangler-0.3.0/setup.cfg
--rw-r--r--   0 maxshaw    (501) staff       (20)     1062 2023-05-01 21:40:29.000000 prompt_wrangler-0.3.0/setup.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      910 2023-05-01 21:04:37.000000 prompt_wrangler-0.3.0/test_mock.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      408 2023-05-01 21:40:20.000000 prompt_wrangler-0.3.0/test_real.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:44:35.550574 prompt_wrangler-0.3.1/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1968 2023-05-01 21:44:35.550415 prompt_wrangler-0.3.1/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1296 2023-05-01 21:43:34.000000 prompt_wrangler-0.3.1/README.md
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:44:35.548519 prompt_wrangler-0.3.1/__pycache__/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1883 2023-05-01 20:47:14.000000 prompt_wrangler-0.3.1/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:44:35.548949 prompt_wrangler-0.3.1/prompt_wrangler/
+-rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 14:12:42.000000 prompt_wrangler-0.3.1/prompt_wrangler/__init__.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:44:35.550046 prompt_wrangler-0.3.1/prompt_wrangler/__pycache__/
+-rw-r--r--   0 maxshaw    (501) staff       (20)      286 2023-05-01 14:12:45.000000 prompt_wrangler-0.3.1/prompt_wrangler/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 maxshaw    (501) staff       (20)     4111 2023-05-01 21:03:40.000000 prompt_wrangler-0.3.1/prompt_wrangler/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0 maxshaw    (501) staff       (20)     3786 2023-05-01 21:03:28.000000 prompt_wrangler-0.3.1/prompt_wrangler/client.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      552 2023-05-01 20:51:29.000000 prompt_wrangler-0.3.1/prompt_wrangler/client.pyi
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 21:44:35.549720 prompt_wrangler-0.3.1/prompt_wrangler.egg-info/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1968 2023-05-01 21:44:35.000000 prompt_wrangler-0.3.1/prompt_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)      510 2023-05-01 21:44:35.000000 prompt_wrangler-0.3.1/prompt_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 21:44:35.000000 prompt_wrangler-0.3.1/prompt_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 21:44:35.000000 prompt_wrangler-0.3.1/prompt_wrangler.egg-info/requires.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 21:44:35.000000 prompt_wrangler-0.3.1/prompt_wrangler.egg-info/top_level.txt
+-rwxr-xr-x   0 maxshaw    (501) staff       (20)      866 2023-05-01 14:35:01.000000 prompt_wrangler-0.3.1/publish.sh
+-rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-01 20:47:41.000000 prompt_wrangler-0.3.1/run_prompt.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 21:44:35.550639 prompt_wrangler-0.3.1/setup.cfg
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1062 2023-05-01 21:44:35.000000 prompt_wrangler-0.3.1/setup.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      910 2023-05-01 21:04:37.000000 prompt_wrangler-0.3.1/test_mock.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      408 2023-05-01 21:40:20.000000 prompt_wrangler-0.3.1/test_real.py
```

### Comparing `prompt_wrangler-0.3.0/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc` & `prompt_wrangler-0.3.1/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.0/prompt_wrangler/__pycache__/client.cpython-310.pyc` & `prompt_wrangler-0.3.1/prompt_wrangler/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.0/prompt_wrangler/client.py` & `prompt_wrangler-0.3.1/prompt_wrangler/client.py`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.0/prompt_wrangler/client.pyi` & `prompt_wrangler-0.3.1/prompt_wrangler/client.pyi`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.0/publish.sh` & `prompt_wrangler-0.3.1/publish.sh`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.0/setup.py` & `prompt_wrangler-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="prompt_wrangler",
-    version="0.3.0",
+    version="0.3.1",
     author="Max Shaw",
     author_email="max@exit38.org",
     description="A Python wrapper for the Prompt Wrangler REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/exit38/prompt_wrangler",
     packages=find_packages(),
```

### Comparing `prompt_wrangler-0.3.0/test_mock.py` & `prompt_wrangler-0.3.1/test_mock.py`

 * *Files identical despite different names*

