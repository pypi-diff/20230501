# Comparing `tmp/poetry_git_version_plugin-0.1.4.dev2.tar.gz` & `tmp/poetry_git_version_plugin-0.1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.4.dev2.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.4a2.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.4.dev2.tar` & `poetry_git_version_plugin-0.1.4a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-04-30 17:38:22.056726 poetry_git_version_plugin-0.1.4.dev2/LICENSE
--rw-r--r--   0        0        0        0 2022-11-21 18:20:04.946186 poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-02-21 22:12:51.921276 poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1654 2023-05-01 10:59:06.888753 poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-04-16 16:54:29.215931 poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1550 2023-04-30 17:58:59.037679 poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5240 2023-04-30 17:58:46.904395 poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2837 2023-04-30 17:39:22.838153 poetry_git_version_plugin-0.1.4.dev2/pyproject.toml
--rw-r--r--   0        0        0     1639 2023-04-30 18:09:34.627191 poetry_git_version_plugin-0.1.4.dev2/readme.md
--rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4.dev2/PKG-INFO
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

### Comparing `poetry_git_version_plugin-0.1.4.dev2/LICENSE` & `poetry_git_version_plugin-0.1.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     _default_setting = {
         # Игнорирование отсутствия тега
         'ignore_errors': True,
         # При отсутствии тега генерировать alpha version
         'make_alpha_version': True,
         # Alpha Version Format
-        'alpha_version_format': '{version}.dev{distance}',
+        'alpha_version_format': '{version}a{distance}',
         # 'alpha_version_format': '{version}a{distance}+{commit_hash}',
         # Ignore PEP440
         'ignore_pep440': True,
         # Ignore public format PEP440
         'ignore_public_pep440': True,
     }
```

### Comparing `poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4.dev2/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4.dev2/pyproject.toml` & `poetry_git_version_plugin-0.1.4a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4.dev2/readme.md` & `poetry_git_version_plugin-0.1.4a2/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4.dev2/PKG-INFO` & `poetry_git_version_plugin-0.1.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.4.dev2
+Version: 0.1.4a2
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

