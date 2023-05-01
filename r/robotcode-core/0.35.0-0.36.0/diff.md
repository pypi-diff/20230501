# Comparing `tmp/robotcode_core-0.35.0.tar.gz` & `tmp/robotcode_core-0.36.0.tar.gz`

## Comparing `robotcode_core-0.35.0.tar` & `robotcode_core-0.36.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/async_cache.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/async_itertools.py
--rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/dataclasses.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/event.py
--rw-r--r--   0        0        0    15842 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/logging.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/py.typed
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/types.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/uri.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/LICENSE.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/README.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/async_cache.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/async_itertools.py
+-rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0    15625 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/dataclasses.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/event.py
+-rw-r--r--   0        0        0    15842 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/logging.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/LICENSE.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/README.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.36.0/PKG-INFO
```

### Comparing `robotcode_core-0.35.0/src/robotcode/core/async_cache.py` & `robotcode_core-0.36.0/src/robotcode/core/async_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/async_itertools.py` & `robotcode_core-0.36.0/src/robotcode/core/async_itertools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/async_tools.py` & `robotcode_core-0.36.0/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/dataclasses.py` & `robotcode_core-0.36.0/src/robotcode/core/dataclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # pyright: reportMissingTypeArgument=true, reportMissingParameterType=true
-import copy
 import dataclasses
 import enum
-import functools
 import inspect
 import itertools
 import json
 import re
 from typing import (
     Any,
     Callable,
@@ -41,35 +39,50 @@
     "CamelSnakeMixin",
 ]
 
 _RE_SNAKE_CASE_1 = re.compile(r"[\-\.\s]")
 _RE_SNAKE_CASE_2 = re.compile(r"[A-Z]")
 
 
-@functools.lru_cache(1024)
+__not_valid = object()
+
+__to_snake_case_cache: Dict[str, str] = {}
+
+
 def to_snake_case(s: str) -> str:
-    s = _RE_SNAKE_CASE_1.sub("_", s)
-    if not s:
-        return s
-    return s[0].lower() + _RE_SNAKE_CASE_2.sub(lambda matched: "_" + matched.group(0).lower(), s[1:])
+    result = __to_snake_case_cache.get(s, __not_valid)
+    if result is __not_valid:
+        s = _RE_SNAKE_CASE_1.sub("_", s)
+        if not s:
+            result = s
+        else:
+            result = s[0].lower() + _RE_SNAKE_CASE_2.sub(lambda matched: "_" + matched.group(0).lower(), s[1:])
+        __to_snake_case_cache[s] = result
+    return cast(str, result)
 
 
 _RE_CAMEL_CASE_1 = re.compile(r"^[\-_\.]")
 _RE_CAMEL_CASE_2 = re.compile(r"[\-_\.\s]([a-z])")
 
+__to_snake_camel_cache: Dict[str, str] = {}
+
 
-@functools.lru_cache(1024)
 def to_camel_case(s: str) -> str:
-    s = _RE_CAMEL_CASE_1.sub("", str(s))
-    if not s:
-        return s
-    return str(s[0]).lower() + _RE_CAMEL_CASE_2.sub(
-        lambda matched: str(matched.group(1)).upper(),
-        s[1:],
-    )
+    result = __to_snake_camel_cache.get(s, __not_valid)
+    if result is __not_valid:
+        s = _RE_CAMEL_CASE_1.sub("", s)
+        if not s:
+            result = s
+        else:
+            result = str(s[0]).lower() + _RE_CAMEL_CASE_2.sub(
+                lambda matched: str(matched.group(1)).upper(),
+                s[1:],
+            )
+        __to_snake_camel_cache[s] = result
+    return cast(str, result)
 
 
 class CamelSnakeMixin:
     @classmethod
     def _encode_case(cls, s: str) -> str:
         return to_camel_case(s)
 
@@ -106,29 +119,21 @@
         return s
 
     @classmethod
     def _decode_case(cls, s: str) -> str:
         return s
 
 
