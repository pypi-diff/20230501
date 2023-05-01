# Comparing `tmp/poetry_git_version_plugin-0.1.4.tar.gz` & `tmp/poetry_git_version_plugin-0.1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.4.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.4a2.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.4.tar` & `poetry_git_version_plugin-0.1.4a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2023-04-30 18:01:25.074022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-04-16 20:16:12.153636 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1651 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-04-16 20:16:12.153636 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1550 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5240 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2837 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1639 2023-04-30 18:01:24.998022 poetry_git_version_plugin-0.1.4/readme.md
--rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 10:00:45.410317 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1651 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1550 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5240 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2837 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/pyproject.toml
+-rw-r--r--   0        0        0     1639 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/readme.md
+-rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4a2/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.4/LICENSE` & `poetry_git_version_plugin-0.1.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4/pyproject.toml` & `poetry_git_version_plugin-0.1.4a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4/readme.md` & `poetry_git_version_plugin-0.1.4a2/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ## Dependencies
 
 Installed `Git` and:
 
 ```toml
 [tool.poetry.dependencies]
 python = ">=3.8"
-poetry = ">=1.2.0"
+poetry = ">=1.2.2"
 ```
 
 ## Setup
 
 ```toml
 [tool.poetry-git-version-plugin]
 # If the tag is not found on the HEAD,
```

### Comparing `poetry_git_version_plugin-0.1.4/PKG-INFO` & `poetry_git_version_plugin-0.1.4a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.4
+Version: 0.1.4a2
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -56,15 +56,15 @@
 ## Dependencies
 
 Installed `Git` and:
 
 ```toml
 [tool.poetry.dependencies]
 python = ">=3.8"
-poetry = ">=1.2.0"
+poetry = ">=1.2.2"
 ```
 
 ## Setup
 
 ```toml
 [tool.poetry-git-version-plugin]
 # If the tag is not found on the HEAD,
```

