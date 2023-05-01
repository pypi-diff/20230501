# Comparing `tmp/fast_depends-1.1.2.tar.gz` & `tmp/fast_depends-1.1.3.tar.gz`

## Comparing `fast_depends-1.1.2.tar` & `fast_depends-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/__init__.py
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/construct.py
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/injector.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/model.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/provider.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/types.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/usage.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fast_depends-1.1.2/fast_depends/library/model.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.1.2/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.2/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.2/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.2/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.2/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.2/README.md
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 fast_depends-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/__init__.py
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/construct.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/injector.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/provider.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/types.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/usage.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.3/README.md
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.3/PKG-INFO
```

### Comparing `fast_depends-1.1.2/CONTRIBUTING.md` & `fast_depends-1.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.2/.github/workflows/documentation.yml` & `fast_depends-1.1.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.2/.github/workflows/publish_coverage.yml` & `fast_depends-1.1.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.2/.github/workflows/publish_pypi.yml` & `fast_depends-1.1.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.2/.github/workflows/tests.yml` & `fast_depends-1.1.3/.github/workflows/tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-          cache: "pip"
-          cache-dependency-path: pyproject.toml
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v03
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
@@ -55,16 +53,14 @@
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: '3.8'
-          cache: "pip"
-          cache-dependency-path: pyproject.toml
 
       - name: Get coverage files
         uses: actions/download-artifact@v3
         with:
           name: coverage
           path: coverage
 
@@ -79,15 +75,14 @@
         uses: actions/upload-artifact@v3
         with:
           name: coverage-html
           path: htmlcov
 
   # https://github.com/marketplace/actions/alls-green#why
   check:  # This job does nothing and is only used for the branch protection
-
     if: always()
 
     needs:
       - coverage-combine
 
     runs-on: ubuntu-latest
```

### Comparing `fast_depends-1.1.2/fast_depends/construct.py` & `fast_depends-1.1.3/fast_depends/construct.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from typing import Any, Optional, Tuple, Type, Union
+from typing import Any, ForwardRef, Optional, Tuple, Type, Union
 
 from pydantic import BaseConfig
 from pydantic.fields import (
     SHAPE_FROZENSET,
     SHAPE_LIST,
     SHAPE_SEQUENCE,
     SHAPE_SET,
@@ -12,21 +12,21 @@
     FieldInfo,
     ModelField,
     Required,
     Undefined,
     UndefinedType,
 )
 from pydantic.schema import get_annotation_from_field_info
-from pydantic.typing import ForwardRef, evaluate_forwardref, get_args, get_origin
+from pydantic.typing import evaluate_forwardref, get_args, get_origin
 from typing_extensions import Annotated
 
 from fast_depends import model
-from fast_depends.types import AnyCallable, AnyDict
 from fast_depends.library import CustomField
-
+from fast_depends.types import AnyCallable, AnyDict
+from fast_depends.utils import is_coroutine_callable
 
 sequence_shapes = {
     SHAPE_LIST,
     SHAPE_SET,
     SHAPE_FROZENSET,
     SHAPE_TUPLE,
     SHAPE_SEQUENCE,
@@ -46,14 +46,16 @@
         call=call,
         path=path,
         name=name,
         use_cache=use_cache,
         return_field=None,
     )
 