-__default_config: Optional[DefaultConfig] = None
-
-
-def __get_default_config() -> DefaultConfig:
-    global __default_config
-
-    if __default_config is None:
-        __default_config = DefaultConfig()
-    return __default_config
+__default_config = DefaultConfig()
 
 
 def __get_config(obj: Any, entry_protocol: Type[_T]) -> _T:
     if isinstance(obj, entry_protocol):
         return obj
-    return cast(_T, __get_default_config())
+    return cast(_T, __default_config)
 
 
 def encode_case(obj: Any, field: dataclasses.Field) -> str:  # type: ignore
     alias = field.metadata.get("alias", None)
     if alias:
         return str(alias)
 
@@ -353,46 +358,55 @@
     *,
     strict: bool = False,
 ) -> _T:
     return from_dict(json.loads(s), types, strict=strict)
 
 
 def as_dict(
-    value: Any, *, remove_defaults: bool = False, dict_factory: Callable[[Any], Dict[str, Any]] = dict
+    value: Any,
+    *,
+    remove_defaults: bool = False,
+    dict_factory: Callable[[Any], Dict[str, Any]] = dict,
+    encode: bool = True,
 ) -> Dict[str, Any]:
     if not dataclasses.is_dataclass(value):
         raise TypeError("as_dict() should be called on dataclass instances")
 
-    return cast(Dict[str, Any], _as_dict_inner(value, remove_defaults, dict_factory))
+    return cast(Dict[str, Any], _as_dict_inner(value, remove_defaults, dict_factory, encode))
 
 
-def _as_dict_inner(value: Any, remove_defaults: bool, dict_factory: Callable[[Any], Dict[str, Any]]) -> Any:
+def _as_dict_inner(
+    value: Any,
+    remove_defaults: bool,
+    dict_factory: Callable[[Any], Dict[str, Any]],
+    encode: bool = True,
+) -> Any:
     if dataclasses.is_dataclass(value):
         result = []
         for f in dataclasses.fields(value):
             v = _as_dict_inner(getattr(value, f.name), remove_defaults, dict_factory)
 
             if remove_defaults and v == f.default:
                 continue
-            result.append((f.name, v))
+            result.append((encode_case(value, f) if encode else f.name, v))
         return dict_factory(result)
 
     if isinstance(value, tuple) and hasattr(value, "_fields"):
         return type(value)(*[_as_dict_inner(v, remove_defaults, dict_factory) for v in value])
 
     if isinstance(value, (list, tuple)):
         return type(value)(_as_dict_inner(v, remove_defaults, dict_factory) for v in value)
 
     if isinstance(value, dict):
         return type(value)(
             (_as_dict_inner(k, remove_defaults, dict_factory), _as_dict_inner(v, remove_defaults, dict_factory))
             for k, v in value.items()
         )
 
-    return copy.deepcopy(value)
+    return value
 
 
 class TypeValidationError(Exception):
     def __init__(self, *args: Any, target: Any, errors: Any) -> None:
         super().__init__(*args)
         self.class_ = target.__class__
         self.errors = errors
```

### Comparing `robotcode_core-0.35.0/src/robotcode/core/event.py` & `robotcode_core-0.36.0/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/logging.py` & `robotcode_core-0.36.0/src/robotcode/core/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/uri.py` & `robotcode_core-0.36.0/src/robotcode/core/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.36.0/src/robotcode/core/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.36.0/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.36.0/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/utils/net.py` & `robotcode_core-0.36.0/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.36.0/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/src/robotcode/core/utils/version.py` & `robotcode_core-0.36.0/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/.gitignore` & `robotcode_core-0.36.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/LICENSE.txt` & `robotcode_core-0.36.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/README.md` & `robotcode_core-0.36.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/pyproject.toml` & `robotcode_core-0.36.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.35.0/PKG-INFO` & `robotcode_core-0.36.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-core
-Version: 0.35.0
+Version: 0.36.0
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

