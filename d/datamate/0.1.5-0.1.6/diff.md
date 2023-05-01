# Comparing `tmp/datamate-0.1.5.tar.gz` & `tmp/datamate-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamate-0.1.5.tar", last modified: Sun Apr 30 17:33:14 2023, max compression
+gzip compressed data, was "datamate-0.1.6.tar", last modified: Mon May  1 19:13:36 2023, max compression
```

## Comparing `datamate-0.1.5.tar` & `datamate-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.398858 datamate-0.1.5/
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-04-30 17:33:14.398000 datamate-0.1.5/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3642 2023-03-06 13:58:32.000000 datamate-0.1.5/README.md
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.393271 datamate-0.1.5/datamate/
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      612 2023-03-15 22:43:05.000000 datamate-0.1.5/datamate/__init__.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    50945 2023-04-30 17:25:37.000000 datamate-0.1.5/datamate/directory.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    10441 2023-04-24 19:52:52.000000 datamate-0.1.5/datamate/namespaces.py
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.396179 datamate-0.1.5/datamate.egg-info/
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      292 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/SOURCES.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        1 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/dependency_links.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      109 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/requires.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        9 2023-04-30 17:33:14.000000 datamate-0.1.5/datamate.egg-info/top_level.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)       38 2023-04-30 17:33:14.399105 datamate-0.1.5/setup.cfg
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      715 2023-04-24 21:33:17.000000 datamate-0.1.5/setup.py
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-04-30 17:33:14.397348 datamate-0.1.5/tests/
--rwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    21665 2023-04-30 17:00:43.000000 datamate-0.1.5/tests/test_directory.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3747 2023-04-04 14:23:09.000000 datamate-0.1.5/tests/test_namespaces.py
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:13:36.093190 datamate-0.1.6/
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-05-01 19:13:36.092493 datamate-0.1.6/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3642 2023-03-06 13:58:32.000000 datamate-0.1.6/README.md
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:13:36.088283 datamate-0.1.6/datamate/
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      758 2023-04-30 18:04:13.000000 datamate-0.1.6/datamate/__init__.py
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    55504 2023-05-01 19:06:32.000000 datamate-0.1.6/datamate/directory.py
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    11921 2023-05-01 17:35:54.000000 datamate-0.1.6/datamate/namespaces.py
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:13:36.090734 datamate-0.1.6/datamate.egg-info/
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-05-01 19:13:35.000000 datamate-0.1.6/datamate.egg-info/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      292 2023-05-01 19:13:36.000000 datamate-0.1.6/datamate.egg-info/SOURCES.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        1 2023-05-01 19:13:35.000000 datamate-0.1.6/datamate.egg-info/dependency_links.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      109 2023-05-01 19:13:35.000000 datamate-0.1.6/datamate.egg-info/requires.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        9 2023-05-01 19:13:35.000000 datamate-0.1.6/datamate.egg-info/top_level.txt
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)       38 2023-05-01 19:13:36.093342 datamate-0.1.6/setup.cfg
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      869 2023-04-30 23:22:33.000000 datamate-0.1.6/setup.py
+drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:13:36.091900 datamate-0.1.6/tests/
+-rwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    28917 2023-05-01 19:06:56.000000 datamate-0.1.6/tests/test_directory.py
+-rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3747 2023-04-04 14:23:09.000000 datamate-0.1.6/tests/test_namespaces.py
```

### Comparing `datamate-0.1.5/PKG-INFO` & `datamate-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.5
+Version: 0.1.6
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.5/README.md` & `datamate-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `datamate-0.1.5/datamate/__init__.py` & `datamate-0.1.6/datamate/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 A data organization and compilation system.
 """
 
-__version__ = "0.1"
-
 from datamate.directory import (
     Directory,
     ArrayFile,
     set_root_dir,
     get_root_dir,
     enforce_config_match,
     check_size_on_init,
@@ -22,7 +20,16 @@
 __all__ = ["ArrayFile", "Directory", "Namespace"]
 
 # -- `__module__` rebinding ----------------------------------------------------
 
 Directory.__module__ = __name__
 ArrayFile.__module__ = __name__
 Namespace.__module__ = __name__
+
+
+def get_version():
+    from pathlib import Path
+    root = Path(__file__).parent
+    return open(root / "version", "r").read().strip()
+
+
+__version__ = get_version()
```

### Comparing `datamate-0.1.5/datamate/directory.py` & `datamate-0.1.6/datamate/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 This module exports the `Directory` class, an array- and metadata-friendly view
 into a directory.
 
 Instances of the base Directory class have methods to simplify reading/writing
-collections of arrays. `Directory` can also be subclassed to define Configurable,
-persistent computed asset types, within Python/PEP 484's type system.
+collections of arrays.
 
 This module also exports `ArrayFile` a descriptor protocol intended to be used
 as attribute type annotations within `Directory` subclass definition.
 """
 import os
 import warnings
 import itertools
@@ -27,29 +26,28 @@
     Mapping,
     MutableMapping,
     Optional,
     Tuple,
     Dict,
     Union,
     cast,
+    get_origin
 )
 from typing_extensions import Protocol
 import datetime
 from traceback import format_tb
 
 
 from contextlib import contextmanager
 
 import h5py as h5
 import numpy as np
 from pandas import DataFrame
-from ruamel import yaml
-from toolz import valmap
 
-from datamate.namespaces import Namespace, namespacify
+from datamate.namespaces import Namespace, namespacify, is_disjoint, is_superset, to_dict
 
 __all__ = ["Directory", "ArrayFile"]
 
 # -- Custom Errors and Warnings ------------------------------------------------
 
 
 class ConfigWarning(Warning):
@@ -133,36 +131,59 @@
 
     Example:
         with set_root_context(new_dir):
             dir = MyDirectory(...)
     """
 
     def decorator(callable):
-        @functools.wraps(callable)
-        def function(*args, **kwargs):
-            _root_dir = get_root_dir()
-            within_context = getattr(context, "within_root_context", False)
-            # case 1: root_dir provided
-            if root_dir is not None and not within_context:
-                set_root_dir(root_dir)
-            # case 2: root_dir provided and not within context
-            # case 3: root_dir provided and within context
-            # case 4: root dir not provided and not within context
-            # case 5: root dir not provided and within context
-            else:
+        if inspect.isfunction(callable):
+            @functools.wraps(callable)
+            def function(*args, **kwargs):
+                _root_dir = get_root_dir()
+                within_context = getattr(context, "within_root_context", False)
+                # case 1: root_dir provided
+                if root_dir is not None and not within_context:
+                    set_root_dir(root_dir)
+                # case 2: root_dir provided and not within context
+                # case 3: root_dir provided and within context
+                # case 4: root dir not provided and not within context
+                # case 5: root dir not provided and within context
+                else:
+                    set_root_dir(_root_dir)
+                _return = callable(*args, **kwargs)
+                set_root_dir(_root_dir)
+                return _return
+            return function
+        elif inspect.isclass(callable):
+            new = callable.__new__
+
+            @functools.wraps(callable)
+            def function(*args, **kwargs):
+                _root_dir = get_root_dir()
+                within_context = getattr(context, "within_root_context", False)
+                # case 1: root_dir provided
+                if root_dir is not None and not within_context:
+                    set_root_dir(root_dir)
+                # case 2: root_dir provided and not within context
+                # case 3: root_dir provided and within context
+                # case 4: root dir not provided and not within context
+                # case 5: root dir not provided and within context
+                else:
+                    set_root_dir(_root_dir)
+                _return = new(*args, **kwargs)
                 set_root_dir(_root_dir)
-            _return = callable(*args, **kwargs)
-            set_root_dir(_root_dir)
-            return _return
+                return _return
 
-        return function
+            callable.__new__ = function
 
+            return callable
+        else:
+            raise ValueError
     return decorator
 
-
 @contextmanager
 def set_root_context(root_dir: Union[str, Path, NoneType] = None):
     """Set root directory within a context and revert after.
 
     Example:
         with set_root_context(dir):
             Directory(config)
@@ -200,31 +221,31 @@
 
     Note: checking the size of a directory is slow, therefore this should
     be used only consciously.
     """
     context.check_size_on_init = enforce
 
 
+def get_check_size_on_init() -> bool:
+    return context.check_size_on_init
+
+
 def set_verbosity_level(level: int) -> None:
     """
     Set verbosity level of representation for Directorys.
 
     0: only the top level directory name and the last modified date are shown.
     1: maximally 2 levels and 25 lines are represented.
     2: all directorys and files are represented.
 
     Defaults to 2.
     """
     context.verbosity_level = level
 
 
