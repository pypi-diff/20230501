# Comparing `tmp/robotcode_robot-0.35.0.tar.gz` & `tmp/robotcode_robot-0.36.0.tar.gz`

## Comparing `robotcode_robot-0.35.0.tar` & `robotcode_robot-0.36.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    77317 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    77317 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/pyproject.toml
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/PKG-INFO
```

### Comparing `robotcode_robot-0.35.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.36.0/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.35.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.36.0/src/robotcode/robot/config/model.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.35.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.36.0/src/robotcode/robot/config/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     raise_on_error: bool = True,
     verbose_callback: Optional[Callable[[str], None]] = None,
 ) -> Tuple[Sequence[Tuple[Path, ConfigType]], Optional[Path], DiscoverdBy]:
     root_folder, discovered_by = find_project_root(*(paths or []))
 
     if root_folder is None:
         if raise_on_error:
-            raise FileNotFoundError("Cannot detect root folder for project. 😥")
+            raise FileNotFoundError("Cannot detect root folder. 😥")
         if verbose_callback:
-            verbose_callback("Cannot detect root folder for project. 😥")
+            verbose_callback("Cannot detect root folder. 😥")
         return [], None, DiscoverdBy.NOT_FOUND
 
     if verbose_callback:
-        verbose_callback(f"Found project root at:\n    {root_folder} ({discovered_by.value})")
+        verbose_callback(f"Found root at:\n    {root_folder} ({discovered_by.value})")
 
     if config_files:
         if verbose_callback:
             verbose_callback("Using config file:" + "\n    ".join(str(config_files)))
 
         return [(f, ConfigType.CUSTOM_TOML) for f in config_files], root_folder, discovered_by
```

### Comparing `robotcode_robot-0.35.0/.gitignore` & `robotcode_robot-0.36.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.35.0/LICENSE.txt` & `robotcode_robot-0.36.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.35.0/README.md` & `robotcode_robot-0.36.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.35.0/pyproject.toml` & `robotcode_robot-0.36.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core==0.35.0",
+  "robotcode-core==0.36.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.35.0/PKG-INFO` & `robotcode_robot-0.36.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.35.0
+Version: 0.36.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.35.0
+Requires-Dist: robotcode-core==0.36.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

