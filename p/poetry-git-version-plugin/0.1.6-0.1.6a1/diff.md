# Comparing `tmp/poetry_git_version_plugin-0.1.6.tar.gz` & `tmp/poetry_git_version_plugin-0.1.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.6.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.6a1.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.6.tar` & `poetry_git_version_plugin-0.1.6a1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 18:09:40.772367 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1187 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5662 2023-05-01 18:03:38.089366 poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2832 2023-05-01 18:09:19.632432 poetry_git_version_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4402 2023-05-01 17:03:01.127393 poetry_git_version_plugin-0.1.6/readme.md
--rw-r--r--   0        0        0     5954 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.6a1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 19:05:14.286729 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      837 2023-05-01 19:02:48.091434 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1114 2023-05-01 19:02:48.091434 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5882 2023-05-01 19:02:48.095434 poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2776 2023-05-01 19:04:49.982846 poetry_git_version_plugin-0.1.6a1/pyproject.toml
+-rw-r--r--   0        0        0     4406 2023-05-01 19:02:48.095434 poetry_git_version_plugin-0.1.6a1/readme.md
+-rw-r--r--   0        0        0     5960 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.6a1/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.6/LICENSE` & `poetry_git_version_plugin-0.1.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 class PluginException(RuntimeError):
     def __str__(self) -> str:
         if isinstance(self.args[0], BaseException):
             ex = self.args[0]
             message = ex.__class__.__name__
             if ex.args:
-                message = f'{message}: {ex.args}'
+                args_message = ': ' + '; '.join(ex.args) if ex.args else ''
+                message = f'{message}{args_message}'
 
         else:
             message = '; '.join(self.args)
 
         return f'<b>{config.PLUGIN_NAME}</b>: {message}'
```

### Comparing `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/plugins.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 class PoetryGitVersionPlugin(Plugin):
     """Плагин определения версии по гит тегу"""
 
     @plugin_exception_wrapper
     def activate(self, poetry: Poetry, io: IO):  # pragma: no cover
         io.write_line(f'<b>{config.PLUGIN_NAME}</b>: Init', Verbosity.VERBOSE)
 
-        plugin_config = config.PluginConfig(poetry.pyproject)
-
-        version = VersionService(io, plugin_config).get_version()
+        version = VersionService.safe_get_version(io, poetry)
 
         if version is not None:
             poetry.package.version = version
 
-        io.write_error_line(f'<b>{config.PLUGIN_NAME}</b>: Finished\n', Verbosity.VERBOSE)
+        io.write_line(f'<b>{config.PLUGIN_NAME}</b>: Finished\n', Verbosity.VERBOSE)
 
 
 class PoetryGitVersionApplicationPlugin(ApplicationPlugin):
     commands = [GitVersionCommand]
```

### Comparing `poetry_git_version_plugin-0.1.6/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.6a1/poetry_git_version_plugin/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import git
 from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
 from git.objects import Commit
 from packaging.version import VERSION_PATTERN
 from poetry.core.constraints.version import Version
+from poetry.poetry import Poetry
 
 from poetry_git_version_plugin import config
 from poetry_git_version_plugin.exceptions import PluginException
 
 VERSION_REGEX_COMPILE = re.compile(r'^\s*' + VERSION_PATTERN + r'\s*$', re.VERBOSE | re.IGNORECASE)
 VERSION_CANON_REGEX_COMPILE = re.compile(
     r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)(0|[1-9][0-9]*))?(\.post(0|[1-9][0-9]*))?(\.dev(0|[1-9][0-9]*))?$'
@@ -161,23 +162,30 @@
 
         if is_valid == 2:
             self.io.write_line(f'Invalid public PEP 440 version: "{version}"', Verbosity.VERBOSE)
 
             if not self.plugin_config.ignore_public_pep440:
                 raise PluginException(f'Invalid public PEP 440 version: "{version}"')
 
-    def get_version(self) -> Optional[Version]:
+    def get_version(self) -> str:
+        version = self.__get_version()
+        self.validate_version(version)
+        return version
+
+    @classmethod
+    def safe_get_version(cls, io: IO, poetry: Poetry) -> Optional[Version]:
+        plugin_config = config.PluginConfig(poetry.pyproject)
+
         try:
-            version = self.__get_version()
-            self.validate_version(version)
+            version = cls(io, plugin_config).get_version()
             return Version.parse(version)
 
         except Exception as ex:
-            if not self.plugin_config.ignore_errors:
+            if not plugin_config.ignore_errors:
                 raise ex
 
             if not isinstance(ex, PluginException):
                 ex = PluginException(ex)
 
-            self.io.write_error_line(f'{ex}. Ignore Exception\n', Verbosity.VERBOSE)
+            io.write_error_line(f'{ex}. Ignore Exception.')
 
             return None
```

### Comparing `poetry_git_version_plugin-0.1.6/pyproject.toml` & `poetry_git_version_plugin-0.1.6a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -78,17 +78,14 @@
     "pragma: no cover",
     "def __repr__",
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
 ]
 
-[tool.poetry-git-version-plugin]
-ignore_errors = false
-
 [tool.pytest.ini_options]
 addopts = "-vvs --tb=short"
 xfail_strict = true
 testpaths = [
     "tests",
     "integration",
 ]
@@ -98,8 +95,8 @@
 ]
 filterwarnings = [
     "ignore::DeprecationWarning",
     "ignore:Module already imported:pytest.PytestWarning"
 ]
 
 [tool.mypy]
-python_version = 3.7
+python_version = 3.8
```

### Comparing `poetry_git_version_plugin-0.1.6/readme.md` & `poetry_git_version_plugin-0.1.6a1/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 Issue Tracker: <https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/issues>  
 Source Code: <https://gitlab.com/rocshers/python/poetry-git-version-plugin>
 
 Before adding changes:
 
 ```bash
-make install
+make install-dev
 ```
 
 After changes:
 
 ```bash
 make format test
 ```
```

### Comparing `poetry_git_version_plugin-0.1.6/PKG-INFO` & `poetry_git_version_plugin-0.1.6a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 0.1.6
+Version: 0.1.6a1
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -184,15 +184,15 @@
 
 Issue Tracker: <https://gitlab.com/rocshers/python/poetry-git-version-plugin/-/issues>  
 Source Code: <https://gitlab.com/rocshers/python/poetry-git-version-plugin>
 
 Before adding changes:
 
 ```bash
-make install
+make install-dev
 ```
 
 After changes:
 
 ```bash
 make format test
 ```
```

