# Comparing `tmp/redmage-0.0.1.tar.gz` & `tmp/redmage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.0.1.tar", max compression
+gzip compressed data, was "redmage-0.0.2.tar", max compression
```

## Comparing `redmage-0.0.1.tar` & `redmage-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.1/LICENSE
--rw-r--r--   0        0        0    14529 2023-04-29 20:46:36.265033 redmage-0.0.1/README.md
--rw-r--r--   0        0        0      624 2023-04-30 18:54:33.311489 redmage-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.1/redmage/__init__.py
--rw-r--r--   0        0        0     6079 2023-04-30 17:53:11.381924 redmage-0.0.1/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.1/redmage/convertors.py
--rw-r--r--   0        0        0     6966 2023-04-30 16:16:06.542830 redmage-0.0.1/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.1/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.1/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.1/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.1/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.1/redmage/triggers.py
--rw-r--r--   0        0        0      936 2023-04-04 02:55:52.571857 redmage-0.0.1/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.1/redmage/utils.py
--rw-r--r--   0        0        0    15230 1970-01-01 00:00:00.000000 redmage-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.0.2/LICENSE
+-rw-r--r--   0        0        0    14693 2023-04-30 22:37:22.299063 redmage-0.0.2/README.md
+-rw-r--r--   0        0        0      624 2023-04-30 22:38:41.524069 redmage-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-21 18:11:35.917318 redmage-0.0.2/redmage/__init__.py
+-rw-r--r--   0        0        0     6164 2023-04-30 22:25:43.512248 redmage-0.0.2/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.0.2/redmage/convertors.py
+-rw-r--r--   0        0        0     6979 2023-04-30 21:11:15.121820 redmage-0.0.2/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.0.2/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.0.2/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.0.2/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.0.2/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.0.2/redmage/triggers.py
+-rw-r--r--   0        0        0      936 2023-04-04 02:55:52.571857 redmage-0.0.2/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.0.2/redmage/utils.py
+-rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.0.2/PKG-INFO
```

### Comparing `redmage-0.0.1/LICENSE` & `redmage-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/README.md` & `redmage-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # redmage
 
+[![run-tests](https://github.com/redmage-labs/redmage/actions/workflows/main.yaml/badge.svg)](https://github.com/redmage-labs/redmage/actions/workflows/main.yaml)
+
 Redmage is component based library for building [htmx](https://htmx.org/) powered web applications.
 
 It is built on top of the [starlette](https://www.starlette.io/) web framework.
 
 ## Example
 
 Redmage is meant to reduce the complexity of designing htmx powered applications by abstracting the need to explicitly register routes and configure the hx-* attributes for each interaction on your app.
```

### Comparing `redmage-0.0.1/pyproject.toml` & `redmage-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.0.1"
+version = "0.0.2"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.0.1/redmage/components.py` & `redmage-0.0.2/redmage/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,17 @@
             return "-".join(parts[1:])
 
         uuid = get_uuid(instance) if instance else "{id:str}"
         path = f"/{cls.__name__}/{uuid}"
 
         if getattr(cls, "__annotations__", None):
             for field, field_type in cls.__annotations__.items():
-                convertor = starlette_convertors[field_type.__name__]
+                convertor = starlette_convertors[
+                    field_type if isinstance(field_type, str) else field_type.__name__
+                ]
                 value = (
                     convertor.to_string(getattr(instance, field, None))
                     if instance
                     else f"{{{field}:{field_type.__name__}}}"
                 )
                 path += f"/{field}/{value}"
         return path
```

### Comparing `redmage-0.0.1/redmage/convertors.py` & `redmage-0.0.2/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/redmage/core.py` & `redmage-0.0.2/redmage/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from inspect import Parameter, getmembers, isfunction, signature
 from types import FunctionType
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 from starlette.applications import Starlette
 from starlette.convertors import CONVERTOR_TYPES as starlette_convertors
 from starlette.datastructures import FormData, QueryParams
 from starlette.requests import Request
 from starlette.responses import HTMLResponse
 from starlette.routing import Route
@@ -100,15 +100,15 @@
         if key in params:
             type_name = params[key].annotation.__name__
             value = starlette_convertors[type_name].convert(value)
         return value
 
     def _split_params(
         self,
-        params: Dict[str, Any] | QueryParams,
+        params: Union[Dict[str, Any], QueryParams],
         method_name: str,
         method_fn: Callable,
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         comp_params = {}
         method_params = {}
 
         for k, v in params.items():
```

### Comparing `redmage-0.0.1/redmage/elements.py` & `redmage-0.0.2/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/redmage/targets.py` & `redmage-0.0.2/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/redmage/triggers.py` & `redmage-0.0.2/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/redmage/types.py` & `redmage-0.0.2/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/redmage/utils.py` & `redmage-0.0.2/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.0.1/PKG-INFO` & `redmage-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.0.1
+Version: 0.0.2
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,16 @@
 Requires-Dist: hype-html (>=1.1.3,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: starlette (>=0.26.1,<0.27.0)
 Description-Content-Type: text/markdown
 
 # redmage
 
+[![run-tests](https://github.com/redmage-labs/redmage/actions/workflows/main.yaml/badge.svg)](https://github.com/redmage-labs/redmage/actions/workflows/main.yaml)
+
 Redmage is component based library for building [htmx](https://htmx.org/) powered web applications.
 
 It is built on top of the [starlette](https://www.starlette.io/) web framework.
 
 ## Example
 
 Redmage is meant to reduce the complexity of designing htmx powered applications by abstracting the need to explicitly register routes and configure the hx-* attributes for each interaction on your app.
```

