# Comparing `tmp/poetry_git_version_plugin-0.1.4a5.tar.gz` & `tmp/poetry_git_version_plugin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.4a5.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.5.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.4a5.tar` & `poetry_git_version_plugin-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a5/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 16:33:38.966691 poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1651 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1550 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5240 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2837 2023-05-01 16:33:18.206800 poetry_git_version_plugin-0.1.4a5/pyproject.toml
--rw-r--r--   0        0        0     4450 2023-05-01 16:31:09.691481 poetry_git_version_plugin-0.1.4a5/readme.md
--rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4a5/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 17:05:34.118757 poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1653 2023-05-01 17:03:01.127393 poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1550 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5245 2023-05-01 17:03:01.127393 poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2837 2023-05-01 17:05:12.762847 poetry_git_version_plugin-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4402 2023-05-01 17:03:01.127393 poetry_git_version_plugin-0.1.5/readme.md
+-rw-r--r--   0        0        0     5998 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.5/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.4a5/LICENSE` & `poetry_git_version_plugin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         # Игнорирование отсутствия тега
         'ignore_errors': True,
         # При отсутствии тега генерировать alpha version
         'make_alpha_version': True,
         # Alpha Version Format
         'alpha_version_format': '{version}a{distance}',
         # 'alpha_version_format': '{version}a{distance}+{commit_hash}',
-        # Ignore PEP440
+        # Ignore PEP 440
         'ignore_pep440': True,
-        # Ignore public format PEP440
+        # Ignore public format PEP 440
         'ignore_public_pep440': True,
     }
 
     def __init__(self, pyproject: PyProjectTOML) -> None:
         self.pyproject = pyproject
 
     @property
```

### Comparing `poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a5/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.5/poetry_git_version_plugin/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 VERSION_REGEX_COMPILE = re.compile(r'^\s*' + VERSION_PATTERN + r'\s*$', re.VERBOSE | re.IGNORECASE)
 VERSION_CANON_REGEX_COMPILE = re.compile(
     r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)(0|[1-9][0-9]*))?(\.post(0|[1-9][0-9]*))?(\.dev(0|[1-9][0-9]*))?$'
 )
 
 
 def validate_version(version_string: str):
-    """Проверка версии на PEP440
+    """Проверка версии на PEP 440
 
     Args:
         version_string (str): Версия
 
     Raises:
         PluginException: Версия не соответствует стандарту
 
@@ -149,24 +149,24 @@
     def validate_version(self, version: str):
         is_valid = validate_version(version)
 
         if is_valid == 0:
             return version
 
         if is_valid == 1:
-            self.io.write_line(f'Invalid PEP440 version: "{version}"', Verbosity.VERBOSE)
+            self.io.write_line(f'Invalid PEP 440 version: "{version}"', Verbosity.VERBOSE)
 
             if not self.plugin_config.ignore_pep440:
-                raise PluginException(f'Invalid PEP440 version: "{version}"')
+                raise PluginException(f'Invalid PEP 440 version: "{version}"')
 
         if is_valid == 2:
-            self.io.write_line(f'Invalid public PEP440 version: "{version}"', Verbosity.VERBOSE)
+            self.io.write_line(f'Invalid public PEP 440 version: "{version}"', Verbosity.VERBOSE)
 
             if not self.plugin_config.ignore_public_pep440:
-                raise PluginException(f'Invalid public PEP440 version: "{version}"')
+                raise PluginException(f'Invalid public PEP 440 version: "{version}"')
 
     def get_version(self) -> str:
         version = self.__get_version()
 
         self.validate_version(version)
 
         return version
```

### Comparing `poetry_git_version_plugin-0.1.4a5/pyproject.toml` & `poetry_git_version_plugin-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a5/readme.md` & `poetry_git_version_plugin-0.1.5/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Poetry Git Version Plugin
 
