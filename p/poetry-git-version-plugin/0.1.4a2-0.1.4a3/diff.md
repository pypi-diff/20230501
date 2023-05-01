# Comparing `tmp/poetry_git_version_plugin-0.1.4a2.tar.gz` & `tmp/poetry_git_version_plugin-0.1.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-0.1.4a2.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-0.1.4a3.tar", max compression
```

## Comparing `poetry_git_version_plugin-0.1.4a2.tar` & `poetry_git_version_plugin-0.1.4a3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 10:00:45.410317 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1651 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1550 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5240 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2837 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/pyproject.toml
--rw-r--r--   0        0        0     1639 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a2/readme.md
--rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4a2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 11:35:48.258809 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     1651 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      758 2023-05-01 10:00:45.334318 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1550 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5240 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0     2837 2023-05-01 10:00:45.338318 poetry_git_version_plugin-0.1.4a3/pyproject.toml
+-rw-r--r--   0        0        0     3449 2023-05-01 11:35:48.190810 poetry_git_version_plugin-0.1.4a3/readme.md
+-rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 poetry_git_version_plugin-0.1.4a3/PKG-INFO
```

### Comparing `poetry_git_version_plugin-0.1.4a2/LICENSE` & `poetry_git_version_plugin-0.1.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/plugins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
+from poetry.core.constraints.version import Version
 from poetry.plugins.application_plugin import ApplicationPlugin
 from poetry.plugins.plugin import Plugin
 from poetry.poetry import Poetry
 
 from poetry_git_version_plugin import config
 from poetry_git_version_plugin.commands import GitVersionCommand
 from poetry_git_version_plugin.exceptions import PluginException, plugin_exception_wrapper
 from poetry_git_version_plugin.services import GitVersionService
-from poetry.core.constraints.version import Version
 
 
 class PoetryGitVersionPlugin(Plugin):
     """Плагин определения версии по гит тегу"""
 
     @plugin_exception_wrapper
     def activate(self, poetry: Poetry, io: IO):
```

### Comparing `poetry_git_version_plugin-0.1.4a2/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-0.1.4a3/poetry_git_version_plugin/services.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from pathlib import Path
 from typing import List, Optional
 
 import git
-from git.objects import Commit
 from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
+from git.objects import Commit
 from packaging.version import VERSION_PATTERN
 
 from poetry_git_version_plugin import config
 from poetry_git_version_plugin.exceptions import PluginException
 
 VERSION_REGEX_COMPILE = re.compile(r'^\s*' + VERSION_PATTERN + r'\s*$', re.VERBOSE | re.IGNORECASE)
 VERSION_CANON_REGEX_COMPILE = re.compile(
```

### Comparing `poetry_git_version_plugin-0.1.4a2/pyproject.toml` & `poetry_git_version_plugin-0.1.4a3/pyproject.toml`

 * *Files identical despite different names*