+    is_async = is_coroutine_callable(call)
+
     endpoint_signature = get_typed_signature(call)
     signature_params = endpoint_signature.parameters
 
     for param in signature_params.values():
         custom, depends, param_field = analyze_param(
             param_name=param.name,
             annotation=param.annotation,
@@ -64,14 +66,18 @@
             dependant.return_field = param_field
             continue
 
         elif custom is not None:
             dependant.custom.append(custom)
 
         elif depends is not None:
+            assert is_async or not is_coroutine_callable(
+                depends.dependency
+            ), f"You cannot use async dependency `{depends}` with sync `{dependant}`"
+
             sub_dependant = get_param_sub_dependant(
                 param_name=param.name,
                 depends=depends,
                 path=path,
             )
             dependant.dependencies.append(sub_dependant)
 
@@ -81,15 +87,15 @@
 
 
 def analyze_param(
     *,
     param_name: str,
     annotation: Any,
     default: Any,
-) -> Tuple[Optional[CustomField], Optional[model.Depends], Optional[ModelField]]:
+) -> Tuple[Optional[CustomField], Optional[model.Depends], ModelField]:
     depends = None
     custom = None
     field_info = None
 
     if (
         annotation is not inspect.Signature.empty
         and get_origin(annotation) is Annotated  # type: ignore[comparison-overlap]
```

### Comparing `fast_depends-1.1.2/fast_depends/injector.py` & `fast_depends-1.1.3/fast_depends/injector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,39 @@
 from contextlib import AsyncExitStack, ExitStack
 from copy import deepcopy
-from typing import (
-    Any,
-    Dict,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    TypeVar,
-    cast,
-)
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, TypeVar, cast
 
-from pydantic.error_wrappers import ErrorWrapper
+from pydantic.error_wrappers import ErrorList, ErrorWrapper
 from pydantic.errors import MissingError
 from pydantic.fields import ModelField
 
 from fast_depends.construct import get_dependant
 from fast_depends.model import Dependant
 from fast_depends.types import AnyCallable, AnyDict
 from fast_depends.utils import (
-    run_async,
+    is_async_gen_callable,
     is_coroutine_callable,
     is_gen_callable,
-    is_async_gen_callable,
+    run_async,
     solve_generator_async,
     solve_generator_sync,
 )
 
-
 T = TypeVar("T")
 
 
 async def solve_dependencies_async(
     *,
     dependant: Dependant,
     stack: AsyncExitStack,
     body: Optional[AnyDict] = None,
     dependency_overrides_provider: Optional[Any] = None,
     dependency_cache: Optional[Dict[Tuple[AnyCallable, Tuple[str]], Any]] = None,
-) -> Tuple[
-    Dict[str, Any],
-    List[ErrorWrapper],
-    Dict[Tuple[AnyCallable, Tuple[str]], Any],
-]:
-    errors: List[ErrorWrapper] = []
+) -> Tuple[Dict[str, Any], List[ErrorList], Dict[Tuple[AnyCallable, Tuple[str]], Any],]:
+    errors: List[ErrorList] = []
 
     dependency_cache = dependency_cache or {}
 
     sub_dependant: Dependant
     for sub_dependant in dependant.dependencies:
         sub_dependant.call = cast(AnyCallable, sub_dependant.call)
         sub_dependant.cache_key = cast(
@@ -65,15 +50,15 @@
             ).get(sub_dependant.call)
             if call is not None:  # pragma: no branch
                 use_sub_dependant = get_dependant(
                     path=sub_dependant.path,
                     call=call,
                     name=sub_dependant.name,
                 )
-
+        assert call
         solved_result = await solve_dependencies_async(
             dependant=use_sub_dependant,
             body=body,
             dependency_overrides_provider=dependency_overrides_provider,
             dependency_cache=dependency_cache,
             stack=stack,
         )
@@ -126,24 +111,20 @@
 def solve_dependencies_sync(
     *,
     dependant: Dependant,
     stack: ExitStack,
     body: Optional[AnyDict] = None,
     dependency_overrides_provider: Optional[Any] = None,
     dependency_cache: Optional[Dict[Tuple[AnyCallable, Tuple[str]], Any]] = None,
-) -> Tuple[
-    Dict[str, Any],
-    List[ErrorWrapper],
-    Dict[Tuple[AnyCallable, Tuple[str]], Any],
-]:
+) -> Tuple[Dict[str, Any], List[ErrorList], Dict[Tuple[AnyCallable, Tuple[str]], Any],]:
     assert not is_coroutine_callable(dependant.call) and not is_async_gen_callable(
         dependant.call
     ), f"You can't call async `{dependant.call.__name__}` at sync code"
 
