# Comparing `tmp/robotcode_runner-0.35.0.tar.gz` & `tmp/robotcode_runner-0.36.0.tar.gz`

## Comparing `robotcode_runner-0.35.0.tar` & `robotcode_runner-0.36.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/PKG-INFO
```

### Comparing `robotcode_runner-0.35.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.36.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.35.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.36.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.35.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.36.0/src/robotcode/runner/cli/robot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,176 @@
 import os
+import sys
 from pathlib import Path
 from typing import Any, List, Optional, Tuple, Union, cast
 
 import click
 from robot.errors import DataError, Information
 from robot.run import USAGE, RobotFramework
 from robot.version import get_full_version
 from robotcode.plugin import Application, pass_application
 from robotcode.plugin.click_helper.aliases import AliasedCommand
+from robotcode.plugin.click_helper.types import add_options
 from robotcode.robot.config.loader import load_config_from_path
+from robotcode.robot.config.model import RobotBaseProfile
 from robotcode.robot.config.utils import get_config_files
 
 from ..__version__ import __version__
 
 
 class RobotFrameworkEx(RobotFramework):
-    def __init__(self, paths: List[str], dry: bool, root_folder: Optional[Path]) -> None:
+    def __init__(self, app: Application, paths: List[str], dry: bool, root_folder: Optional[Path]) -> None:
         super().__init__()
+        self.app = app
         self.paths = paths
         self.dry = dry
         self.root_folder = root_folder
+        self._orig_cwd = Path.cwd()
 
     def parse_arguments(self, cli_args: Any) -> Any:
+        if self.root_folder is not None:
+            self.app.verbose(f"Changing working directory from {self._orig_cwd} to {self.root_folder}")
+            os.chdir(self.root_folder)
+
         try:
             options, arguments = super().parse_arguments(cli_args)
+            if self.root_folder is not None:
+                for i, arg in enumerate(arguments.copy()):
+                    if Path(arg).is_absolute():
+                        continue
+
+                    arguments[i] = str((self._orig_cwd / Path(arg)).absolute().relative_to(self.root_folder))
+
         except DataError:
             options, arguments = super().parse_arguments((*cli_args, *self.paths))
 
         if not arguments:
             arguments = self.paths
 
-        if self.root_folder is not None:
-            for i, arg in enumerate(arguments.copy()):
-                if Path(arg).is_absolute():
-                    continue
-
-                arguments[i] = str(Path(arg).absolute().relative_to(self.root_folder))
-
         if self.dry:
             line_end = "\n"
             raise Information(
                 "Dry run, not executing any commands. "
                 f"Would execute robot with the following options and arguments:\n"
                 f'{line_end.join((*(f"{k} = {repr(v)}" for k, v in options.items()) ,*arguments))}'
             )
 
         return options, arguments
 
-    def main(self, arguments: Any, **options: Any) -> Any:
-        if self.root_folder is not None:
-            os.chdir(self.root_folder)
 
-        return super().main(arguments, **options)
+ROBOT_OPTIONS = (
+    click.option("--by-longname", type=str, multiple=True, help="Select tests/tasks or suites by longname."),
+    click.option(
+        "--exclude-by-longname",
+        type=str,
+        multiple=True,
+        help="Excludes tests/tasks or suites by longname.",
+    ),
+    click.version_option(
+        version=__version__,
+        package_name="robotcode.runner",
+        prog_name="RobotCode Runner",
+        message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
+    ),
+    click.argument("robot_options_and_args", nargs=-1, type=click.Path()),
+)
 
 
-@click.command(
-    cls=AliasedCommand,
-    aliases=["run"],
-    context_settings={
-        "allow_extra_args": True,
-        "ignore_unknown_options": True,
-    },
-    add_help_option=True,
-    epilog='Use "-- --help" to see `robot` help.',
-)
-@click.option("--by-longname", type=str, multiple=True, help="Select tests/tasks or suites by longname.")
-@click.option(
-    "--exclude-by-longname",
-    type=str,
-    multiple=True,
-    help="Excludes tests/tasks or suites by longname.",
-)
-@click.version_option(
-    version=__version__,
-    package_name="robotcode.runner",
-    prog_name="RobotCode Runner",
-    message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
-)
-@click.argument("robot_options_and_args", nargs=-1, type=click.Path())
-@pass_application
-def robot(
+def handle_robot_options(
     app: Application,
     by_longname: Tuple[str, ...],
     exclude_by_longname: Tuple[str, ...],
     robot_options_and_args: Tuple[str, ...],
-) -> None:
-    """Runs `robot` with the selected configuration, profiles, options and arguments.
-
-    The options and arguments are passed to `robot` as is.
-
-    Examples:
-    ```
-    robotcode run
-    ```
-    """
-
+) -> Tuple[Optional[Path], RobotBaseProfile, List[str]]:
     robot_arguments: Optional[List[Union[str, Path]]] = None
