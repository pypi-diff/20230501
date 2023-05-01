# Comparing `tmp/goatl-0.4.0.tar.gz` & `tmp/goatl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goatl-0.4.0.tar", max compression
+gzip compressed data, was "goatl-0.4.1.tar", max compression
```

## Comparing `goatl-0.4.0.tar` & `goatl-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.4.0/LICENSE
--rw-r--r--   0        0        0     3619 2023-05-01 14:34:39.857535 goatl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11845 2023-05-01 14:09:02.446004 goatl-0.4.0/README.md
--rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.4.0/src/goatl/__init__.py
--rw-r--r--   0        0        0    12402 2023-05-01 13:42:11.568237 goatl-0.4.0/src/goatl/core.py
--rw-r--r--   0        0        0    12353 1970-01-01 00:00:00.000000 goatl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-01 13:53:20.360927 goatl-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3611 2023-05-01 17:47:27.445311 goatl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1833 2023-05-01 17:09:23.873407 goatl-0.4.1/README.md
+-rw-r--r--   0        0        0      614 2023-04-30 22:21:56.019567 goatl-0.4.1/src/goatl/__init__.py
+-rw-r--r--   0        0        0    11739 2023-05-01 18:15:42.624341 goatl-0.4.1/src/goatl/core.py
+-rw-r--r--   0        0        0     1423 2023-05-01 18:21:49.215963 goatl-0.4.1/src/goatl/utils.py
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 goatl-0.4.1/PKG-INFO
```

### Comparing `goatl-0.4.0/LICENSE` & `goatl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goatl-0.4.0/pyproject.toml` & `goatl-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "goatl"
-version = "0.4.0"
+version = "0.4.1"
 description = "Greatest of all time logger"
 readme = "README.md"
 authors = ["goatl <EytanDn@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/EytanDn/goatl"
 homepage = "https://github.com/EytanDn/goatl"
 
@@ -30,29 +30,29 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
-black = {version = "^21.10b0", allow-prereleases = true}
+black = {version = "^23.3", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
-mypy = "^0.910"
+mypy = "^1.0"
 mypy-extensions = "^0.4.3"
-pre-commit = "^2.15.0"
+pre-commit = "^3.2.2"
 pydocstyle = "^6.1.1"
 pylint = "^2.11.1"
-pytest = "^6.2.5"
-pyupgrade = "^2.29.1"
-safety = "^1.10.3"
-coverage = "^6.1.2"
+pytest = "^7.3.1"
+pyupgrade = "^3.3.2"
+safety = "^2.3.5"
+coverage = "^7.2.5"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
 color = true
```

### Comparing `goatl-0.4.0/src/goatl/__init__.py` & `goatl-0.4.1/src/goatl/__init__.py`

 * *Files identical despite different names*

### Comparing `goatl-0.4.0/src/goatl/core.py` & `goatl-0.4.1/src/goatl/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import inspect
 import functools
 from dataclasses import dataclass, field
 from typing import Callable, Optional, Union, TypeVar
+from .utils import _wrap_and_bind, _transfer_class_meta
 
 import sys
 _logger = logging.getLogger()
 handler = logging.StreamHandler(stream=sys.stdout)
 handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
 _logger.addHandler(handler)
 _logger.setLevel(logging.DEBUG)
@@ -84,15 +85,16 @@
         return Log(message=message, level=level, logger=kwargs.get("logger", None))
     
 @dataclass
 class CallLogParams:
     kwargs: Optional[dict] = field(default_factory=dict)
 
     def __post_init__(self): # TODO: seperate between level, call_level, reutrn_level
-        # if call_message is present use it, else use message if present, else use default
+        # if call_message is present use it, 
+        # else use message if present, else use default
         # if call_level is present use it, else use level if present, else use default
 
         self.call_log = Log._from_kwargs(self.kwargs, 
                                           DEFAULT_CALL_MESSAGE, 
                                           DEFAULT_CALL_LEVEL,
                                           prefix="call") 
         self.return_log = Log._from_kwargs(self.kwargs, 
@@ -141,32 +143,23 @@
             
         return return_value
 
     setattr(wrapper, "__log_params__", params)
 
     return wrapper
 
-def _transfer_class_meta(wrapped: type, wrapper: type) -> type:
-    """transfer meta data from wrapped to wrapper"""
-    wrapper.__name__ = wrapped.__name__
-    wrapper.__module__ = wrapped.__module__
-    wrapper.__qualname__ = wrapped.__qualname__
-    wrapper.__doc__ = wrapped.__doc__
-    wrapper.__annotations__ = wrapped.__annotations__
-    
-    return wrapper
-
 def _wrap_class(wrapped: type, params: ClassLogParams) -> type:
     """wrap a class with a log"""
     
     class Wrapper(wrapped):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             
-            for name, value in inspect.getmembers(self): # TODO: what about static methods?
+            for name, value in inspect.getmembers(self): 
+                # TODO: what about static methods?
                 if name.startswith("__"):
                     continue
                 if name.startswith("_"):
                     if params.private_log:
                         _wrap_and_bind(value, _wrap_function, params.private_log)
                 elif isinstance(value, property):
                     if params.property_log:
@@ -176,27 +169,14 @@
                         _wrap_and_bind(value, _wrap_function, params.method_log)
                         
             if params.init_log:
                 params.init_log(className=wrapped.__name__, args=args, kwargs=kwargs)
     
     return _transfer_class_meta(wrapped, Wrapper)
 
-def _wrap_and_bind(func: Callable,
-                  wrapper: Callable,
-                  *args,
-                  **kwargs) -> Callable:
-    """Wraps a method and binds it to the instance"""
-    func = getattr(func.__self__, func.__name__)
-    instance = func.__self__
-    wrapped = wrapper(getattr(instance.__class__, func.__name__), *args, **kwargs)
-    bound_method = wrapped.__get__(instance, instance.__class__)
-    setattr(instance, wrapped.__name__, bound_method)
-
-    return getattr(instance, wrapped.__name__)
-
 def _wrap(wrapped: Wrappable = None, **kwargs) -> Wrappable:
     """wrap a callable with a log"""
     if inspect.isclass(wrapped):
         class_log_params = ClassLogParams(kwargs)
         return _wrap_class(wrapped, class_log_params)
     else: # TODO: maybe seperate between class kwargs and function kwargs
         call_log_params = CallLogParams(kwargs)
@@ -274,17 +254,18 @@
     ...     return x * 2
     >>> foo(21)
     42
     >>> # DEBUG:root:called foo with x=21
     >>> # INFO:root:foo returned 42
     
     ### Custom log message for class one class method:
+    >>> custom_message = "[%(asctime)s] %(levelname)s: %(return)s from %(funcName)s"
     >>> @log
     ... class Bar:
-    ...     @log.info(return_message="[%(asctime)s] %(levelname)s: %(return)s from %(funcName)s")
+    ...     @log.info(return_message=custom_message)
     ...     def bar(self):
     ...         return 42
     >>> Bar().bar()
     42
     >>> # [2021-01-01 00:00:00] INFO: 42 from Foo.bar
 
     see the documentation for more details
@@ -312,18 +293,21 @@
         def decorate(wrapped: Wrappable) -> Wrappable:
             return _wrap(wrapped, **log_kwargs, **kwargs)
         
         if magic is None:
             return decorate
         return decorate(magic)
     else:
+        if level is None: # TODO: maybe search for level in current score?
+            level = logging.INFO
+        
         Log(message=magic, level=level, logger=logger)(*args, **kwargs)
 
 info: Callable = functools.partial(log, level=logging.INFO)
-setattr(log, "info", info)
+log.info = info
 debug: Callable = functools.partial(log, level=logging.DEBUG)
 setattr(log, "debug", debug)
 warning: Callable = functools.partial(log, level=logging.WARNING)
 setattr(log, "warning", warning)  
 error: Callable = functools.partial(log, level=logging.ERROR)
 setattr(log, "error", error)
 critical: Callable = functools.partial(log, level=logging.CRITICAL)
@@ -333,8 +317,8 @@
     info: logging.INFO,
     debug: logging.DEBUG,
     warning: logging.WARNING,
     error: logging.ERROR,
     critical: logging.CRITICAL
 }
 
-setattr(log, "levels", levels)
+log.levels: dict[Callable, int] = levels
```

