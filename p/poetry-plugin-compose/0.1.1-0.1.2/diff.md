# Comparing `tmp/poetry_plugin_compose-0.1.1.tar.gz` & `tmp/poetry_plugin_compose-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_compose-0.1.1.tar", max compression
+gzip compressed data, was "poetry_plugin_compose-0.1.2.tar", max compression
```

## Comparing `poetry_plugin_compose-0.1.1.tar` & `poetry_plugin_compose-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     3065 2023-04-29 11:44:07.318735 poetry_plugin_compose-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-09 22:22:48.699457 poetry_plugin_compose-0.1.1/poetry_plugin_compose/__init__.py
--rw-r--r--   0        0        0     2499 2023-04-29 11:00:13.820256 poetry_plugin_compose-0.1.1/poetry_plugin_compose/compose_command.py
--rw-r--r--   0        0        0     1355 2023-04-29 11:00:13.820507 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_command_list.py
--rw-r--r--   0        0        0        0 2023-04-09 23:11:55.579203 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/__init__.py
--rw-r--r--   0        0        0     1122 2023-04-29 11:43:36.561486 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_add_command.py
--rw-r--r--   0        0        0      848 2023-04-29 11:00:13.821406 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_build_command.py
--rw-r--r--   0        0        0      862 2023-04-29 11:00:13.821638 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_check_command.py
--rw-r--r--   0        0        0     3673 2023-04-29 11:28:13.459985 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_command.py
--rw-r--r--   0        0        0      218 2023-04-29 11:00:13.822441 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_command_utils.py
--rw-r--r--   0        0        0      907 2023-04-29 11:00:13.822846 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_install_command.py
--rw-r--r--   0        0        0      840 2023-04-29 11:00:13.823132 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_lock_command.py
--rw-r--r--   0        0        0      864 2023-04-29 11:00:13.823612 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_publish_command.py
--rw-r--r--   0        0        0     1167 2023-04-29 11:00:13.823871 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_remove_command.py
--rw-r--r--   0        0        0      903 2023-04-29 11:00:13.824363 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_run_command.py
--rw-r--r--   0        0        0      897 2023-04-29 11:00:13.824612 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_update_command.py
--rw-r--r--   0        0        0      905 2023-04-29 11:00:13.824969 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/dependency_order_command.py
--rw-r--r--   0        0        0     1271 2023-04-29 11:00:13.825347 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/package_filter.py
--rw-r--r--   0        0        0      515 2023-04-29 11:00:13.825956 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/sub_command_runner.py
--rw-r--r--   0        0        0        0 2023-04-29 11:00:13.826113 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-29 11:00:13.827657 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/build_dependency_graph.py
--rw-r--r--   0        0        0     1015 2023-04-29 11:00:13.828651 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/discover_packages.py
--rw-r--r--   0        0        0      821 2023-04-29 11:00:13.833010 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/get_package_dependencies.py
--rw-r--r--   0        0        0      436 2023-04-29 11:00:13.834611 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/get_package_descriptor.py
--rw-r--r--   0        0        0      124 2023-04-29 11:00:13.835880 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/sub_package_contains.py
--rw-r--r--   0        0        0      318 2023-04-29 11:00:13.836803 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/sub_package_has_dependency.py
--rw-r--r--   0        0        0      947 2023-04-10 19:09:13.625373 poetry_plugin_compose-0.1.1/poetry_plugin_compose/plugin.py
--rw-r--r--   0        0        0        0 2023-04-29 11:00:13.836957 poetry_plugin_compose-0.1.1/poetry_plugin_compose/toposort/__init__.py
--rw-r--r--   0        0        0     3567 2023-04-29 11:00:13.838018 poetry_plugin_compose-0.1.1/poetry_plugin_compose/toposort/graph.py
--rw-r--r--   0        0        0      698 2023-04-29 11:44:12.545215 poetry_plugin_compose-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 poetry_plugin_compose-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3065 2023-05-01 18:49:13.239224 poetry_plugin_compose-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 22:22:48.699457 poetry_plugin_compose-0.1.2/poetry_plugin_compose/__init__.py
+-rw-r--r--   0        0        0     2499 2023-04-29 11:00:13.820256 poetry_plugin_compose-0.1.2/poetry_plugin_compose/compose_command.py
+-rw-r--r--   0        0        0     1355 2023-04-29 11:00:13.820507 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_command_list.py
+-rw-r--r--   0        0        0        0 2023-04-09 23:11:55.579203 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/__init__.py
+-rw-r--r--   0        0        0     1122 2023-04-29 11:43:36.561486 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_add_command.py
+-rw-r--r--   0        0        0      848 2023-04-29 11:00:13.821406 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_build_command.py
+-rw-r--r--   0        0        0      862 2023-04-29 11:00:13.821638 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_check_command.py
+-rw-r--r--   0        0        0     4267 2023-05-01 18:47:41.759788 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_command.py
+-rw-r--r--   0        0        0      218 2023-04-29 11:00:13.822441 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_command_utils.py
+-rw-r--r--   0        0        0      907 2023-04-29 11:00:13.822846 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_install_command.py
+-rw-r--r--   0        0        0      840 2023-04-29 11:00:13.823132 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_lock_command.py
+-rw-r--r--   0        0        0      864 2023-04-29 11:00:13.823612 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_publish_command.py
+-rw-r--r--   0        0        0     1167 2023-04-29 11:00:13.823871 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_remove_command.py
+-rw-r--r--   0        0        0      903 2023-04-29 11:00:13.824363 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_run_command.py
+-rw-r--r--   0        0        0      897 2023-04-29 11:00:13.824612 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_update_command.py
+-rw-r--r--   0        0        0      905 2023-04-29 11:00:13.824969 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/dependency_order_command.py
+-rw-r--r--   0        0        0     1271 2023-04-29 11:00:13.825347 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/package_filter.py
+-rw-r--r--   0        0        0      515 2023-04-29 11:00:13.825956 poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/sub_command_runner.py
+-rw-r--r--   0        0        0        0 2023-04-29 11:00:13.826113 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/__init__.py
+-rw-r--r--   0        0        0     1087 2023-04-29 11:00:13.827657 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/build_dependency_graph.py
+-rw-r--r--   0        0        0      455 2023-05-01 18:47:41.760022 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/build_natural_order.py
+-rw-r--r--   0        0        0     1015 2023-04-29 11:00:13.828651 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/discover_packages.py
+-rw-r--r--   0        0        0      821 2023-04-29 11:00:13.833010 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/get_package_dependencies.py
+-rw-r--r--   0        0        0      436 2023-04-29 11:00:13.834611 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/get_package_descriptor.py
+-rw-r--r--   0        0        0      124 2023-04-29 11:00:13.835880 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/sub_package_contains.py
+-rw-r--r--   0        0        0      318 2023-04-29 11:00:13.836803 poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/sub_package_has_dependency.py
+-rw-r--r--   0        0        0      947 2023-04-10 19:09:13.625373 poetry_plugin_compose-0.1.2/poetry_plugin_compose/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-29 11:00:13.836957 poetry_plugin_compose-0.1.2/poetry_plugin_compose/toposort/__init__.py
+-rw-r--r--   0        0        0     3567 2023-04-29 11:00:13.838018 poetry_plugin_compose-0.1.2/poetry_plugin_compose/toposort/graph.py
+-rw-r--r--   0        0        0      698 2023-05-01 18:49:18.272208 poetry_plugin_compose-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 poetry_plugin_compose-0.1.2/PKG-INFO
```

### Comparing `poetry_plugin_compose-0.1.1/README.md` & `poetry_plugin_compose-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/compose_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/compose_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_command_list.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_command_list.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_add_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_add_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_build_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_build_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_check_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_check_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 )
 from poetry_plugin_compose.packages.build_dependency_graph import build_dependency_graph
 from poetry_plugin_compose.composed_commands.package_filter import (
     PackageContainsFileFilter,
     PackageHasDependencyFilter,
     PackageIsDirectory,
 )
