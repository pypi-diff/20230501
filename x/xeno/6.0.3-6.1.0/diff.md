# Comparing `tmp/xeno-6.0.3.tar.gz` & `tmp/xeno-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-6.0.3.tar", last modified: Wed Apr 26 00:40:21 2023, max compression
+gzip compressed data, was "xeno-6.1.0.tar", last modified: Mon May  1 08:49:10 2023, max compression
```

## Comparing `xeno-6.0.3.tar` & `xeno-6.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-26 00:40:21.344179 xeno-6.0.3/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.0.3/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.0.3/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-26 00:40:21.344179 xeno-6.0.3/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.0.3/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-26 00:40:21.344179 xeno-6.0.3/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-26 00:40:02.000000 xeno-6.0.3/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-26 00:40:21.344179 xeno-6.0.3/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19114 2023-04-26 00:33:27.000000 xeno-6.0.3/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-04-25 22:04:51.000000 xeno-6.0.3/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10217 2023-04-25 17:49:47.000000 xeno-6.0.3/xeno/cookbook.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.0.3/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/events.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.0.3/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.0.3/xeno/pkg_config.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26055 2023-04-25 17:49:47.000000 xeno-6.0.3/xeno/recipe.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-04-25 17:49:47.000000 xeno-6.0.3/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-04-25 22:05:30.000000 xeno-6.0.3/xeno/spinner.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/testing.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-26 00:40:21.344179 xeno-6.0.3/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-01 08:49:10.575149 xeno-6.1.0/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.1.0/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.1.0/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-05-01 08:49:10.575149 xeno-6.1.0/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.1.0/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-01 08:49:10.575149 xeno-6.1.0/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-05-01 08:48:50.000000 xeno-6.1.0/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-01 08:49:10.575149 xeno-6.1.0/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19364 2023-05-01 08:47:56.000000 xeno-6.1.0/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-05-01 08:08:44.000000 xeno-6.1.0/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10293 2023-05-01 08:38:33.000000 xeno-6.1.0/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.1.0/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-05-01 07:35:53.000000 xeno-6.1.0/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.1.0/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.1.0/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25812 2023-05-01 08:45:14.000000 xeno-6.1.0/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-05-01 08:08:44.000000 xeno-6.1.0/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-05-01 08:08:44.000000 xeno-6.1.0/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.1.0/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-01 08:49:10.575149 xeno-6.1.0/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-05-01 08:49:10.000000 xeno-6.1.0/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-05-01 08:49:10.000000 xeno-6.1.0/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-01 08:49:10.000000 xeno-6.1.0/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-05-01 08:49:10.000000 xeno-6.1.0/xeno.egg-info/top_level.txt
```

### Comparing `xeno-6.0.3/LICENSE` & `xeno-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/PKG-INFO` & `xeno-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.0.3
+Version: 6.1.0
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xeno-6.0.3/README.md` & `xeno-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/setup.py` & `xeno-6.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="6.0.3",
+    version="6.1.0",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `xeno-6.0.3/xeno/__init__.py` & `xeno-6.1.0/xeno/__init__.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/abstract.py` & `xeno-6.1.0/xeno/abstract.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/async_injector.py` & `xeno-6.1.0/xeno/async_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/attributes.py` & `xeno-6.1.0/xeno/attributes.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/build.py` & `xeno-6.1.0/xeno/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # Author: Lain Musgrove (lain.proliant@gmail.com)
 # Date: Friday March 17, 2023
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
+import fnmatch
 import asyncio
 import multiprocessing
 import sys
 from argparse import ArgumentParser, HelpFormatter
 from collections import defaultdict
 from typing import Any, Callable, Iterable, Optional, cast
 
@@ -44,17 +45,17 @@
 
     class CleanupMode:
         NONE = "none"
         SHALLOW = "shallow"
         RECURSIVE = "recursive"
 
     class ColorOptions:
-        YES = 'yes'
-        NO = 'no'
-        AUTO = 'auto'
+        YES = "yes"
+        NO = "no"
+        AUTO = "auto"
 
     class SortingHelpFormatter(HelpFormatter):
         def add_arguments(self, actions):
             actions = sorted(actions, key=lambda a: a.option_strings)
             super().add_arguments(actions)
 
     def __init__(self):
@@ -313,25 +314,31 @@
 
         if callable(name_or_f):
             return wrapper(name_or_f)
 
         return wrapper
 
     async def _resolve_tasks(self, config: Config) -> list[Recipe]:
-        task_map = await self.addressable_task_map()
-        task_names = config.targets
+        task_map: dict[str, Recipe] = await self.addressable_task_map()
+        targets = config.targets
 
-        if not task_names:
+        if not targets:
             default_task = self.default_task()
             if default_task is not None:
-                task_names = [default_task]
+                targets = [default_task]
             else:
                 raise ValueError("No task specified and no default task defined.")
 
-        tasks = [task_map[k] for k in task_names]
+        task_names: set[str] = set()
+        tasks = []
+        for target in targets:
+            for name in fnmatch.filter(task_map.keys(), target):
+                if name not in task_names:
+                    task_names.add(name)
+                    tasks.append(task_map[name])
 
         return tasks
 
     async def _make_tasks(self, config, tasks):
         self.scan.scan_params(*tasks)
 
         try:
@@ -341,17 +348,16 @@
             args = self.scan.args(Recipe.PassMode.RESULTS)
             self.scan.clear()
             self.txt("OK", fg="green", render="bold")
             return args
 
         except BuildError as e:
             self.txt.embrace("ERROR", fg="red", render="bold")
-            self.txt(str(e))
             self.txt("FAIL", fg="red", render="bold")
-            return None
+            raise e
 
     async def _clean_tasks(self, config, tasks):
         match config.cleanup_mode:
             case Config.CleanupMode.SHALLOW:
                 return await asyncio.gather(*[task.clean() for task in tasks])
             case Config.CleanupMode.RECURSIVE:
                 return await asyncio.gather(
@@ -545,22 +551,25 @@
             self.print(event.data)
 
     def __call__(self, config: Config, engine: Engine, bus: EventBus):
         self.txt = engine.txt
         self.spinner.colorized = is_color_enabled()
         self.quiet = config.quiet
         self.to_stdout = config.to_stdout
-        bus.subscribe(Events.CLEAN, self.on_clean)
-        bus.subscribe(Events.ERROR, self.on_error)
-        bus.subscribe(Events.FAIL, self.on_fail)
-        bus.subscribe(Events.INFO, self.on_info)
-        bus.subscribe(Events.START, self.on_start)
-        bus.subscribe(Events.SUCCESS, self.on_success)
-        bus.subscribe(Events.WARNING, self.on_warning)
-        bus.subscribe(EventBus.FRAME, self.on_frame)
+        for event, listener in [
+            (Events.CLEAN, self.on_clean),
+            (Events.ERROR, self.on_error),
+            (Events.FAIL, self.on_fail),
+            (Events.INFO, self.on_info),
+            (Events.START, self.on_start),
+            (Events.SUCCESS, self.on_success),
+            (Events.WARNING, self.on_warning),
+            (EventBus.FRAME, self.on_frame),
+        ]:
+            bus.subscribe(event, listener)
 
 
 # --------------------------------------------------------------------
 engine = Engine()
 engine.add_hook(DefaultEngineHook())
 provide = engine.provide
 recipe = engine.recipe
```