-def get_check_size_on_init() -> bool:
-    return context.check_size_on_init
-
-
 def set_scope(scope: Optional[Dict[str, type]]) -> None:
     """
     Set the scope used for "type" field resolution.
     """
     if hasattr(context, "scope"):
         del context.scope
     if scope is not None:
@@ -271,118 +292,135 @@
 
 
 class Directory(metaclass=NonExistingDirectory):
     """
     An array- and metadata-friendly view into a directory
 
     Arguments:
-        path (Path|str): The path at which the Directory is, or should be,
-            stored
-        conf (Mapping[str, object]): The build Namespace, optionally
-            including a "type" field indicating the type of Directory to search
-            for/construct
+        path Union[str, Path]: The path at which the Directory is, or should be,
+            stored, can be relative to the current `root_dir`.
+        config Dict[str, object]: The configuration of the Directory.
+            When including a "type" field indicates the type of Directory to
+            search for and construct in the scope. Note, the config can be
+            unpacked into the constructor as keyword arguments.
 
     Constructors:
-         - Directory(name: str)\n'
-         - Directory(name: str, conf: Mapping[str, object])'
-         - Directory(conf: Mapping[str, object])\n'
-         - Directory(path: Path|str)\n'
-         - Directory(path: Path|str, conf: Mapping[str, object])\n'
+         - Directory(): creates auto-named Directory inside the current
+            `root_dir`.
+         - Directory(config: Dict[str, object]): creates auto-named Directory inside
+            the current `root_dir` with the given config. If __init__ is
+            implemented, it will be called with the config as keyword arguments.
+         - Directory(path: Union[str, Path]): creates named Directory inside the
+             current `root_dir`. `path` will be either relative to the current
+                `root_dir` or absolute.
+         - Directory(path: Union[str, Path], config: Dict[str, object]): creates
+            named Directory inside the
+             current `root_dir`. `path` will be either relative to the current
+                `root_dir` or absolute. If __init__ is
+            implemented, it will be called with the config as keyword arguments.
 
 
-    If only `path` is provided, the Directory corresponding to `Path` is
+    If only `path` is provided, the corresponding Directory is
     returned. It will be empty if `path` points to an empty or nonexistent
     directory.
 
-    If only `conf` is provided, it will search the current `root_dir`
+    If only `config` is provided, it will search the current `root_dir`
     for a matching directory, and return a Directory pointing there if it
     exists. Otherwise, a new Directory will be constructed at the top level of
     the `root_dir`.
 
-    If both `path` and `conf` are provided, it will return the Directory
+    If both `path` and `config` are provided, it will return the Directory
     at `path`, building it if necessary. If `path` points to an existing
-    directory that is not a sucessfully built Directory matching `conf`, an
+    directory that is not a sucessfully built Directory matching `config`, an
     error is raised.
 
-    Fields:
-        - **path** (*Path*): The path to the root of the file tree backing this \
-            Directory
-        - **conf** (*Namespace*): The Namespace (inherited from
-            `Configurable`)
-        - **meta** (*Namespace*): The metadata stored in \
-            `{self.path}/_meta.yaml`
-
-    After instantiation, Directorys act as string-keyed `MutableMapping`s (with
-    some additional capabilities), containing three types of entries:
-    `ArrayFile`s, `Path`s, and other `Directory`s.
+    Attributes:
+        path (Path): The path at which the Directory is, or should be, stored.
+        config (Dict[str, object]): The configuration of the Directory.
+
+    After instantiation, Directorys act as string-keyed mutable dictionaries,
+    containing three types of entries: `ArrayFile`s, `Path`s, and other `Directory`s.
 
     `ArrayFile`s are single-entry HDF5 files, in SWMR mode. Array-like numeric
     and byte-string data (valid operands of `numpy.asarray`) written into an
     Directory via `__setitem__`, `__setattr__`, or `extend` is stored as an array
     file.
 
     `Path`s are non-array files, presumed to be encoded in a format that
     is not understood. They are written and read as normal
     `Path`s, which support simple text and byte I/O, and can be passed to more
     specialized libraries for further processing.
 
     `Directory` entries are returned as properly subtyped Directorys, and can be
     created, via `__setitem__`, `__setattr__`, or `extend`, from existing
-    Directorys or (possibly nested) string-keyed `Mapping`s (*e.g* a dictionary
-    of arrays).
+    Directorys or (possibly nested) dictionaries of arrays.
     """
 
     class Config(Protocol):
         """
-        A configuration
-
-        If its definition is inline (lexically within the containing class'
-        definition), it will be translated into a JSON-Schema to validate
-        configurations passed into the outer class' constructor.
-
-        `Config` classes are intended to be interface definitions. They can extend
-        `typing_extensions.Protocol` to support static analysis.
-
-        An empty `Conf` definition is created for every `Configurable` subclass
-        defined without one.
+        `Config` classes are intended to be interface definitions. They are
+        used to define the structure of the `config` argument to the
+        `Directory` constructor, and to provide type hints for the `config`
+        attribute of `Directory` instances.
         """
 
         pass
 
     path: Path
     config: Config
 
-    def __new__(cls, *args: object, **kwargs: object) -> Any:
+    def __new__(_type, *args: object, **kwargs: object) -> Any:
         path, config = _parse_directory_args(args, kwargs)
-        cls = _directory(cls)
+        cls = _directory(_type)
         _check_implementation(cls)
-        if config is None and has_defaults_for_init(cls) and _implements_init(cls):
-            config = get_defaults(cls)
+
+        defaults = get_defaults(cls)
+
+        if config is None and defaults:  # and _implements_init(cls):
+            # to initialize from defaults if no config or path is provided
+            if path is None:
+                config = defaults
+            # to initialize from defaults if no config and empty path is provided
+            elif path is not None and not path.exists():
+                config = defaults
+            # if a non-empty path is provided, we cannot initialize from defaults
+            else:
+                pass
         # breakpoint()
         if path is not None and config is None:
-            cls = _check_size(_directory_from_path(cls, _resolve_path(path)))
+            cls = _directory_from_path(cls, _resolve_path(path))
         elif path is None and config is not None:
-            cls = _check_size(_directory_from_config(cls, config))
+            cls = _directory_from_config(cls, config)
         elif path is not None and config is not None:
-            cls = _check_size(
-                _directory_from_path_and_config(cls, _resolve_path(path), config)
-            )
+            cls = _directory_from_path_and_config(cls, _resolve_path(path), config)
         elif path is None and config is None:
             if _implements_init(cls):
                 # raise ValueError("no configuration provided")
                 pass
 
-        cls.__doc__ = _update_doc(cls)
+        if context.check_size_on_init:
+            cls.check_size()
 
         return cls
 
-    def __init__(self, config: Config):
-        """Implement to compile data at runtime from a configuration."""
+    def __init__(self):
+        """Implement to compile `Directory` from a configuration.
+
+        Note, subclasses can either implement Config to determine the interface,
+        types and defaults of `config`, or implement `__init__` with keyword
+        arguments to determine the interface, types and defaults of `config`.
+        In case both are implemented, the config is created from the joined
+        interface of both as long as defaults are not conflicting.
+        """
         pass
 
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+        cls.__doc__ = _auto_doc(cls)
+
     @property
     def meta(self) -> Namespace:
         """
         The metadata stored in `{self.path}/_meta.yaml`
         """
         return read_meta(self.path)
 
@@ -420,158 +458,48 @@
 
     def __deepcopy__(self, memodict={}):
         return self.__copy__()
 
     def keys(self) -> Iterator[str]:
         return self.__iter__()
 
-    def size(self) -> None:
-        __check_size = get_check_size_on_init()
-        check_size_on_init(True)
-        _check_size(self, print_size=True)
-        check_size_on_init(__check_size)
-
     def items(self) -> Iterator[Tuple[str, ArrayFile]]:
         for key in self.keys():
             yield (key, self[key])
 
-    def to_df(self, dtypes: dict = None) -> DataFrame:
-        """
-        Returns a DataFrame from all equal length, single-dim .h5 datasets in self.path.
-        """
-        # to cache the dataframe that is expensive to create.
-        try:
-            return object.__getattribute__(self, "_as_df")
-        except:
-            object.__setattr__(self, "_as_df", directory_to_df(self, dtypes))
-            return self.to_df()
-
     @classmethod
     def from_df(cls, df: DataFrame, dtypes: dict, *args, **kwargs):
         directory = Directory.__new__(Directory, *args, **kwargs)
         directory.update(
             {column: df[column].values.astype(dtypes[column]) for column in df.columns}
         )
         return directory
 
