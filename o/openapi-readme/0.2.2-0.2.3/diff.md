# Comparing `tmp/openapi_readme-0.2.2.tar.gz` & `tmp/openapi_readme-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_readme-0.2.2.tar", max compression
+gzip compressed data, was "openapi_readme-0.2.3.tar", max compression
```

## Comparing `openapi_readme-0.2.2.tar` & `openapi_readme-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1069 2022-10-21 14:13:36.329262 openapi_readme-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1965 2023-04-20 11:23:36.904701 openapi_readme-0.2.2/README.md
--rw-r--r--   0        0        0        0 2022-10-21 08:37:08.347794 openapi_readme-0.2.2/openapi_readme/__init__.py
--rw-r--r--   0        0        0     4504 2023-04-20 11:51:18.263740 openapi_readme-0.2.2/openapi_readme/main.py
--rw-r--r--   0        0        0     1354 2023-04-20 11:51:18.263740 openapi_readme-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 openapi_readme-0.2.2/setup.py
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 openapi_readme-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-21 14:13:36.329262 openapi_readme-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1965 2023-04-20 11:23:36.904701 openapi_readme-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2022-10-21 08:37:08.347794 openapi_readme-0.2.3/openapi_readme/__init__.py
+-rw-r--r--   0        0        0     4535 2023-05-01 14:03:27.608275 openapi_readme-0.2.3/openapi_readme/main.py
+-rw-r--r--   0        0        0     1354 2023-05-01 14:03:07.880360 openapi_readme-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 openapi_readme-0.2.3/PKG-INFO
```

### Comparing `openapi_readme-0.2.2/LICENSE.txt` & `openapi_readme-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openapi_readme-0.2.2/README.md` & `openapi_readme-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openapi_readme-0.2.2/openapi_readme/main.py` & `openapi_readme-0.2.3/openapi_readme/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 from pathlib import Path
-from typing import Optional
 
 try:
     from importlib import metadata
 except ImportError:  # for Python<3.8
     import importlib_metadata as metadata
 
 import typer
@@ -13,15 +12,19 @@
 
 path_to_pyproject_dir = Path(__file__).parent.parent
 __version__ = get_version(__name__, path_to_pyproject_dir, default_return=None)
 
 if __version__ is None:
     __version__ = metadata.version("openapi-readme")
 
-app = typer.Typer(pretty_exceptions_show_locals=False)
+app = typer.Typer(
+    pretty_exceptions_show_locals=False,
+    add_completion=False,
+    no_args_is_help=True,
+)
 
 OPENAPI_FILENAME = "openapi.json"
 README_FILENAME = "README.md"
 
 
 def get_api_data(filename: str) -> dict:
     """Return a python dictionary containing the API data from schema file."""
```

### Comparing `openapi_readme-0.2.2/pyproject.toml` & `openapi_readme-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-readme"
-version = "0.2.2"
+version = "0.2.3"
 description = "Generate Markdown from an openapi JSON file."
 authors = ["Grant Ramsay <grant@gnramsay.com>"]
 readme = "README.md"
 packages = [{ include = "openapi_readme" }]
 license = "MIT"
 repository = "https://github.com/seapagan/openapi-readme"
 homepage = "https://github.com/seapagan/openapi-readme"
@@ -26,15 +26,15 @@
 "Bug Tracker" = "https://github.com/seapagan/openapi-readme/issues"
 
 [tool.poetry.scripts]
 openapi-readme = "openapi_readme.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<4.0"
-typer = { extras = ["all"], version = ">=0.6.1,<0.8.0" }
+typer = { extras = ["all"], version = ">=0.6.1,<0.9.0" }
 pydantic = "^1.10.2"
 single-source = "^0.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = ">=5.0.4,<7.0.0"
 black = ">=22.10,<24.0"
```

### Comparing `openapi_readme-0.2.2/PKG-INFO` & `openapi_readme-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-readme
-Version: 0.2.2
+Version: 0.2.3
 Summary: Generate Markdown from an openapi JSON file.
 Home-page: https://github.com/seapagan/openapi-readme
 License: MIT
 Author: Grant Ramsay
 Author-email: grant@gnramsay.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
-Requires-Dist: typer[all] (>=0.6.1,<0.8.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.9.0)
 Project-URL: Bug Tracker, https://github.com/seapagan/openapi-readme/issues
 Project-URL: Pull Requests, https://github.com/seapagan/openapi-readme/pulls
 Project-URL: Repository, https://github.com/seapagan/openapi-readme
 Description-Content-Type: text/markdown
 
 # OpenAPI Readme Generator  <!-- omit in toc -->
```

