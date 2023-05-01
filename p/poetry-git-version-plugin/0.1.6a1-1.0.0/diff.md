# Comparing `tmp/poetry_git_version_plugin-0.1.6a1.tar.gz` & `tmp/poetry_git_version_plugin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.6a1.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-1.0.0.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.6a1.tar` & `poetry_git_version_plugin-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.6a1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 19:05:14.286729 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      837 2023-05-01 19:02:48.091434 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1114 2023-05-01 19:02:48.091434 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5882 2023-05-01 19:02:48.095434 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2776 2023-05-01 19:04:49.982846 poetry_git_version_plugin-0.1.6a1/pyproject.toml
--rw-r--r--   0        0        0     4406 2023-05-01 19:02:48.095434 poetry_git_version_plugin-0.1.6a1/readme.md
--rw-r--r--   0        0        0     5960 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.6a1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-1.0.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 19:09:05.377623 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      837 2023-05-01 19:02:48.091434 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1114 2023-05-01 19:02:48.091434 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5882 2023-05-01 19:02:48.095434 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2776 2023-05-01 19:08:44.061725 poetry_git_version_plugin-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4406 2023-05-01 19:02:48.095434 poetry_git_version_plugin-1.0.0/readme.md
+-rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.0/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.6a1/LICENSE` & `poetry_git_version_plugin-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/pyproject.toml` & `poetry_git_version_plugin-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/readme.md` & `poetry_git_version_plugin-1.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6a1/PKG-INFO` & `poetry_git_version_plugin-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.6a1
+Version: 1.0.0
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