### Comparing `xeno-6.0.3/xeno/color.py` & `xeno-6.1.0/xeno/color.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/cookbook.py` & `xeno-6.1.0/xeno/cookbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     docs: Optional[str] = None,
     factory=False,
     fmt: Optional[Recipe.Format] = None,
     keep=False,
     memoize=False,
     sigil: Optional[FormatF] = None,
     sync=False,
+    target: Optional[FormatF] = None,
 ):
     """
     Decorator for a function that defines a recipe template.
 
     The function is meant to be a recipe implementation method.  The
     parameters eventually passed to the method depend on whether the
     parameters are recipes or plain values.  Each recipe parameter has its
@@ -106,14 +107,15 @@
                         [*result],
                         docs=docs,
                         fmt=fmt or Recipe.Format(),
                         keep=keep,
                         memoize=memoize,
                         name=truename,
                         sync=sync,
+                        target=target
                     )
                 else:
                     result = cast(Recipe, result)
 
                     result.docs = docs
                     result.fmt = fmt or result.fmt
                     result.keep = keep
```

### Comparing `xeno-6.0.3/xeno/decorators.py` & `xeno-6.1.0/xeno/decorators.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/errors.py` & `xeno-6.1.0/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/events.py` & `xeno-6.1.0/xeno/events.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/namespaces.py` & `xeno-6.1.0/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/pkg_config.py` & `xeno-6.1.0/xeno/pkg_config.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/recipe.py` & `xeno-6.1.0/xeno/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,19 @@
         def __init__(self, fmt: "Recipe.Format", **overrides):
             self.fmt = fmt
             for key in overrides.keys():
                 if not hasattr(fmt, key):
                     raise ValueError(key)
             self.overrides = overrides
 
+        def add_override(self, key: str, value: Any):
+            self.overrides[key] = value
+
         def __getattribute__(self, name):
-            if name in ("overrides", "fmt"):
+            if name in ("overrides", "fmt", "add_override"):
                 return super().__getattribute__(name)
             if name in self.overrides:
                 return self.overrides[name]
             else:
                 return self.fmt.__getattribute__(name)
 
     class PassMode(Enum):
@@ -193,17 +196,14 @@
         async def gather_args(self):
             """
             Await resolution of recipes in args and update args with their results.
             """
             results = await asyncio.gather(
                 *[v() if isinstance(v, Recipe) else async_vwrap(v) for v in self._args]
             )
-            for n in self._arg_offsets:
-                if isinstance(results[n], Recipe):
-                    results[n].configure(self._args[n])
             self.scan_params(*results)
 
         def bind(self, f: Callable, mode: "Recipe.PassMode"):
             """
             Bind args and kwargs to the given callable.
             """
             return inspect.signature(f).bind(*self.args(mode), **self.kwargs(mode))
@@ -215,17 +215,14 @@
             result_tuples = asyncio.gather(
                 *[
                     async_map(k, v() if isinstance(v, Recipe) else async_vwrap(v))
                     for k, v in self._kwargs.items()
                 ]
             )
             results = {k: v for k, v in result_tuples}
-            for k in self._kwarg_keys:
-                if isinstance(results[k], Recipe):
-                    results[k].configure(self._kwargs[k])
             self.scan_params(**results)
 
         def gather_all(self):
             """
             Await resolution of recipes in args and kwargs and update both with
             their results.
             """
@@ -703,18 +700,17 @@
 
         if is_iterable(result):
             scanner = Recipe.Scanner()
             scanner.scan_params(*result)
             while scanner.has_recipes():
                 await scanner.gather_all()
             result = scanner.args(pass_mode=Recipe.PassMode.RESULTS)
-        else:
-            if isinstance(result, Recipe):
-                result._configure(self)
-                result = await result()
+
+        elif isinstance(result, Recipe):
+            result = await result()
 
         if self.has_target():
             assert isinstance(
                 result, str | Path
             ), "Recipe declared a file target, but the result was not a string or Path object."
 
             result = Path(result)
```

### Comparing `xeno-6.0.3/xeno/shell.py` & `xeno-6.1.0/xeno/shell.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/spinner.py` & `xeno-6.1.0/xeno/spinner.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/sync_injector.py` & `xeno-6.1.0/xeno/sync_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/testing.py` & `xeno-6.1.0/xeno/testing.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno/utils.py` & `xeno-6.1.0/xeno/utils.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.3/xeno.egg-info/PKG-INFO` & `xeno-6.1.0/xeno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.0.3
+Version: 6.1.0
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