-    def to_dict(self) -> DataFrame:
-        """
-        Returns a DataFrame from all equal length, single-dim .h5 datasets in self.path.
-        """
-        # to cache the dict that is expensive to create.
-        try:
-            return object.__getattribute__(self, "_as_dict")
-        except:
-            object.__setattr__(self, "_as_dict", directory_to_dict(self))
-            return self.to_dict()
-
-    # TODO: from dict
-
     def update(self, other, suffix: str = "") -> None:
         """
         Updates self with items of other and appends an optional suffix.
         """
         for key in other:
             if key + suffix not in self:
                 self[key + suffix] = other[key]
 
     def move(self, dst):
         """Move directory to dst."""
-        return shutil.move(self.path, dst)
+        shutil.move(self.path, dst)
+        return Directory(dst)
 
     def rmtree(self, y_n=None):
         reply = y_n or input(f"delete {self.path} recursively, y/n?")
         if reply.lower() == "y":
             shutil.rmtree(self.path, ignore_errors=True)
 
     def _rebuild(self, y_n=None):
         self.rmtree(y_n)
         _build(self)
 
-    def check_size(self, print=True):
-        return check_size(self.path, print_size=print)
-
-    def mtime(self):
-        return datetime.datetime.fromtimestamp(self.path.stat().st_mtime)
-
-    @property
-    def parent(self):
-        return Directory(self.path.absolute().parent)
-
-    def _override_config(self, config, status=None):
-        """Overriding config stored in _meta.yaml.
-
-        config (Dict): update for meta.config
-        status (str): status if config did not exist before, i.e. _overrid_config
-            is used to store a _meta.yaml for the first time instead of build.
-        """
-        meta_path = self.path / "_meta.yaml"
-
-        def write_meta(**kwargs):
-            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
-
-        current_config = self.config
-        if current_config is not None:
-            with warnings.catch_warnings():
-                warnings.simplefilter("always")
-                warnings.warn(
-                    (
-                        f"Overriding config. Diff is:"
-                        f'{config.diff(current_config, name1="passed", name2="stored")}'
-                    ),
-                    ConfigWarning,
-                    stacklevel=2,
-                )
-            write_meta(config=config, status="overridden")
-        else:
-            write_meta(config=config, status=status or self.status)
-
-    def _override_status(self, status):
-        meta_path = self.path / "_meta.yaml"
-
-        def write_meta(**kwargs):
-            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
-
-        current_status = self.status
-        if current_status is not None:
-            with warnings.catch_warnings():
-                warnings.simplefilter("always")
-                warnings.warn(
-                    (f"Overriding status {current_status} to {status}"),
-                    ConfigWarning,
-                    stacklevel=2,
-                )
-        write_meta(config=self.config, status=status)
-
-    def _modified_past_init(self, is_modified):
-        meta_path = self.path / "_meta.yaml"
-
-        def write_meta(**kwargs):
-            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
-
-        if is_modified:
-            write_meta(config=self.config, status=self.status, modified=True)
-
-    def _count(self) -> int:
-        root = self.path
-        count = 0
-        for i in itertools.count():
-            dst = root / f"{i:04x}"
-            if dst.exists():
-                count += 1
-            else:
-                return count
-        return count
-
-    def _next(self) -> int:
-        root = self.path
-        dst = root / f"{self._count():04x}"
-        assert not dst.exists()
-        return Directory(dst, self.config)
-
     def __truediv__(self, other):
         return self.__getitem__(other)
 
     def __getitem__(self, key: str) -> Any:
         """
         Returns an `ArrayFile`, `Path`, or `Directory` corresponding to
         `self.path/key`
@@ -590,15 +518,15 @@
             # this will yield a TypeError because Path / slice does not work.
             path = self.path / key
         except TypeError as e:
             if not self.path.exists():
                 raise (
                     AssertionError(
                         f"Indexing {self.path.name} at {key} not possible for"
-                        f"Directory at {self.path.parent}. File "
+                        f" Directory at {self.path.parent}. File "
                         f"{self.path.name}.h5 does not exist."
                     )
                 )
             raise e
 
         # Return an array.
         if path.with_suffix(".h5").is_file():
@@ -677,14 +605,49 @@
         elif path.is_file():
             path.unlink()
 
         # Delete a Directory.
         else:
             shutil.rmtree(path, ignore_errors=True)
 
+    def extend(self, key: str, val: object) -> None:
+        """
+        Extends an `ArrayFile`, `Path`, or `Directory` at `self.path/key`
+
+        Extending `ArrayFile`s performs concatenation along the first axis,
+        extending `Path`s performs byte-level concatenation, and
+        extending subDirectorys extends their fields.
+
+        Files corresponding to `self[key]` are created if they do not already
+        exist.
+        """
+        path = self.path / key
+
+        # Append an existing file.
+        if isinstance(val, Path):
+            assert path.suffix != ""
+            _extend_file(path, val)
+
+        # Append a subDirectory.
+        elif isinstance(val, (Mapping, Directory)):
+            assert path.suffix == ""
+            for k in val:
+                Directory(path).extend(k, val[k])
+
+        # Append an array.
+        else:
+            assert path.suffix == ""
+            _extend_h5(path.with_suffix(".h5"), val)
+
+        if self.config is not None and self.status == "done":
+            # Track if a Directory has been modified past __init__
+            self._modified_past_init(True)
+
+    # --- Views ---
+
     def __repr__(self):
         if context.verbosity_level == 1:
             string = tree(
                 self.path,
                 last_modified=True,
                 level=2,
                 length_limit=25,
@@ -726,43 +689,14 @@
                 length_limit=length_limit,
                 last_modified=last_modified,
                 verbose=verbose,
                 limit_to_directories=limit_to_directories,
             )
         )
 
-    def extend(self, key: str, val: object) -> None:
-        """
-        Extends an `ArrayFile`, `Path`, or `Directory` at `self.path/key`
-
-        Extending `ArrayFile`s performs concatenation along the first axis,
-        extending `Path`s performs byte-level concatenation, and
-        extending subDirectorys extends their fields.
-
-        Files corresponding to `self[key]` are created if they do not already
-        exist.
-        """
-        path = self.path / key
-
-        # Append an existing file.
-        if isinstance(val, Path):
-            assert path.suffix != ""
-            _extend_file(path, val)
-
-        # Append a subDirectory.
-        elif isinstance(val, (Mapping, Directory)):
-            assert path.suffix == ""
-            for k in val:
-                Directory(path).extend(k, val[k])
-
-        # Append an array.
-        else:
-            assert path.suffix == ""
-            _extend_h5(path.with_suffix(".h5"), val)
-
     # -- Attribute-style element access --------------------
 
     def __getattr__(self, key: str) -> Any:
         return self.__getitem__(key.replace("__", "."))
 
     def __setattr__(self, key: str, value: object) -> None:
         # Fix autoreload related effect.
@@ -792,44 +726,190 @@
 
         for key in set(self).difference(object.__dir__(self)):
             object.__setattr__(self, key, self[key])
             self._cached_keys.add(key)
 
         return cast(list, object.__dir__(self))
 
-    # -- Other convenience methods --------------------
+    # -- Convenience methods
+
+    def _override_config(self, config, status=None):
+        """Overriding config stored in _meta.yaml.
+
+        config (Dict): update for meta.config
+        status (str): status if config did not exist before, i.e. _overrid_config
+            is used to store a _meta.yaml for the first time instead of build.
+        """
+        meta_path = self.path / "_meta.yaml"
+
+        def write_meta(**kwargs):
+            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
+
+        current_config = self.config
+        if current_config is not None:
+            with warnings.catch_warnings():
+                warnings.simplefilter("always")
+                warnings.warn(
+                    (
+                        f"Overriding config. Diff is:"
+                        f'{config.diff(current_config, name1="passed", name2="stored")}'
+                    ),
+                    ConfigWarning,
+                    stacklevel=2,
+                )
+            write_meta(config=config, status="overridden")
+        else:
+            write_meta(config=config, status=status or self.status)
+
+    def _override_status(self, status):
+        meta_path = self.path / "_meta.yaml"
+
+        def write_meta(**kwargs):
+            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
+
+        current_status = self.status
+        if current_status is not None:
+            with warnings.catch_warnings():
+                warnings.simplefilter("always")
+                warnings.warn(
+                    (f"Overriding status {current_status} to {status}"),
+                    ConfigWarning,
+                    stacklevel=2,
+                )
+        write_meta(config=self.config, status=status)
+
+    def _modified_past_init(self, is_modified):
+        meta_path = self.path / "_meta.yaml"
+
+        def write_meta(**kwargs):
+            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
+
+        if is_modified:
+            write_meta(config=self.config, status=self.status, modified=True)
+
+    def check_size(self, warning_at=20 * 1024**3, print_size=False) -> None:
+        """Prints the size of the directory in bytes."""
+        return check_size(self.path, warning_at, print_size)
+
+    def to_df(self, dtypes: dict = None) -> DataFrame:
+        """
+        Returns a DataFrame from all equal length, single-dim .h5 datasets in self.path.
+        """
+        # to cache the dataframe that is expensive to create.
+        try:
+            return object.__getattribute__(self, "_as_df")
+        except:
+            object.__setattr__(self, "_as_df", directory_to_df(self, dtypes))
+            return self.to_df()
+
+    def to_dict(self) -> DataFrame:
+        """
+        Returns a DataFrame from all equal length, single-dim .h5 datasets in self.path.
+        """
+        # to cache the dict that is expensive to create.
+        try:
+            return object.__getattribute__(self, "_as_dict")
+        except:
+            object.__setattr__(self, "_as_dict", directory_to_dict(self))
+            return self.to_dict()
+
+    def mtime(self):
+        return datetime.datetime.fromtimestamp(self.path.stat().st_mtime)
+
+    @property
+    def parent(self):
+        return Directory(self.path.absolute().parent)
 
-    def _clear_dir(self, suffix: str) -> None:
+    def _count(self) -> int:
+        root = self.path
+        count = 0
+        for i in itertools.count():
+            dst = root / f"{i:04x}"
+            if dst.exists():
+                count += 1
+            else:
+                return count
+        return count
+
+    def _next(self) -> int:
+        root = self.path
+        dst = root / f"{self._count():04x}"
+        assert not dst.exists()
+        return Directory(dst, self.config)
+
+    def _clear_filetype(self, suffix: str) -> None:
         """
