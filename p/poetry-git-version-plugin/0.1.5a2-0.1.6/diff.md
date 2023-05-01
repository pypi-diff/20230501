# Comparing `tmp/poetry_git_version_plugin-0.1.5a2.tar.gz` & `tmp/poetry_git_version_plugin-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.5a2.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.6.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.5a2.tar` & `poetry_git_version_plugin-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.5a2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 18:06:22.960948 poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1187 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5662 2023-05-01 18:03:38.089366 poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2832 2023-05-01 18:06:01.589006 poetry_git_version_plugin-0.1.5a2/pyproject.toml
--rw-r--r--   0        0        0     4402 2023-05-01 17:03:01.127393 poetry_git_version_plugin-0.1.5a2/readme.md
--rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.5a2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 18:09:40.772367 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1187 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5662 2023-05-01 18:03:38.089366 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2832 2023-05-01 18:09:19.632432 poetry_git_version_plugin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4402 2023-05-01 17:03:01.127393 poetry_git_version_plugin-0.1.6/readme.md
+-rw-r--r--   0        0        0     5954 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.6/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.5a2/LICENSE` & `poetry_git_version_plugin-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/pyproject.toml` & `poetry_git_version_plugin-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/readme.md` & `poetry_git_version_plugin-0.1.6/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.5a2/PKG-INFO` & `poetry_git_version_plugin-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.5a2
+Version: 0.1.6
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