-    errors: List[ErrorWrapper] = []
+    errors: List[ErrorList] = []
 
     dependency_cache = dependency_cache or {}
 
     sub_dependant: Dependant
     for sub_dependant in dependant.dependencies:
         sub_dependant.call = cast(AnyCallable, sub_dependant.call)
         sub_dependant.cache_key = cast(
@@ -160,15 +141,15 @@
             ).get(sub_dependant.call)
             if call is not None:  # pragma: no branch
                 use_sub_dependant = get_dependant(
                     path=sub_dependant.path,
                     call=call,
                     name=sub_dependant.name,
                 )
-
+        assert call
         solved_result = solve_dependencies_sync(
             dependant=use_sub_dependant,
             body=body,
             stack=stack,
             dependency_overrides_provider=dependency_overrides_provider,
             dependency_cache=dependency_cache,
         )
@@ -203,29 +184,30 @@
         if use_sub_dependant.name is not None:  # pragma: no branch
             body[sub_dependant.name] = solved
 
         if use_sub_dependant.cache_key not in dependency_cache:
             dependency_cache[use_sub_dependant.cache_key] = solved
 
     for custom in dependant.custom:
-        assert not is_coroutine_callable(custom.use) and not is_async_gen_callable(custom.use), \
-                f"You can't use async `{type(custom).__name__}` at sync code"
+        assert not is_coroutine_callable(custom.use) and not is_async_gen_callable(
+            custom.use
+        ), f"You can't use async `{type(custom).__name__}` at sync code"
         body = custom.use(**(body or {}))
 
     params, main_errors = params_to_args(dependant.params, body or {})
     errors.extend(main_errors)
     return params, errors, dependency_cache
 
 
 def params_to_args(
     required_params: Sequence[ModelField],
     received_params: Mapping[str, Any],
-) -> Tuple[AnyDict, List[ErrorWrapper]]:
+) -> Tuple[AnyDict, List[ErrorList]]:
     values: AnyDict = {}
-    errors: List[ErrorWrapper] = []
+    errors: List[ErrorList] = []
     for field in required_params:
         value = received_params.get(field.alias)
         if value is None:
             if field.required:
                 errors.append(ErrorWrapper(MissingError(), loc=(field.alias,)))
             else:
                 values[field.name] = deepcopy(field.default)
```

### Comparing `fast_depends-1.1.2/fast_depends/model.py` & `fast_depends-1.1.3/fast_depends/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from typing import Any, List, Optional, Tuple
 
 from pydantic import create_model
 from pydantic.error_wrappers import ErrorList
 from pydantic.fields import ModelField
 
-from fast_depends.types import AnyCallable
 from fast_depends.library import CustomField
