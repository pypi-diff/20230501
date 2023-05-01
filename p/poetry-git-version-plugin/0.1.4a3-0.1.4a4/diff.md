# Comparing `tmp/poetry_git_version_plugin-0.1.4a3.tar.gz` & `tmp/poetry_git_version_plugin-0.1.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.4a3.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.4a4.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.4a3.tar` & `poetry_git_version_plugin-0.1.4a4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 11:35:48.258809 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1651 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1550 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5240 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2837 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a3/pyproject.toml
--rw-r--r--   0        0        0     3449 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a3/readme.md
--rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4a3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a4/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 12:11:15.365267 poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1651 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1550 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5240 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2837 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a4/pyproject.toml
+-rw-r--r--   0        0        0     3449 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a4/readme.md
+-rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4a4/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.4a3/LICENSE` & `poetry_git_version_plugin-0.1.4a4/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.4a4/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/pyproject.toml` & `poetry_git_version_plugin-0.1.4a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/readme.md` & `poetry_git_version_plugin-0.1.4a4/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a3/PKG-INFO` & `poetry_git_version_plugin-0.1.4a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.4a3
+Version: 0.1.4a4
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

