# Comparing `tmp/mkdocs-placeholder-plugin-0.3.0.tar.gz` & `tmp/mkdocs-placeholder-plugin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-placeholder-plugin-0.3.0.tar", last modified: Fri Apr  7 11:56:56 2023, max compression
+gzip compressed data, was "mkdocs-placeholder-plugin-0.3.1.tar", last modified: Mon May  1 19:01:17 2023, max compression
```

## Comparing `mkdocs-placeholder-plugin-0.3.0.tar` & `mkdocs-placeholder-plugin-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-07 11:56:56.600991 mkdocs-placeholder-plugin-0.3.0/
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.3.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       65 2023-03-27 05:22:55.000000 mkdocs-placeholder-plugin-0.3.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     7156 2023-04-07 11:56:56.601042 mkdocs-placeholder-plugin-0.3.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     6518 2023-04-07 11:55:42.000000 mkdocs-placeholder-plugin-0.3.0/README.md
--rw-r--r--   0 user       (501) staff       (20)       85 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.3.0/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)      943 2023-04-07 11:56:56.601284 mkdocs-placeholder-plugin-0.3.0/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-07 11:56:56.596497 mkdocs-placeholder-plugin-0.3.0/src/
--rwxr-xr-x   0 user       (501) staff       (20)     1467 2022-12-31 08:17:05.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs-placeholder-replace-static.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-07 11:56:56.599514 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/
--rw-r--r--   0 user       (501) staff       (20)      626 2022-09-10 08:23:28.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-07 11:56:56.600844 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets/
--rw-r--r--   0 user       (501) staff       (20)      312 2023-03-27 05:34:32.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets/placeholder-data.js
--rw-------   0 user       (501) staff       (20)    21736 2023-04-07 11:52:41.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js
--rw-------   0 user       (501) staff       (20)    91944 2023-04-07 11:52:41.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
--rw-r--r--   0 user       (501) staff       (20)     5288 2023-04-02 08:07:34.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets.py
--rw-r--r--   0 user       (501) staff       (20)     3275 2023-03-05 14:38:09.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/auto_input_table.py
--rw-r--r--   0 user       (501) staff       (20)     1315 2023-03-04 18:17:05.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/html_tag_parser.py
--rw-r--r--   0 user       (501) staff       (20)     8119 2023-03-04 18:17:05.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/input_table.py
--rw-r--r--   0 user       (501) staff       (20)     4122 2023-03-04 18:17:05.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/input_tag_handler.py
--rw-r--r--   0 user       (501) staff       (20)    13905 2023-03-28 17:35:35.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/placeholder_data.py
--rw-r--r--   0 user       (501) staff       (20)     5699 2023-03-31 17:41:46.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/plugin.py
--rw-r--r--   0 user       (501) staff       (20)     2239 2023-03-31 17:42:43.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/plugin_config.py
--rw-r--r--   0 user       (501) staff       (20)     5202 2023-03-04 18:17:05.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/static_replacer.py
--rw-r--r--   0 user       (501) staff       (20)     2196 2023-04-01 12:57:06.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/style.py
--rw-r--r--   0 user       (501) staff       (20)     5043 2023-03-28 17:34:25.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/validators.py
--rw-r--r--   0 user       (501) staff       (20)     8885 2023-03-28 17:25:38.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/validators_predefined.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-04-07 11:56:56.600334 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     7156 2023-04-07 11:56:56.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1189 2023-04-07 11:56:56.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-04-07 11:56:56.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       75 2023-04-07 11:56:56.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2023-04-07 11:56:56.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       26 2023-04-07 11:56:56.000000 mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.277819 mkdocs-placeholder-plugin-0.3.1/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.3.1/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       65 2023-03-27 05:22:55.000000 mkdocs-placeholder-plugin-0.3.1/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     7362 2023-05-01 19:01:17.277870 mkdocs-placeholder-plugin-0.3.1/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     6724 2023-05-01 19:00:26.000000 mkdocs-placeholder-plugin-0.3.1/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.3.1/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)      943 2023-05-01 19:01:17.278105 mkdocs-placeholder-plugin-0.3.1/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.273761 mkdocs-placeholder-plugin-0.3.1/src/
+-rwxr-xr-x   0 user       (501) staff       (20)     1467 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs-placeholder-replace-static.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.275727 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/
+-rw-r--r--   0 user       (501) staff       (20)      626 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.277294 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/
+-rw-r--r--   0 user       (501) staff       (20)      312 2023-03-27 05:34:32.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder-data.js
+-rw-------   0 user       (501) staff       (20)    21736 2023-05-01 19:00:55.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js
+-rw-------   0 user       (501) staff       (20)    91944 2023-05-01 19:00:55.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
+-rw-r--r--   0 user       (501) staff       (20)     5288 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets.py
+-rw-r--r--   0 user       (501) staff       (20)     3275 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/auto_input_table.py
+-rw-r--r--   0 user       (501) staff       (20)     1315 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/html_tag_parser.py
+-rw-r--r--   0 user       (501) staff       (20)     7847 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_table.py
+-rw-r--r--   0 user       (501) staff       (20)     4122 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_tag_handler.py
+-rw-r--r--   0 user       (501) staff       (20)    13905 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/placeholder_data.py
+-rw-r--r--   0 user       (501) staff       (20)     6016 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)     2239 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin_config.py
+-rw-r--r--   0 user       (501) staff       (20)     5202 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/static_replacer.py
+-rw-r--r--   0 user       (501) staff       (20)     2196 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/style.py
+-rw-r--r--   0 user       (501) staff       (20)     5043 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators.py
+-rw-r--r--   0 user       (501) staff       (20)     8885 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators_predefined.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.276613 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     7362 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1189 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       75 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       26 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/top_level.txt
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/LICENSE` & `mkdocs-placeholder-plugin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/PKG-INFO` & `mkdocs-placeholder-plugin-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-placeholder-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Add dynamic placeholders to your mkdocs page
 Home-page: https://github.com/six-two/mkdocs-placeholder-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -46,14 +46,18 @@
 
 - Rewrite python code and decouple it from MkDocs (to be able to use it with other projects).
 - Implement propper exception handling for TypeScript code to recover from / compartmentalize non-critical errors.
 - Update the documentation.
 
 ### HEAD
 