-Poetry plugin to get package version from git.
+Poetry plugin to set package version based on git tag.
 
 [![PyPI](https://img.shields.io/pypi/v/poetry-git-version-plugin)](https://pypi.org/project/poetry-git-version-plugin/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-git-version-plugin)
-[![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/poetry-git-version-plugin)](https://gitlab.com/rocshers/python/poetry-git-version-plugin)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-git-version-plugin)](https://pypi.org/project/poetry-git-version-plugin/)
+[![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/poetry-git-version-plugin)](https://gitlab.com/rocshers/python/poetry-git-version-plugin)
 
 [![Test coverage](https://codecov.io/gitlab/rocshers:python/poetry-git-version-plugin/branch/release/graph/badge.svg?token=RPFNZ8SBQ6)](https://codecov.io/gitlab/rocshers:python/poetry-git-version-plugin)
 [![Downloads](https://static.pepy.tech/badge/poetry-git-version-plugin)](https://pepy.tech/project/poetry-git-version-plugin)
-![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/poetry-git-version-plugin)
-[![pipeline status](https://gitlab.com/rocshers/python/poetry-git-version-plugin/badges/release/pipeline.svg)](https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/commits/release)
+[![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/poetry-git-version-plugin)](https://gitlab.com/rocshers/python/poetry-git-version-plugin)
 
 ## Functionality
 
-- Git tag parsing
-- Make alpha version
-- Substitution of the project tag (if any) in the poetry.version value
-- Maintenance of PEP 440
-- Command to output a new version
+- **Git tag** parsing
+- **Alpha version** making
+- Setting found or generated version as package **poetry.version**
+- Maintenance of **PEP 440**
+- **Command** to output a new version
 
 ## Quick start
 
 ```bash
 poetry self add poetry-git-version-plugin
 poetry git-version # Write package version based on git tag
 poetry build # Build package with version based on git tag
@@ -77,18 +76,18 @@
 Three variables to **ignore errors**
 
 - Type: bool
 - Default = true
 
 ```toml
 [tool.poetry-git-version-plugin]
-# Ignore mismatch error PEP440 version format
+# Ignore mismatch error PEP 440 version format
 ignore_pep440 = true
 
-# Ignore mismatch error PEP440 public version format
+# Ignore mismatch error PEP 440 public version format
 ignore_public_pep440 = true
 
 # Ignore all errors
 # including version not found errors
 ignore_errors = true
 ```
```

### Comparing `poetry_git_version_plugin-0.1.4a5/PKG-INFO` & `poetry_git_version_plugin-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.4a5
+Version: 0.1.5
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -31,32 +31,31 @@
 Requires-Dist: gitpython (>=3.1.29,<4.0.0)
 Requires-Dist: poetry (>=1.2.2,<2.0.0)
 Project-URL: Repository, https://gitlab.com/rocshers/python/poetry-git-version-plugin
 Description-Content-Type: text/markdown
 
 # Poetry Git Version Plugin
 
-Poetry plugin to get package version from git.
+Poetry plugin to set package version based on git tag.
 
 [![PyPI](https://img.shields.io/pypi/v/poetry-git-version-plugin)](https://pypi.org/project/poetry-git-version-plugin/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-git-version-plugin)
-[![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/poetry-git-version-plugin)](https://gitlab.com/rocshers/python/poetry-git-version-plugin)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-git-version-plugin)](https://pypi.org/project/poetry-git-version-plugin/)
+[![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/poetry-git-version-plugin)](https://gitlab.com/rocshers/python/poetry-git-version-plugin)
 
 [![Test coverage](https://codecov.io/gitlab/rocshers:python/poetry-git-version-plugin/branch/release/graph/badge.svg?token=RPFNZ8SBQ6)](https://codecov.io/gitlab/rocshers:python/poetry-git-version-plugin)
 [![Downloads](https://static.pepy.tech/badge/poetry-git-version-plugin)](https://pepy.tech/project/poetry-git-version-plugin)
-![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/poetry-git-version-plugin)
-[![pipeline status](https://gitlab.com/rocshers/python/poetry-git-version-plugin/badges/release/pipeline.svg)](https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/commits/release)
+[![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/poetry-git-version-plugin)](https://gitlab.com/rocshers/python/poetry-git-version-plugin)
 
 ## Functionality
 
-- Git tag parsing
-- Make alpha version
-- Substitution of the project tag (if any) in the poetry.version value
-- Maintenance of PEP 440
-- Command to output a new version
+- **Git tag** parsing
+- **Alpha version** making
+- Setting found or generated version as package **poetry.version**
+- Maintenance of **PEP 440**
+- **Command** to output a new version
 
 ## Quick start
 
 ```bash
 poetry self add poetry-git-version-plugin
 poetry git-version # Write package version based on git tag
 poetry build # Build package with version based on git tag
@@ -112,18 +111,18 @@
 Three variables to **ignore errors**
 
 - Type: bool
 - Default = true
 
 ```toml
 [tool.poetry-git-version-plugin]
-# Ignore mismatch error PEP440 version format
+# Ignore mismatch error PEP 440 version format
 ignore_pep440 = true
 
-# Ignore mismatch error PEP440 public version format
+# Ignore mismatch error PEP 440 public version format
 ignore_public_pep440 = true
 
 # Ignore all errors
 # including version not found errors
 ignore_errors = true
 ```
```