-        Delete files ending with suffix in the current wrap path
+        Delete files ending with suffix in the current directory path
         """
         for file in self.path.iterdir():
             if file.is_file() and file.suffix == suffix:
                 file.unlink()
 
 
 # -- Directory construction -----------------------------------------------------
 
 
-def get_defaults(cls):
+def merge(dict1, dict2):
+    merged = {}
+    if is_disjoint(dict1, dict2):
+        merged.update(dict1)
+        merged.update(dict2)
+    elif is_superset(dict1, dict2):
+        merged.update(dict1)
+    elif is_superset(dict2, dict1):
+        merged.update(dict2)
+    else:
+        raise ValueError(f"merge conflict: {dict1} and {dict2}")
+    return merged
+
+
+def get_defaults(cls: Directory):
+    try:
+        return merge(get_defaults_from_Config(cls), get_defaults_from_init(cls))
+    except ValueError as e:
+        raise ValueError("conflicting defaults") from e
+
+
+def get_defaults_from_Config(cls: Union[type, Directory]):
+    cls = cls if isinstance(cls, type) else type(cls)
     if "Config" in cls.__dict__:
-        defaults = {
+        return {
             k: v
             for k, v in cls.Config.__dict__.items()
             if not (k.startswith("_") or (k.startswith("__") and k.endswith("__")))
         }
-        return Namespace(defaults)
-    return Namespace({})
+    return {}
+
 
+def get_defaults_from_init(cls: Directory):
+    cls = cls if isinstance(cls, type) else type(cls)
+    signature = inspect.signature(cls.__init__)
+    defaults = {
+        k: v.default
+        for k, v in signature.parameters.items()
+        if v.default != inspect._empty
+    }
+    return defaults
 
-def get_annotations(cls):
+
+def get_annotations(cls: Union[type, Directory]):
+    return merge(get_annotations_from_Config(cls), get_annotations_from_init(cls))
+
+
+def get_annotations_from_Config(cls: Union[type, Directory]):
+    cls = cls if isinstance(cls, type) else type(cls)
     if "Config" in cls.__dict__:
         annotations = getattr(cls.Config, "__annotations__", {})
-        return Namespace(annotations)
-    return Namespace({})
+        return annotations
+    return {}
+
+
+def get_annotations_from_init(cls: Directory):
+    cls = cls if isinstance(cls, type) else type(cls)
+    return {k: v for k, v in cls.__init__.__annotations__.items() if v is not None}
 
 
 def _parse_directory_args(
     args: Tuple[object, ...], kwargs: Mapping[str, object]
 ) -> Tuple[Optional[Path], Optional[Mapping[str, object]]]:
     """
     Return `(path, conf)` or raise an error.
@@ -899,95 +979,67 @@
             "    - Directory(path: Path|str)\n"
             "    - Directory(path: Path|str, conf: Mapping[str, object])\n"
             "    - Directory(name: str)\n"
             "    - Directory(name: str, conf: Mapping[str, object])"
         )
 
 
-def _implements_init(cls: type) -> bool:
+def _implements_init(cls: Directory) -> bool:
     """True if the class implements `__init__`."""
     return inspect.getsource(cls.__init__).split("\n")[-2].replace(" ", "") != "pass"
 
 
-def has_defaults_for_init(cls):
-    """Directory subclasses that specify
+def _check_implementation(cls: Directory):
+    defaults = get_defaults(cls)
+    # check if Config only has annotations, no defaults
+    annotations = get_annotations(cls)
 
-    class Config:
-        foo = 1
-        bar = 2
-
-    and are constructed without arguments will be initialized with
-    `foo=1` and `bar=2`.
-    """
-    return (
-        "Config" in cls.__class__.__dict__
-        # and len(inspect.signature(cls.__init__).parameters) == 1
-        and get_defaults(cls.__class__)
-    )
-
-
-def _check_implementation(cls):
-    defaults = get_defaults(cls.__class__)
-
-    if not defaults:
-        # check if Config only has annotations, no defaults
-        defaults = get_annotations(cls.__class__)
-
-    if _implements_init(cls) and not defaults:
+    if _implements_init(cls) and not defaults and not annotations:
         with warnings.catch_warnings():
             warnings.simplefilter("always")
             warnings.warn(
                 (f"The Directory {type(cls)} implements __init__ but not Config."),
                 ImplementationWarning,
                 stacklevel=2,
             )
 
 
 def _directory(cls: type) -> Directory:
     """
-    Return a new Directory corresponding to the file tree at root_dir / cls.__name___ *
+    Return a new Directory at the root of the file tree.
     """
     directory = _forward_subclass(cls, {})
     path = _new_directory_path(type(directory))
     object.__setattr__(directory, "_cached_keys", set())
     object.__setattr__(directory, "path", path)
     return directory
 
 
-def _directory_from_path(cls: type, path: Path) -> Directory:
+def _directory_from_path(cls: Directory, path: Path) -> Directory:
     """
     Return a Directory corresponding to the file tree at `path`.
 
     An error is raised if the type recorded in `_meta.yaml`, if any, is not a
     subtype of `cls`.
     """
 
-    def _has_defaults_for_init(cls):
-        """True if cls implements Config and __init__(self, config)"""
-        return (
-            "Config" in cls.__dict__
-            and len(inspect.signature(cls.__init__).parameters) == 2
-        )
-
     config = read_meta(path).config or {}
     written_type = get_scope().get(config.get("type", None), None)
 
     if path.is_file():
         raise FileExistsError(f"{path} is a file.")
 
     # if context.enforce_config_match:
 