+    old_sys_path = sys.path.copy()
     try:
         _, robot_arguments = RobotFramework().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
+    finally:
+        sys.path = old_sys_path
 
     config_files, root_folder, _ = get_config_files(
         robot_arguments, app.config.config_files, raise_on_error=False, verbose_callback=app.verbose
     )
     try:
         profile = (
             load_config_from_path(*config_files)
             .combine_profiles(*(app.config.profiles or []), verbose_callback=app.verbose)
             .evaluated()
         )
     except (TypeError, ValueError) as e:
         raise click.ClickException(str(e)) from e
 
-    options = profile.build_command_line()
+    cmd_options = profile.build_command_line()
 
     if by_longname:
         sep = ";" if any(True for l in by_longname if ":" in l) else ":"
-        options += ("--prerunmodifier", f"robotcode.modifiers.ByLongName:{sep.join(by_longname)}")
+        cmd_options += ("--prerunmodifier", f"robotcode.modifiers.ByLongName{sep}{sep.join(by_longname)}")
 
     if exclude_by_longname:
         sep = ";" if any(True for l in exclude_by_longname if ":" in l) else ":"
-        options += ("--prerunmodifier", f"robotcode.modifiers.ExcludedByLongName:{sep.join(exclude_by_longname)}")
+        cmd_options += (
+            "--prerunmodifier",
+            f"robotcode.modifiers.ExcludedByLongName{sep}{sep.join(exclude_by_longname)}",
+        )
 
     if profile.env:
         for k, v in profile.env.items():
             os.environ[k] = v
             app.verbose(lambda: f"Set environment variable {k} to {v}")
 
     app.verbose(
         lambda: "Executing robot with the following options:\n    "
-        + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
+        + " ".join(f'"{o}"' for o in (cmd_options + list(robot_options_and_args)))
+    )
+
+    return root_folder, profile, cmd_options
+
+
+@click.command(
+    cls=AliasedCommand,
+    aliases=["run"],
+    context_settings={
+        "allow_extra_args": True,
+        "ignore_unknown_options": True,
+    },
+    add_help_option=True,
+    epilog='Use "-- --help" to see `robot` help.',
+)
+@add_options(*ROBOT_OPTIONS)
+@pass_application
+def robot(
+    app: Application,
+    by_longname: Tuple[str, ...],
+    exclude_by_longname: Tuple[str, ...],
+    robot_options_and_args: Tuple[str, ...],
+) -> None:
+    """Runs `robot` with the selected configuration, profiles, options and arguments.
+
+    The options and arguments are passed to `robot` as is.
+
+    Examples:
+    ```
+    robotcode run
+    ```
+    """
+
+    root_folder, profile, cmd_options = handle_robot_options(
+        app, by_longname, exclude_by_longname, robot_options_and_args
     )
 
     app.exit(
         cast(
             int,
             RobotFrameworkEx(
+                app,
                 [] if profile.paths is None else profile.paths if isinstance(profile.paths, list) else [profile.paths],
                 app.config.dry,
                 root_folder,
             ).execute_cli(
-                (*options, *robot_options_and_args),
+                (*cmd_options, *robot_options_and_args),
                 exit=False,
             ),
         )
     )
```

### Comparing `robotcode_runner-0.35.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.36.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.35.0/.gitignore` & `robotcode_runner-0.36.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.35.0/LICENSE.txt` & `robotcode_runner-0.36.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.35.0/README.md` & `robotcode_runner-0.36.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.35.0/pyproject.toml` & `robotcode_runner-0.36.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.35.0",
-  "robotcode-modifiers==0.35.0",
-  "robotcode==0.35.0",
+  "robotcode-robot==0.36.0",
+  "robotcode-modifiers==0.36.0",
+  "robotcode==0.36.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.35.0/PKG-INFO` & `robotcode_runner-0.36.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.35.0
+Version: 0.36.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.35.0
-Requires-Dist: robotcode-robot==0.35.0
-Requires-Dist: robotcode==0.35.0
+Requires-Dist: robotcode-modifiers==0.36.0
+Requires-Dist: robotcode-robot==0.36.0
+Requires-Dist: robotcode==0.36.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

