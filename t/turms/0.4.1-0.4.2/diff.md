# Comparing `tmp/turms-0.4.1.tar.gz` & `tmp/turms-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turms-0.4.1.tar", max compression
+gzip compressed data, was "turms-0.4.2.tar", max compression
```

## Comparing `turms-0.4.1.tar` & `turms-0.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     4881 2023-03-18 12:48:25.735186 turms-0.4.1/README.md
--rw-r--r--   0        0        0     1645 2023-03-18 14:56:18.070160 turms-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744547 turms-0.4.1/turms/__init__.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744647 turms-0.4.1/turms/cli/__init__.py
--rw-r--r--   0        0        0     8574 2023-03-18 14:44:25.564848 turms-0.4.1/turms/cli/main.py
--rw-r--r--   0        0        0      549 2023-03-18 14:44:25.565090 turms-0.4.1/turms/cli/watch.py
--rw-r--r--   0        0        0    11698 2023-03-18 14:44:25.565234 turms-0.4.1/turms/config.py
--rw-r--r--   0        0        0      799 2023-03-18 12:48:25.744917 turms-0.4.1/turms/errors.py
--rw-r--r--   0        0        0     4520 2023-03-18 14:44:25.565351 turms-0.4.1/turms/helpers.py
--rw-r--r--   0        0        0      750 2023-03-18 12:48:25.745032 turms-0.4.1/turms/mocks.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745083 turms-0.4.1/turms/parsers/__init__.py
--rw-r--r--   0        0        0      525 2023-03-18 12:48:25.745145 turms-0.4.1/turms/parsers/base.py
--rw-r--r--   0        0        0     2102 2023-03-18 12:48:25.745211 turms-0.4.1/turms/parsers/polyfill.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745260 turms-0.4.1/turms/plugins/__init__.py
--rw-r--r--   0        0        0     1007 2023-03-18 14:44:25.565461 turms-0.4.1/turms/plugins/base.py
--rw-r--r--   0        0        0     3718 2023-03-18 14:44:25.565640 turms-0.4.1/turms/plugins/enums.py
--rw-r--r--   0        0        0    10361 2023-03-18 14:44:25.565767 turms-0.4.1/turms/plugins/fragments.py
--rw-r--r--   0        0        0    28213 2023-03-18 14:44:25.566020 turms-0.4.1/turms/plugins/funcs.py
--rw-r--r--   0        0        0     8477 2023-03-18 14:44:25.566166 turms-0.4.1/turms/plugins/inputs.py
--rw-r--r--   0        0        0    13761 2023-03-18 14:44:25.566303 turms-0.4.1/turms/plugins/objects.py
--rw-r--r--   0        0        0     9775 2023-03-18 14:44:25.566430 turms-0.4.1/turms/plugins/operations.py
--rw-r--r--   0        0        0    33581 2023-03-18 14:44:25.566568 turms-0.4.1/turms/plugins/strawberry.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746147 turms-0.4.1/turms/processors/__init__.py
--rw-r--r--   0        0        0      685 2023-03-18 12:48:25.746208 turms-0.4.1/turms/processors/base.py
--rw-r--r--   0        0        0      751 2023-03-18 12:48:25.746259 turms-0.4.1/turms/processors/black.py
--rw-r--r--   0        0        0      968 2023-03-18 12:48:25.746301 turms-0.4.1/turms/processors/disclaimer.py
--rw-r--r--   0        0        0      573 2023-03-18 12:48:25.746348 turms-0.4.1/turms/processors/isort.py
--rw-r--r--   0        0        0     8277 2023-03-18 14:44:25.566725 turms-0.4.1/turms/processors/merge.py
--rw-r--r--   0        0        0    20443 2023-03-18 14:44:25.566832 turms-0.4.1/turms/recurse.py
--rw-r--r--   0        0        0     6239 2023-03-18 14:44:25.567091 turms-0.4.1/turms/referencer.py
--rw-r--r--   0        0        0    16522 2023-03-18 14:44:25.567350 turms-0.4.1/turms/registry.py
--rw-r--r--   0        0        0    12975 2023-03-18 14:44:25.567666 turms-0.4.1/turms/run.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746858 turms-0.4.1/turms/stylers/__init__.py
--rw-r--r--   0        0        0     1112 2023-03-18 12:48:25.746926 turms-0.4.1/turms/stylers/appender.py
--rw-r--r--   0        0        0     2817 2023-03-18 12:48:25.746981 turms-0.4.1/turms/stylers/base.py
--rw-r--r--   0        0        0     1163 2023-03-18 12:48:25.747037 turms-0.4.1/turms/stylers/capitalize.py
--rw-r--r--   0        0        0     1438 2023-03-18 12:48:25.747085 turms-0.4.1/turms/stylers/default.py
--rw-r--r--   0        0        0      727 2023-03-18 12:48:25.747135 turms-0.4.1/turms/stylers/snake_case.py
--rw-r--r--   0        0        0    19484 2023-03-18 14:44:25.567814 turms-0.4.1/turms/utils.py
--rw-r--r--   0        0        0     6259 1970-01-01 00:00:00.000000 turms-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4881 2023-03-18 12:48:25.735186 turms-0.4.2/README.md
+-rw-r--r--   0        0        0     1645 2023-05-01 10:12:24.287494 turms-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744547 turms-0.4.2/turms/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744647 turms-0.4.2/turms/cli/__init__.py
+-rw-r--r--   0        0        0     8877 2023-05-01 10:12:04.859637 turms-0.4.2/turms/cli/main.py
+-rw-r--r--   0        0        0      549 2023-03-18 14:44:25.565090 turms-0.4.2/turms/cli/watch.py
+-rw-r--r--   0        0        0    11821 2023-05-01 10:12:04.859848 turms-0.4.2/turms/config.py
+-rw-r--r--   0        0        0      799 2023-03-18 12:48:25.744917 turms-0.4.2/turms/errors.py
+-rw-r--r--   0        0        0     4520 2023-03-18 14:44:25.565351 turms-0.4.2/turms/helpers.py
+-rw-r--r--   0        0        0      750 2023-03-18 12:48:25.745032 turms-0.4.2/turms/mocks.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745083 turms-0.4.2/turms/parsers/__init__.py
+-rw-r--r--   0        0        0      525 2023-03-18 12:48:25.745145 turms-0.4.2/turms/parsers/base.py
+-rw-r--r--   0        0        0     2102 2023-03-18 12:48:25.745211 turms-0.4.2/turms/parsers/polyfill.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745260 turms-0.4.2/turms/plugins/__init__.py
+-rw-r--r--   0        0        0     1007 2023-03-18 14:44:25.565461 turms-0.4.2/turms/plugins/base.py
+-rw-r--r--   0        0        0     3718 2023-03-18 14:44:25.565640 turms-0.4.2/turms/plugins/enums.py
+-rw-r--r--   0        0        0    10361 2023-03-18 14:44:25.565767 turms-0.4.2/turms/plugins/fragments.py
+-rw-r--r--   0        0        0    28213 2023-03-18 14:44:25.566020 turms-0.4.2/turms/plugins/funcs.py
+-rw-r--r--   0        0        0     8477 2023-03-18 14:44:25.566166 turms-0.4.2/turms/plugins/inputs.py
+-rw-r--r--   0        0        0    13761 2023-03-18 14:44:25.566303 turms-0.4.2/turms/plugins/objects.py
+-rw-r--r--   0        0        0     9775 2023-03-18 14:44:25.566430 turms-0.4.2/turms/plugins/operations.py
+-rw-r--r--   0        0        0    33581 2023-03-18 14:44:25.566568 turms-0.4.2/turms/plugins/strawberry.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746147 turms-0.4.2/turms/processors/__init__.py
+-rw-r--r--   0        0        0      685 2023-03-18 12:48:25.746208 turms-0.4.2/turms/processors/base.py
+-rw-r--r--   0        0        0      751 2023-03-18 12:48:25.746259 turms-0.4.2/turms/processors/black.py
+-rw-r--r--   0        0        0      968 2023-03-18 12:48:25.746301 turms-0.4.2/turms/processors/disclaimer.py
+-rw-r--r--   0        0        0      573 2023-03-18 12:48:25.746348 turms-0.4.2/turms/processors/isort.py
+-rw-r--r--   0        0        0     8277 2023-03-18 14:44:25.566725 turms-0.4.2/turms/processors/merge.py
+-rw-r--r--   0        0        0    20443 2023-03-18 14:44:25.566832 turms-0.4.2/turms/recurse.py
+-rw-r--r--   0        0        0     6239 2023-03-18 14:44:25.567091 turms-0.4.2/turms/referencer.py
+-rw-r--r--   0        0        0    16522 2023-03-18 14:44:25.567350 turms-0.4.2/turms/registry.py
+-rw-r--r--   0        0        0    12975 2023-03-18 14:44:25.567666 turms-0.4.2/turms/run.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746858 turms-0.4.2/turms/stylers/__init__.py
+-rw-r--r--   0        0        0     1112 2023-03-18 12:48:25.746926 turms-0.4.2/turms/stylers/appender.py
+-rw-r--r--   0        0        0     2817 2023-03-18 12:48:25.746981 turms-0.4.2/turms/stylers/base.py
+-rw-r--r--   0        0        0     1163 2023-03-18 12:48:25.747037 turms-0.4.2/turms/stylers/capitalize.py
+-rw-r--r--   0        0        0     1438 2023-03-18 12:48:25.747085 turms-0.4.2/turms/stylers/default.py
+-rw-r--r--   0        0        0      727 2023-03-18 12:48:25.747135 turms-0.4.2/turms/stylers/snake_case.py
+-rw-r--r--   0        0        0    19484 2023-03-18 14:44:25.567814 turms-0.4.2/turms/utils.py
+-rw-r--r--   0        0        0     6259 1970-01-01 00:00:00.000000 turms-0.4.2/PKG-INFO
```

### Comparing `turms-0.4.1/README.md` & `turms-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/pyproject.toml` & `turms-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turms"
-version = "0.4.1"
+version = "0.4.2"
 description = "graphql-codegen powered by pydantic"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 readme = "README.md"
 packages = [{ include = "turms" }]
 homepage = "https://jhnnsrs.github.io/turms"
 repository = "https://github.com/jhnnsrs/turms"