-    # if directory is constructed from path that does not exist,
-    # but that does implement an init function method and has no defaults
-    # for the config, raise an error
-    if _implements_init(cls) and not _has_defaults_for_init(cls) and not path.is_dir():
-        raise FileNotFoundError(f"{path} does not exist.")
-
-    # otherwise pass which is important for the case where the directory
-    # is constructed from a path that does not exist
+    if not path.is_dir():
+        if _implements_init(cls) and not get_defaults(cls):
+            raise FileNotFoundError(
+                f"cannot initialize {path}. It does not yet exist"
+                f" and no config was provided to initialize it."
+            )
     else:
         pass
 
     if written_type is not None and not issubclass(written_type, type(cls)):
         raise FileExistsError(
             f"{path} is a {written_type.__module__}.{written_type.__qualname__}"
             f", not a {cls.__module__}.{cls.__qualname__}."
@@ -999,28 +1051,31 @@
     #     directory = _forward_subclass(type(cls), {})
 
     object.__setattr__(directory, "_cached_keys", set())
     object.__setattr__(directory, "path", path)
     return directory
 
 
-def _directory_from_config(cls: type, conf: Mapping[str, object]) -> Directory:
+def _directory_from_config(cls: Directory, conf: Mapping[str, object]) -> Directory:
     """
-    Find or build a Directory with the given type and Namespace.
+    Find or build a Directory with the given type and config.
     """
     directory = _forward_subclass(type(cls), conf)
     new_dir_path = _new_directory_path(type(directory))
     object.__setattr__(directory, "_cached_keys", set())
     config = Namespace(**directory._config)
 
     def _new_directory():
         object.__setattr__(directory, "path", new_dir_path)
-        # return empty path cause only the type field is populated
+        # don't build cause only the type field is populated
         if list(config.keys()) == ["type"]:
             return directory
+        # don't build cause the config matches the defaults and init is not implemented
+        if not _implements_init(cls) and config.without("type") == get_defaults(cls):
+            return directory
         # catches FileExistsError for the case when two processes try to
         # build the same directory simultaneously
         try:
             _build(directory)
         except FileExistsError:
             return _directory_from_config(cls, conf)
         return directory
@@ -1059,18 +1114,18 @@
             if meta.status == "done":
                 object.__setattr__(directory, "path", path)
                 return directory
     return _new_directory()
 
 
 def _directory_from_path_and_config(
-    cls: type, path: Path, conf: Mapping[str, object]
+    cls: Directory, path: Path, conf: Mapping[str, object]
 ) -> Directory:
     """
-    Find or build a Directory with the given type, path, and Namespace.
+    Find or build a Directory with the given type, path, and config.
     """
     directory = _forward_subclass(type(cls), conf)
     object.__setattr__(directory, "_cached_keys", set())
     object.__setattr__(directory, "path", path)
 
     if path.exists():
         meta = read_meta(path)
@@ -1094,28 +1149,35 @@
                     )
         while meta.status == "running":
             sleep(0.01)
             meta = read_meta(path)
         if directory.meta.status == "stopped":
             raise FileExistsError(f'"{directory.path}" was stopped mid-build.')
     else:
+        # don't build cause only the type field is populated
+        if list(directory._config.keys()) == ["type"]:
+            return directory
+        # don't build cause the config matches the defaults and init is not implemented
+        if not _implements_init(cls) and directory._config.without(
+            "type"
+        ) == get_defaults(cls):
+            return directory
         # catches FileExistsError for the case when two processes try to
         # build the same directory simultaneously
         try:
             _build(directory)
         except FileExistsError:
             return _directory_from_path_and_config(cls, path, conf)
     return directory
 
 
 def _build(directory: Directory) -> None:
     """
     Create parent directories, invoke `Directory.__init__`, and store metadata.
     """
-    # TODO: Fix YAML generation.
 
     if directory.path.exists() and directory.status == "done":
         return
     elif directory.path.exists() and directory.status == "running":
         sleep(0.01)
         return _build(directory)
 
@@ -1128,53 +1190,108 @@
     )
 
     write_meta(config=config, status="running")
 
     try:
         if callable(getattr(type(directory), "__init__", None)):
             n_build_args = directory.__init__.__code__.co_argcount
-            build_args = [directory._config] if n_build_args > 1 else []
-            directory.__init__(*build_args)
+            # case 1: __init__(self)
+            if n_build_args <= 1:
+                build_args = []
+                build_kwargs = {}
+            # case 2: __init__(self, config)
+            elif n_build_args == 2:
+                build_args = [directory._config]
+                build_kwargs = {}
+            # case 3: __init__(self, foo=1, bar=2) to specify defaults and config
+            else:
+                kwargs = namespacify(get_defaults_from_init(directory))
+                assert kwargs
+                build_args = []
+                build_kwargs = {k: directory._config[k] for k in kwargs}
+            directory.__init__(*build_args, **build_kwargs)
+
         write_meta(config=config, status="done")
     except BaseException as e:
         write_meta(config=config, status="stopped")
         raise e
 
 
-def _update_doc(cls):
-    if "Config" not in cls.__class__.__dict__ or not get_defaults(cls.__class__):
-        return cls.__doc__
-    Config = cls.__class__.__dict__["Config"]
-
-    def clsstrip(string):
-        string = string[string.find("'") + 1 : string.rfind("'")]
-        return string.replace("__main__.", "")
-
-    doc = cls.__doc__
-    if doc is None:
-        doc = ""
-    else:
-        doc += "\n\n"
-    doc += "Initialize from config or leave default:\n"
-    doc += "{}(dict(\n{}))"
-    attributes = ""
-    for k, v in Config.__dict__.items():
-        if not k.startswith("__"):
-            if (
-                hasattr(Config, "__annotations__")
-                and Config.__annotations__.get(k, None) is not None
-            ):
-                annotation = Config.__annotations__.get(k)
-                attributes += f"{k}: {clsstrip(repr(annotation))} = {v},\n"
-            else:
-                attributes += f"{k} = {v},\n"
+def call_signature(cls):
+    signature = (
+"""
+
+Example call signature:
+    {}
+    {}
+Note, these use the `Directory(config: Dict[str, object])` constructor and are
+inferred from defaults and annotations, i.e. they are equivalent to constructing
+without arguments."""
+)
+    defaults = to_dict(get_defaults(cls))
+    string = ""
+    for key, val in defaults.items():
+        string += f"{key}={val}, "
+    if string.endswith(", "):
+        string = string[:-2]
+    # variant 1: unpacking config kwargs
+    signature1 = ""
+    if string:
+        signature1 = f"{cls.__qualname__}({string})"
+    # variant 2: whole config
+    signature2 = ""
+    if defaults:
+        signature2 = f"{cls.__qualname__}({defaults})"
+
+    if signature1 and signature2:
+        return signature.format(signature1, signature2)
+
+    return signature.format("(specify defaults for auto-doc of call signature)", "")
 
-    name = clsstrip(repr(Config)).replace(".Config", "")
-    return doc.format(name, attributes)
 
+def type_signature(cls):
+    signature = (
+    """
+
+    Types of config elements:
+       {}
+
+    """
+    )
+    annotations = to_dict(get_annotations(cls))
+    def qualname(annotation):
+        origin = get_origin(annotation)
+        if origin:
+            return repr(annotation)
+        return annotation.__qualname__
+    signature1 = ""
+    for key, val in annotations.items():
+        signature1 += f"{key}: {qualname(val)}, "
+    if signature1.endswith(", "):
+        signature1 = signature1[:-2]
+    if signature1:
+        return signature.format(signature1)
+    return signature.format("(annotate types for auto-doc of type signature)")
+
+def _auto_doc(cls: type, cls_doc=True, base_doc=False):
+    docstring = "{}{}{}{}"
+    if isinstance(cls, Directory):
+        cls = type(cls)
+    call_sig = call_signature(cls)
+    type_sig = type_signature(cls)
+
+    _cls_doc = ""
+    if cls_doc and cls.__doc__:
+        _cls_doc = cls.__doc__
+
+    _base_doc = ""
+    if base_doc and cls.__base__.__doc:
+        _base_doc = cls.__base__.__doc__
+
+    return docstring.format(_cls_doc, call_sig, type_sig, _base_doc)
 
 def _resolve_path(path: Path) -> Path:
     """
     Dereference ".", "..", "~", and "@".
     """
     if path.parts[0] == "@":
         path = get_root_dir() / "/".join(path.parts[1:])
@@ -1190,24 +1307,17 @@
     for i in itertools.count():
         dst = root / f"{type_name}_{i:04x}"
         if not dst.exists():
             return dst.absolute()
     assert False  # for MyPy
 
 
-def _check_size(directory: Directory, warning_at=20 * 1024**3, print_size=False):
-    """
-    Checks the size of the Directory directory on instantiation and warns if it exceeds 20GiB (default).
-    """
-    if context.check_size_on_init:
-        _check_size(directory.path, warning_at, print_size)
-    return directory
-
-
 def check_size(path: Path, warning_at=20 * 1024**3, print_size=False) -> None:
+    """Prints the size of the directory at path and warns if it exceeds warning_at."""
+
     def sizeof_fmt(num, suffix="B"):
         for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
             if abs(num) < 1024.0:
                 return "%3.1f%s%s" % (num, unit, suffix)
             num /= 1024.0
         return "%.1f%s%s" % (num, "Yi", suffix)
 
@@ -1231,14 +1341,15 @@
         with warnings.catch_warnings():
             warnings.simplefilter("always")
             warnings.warn(
                 f"This directory {path.name} occupies {sizeof_fmt(size_in_bytes)} of disk space.",
                 ResourceWarning,
                 stacklevel=2,
             )
+    return size_in_bytes
 
 
 def _forward_subclass(cls: type, config: object = {}) -> object:
     # Coerce `config` to a `dict`.
     config = dict(
         config if isinstance(config, Mapping) else getattr(config, "__dict__", {})
     )
```

### Comparing `datamate-0.1.5/datamate/namespaces.py` & `datamate-0.1.6/datamate/namespaces.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 This module exports `Namespace`, a `dict` that supports accessing items at
 attributes, for convenience, and to better support static analysis.
 
 It also exports`namespacify`, a function that recursively converts mappings and
 Namespace-like containers in JSON-like objects to `Namespace`s.
 """
 
-from typing import Any, Dict, List, Mapping
+from typing import Any, Dict, List, Mapping, get_origin
 from copy import copy, deepcopy
 from numpy import ndarray
 from pathlib import Path
 
 import pandas as pd
 
-__all__ = ["Namespace", "namespacify"]
+__all__ = ["Namespace", "namespacify", "is_disjoint", "is_subset", "is_superset"]
 
 # -- Namespaces ----------------------------------------------------------------
 
 
 class Namespace(Dict[str, Any]):
     """
-    A `dict` that supports accessing items as attributes
+    A `dict` that supports accessing items as attributes and comparison methods
+    between multiple `Namespace`s.
     """
 
     def __dir__(self) -> List[str]:
         return list(set([*dict.__dir__(self), *dict.__iter__(self)]))
 
     def __getattr__(self, key: str) -> Any:
         try:
@@ -95,40 +96,44 @@
 
     def without(self, key):
         """Return a copy of the namespace without the specified key."""
         _copy = self.deepcopy()
         _copy.pop(key)
         return _copy
 
-    def is_superset(self, superset):
-        _keys_subset = set(self)
-        _keys_superset = set(superset)
-        return _keys_subset.issubset(_keys_superset)
+    def is_superset(self, other):
+        return is_subset(self, other)
 
-    def is_value_matching_superset(self, subset):
+    def is_subset(self, other):
         """
-        Args:
-            self (dict): potential superset
-            subset (dict): potential subset
+        Check whether dict2 is a subset of dict1.
 
-        Returns: True if subset is a subset of superset
-            and all values match.
+        Parameters:
+        dict1 (dict): The superset dictionary.
+        dict2 (dict): The subset dictionary.
+
+        Returns:
+        bool: True if dict2 is a subset of dict1, False otherwise.
         """
-        # namespacify for type coercion from array to list
-        self = namespacify(self)
-        subset = namespacify(subset)
-        _keys_superset = set(self)
-        _keys_subset = set(subset)
-        _keys_are_superset = _keys_superset.issuperset(_keys_subset)
-        _values_are_matching = all(
-            self[key] == subset[key]
-            for key in _keys_superset.intersection(_keys_subset)
-        )
+        return is_superset(other, self)
+
+    def is_disjoint(self, other_dict):
+        """
+        Check whether another dictionary is disjoint with respect to this one.
+
+        Two dictionaries are considered disjoint if they have no common keys.
 
-        return _keys_are_superset & _values_are_matching
+        Parameters:
+        other_dict (dict): The other dictionary to check for disjointness.
+
+        Returns:
+        bool: True if the other dictionary is disjoint with respect to this one,
+              False otherwise.
+        """
+        return is_disjoint(self, other_dict)
 
     def to_df(self, name="", seperator="."):
         """Dict to flattened dataframe."""
         as_dict = self.to_dict()  # namespace need deepcopy method
         df = pd.json_normalize(as_dict, sep=seperator).T
         if name:
             df = df.rename({0: name}, axis=1)
@@ -171,85 +176,126 @@
                     _diff2 = f"+{parent}.{k}: {v}" if parent else f"+{k}: {v}"
                     diff1.append(_diff1)
                     diff2.append(_diff2)
 
         _diff(_self, other)
         return namespacify(diff)
 
-    def walk(self, _parents=tuple()):
-        """Walks a dictionary, like os.walk(dir)."""
-        _childs = tuple()
-        _values = tuple()
-        for key, value in self.items():
-            parents = _parents + (key,)
-            childs = (
-                _childs + tuple(value.keys()) if isinstance(value, dict) else _childs
-            )
-            values = _values if isinstance(value, dict) else _values + (value,)
-            yield parents, childs, values
+    def walk(self):
+        """
+        Recursively walk through the dictionary and yield a tuple for each
+        key-value pair.
 
-            if isinstance(value, dict):
-                yield from self.walk(value, _parents=parents)
+        Yields:
+        tuple: A tuple containing the current key and its corresponding value.
+        """
+        yield from dict_walk(self)
 
     def equal_values(self, other):
         "Comparison of values, nested."
         # namespacify for type coercion from array to list
         return compare(self, other)
 
     def copy(self):
         return copy(self)
 
     def deepcopy(self):
         return deepcopy(self)
 
     def to_dict(self):
-        return to_dict(self)
+        return dict(
+            (k, to_dict(v) if isinstance(v, dict) or isinstance(v, Namespace) else v)
+            for k, v in self.items()
+        )
 
     def depth(self):
         return depth(self)
 
     def pformat(self):
         return pformat(self)
 
     def all(self):
         return all_true(self)
 
 
-def namespacify(obj: object) -> object:
+def namespacify(obj: object) -> Namespace:
     """
     Recursively convert mappings (item access only) and ad-hoc Namespaces
     (attribute access only) to `Namespace`s (both item and element access).
     """
     if isinstance(obj, (type(None), bool, int, float, str, type, bytes)):
         return obj
     elif isinstance(obj, Path):
         return str(obj)
     elif isinstance(obj, (list, tuple)):
         return [namespacify(v) for v in obj]
     elif isinstance(obj, (ndarray)):
         return [namespacify(v.item()) for v in obj]
     elif isinstance(obj, Mapping):
         return Namespace({k: namespacify(obj[k]) for k in obj})
+    elif get_origin(obj) is not None:
+        return obj
     else:
         try:
             return namespacify(vars(obj))
         except TypeError as e:
             raise TypeError(f"namespacifying {obj} of type {type(obj)}: {e}.") from e
 
 
-def to_dict(cls):
+def is_subset(dict1, dict2):
     """