+from poetry_plugin_compose.packages.build_natural_order import build_natural_order
+from poetry_plugin_compose.toposort.graph import CircularGraphException
 
 
 class ComposedCommand:
     name: str
     io: IO
     parser: argparse.ArgumentParser
     description: str
@@ -36,15 +38,22 @@
     def split_args(self, args: List[str]):
         return split_compose_command_and_sub_command(args)
 
     def handle(self, args: List[str]):
         root_command, sub_command = self.split_args(args)
         options = self.parser.parse_args(root_command[1:])
         filters = self._get_package_filters(options)
-        package_order, package_map = build_dependency_graph()
+        try:
+            package_order, package_map = build_dependency_graph()
+        except CircularGraphException as e:
+            self._write_warning(
+                "Circular dependencies detected, falling back to natural ordering: "
+                + str(e)
+            )
+            package_order, package_map = build_natural_order()
         return_code = 0
         for package_name in package_order:
             package_dir = package_map[package_name].dir
             if self.filter_package(package_dir, filters):
                 return_code += self.run(sub_command, package_dir)
         return return_code
 
@@ -78,14 +87,19 @@
         self.io.write_line("<comment>" + self.get_log_intro() + " success</comment>")
 
     def _write_error(self, error):
         self.io.write_line(
             "<error>" + self.get_log_intro() + error + " failure</error>"
         )
 
+    def _write_warning(self, warning):
+        self.io.write_line(
+            "<warning>" + self.get_log_intro() + warning + " failure</warning>"
+        )
+
     def _write_failure(self):
         self._write_error("failure")
 
     def _get_package_filters(self, options):
         filters = []
         if options.contains:
             filters.append(PackageContainsFileFilter(options.contains))
```

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_install_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_install_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_lock_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_lock_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_publish_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_publish_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_remove_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_remove_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_run_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_run_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_update_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/composed_update_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/dependency_order_command.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/dependency_order_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/package_filter.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/package_filter.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/sub_command_runner.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/composed_commands/sub_command_runner.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/build_dependency_graph.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/build_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/discover_packages.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/discover_packages.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/get_package_dependencies.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/packages/get_package_dependencies.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/plugin.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/poetry_plugin_compose/toposort/graph.py` & `poetry_plugin_compose-0.1.2/poetry_plugin_compose/toposort/graph.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.1/pyproject.toml` & `poetry_plugin_compose-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-compose"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Max <maximilienlarue@gmail.com>"]
 readme = "README.md"
 packages = [{include = "poetry_plugin_compose"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `poetry_plugin_compose-0.1.1/PKG-INFO` & `poetry_plugin_compose-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-compose
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Max
 Author-email: maximilienlarue@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

