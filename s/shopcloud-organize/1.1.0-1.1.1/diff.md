# Comparing `tmp/shopcloud_organize-1.1.0.tar.gz` & `tmp/shopcloud_organize-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud_organize-1.1.0.tar", last modified: Mon May  1 06:40:05 2023, max compression
+gzip compressed data, was "shopcloud_organize-1.1.1.tar", last modified: Mon May  1 06:42:52 2023, max compression
```

## Comparing `shopcloud_organize-1.1.0.tar` & `shopcloud_organize-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:40:05.907167 shopcloud_organize-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 06:40:05.907167 shopcloud_organize-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:40:05.907167 shopcloud_organize-1.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/scripts/organize
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:40:05.907167 shopcloud_organize-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:40:05.907167 shopcloud_organize-1.1.0/shopcloud_organize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/shopcloud_organize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/shopcloud_organize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/shopcloud_organize/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/shopcloud_organize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 06:39:46.000000 shopcloud_organize-1.1.0/shopcloud_organize/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:40:05.907167 shopcloud_organize-1.1.0/shopcloud_organize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 06:40:05.000000 shopcloud_organize-1.1.0/shopcloud_organize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 06:40:05.000000 shopcloud_organize-1.1.0/shopcloud_organize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:40:05.000000 shopcloud_organize-1.1.0/shopcloud_organize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 06:40:05.000000 shopcloud_organize-1.1.0/shopcloud_organize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:40:05.000000 shopcloud_organize-1.1.0/shopcloud_organize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:42:52.903556 shopcloud_organize-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 06:42:52.903556 shopcloud_organize-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:42:52.903556 shopcloud_organize-1.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/scripts/organize
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:42:52.903556 shopcloud_organize-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:42:52.903556 shopcloud_organize-1.1.1/shopcloud_organize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/shopcloud_organize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/shopcloud_organize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/shopcloud_organize/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/shopcloud_organize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 06:42:26.000000 shopcloud_organize-1.1.1/shopcloud_organize/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:42:52.903556 shopcloud_organize-1.1.1/shopcloud_organize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 06:42:52.000000 shopcloud_organize-1.1.1/shopcloud_organize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 06:42:52.000000 shopcloud_organize-1.1.1/shopcloud_organize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:42:52.000000 shopcloud_organize-1.1.1/shopcloud_organize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 06:42:52.000000 shopcloud_organize-1.1.1/shopcloud_organize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:42:52.000000 shopcloud_organize-1.1.1/shopcloud_organize.egg-info/top_level.txt
```

### Comparing `shopcloud_organize-1.1.0/LICENSE` & `shopcloud_organize-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shopcloud_organize-1.1.0/PKG-INFO` & `shopcloud_organize-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud_organize
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLI tool for task management @talk-point
 Home-page: https://github.com/Talk-Point/shopcloud-organize
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud_organize-1.1.0/setup.py` & `shopcloud_organize-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = {
     "name": 'shopcloud_organize',
-    "version": '1.1.0',
+    "version": '1.1.1',
     "description": 'CLI tool for task management @talk-point',
     "long_description_content_type": "text/markdown",
     "long_description": README,
     "license": 'MIT',
     "packages": find_packages(),
     "author": 'Konstantin Stoldt',
     "author_email": 'konstantin.stoldt@talk-point.de',
```

### Comparing `shopcloud_organize-1.1.0/shopcloud_organize/__main__.py` & `shopcloud_organize-1.1.1/shopcloud_organize/__main__.py`

 * *Files identical despite different names*

### Comparing `shopcloud_organize-1.1.0/shopcloud_organize/cli.py` & `shopcloud_organize-1.1.1/shopcloud_organize/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                 json=data
             )
             if not (200 <= response.status_code < 300):
                 raise exceptions.IssueCreateException(response.text)
             
             items = [x for x in response.json() if x.get('title') == data.get('title')]
             if len(items) > 0:
-                return items.get('html_url')
+                return items[0].get('html_url')
 
         if kwargs.get('simulate', False):
             return f'https://github.com/{owner}/{repo}/issues/<id>`'
 
         response = requests.post(
             f'https://api.github.com/repos/{owner}/{repo}/issues',
             auth=(
```

### Comparing `shopcloud_organize-1.1.0/shopcloud_organize/helpers.py` & `shopcloud_organize-1.1.1/shopcloud_organize/helpers.py`

 * *Files identical despite different names*

### Comparing `shopcloud_organize-1.1.0/shopcloud_organize.egg-info/PKG-INFO` & `shopcloud_organize-1.1.1/shopcloud_organize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-organize
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLI tool for task management @talk-point
 Home-page: https://github.com/Talk-Point/shopcloud-organize
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