-
+from fast_depends.types import AnyCallable
 
 RETURN_FIELD = "custom_return"
 
 
 class Dependant:
     def __init__(
         self,
         *,
-        call: Optional[AnyCallable] = None,
+        call: AnyCallable,
         params: Optional[List[ModelField]] = None,
         return_field: Optional[ModelField] = None,
         dependencies: Optional[List["Dependant"]] = None,
         custom: Optional[List[CustomField]] = None,
         use_cache: bool = True,
         path: Optional[str] = None,
         name: Optional[str] = None,
@@ -41,17 +40,15 @@
     def cast_response(self, response: Any) -> Tuple[Optional[Any], Optional[ErrorList]]:
         if self.return_field is None:
             return response, []
         return self.return_field.validate(response, {}, loc=RETURN_FIELD)
 
 
 class Depends:
-    def __init__(
-        self, dependency: Optional[AnyCallable] = None, *, use_cache: bool = True
-    ) -> None:
+    def __init__(self, dependency: AnyCallable, *, use_cache: bool = True) -> None:
         self.dependency = dependency
         self.use_cache = use_cache
 
     def __repr__(self) -> str:
         attr = getattr(self.dependency, "__name__", type(self.dependency).__name__)
         cache = "" if self.use_cache else ", use_cache=False"
         return f"{self.__class__.__name__}({attr}{cache})"
```

### Comparing `fast_depends-1.1.2/fast_depends/usage.py` & `fast_depends-1.1.3/fast_depends/usage.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,23 @@
 from functools import partial, wraps
 from typing import Any, Callable, Optional, TypeVar
 
 from pydantic import ValidationError
 
 from fast_depends import model
 from fast_depends.construct import get_dependant
-from fast_depends.injector import (
-    is_coroutine_callable,
-    run_async,
-    solve_dependencies_async,
-    solve_dependencies_sync,
-)
+from fast_depends.injector import solve_dependencies_async, solve_dependencies_sync
 from fast_depends.provider import dependency_provider
 from fast_depends.types import AnyCallable, P
-from fast_depends.utils import args_to_kwargs
+from fast_depends.utils import args_to_kwargs, is_coroutine_callable, run_async
 
 T = TypeVar("T")
 
 
-def Depends(  # noqa: N802
-    dependency: Optional[AnyCallable] = None, *, use_cache: bool = True
-) -> Any:
+def Depends(dependency: AnyCallable, *, use_cache: bool = True) -> Any:  # noqa: N802
     return model.Depends(dependency=dependency, use_cache=use_cache)
 
 
 def wrap_dependant(dependant: model.Dependant) -> model.Dependant:
     return dependant
 
 
@@ -68,19 +61,19 @@
             stack=stack,
             dependency_overrides_provider=dependency_overrides_provider,
         )
 
         if errors:
             raise ValidationError(errors, dependant.error_model)
 
