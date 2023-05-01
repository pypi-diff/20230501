# Comparing `tmp/bow_cli-1.0.0.tar.gz` & `tmp/bow_cli-1.0.0.1.tar.gz`

## Comparing `bow_cli-1.0.0.tar` & `bow_cli-1.0.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bow_cli-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/py.typed
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/config.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/templates.json
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/commands/add.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/commands/g.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/commands/list.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/commands/remove.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/utils/fs.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/utils/http.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bow_cli-1.0.0/src/bow/cli/utils/logger.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bow_cli-1.0.0/templates/pycord/main.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bow_cli-1.0.0/templates/pycordv3/main.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bow_cli-1.0.0/templates/web/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0/templates/web/assets/css/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0/templates/web/assets/img/favicon.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0/templates/web/assets/js/script.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bow_cli-1.0.0/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bow_cli-1.0.0/README.md
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 bow_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 bow_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/py.typed
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/config.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/templates.json
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/commands/add.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/commands/g.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/commands/list.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/commands/remove.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/utils/fs.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/utils/http.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/src/bow/cli/utils/logger.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/templates/pycord/main.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/templates/pycordv3/main.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/templates/web/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/templates/web/assets/css/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/templates/web/assets/img/favicon.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/templates/web/assets/js/script.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/README.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bow_cli-1.0.0.1/PKG-INFO
```

### Comparing `bow_cli-1.0.0/src/bow/cli/__init__.py` & `bow_cli-1.0.0.1/src/bow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/src/bow/cli/templates.json` & `bow_cli-1.0.0.1/src/bow/cli/templates.json`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/src/bow/cli/commands/add.py` & `bow_cli-1.0.0.1/src/bow/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/src/bow/cli/commands/g.py` & `bow_cli-1.0.0.1/src/bow/cli/commands/g.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/src/bow/cli/commands/list.py` & `bow_cli-1.0.0.1/src/bow/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/src/bow/cli/commands/remove.py` & `bow_cli-1.0.0.1/src/bow/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/src/bow/cli/utils/http.py` & `bow_cli-1.0.0.1/src/bow/cli/utils/http.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/.gitignore` & `bow_cli-1.0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0/pyproject.toml` & `bow_cli-1.0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling>=1.14.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bow-cli"
 description = 'Generate projects using built-in or custom templates via command-line.'
 readme = "README.md"
 requires-python = ">=3.7"
@@ -38,15 +38,15 @@
 
 [project.urls]
 Homepage = "https://github.com/woidzero/bow#readme"
 Tracker = "https://github.com/woidzero/bow/issues"
 Source = "https://github.com/woidzero/bow"
 
 [project.scripts]
-hatch = "bow.cli:main"
+bow = "bow.cli:main"
 
 [tool.hatch.version]
 path = "src/bow/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
```

### Comparing `bow_cli-1.0.0/PKG-INFO` & `bow_cli-1.0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bow-cli
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: Generate projects using built-in or custom templates via command-line.
 Project-URL: Homepage, https://github.com/woidzero/bow#readme
 Project-URL: Tracker, https://github.com/woidzero/bow/issues
 Project-URL: Source, https://github.com/woidzero/bow
 Author-email: woidzero <woidzeroo@gmail.com>
 License-Expression: MIT
 Keywords: bow,cli,utility
```

