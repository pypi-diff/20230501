# Comparing `tmp/deche-0.6.0.tar.gz` & `tmp/deche-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deche-0.6.0.tar", max compression
+gzip compressed data, was "deche-0.7.0.tar", max compression
```

## Comparing `deche-0.6.0.tar` & `deche-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      172 2022-01-16 00:35:30.182964 deche-0.6.0/deche/__init__.py
--rw-r--r--   0        0        0    14561 2022-02-24 04:10:31.693869 deche-0.6.0/deche/core.py
--rw-r--r--   0        0        0      609 2022-02-24 04:10:31.694169 deche-0.6.0/deche/inspection.py
--rw-r--r--   0        0        0     1154 2022-02-24 02:27:45.440238 deche-0.6.0/deche/test_utils/__init__.py
--rw-r--r--   0        0        0     2232 2022-02-24 04:10:31.694435 deche-0.6.0/deche/util.py
--rw-r--r--   0        0        0      660 2022-01-16 00:35:24.724452 deche-0.6.0/deche/validators.py
--rw-r--r--   0        0        0      718 2022-02-24 04:10:55.766533 deche-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      742 2022-02-24 04:10:59.493018 deche-0.6.0/setup.py
--rw-r--r--   0        0        0      535 2022-02-24 04:10:59.493232 deche-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2023-05-01 03:34:25.365554 deche-0.7.0/deche/__init__.py
+-rw-r--r--   0        0        0    15628 2023-05-01 03:34:25.365747 deche-0.7.0/deche/core.py
+-rw-r--r--   0        0        0      609 2023-05-01 03:34:20.574161 deche-0.7.0/deche/inspection.py
+-rw-r--r--   0        0        0     1154 2023-05-01 03:34:20.574359 deche-0.7.0/deche/test_utils/__init__.py
+-rw-r--r--   0        0        0     2277 2023-05-01 03:34:25.365890 deche-0.7.0/deche/util.py
+-rw-r--r--   0        0        0      660 2023-05-01 03:34:20.575068 deche-0.7.0/deche/validators.py
+-rw-r--r--   0        0        0      636 2023-05-01 03:34:25.368210 deche-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 deche-0.7.0/PKG-INFO
```

### Comparing `deche-0.6.0/deche/core.py` & `deche-0.7.0/deche/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import datetime
 import functools
 import hashlib
 import inspect
 import logging
 import pathlib
 import pickle
+from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum
 from functools import partial
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Any, Optional, Union
 
 import cloudpickle
 from fsspec import filesystem
 
 from deche import config
 from deche.inspection import args_kwargs_to_kwargs
+from deche.util import ValidationError
 from deche.util import ensure_path
 from deche.util import frozendict
 from deche.util import identity
 from deche.util import is_class_instance
 from deche.util import is_input_filename
 from deche.util import not_cache_append_file
 from deche.util import wrapped_partial
@@ -28,30 +30,30 @@
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_SERIALIZER = partial(cloudpickle.dumps, protocol=pickle.DEFAULT_PROTOCOL)
 DEFAULT_DESERIALIZER = partial(cloudpickle.loads)
 
 
-def tokenize(obj: object, serializer: Callable = DEFAULT_SERIALIZER) -> Tuple[str, bytes]:
+def tokenize(obj: object, serializer: Callable = DEFAULT_SERIALIZER) -> tuple[str, bytes]:
     value = serializer(obj)
     key = hashlib.sha256(value).hexdigest()
     return key, value
 
 
 def tokenize_func(func, ignore=None, cls_attrs=None):
     def inner(*args, **kwargs):
         full_kwargs = args_kwargs_to_kwargs(func=func, args=args, kwargs=kwargs)
         key, value = tokenize(obj=prepare_full_kwargs(all_kwargs=full_kwargs, ignore=ignore, cls_attrs=cls_attrs))
         return key
 
     return inner
 
 
