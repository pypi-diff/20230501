# Comparing `tmp/commitizen-3.1.1.tar.gz` & `tmp/commitizen-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.1.1.tar", max compression
+gzip compressed data, was "commitizen-3.2.0.tar", max compression
```

## Comparing `commitizen-3.1.1.tar` & `commitizen-3.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-04-28 07:42:11.206104 commitizen-3.1.1/LICENSE
--rw-r--r--   0        0        0      593 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/__version__.py
--rw-r--r--   0        0        0     8613 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/bump.py
--rw-r--r--   0        0        0    11956 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16605 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13932 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7266 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5067 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/check.py
--rw-r--r--   0        0        0     3059 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-04-28 07:42:11.206104 commitizen-3.1.1/commitizen/commands/info.py
--rw-r--r--   0        0        0    12935 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/commands/version.py
--rw-r--r--   0        0        0     1229 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/__init__.py
--rw-r--r--   0        0        0      915 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1384 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1753 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1438 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1226 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     3016 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3125 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3310 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/factory.py
--rw-r--r--   0        0        0     6916 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/out.py
--rw-r--r--   0        0        0     6657 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2400 2023-04-28 07:42:11.210104 commitizen-3.1.1/commitizen/version_types.py
--rw-r--r--   0        0        0     5800 2023-04-28 07:42:11.210104 commitizen-3.1.1/docs/README.md
--rw-r--r--   0        0        0     3959 2023-04-28 07:42:11.222104 commitizen-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 18:45:22.914135 commitizen-3.2.0/LICENSE
+-rw-r--r--   0        0        0      609 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     8609 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/bump.py
+-rw-r--r--   0        0        0    11956 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3431 2023-05-01 18:45:22.914135 commitizen-3.2.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16927 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13932 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7266 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5067 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12929 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1229 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      915 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1575 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1753 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1438 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1226 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     3016 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7114 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3125 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      272 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3327 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/factory.py
+-rw-r--r--   0        0        0     6916 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/out.py
+-rw-r--r--   0        0        0     6657 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2400 2023-05-01 18:45:22.918135 commitizen-3.2.0/commitizen/version_types.py
+-rw-r--r--   0        0        0     5748 2023-05-01 18:45:22.918135 commitizen-3.2.0/docs/README.md
+-rw-r--r--   0        0        0     3929 2023-05-01 18:45:22.930135 commitizen-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 commitizen-3.2.0/PKG-INFO
```

### Comparing `commitizen-3.1.1/LICENSE` & `commitizen-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/__init__.py` & `commitizen-3.2.0/commitizen/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import logging.config
 
