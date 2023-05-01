# Comparing `tmp/bow_cli-1.0.0.4.tar.gz` & `tmp/bow_cli-1.0.0.5.tar.gz`

## Comparing `bow_cli-1.0.0.4.tar` & `bow_cli-1.0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/CHANGELOG.md
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/tt.bat
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/__about__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/__main__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/py.typed
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/templates.json
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/add.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/g.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/list.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/remove.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/utils/fs.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/utils/http.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/utils/logger.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/pycord/main.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/pycordv3/main.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/assets/css/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/assets/img/favicon.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/assets/js/script.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/README.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/CHANGELOG.md
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/tt.bat
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/__about__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/__init__.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/__main__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/py.typed
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/templates.json
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/commands/add.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/commands/g.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/commands/list.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/commands/remove.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/utils/fs.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/utils/http.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/src/bow/utils/logger.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/templates/pycord/main.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/templates/pycordv3/main.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/templates/web/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/templates/web/assets/css/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/templates/web/assets/img/favicon.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/templates/web/assets/js/script.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/README.md
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bow_cli-1.0.0.5/PKG-INFO
```

### Comparing `bow_cli-1.0.0.4/src/bow/__init__.py` & `bow_cli-1.0.0.5/src/bow/__init__.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/src/bow/templates.json` & `bow_cli-1.0.0.5/src/bow/templates.json`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/src/bow/commands/add.py` & `bow_cli-1.0.0.5/src/bow/commands/add.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/src/bow/commands/g.py` & `bow_cli-1.0.0.5/src/bow/commands/g.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/src/bow/commands/list.py` & `bow_cli-1.0.0.5/src/bow/commands/list.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/src/bow/commands/remove.py` & `bow_cli-1.0.0.5/src/bow/commands/remove.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/src/bow/utils/http.py` & `bow_cli-1.0.0.5/src/bow/utils/http.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/.gitignore` & `bow_cli-1.0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.4/pyproject.toml` & `bow_cli-1.0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 [project.urls]
 Homepage = "https://github.com/woidzero/bow#readme"
 Tracker = "https://github.com/woidzero/bow/issues"
 Source = "https://github.com/woidzero/bow"
 
 [project.scripts]
-bow = "bow.cli:main"
+bow = "bow:main"
 
 [tool.hatch.version]
 path = "src/bow/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
```

### Comparing `bow_cli-1.0.0.4/PKG-INFO` & `bow_cli-1.0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bow-cli
-Version: 1.0.0.4
+Version: 1.0.0.5
 Summary: Generate projects using built-in or custom templates via command-line.
 Project-URL: Homepage, https://github.com/woidzero/bow#readme
 Project-URL: Tracker, https://github.com/woidzero/bow/issues
 Project-URL: Source, https://github.com/woidzero/bow
 Author-email: woidzero <woidzeroo@gmail.com>
 License-Expression: MIT
 Keywords: bow,cli,utility
```