-def prepare_full_kwargs(all_kwargs: Dict, ignore=None, cls_attrs=None):
+def prepare_full_kwargs(all_kwargs: dict, ignore=None, cls_attrs=None):
     all_kwargs = {k: v for k, v in all_kwargs.items() if k not in (ignore or ())}
     if is_class_instance(all_kwargs):
         # Remove self, add any cls_attrs
         self = all_kwargs.pop("self")
         all_kwargs.update({k: getattr(self, k) for k in (cls_attrs or {})})
     return frozendict(all_kwargs)
 
@@ -84,17 +86,19 @@
     prefix: Optional[str] = None
     input_serializer: Callable = DEFAULT_SERIALIZER
     input_deserializer: Callable = DEFAULT_DESERIALIZER
     output_serializer: Callable = DEFAULT_SERIALIZER
     output_deserializer: Callable = DEFAULT_DESERIALIZER
     cache_ttl: Optional[Union[datetime.timedelta, datetime.datetime, int]] = None
     cache_expiry_mode: CacheExpiryMode = CacheExpiryMode.REMOVE
-    cache_validators: Tuple[Callable] = None
-    non_hashable_kwargs: Optional[Tuple[str]] = None
-    cls_attrs: Optional[Tuple[str]] = None
+    cache_validators: tuple[Callable] = None
+    non_hashable_kwargs: Optional[tuple[str]] = None
+    cls_attrs: Optional[tuple[str]] = None
+    path_callable: Optional[Callable[[Callable, dict], str]] = None
+    result_validator: Optional[Callable[[Any], None]] = None
 
     def __post_init__(self):
         self._fs = None
         if self.cache_validators is None:
             self.cache_validators = DEFAULT_VALIDATORS
         if isinstance(self.cache_ttl, datetime.timedelta):
             self.cache_ttl: float = self.cache_ttl.total_seconds()
@@ -130,17 +134,19 @@
             logger.debug(f"fs_protocol: {self.fs_protocol}")
             self.fs_storage_options = config.get("fs.storage_options", None)
             logger.debug(f"fs_storage_options: {self.fs_storage_options}")
             self.prefix = ensure_path(config.get("fs.prefix", None))
             logger.debug(f"prefix: {self.prefix}")
             self.__post_init__()
 
-    def _path(self, func):
+    def _path(self, func, kwargs: Optional[dict] = None):
         if not self._fs:
-            self.fs
+            self.fs  # noqa - ensure fs is loaded
+        if self.path_callable is not None:
+            return self.path_callable(func, kwargs)
         path = f"{func.__module__}.{func.__name__}"
         return f"{self.prefix}/{path}" if self.prefix is not None else path
 
     def valid(self, path):
         validator = None
         try:
             for validator in self.cache_validators:
@@ -275,55 +281,67 @@
         # TODO - very lazy async support. Refactor
         # TODO - fsspec also has async support - could make exists/load calls async
 
         if inspect.iscoroutinefunction(func):
 
             @functools.wraps(func)
             async def wrapper(*args, **kwargs):
-                path = self._path(func=func)
                 all_kwargs = args_kwargs_to_kwargs(func=func, args=args, kwargs=kwargs)
+                path = self._path(func=func, kwargs=all_kwargs)
                 inputs = prepare_full_kwargs(
                     all_kwargs=all_kwargs, ignore=self.non_hashable_kwargs, cls_attrs=self.cls_attrs
                 )
                 key, _ = tokenize(obj=inputs)
                 if self.valid(path=f"{path}/{key}"):
                     return self._load(func=func)(key=key)
                 elif self._exists(func=func, ext=Extensions.exception)(key=key):
                     raise self._load(func=func, ext=Extensions.exception)(key=key)
                 try:
                     self.write_input(path=f"{path}/{key}", inputs=inputs)
                     logger.debug(f"Calling {func}")
                     output = await func(*args, **kwargs)
