# Comparing `tmp/bow_cli-1.0.0.3.tar.gz` & `tmp/bow_cli-1.0.0.4.tar.gz`

## Comparing `bow_cli-1.0.0.3.tar` & `bow_cli-1.0.0.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/CHANGELOG.md
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/tt.bat
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/py.typed
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/config.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/templates.json
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/commands/add.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/commands/g.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/commands/list.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/commands/remove.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/utils/fs.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/utils/http.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/src/bow/cli/utils/logger.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/templates/pycord/main.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/templates/pycordv3/main.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/templates/web/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/templates/web/assets/css/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/templates/web/assets/img/favicon.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/templates/web/assets/js/script.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/README.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bow_cli-1.0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/tt.bat
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/__about__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/__main__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/py.typed
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/templates.json
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/add.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/g.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/list.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/commands/remove.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/utils/fs.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/utils/http.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/src/bow/utils/logger.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/pycord/main.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/pycordv3/main.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/assets/css/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/assets/img/favicon.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/templates/web/assets/js/script.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/README.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bow_cli-1.0.0.4/PKG-INFO
```

### Comparing `bow_cli-1.0.0.3/src/bow/cli/templates.json` & `bow_cli-1.0.0.4/src/bow/templates.json`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.3/src/bow/cli/commands/add.py` & `bow_cli-1.0.0.4/src/bow/commands/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import click
 
-from bow.cli.config import tempfile
-from bow.cli.utils.http import check_url_validate
-from bow.cli.utils.logger import info, success
+from bow.config import tempfile
+from bow.utils.http import check_url_validate
+from bow.utils.logger import info, success
 
 
 @click.command()
 @click.argument("name")
 @click.argument("url")
 @click.option("-r", "--require", "req", help="Modules, libraries, SDKs that your template requires.", multiple=True)
 @click.option("-U", "--disable-url-checking", "duc", help="Disable URL validation checking.", is_flag=True, default=False, show_default=False)
```

### Comparing `bow_cli-1.0.0.3/src/bow/cli/commands/g.py` & `bow_cli-1.0.0.4/src/bow/commands/g.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 import click
 import git
 
-from bow.cli.config import templates
-from bow.cli.utils.fs import rmtree
-from bow.cli.utils.http import (check_url_validate, extract_repo_name,
+from bow.config import templates
+from bow.utils.fs import rmtree
+from bow.utils.http import (check_url_validate, extract_repo_name,
                             validate_git_repo)
-from bow.cli.utils.logger import error, info, success
+from bow.utils.logger import error, info, success
 
 
 @click.command()
 @click.argument("template")
 @click.option("-n", "--name", "name_", help="The name of the project, which will be specified in generated files (README and others).")
 @click.option("-d", "--dir", "dir_", help="Path where project will be generated in.")
 @click.option("-r", "--remove-git", help="Removes /.git directory.", default=False, show_default=False, is_flag=True)
```

### Comparing `bow_cli-1.0.0.3/src/bow/cli/commands/list.py` & `bow_cli-1.0.0.4/src/bow/commands/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 from rich.console import Console
 from rich.table import Table
 
-from bow.cli.config import templates
+from bow.config import templates
 
 
 @click.command()
 def list():
     """List of all available templates."""
     console = Console()
     table = Table(title="All available templates")
```

### Comparing `bow_cli-1.0.0.3/src/bow/cli/commands/remove.py` & `bow_cli-1.0.0.4/src/bow/commands/remove.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 import click
 
-from bow.cli.config import tempfile
-from bow.cli.utils.logger import info, success
+from bow.config import tempfile
+from bow.utils.logger import info, success
 
 
 @click.command()
 @click.argument("name")
 def remove(name):
     """Removes a template from templates file."""
     with open(tempfile, "r") as f:
```

### Comparing `bow_cli-1.0.0.3/src/bow/cli/utils/http.py` & `bow_cli-1.0.0.4/src/bow/utils/http.py`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.3/.gitignore` & `bow_cli-1.0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.3/pyproject.toml` & `bow_cli-1.0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bow_cli-1.0.0.3/PKG-INFO` & `bow_cli-1.0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bow-cli
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: Generate projects using built-in or custom templates via command-line.
 Project-URL: Homepage, https://github.com/woidzero/bow#readme
 Project-URL: Tracker, https://github.com/woidzero/bow/issues
 Project-URL: Source, https://github.com/woidzero/bow
 Author-email: woidzero <woidzeroo@gmail.com>
 License-Expression: MIT
 Keywords: bow,cli,utility
```