-from colorama import init
+from colorama import init  # type: ignore
 
 from commitizen.cz.base import BaseCommitizen
 
 init()
 
 
 LOGGING = {
```

### Comparing `commitizen-3.1.1/commitizen/bump.py` & `commitizen-3.2.0/commitizen/bump.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,36 +19,36 @@
     # workaround mypy issue for 3.7 python
     VersionProtocol = typing.Any
 
 
 def find_increment(
     commits: List[GitCommit], regex: str, increments_map: Union[dict, OrderedDict]
 ) -> Optional[str]:
-
     if isinstance(increments_map, dict):
         increments_map = OrderedDict(increments_map)
 
     # Most important cases are major and minor.
     # Everything else will be considered patch.
     select_pattern = re.compile(regex)
     increment: Optional[str] = None
 
     for commit in commits:
         for message in commit.message.split("\n"):
             result = select_pattern.search(message)
+
             if result:
-                found_keyword = result.group(0)
+                found_keyword = result.group(1)
                 new_increment = None
                 for match_pattern in increments_map.keys():
                     if re.match(match_pattern, found_keyword):
                         new_increment = increments_map[match_pattern]
                         break
 
                 if increment == "MAJOR":
-                    continue
+                    break
                 elif increment == "MINOR" and new_increment == "MAJOR":
                     increment = new_increment
                 elif increment == "PATCH" or increment is None:
                     increment = new_increment
 
     return increment
 
@@ -99,15 +99,14 @@
     increments_version = dict(zip_longest(increments, prev_release, fillvalue=0))
 
     # This flag means that current version
     # must remove its prerelease tag,
     # so it doesn't matter the increment.
     # Example: 1.0.0a0 with PATCH/MINOR -> 1.0.0
     if not version.is_prerelease:
-
         if increment == MAJOR:
             increments_version[MAJOR] += 1
             increments_version[MINOR] = 0
             increments_version[PATCH] = 0
         elif increment == MINOR:
             increments_version[MINOR] += 1
             increments_version[PATCH] = 0
```

### Comparing `commitizen-3.1.1/commitizen/changelog.py` & `commitizen-3.2.0/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/changelog_parser.py` & `commitizen-3.2.0/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cli.py` & `commitizen-3.2.0/commitizen/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import logging
 import sys
+from pathlib import Path
 from functools import partial
 from types import TracebackType
 from typing import List
 
 import argcomplete
 from decli import cli
 
@@ -59,17 +60,23 @@
                     },
                     {
                         "name": "--dry-run",
                         "action": "store_true",
                         "help": "show output to stdout, no commit, no modified files",
                     },
                     {
+                        "name": "--write-message-to-file",
+                        "type": Path,
+                        "metavar": "FILE_PATH",
+                        "help": "write message to file before commiting (can be combined with --dry-run)",
+                    },
+                    {
                         "name": ["-s", "--signoff"],
                         "action": "store_true",
-                        "help": "Sign off the commit",
+                        "help": "sign off the commit",
                     },
                 ],
             },
             {
                 "name": "ls",
                 "help": "show available commitizens",
                 "func": commands.ListCz,
```

### Comparing `commitizen-3.1.1/commitizen/cmd.py` & `commitizen-3.2.0/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/commands/bump.py` & `commitizen-3.2.0/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/commands/changelog.py` & `commitizen-3.2.0/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/commands/check.py` & `commitizen-3.2.0/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/commands/commit.py` & `commitizen-3.2.0/commitizen/commands/commit.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from commitizen.exceptions import (
     CommitError,
     CustomError,
     DryRunExit,
     NoAnswersError,
     NoCommitBackupError,
     NotAGitProjectError,
+    NotAllowed,
     NothingToCommitError,
 )
 from commitizen.git import smart_open
 
 
 class Commit:
     """Show prompt for the user to create a guided commit."""
@@ -59,27 +60,35 @@
 
         if not answers:
             raise NoAnswersError()
         return cz.message(answers)
 
     def __call__(self):
         dry_run: bool = self.arguments.get("dry_run")
+        write_message_to_file = self.arguments.get("write_message_to_file")
 
         if git.is_staging_clean() and not dry_run:
             raise NothingToCommitError("No files added to staging!")
 
+        if write_message_to_file is not None and write_message_to_file.is_dir():
+            raise NotAllowed(f"{write_message_to_file} is a directory")
+
         retry: bool = self.arguments.get("retry")
 
         if retry:
             m = self.read_backup_message()
         else:
             m = self.prompt_commit_questions()
 
         out.info(f"\n{m}\n")
 
+        if write_message_to_file:
+            with smart_open(write_message_to_file, "w") as file:
+                file.write(m)
+
         if dry_run:
             raise DryRunExit()
 
         signoff: bool = self.arguments.get("signoff")
 
         if signoff:
             c = git.commit(m, "-s")
```

### Comparing `commitizen-3.1.1/commitizen/commands/init.py` & `commitizen-3.2.0/commitizen/commands/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return os.path.isfile(".pre-commit-config.yaml")
 
     @property
     def is_python_poetry(self) -> bool:
         if not self.has_pyproject:
             return False
         with open("pyproject.toml") as f:
-            return "tool.poetry.version" in f.read()
+            return "[tool.poetry]" in f.read()
 
     @property
     def is_python(self) -> bool:
         return self.has_pyproject or self.has_setup
 
     @property
     def is_rust_cargo(self) -> bool:
```

### Comparing `commitizen-3.1.1/commitizen/commands/version.py` & `commitizen-3.2.0/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/config/__init__.py` & `commitizen-3.2.0/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/config/base_config.py` & `commitizen-3.2.0/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/config/json_config.py` & `commitizen-3.2.0/commitizen/config/json_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 from pathlib import Path
 from typing import Union
+from commitizen.exceptions import InvalidConfigurationError
 
 from commitizen.git import smart_open
 
 from .base_config import BaseConfig
 
 
 class JsonConfig(BaseConfig):
     def __init__(self, *, data: Union[bytes, str], path: Union[Path, str]):
         super(JsonConfig, self).__init__()
         self.is_empty_config = False
-        self._parse_setting(data)
         self.add_path(path)
+        self._parse_setting(data)
 
     def init_empty_config_content(self):
         with smart_open(self.path, "a") as json_file:
             json.dump({"commitizen": {}}, json_file)
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
@@ -39,12 +40,16 @@
         {
             "commitizen": {
                 "name": "cz_conventional_commits"
             }
         }
         ```
         """
-        doc = json.loads(data)
+        try:
+            doc = json.loads(data)
+        except json.JSONDecodeError:
+            raise InvalidConfigurationError(f"Failed to parse {self.path}")
+
         try:
             self.settings.update(doc["commitizen"])
         except KeyError:
             self.is_empty_config = True
```

### Comparing `commitizen-3.1.1/commitizen/config/toml_config.py` & `commitizen-3.2.0/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/config/yaml_config.py` & `commitizen-3.2.0/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/__init__.py` & `commitizen-3.2.0/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/base.py` & `commitizen-3.2.0/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.2.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/customize/customize.py` & `commitizen-3.2.0/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/jira/jira.py` & `commitizen-3.2.0/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/cz/jira/jira_info.txt` & `commitizen-3.2.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/defaults.py` & `commitizen-3.2.0/commitizen/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     "version_type": None,
 }
 
 MAJOR = "MAJOR"
 MINOR = "MINOR"
 PATCH = "PATCH"
 