```

### Comparing `turms-0.4.1/turms/cli/main.py` & `turms-0.4.2/turms/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
     panel = Panel(
         panel_group,
         title=title,
         title_align="left",
         border_style="green",
         padding=(1, 1),
     )
+
+    raised_exceptions = []
+
     with Live(panel, screen=False) as live:
         for key, project in projects.items():
 
             project_tree = Tree(f"{key}", style="not bold white")
             tree.add(project_tree)
             live.update(panel)
 
@@ -99,16 +102,23 @@
                     project.extensions.turms.generated_name,
                 )
 
             except Exception as e:
                 project_tree.style = "red"
                 project_tree.label = f"{key} 💥"
                 project_tree.add(Tree(str(e), style="red"))
+                if project.extensions.turms.exit_on_error:
+                    raised_exceptions.append(e)
                 live.update(panel)
 
+    if raised_exceptions:
+        raise click.ClickException(
+            "One or more projects failed to generate. First error"
+        ) from raised_exceptions[0]
+
 
 def with_projects(func):
     @click.argument("project", default=None, required=False)
     @click.option("--config", default=None)
     @wraps(func)
     def wrapper(*args, config=None, project=None, **kwargs):
         try:
@@ -156,14 +166,15 @@
     panel = Panel(
         panel_group,
         title=title,
         title_align="left",
         border_style="green",
         padding=(1, 1),
     )