-    Recursively converts a Namespace to a dictionary.
+    Check whether dict2 is a subset of dict1.
+
+    Parameters:
+    dict1 (dict): The superset dictionary.
+    dict2 (dict): The subset dictionary.
+
+    Returns:
+    bool: True if dict2 is a subset of dict1, False otherwise.
     """
-    if isinstance(cls, Namespace):
-        return {k: to_dict(v) for k, v in cls.__dict__.items()}
-    elif isinstance(cls, (list, tuple)):
-        return type(cls)(to_dict(v) for v in cls)
+    for key, value in dict2.items():
+        if key not in dict1:
+            return False
+        if isinstance(value, dict):
+            if not is_subset(dict1[key], value):
+                return False
+        else:
+            if dict1[key] != value:
+                return False
+    return True
+
+
+def is_superset(dict1, dict2):
+    """
+    Check whether dict2 is a superset of dict1.
+
+    Parameters:
+    dict1 (dict): The subset dictionary.
+    dict2 (dict): The superset dictionary.
+
+    Returns:
+    bool: True if dict2 is a superset of dict1, False otherwise.
+    """
+    return is_subset(dict2, dict1)
+
+
+def is_disjoint(dict1, dict2):
+    """Check whether two dictionaries are disjoint."""
+    dict1_keys = set(key for key, _ in dict_walk(dict1))
+    dict2_keys = set(key for key, _ in dict_walk(dict2))
+    return dict1_keys.isdisjoint(dict2_keys)
+
+
+def to_dict(obj):
+    if isinstance(obj, dict):
+        return dict((k, to_dict(v)) for k, v in obj.items())
+    elif isinstance(obj, Namespace):
+        return obj.to_dict()
     else:
-        return cls
+        return obj
 
 
 def depth(cls):
     if isinstance(cls, (dict, Namespace)):
         return 1 + (max(map(depth, cls.values())) if cls else 0)
     return 0
 
@@ -306,7 +352,24 @@
     elif isinstance(obj, Mapping):
         return all([all_true(obj[k]) for k in obj])
     else:
         try:
             return all_true(vars(obj))
         except TypeError as e:
             raise TypeError(f"all {obj} of type {type(obj)}: {e}.") from e
+
+
+def dict_walk(dictionary):
+    """
+    Recursively walk through a nested dictionary and yield a tuple
+    for each key-value pair.
+
+    Parameters:
+    dictionary (dict): The dictionary to walk through.
+
+    Yields:
+    tuple: A tuple containing the current key and its corresponding value.
+    """
+    for key, value in dictionary.items():
+        yield (key, value)
+        if isinstance(value, dict):
+            yield from dict_walk(value)
```

### Comparing `datamate-0.1.5/datamate.egg-info/PKG-INFO` & `datamate-0.1.6/datamate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.5
+Version: 0.1.6
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.5/tests/test_directory.py` & `datamate-0.1.6/tests/test_directory.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from datamate.directory import (
     ModifiedError,
     ModifiedWarning,
     ConfigWarning,
     ImplementationWarning,
     ImplementationError,
+    _auto_doc
 )
 
 # -- Helper functions ----------------------------------------------------------
 
 
 def data_file(path: Path) -> Path:
     path.parent.mkdir(parents=True, exist_ok=True)
@@ -42,14 +43,18 @@
         assert isinstance(directory, target.pop("__type__"))
     if "__path__" in target:
         assert directory.path == target.pop("__path__")
     if "__conf__" in target:
         assert directory._config == target.pop("__conf__")
     if "__meta__" in target:
         assert directory.meta == target.pop("__meta__")
+    if "__doc__" in target:
+        assert directory.__doc__ == target.pop("__doc__")
+    if "__exists__" in target:
+        assert directory.path.exists() == target.pop("__exists__")
 
     assert len(directory) == len(target)
     assert len(list(directory)) == len(target)
 
     for k, v in target.items():
         assert k in directory
         assert k in list(directory)
@@ -533,45 +538,78 @@
 def test_root_dir_provided(tmp_path, rooted_dir):
     RootedDirectory, rooted_dir_root_path = rooted_dir
 
     assert rooted_dir_root_path != tmp_path
 
     # case 1: root dir provided in decorator
     dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
-    assert dir.path.parent == rooted_dir_root_path
+    assert_directory_equals(
+            dir,
+            dict(
+                __type__=RootedDirectory,
+                __path__= rooted_dir_root_path / dir.path.name,
+                array=np.arange(0, 10, 1),
+            ),
+        )
 
     # case 2: root dir provided and not within context
     set_root_dir(tmp_path)
     dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
-    assert dir.path.parent == rooted_dir_root_path
+    assert_directory_equals(
+            dir,
+            dict(
+                __type__=RootedDirectory,
+                __path__= rooted_dir_root_path / dir.path.name,
+                array=np.arange(0, 10, 1),
+            ),
+        )
 
     # case 3: root_dir provided and within context
     with set_root_context(tmp_path):
         dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
-        assert dir.path.parent == tmp_path
+        assert_directory_equals(
+            dir,
+            dict(
+                __type__=RootedDirectory,
+                __path__= tmp_path / dir.path.name,
+                array=np.arange(0, 10, 1),
+            ),
+        )
 
 
 @root()
 class RootedDirectory(Directory):
     def __init__(self, config) -> None:
         self.array = np.arange(config.start, config.stop, config.step)
 
 
 def test_root_dir_not_provided(tmp_path):
     set_root_dir(tmp_path)
 
     # case 4: root dir not provided and not within context
     dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
-    assert dir.path.parent == tmp_path
-
+    assert_directory_equals(
+            dir,
+            dict(
+                __type__=RootedDirectory,
+                __path__= tmp_path / dir.path.name,
+                array=np.arange(0, 10, 1),
+            ),
+    )
     # case 5: root dir not provided and within context
     with set_root_context(tmp_path / "subdir"):
         dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
-        assert dir.path.parent == tmp_path / "subdir"
-
+        assert_directory_equals(
+            dir,
+            dict(
+                __type__=RootedDirectory,
+                __path__= tmp_path / "subdir" / dir.path.name,
+                array=np.arange(0, 10, 1),
+            ),
+        )
 
 # -- test default config
 
 
 class DefaultConfigDir(Directory):
     class Config:
         x: int = 2
@@ -591,134 +629,378 @@
 
 
 def test_default_config(tmp_path):
     set_root_dir(tmp_path)
 
     # from default config
     dir = DefaultConfigDir()
-    assert isinstance(dir, DefaultConfigDir)
-    assert (dir.x[()] == np.arange(2)).all()
-    assert dir.path.parent == tmp_path
-    _first = dir.path.name
-    assert "DefaultConfigDir" in _first
+    name = dir.path.name
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / name,
+            __conf__=Namespace(type="DefaultConfigDir", x=2),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 2}, "status": "done"},
+            x=np.arange(2),
+        ),
+    )
 
     # again
     dir = DefaultConfigDir()
-    assert isinstance(dir, DefaultConfigDir)
-    assert (dir.x[()] == np.arange(2)).all()
-    assert dir.path.parent == tmp_path
-    assert _first == dir.path.name
+    assert name == dir.path.name
 
     # from custom config
     dir = DefaultConfigDir(x=3)
-    assert isinstance(dir, DefaultConfigDir)
-    assert (dir.x[()] == np.arange(3)).all()
-    assert dir.path.parent == tmp_path
-    assert "DefaultConfigDir" in dir.path.name
-    assert _first != dir.path.name
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / dir.path.name,
+            __conf__=Namespace(type="DefaultConfigDir", x=3),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 3}, "status": "done"},
+            x=np.arange(3),
+        ),
+    )
+    assert name != dir.path.name
+
+    # rereference
+    dir = DefaultConfigDir(dir.path.name)
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / dir.path.name,
+            __conf__=Namespace(type="DefaultConfigDir", x=3),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 3}, "status": "done"},
+            x=np.arange(3),
+        ),
+    )
 
     # with path from default config
     dir = DefaultConfigDir(tmp_path / "test3")
-    assert isinstance(dir, DefaultConfigDir)
-    assert (dir.x[()] == np.arange(2)).all()
-    assert dir.path.parent == tmp_path
-    assert "test3" == dir.path.name
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / "test3",
+            __conf__=Namespace(type="DefaultConfigDir", x=2),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 2}, "status": "done"},
+            x=np.arange(2),
+        ),
+    )
 
     # with path and custom config
     dir = DefaultConfigDir(tmp_path / "test4", dict(x=3))
-    assert isinstance(dir, DefaultConfigDir)
-    assert (dir.x[()] == np.arange(3)).all()
-    assert dir.path.parent == tmp_path
-    assert "test4" == dir.path.name
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / "test4",
+            __conf__=Namespace(type="DefaultConfigDir", x=3),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 3}, "status": "done"},
+            x=np.arange(3),
+        ),
+    )
 
     # with name/ path from custom config but directory exists
     with pytest.raises(FileExistsError):
         dir = DefaultConfigDir(tmp_path / "test3", dict(x=3))
 
     # bad implementation warning
     with pytest.warns(ImplementationWarning):
         dir = BadImplementation()
+        assert_directory_equals(
+            dir,
+            dict(
+                __type__=BadImplementation,
+                __path__=tmp_path / dir.path.name,
+                __conf__=Namespace(type="BadImplementation"),
+                __meta__={"config": None, "status": "done"},
+            ),
+        )
 
     with pytest.warns(ImplementationWarning):
         with pytest.raises(FileNotFoundError):
             dir = BadImplementation(tmp_path / "test8")
 
     # config has no default attributes but directory has init, with custom config
     with pytest.warns(ImplementationWarning):
         dir = BadImplementation(dict(x=2))
-        assert (dir.x[()] == np.arange(2)).all()
+        assert_directory_equals(
+            dir,
+            dict(
+                __type__=BadImplementation,
+                __path__=tmp_path / dir.path.name,
+                __conf__=Namespace(type="BadImplementation", x=2),
+                __meta__={
+                    "config": {"type": "BadImplementation", "x": 2},
+                    "status": "done",
+                },
+                x=np.arange(2)
+            ),
+        )
 
     with pytest.warns(ImplementationWarning):
         dir = BadImplementation(tmp_path / "test10", dict(x=2))
-        assert (dir.x[()] == np.arange(2)).all()
+        assert_directory_equals(
+            dir,
+            dict(
+                __type__=BadImplementation,
+                __path__=tmp_path / "test10",
+                __conf__=Namespace(type="BadImplementation", x=2),
+                __meta__={
+                    "config": {"type": "BadImplementation", "x": 2},
+                    "status": "done",
+                },
+                x=np.arange(2)
+            ),
+        )
 
     # config has no default attributes but directory has init, with custom, wrong config
     with pytest.raises(AttributeError):
         with pytest.warns(ImplementationWarning):
             dir = BadImplementation(dict(y=2))
 
     with pytest.raises(AttributeError):
         with pytest.warns(ImplementationWarning):
             dir = BadImplementation(tmp_path / "test12", dict(y=2))
 
 
 # -- test auto docstring
 
-
 class AutoDocConfigDir(Directory):
     """Dir to test auto docstring based on config."""
 
     class Config:
         x: int = 2
         y: float = 2.0
         q = Namespace(a=1, b=2)
 
 
+class AutoDocInitDir(Directory):
+    "Dir to test auto docstring based on config."
+
+    def __init__(self, x: int = 2, y: float = 2.0, q=Namespace(a=1, b=2)):
+        pass
+
+
 class SoloConfigDocDir(Directory):
     class Config:
         x: int = 2
         y: float = 2.0
         q = Namespace(a=1, b=2)
 
 
+class SoloInitDocDir(Directory):
+    def __init__(self, x: int = 2, y: float = 2.0, q=Namespace(a=1, b=2)):
+        pass
+
+
 class EmptyConfigDocDir(Directory):
     """Dir to test auto docstring based on config."""
 
     class Config:
         pass
 
 
+class EmptyInitDocDir(Directory):
+    """Dir to test auto docstring based on config."""
+
+    def __init__(self):
+        pass
+
+
 class NoConfigDocDir(Directory):
     """Dir to test auto docstring based on config."""
 
     pass
 
 
 def test_auto_doc(tmp_path):
     a = AutoDocConfigDir()
+    doc = "Dir to test auto docstring based on config.{}".format(_auto_doc(a, cls_doc=False))
+    # breakpoint()
+    assert_directory_equals(
+        a,
+        dict(
+            __doc__=doc,
+            __exists__=False,
+        ),
+    )
 
-    doc = "Dir to test auto docstring based on config."
-    doc += "\n\n"
-    doc += "Initialize from config or leave default:\n"
-    doc += "{}(dict(\n{}))"
-    doc = doc.format(
-        "test_directory.AutoDocConfigDir",
-        "x: int = 2,\ny: float = 2.0,\nq = Namespace(a=1, b=2),\n",
+    a1 = AutoDocInitDir()
+    assert_directory_equals(
+        a1,
+        dict(
+            __doc__=doc.replace("AutoDocConfigDir", "AutoDocInitDir"),
+            __exists__=False,
+        ),
     )
-    assert a.__doc__ == doc
 
     b = SoloConfigDocDir()
-    doc = "Initialize from config or leave default:\n"
-    doc += "{}(dict(\n{}))"
-    doc = doc.format(
-        "test_directory.SoloConfigDocDir",
-        "x: int = 2,\ny: float = 2.0,\nq = Namespace(a=1, b=2),\n",
+    doc = _auto_doc(b, cls_doc=False)
+    assert_directory_equals(
+        b,
+        dict(
+            __doc__=doc,
+            __exists__=False,
+        ),
+    )
+
+    b1 = SoloInitDocDir()
+    assert_directory_equals(
+        b1,
+        dict(
+            __doc__=doc.replace("SoloConfigDocDir", "SoloInitDocDir"),
+            __exists__=False,
+        ),
     )
-    assert b.__doc__ == doc
 
     c = EmptyConfigDocDir()
-    doc = "Dir to test auto docstring based on config."
-    assert c.__doc__ == doc
+    doc = "Dir to test auto docstring based on config.{}".format(_auto_doc(c, cls_doc=False))
+    assert_directory_equals(
+        c,
+        dict(
+            __doc__=doc,
+            __exists__=False,
+        ),
+    )
+
+    c1 = EmptyInitDocDir()
+    assert_directory_equals(
+        c1,
+        dict(
+            __doc__=doc,
+            __exists__=False,
+        ),
+    )
 
     d = NoConfigDocDir()
-    doc = "Dir to test auto docstring based on config."
-    assert d.__doc__ == doc
+    doc = "Dir to test auto docstring based on config.{}".format(_auto_doc(d, cls_doc=False))
+    assert_directory_equals(
+        d,
+        dict(__doc__=doc, __exists__=False),
+    )
+
+
+# --- test default config and init from init kwargs
+
+
+class SmartDir(Directory):
+    def __init__(self, foo: int = 2, bar: int = 3):
+        self.foo = foo
+        self.bar = bar
+
+
+def test_init_from_kwargs(tmp_path):
+    set_root_dir(tmp_path)
+    dir = SmartDir()
+    assert_directory_equals(
+            dir,
+            dict(
+                __path__=tmp_path / dir.path.name,
+                __conf__=Namespace(type="SmartDir", foo=2, bar=3),
+                __meta__={"config": {"type": "SmartDir", "foo": 2, "bar": 3}, "status": "done"},
+                foo=2,
+                bar=3
+            ),
+    )
+
+    dir = SmartDir(foo=5, bar=1)
+    assert_directory_equals(
+            dir,
+            dict(
+                __path__=tmp_path / dir.path.name,
+                __conf__=Namespace(type="SmartDir", foo=5, bar=1),
+                __meta__={"config": {"type": "SmartDir", "foo": 5, "bar": 1}, "status": "done"},
+                foo=5,
+                bar=1
+            ),
+    )
+    name = dir.path.name
+
+    dir = SmartDir(name)
+    assert_directory_equals(
+            dir,
+            dict(
+                __path__=tmp_path / name,
+                __conf__=Namespace(type="SmartDir", foo=5, bar=1),
+                __meta__={"config": {"type": "SmartDir", "foo": 5, "bar": 1}, "status": "done"},
+                foo=5,
+                bar=1
+            ),
+    )
+
+    with pytest.raises(FileExistsError):
+        dir = SmartDir(dir.path.name, foo=3, bar=2)
+
+
+# --- test directory with Config but without init
+
+
+class NetworkDir(Directory):
+    class Config:
+        tau: float = 200.0
+        sigma: float = 0.1
+
+    def train(self):
+        del self.loss
+        for i in range(self.config.N):
+            self.extend(
+                "loss",
+                [np.exp(-i / self.config.tau) + np.random.rand() * self.config.sigma],
+            )
+
+
+def test_directory_with_config_without_init(tmp_path):
+    set_root_dir(tmp_path)
+
+    nnd = NetworkDir()
+    assert_directory_equals(
+            nnd,
+            dict(
+                __conf__=Namespace(type="NetworkDir", tau=200.0, sigma=0.1),
+                __exists__=False,
+            ),
+    )
+
+    nnd = NetworkDir(tmp_path / "test")
+    assert_directory_equals(
+            nnd,
+            dict(
+                __path__=tmp_path / "test",
+                __conf__=Namespace(type="NetworkDir", tau=200.0, sigma=0.1),
+                __exists__=False,
+            ),
+    )
+
+
+# --- test merge of defaults
+
+
+class ConIni1(Directory):
+    class Config:
+        sigma: float = 0.1
+
+    def __init__(self, tau=200):
+        pass
+
+
+def test_cross_configs(tmp_path):
+    dir = ConIni1()
+    assert_directory_equals(
+            dir,
+            dict(
+                __conf__=Namespace(type="ConIni1", tau=200.0, sigma=0.1),
+                __exists__=False,
+            ),
+    )
+
+    with pytest.raises(ValueError):
+        class ConIni2(Directory):
+            class Config:
+                tau: float = 200.0
+                sigma: float = 0.1
+
+            def __init__(self, sigma=2):
+                pass
```

### Comparing `datamate-0.1.5/tests/test_namespaces.py` & `datamate-0.1.6/tests/test_namespaces.py`

 * *Files identical despite different names*