-bump_pattern = r"^(BREAKING[\-\ ]CHANGE|feat|fix|refactor|perf)(\(.+\))?(!)?"
+bump_pattern = r"^(((BREAKING[\-\ ]CHANGE|feat|fix|refactor|perf)(\(.+\))?(!)?)|\w+!):"
 bump_map = OrderedDict(
     (
         (r"^.+!$", MAJOR),
         (r"^BREAKING[\-\ ]CHANGE", MAJOR),
         (r"^feat", MINOR),
         (r"^fix", PATCH),
         (r"^refactor", PATCH),
@@ -108,9 +108,9 @@
         (r"^refactor", PATCH),
         (r"^perf", PATCH),
     )
 )
 change_type_order = ["BREAKING CHANGE", "Feat", "Fix", "Refactor", "Perf"]
 bump_message = "bump: version $current_version → $new_version"
 
-commit_parser = r"^(?P<change_type>feat|fix|refactor|perf|BREAKING CHANGE)(?:\((?P<scope>[^()\r\n]*)\)|\()?(?P<breaking>!)?:\s(?P<message>.*)?"  # noqa
+commit_parser = r"^((?P<change_type>feat|fix|refactor|perf|BREAKING CHANGE)(?:\((?P<scope>[^()\r\n]*)\)|\()?(?P<breaking>!)?|\w+!):\s(?P<message>.*)?"  # noqa
 version_parser = r"(?P<version>([0-9]+)\.([0-9]+)\.([0-9]+)(?:-([0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+[0-9A-Za-z-]+)?(\w+)?)"
```

### Comparing `commitizen-3.1.1/commitizen/exceptions.py` & `commitizen-3.2.0/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/factory.py` & `commitizen-3.2.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/git.py` & `commitizen-3.2.0/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/hooks.py` & `commitizen-3.2.0/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/out.py` & `commitizen-3.2.0/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/providers.py` & `commitizen-3.2.0/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/commitizen/version_types.py` & `commitizen-3.2.0/commitizen/version_types.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.1.1/docs/README.md` & `commitizen-3.2.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 - Display information about your commit rules (commands: schema, example, info)
 - Create your own set of rules and publish them to pip. Read more on [Customization](./customization.md)
 
 ## Requirements
 
 [Python](https://www.python.org/downloads/) `3.7+`
 
-[Poetry](https://python-poetry.org/docs/) `1.2.0+`
-
 [Git][gitscm] `1.8.5.2+`
 
 ## Installation
 
 To make commitizen available in your system
 
 ```bash
```

### Comparing `commitizen-3.1.1/pyproject.toml` & `commitizen-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.1.1"
+version = "3.2.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.1.1"
+version = "3.2.0"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 questionary = "^1.4.0"
-decli = "^0.5.2"
+decli = "^0.6.0"
 colorama = "^0.4.1"
 termcolor = ">= 1.1, < 3"
 packaging = ">=19"
 tomlkit = ">=0.5.3,<1.0.0"
 jinja2 = ">=2.10.3"
 pyyaml = ">=3.08"
 argcomplete = ">=1.12.1,<3.1"
@@ -136,14 +136,13 @@
 known-first-party = ["commitizen", "tests"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.mypy]
 files = "commitizen"
-ignore_missing_imports = true
 disallow_untyped_decorators = true
 disallow_subclassing_any = true
 warn_return_any = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unused_configs = true
```

### Comparing `commitizen-3.1.1/PKG-INFO` & `commitizen-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: argcomplete (>=1.12.1,<3.1)
 Requires-Dist: charset-normalizer (>=2.1.0,<4)
 Requires-Dist: colorama (>=0.4.1,<0.5.0)
-Requires-Dist: decli (>=0.5.2,<0.6.0)
+Requires-Dist: decli (>=0.6.0,<0.7.0)
 Requires-Dist: importlib_metadata (>=4.13,<5)
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: packaging (>=19)
 Requires-Dist: pyyaml (>=3.08)
 Requires-Dist: questionary (>=1.4.0,<2.0.0)
 Requires-Dist: termcolor (>=1.1,<3)
 Requires-Dist: tomlkit (>=0.5.3,<1.0.0)
@@ -82,16 +82,14 @@
 - Display information about your commit rules (commands: schema, example, info)
 - Create your own set of rules and publish them to pip. Read more on [Customization](./customization.md)
 
 ## Requirements
 
 [Python](https://www.python.org/downloads/) `3.7+`
 
-[Poetry](https://python-poetry.org/docs/) `1.2.0+`
-
 [Git][gitscm] `1.8.5.2+`
 
 ## Installation
 
 To make commitizen available in your system
 
 ```bash
```