-        v, errors = dependant.cast_response(
+        v, casted_errors = dependant.cast_response(
             await run_async(dependant.call, **solved_result)
         )
 
-        if errors:
+        if casted_errors:
             raise ValidationError(errors, dependant.error_model)
 
         return v
 
 
 def sync_typed_wrapper(
     *args: P.args,
@@ -97,13 +90,13 @@
             stack=stack,
             dependency_overrides_provider=dependency_overrides_provider,
         )
 
         if errors:
             raise ValidationError(errors, dependant.error_model)
 
-        v, errors = dependant.cast_response(dependant.call(**solved_result))
+        v, casted_errors = dependant.cast_response(dependant.call(**solved_result))
 
-        if errors:
+        if casted_errors:
             raise ValidationError(errors, dependant.error_model)
 
         return v
```

### Comparing `fast_depends-1.1.2/fast_depends/utils.py` & `fast_depends-1.1.3/fast_depends/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,89 +4,88 @@
 from contextlib import AsyncExitStack, ExitStack, asynccontextmanager, contextmanager
 from typing import (
     Any,
     AsyncGenerator,
     Callable,
     ContextManager,
     Dict,
-    Sequence,
+    Iterable,
     TypeVar,
+    cast,
 )
 
 import anyio
 
-from fast_depends.types import AnyDict, P, AnyCallable
-
+from fast_depends.types import AnyCallable, AnyDict, P
 
 T = TypeVar("T")
 
 
 def args_to_kwargs(
-    arguments: Sequence[str], *args: P.args, **kwargs: P.kwargs
+    arguments: Iterable[str], *args: P.args, **kwargs: P.kwargs
 ) -> AnyDict:
     if not args:
         return kwargs
 
     unused = filter(lambda x: x not in kwargs, arguments)
 
     return dict((*zip(unused, args), *kwargs.items()))
 
 
-
-async def run_async(func: AnyCallable, *args: Any, **kwargs: AnyDict) -> Any:
+async def run_async(func: Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> T:
     if asyncio.iscoroutinefunction(func):
-        return await func(*args, **kwargs)
+        r = await func(*args, **kwargs)
+        return cast(T, r)
     else:
         return await run_in_threadpool(func, *args, **kwargs)
 
 
 async def run_in_threadpool(
     func: Callable[P, T], *args: P.args, **kwargs: P.kwargs
 ) -> T:
     if kwargs:  # pragma: no cover
         func = functools.partial(func, **kwargs)
     return await anyio.to_thread.run_sync(func, *args)
 
 
-
-def is_async_gen_callable(call: Callable[..., Any]) -> bool:
+def is_async_gen_callable(call: AnyCallable) -> bool:
     if inspect.isasyncgenfunction(call):
         return True
     dunder_call = getattr(call, "__call__", None)  # noqa: B004
     return inspect.isasyncgenfunction(dunder_call)
 
 
-def is_gen_callable(call: Callable[..., Any]) -> bool:
+def is_gen_callable(call: AnyCallable) -> bool:
     if inspect.isgeneratorfunction(call):
         return True
     dunder_call = getattr(call, "__call__", None)  # noqa: B004
     return inspect.isgeneratorfunction(dunder_call)
 
 
 def is_coroutine_callable(call: AnyCallable) -> bool:
     if inspect.isroutine(call):
         return inspect.iscoroutinefunction(call)
     if inspect.isclass(call):
         return False
-    call = getattr(call, "__call__", None)  # noqa: B004
-    return inspect.iscoroutinefunction(call)
+    call_ = getattr(call, "__call__", None)  # noqa: B004
+    return inspect.iscoroutinefunction(call_)
 
 
 async def solve_generator_async(
-    *, call: Callable[..., Any], stack: AsyncExitStack, sub_values: Dict[str, Any]
+    *, call: AnyCallable, stack: AsyncExitStack, sub_values: Dict[str, Any]
 ) -> Any:
     if is_gen_callable(call):
         cm = contextmanager_in_threadpool(contextmanager(call)(**sub_values))
     elif is_async_gen_callable(call):  # pragma: no branch
         cm = asynccontextmanager(call)(**sub_values)
     return await stack.enter_async_context(cm)
 
 
 def solve_generator_sync(
-    *, call: Callable[..., Any], stack: ExitStack, sub_values: Dict[str, Any]
+    *, call: AnyCallable, stack: ExitStack, sub_values: Dict[str, Any]
 ) -> Any:
     cm = contextmanager(call)(**sub_values)
     return stack.enter_context(cm)
 
 
 @asynccontextmanager
 async def contextmanager_in_threadpool(
@@ -103,8 +102,7 @@
         )
         if not ok:  # pragma: no branch
             raise e
     else:
         await anyio.to_thread.run_sync(
             cm.__exit__, None, None, None, limiter=exit_limiter
         )
-
```

### Comparing `fast_depends-1.1.2/fast_depends/library/model.py` & `fast_depends-1.1.3/fast_depends/library/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from abc import ABC
-from typing import Optional
+from typing import Optional, TypeVar
 
 from fast_depends.types import AnyDict
 
+Cls = TypeVar("Cls", bound="CustomField")
+
 
 class CustomField(ABC):
     param_name: Optional[str]
     cast: bool
     required: bool
 
     def __init__(self, *, cast: bool = True, required: bool = True) -> None:
         self.cast = cast
         self.param_name = None
         self.required = required
 
-    def set_param_name(self, name: str) -> "CustomField":
+    def set_param_name(self: Cls, name: str) -> Cls:
         self.param_name = name
+        return self
 
     def use(self, **kwargs: AnyDict) -> AnyDict:
         assert self.param_name, "You should specify `param_name` before using"
         return kwargs
```

### Comparing `fast_depends-1.1.2/LICENSE` & `fast_depends-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.2/README.md` & `fast_depends-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.2/pyproject.toml` & `fast_depends-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,20 @@
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "C901",  # too complex
 ]
 
+[tool.ruff.flake8-bugbear]
+extend-immutable-calls = [
+    "fast_depends.Depends",
+    "AsyncHeader", "Header", "MyDep"
+]
+
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-q"
 testpaths = [
     "tests",
 ]
```

### Comparing `fast_depends-1.1.2/PKG-INFO` & `fast_depends-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.1.2
+Version: 1.1.3
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