+### Version 0.3.1
+
+- Removed `Apply all changes` buttons. See [issue #3](https://github.com/six-two/mkdocs-placeholder-plugin/issues/3)
+
 ### Version 0.3.0
 
 This release may be a bit buggy due to the rewrite and the documentation is not entirely accurate yet.
 I will update the docs after I also clean up / rewrite the python code (planed for v0.4.0).
 
 - Rewrote the JavaScript code in TypeScript:
     - Packed and minified using Webpack, so the file is a bit smaller
@@ -142,12 +146,16 @@
     ```
     pyflakes src
     ```
 2. Update the changelog in this README file.
 3. Update version number in `setup.cfg`.
 4. Build and update package.
 5. Create a commit for the release (`Version 0.X.Y`) and push it.
-6. Update the `latest-release` branch, so that the documentation website gets updated:
+6. Add a tag named `0.X.Y`:
+    ```
+    git tag 0.X.Y
+    ```
+7. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
-    git push origin latest-release
+    git push --tags origin latest-release
     ```
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/README.md` & `mkdocs-placeholder-plugin-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
 - Rewrite python code and decouple it from MkDocs (to be able to use it with other projects).
 - Implement propper exception handling for TypeScript code to recover from / compartmentalize non-critical errors.
 - Update the documentation.
 
 ### HEAD
 
+### Version 0.3.1
+
+- Removed `Apply all changes` buttons. See [issue #3](https://github.com/six-two/mkdocs-placeholder-plugin/issues/3)
+
 ### Version 0.3.0
 
 This release may be a bit buggy due to the rewrite and the documentation is not entirely accurate yet.
 I will update the docs after I also clean up / rewrite the python code (planed for v0.4.0).
 
 - Rewrote the JavaScript code in TypeScript:
     - Packed and minified using Webpack, so the file is a bit smaller
@@ -124,12 +128,16 @@
     ```
     pyflakes src
     ```
 2. Update the changelog in this README file.
 3. Update version number in `setup.cfg`.
 4. Build and update package.
 5. Create a commit for the release (`Version 0.X.Y`) and push it.
-6. Update the `latest-release` branch, so that the documentation website gets updated:
+6. Add a tag named `0.X.Y`:
+    ```
+    git tag 0.X.Y
+    ```
+7. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
-    git push origin latest-release
+    git push --tags origin latest-release
     ```
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/setup.cfg` & `mkdocs-placeholder-plugin-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-placeholder-plugin
-version = 0.3.0
+version = 0.3.1
 author = six-two
 author_email = pip@six-two.dev
 description = Add dynamic placeholders to your mkdocs page
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/mkdocs-placeholder-plugin
 license = MIT License
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs-placeholder-replace-static.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs-placeholder-replace-static.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/__init__.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/assets.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/auto_input_table.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/auto_input_table.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/html_tag_parser.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/html_tag_parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/input_table.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .placeholder_data import Placeholder
 from .html_tag_parser import parse_html_tag
 
 
 INPUT_TABLE_PLACEHOLDER = re.compile("<placeholdertable[^>]*>")
 # "md-button md-button--primary" make it look pretty if you are using Material for Mkdocs (https://squidfunk.github.io/mkdocs-material/reference/buttons/#adding-icon-buttons)
 # Otherwise it will be styled in the default button way, with the option to use "placeholder-input-apply-button" to give it a custom style
-RELAOD_BUTTON = '<button class="placeholder-input-apply-button md-button md-button--primary" onclick="PlaceholderPlugin.reload_page()">Apply new values</button>'
+# RELAOD_BUTTON = '<button class="placeholder-input-apply-button md-button md-button--primary" onclick="PlaceholderPlugin.reload_page()">Apply new values</button>'
 
 class PlaceholderTableSettings(NamedTuple):
     table_type: str
     # ["auto"], ["all"], or a list of explicit placeholder names
     entries: list[str]
     show_readonly: bool
 
@@ -146,21 +146,14 @@
             # Table body
             for index, placeholder in enumerate(placeholder_entries):
                 cell = self.create_table_cell(column, placeholder)
                 # escape potentially dangerous characters that could mess up the table syntax
                 cell = cell.replace("|", "&#124;").replace("\r", " ").replace("\n", " ")
                 rows[index+2].append(cell)
 
-        if self.add_apply_table_column and "input" in column_list:
-            apply_row = []
-            for column in column_list:
-                cell = RELAOD_BUTTON if column == "input" else ""
-                apply_row.append(cell)
-            rows.append(apply_row)
-
         lines = [" | ".join(cells) for cells in rows]
         return "\n".join([*lines, "", ""])
 
     def create_table_cell(self, column: str, placeholder: Placeholder) -> str:
         if column == "name":
             return html.escape(placeholder.name)
         elif column == "description":
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/input_tag_handler.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_tag_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/placeholder_data.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/placeholder_data.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/plugin.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .plugin_config import PlaceholderPluginConfig
 from .placeholder_data import load_placeholder_data
 from .assets import copy_assets_to_mkdocs_site_directory
 from .static_replacer import StaticReplacer
 from .input_tag_handler import create_normal_input_class_handler
 from .auto_input_table import AutoTableInserter
 from .input_table import InputTableGenerator
-from . import set_warnings_enabled, debug
+from . import set_warnings_enabled, debug, warning
 
 
 def convert_exceptions(function: Callable) -> Callable:
     @wraps(function)
     def wrap(*args, **kwargs):
         try:
             return function(*args, **kwargs)
@@ -78,14 +78,17 @@
         """
         if self.config.enabled:
             self.after_build_action(config)
 
     def initialize_plugin(self, config: MkDocsConfig) -> None:
         set_warnings_enabled(self.config.show_warnings)
 
+        if self.config.add_apply_table_column:
+            warning("The 'Apply new values' are broken/no longer useful and have thus been removed. You can set the add_apply_table_column to False to disable this warning. If you really want the button, downgrade to version 0.2.5 of the placeholder plugin.")
+
         # Make sure that the custom JS is included on every page
         if self.config.placeholder_js not in config.extra_javascript:
             config.extra_javascript.append(self.config.placeholder_js)
 
         # Make sure that the custom CSS is included on every page
         if self.config.placeholder_css:
             if self.config.placeholder_css not in config.extra_css:
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/plugin_config.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/static_replacer.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/static_replacer.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/style.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/style.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/validators.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin/validators_predefined.py` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators_predefined.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-placeholder-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Add dynamic placeholders to your mkdocs page
 Home-page: https://github.com/six-two/mkdocs-placeholder-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -46,14 +46,18 @@
 
 - Rewrite python code and decouple it from MkDocs (to be able to use it with other projects).
 - Implement propper exception handling for TypeScript code to recover from / compartmentalize non-critical errors.
 - Update the documentation.
 
 ### HEAD
 
+### Version 0.3.1
+
+- Removed `Apply all changes` buttons. See [issue #3](https://github.com/six-two/mkdocs-placeholder-plugin/issues/3)
+
 ### Version 0.3.0
 
 This release may be a bit buggy due to the rewrite and the documentation is not entirely accurate yet.
 I will update the docs after I also clean up / rewrite the python code (planed for v0.4.0).
 
 - Rewrote the JavaScript code in TypeScript:
     - Packed and minified using Webpack, so the file is a bit smaller
@@ -142,12 +146,16 @@
     ```
     pyflakes src
     ```
 2. Update the changelog in this README file.
 3. Update version number in `setup.cfg`.
 4. Build and update package.
 5. Create a commit for the release (`Version 0.X.Y`) and push it.
-6. Update the `latest-release` branch, so that the documentation website gets updated:
+6. Add a tag named `0.X.Y`:
+    ```
+    git tag 0.X.Y
+    ```
+7. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
-    git push origin latest-release
+    git push --tags origin latest-release
     ```
```

### Comparing `mkdocs-placeholder-plugin-0.3.0/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt` & `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

