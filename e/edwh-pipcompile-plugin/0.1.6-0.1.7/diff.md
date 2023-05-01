# Comparing `tmp/edwh_pipcompile_plugin-0.1.6.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.7.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.6.tar` & `edwh_pipcompile_plugin-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/README.md
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/README.md
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.6/CHANGELOG.md` & `edwh_pipcompile_plugin-0.1.7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.7 (2023-05-01)
+### Fix
+* **upgrade:** `pip.upgrade` now actually includes the upgrade flag to pip-compile ([`8ada23d`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/8ada23df192f3813a6628c0ca77169dadae058ca))
+
 ## v0.1.6 (2023-04-17)
 ### Fix
 * **semver:** Semantic-release types should be a comma-separated string, not an array ([`4dd0394`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/4dd039434decb2ed8e2b1feff6a061f5bc49b4e3))
 
 ## v0.1.5 (2023-04-17)
```

### Comparing `edwh_pipcompile_plugin-0.1.6/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.7/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.6/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
         PACKAGE_RE.format(package=package),
         re.MULTILINE | re.IGNORECASE,
     )
 
 
 ### ONLY @task's AFTER THIS!!!
 
+
 @task()
 def compile(ctx, path, pypi_server=DEFAULT_SERVER):
     """
     Task (invoke pip.compile) to run pip-compile on one or more files (-f requirements1.in -f requirements2.in)
 
     Arguments:
         ctx (invoke.Context): invoke context
@@ -279,17 +280,15 @@
     for file in files:
         with open(file, "r") as f:
             contents = f.read()
 
         _package, *_ = extract_package_info(package)
 
         if compile_package_re(_package).search(contents):
-            error(
-                f"Warning: {_package} already installed, use pip-upgrade to upgrade. "
-            )
+            error(f"Warning: {_package} already installed, use pip-upgrade to upgrade. ")
             continue
 
         with open(file, "a") as f:
             f.write("\n" + package)
 
         success(f"Installing {package} in {file}")
 
@@ -317,15 +316,15 @@
     files = _find_infiles(Path(path))
 
     for file in files:
         with open(file, "r") as f:
             contents = f.read()
 
         out = in_to_out(file)
-        args = {}
+        args = {"upgrade": True}
         if pypi_server:
             args["i"] = pypi_server
 
         if package:
             _package, operator, version = extract_package_info(package)
 
             reg = compile_package_re(_package)
@@ -340,17 +339,15 @@
 
             if force or (operator and version):
                 with open(file, "w") as f:
                     f.write(reg.sub(package, contents))
             else:
                 dep_version = dependency[0][2]
                 if dep_version:
-                    warn(
-                        f"{package} is pinned to {dep_version} in {file}. Use --force to upgrade anyway."
-                    )
+                    warn(f"{package} is pinned to {dep_version} in {file}. Use --force to upgrade anyway.")
                     continue
                 # else: --upgrade-package will do its job
 
             # arg = f'--upgrade-package "{package}"'
             args["upgrade-package"] = package
 
             success(f"Upgrading {package} in {file}")
@@ -400,13 +397,11 @@
         # else
 
         new_deps = compile_package_re(_package).sub("", contents)
         new_deps = new_deps.replace("\n\n", "\n")  # remove empty line
         with open(file, "w") as f:
             f.write(new_deps)
 
-        with show_diff(
-            in_to_out(file)
-        ):  # no rollback required since pip compile can't fail on remove
+        with show_diff(in_to_out(file)):  # no rollback required since pip compile can't fail on remove
             compile(ctx, path=path, pypi_server=pypi_server)
 
         success(f"Package {_package} removed from {file}")
```

### Comparing `edwh_pipcompile_plugin-0.1.6/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.6/README.md` & `edwh_pipcompile_plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.6/pyproject.toml` & `edwh_pipcompile_plugin-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.6/PKG-INFO` & `edwh_pipcompile_plugin-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