+                    if self.result_validator is not None:
+                        logger.debug(f"Validating result with {self.result_validator}")
+                        try:
+                            self.result_validator(output)
+                        except Exception as e:
+                            raise ValidationError(e)
                     logger.debug(f"Function {func} ran successfully")
                     self.write_output(path=f"{path}/{key}", output=output)
                 except Exception as e:
                     logger.debug(f"Function {func} raised {e}")
                     self.write_output(path=f"{path}/{key}{Extensions.exception}", output=e)
                     raise e
 
                 return output
 
         else:
 
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
-                path = self._path(func=func)
                 all_kwargs = args_kwargs_to_kwargs(func=func, args=args, kwargs=kwargs)
+                path = self._path(func=func, kwargs=all_kwargs)
                 inputs = prepare_full_kwargs(
                     all_kwargs=all_kwargs, ignore=self.non_hashable_kwargs, cls_attrs=self.cls_attrs
                 )
                 key, _ = tokenize(obj=inputs)
                 if self.valid(path=f"{path}/{key}"):
                     return self._load(func=func)(key=key)
                 elif self._exists(func=func, ext=Extensions.exception)(key=key):
                     raise self._load(func=func, ext=Extensions.exception)(key=key)
                 try:
                     self.write_input(path=f"{path}/{key}", inputs=inputs)
                     logger.debug(f"Calling {func}")
                     output = func(*args, **kwargs)
+                    if self.result_validator is not None:
+                        logger.debug(f"Validating result with {self.result_validator}")
+                        try:
+                            assert self.result_validator(output) is not False
+                        except Exception as e:
+                            raise ValidationError(e)
                     logger.debug(f"Function {func} ran successfully")
                     self.write_output(path=f"{path}/{key}", output=output)
                 except Exception as e:
                     logger.debug(f"Function {func} raised {e}")
                     self.write_output(path=f"{path}/{key}{Extensions.exception}", output=e)
                     raise e
```

### Comparing `deche-0.6.0/deche/inspection.py` & `deche-0.7.0/deche/inspection.py`

 * *Files identical despite different names*

### Comparing `deche-0.6.0/deche/test_utils/__init__.py` & `deche-0.7.0/deche/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deche-0.6.0/deche/util.py` & `deche-0.7.0/deche/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,7 +94,11 @@
     if "self" in kwargs:
         try:
             kwargs["self"].__class__
             return True
         except AttributeError:
             pass
     return False
+
+
+class ValidationError(Exception):
+    pass
```

### Comparing `deche-0.6.0/deche/validators.py` & `deche-0.7.0/deche/validators.py`

 * *Files identical despite different names*

### Comparing `deche-0.6.0/pyproject.toml` & `deche-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 [tool.poetry]
 name = "deche"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 fsspec = ">=2021.10.1"
 donfig = "^0.7.0"
 cloudpickle = "^2.0.0"
 s3fs = {version = ">=2021.7.0", optional = true }
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.4"
-mypy = "^0.931"
-jupyter-book = "^0.12.0"
+pytest = "^7.3"
+pytest-asyncio = "^0.21"
+jupyter-book = "^0.15"
 ipykernel = "^6.4.2"
 poetry2setup = "^1.0.0"
-setuptools = "^58.0.4"
-pip = "^21.2.4"
-coverage = "^6.0.2"
-pandas = "^1.3.5"
-pyarrow = "^7.0.0" # required for test_custom_serializer
-pytest-asyncio = "^0.18.1"
+pandas = "^1.5"
+pyarrow = "^11.0.0" # required for test_custom_serializer
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 s3 = ["s3fs"]
```

### Comparing `deche-0.6.0/PKG-INFO` & `deche-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deche
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: s3
 Requires-Dist: cloudpickle (>=2.0.0,<3.0.0)
 Requires-Dist: donfig (>=0.7.0,<0.8.0)
 Requires-Dist: fsspec (>=2021.10.1)
-Requires-Dist: s3fs (>=2021.7.0); extra == "s3"
+Requires-Dist: s3fs (>=2021.7.0) ; extra == "s3"
```