+
     with Live(panel, screen=False) as live:
 
         tree.renderable = f"Watching {project.documents}..."
         live.update(panel)
 
         for event in stream_changes(project.documents):
             live.update(panel)
```

### Comparing `turms-0.4.1/turms/cli/watch.py` & `turms-0.4.2/turms/cli/watch.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/config.py` & `turms-0.4.2/turms/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 import builtins
 from pydantic import AnyHttpUrl, BaseModel, BaseSettings, Field, validator
-from typing import Any, Dict, List, Optional, Union, Protocol, Literal, runtime_checkable
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Union,
+    Protocol,
+    Literal,
+    runtime_checkable,
+)
 from turms.helpers import import_string
 from enum import Enum
 
 
 class ConfigProxy(BaseModel):
     type: str
 
@@ -61,17 +70,17 @@
 class LogLevel(str, Enum):
     DEBUG = "DEBUG"
     INFO = "INFO"
     WARNING = "WARNING"
     ERROR = "ERROR"
     CRITICAL = "CRITICAL"
 
+
 @runtime_checkable
 class LogFunction(Protocol):
-
     def __call__(self, message, level: LogLevel = LogLevel.INFO):
         pass
 
 
 class FreezeConfig(BaseSettings):
     """Configuration for freezing the generated pydantic
     models
@@ -176,14 +185,17 @@
     generated_name: str = "schema.py"
     """ The name of the generated file within the output directory"""
     documents: Optional[str]
     """The documents to parse. Setting this will overwrite the documents in the graphql config"""
     verbose: bool = False
     """Enable verbose logging"""
 
+    exit_on_error: bool = True
+    """Will cause a sys.exit(1) if an error occurs"""
+
     allow_introspection: bool = True
     """Allow introspection queries"""
 
     object_bases: List[str] = ["pydantic.BaseModel"]
     """The base classes for the generated objects. This is useful if you want to change the base class from BaseModel to something else"""
 
     interface_bases: Optional[List[str]] = None
```

### Comparing `turms-0.4.1/turms/errors.py` & `turms-0.4.2/turms/errors.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/helpers.py` & `turms-0.4.2/turms/helpers.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/mocks.py` & `turms-0.4.2/turms/mocks.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/parsers/base.py` & `turms-0.4.2/turms/parsers/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/parsers/polyfill.py` & `turms-0.4.2/turms/parsers/polyfill.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/base.py` & `turms-0.4.2/turms/plugins/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/enums.py` & `turms-0.4.2/turms/plugins/enums.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/fragments.py` & `turms-0.4.2/turms/plugins/fragments.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/funcs.py` & `turms-0.4.2/turms/plugins/funcs.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/inputs.py` & `turms-0.4.2/turms/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/objects.py` & `turms-0.4.2/turms/plugins/objects.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/operations.py` & `turms-0.4.2/turms/plugins/operations.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/plugins/strawberry.py` & `turms-0.4.2/turms/plugins/strawberry.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/processors/base.py` & `turms-0.4.2/turms/processors/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/processors/black.py` & `turms-0.4.2/turms/processors/black.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/processors/disclaimer.py` & `turms-0.4.2/turms/processors/disclaimer.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/processors/isort.py` & `turms-0.4.2/turms/processors/isort.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/processors/merge.py` & `turms-0.4.2/turms/processors/merge.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/recurse.py` & `turms-0.4.2/turms/recurse.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/referencer.py` & `turms-0.4.2/turms/referencer.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/registry.py` & `turms-0.4.2/turms/registry.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/run.py` & `turms-0.4.2/turms/run.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/stylers/appender.py` & `turms-0.4.2/turms/stylers/appender.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/stylers/base.py` & `turms-0.4.2/turms/stylers/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/stylers/capitalize.py` & `turms-0.4.2/turms/stylers/capitalize.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/stylers/default.py` & `turms-0.4.2/turms/stylers/default.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/stylers/snake_case.py` & `turms-0.4.2/turms/stylers/snake_case.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/turms/utils.py` & `turms-0.4.2/turms/utils.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.1/PKG-INFO` & `turms-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turms
-Version: 0.4.1
+Version: 0.4.2
 Summary: graphql-codegen powered by pydantic
 Home-page: https://jhnnsrs.github.io/turms
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 6 - Mature
```

